---
title: Come creare stoccaggi mediante stoccaggi interni
description: Dopo avere stoccato gli articoli e prima di prelevarli per soddisfare le richieste di un ordine di produzione o di una spedizione, gli articoli vengono inclusi tra le giacenze disponibili all'interno della warehouse.
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/16/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 970b9b9046018b0dcea5b9996d10e19e444a7639
ms.contentlocale: it-it
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-pick-and-put-away-without-a-source-document"></a><span data-ttu-id="432f1-103">Procedura: Selezionare e stoccare senza un documento di origine</span><span class="sxs-lookup"><span data-stu-id="432f1-103">How to: Pick and Put Away Without a Source Document</span></span>
<span data-ttu-id="432f1-104">Dopo avere stoccato gli articoli e prima di prelevarli per soddisfare le richieste di un ordine di produzione o di una spedizione, gli articoli vengono inclusi tra le giacenze disponibili all'interno della warehouse.</span><span class="sxs-lookup"><span data-stu-id="432f1-104">After items have been put away and before they are picked to fulfill the needs of a production order or shipment, they are stored in the warehouse as part of available inventory.</span></span>  

<span data-ttu-id="432f1-105">È possibile che, in circostanze particolari, gli articoli debbano essere prelevati temporaneamente dalle collocazioni di prelievo della warehouse per essere utilizzati, ad esempio, come modelli in contesti di vendita dimostrativi.</span><span class="sxs-lookup"><span data-stu-id="432f1-105">Situations can arise where items must be taken out of the warehouse pick bins temporarily, perhaps to serve as demonstration models in a sales presentation.</span></span> <span data-ttu-id="432f1-106">Tali articoli sono ancora di proprietà della società e fanno ancora parte delle giacenze a magazzino, ma non sono disponibili per il prelievo.</span><span class="sxs-lookup"><span data-stu-id="432f1-106">These items are still owned by the company and are part of inventory, but they are not available for picking.</span></span> <span data-ttu-id="432f1-107">Gli articoli vengono registrati in una collocazione ad uso speciale creata a tale scopo e, benché tecnicamente siano ancora registrati nella warehouse, fisicamente possano trovarsi in una sala riunioni o in un salone di esposizione.</span><span class="sxs-lookup"><span data-stu-id="432f1-107">They are registered in a special purpose bin that you create for this purpose; technically, the items are in the warehouse, but physically, they could be in a conference or demonstration room.</span></span>  

<span data-ttu-id="432f1-108">In altre circostanze, è possibile che l'unità di produzione abbia bisogno di alcuni componenti non previsti per un processo.</span><span class="sxs-lookup"><span data-stu-id="432f1-108">In other situations, the production unit might unexpectedly need a few parts for a process.</span></span> <span data-ttu-id="432f1-109">In tal caso, è possibile prelevare articoli per le collocazioni di produzione utilizzando la funzione di prelievo interno.</span><span class="sxs-lookup"><span data-stu-id="432f1-109">You can pick items for the production bins using the internal pick.</span></span> <span data-ttu-id="432f1-110">Al termine del processo e una volta realizzato l'output di produzione, è necessario registrare il consumo degli articoli e svuotare la collocazione di produzione, il che comporta, a sua volta, una diminuzione della quantità dell'articolo nell'ubicazione.</span><span class="sxs-lookup"><span data-stu-id="432f1-110">When the process is over and output is created, you post the consumption of the items and empty the production bin, which in turn decreases the quantity of the item at your location.</span></span>  

<span data-ttu-id="432f1-111">Analogamente, gli articoli possono essere restituiti alla warehouse per lo stoccaggio.</span><span class="sxs-lookup"><span data-stu-id="432f1-111">Likewise, items can be returned to the warehouse to be put away.</span></span> <span data-ttu-id="432f1-112">È ad esempio possibile che determinati articoli siano stati prelevati dalle giacenze disponibili per un ordine di produzione e che non siano stati utilizzati.</span><span class="sxs-lookup"><span data-stu-id="432f1-112">The items may have been taken out of available inventory for a production order, and then not used at all.</span></span> <span data-ttu-id="432f1-113">Per reintegrarli nuovamente nelle giacenze disponibili, è necessario stoccarli nella collocazione.</span><span class="sxs-lookup"><span data-stu-id="432f1-113">To make them part of available inventory again, they must be put away in the bin.</span></span>  

<span data-ttu-id="432f1-114">**Stoccaggi interni** consente di eseguire stoccaggi senza dover fare riferimento a uno specifico documento di origine.</span><span class="sxs-lookup"><span data-stu-id="432f1-114">The **Internal Put-aways** enables you to perform put-aways without having to refer to a particular source document.</span></span> <span data-ttu-id="432f1-115">È possibile impostare facilmente tutte le informazioni necessarie per la creazione di un'istruzione di warehouse di stoccaggio.</span><span class="sxs-lookup"><span data-stu-id="432f1-115">You can easily set up all the information you need to create a put-away warehouse instruction.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="432f1-116">Se non si utilizzano i prelievi interni e gli stoccaggi interni, è possibile apportare queste rettifiche tramite lo spostamento degli articoli da una collocazione a un'altra o la registrazione delle rettifiche della quantità in una collocazione.</span><span class="sxs-lookup"><span data-stu-id="432f1-116">If you are not using internal picks and internal put-aways, these adjustments can be performed using the methods to move items from bin to bin or to post quantity adjustments in a bin.</span></span>  
>   
>  <span data-ttu-id="432f1-117">Quando per una determinata ubicazione sono previsti stoccaggi e prelievi guidati, e si utilizzano pertanto i tipi di collocazione, non è possibile spostare manualmente gli articoli all'interno o all'esterno di una collocazione di tipo Ricevi poiché gli articoli presenti in questo tipo di collocazione devono essere registrati come stoccati prima di essere inseriti nella giacenza disponibile.</span><span class="sxs-lookup"><span data-stu-id="432f1-117">When the location uses directed put-away and pick, and therefore uses bin types, you cannot manually move items in or out of a bin of bin type RECEIVE, because items that are in a RECEIVE-type bin must be registered as being put away before they are part of available inventory.</span></span>  

## <a name="to-create-an-internal-pick"></a><span data-ttu-id="432f1-118">Per creare un prelievo interno</span><span class="sxs-lookup"><span data-stu-id="432f1-118">To create an internal pick</span></span>  
1.  <span data-ttu-id="432f1-119">Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "Cerca pagina o report"), immettere **Prelievo interno whse.**, quindi scegliere il collegamento correlato.</span><span class="sxs-lookup"><span data-stu-id="432f1-119">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Whse. Internal Pick**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="432f1-120">Compilare il campo **Nr.**</span><span class="sxs-lookup"><span data-stu-id="432f1-120">Fill in the **No.**</span></span> <span data-ttu-id="432f1-121">e il campo **A codice collocazione** nella Scheda dettaglio **Generale**.</span><span class="sxs-lookup"><span data-stu-id="432f1-121">field and the **To Bin Code** field on the **General** FastTab.</span></span> <span data-ttu-id="432f1-122">Il campo **A codice collocazione** indica la collocazione da cui devono essere prelevati gli articoli.</span><span class="sxs-lookup"><span data-stu-id="432f1-122">The **To Bin Code** field specifies the bin from which you want to get the items.</span></span> <span data-ttu-id="432f1-123">Ai fini della produzione, questa collocazione rappresenta la collocazione di produzione in entrata o la collocazione del reparto produttivo aperto.</span><span class="sxs-lookup"><span data-stu-id="432f1-123">For production purposes, this bin would be the inbound production bin or the open shop bin.</span></span> <span data-ttu-id="432f1-124">Viceversa, per altri scopi scegliere il campo A codice collocazione immettendo il codice per un tipo di collocazione che non viene utilizzata per il prelievo, in genere una collocazione di stazionamento, una collocazione di spedizione o un collocazione ad uso speciale.</span><span class="sxs-lookup"><span data-stu-id="432f1-124">For other purposes, choose a To Bin Code of a bin type that is not used for picking, most likely a staging, shipping or special purpose bin.</span></span>  
3.  <span data-ttu-id="432f1-125">Selezionare un articolo nel campo **Nr. articolo**, quindi immettere le quantità che si desidera prelevare.</span><span class="sxs-lookup"><span data-stu-id="432f1-125">Select an item in the **Item No.** field, and fill in the quantities you want to pick.</span></span>  
4. <span data-ttu-id="432f1-126">Scegliere l'azione **Crea prelievo**.</span><span class="sxs-lookup"><span data-stu-id="432f1-126">Choose the **Create Pick** action.</span></span> <span data-ttu-id="432f1-127">Verrà creata un'istruzione di prelievo indirizzata agli impiegati warehouse.</span><span class="sxs-lookup"><span data-stu-id="432f1-127">A warehouse pick instruction is now ready for a warehouse employee to perform.</span></span>  

## <a name="to-create-an-internal-put-away"></a><span data-ttu-id="432f1-128">Per creare uno stoccaggio interno</span><span class="sxs-lookup"><span data-stu-id="432f1-128">To create an internal put-away</span></span>  
1.  <span data-ttu-id="432f1-129">Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "Cerca pagina o report"), immettere **Prelievo interno whse.**, quindi scegliere il collegamento correlato.</span><span class="sxs-lookup"><span data-stu-id="432f1-129">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Whse. Internal Put-away**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="432f1-130">Compilare il campo **Nr.**</span><span class="sxs-lookup"><span data-stu-id="432f1-130">Fill in the **No.**</span></span> <span data-ttu-id="432f1-131">e il campo **Dal codice collocazione** nella Scheda dettaglio **Generale**.</span><span class="sxs-lookup"><span data-stu-id="432f1-131">and **From Bin Code** fields on the **General** FastTab.</span></span> <span data-ttu-id="432f1-132">Il campo **Dal codice collocazione** indica la collocazione in cui vengono posizionati gli articoli restituiti alla warehouse, ad esempio dalla produzione.</span><span class="sxs-lookup"><span data-stu-id="432f1-132">The **From Bin Code** field specifies the bin where the items being returned to the warehouse, perhaps from production, are located.</span></span>  
3.  <span data-ttu-id="432f1-133">Immettere i numeri di articolo e le quantità nelle righe appropriate.</span><span class="sxs-lookup"><span data-stu-id="432f1-133">Fill in the item numbers and quantities on the lines.</span></span>  
4.  <span data-ttu-id="432f1-134">Selezionare l'azione **Crea stoccaggio**.</span><span class="sxs-lookup"><span data-stu-id="432f1-134">Choose the **Create Put-away** action.</span></span> <span data-ttu-id="432f1-135">Verrà creata un'istruzione di stoccaggio indirizzata agli impiegati warehouse.</span><span class="sxs-lookup"><span data-stu-id="432f1-135">A warehouse put-away instruction is now ready for a warehouse employee to perform.</span></span>  

## <a name="see-also"></a><span data-ttu-id="432f1-136">Vedi anche</span><span class="sxs-lookup"><span data-stu-id="432f1-136">See Also</span></span>  
[<span data-ttu-id="432f1-137">Gestione warehouse</span><span class="sxs-lookup"><span data-stu-id="432f1-137">Warehouse Management</span></span>](warehouse-manage-warehouse.md)  
[<span data-ttu-id="432f1-138">Magazzino</span><span class="sxs-lookup"><span data-stu-id="432f1-138">Inventory</span></span>](inventory-manage-inventory.md)  
<span data-ttu-id="432f1-139">[Impostazione gestione warehouse](warehouse-setup-warehouse.md)   </span><span class="sxs-lookup"><span data-stu-id="432f1-139">[Setting Up Warehouse Management](warehouse-setup-warehouse.md)   </span></span>  
<span data-ttu-id="432f1-140">[Gestione assemblaggio](assembly-assemble-items.md)  </span><span class="sxs-lookup"><span data-stu-id="432f1-140">[Assembly Management](assembly-assemble-items.md)  </span></span>  
[<span data-ttu-id="432f1-141">Dettagli di progettazione: Gestione warehouse</span><span class="sxs-lookup"><span data-stu-id="432f1-141">Design Details: Warehouse Management</span></span>](design-details-warehouse-management.md)  
<span data-ttu-id="432f1-142">[Utilizzo di [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="432f1-142">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
