---
title: Impostare una scheda ubicazione e definire i percorsi di trasferimento
description: "È possibile creare una scheda ubicazione per ogni area in cui vengono immagazzinati gli articoli in magazzino, ad esempio warehouse o centro di distribuzione, per impostare percorsi per il trasferimento degli articoli tra le ubicazioni."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: warehouse, distribution center
ms.date: 06/02/2017
ms.author: SorenGP
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: ca48f5df7977328aec3cc6ba352eadb361144bcb
ms.contentlocale: it-it
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-set-up-locations"></a><span data-ttu-id="e7da3-103">Procedura: Impostare le ubicazioni</span><span class="sxs-lookup"><span data-stu-id="e7da3-103">How to: Set Up Locations</span></span>
<span data-ttu-id="e7da3-104">Se si acquista, immagazzina o si vendono articoli in più aree o warehouse, è necessario impostare ogni ubicazione con una scheda ubicazione e definire i percorsi di trasferimento.</span><span class="sxs-lookup"><span data-stu-id="e7da3-104">If you buy, store, or sell items at more than one place or warehouse, you must set each location up with a location card and define transfer routes.</span></span>

<span data-ttu-id="e7da3-105">È quindi possibile creare le righe del documento per una specifica ubicazione, visualizzare la disponibilità per ubicazione e trasferire il magazzino tra le ubicazioni.</span><span class="sxs-lookup"><span data-stu-id="e7da3-105">You can then create document lines for a specific location, view availability by location, and transfer inventory between locations.</span></span> <span data-ttu-id="e7da3-106">Per ulteriori informazioni, vedere [Gestire il magazzino](inventory-manage-inventory.md).</span><span class="sxs-lookup"><span data-stu-id="e7da3-106">For more information, see [Manage Inventory](inventory-manage-inventory.md).</span></span>

## <a name="to-create-a-location-card"></a><span data-ttu-id="e7da3-107">Per creare una nuova scheda Ubicazione</span><span class="sxs-lookup"><span data-stu-id="e7da3-107">To create a location card</span></span>
1. <span data-ttu-id="e7da3-108">Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "Cerca pagina o report"), immettere **Ubicazioni**, quindi scegliere il collegamento correlato.</span><span class="sxs-lookup"><span data-stu-id="e7da3-108">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Locations**, and then choose the related link.</span></span>
2. <span data-ttu-id="e7da3-109">Scegliere l'azione **Nuovo**.</span><span class="sxs-lookup"><span data-stu-id="e7da3-109">Choose the **New** action.</span></span>
3. <span data-ttu-id="e7da3-110">Nella finestra **Scheda ubicazione** compilare i campi secondo le necessità.</span><span class="sxs-lookup"><span data-stu-id="e7da3-110">In the **Location Card** window, fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
4. <span data-ttu-id="e7da3-111">Ripetere i passaggi 2 e 3 per ogni ubicazione in cui si desidera mantenere il magazzino.</span><span class="sxs-lookup"><span data-stu-id="e7da3-111">Repeat steps 2 and 3 for every location where you want to keep inventory.</span></span>

> [!NOTE]  
> <span data-ttu-id="e7da3-112">Molti campi della scheda ubicazione fanno riferimento alla gestione degli articoli nei processi della warehouse in entrata e in uscita.</span><span class="sxs-lookup"><span data-stu-id="e7da3-112">Many fields on the location card refer to the handling of items in inbound and outbound warehouse processes.</span></span> <span data-ttu-id="e7da3-113">Per ulteriori informazioni, vedere [Impostazione gestione warehouse](warehouse-setup-warehouse.md).</span><span class="sxs-lookup"><span data-stu-id="e7da3-113">For more information, see [Setting Up Warehouse Management](warehouse-setup-warehouse.md).</span></span>

## <a name="to-create-a-transfer-route"></a><span data-ttu-id="e7da3-114">Per creare i percorsi di trasferimento</span><span class="sxs-lookup"><span data-stu-id="e7da3-114">To create a transfer route</span></span>
1. <span data-ttu-id="e7da3-115">Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **Percorsi di trasferimento**, quindi scegliere il collegamento correlato.</span><span class="sxs-lookup"><span data-stu-id="e7da3-115">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Transfer Routes**, and then choose the related link.</span></span>
2. <span data-ttu-id="e7da3-116">In alternativa, da una qualsiasi finestra **Scheda Ubicazione** scegliere l'azione **Percorsi trasferimento**.</span><span class="sxs-lookup"><span data-stu-id="e7da3-116">Alternatively, from any **Location Card** window, choose the **Transfer Routes** action.</span></span>
3. <span data-ttu-id="e7da3-117">Scegliere l'azione **Nuovo**.</span><span class="sxs-lookup"><span data-stu-id="e7da3-117">Choose the **New** action.</span></span>
4. <span data-ttu-id="e7da3-118">Nella finestra **Scheda ubicazione** compilare i campi secondo le necessità.</span><span class="sxs-lookup"><span data-stu-id="e7da3-118">In the **Location Card** window, fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

<span data-ttu-id="e7da3-119">A questo punto è possibile trasferire agli articoli di magazzino tra due ubicazioni.</span><span class="sxs-lookup"><span data-stu-id="e7da3-119">You can now transfer inventory items between two locations.</span></span> <span data-ttu-id="e7da3-120">Per ulteriori informazioni, vedere [Procedura: Trasferire il magazzino tra le ubicazioni](inventory-how-transfer-between-locations.md).</span><span class="sxs-lookup"><span data-stu-id="e7da3-120">For more information, see [How to: Transfer Inventory Between Locations](inventory-how-transfer-between-locations.md).</span></span>    

## <a name="see-also"></a><span data-ttu-id="e7da3-121">Vedi anche</span><span class="sxs-lookup"><span data-stu-id="e7da3-121">See Also</span></span>
[<span data-ttu-id="e7da3-122">Gestire i costi del magazzino</span><span class="sxs-lookup"><span data-stu-id="e7da3-122">Manage Inventory</span></span>](inventory-manage-inventory.md)  
<span data-ttu-id="e7da3-123">[Procedura: Trasferire il magazzino tra le ubicazioni](inventory-how-transfer-between-locations.md)  </span><span class="sxs-lookup"><span data-stu-id="e7da3-123">[How to: Transfer Inventory Between Locations](inventory-how-transfer-between-locations.md)  </span></span>  
<span data-ttu-id="e7da3-124">[Utilizzo di [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="e7da3-124">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  
<span data-ttu-id="e7da3-125">[Personalizzazione di [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-customizing-overview.md)</span><span class="sxs-lookup"><span data-stu-id="e7da3-125">[Customizing [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-customizing-overview.md)</span></span>  
[<span data-ttu-id="e7da3-126">Funzionalità aziendali generali</span><span class="sxs-lookup"><span data-stu-id="e7da3-126">General Business Functionality</span></span>](ui-across-business-areas.md)

