---
title: Registrazione di assistenza
description: "La funzionalità di registrazione dei servizi di assistenza consente di elaborare i documenti in modo efficiente e di gestire in modo efficace il servizio di assistenza offerto ai clienti. È possibile creare e aggiornare documenti registrati, nonché creare movimenti contabili sia nell'area di assistenza che in altri moduli per garantire modifiche correttamente aggiornate."
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 09/18/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 7ab0d57c960b0568c1da1896914f1a1ce939d0ea
ms.contentlocale: it-it
ms.lasthandoff: 10/16/2017

---
# <a name="service-posting"></a><span data-ttu-id="34a71-104">Registrazione di assistenza</span><span class="sxs-lookup"><span data-stu-id="34a71-104">Service Posting</span></span>
<span data-ttu-id="34a71-105">La funzionalità di registrazione dei servizi di assistenza consente di elaborare i documenti in modo efficiente e di gestire in modo efficace il servizio di assistenza offerto ai clienti.</span><span class="sxs-lookup"><span data-stu-id="34a71-105">Service posting functionality lets you process your documents efficiently and maintain successful customer service policy.</span></span> <span data-ttu-id="34a71-106">È possibile creare e aggiornare documenti registrati, nonché creare movimenti contabili sia nell'area di assistenza che in altri moduli per garantire modifiche correttamente aggiornate.</span><span class="sxs-lookup"><span data-stu-id="34a71-106">You can create and update posted documents, and create ledger entries both in the service area and in other modules to ensure the correct update.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="34a71-107">Di seguito viene descritta la registrazione di assistenza indipendentemente dalla modalità di gestione fisica degli articoli nella warehouse.</span><span class="sxs-lookup"><span data-stu-id="34a71-107">The following describes service posting regardless of how items are physically handled in the warehouse.</span></span>  
>   
>  <span data-ttu-id="34a71-108">In un'ubicazione non impostata per richiedere la gestione warehouse, le azioni di registrazione vengono effettuate direttamente nella finestra **Righe assistenza**.</span><span class="sxs-lookup"><span data-stu-id="34a71-108">In a location that is not set up to require warehouse handling, you perform the posting actions directly from the **Service Lines** window.</span></span> <span data-ttu-id="34a71-109">Nelle ubicazioni che prevedono la gestione in warehouse, le azioni di registrazione descritte, tranne Spedizione e consumo, vengono eseguite indirettamente tramite diverse funzioni di spedizione warehouse, a seconda del setup.</span><span class="sxs-lookup"><span data-stu-id="34a71-109">In locations that involve warehouse handling, the described posting actions, except Ship and Consume, are performed indirectly through varying warehouse ship functions, depending on setup.</span></span> <span data-ttu-id="34a71-110">Per ulteriori informazioni, vedere [Procedura: Prelevare articoli con prelievi magazzino](warehouse-how-to-pick-items-with-inventory-picks.md).</span><span class="sxs-lookup"><span data-stu-id="34a71-110">For more information, see [How to: Pick Items with Inventory Picks](warehouse-how-to-pick-items-with-inventory-picks.md).</span></span>  

## <a name="ship"></a><span data-ttu-id="34a71-111">Spedizione</span><span class="sxs-lookup"><span data-stu-id="34a71-111">Ship</span></span>  
<span data-ttu-id="34a71-112">L'opzione relativa alla spedizione consente di registrare gli articoli e il tempo appropriati immessi nelle righe di un ordine di assistenza dopo il completamento dell'assistenza stessa.</span><span class="sxs-lookup"><span data-stu-id="34a71-112">The ship option lets you register the relevant items and time entered on the lines of a service order after you complete the service.</span></span> <span data-ttu-id="34a71-113">Viene creata una spedizione registrata e si verificano aggiornamenti nel modulo Magazzino e in altri moduli di [!INCLUDE[d365fin](includes/d365fin_md.md)] con l'indicazione che gli articoli sono stati prelevati dal magazzino e inviati al cliente.</span><span class="sxs-lookup"><span data-stu-id="34a71-113">A posted shipment is created and updates occur in the Inventory module and other modules in [!INCLUDE[d365fin](includes/d365fin_md.md)] to reflect that the items have been taken out of the inventory and sent to the customer.</span></span> <span data-ttu-id="34a71-114">In particolare, vengono generati movimenti contabili relativi agli articoli e al valore, movimenti assistenza e movimenti garanzia.</span><span class="sxs-lookup"><span data-stu-id="34a71-114">In particular, the item ledger entries, value ledger entries, service ledger entries, and warranty ledger entries are produced.</span></span>  

<span data-ttu-id="34a71-115">Se l'ubicazione è impostata in modo da richiedere la gestione warehouse, la spedizione e movimentazione degli articoli nelle righe di assistenza funzionano allo stesso modo di altri documenti di origine.</span><span class="sxs-lookup"><span data-stu-id="34a71-115">If the location is set up to require warehouse handling, then the shipping and moving of service line items functions in the same ways as for other source documents.</span></span> <span data-ttu-id="34a71-116">La sola differenza sta nel fatto che gli articoli nelle righe di assistenza possono essere consumati esternamente o internamente e richiedono due diverse funzioni di rilascio.</span><span class="sxs-lookup"><span data-stu-id="34a71-116">The only difference is that service line items can be consumed either externally or internally, which requires two different release functions.</span></span>

## <a name="invoice"></a><span data-ttu-id="34a71-117">Fattura</span><span class="sxs-lookup"><span data-stu-id="34a71-117">Invoice</span></span>  
<span data-ttu-id="34a71-118">Questa opzione consente di emettere una fattura verso il cliente a cui si desidera addebitare l'assistenza.</span><span class="sxs-lookup"><span data-stu-id="34a71-118">You have to use the invoice option to issue an invoice to the customer you want to charge for the service.</span></span> <span data-ttu-id="34a71-119">L'importo da fatturare è in genere costituito dalla differenza tra la quantità spedita registrata mediante la funzione **Registrare spedizione** e la quantità consumata registrata mediante la funzione **Registra consumo**.</span><span class="sxs-lookup"><span data-stu-id="34a71-119">Usually, it is the difference between the shipped quantity registered by the **Post Shipment** function and the consumed quantity registered by the **Post Consumption** function that is subject to invoice.</span></span> <span data-ttu-id="34a71-120">Non è possibile fatturare quantità che non sono state spedite.</span><span class="sxs-lookup"><span data-stu-id="34a71-120">You cannot invoice what has not been shipped.</span></span> <span data-ttu-id="34a71-121">Quando si esegue la funzione **Registra fatture**, viene creata una fattura di assistenza registrata e vengono aggiornati i documenti registrati prima di modificarli in base alle quantità contenute nella fattura emessa.</span><span class="sxs-lookup"><span data-stu-id="34a71-121">When you run the **Post Invoice** function, you create a posted service invoice and update the documents posted before to make them consistent with the quantities that are contained in the issued invoice.</span></span> <span data-ttu-id="34a71-122">Analogamente ad altre procedure di registrazione, vengono generati i movimenti contabili corrispondenti, inclusi i movimenti di contabilità generale.</span><span class="sxs-lookup"><span data-stu-id="34a71-122">Like in other posting procedures, the relevant ledger entries that includes general ledger entries, are generated.</span></span>  

## <a name="ship-and-invoice"></a><span data-ttu-id="34a71-123">Spedizione e Fattura</span><span class="sxs-lookup"><span data-stu-id="34a71-123">Ship and Invoice</span></span>  
<span data-ttu-id="34a71-124">L'opzione di spedizione e fattura consente di emettere sia una spedizione di assistenza che una fattura contemporaneamente.</span><span class="sxs-lookup"><span data-stu-id="34a71-124">The ship and invoice option lets you issue both a service shipment and an invoice at the same time.</span></span>  

## <a name="ship-and-consume"></a><span data-ttu-id="34a71-125">Spedizione e consumo</span><span class="sxs-lookup"><span data-stu-id="34a71-125">Ship and Consume</span></span>  
<span data-ttu-id="34a71-126">L'opzione di spedizione e consumo consente di registrare e contabilizzare articoli, costi oppure ore utilizzati per prestare assistenza, ma che non possono essere inclusi nella fattura da inviare al cliente.</span><span class="sxs-lookup"><span data-stu-id="34a71-126">With the ship and consume option, you can register and post items, costs, or hours that have been used for servicing but that cannot be included in the invoice to the customer.</span></span> <span data-ttu-id="34a71-127">In base a questa opzione non viene emessa alcuna fattura, ma è possibile generare contemporaneamente una spedizione e un consumo di assistenza per indicare che al cliente sono stati concessi alcuni articoli oppure ore gratuiti.</span><span class="sxs-lookup"><span data-stu-id="34a71-127">An invoice is not issued, but you can issue both a service shipment and service consumption at the same time to reflect the fact that some items or hours have been given to the customer free of charge.</span></span> <span data-ttu-id="34a71-128">Per registrare il consumo, vengono inoltre creati i movimenti contabili corrispondenti.</span><span class="sxs-lookup"><span data-stu-id="34a71-128">The corresponding ledger entries are also created to register consumption.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="34a71-129">La procedura di registrazione di assistenza consente di eseguire la registrazione parziale.</span><span class="sxs-lookup"><span data-stu-id="34a71-129">The service posting procedure enables you to perform partial posting.</span></span> <span data-ttu-id="34a71-130">Prima di effettuare la registrazione, è inoltre possibile creare una spedizione parziale o una fattura parziale compilando i campi **Qtà da spedire** e **Qtà da fatturare** nelle singole righe di assistenza degli ordini di assistenza.</span><span class="sxs-lookup"><span data-stu-id="34a71-130">You can create a partial shipment or a partial invoice by filling in the **Qty. to Ship** and **Qty. to Invoice** fields on the individual service lines of the service orders before you post.</span></span> <span data-ttu-id="34a71-131">Si tenga presente che non è possibile creare una fattura per un articolo che non è stato spedito.</span><span class="sxs-lookup"><span data-stu-id="34a71-131">Note that you cannot create an invoice for something that is not shipped.</span></span> <span data-ttu-id="34a71-132">Ciò significa che è necessario registrare una spedizione prima di emettere una fattura oppure la spedizione e la fattura devono essere contemporanee.</span><span class="sxs-lookup"><span data-stu-id="34a71-132">That is, before you can invoice, you must have registered a shipment, or you must choose to ship and invoice at the same time.</span></span>  

<span data-ttu-id="34a71-133">Dopo il completamento della registrazione, sarà possibile visualizzare i documenti di assistenza registrati nelle finestre corrispondenti, ovvero **Spedizione assistenza registrata** e **Fattura assistenza registrata**.</span><span class="sxs-lookup"><span data-stu-id="34a71-133">After the posting has been completed, you will be able to view the posted service documents from the corresponding **Posted Service Shipment** and **Posted Service Invoice** windows.</span></span> <span data-ttu-id="34a71-134">I movimenti creati possono essere visualizzati in apposite finestre contenenti movimenti registrati, ad esempio **Movimenti C/G**, **Mov. contabili articoli**, **Movimenti warehouse**, **Movimenti assistenza**, **Movimenti cont. commesse** e **Movimenti garanzia**.</span><span class="sxs-lookup"><span data-stu-id="34a71-134">The posted entries created can be seen in various windows that contain posted entries, such as **G/L Entries**, **Item Ledger Entries**, **Warehouse Entries**, **Service Ledger Entries**, **Job Ledger Entries**, and **Warranty Ledger Entries**.</span></span>  

## <a name="to-view-information-about-a-posted-service-document"></a><span data-ttu-id="34a71-135">Per visualizzare informazioni su un documento di assistenza registrato</span><span class="sxs-lookup"><span data-stu-id="34a71-135">To view information about a posted service document</span></span>  
<span data-ttu-id="34a71-136">Quando si registra una fattura, una spedizione o una nota di credito di assistenza, le informazioni presenti nel documento vengono trasferite nella finestra **Fattura assistenza registrata**, **Spedizione assistenza registrata** o **Nota credito assistenza registrata** rispettivamente.</span><span class="sxs-lookup"><span data-stu-id="34a71-136">When you post a service invoice, a service shipment, or a service credit memo, the information on the document is transferred to the **Posted Service Invoice**, **Posted Service Shipment**, or **Posted Service Credit Memo** windows respectively.</span></span> <span data-ttu-id="34a71-137">In queste finestre non è possibile immettere, modificare né eliminare alcuna informazione.</span><span class="sxs-lookup"><span data-stu-id="34a71-137">You cannot enter, change, or delete anything in these windows.</span></span> <span data-ttu-id="34a71-138">Nelle finestre è possibile stampare una spedizione, una fattura o una nota di credito.</span><span class="sxs-lookup"><span data-stu-id="34a71-138">You can print a shipment, invoice, or credit memo from these windows.</span></span>  

<span data-ttu-id="34a71-139">Nella procedura seguente viene utilizzata una fattura di assistenza registrata come esempio, ma la stessa procedura può essere applicata alle spedizioni di assistenza registrate e alle note di credito registrate.</span><span class="sxs-lookup"><span data-stu-id="34a71-139">The following procedure uses a posted service invoice as an example, but the same procedure can apply to posted service shipments and posted credit memos.</span></span>  

1. <span data-ttu-id="34a71-140">Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **Fattura assistenza registrata**, quindi scegliere il collegamento correlato.</span><span class="sxs-lookup"><span data-stu-id="34a71-140">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Posted Service Invoice**, and then choose the related link.</span></span>  
2. <span data-ttu-id="34a71-141">Aprire la fattura di assistenza registrata che si desidera visualizzare.</span><span class="sxs-lookup"><span data-stu-id="34a71-141">Open the posted service invoice you want to view.</span></span>  
3. <span data-ttu-id="34a71-142">Per ottenere una panoramica della fattura registrata, scegliere l'azione **Statistiche**.</span><span class="sxs-lookup"><span data-stu-id="34a71-142">To get an overview of the posted invoice, choose the **Statistics** action.</span></span>  

    <span data-ttu-id="34a71-143">Viene visualizzata la finestra **Statistiche ordine assistenza**.</span><span class="sxs-lookup"><span data-stu-id="34a71-143">The **Service Order Statistics** window opens.</span></span> <span data-ttu-id="34a71-144">Nella finestra vengono visualizzate informazioni quali quantità, importo, IVA, costo, margine e limite di credito del cliente per il documento registrato.</span><span class="sxs-lookup"><span data-stu-id="34a71-144">The window displays information such as quantity, amount, VAT, cost, profit, and customer credit limit for the posted document.</span></span>

## <a name="see-also"></a><span data-ttu-id="34a71-145">Vedi anche</span><span class="sxs-lookup"><span data-stu-id="34a71-145">See Also</span></span>  
<span data-ttu-id="34a71-146">[Procedura: Registrare gli ordini di assistenza](service-how-to-post-service-orders.md) </span><span class="sxs-lookup"><span data-stu-id="34a71-146">[How to: Post Service Orders](service-how-to-post-service-orders.md) </span></span>  
[<span data-ttu-id="34a71-147">Procedura: Creare ordini di assistenza</span><span class="sxs-lookup"><span data-stu-id="34a71-147">How to: Create Service Orders</span></span>](service-how-to-create-service-orders.md)
