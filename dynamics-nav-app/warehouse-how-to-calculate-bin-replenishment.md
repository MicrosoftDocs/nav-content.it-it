---
title: Come calcolare il rifornimento della collocazione
description: "Quando l'ubicazione è impostata per l'utilizzo di stoccaggi e prelievi guidati, per effettuare lo stoccaggio dei carichi vengono prese in considerazione le priorità del modello di stoccaggio per l'ubicazione."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/23/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 3a6ff833aad54cf98720857a8ae67492abe9af4f
ms.contentlocale: it-it
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-calculate-bin-replenishment"></a><span data-ttu-id="2870c-103">Procedura: Calcolare il rifornimento della collocazione</span><span class="sxs-lookup"><span data-stu-id="2870c-103">How to: Calculate Bin Replenishment</span></span>
<span data-ttu-id="2870c-104">Quando l'ubicazione è impostata per l'utilizzo di stoccaggi e prelievi guidati, per effettuare lo stoccaggio dei carichi vengono prese in considerazione le priorità del modello di stoccaggio per l'ubicazione.</span><span class="sxs-lookup"><span data-stu-id="2870c-104">When the location is set up to use directed put-away and pick, priorities of the put-away template for the location are taken into account when putting receipts away.</span></span> <span data-ttu-id="2870c-105">Le priorità includono le quantità minima e massima di contenuto collocazione fissate per una collocazione specifica e le valutazioni delle collocazioni.</span><span class="sxs-lookup"><span data-stu-id="2870c-105">Priorities include the minimum and maximum quantities of bin content that have been fixed for a particular bin, and the bin rankings.</span></span> <span data-ttu-id="2870c-106">Pertanto, se gli articoli giungono in magazzino a intervalli regolari, le collocazioni di prelievo più utilizzate vengono riempite non appena vengono svuotate.</span><span class="sxs-lookup"><span data-stu-id="2870c-106">Therefore, if items are arriving at a steady pace, the most-used pick bins will be filled up as they are emptied.</span></span>  

<span data-ttu-id="2870c-107">Tuttavia, non sempre la frequenza di arrivo degli articoli in magazzino è costante.</span><span class="sxs-lookup"><span data-stu-id="2870c-107">But inventory does not always arrive in a steady trickle.</span></span> <span data-ttu-id="2870c-108">Talvolta la società acquista grandi quantitativi di articoli in modo da ottenere una riduzione sul prezzo oppure l'unità di produzione può attendere che venga terminato un intero lotto di un singolo articolo in modo da ridurre il costo unitario.</span><span class="sxs-lookup"><span data-stu-id="2870c-108">Sometimes, items are purchased in large quantities so that the company can obtain a rebate, or your production unit might produce a lot of one item to achieve a low unit cost.</span></span> <span data-ttu-id="2870c-109">In tal caso, l'arrivo degli articoli nella warehouse si interromperà per un certo periodo e si renderà necessario spostare periodicamente gli articoli dalle aree di immagazzinamento a massa alle collocazioni di prelievo.</span><span class="sxs-lookup"><span data-stu-id="2870c-109">Then items will not be received in the warehouse again for some time, and the warehouse needs to periodically move items to pick bins from bulk storage areas.</span></span>  

<span data-ttu-id="2870c-110">È inoltre possibile che sia previsto l'arrivo di una nuova partita di merce a breve termine e si desideri svuotare l'area di immagazzinamento a massa prima che gli articoli giungano nella warehouse.</span><span class="sxs-lookup"><span data-stu-id="2870c-110">It could also be that the warehouse is expecting new stock to arrive soon and wants to empty the bulk storage area of items before the new merchandise arrives.</span></span>  

<span data-ttu-id="2870c-111">Infine, se per le collocazioni di immagazzinamento a massa è stato impostato un tipo di collocazione a cui è associata la sola azione **Stoccaggio**, ovvero per il tipo di collocazione non è stata selezionata l'azione **Prelievo**, sarà necessario rifornire continuamente le collocazioni di prelievo poiché non vengono forniti suggerimenti circa le collocazioni di tipo stoccaggio per un prelievo delle quantità in giacenza.</span><span class="sxs-lookup"><span data-stu-id="2870c-111">Finally, if you have defined your bulk storage bins with a bin type action **Put Away** only, that is, the bin type does not have the **Pick** action selected, you must always keep your pick bins replenished, since Put Away-type bins are not suggested for a pick of inventory.</span></span>  

## <a name="to-replenish-pick-bins"></a><span data-ttu-id="2870c-112">Per rifornire le collocazioni di prelievo</span><span class="sxs-lookup"><span data-stu-id="2870c-112">To replenish pick bins</span></span>  
1.  <span data-ttu-id="2870c-113">Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "Cerca pagina o report"), immettere **Movimento worksheet**, quindi scegliere il collegamento correlato.</span><span class="sxs-lookup"><span data-stu-id="2870c-113">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Movement Worksheet**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="2870c-114">Scegliere l'azione **Calcola rifornimento collocazione** per aprire la pagina di richiesta report.</span><span class="sxs-lookup"><span data-stu-id="2870c-114">Choose the **Calculate Bin Replenishment** action to open the report request page.</span></span>  
3.  <span data-ttu-id="2870c-115">Compilare i campi della finestra di richiesta del processo batch in modo da circoscrivere l'ambito dei suggerimenti calcolati relativi al rifornimento.</span><span class="sxs-lookup"><span data-stu-id="2870c-115">Fill in the batch job request window to limit the scope of the replenishment suggestions that will be calculated.</span></span> <span data-ttu-id="2870c-116">È ad esempio possibile che si sia interessati solo a specifici articoli, zone o collocazioni.</span><span class="sxs-lookup"><span data-stu-id="2870c-116">For example, you might be concerned with particular items, zones, or bins.</span></span>  
4.  <span data-ttu-id="2870c-117">Scegliere il pulsante **OK**.</span><span class="sxs-lookup"><span data-stu-id="2870c-117">Choose the **OK** button.</span></span> <span data-ttu-id="2870c-118">Le righe vengono create per i movimenti di rifornimento da eseguire in base alle regole impostate per le collocazioni e il relativo contenuto, ovvero articoli nelle collocazioni.</span><span class="sxs-lookup"><span data-stu-id="2870c-118">Lines are created for the replenishment movements that need to be performed according to the rules that have been set up for the bins and bin contents, that is, items in bins.</span></span>  
5.  <span data-ttu-id="2870c-119">Se si desidera effettuare tutti i rifornimenti suggeriti, scegliere l'azione **Crea movimento**.</span><span class="sxs-lookup"><span data-stu-id="2870c-119">If you want to perform all the suggested replenishments, choose the **Create Movement** action.</span></span> <span data-ttu-id="2870c-120">A questo punto, gli impiegati potranno visualizzare le istruzioni utilizzando la voce di menu **Movimentazioni**, eseguirle e registrarle.</span><span class="sxs-lookup"><span data-stu-id="2870c-120">Employees can now find instructions in the **Movements** menu item, carry them out and register them.</span></span>  
6.  <span data-ttu-id="2870c-121">Se si desidera che vengano eseguiti solo alcuni suggerimenti, eliminare le righe meno importanti e creare un movimento.</span><span class="sxs-lookup"><span data-stu-id="2870c-121">If you only want some of the suggestions to be performed, delete the lines that are less important and then create a movement.</span></span>  

<span data-ttu-id="2870c-122">Al successivo calcolo per il rifornimento delle collocazioni, i suggerimenti precedentemente eliminati verranno ricreati, qualora risultino ancora validi.</span><span class="sxs-lookup"><span data-stu-id="2870c-122">The next time you calculate bin replenishment, the suggestions that you have deleted will be recreated, if they are still valid at that time.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="2870c-123">Se per l'articolo vengono soddisfatte le seguenti condizioni:</span><span class="sxs-lookup"><span data-stu-id="2870c-123">If the following conditions are met for an item:</span></span>  
>   
>  -   <span data-ttu-id="2870c-124">L'articolo ha una data di scadenza</span><span class="sxs-lookup"><span data-stu-id="2870c-124">The item has an expiration date, and</span></span>  
> -   <span data-ttu-id="2870c-125">Il campo **Prelievo in base a FEFO** della scheda ubicazione viene selezionato</span><span class="sxs-lookup"><span data-stu-id="2870c-125">The **Pick According to FEFO** field on the location card is selected, and</span></span>  
> -   <span data-ttu-id="2870c-126">Viene utilizzata la funzionalità **Calcola rifornimento collocazione**</span><span class="sxs-lookup"><span data-stu-id="2870c-126">You use the **Calculate Bin Replenishment** functionality</span></span>  
>   
>  <span data-ttu-id="2870c-127">I campi **Dal codice zona** e **Dal codice collocazione** non saranno specificati, in quanto l'algoritmo per calcolare la posizione in cui spostare gli articoli viene attivato solo quando si utilizza la funzione **Crea movimento**.</span><span class="sxs-lookup"><span data-stu-id="2870c-127">then the **From Zone** and **From Bin** fields will be blank because the algorithm to calculate from where to move the items is triggered only when you activate the **Create Movement** function.</span></span>  

## <a name="see-also"></a><span data-ttu-id="2870c-128">Vedi anche</span><span class="sxs-lookup"><span data-stu-id="2870c-128">See Also</span></span>  
[<span data-ttu-id="2870c-129">Gestione warehouse</span><span class="sxs-lookup"><span data-stu-id="2870c-129">Warehouse Management</span></span>](warehouse-manage-warehouse.md)  
[<span data-ttu-id="2870c-130">Prelievo in base al metodo FEFO</span><span class="sxs-lookup"><span data-stu-id="2870c-130">Picking by FEFO</span></span>](warehouse-picking-by-fefo.md)  
[<span data-ttu-id="2870c-131">Magazzino</span><span class="sxs-lookup"><span data-stu-id="2870c-131">Inventory</span></span>](inventory-manage-inventory.md)  
<span data-ttu-id="2870c-132">[Impostazione gestione warehouse](warehouse-setup-warehouse.md)   </span><span class="sxs-lookup"><span data-stu-id="2870c-132">[Setting Up Warehouse Management](warehouse-setup-warehouse.md)   </span></span>  
<span data-ttu-id="2870c-133">[Gestione assemblaggio](assembly-assemble-items.md)  </span><span class="sxs-lookup"><span data-stu-id="2870c-133">[Assembly Management](assembly-assemble-items.md)  </span></span>  
[<span data-ttu-id="2870c-134">Dettagli di progettazione: Gestione warehouse</span><span class="sxs-lookup"><span data-stu-id="2870c-134">Design Details: Warehouse Management</span></span>](design-details-warehouse-management.md)  
<span data-ttu-id="2870c-135">[Utilizzo di [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="2870c-135">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
