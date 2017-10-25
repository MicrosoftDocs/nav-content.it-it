---
title: Come registrare l'output e i tempi di lavorazione tramite processo batch
description: "La quantità di output rappresenta la quantità finita nel WIP ( work in progress)."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 09/06/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 266c3f52dda22133acebf6052326ab57551b2ec0
ms.contentlocale: it-it
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-batch-post-output-and-run-times"></a><span data-ttu-id="b34c1-103">Procedura: Registrare l'output e i tempi di lavorazione tramite processo batch</span><span class="sxs-lookup"><span data-stu-id="b34c1-103">How to: Batch Post Output and Run Times</span></span>
<span data-ttu-id="b34c1-104">La quantità di output rappresenta la quantità finita nel WIP (work in progress).</span><span class="sxs-lookup"><span data-stu-id="b34c1-104">The output quantity represents the work progress in the form of the finished quantity.</span></span>  

> [!NOTE]
> <span data-ttu-id="b34c1-105">il magazzino viene aggiornato automaticamente solo quando si registra la quantità di output per l'ultima operazione.</span><span class="sxs-lookup"><span data-stu-id="b34c1-105">Only when you post output quantity on the last operation, the inventory is updated automatically.</span></span>  

## <a name="to-post-output-quantities-for-one-or-more-production-order-lines"></a><span data-ttu-id="b34c1-106">Per registrare quantità di output per una o più righe dell'ordine di produzione</span><span class="sxs-lookup"><span data-stu-id="b34c1-106">To post output quantities for one or more production order lines</span></span>
1. <span data-ttu-id="b34c1-107">Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **Registrazioni output**, quindi scegliere il collegamento correlato.</span><span class="sxs-lookup"><span data-stu-id="b34c1-107">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Output Journal**, and then choose the related link.</span></span>  
2. <span data-ttu-id="b34c1-108">Compilare i campi inserendo i dati relativi agli ordini di produzione e all'output.</span><span class="sxs-lookup"><span data-stu-id="b34c1-108">Fill in the fields with the production order data and the output data.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
3. <span data-ttu-id="b34c1-109">Se l'operazione è stata completata, selezionare il campo **Completato** .</span><span class="sxs-lookup"><span data-stu-id="b34c1-109">If the operation has been completed, select the **Finished** field.</span></span>  

    <span data-ttu-id="b34c1-110">Se l'ubicazione della warehouse in cui devono essere stoccati gli articoli prevede l'utilizzo di collocazioni, ma non richiede l'elaborazione degli stoccaggi,  assegnare un codice collocazione alla riga delle registrazioni per specificare dove dovranno essere immagazzinati gli articoli nella warehouse.</span><span class="sxs-lookup"><span data-stu-id="b34c1-110">If the warehouse location where the items should be put away uses bins but does not require put-away processing,  assign a bin code to the journal line to specify where the items should be placed in the warehouse.</span></span> <span data-ttu-id="b34c1-111">Per ulteriori informazioni, vedere [Procedura: Stoccare l'output produzione o l'output assemblaggio](warehouse-how-to-put-away-production-output.md).</span><span class="sxs-lookup"><span data-stu-id="b34c1-111">For more information, see [How to: Put Away Production or Assembly Output](warehouse-how-to-put-away-production-output.md).</span></span>  

4. <span data-ttu-id="b34c1-112">Per registrare le operazioni scegliere l'azione **Registra**.</span><span class="sxs-lookup"><span data-stu-id="b34c1-112">Choose the **Post** acto post the operations.</span></span> <span data-ttu-id="b34c1-113">La quantità di output verrà registrata.</span><span class="sxs-lookup"><span data-stu-id="b34c1-113">The output quantity will be posted.</span></span> <span data-ttu-id="b34c1-114">A questo punto, l'articolo è disponibile per la spedizione.</span><span class="sxs-lookup"><span data-stu-id="b34c1-114">The item is now available for shipping.</span></span>  

## <a name="to-post-run-times-for-one-or-more-production-order-lines"></a><span data-ttu-id="b34c1-115">Per registrare il tempo di lavorazione per una o più righe dell'ordine di produzione</span><span class="sxs-lookup"><span data-stu-id="b34c1-115">To post run times for one or more production order lines</span></span>
<span data-ttu-id="b34c1-116">Il tempo di lavorazione rappresenta le ore di lavoro necessarie per il WIP (work in progress).</span><span class="sxs-lookup"><span data-stu-id="b34c1-116">The run time represents work progress in the form of the necessary working time.</span></span>    

1.  <span data-ttu-id="b34c1-117">Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **Registrazioni output**, quindi scegliere il collegamento correlato.</span><span class="sxs-lookup"><span data-stu-id="b34c1-117">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Output Journal**, and then choose the related link.</span></span>  
2. <span data-ttu-id="b34c1-118">Compilare i campi inserendo i dati relativi agli ordini di produzione e all'output.</span><span class="sxs-lookup"><span data-stu-id="b34c1-118">Fill in the fields with the production order data and the output data.</span></span>  
3.  <span data-ttu-id="b34c1-119">Se l'operazione è terminata, selezionare il campo **Completato** .</span><span class="sxs-lookup"><span data-stu-id="b34c1-119">If the operation is completed, select the **Finished** field.</span></span>  
4. <span data-ttu-id="b34c1-120">Scegliere l'azione **Registra** per registrare il tempo impiegato per operazione.</span><span class="sxs-lookup"><span data-stu-id="b34c1-120">Choose the **Post** action to post the time spent per operation.</span></span> <span data-ttu-id="b34c1-121">I movimenti contabili capacità vengono aggiornati per le aree di produzione o i centri di lavoro utilizzati.</span><span class="sxs-lookup"><span data-stu-id="b34c1-121">Capacity ledger entries are updated for the used work or machine centers.</span></span>

## <a name="see-also"></a><span data-ttu-id="b34c1-122">Vedi anche</span><span class="sxs-lookup"><span data-stu-id="b34c1-122">See Also</span></span>  
<span data-ttu-id="b34c1-123">[Manufacturing](production-manage-manufacturing.md)  </span><span class="sxs-lookup"><span data-stu-id="b34c1-123">[Manufacturing](production-manage-manufacturing.md)  </span></span>  
[<span data-ttu-id="b34c1-124">Impostazione della produzione</span><span class="sxs-lookup"><span data-stu-id="b34c1-124">Setting Up Manufacturing</span></span>](production-configure-production-processes.md)  
<span data-ttu-id="b34c1-125">[Pianif.](production-planning.md)    </span><span class="sxs-lookup"><span data-stu-id="b34c1-125">[Planning](production-planning.md)    </span></span>  
[<span data-ttu-id="b34c1-126">Magazzino</span><span class="sxs-lookup"><span data-stu-id="b34c1-126">Inventory</span></span>](inventory-manage-inventory.md)  
[<span data-ttu-id="b34c1-127">Acquisti</span><span class="sxs-lookup"><span data-stu-id="b34c1-127">Purchasing</span></span>](purchasing-manage-purchasing.md)  
<span data-ttu-id="b34c1-128">[Utilizzo di [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="b34c1-128">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

