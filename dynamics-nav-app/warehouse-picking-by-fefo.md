---
title: Come abilitare prelievi tramite il metodo FEFO
description: "FEFO (First-Expired-First-Out) è un metodo di ordinamento che assicura che vengano prelevati per primi gli articoli meno recenti, ovvero quelli con le date di scadenza più prossime."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: d3977cd235293d685490464e51aec16a95d01e9d
ms.contentlocale: it-it
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-enable-picking-items-by-fefo"></a><span data-ttu-id="1cb7c-103">Procedura: Abilitare il prelievo di articoli tramite il metodo FEFO</span><span class="sxs-lookup"><span data-stu-id="1cb7c-103">How to: Enable Picking Items by FEFO</span></span>
<span data-ttu-id="1cb7c-104">FEFO (First-Expired-First-Out) è un metodo di ordinamento che assicura che vengano prelevati per primi gli articoli meno recenti, ovvero quelli con le date di scadenza più prossime.</span><span class="sxs-lookup"><span data-stu-id="1cb7c-104">First-Expired-First-Out (FEFO) is a sorting method that ensures that the oldest items, those with the earliest expiration dates, are picked first.</span></span>  

 <span data-ttu-id="1cb7c-105">La funzionalità può essere utilizzata solo quando vengono soddisfatti i seguenti criteri:</span><span class="sxs-lookup"><span data-stu-id="1cb7c-105">This functionality only works when the following criteria are met:</span></span>  

-   <span data-ttu-id="1cb7c-106">L'articolo deve avere un numero seriale o di lotto.</span><span class="sxs-lookup"><span data-stu-id="1cb7c-106">The item must have a serial/lot number.</span></span>  
-   <span data-ttu-id="1cb7c-107">Nel setup del codice di tracciabilità dell'articolo è necessario selezionare il campo **Tracciab. NS in warehouse** o **Tracciab. lotto in warehouse**.</span><span class="sxs-lookup"><span data-stu-id="1cb7c-107">On the item’s item tracking code setup, the **SN-Specific Warehouse Tracking** field or the **Lot-Specific Warehouse Tracking** field must be selected.</span></span>  
-   <span data-ttu-id="1cb7c-108">L'articolo deve essere registrato in magazzino con una data di scadenza.</span><span class="sxs-lookup"><span data-stu-id="1cb7c-108">The item must be posted to inventory with an expiration date.</span></span>  
-   <span data-ttu-id="1cb7c-109">Nella scheda Ubicazione, la casella di controllo **Richiesto prelievo** deve essere selezionata.</span><span class="sxs-lookup"><span data-stu-id="1cb7c-109">On the location card, the **Require Pick** check box must be selected.</span></span>  
-   <span data-ttu-id="1cb7c-110">Nella scheda ubicazione è necessario selezionare la casella di controllo **Prelievo in base a FEFO**.</span><span class="sxs-lookup"><span data-stu-id="1cb7c-110">On the location card, the **Pick According to FEFO** check box must be selected.</span></span>  
-   <span data-ttu-id="1cb7c-111">Nella scheda Ubicazione, la casella di controllo **Collocazione obbligatoria** deve essere selezionata.</span><span class="sxs-lookup"><span data-stu-id="1cb7c-111">On the location card, the **Bin Mandatory** check box must be selected.</span></span>  

 <span data-ttu-id="1cb7c-112">Una volta soddisfatti tutti i criteri, gli articoli con numeri seriali/di lotto da prelevare verranno ordinati con i più vecchi per primi in tutti gli prelievi e tutte le movimentazioni, ad eccezione degli articoli che utilizzano la tracciabilità NS specifico o lotto specifico.</span><span class="sxs-lookup"><span data-stu-id="1cb7c-112">When all the criteria are met, then serial/lot-numbered items to be picked are sorted with the oldest first in all picks and movements, except for items that use SN-specific or lot-specific tracking.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="1cb7c-113">Se alcuni articoli con numeri seriali/di lotto utilizzano la tracciabilità specifica, questi vengono rispettati per primi e quindi vengono elencati i rimanenti numeri seriali/di lotto in base al metodo FEFO.</span><span class="sxs-lookup"><span data-stu-id="1cb7c-113">If some serial/lot-numbered items use specific tracking, then those are respected first and under them, the remaining, non-specific, serial/lot numbers are listed according to FEFO.</span></span>  

 <span data-ttu-id="1cb7c-114">Se due articoli con numeri seriali o di lotto hanno la stessa data di scadenza, viene selezionato automaticamente quello con il numero di lotto o seriale inferiore.</span><span class="sxs-lookup"><span data-stu-id="1cb7c-114">If two serial/lot-numbered items have the same expiration date, then the program selects the item with the lowest serial or lot number.</span></span> <span data-ttu-id="1cb7c-115">Se i numeri di lotto o seriali sono identici, viene selezionato automaticamente l'articolo registrato per primo.</span><span class="sxs-lookup"><span data-stu-id="1cb7c-115">If the serial or lot numbers are the same, then the program selects the item that was registered first.</span></span>  

> [!NOTE]  
>  -   <span data-ttu-id="1cb7c-116">Quando si prelevano articoli con numeri di serie o di lotto in ubicazioni impostate per stoccaggi e prelievi guidati, solo le quantità nelle collocazioni di tipo *Prelievo* vengono prelevate in base al metodo FEFO.</span><span class="sxs-lookup"><span data-stu-id="1cb7c-116">When picking serial/lot-numbered items in locations set up for directed put-away and pick, only quantities on bins of type *Pick* are picked according to FEFO.</span></span>  
> -   <span data-ttu-id="1cb7c-117">Per abilitare le movimentazioni in base al metodo FEFO, nella finestra **Movimento di magazzino** o **Prospetto movimentazioni**, è necessario lasciare vuoto il campo **Dal codice collocazione**.</span><span class="sxs-lookup"><span data-stu-id="1cb7c-117">To enable movements according to FEFO, either in the **Inventory Movement** window or the **Movement Worksheet** window, you must leave the **From Bin** field empty.</span></span>  
> -   <span data-ttu-id="1cb7c-118">Se il campo **Registrazione scadenza vincolante** è selezionato, solo gli articoli che non sono scaduti verranno inclusi nel prelievo.</span><span class="sxs-lookup"><span data-stu-id="1cb7c-118">If the **Strict Expiration Posting** field is selected, then only items that are not expired will be included in the pick.</span></span> <span data-ttu-id="1cb7c-119">Ciò si applica anche se non viene utilizzata l'opzione Prelievo in base a FEFO.</span><span class="sxs-lookup"><span data-stu-id="1cb7c-119">This applies even if you are not using Pick according to FEFO.</span></span>  

## <a name="see-also"></a><span data-ttu-id="1cb7c-120">Vedi anche</span><span class="sxs-lookup"><span data-stu-id="1cb7c-120">See Also</span></span>  
<span data-ttu-id="1cb7c-121">[Prelievo di articoli](warehouse-pick-items.md) </span><span class="sxs-lookup"><span data-stu-id="1cb7c-121">[Picking Items](warehouse-pick-items.md) </span></span>  
<span data-ttu-id="1cb7c-122">[Procedura: Prelevare articoli per la spedizione warehouse](warehouse-how-to-pick-items-for-warehouse-shipment.md) </span><span class="sxs-lookup"><span data-stu-id="1cb7c-122">[How to: Pick Items for Warehouse Shipment](warehouse-how-to-pick-items-for-warehouse-shipment.md) </span></span>  
<span data-ttu-id="1cb7c-123">[Procedura: prelevare articoli con prelievi magazzino](warehouse-how-to-pick-items-with-inventory-picks.md) </span><span class="sxs-lookup"><span data-stu-id="1cb7c-123">[How to: Pick Items with Inventory Picks](warehouse-how-to-pick-items-with-inventory-picks.md) </span></span>  
[<span data-ttu-id="1cb7c-124">Dettagli di progettazione: Gestione warehouse</span><span class="sxs-lookup"><span data-stu-id="1cb7c-124">Design Details: Warehouse Management</span></span>](design-details-warehouse-management.md)  
[<span data-ttu-id="1cb7c-125">Magazzino</span><span class="sxs-lookup"><span data-stu-id="1cb7c-125">Inventory</span></span>](inventory-manage-inventory.md)  
<span data-ttu-id="1cb7c-126">[Utilizzo di [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="1cb7c-126">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
