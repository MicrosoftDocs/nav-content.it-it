---
title: Come convertire le ubicazioni esistenti in ubicazione warehouse
description: "È possibile consentire l'utilizzo di zone e collocazioni in un'ubicazione magazzino esistente, in modo da utilizzare tale ubicazione come ubicazione warehouse."
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
ms.openlocfilehash: 16f1d8ac06c39361ee00e8c7514a282ad4d709e5
ms.contentlocale: it-it
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-convert-existing-locations-to-warehouse-locations"></a><span data-ttu-id="e899f-103">Procedura: Convertire le ubicazioni esistenti in ubicazione warehouse</span><span class="sxs-lookup"><span data-stu-id="e899f-103">How to: Convert Existing Locations to Warehouse Locations</span></span>
<span data-ttu-id="e899f-104">È possibile consentire l'utilizzo di zone e collocazioni in un'ubicazione magazzino esistente, in modo da utilizzare tale ubicazione come ubicazione warehouse.</span><span class="sxs-lookup"><span data-stu-id="e899f-104">You can enable an existing inventory location to use zones and bins and to operate as a warehouse location.</span></span>  

<span data-ttu-id="e899f-105">Il processo batch per l'abilitazione di un'ubicazione per le attività warehouse comporta la creazione di movimenti warehouse iniziali per la collocazione di rettifica della warehouse per tutti gli articoli in magazzino nell'ubicazione.</span><span class="sxs-lookup"><span data-stu-id="e899f-105">The batch job to enable a location for warehouse operation creates initial warehouse entries for the warehouse adjustment bin for all items that have inventory in the location.</span></span> <span data-ttu-id="e899f-106">Tali movimenti iniziali verranno convertiti quando i movimenti di inventario fisico della warehouse vengono immessi dopo l'esecuzione del processo batch.</span><span class="sxs-lookup"><span data-stu-id="e899f-106">These initial entries will be balanced when warehouse physical inventory entries are entered after the batch job is run.</span></span>  

<span data-ttu-id="e899f-107">È possibile creare zone e collocazioni prima o dopo la conversione.</span><span class="sxs-lookup"><span data-stu-id="e899f-107">You can create zones and bins either before or after the conversion.</span></span> <span data-ttu-id="e899f-108">L'unica collocazione da creare prima della conversione è quella da utilizzare come collocazione di rettifica futura.</span><span class="sxs-lookup"><span data-stu-id="e899f-108">The only bin that you must create before the conversion is the one that is to be used as the future adjustment bin.</span></span>  

> [!IMPORTANT]  
>  <span data-ttu-id="e899f-109">Per eliminare tutte le giacenze negative ed eventuali documenti warehouse aperti prima di convertire l'ubicazione per la gestione warehouse, eseguire un report per identificare gli articoli con giacenza negativa e documenti warehouse aperti per l'ubicazione specificata.</span><span class="sxs-lookup"><span data-stu-id="e899f-109">To clear all negative inventory and any open warehouse documents before you convert the location for warehouse handling, run a report to identify the items with negative inventory and open warehouse documents for the location.</span></span> <span data-ttu-id="e899f-110">Per ulteriori informazioni, vedere Verifica giacenze negative.</span><span class="sxs-lookup"><span data-stu-id="e899f-110">For more information, see Check on Negative Inventory.</span></span>  

## <a name="to-enable-an-existing-location-to-operate-as-a-warehouse-location"></a><span data-ttu-id="e899f-111">Per abilitare un'ubicazione esistente come ubicazione di warehouse</span><span class="sxs-lookup"><span data-stu-id="e899f-111">To enable an existing location to operate as a warehouse location</span></span>  
1.  <span data-ttu-id="e899f-112">Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "Cerca pagina o report"), immettere **Crea ubicazione warehouse**, quindi scegliere il collegamento correlato.</span><span class="sxs-lookup"><span data-stu-id="e899f-112">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Create Warehouse Location**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="e899f-113">Nel campo **Cod. ubicazione** specificare l'ubicazione che si desidera abilitare per l'elaborazione warehouse.</span><span class="sxs-lookup"><span data-stu-id="e899f-113">In the **Location Code** field, specify the location that you want to enable for warehouse processing.</span></span>  
3.  <span data-ttu-id="e899f-114">Nel campo **Codice collocazione rettifica** specificare la collocazione nell'ubicazione in cui sono archiviati i movimenti warehouse non sincronizzati.</span><span class="sxs-lookup"><span data-stu-id="e899f-114">In the **Adjustment Bin Code** field, specify the bin at the location where unsynchronized warehouse entries are stored.</span></span> <span data-ttu-id="e899f-115">Per ulteriori informazioni, vedere la sezione "Per sincronizzare i movimenti warehouse rettificati con i movimenti contabili articoli correlati in [Procedura: Conteggio, rettifica e riclassificazione dell'inventario](inventory-how-count-adjust-reclassify.md).</span><span class="sxs-lookup"><span data-stu-id="e899f-115">For more information, see the "To synchronize the adjusted warehouse entries with the related item ledger entries" section in [How to: Count, Adjust, and Reclassify Inventory](inventory-how-count-adjust-reclassify.md).</span></span>  

    <span data-ttu-id="e899f-116">Utilizzando i movimenti contabili articoli aperti per l'ubicazione specificata, vengono create righe di registrazione warehouse, in cui vengono riassunte tutte le combinazioni di Nr. Articolo, Cod. Variante, Cod. Unità di Misura e, se necessario, Nr. Lotto e Nr. Seriale nei movimenti contabili articoli.</span><span class="sxs-lookup"><span data-stu-id="e899f-116">Using the open item ledger entries for the specified location, warehouse journal lines are created that sum up every combination of Item No., Variant Code, Unit of Measure Code, and, if necessary, Lot No. and Serial No. in the item ledger entries.</span></span> <span data-ttu-id="e899f-117">Le righe di registrazione warehouse vengono quindi registrate,</span><span class="sxs-lookup"><span data-stu-id="e899f-117">The warehouse journal lines are then posted.</span></span> <span data-ttu-id="e899f-118">in modo da creare movimenti warehouse che consentano di inserire il magazzino nella collocazione di rettifica della warehouse.</span><span class="sxs-lookup"><span data-stu-id="e899f-118">This posting creates warehouse entries that place the inventory in the warehouse adjustment bin.</span></span> <span data-ttu-id="e899f-119">Viene inoltre impostata l'opzione **Codice collocazione rettifica** nella scheda Ubicazione.</span><span class="sxs-lookup"><span data-stu-id="e899f-119">The **Adjustment Bin Code** on the location card is also set.</span></span>  

4.  <span data-ttu-id="e899f-120">Per visualizzare gli articoli aggiunti alla collocazione di rettifica durante il processo batch, è possibile eseguire il report **Collocazione rettifica warehouse**.</span><span class="sxs-lookup"><span data-stu-id="e899f-120">To see which items were added to the adjustment bin during the batch job, run the **Warehouse Adjustment Bin** report.</span></span>  
5.  <span data-ttu-id="e899f-121">Al termine del processo batch **Crea ubicazione warehouse**, eseguire e registrare un inventario fisico della warehouse.</span><span class="sxs-lookup"><span data-stu-id="e899f-121">When the **Create Warehouse Location** batch job has completed, perform and post a warehouse physical inventory.</span></span> <span data-ttu-id="e899f-122">Per ulteriori informazioni, vedere [Procedura: Conteggio, rettifica e riclassificazione dell'inventario](inventory-how-count-adjust-reclassify.md).</span><span class="sxs-lookup"><span data-stu-id="e899f-122">For more information, see [How to: Count, Adjust, and Reclassify Inventory](inventory-how-count-adjust-reclassify.md).</span></span>  

> [!NOTE]  
>  <span data-ttu-id="e899f-123">È consigliabile eseguire il processo batch **Crea ubicazione warehouse** in un orario che non ostacoli il funzionamento quotidiano del sistema.</span><span class="sxs-lookup"><span data-stu-id="e899f-123">It is recommended that you run the **Create Warehouse Location** batch job at a time when it will not impact the daily work in the system.</span></span> <span data-ttu-id="e899f-124">Durante il processo vengono elaborati tutti i movimenti disponibili nella tabella **Mov. contabili articoli**. Se il numero di movimenti è elevato, tale operazione potrebbe richiedere alcune ore.</span><span class="sxs-lookup"><span data-stu-id="e899f-124">This job processes each entry in the **Item Ledger Entry** table, and if there are a large number of item ledger entries, the job can last several hours.</span></span>  

 <span data-ttu-id="e899f-125">Nel caso delle ubicazioni in cui i documenti di gestione della warehouse non venivano utilizzati prima della conversione, è necessario riaprire e rilasciare eventuali documenti di origine ricevuti parzialmente o spediti parzialmente prima della conversione.</span><span class="sxs-lookup"><span data-stu-id="e899f-125">For those locations that did not use warehouse management documents before the conversion, you must re-open and release any source documents that were partially received or partially shipped before the conversion.</span></span>  

## <a name="see-also"></a><span data-ttu-id="e899f-126">Vedi anche</span><span class="sxs-lookup"><span data-stu-id="e899f-126">See Also</span></span>  
[<span data-ttu-id="e899f-127">Gestione warehouse</span><span class="sxs-lookup"><span data-stu-id="e899f-127">Warehouse Management</span></span>](warehouse-manage-warehouse.md)  
[<span data-ttu-id="e899f-128">Magazzino</span><span class="sxs-lookup"><span data-stu-id="e899f-128">Inventory</span></span>](inventory-manage-inventory.md)  
<span data-ttu-id="e899f-129">[Impostazione gestione warehouse](warehouse-setup-warehouse.md)   </span><span class="sxs-lookup"><span data-stu-id="e899f-129">[Setting Up Warehouse Management](warehouse-setup-warehouse.md)   </span></span>  
<span data-ttu-id="e899f-130">[Gestione assemblaggio](assembly-assemble-items.md)  </span><span class="sxs-lookup"><span data-stu-id="e899f-130">[Assembly Management](assembly-assemble-items.md)  </span></span>  
[<span data-ttu-id="e899f-131">Dettagli di progettazione: Gestione warehouse</span><span class="sxs-lookup"><span data-stu-id="e899f-131">Design Details: Warehouse Management</span></span>](design-details-warehouse-management.md)  
<span data-ttu-id="e899f-132">[Utilizzo di [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="e899f-132">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
