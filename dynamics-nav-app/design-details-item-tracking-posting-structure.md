---
title: "Dettagli di progettazione - Struttura di registrazione di tracciabilità articolo"
description: "Informazioni su come utilizzare i movimenti contabili articoli come vettori principali dei numeri di tracciabilità articolo."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: design, item tracking, posting, inventory
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: f31c9da412b4411cc8b104e59d1255456d096794
ms.contentlocale: it-it
ms.lasthandoff: 10/16/2017

---
# <a name="design-details-item-tracking-posting-structure"></a><span data-ttu-id="34193-103">Dettagli di progettazione: Struttura di registrazione di tracciabilità articolo</span><span class="sxs-lookup"><span data-stu-id="34193-103">Design Details: Item Tracking Posting Structure</span></span>
<span data-ttu-id="34193-104">Per conformità con la funzionalità di costing di magazzino e per ottenere una soluzione più semplice e più affidabile, i movimenti contabili articoli vengono utilizzati come principali vettori dei numeri di tracciabilità articolo.</span><span class="sxs-lookup"><span data-stu-id="34193-104">To align with inventory costing functionality and to obtain a simpler and more robust solution, item ledger entries are used as the primary carrier of item tracking numbers.</span></span>  
  
<span data-ttu-id="34193-105">I numeri di tracciabilità articolo nelle entità di rete di ordini e nelle entità di rete diverse dagli ordini sono specificati nella tabella **Movimenti impegni** (T337).</span><span class="sxs-lookup"><span data-stu-id="34193-105">Item tracking numbers on order network entities and non-order network entities are specified in the **Reservation Entry** table (T337).</span></span> <span data-ttu-id="34193-106">I numeri di tracciabilità articolo correlati a informazioni dello storico vengono recuperati direttamente dai movimenti contabili articoli correlati alla transazione in questione.</span><span class="sxs-lookup"><span data-stu-id="34193-106">Item tracking numbers that are related to historical information are retrieved directly from the item ledger entries that are related to the transaction in question.</span></span> <span data-ttu-id="34193-107">Ciò significa che i movimenti contabili articoli riflettono la specifica di tracciabilità articolo della riga dell'ordine registrato.</span><span class="sxs-lookup"><span data-stu-id="34193-107">This means that item ledger entries reflect the item tracking specification of the posted order line.</span></span>  
  
<span data-ttu-id="34193-108">La finestra **Righe tracciabilità articolo** recupera le informazioni da T337 e dai movimenti contabili articoli e le mostra attraverso la tabella temporale denominata **Specifica tracciabilità** (T336).</span><span class="sxs-lookup"><span data-stu-id="34193-108">The **Item Tracking Lines** window retrieves the information from T337 and the item ledger entries and shows it through the temporary table, **Tracking Specification** (T336).</span></span> <span data-ttu-id="34193-109">La tabella T336 contiene anche i dati temporanei nella finestra **Righe tracciabilità articolo** per le quantità di tracciabilità articolo che restano da fatturare.</span><span class="sxs-lookup"><span data-stu-id="34193-109">T336 also hold the temporary data in the **Item Tracking Lines window** for item tracking quantities that remain to be invoiced.</span></span>  
  
## <a name="one-to-many-relation"></a><span data-ttu-id="34193-110">Relazione uno-a-molti</span><span class="sxs-lookup"><span data-stu-id="34193-110">One-to-Many Relation</span></span>  
<span data-ttu-id="34193-111">La tabella **Relazione movimento articolo**, che viene utilizzata per collegare una riga di documento registrata con i relativi movimenti contabili articolo, è costituita da due parti principali:</span><span class="sxs-lookup"><span data-stu-id="34193-111">The **Item Entry Relation** table, which is used to link a posted document line with its related item ledger entries, consists of two main parts:</span></span>  
  
* <span data-ttu-id="34193-112">Un puntatore alla riga di documento registrata, il campo **Nr. riga ordine**.</span><span class="sxs-lookup"><span data-stu-id="34193-112">A pointer to the posted document line, the **Order Line No.**</span></span> <span data-ttu-id="34193-113">.</span><span class="sxs-lookup"><span data-stu-id="34193-113">field.</span></span>  
* <span data-ttu-id="34193-114">Un numero di movimento che punta a un movimento contabile articolo, il campo **Nr. movimento articolo**.</span><span class="sxs-lookup"><span data-stu-id="34193-114">An entry number pointing to an item ledger entry, the **Item Entry No.** field.</span></span>  
  
<span data-ttu-id="34193-115">La funzionalità del campo **Nr. movimento**, che collega un movimento contabile articolo a una riga di documento registrato, gestisce la tipica relazione uno a uno quando non sono presenti numeri di tracciabilità articolo nella riga del documento registrato.</span><span class="sxs-lookup"><span data-stu-id="34193-115">The functionality of the existing **Entry No.** field, which relates an item ledger entry to a posted document line, handles the typical one-to-one relation when no item tracking numbers exist on the posted document line.</span></span> <span data-ttu-id="34193-116">Se sono presenti dei numeri di tracciabilità articolo, il campo **Nr. movimento** viene lasciato vuoto e la relazione uno a molti viene gestita dalla tabella **Relazione movimento articolo**.</span><span class="sxs-lookup"><span data-stu-id="34193-116">If item tracking numbers exist, then the **Entry No.** field is left blank, and the one-to-many relation is handled by the **Item Entry Relation** table.</span></span> <span data-ttu-id="34193-117">Se la riga del documento registrata contiene numeri di tracciabilità articolo ma si riferisce solo a un singolo movimento contabile articolo, il campo **Nr. movimento** gestisce la relazione e nella tabella **Relazione movimento articolo** non viene creato alcun record.</span><span class="sxs-lookup"><span data-stu-id="34193-117">If the posted document line carries item tracking numbers but only relates to a single item ledger entry, then the **Entry No.** field handles the relation, and the no record is created in the **Item Entry Relation** table.</span></span>  
  
## <a name="codeunits-80-and-90"></a><span data-ttu-id="34193-118">Codeunit 80 e 90</span><span class="sxs-lookup"><span data-stu-id="34193-118">Codeunits 80 and 90</span></span>  
<span data-ttu-id="34193-119">Per suddividere i movimenti contabili articoli durante la registrazione, il codice nella codeunit 80 e nella codeunit 90 è circondato di cicli che vengono eseguiti attraverso variabili di record temporanee globali.</span><span class="sxs-lookup"><span data-stu-id="34193-119">To split the item ledger entries during posting, the code in codeunit 80 and codeunit 90, is encircled by loops that run through global temporary record variables.</span></span> <span data-ttu-id="34193-120">Questo codice chiama la codeunit 22 con una riga di registrazioni magazzino.</span><span class="sxs-lookup"><span data-stu-id="34193-120">This code calls codeunit 22 with an item journal line.</span></span> <span data-ttu-id="34193-121">Queste variabili vengono inizializzate quando sono presenti numeri di tracciabilità articolo per la riga del documento.</span><span class="sxs-lookup"><span data-stu-id="34193-121">These variables are initialized when item tracking numbers exist for the document line.</span></span> <span data-ttu-id="34193-122">Per mantenere il codice semplice, viene sempre utilizzata questa struttura ciclica.</span><span class="sxs-lookup"><span data-stu-id="34193-122">To keep the code simple, this looping structure is always used.</span></span> <span data-ttu-id="34193-123">Se non sono presenti numeri di tracciabilità articolo per la riga del documento, verrà inserito un unico record e il ciclo verrà eseguito solo una volta.</span><span class="sxs-lookup"><span data-stu-id="34193-123">If no item tracking numbers exist for the document line, then a single record is inserted, and the loop runs only once.</span></span>  
  
## <a name="posting-the-item-journal"></a><span data-ttu-id="34193-124">Contabilizzazione della registrazione magazzino</span><span class="sxs-lookup"><span data-stu-id="34193-124">Posting the Item Journal</span></span>  
<span data-ttu-id="34193-125">I numeri di tracciabilità articolo vengono trasferiti tramite i movimenti impegni che sono correlati al movimento contabile articolo e il loop attraverso i numeri di tracciabilità articolo si verifica nella codeunit 22.</span><span class="sxs-lookup"><span data-stu-id="34193-125">Item tracking numbers are transferred via the reservation entries that relate to the item ledger entry, and the looping through item tracking numbers occurs in codeunit 22.</span></span> <span data-ttu-id="34193-126">Questo concetto funziona in modo analogo sia quando una riga di registrazioni magazzino viene utilizzata indirettamente per registrare una vendita o un ordine di acquisto sia quando una riga di registrazioni magazzino viene utilizzata direttamente.</span><span class="sxs-lookup"><span data-stu-id="34193-126">This concept works in the same way when an item journal line is used indirectly to post a sale or purchase order as when an item journal line is used directly.</span></span> <span data-ttu-id="34193-127">Quando le registrazioni magazzino vengono utilizzate direttamente, il campo **ID riga origine** punta alla riga di registrazione magazzino stessa.</span><span class="sxs-lookup"><span data-stu-id="34193-127">When the item journal is used directly, the **Source Row ID** field points to the item journal line itself.</span></span>  
  
## <a name="code-unit-22"></a><span data-ttu-id="34193-128">Codeunit 22</span><span class="sxs-lookup"><span data-stu-id="34193-128">Code Unit 22</span></span>  
<span data-ttu-id="34193-129">Le Codeunit 80 e 90 eseguono il ciclo della chiamata della codeunit 22 durante la registrazione della fattura dei numeri di tracciabilità articolo e durante la fatturazione delle spedizioni esistenti o dei carichi.</span><span class="sxs-lookup"><span data-stu-id="34193-129">Codeunits 80 and 90 loop the call of codeunit 22 during the invoice posting of item tracking numbers and during the invoicing of existing shipments or receipts.</span></span>  
  
<span data-ttu-id="34193-130">Durante la registrazione della quantità dei numeri di tracciabilità articolo, la codeunit 22 richiama i numeri di tracciabilità articolo dai movimenti in T337 correlati alla registrazione.</span><span class="sxs-lookup"><span data-stu-id="34193-130">During quantity posting of item tracking numbers, codeunit 22 retrieves item tracking numbers from the entries in T337 that relate to the posting.</span></span> <span data-ttu-id="34193-131">Questi movimenti vengono inseriti direttamente nella riga registrazioni magazzino.</span><span class="sxs-lookup"><span data-stu-id="34193-131">These entries are placed directly on the item journal line.</span></span>  
  
<span data-ttu-id="34193-132">La Codeunit 22 esegue il ciclo tramite i numeri di tracciabilità articolo e suddivide la registrazione in rispettivi movimenti articolo collegati contabili che includono i numeri di tracciabilità articolo.</span><span class="sxs-lookup"><span data-stu-id="34193-132">Codeunit 22 loops through the item tracking numbers and splits the posting into the respective item ledger entries that carry the item tracking numbers.</span></span> <span data-ttu-id="34193-133">Le informazioni sui movimenti contabili articoli che vengono creati vengono restituite a T337 utilizzando un record temporaneo T336, richiamato da una routine nella codeunit 22.</span><span class="sxs-lookup"><span data-stu-id="34193-133">Information about which item ledger entries are created is returned to T337 by using a temporary T336 record, which is called by a procedure in codeunit 22.</span></span> <span data-ttu-id="34193-134">Questa procedura viene avviata al termine dell'esecuzione della codeunit 22 perché, a quel punto, l'oggetto della codeunit 22 contiene le informazioni.</span><span class="sxs-lookup"><span data-stu-id="34193-134">This procedure is triggered when codeunit 22 has finished its run because at that point, the codeunit 22 object contains the information.</span></span> <span data-ttu-id="34193-135">Quando il record temporaneo T336 viene recuperato, le codeunit 80 e 90 creano dei record nella tabella **Relazione movimento articolo** per collegare i movimenti contabili articoli alla riga di spedizione o di carico creata.</span><span class="sxs-lookup"><span data-stu-id="34193-135">When the temporary T336 record is retrieved, codeunits 80 and 90 create records in the **Item Entry Relation** table to link the created item ledger entries to the created shipment or receipt line.</span></span> <span data-ttu-id="34193-136">Le Codeunit 80 o la codeunit 90 converte quindi i record temporanei T336 in record effettivi T336 collegati alla riga in questione.</span><span class="sxs-lookup"><span data-stu-id="34193-136">Codeunits 80 or codeunit 90 then converts the temporary T336 records to real T336 records that are related to the line in question.</span></span> <span data-ttu-id="34193-137">Tuttavia, questa conversione si verifica solo se la riga del documento registrata non viene eliminata, perché è registrata solo in parte.</span><span class="sxs-lookup"><span data-stu-id="34193-137">However, this conversion occurs only if the posted document line is not deleted, because it is only partially posted.</span></span>  
  
## <a name="see-also"></a><span data-ttu-id="34193-138">Vedi anche</span><span class="sxs-lookup"><span data-stu-id="34193-138">See Also</span></span>  
<span data-ttu-id="34193-139">[Dettagli di progettazione: Tracciabilità articolo](design-details-item-tracking.md) </span><span class="sxs-lookup"><span data-stu-id="34193-139">[Design Details: Item Tracking](design-details-item-tracking.md) </span></span>  
[<span data-ttu-id="34193-140">Dettagli di progettazione: Progettazione tracciabilità articolo</span><span class="sxs-lookup"><span data-stu-id="34193-140">Design Details: Item Tracking Design</span></span>](design-details-item-tracking-design.md)