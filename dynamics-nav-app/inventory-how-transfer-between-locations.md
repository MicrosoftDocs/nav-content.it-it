---
title: Trasferire articoli tra le warehouse
description: Viene descritto come spostare il magazzino da un'area o una warehouse a un'altra con le registrazioni di riclassificazione o gli ordini di trasferimento.
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: move, warehouse
ms.date: 06/02/2017
ms.author: SorenGP
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: f2be3ef1613356bb2b0d1a02c355e09a546de62d
ms.contentlocale: it-it
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-transfer-inventory-between-locations"></a><span data-ttu-id="c8649-103">Procedura: Trasferire il magazzino tra le ubicazioni</span><span class="sxs-lookup"><span data-stu-id="c8649-103">How to: Transfer Inventory Between Locations</span></span>
<span data-ttu-id="c8649-104">È possibile trasferire articoli di magazzino tra ubicazioni creando ordini di trasferimento.</span><span class="sxs-lookup"><span data-stu-id="c8649-104">You can transfer inventory items between locations by creating transfer orders.</span></span> <span data-ttu-id="c8649-105">In alternativa, è possibile utilizzare le registrazioni di riclassificazione articoli.</span><span class="sxs-lookup"><span data-stu-id="c8649-105">Alternatively, you can use the item reclassification journal.</span></span>

<span data-ttu-id="c8649-106">Con gli ordini di trasferimento, si spedisce il trasferimento in uscita da un'ubicazione e si riceve il trasferimento in entrata presso un'altra ubicazione.</span><span class="sxs-lookup"><span data-stu-id="c8649-106">With transfer orders, you ship the outbound transfer from one location and receive the inbound transfer at the other location.</span></span> <span data-ttu-id="c8649-107">Ciò consente di gestire le attività di warehouse implicate e offre maggiore certezza che le quantità di magazzino di vengano aggiornate correttamente.</span><span class="sxs-lookup"><span data-stu-id="c8649-107">This allows you to manage the involved warehouse activities and provides more certainty that inventory quantities are updated correctly.</span></span>

<span data-ttu-id="c8649-108">Con la registrazione di riclassificazione, si compila semplicemente i campi **Codice ubicazione** e **Nuovo codice ubicazione**.</span><span class="sxs-lookup"><span data-stu-id="c8649-108">With the reclassification journal, you simply fill in the **Location Code** and the **New Location Code** fields.</span></span> <span data-ttu-id="c8649-109">Quando si contabilizza la registrazione, i movimenti contabili articoli vengono rettificati nelle ubicazioni in questione.</span><span class="sxs-lookup"><span data-stu-id="c8649-109">When you post the journal, the item ledger entries are adjusted at the locations in question.</span></span> <span data-ttu-id="c8649-110">Con questo metodo, le attività di warehouse non vengono gestite.</span><span class="sxs-lookup"><span data-stu-id="c8649-110">With this method, warehouse activities are not managed.</span></span>

> [!NOTE]  
>   <span data-ttu-id="c8649-111">Se sono stati registrati articoli in magazzino senza un codice ubicazione, ad esempio a partire da un periodo in cui era disponibile solo una warehouse, non è possibile trasferire gli articoli tramite ordini di trasferimento.</span><span class="sxs-lookup"><span data-stu-id="c8649-111">If you have items recorded in your inventory without a location code, for example from a time when you only had one warehouse, then you cannot transfer those items using transfer orders.</span></span> <span data-ttu-id="c8649-112">Al contrario, è necessario utilizzare le registrazioni di riclassificazione per riclassificare gli articoli da un codice di un'ubicazione vuota a un codice di ubicazione effettiva.</span><span class="sxs-lookup"><span data-stu-id="c8649-112">Instead, you must use the reclassification journal to reclassify the items from a blank location code to an actual location code.</span></span>  <span data-ttu-id="c8649-113">Per ulteriori informazioni, vedere il passaggio 3 nella sezione "Per trasferire gli articoli con le registrazioni di riclassificazione articolo".</span><span class="sxs-lookup"><span data-stu-id="c8649-113">For more information, see step 3 in the "To transfer items with the item reclassification journal" section.</span></span>

<span data-ttu-id="c8649-114">Per trasferire gli articoli, le ubicazioni e i percorsi di trasferimento devono essere impostati.</span><span class="sxs-lookup"><span data-stu-id="c8649-114">To transfer items, locations and transfer routes must be set up.</span></span> <span data-ttu-id="c8649-115">Per ulteriori informazioni, vedere [Procedura: Impostare le ubicazioni](inventory-how-setup-locations.md).</span><span class="sxs-lookup"><span data-stu-id="c8649-115">For more information, see [How to: Set Up Locations](inventory-how-setup-locations.md).</span></span>

## <a name="to-transfer-items-with-a-transfer-order"></a><span data-ttu-id="c8649-116">Per trasferire gli articoli con un ordine di trasferimento</span><span class="sxs-lookup"><span data-stu-id="c8649-116">To transfer items with a transfer order</span></span>
1. <span data-ttu-id="c8649-117">Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **Ordini di trasferimento**, quindi scegliere il collegamento correlato.</span><span class="sxs-lookup"><span data-stu-id="c8649-117">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Transfer orders**, and then choose the related link.</span></span>
2. <span data-ttu-id="c8649-118">Nella finestra **Ordine di trasferimento** compilare i campi secondo le necessità.</span><span class="sxs-lookup"><span data-stu-id="c8649-118">In the **Transfer Order** window, fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

    > [!NOTE]  
>   <span data-ttu-id="c8649-119">Se i campi **Codice in transito**, **Cod. spedizioniere** e **Servizi spedizioniere** nella finestra **Specifica percorso trasf.** sono stati compilati al momento dell'impostazione del percorso di trasferimento, i dati verranno immessi automaticamente nei campi corrispondenti dell'ordine di trasferimento.</span><span class="sxs-lookup"><span data-stu-id="c8649-119">If you have filled in the **In-Transit Code**, **Shipping Agent Code**, and **Shipping Agent Service** fields in the **Trans. Route Spec.** window when you set up the transfer route, then the corresponding fields on the transfer order are filled in automatically.</span></span>

    <span data-ttu-id="c8649-120">Se si compila il campo **Servizio spedizioniere**, il programma calcola la data di ricezione nell'ubicazione di trasferimento sommando il tempo di spedizione del servizio spedizioniere alla data di spedizione.</span><span class="sxs-lookup"><span data-stu-id="c8649-120">When you fill in the **Shipping Agent Service** field, the receipt date at the transfer-to location is calculated by adding the shipping time of the shipping agent service to the shipment date.</span></span>

    <span data-ttu-id="c8649-121">Come lavoratore warehouse nell'ubicazione da cui viene effettuato il trasferimento, continuare con la spedizione degli articoli.</span><span class="sxs-lookup"><span data-stu-id="c8649-121">As a warehouse worker at the transfer-from location, proceed to ship the items.</span></span>
3. <span data-ttu-id="c8649-122">Scegliere l'azione **Registra**, selezionare l'opzione **Spedizione**, quindi il pulsante **OK**.</span><span class="sxs-lookup"><span data-stu-id="c8649-122">Choose the **Post** action, choose the **Ship** option, and then choose the **OK** button.</span></span>

    <span data-ttu-id="c8649-123">Gli articoli sono ora in transito tra le ubicazioni specificate, in base al percorso indicato per il trasferimento.</span><span class="sxs-lookup"><span data-stu-id="c8649-123">The items are now in transit between the specified locations, according to the specifies transfer route.</span></span>

    <span data-ttu-id="c8649-124">Come lavoratore warehouse nell'ubicazione da cui viene effettuato il trasferimento, continuare con la ricezione degli articoli.</span><span class="sxs-lookup"><span data-stu-id="c8649-124">As a warehouse worker at the transfer-from location, proceed to receive the items.</span></span>
4. <span data-ttu-id="c8649-125">Scegliere l'azione **Registra**, selezionare l'opzione **Ricevi**, quindi il pulsante **OK**.</span><span class="sxs-lookup"><span data-stu-id="c8649-125">Choose the **Post** action, choose the **Receive** option, and then choose the **OK** button.</span></span>

## <a name="to-transfer-items-with-the-item-reclassification-journal"></a><span data-ttu-id="c8649-126">Per trasferire gli articoli con le registrazioni di riclassificazione articolo</span><span class="sxs-lookup"><span data-stu-id="c8649-126">To transfer items with the item reclassification journal</span></span>
1. <span data-ttu-id="c8649-127">Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **Registrazioni riclassificazioni articoli**, quindi scegliere il collegamento correlato.</span><span class="sxs-lookup"><span data-stu-id="c8649-127">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Item Reclass. Journals**, and then choose the related link.</span></span>
2. <span data-ttu-id="c8649-128">Nella finestra **Batch reg. riclass. articoli** compilare i campi in base alle esigenze.</span><span class="sxs-lookup"><span data-stu-id="c8649-128">In the **Item Reclass. Journal** window, fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
3. <span data-ttu-id="c8649-129">Nel campo **Cod. ubicazione** immettere l'ubicazione in cui gli articoli si trovano attualmente.</span><span class="sxs-lookup"><span data-stu-id="c8649-129">In the **Location Code** field, enter the location where the items are currently stored.</span></span>

    > [!NOTE]  
>   <span data-ttu-id="c8649-130">Per trasferire gli articoli che non presentano codice ubicazione, lasciare vuoto il campo **Codice ubicazione**.</span><span class="sxs-lookup"><span data-stu-id="c8649-130">To transfer items that have no location code, leave the **Location Code** field blank.</span></span>
4. <span data-ttu-id="c8649-131">Nel campo **Nuovo codice ubicazione** immettere l'ubicazione verso cui si intende trasferire gli articoli.</span><span class="sxs-lookup"><span data-stu-id="c8649-131">In the **New Location Code** field, enter the location that you want to transfer the items to.</span></span>
5. <span data-ttu-id="c8649-132">Scegliere l'azione **Registra**.</span><span class="sxs-lookup"><span data-stu-id="c8649-132">Choose the **Post** action.</span></span>

## <a name="see-also"></a><span data-ttu-id="c8649-133">Vedi anche</span><span class="sxs-lookup"><span data-stu-id="c8649-133">See Also</span></span>
[<span data-ttu-id="c8649-134">Gestire i costi del magazzino</span><span class="sxs-lookup"><span data-stu-id="c8649-134">Manage Inventory</span></span>](inventory-manage-inventory.md)  
[<span data-ttu-id="c8649-135">Procedura: Impostare le ubicazioni</span><span class="sxs-lookup"><span data-stu-id="c8649-135">How to: Set Up Locations</span></span>](inventory-how-setup-locations.md)  

<span data-ttu-id="c8649-136">[Utilizzo di [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="c8649-136">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  
<span data-ttu-id="c8649-137">[Personalizzazione di [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-customizing-overview.md)</span><span class="sxs-lookup"><span data-stu-id="c8649-137">[Customizing [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-customizing-overview.md)</span></span>  
[<span data-ttu-id="c8649-138">Funzionalità aziendali generali</span><span class="sxs-lookup"><span data-stu-id="c8649-138">General Business Functionality</span></span>](ui-across-business-areas.md)

##
