---
title: "Dettagli di progettazione - Progettazione tracciabilità articolo"
description: "Questo argomento descrive la progettazione alla base della tracciabilità articolo in [! INCLUDA] [d365fin (includes/d365fin_md.md])."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: design, item, tracking, tracing
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: acbb706d154f164c4e33e0bebaf84cd5a47862cc
ms.contentlocale: it-it
ms.lasthandoff: 10/16/2017

---
# <a name="design-details-item-tracking-design"></a><span data-ttu-id="41013-103">Dettagli di progettazione: Progettazione tracciabilità articolo</span><span class="sxs-lookup"><span data-stu-id="41013-103">Design Details: Item Tracking Design</span></span>
<span data-ttu-id="41013-104">Nella prima versione della funzionalità di tracciabilità articolo in [!INCLUDE[d365fin](includes/d365fin_md.md)] 2.60, i numeri seriali o di lotto venivano registrati direttamente nei movimenti contabili articoli.</span><span class="sxs-lookup"><span data-stu-id="41013-104">In the first version of Item Tracking in [!INCLUDE[d365fin](includes/d365fin_md.md)] 2.60, serial numbers or lot numbers were recorded directly on item ledger entries.</span></span> <span data-ttu-id="41013-105">Questa progettazione forniva informazioni complete sulla disponibilità e sulla tracciabilità semplice dei movimenti storici, ma mancava di flessibilità e funzionalità.</span><span class="sxs-lookup"><span data-stu-id="41013-105">This design provided full availability information and simple tracking of historic entries, but it lacked flexibility and functionality.</span></span>  

<span data-ttu-id="41013-106">Da [!INCLUDE[d365fin](includes/d365fin_md.md)] 3.00, la funzione di tracciabilità articolo rientra in una struttura oggetto separata con collegamenti complessi ai documenti registrati e i movimenti contabili articoli.</span><span class="sxs-lookup"><span data-stu-id="41013-106">From [!INCLUDE[d365fin](includes/d365fin_md.md)] 3.00, item tracking functionality was in a separate object structure with intricate links to posted documents and item ledger entries.</span></span> <span data-ttu-id="41013-107">Questa progettazione era flessibile e piena di funzionalità, ma i movimenti di tracciabilità articolo non erano inclusi completamente nei calcoli della disponibilità.</span><span class="sxs-lookup"><span data-stu-id="41013-107">This design was flexible and rich in functionality, but item tracking entries were not fully involved in availability calculations.</span></span>  

<span data-ttu-id="41013-108">Da [!INCLUDE[d365fin](includes/d365fin_md.md)] 3.60 la funzione di tracciabilità articolo è integrata con il sistema di impegno, che gestisce l'impegno, la tracciabilità ordine e la messaggistica di azione.</span><span class="sxs-lookup"><span data-stu-id="41013-108">Since [!INCLUDE[d365fin](includes/d365fin_md.md)] 3.60, item tracking functionality is integrated with the reservation system, which handles reservation, order tracking, and action messaging.</span></span> <span data-ttu-id="41013-109">Per ulteriori informazioni, vedere “Dettagli di progettazione: Impegno, tracciabilità dell'ordine e messaggistica di azioni" in "Dettagli progettazione: Pianificazione degli approvvigionamenti".</span><span class="sxs-lookup"><span data-stu-id="41013-109">For more information, see “Design Details: Reservation, Order Tracking, and Action Messaging” in “Design Details: Supply Planning”.</span></span>  

<span data-ttu-id="41013-110">Quest'ultima progettazione incorpora i movimenti di tracciabilità articolo nei calcoli della disponibilità totale in tutto il sistema, inclusa la pianificazione, la produzione e il warehouse.</span><span class="sxs-lookup"><span data-stu-id="41013-110">This latest design incorporates item tracking entries in total availability calculations throughout the system, including planning, manufacturing, and warehousing.</span></span> <span data-ttu-id="41013-111">Il vecchio concetto di inserire i numeri seriali e di lotto nei movimenti contabili articoli viene reintrodotto per garantire il semplice accesso ai dati storici a scopo di tracciabilità.</span><span class="sxs-lookup"><span data-stu-id="41013-111">The old concept of carrying serial and lot numbers on the item ledger entries is reintroduced to ensure simple access to historical data for item tracking purposes.</span></span> <span data-ttu-id="41013-112">In relazione ai miglioramenti di tracciabilità articolo in [!INCLUDE[d365fin](includes/d365fin_md.md)] 3.60, il sistema di impegno è stato esteso alle entità della rete diverse dagli ordini, ad esempio le registrazioni, le fatture e le note di credito.</span><span class="sxs-lookup"><span data-stu-id="41013-112">In connection with item tracking improvements in [!INCLUDE[d365fin](includes/d365fin_md.md)] 3.60, the reservation system was expanded to non-order network entities, such as journals, invoices, and credit memos.</span></span>  

<span data-ttu-id="41013-113">Con l'aggiunta dei numeri seriali o di lotto, gli attributi permanenti dell'articolo vengono gestiti dal sistema di impegno contemporaneamente alla gestione dei collegamenti intermittenti tra approvvigionamento e domanda sotto forma di movimenti di tracciabilità ordini e di movimenti impegni.</span><span class="sxs-lookup"><span data-stu-id="41013-113">With the addition of serial or lot numbers, the reservation system handles permanent item attributes while also handling intermittent links between supply and demand in the form of order tracking entries and reservation entries.</span></span> <span data-ttu-id="41013-114">Un'altra caratteristica diversa dei numeri seriali o di lotto confrontati ai dati di impegno convenzionali è il fatto che possono essere registrati, parzialmente o completamente.</span><span class="sxs-lookup"><span data-stu-id="41013-114">Another different characteristic of serial or lot numbers compared to the conventional reservation data is the fact that they can be posted, either partially or fully.</span></span> <span data-ttu-id="41013-115">Di conseguenza, la tabella **Movimenti impegni** (T337) utilizza ora una tabella correlata denominata **Specifica tracciabilità** (T336) che gestisce e visualizza le somme delle quantità di tracciabilità articolo registrate e attive.</span><span class="sxs-lookup"><span data-stu-id="41013-115">Therefore, the **Reservation Entry** table (T337) now works with a related table, the **Tracking Specification** table (T336), which manages and displays summing across active and posted item tracking quantities.</span></span> <span data-ttu-id="41013-116">Per ulteriori informazioni, vedere [Dettagli di progettazione: Movimenti di tracciabilità articolo storici e attivi](design-details-active-versus-historic-item-tracking-entries.md).</span><span class="sxs-lookup"><span data-stu-id="41013-116">For more information, see [Design Details: Active versus Historic Item Tracking Entries](design-details-active-versus-historic-item-tracking-entries.md).</span></span>  

<span data-ttu-id="41013-117">Nel diagramma seguente viene descritta la progettazione della funzionalità di tracciabilità articolo in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="41013-117">The following diagram outlines the design of item tracking functionality in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span>  

<span data-ttu-id="41013-118">![Progettazione tracciabilità articolo](media/design_details_item_tracking_design.png "design_details_item_tracking_design")</span><span class="sxs-lookup"><span data-stu-id="41013-118">![Item tracking design](media/design_details_item_tracking_design.png "design_details_item_tracking_design")</span></span>  

<span data-ttu-id="41013-119">L'oggetto di registrazione centrale è riprogettato per gestire la sottoclassificazione univoca di una riga di documento sotto forma di numero seriale o di numeri di lotto. Speciali tabelle di relazione vengono aggiunte per creare relazioni uno a molti tra i documenti registrati e i relativi movimenti contabili articoli e movimenti contabili di valorizzazione.</span><span class="sxs-lookup"><span data-stu-id="41013-119">The central posting object is redesigned to handle the unique subclassification of a document line in the form of serial or lot numbers, and special relation tables are added to create the one-to-many relations between posted documents and their split item ledger entries and value ledger entries.</span></span>  

<span data-ttu-id="41013-120">Codeunit 22, **Reg. magazzino - registra righe**, ora suddivide la registrazione in base ai numeri di tracciabilità articolo specificati nella riga del documento.</span><span class="sxs-lookup"><span data-stu-id="41013-120">Codeunit 22, **Item Jnl. – Post Line**, now splits the posting according to the item tracking numbers that are specified on the document line.</span></span> <span data-ttu-id="41013-121">Ciascun numero di tracciabilità articolo sulla riga crea il proprio movimento contabile articolo per l'articolo.</span><span class="sxs-lookup"><span data-stu-id="41013-121">Each unique item tracking number on the line creates its own item ledger entry for the item.</span></span> <span data-ttu-id="41013-122">Ciò significa che il collegamento dalla riga del documento registrato ai movimenti contabili articoli associati è una relazione uno a molti.</span><span class="sxs-lookup"><span data-stu-id="41013-122">This means that the link from the posted document line to the associated item ledger entries is now a one-to-many relation.</span></span> <span data-ttu-id="41013-123">Tale relazione viene gestita dalle seguenti tabelle di relazione di tracciabilità articolo.</span><span class="sxs-lookup"><span data-stu-id="41013-123">This relation is handled by the following item tracking relation tables.</span></span>  

|<span data-ttu-id="41013-124">Campo</span><span class="sxs-lookup"><span data-stu-id="41013-124">Field</span></span>|<span data-ttu-id="41013-125">Description</span><span class="sxs-lookup"><span data-stu-id="41013-125">Description</span></span>|  
|---------------|---------------------------------------|  
|<span data-ttu-id="41013-126">**Relazione movimento articolo** (T6507)</span><span class="sxs-lookup"><span data-stu-id="41013-126">**Item Entry Relation** (T6507)</span></span>|<span data-ttu-id="41013-127">Correla la righe spedite o ricevute ai movimenti contabili articoli</span><span class="sxs-lookup"><span data-stu-id="41013-127">Relates shipped or received lines to item ledger entries</span></span>|  
|<span data-ttu-id="41013-128">**Relazione movimento valorizz.** (T6508)</span><span class="sxs-lookup"><span data-stu-id="41013-128">**Value Entry Relation** (T6508)</span></span>|<span data-ttu-id="41013-129">Correla le righe fatturate ai movimenti di valorizzazione</span><span class="sxs-lookup"><span data-stu-id="41013-129">Relates invoiced lines to value entries</span></span>|  

<span data-ttu-id="41013-130">Per ulteriori informazioni, vedere [Dettagli di progettazione: Struttura di registrazione di tracciabilità articolo](design-details-item-tracking-posting-structure.md).</span><span class="sxs-lookup"><span data-stu-id="41013-130">For more information, see [Design Details: Item Tracking Posting Structure](design-details-item-tracking-posting-structure.md).</span></span>  

## <a name="see-also"></a><span data-ttu-id="41013-131">Vedi anche</span><span class="sxs-lookup"><span data-stu-id="41013-131">See Also</span></span>  
[<span data-ttu-id="41013-132">Dettagli di progettazione: Tracciabilità articolo</span><span class="sxs-lookup"><span data-stu-id="41013-132">Design Details: Item Tracking</span></span>](design-details-item-tracking.md)
