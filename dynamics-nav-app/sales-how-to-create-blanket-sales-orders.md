---
title: Come creare ordini di vendita programmati
description: "Gli ordini programmati vengono utilizzati quando un cliente si impegna ad acquistare grandi quantità che verranno consegnate con diverse spedizioni più piccole effettuate in un determinato periodo di tempo."
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 09/08/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 88d4c5ca78e23476115b23a682e6bcdb25526f1d
ms.contentlocale: it-it
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-work-with-blanket-sales-orders"></a><span data-ttu-id="6fb1d-103">Procedura: Utilizzare gli ordini di vendita programmati</span><span class="sxs-lookup"><span data-stu-id="6fb1d-103">How to: Work with Blanket Sales Orders</span></span>
<span data-ttu-id="6fb1d-104">Un ordine di vendita programmato rappresenta la struttura di un accordo a lungo termine fra la società e un cliente.</span><span class="sxs-lookup"><span data-stu-id="6fb1d-104">A blanket sales order represents a framework for a long-term agreement between you and your customer.</span></span>

<span data-ttu-id="6fb1d-105">Un ordine programmato viene in genere creato quando un cliente si impegna ad acquistare grandi quantità che verranno consegnate con diverse spedizioni più piccole effettuate in un determinato periodo di tempo.</span><span class="sxs-lookup"><span data-stu-id="6fb1d-105">A blanket order is typically made when a customer has committed to purchasing large quantities that are to be delivered in several smaller shipments over a certain period of time.</span></span> <span data-ttu-id="6fb1d-106">Gli ordini programmati riguardano spesso un solo articolo con date di consegna predefinite.</span><span class="sxs-lookup"><span data-stu-id="6fb1d-106">Often blanket orders cover only one item with predetermined delivery dates.</span></span> <span data-ttu-id="6fb1d-107">Il motivo principale dell'utilizzo di un ordine programmato anziché di un ordine di vendita consiste nel fatto che le quantità immesse in un ordine programmato non hanno influenza sulla disponibilità dell'articolo e pertanto tali ordini possono essere utilizzati come prospetto per il monitoraggio, le previsioni e le pianificazioni.</span><span class="sxs-lookup"><span data-stu-id="6fb1d-107">The main reason for using a blanket order rather than a sales order is that quantities entered on a blanket order do not affect item availability and thus can be used as a worksheet for monitoring, forecasting, and planning purposes.</span></span>

<span data-ttu-id="6fb1d-108">Nell'ordine programmato ogni singola spedizione può essere impostata come riga di ordine, che è quindi possibile convertire in ordine di vendita al momento della spedizione.</span><span class="sxs-lookup"><span data-stu-id="6fb1d-108">On the blanket order, each separate shipment can be set up as an order line, which can then be converted into a sales order at the time of shipping.</span></span>

<span data-ttu-id="6fb1d-109">È ad esempio possibile utilizzare un ordine di vendita programmato se un cliente ordina 1000 unità di un articolo ma richiede che vengano consegnate 250 unità ogni settimana per tutto il mese seguente.</span><span class="sxs-lookup"><span data-stu-id="6fb1d-109">An example of when a blanket sales order could be used is if a customer calls and places an order of 1000 units of an item and they want the items to be delivered in 250 units every week over the next month.</span></span>

> [!NOTE]
> <span data-ttu-id="6fb1d-110">Gli ordini di acquisto programmati sono simili agli ordini di vendita programmati.</span><span class="sxs-lookup"><span data-stu-id="6fb1d-110">Blanket purchase orders work in a similar way as blanket sales orders.</span></span> <span data-ttu-id="6fb1d-111">In questa documentazione non sono trattati gli ordini di acquisto programmati.</span><span class="sxs-lookup"><span data-stu-id="6fb1d-111">This documentation does not cover blanket purchase orders.</span></span>

## <a name="to-create-a-blanket-sales-order"></a><span data-ttu-id="6fb1d-112">Per creare un ordine di vendita programmato</span><span class="sxs-lookup"><span data-stu-id="6fb1d-112">To create a blanket sales order</span></span>  
1. <span data-ttu-id="6fb1d-113">Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **Ordini di vendita programmati**, quindi scegliere il collegamento correlato.</span><span class="sxs-lookup"><span data-stu-id="6fb1d-113">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Blanket Sales Orders**, and then choose the related link.</span></span>  
2. <span data-ttu-id="6fb1d-114">Scegliere l'azione **Nuovo**.</span><span class="sxs-lookup"><span data-stu-id="6fb1d-114">Choose the **New** action.</span></span>  
3. <span data-ttu-id="6fb1d-115">Compilare i campi, se necessario.</span><span class="sxs-lookup"><span data-stu-id="6fb1d-115">Fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
4.  <span data-ttu-id="6fb1d-116">Lasciare vuoto il campo **Data ordine**.</span><span class="sxs-lookup"><span data-stu-id="6fb1d-116">Leave the **Order Date** field blank.</span></span> <span data-ttu-id="6fb1d-117">Quando vengono creati i diversi ordini di vendita dall'ordine programmato, la data dell'ordine di vendita viene impostata sulla data del lavoro effettiva.</span><span class="sxs-lookup"><span data-stu-id="6fb1d-117">When the separate sales orders are created from the blanket order, the order date of the sales order is set to equal the actual work date.</span></span>
5. <span data-ttu-id="6fb1d-118">Nella Scheda dettaglio **Righe** creare righe separate per ogni spedizione.</span><span class="sxs-lookup"><span data-stu-id="6fb1d-118">On the **Lines** FastTab, create separate lines for each shipment.</span></span> <span data-ttu-id="6fb1d-119">Se, ad esempio, un cliente desidera che 1000 unità vengano divise equamente per quattro settimane, immettere quattro righe separate, ognuna per 250 unità.</span><span class="sxs-lookup"><span data-stu-id="6fb1d-119">For instance, if your customer wants 1000 units split out equally between four weeks, you would enter four separate lines of 250 units each.</span></span>   

## <a name="to-create-a-sales-order-from-a-blanket-sales-order"></a><span data-ttu-id="6fb1d-120">Per creare un ordine di vendita da un ordine di vendita programmato</span><span class="sxs-lookup"><span data-stu-id="6fb1d-120">To create a sales order from a blanket sales order</span></span>  

1.  <span data-ttu-id="6fb1d-121">Per creare un ordine per una delle righe nell'ordine di assemblaggio programmato, rimuovere la quantità dal campo **Qtà da spedire** di tutte le righe che al momento NON si desidera spedire.</span><span class="sxs-lookup"><span data-stu-id="6fb1d-121">To create an order for any of the lines in the blanket assembly order, remove the quantity in the **Qty. to Ship** field on all the lines that you DO NOT wish to ship at this time.</span></span>  
2.  <span data-ttu-id="6fb1d-122">Per creare gli ordini, scegliere l'azione **Crea ordine** e quindi **Sì**.</span><span class="sxs-lookup"><span data-stu-id="6fb1d-122">When you are ready to create orders, choose the **Make Order**m action, and then choose **Yes**.</span></span> <span data-ttu-id="6fb1d-123">Verrà visualizzato un messaggio che informa che all'ordine programmato è stato assegnato un numero di ordine.</span><span class="sxs-lookup"><span data-stu-id="6fb1d-123">A message appears informing you that the blanket order has been assigned an order number.</span></span> <span data-ttu-id="6fb1d-124">Si osservi che l'ordine programmato non è stato eliminato.</span><span class="sxs-lookup"><span data-stu-id="6fb1d-124">Note that the blanket order has not been deleted.</span></span>  
3.  <span data-ttu-id="6fb1d-125">Scegliere il pulsante **OK**.</span><span class="sxs-lookup"><span data-stu-id="6fb1d-125">Choose the **OK** button.</span></span>  
4.  <span data-ttu-id="6fb1d-126">Per visualizzare i risultati dei passaggi precedenti, scegliere l'azione **Riga**, l'azione **Righe non registrate** e l'azione **Ordini**.</span><span class="sxs-lookup"><span data-stu-id="6fb1d-126">To see the results of the preceding steps, choose the **Line** action, choose the **Unposted Lines** action, and then choose the **Orders** action.</span></span>  
5.  <span data-ttu-id="6fb1d-127">Nella finestra **Righe vendita** selezionare l'ordine di vendita appropriato e scegliere l'azione **Riga** e l'azione **Mostra documento**.</span><span class="sxs-lookup"><span data-stu-id="6fb1d-127">In the **Sales Lines** window, select the appropriate sales order, choose the **Line** action, and then choose the **Show Document** action.</span></span>  

<span data-ttu-id="6fb1d-128">Quanto segue si applica agli ordini di vendita creati da ordini di vendita programmati:</span><span class="sxs-lookup"><span data-stu-id="6fb1d-128">The following applies to sales orders after they have been created from blanket sales orders:</span></span>  

- <span data-ttu-id="6fb1d-129">Dopo la conversione dell'ordine programmato in un ordine di vendita, l'ordine di vendita contiene tutte le righe dell'ordine programmato.</span><span class="sxs-lookup"><span data-stu-id="6fb1d-129">After the blanket order is converted into a sales order, the sales order contains all the lines from the blanket order.</span></span> <span data-ttu-id="6fb1d-130">Le righe in cui la quantità indicata nel campo **Qtà da spedire** è stata eliminata vengono visualizzate, ma il relativo campo **Quantità** è vuoto.</span><span class="sxs-lookup"><span data-stu-id="6fb1d-130">The lines where the quantity in the **Qty. to Ship** field was deleted appear, but with blank **Quantity** fields.</span></span> <span data-ttu-id="6fb1d-131">È possibile mantenere queste righe, modificarle o eliminarle.</span><span class="sxs-lookup"><span data-stu-id="6fb1d-131">You may choose to leave, edit, or delete the lines.</span></span>  
- <span data-ttu-id="6fb1d-132">È importante ricordare che la quantità della riga dell'ordine di vendita non deve essere superiore alla quantità associata alla riga dell'ordine programmato.</span><span class="sxs-lookup"><span data-stu-id="6fb1d-132">It is important to remember that the sales order line quantity must not exceed the quantity of the associated blanket order line.</span></span> <span data-ttu-id="6fb1d-133">In caso contrario, non sarà possibile registrare l'ordine di vendita.</span><span class="sxs-lookup"><span data-stu-id="6fb1d-133">Otherwise, posting of the sales order will not be possible.</span></span>  
- <span data-ttu-id="6fb1d-134">Quando l'ordine di vendita viene registrato come spedito e/o fatturato, i campi **Quantità spedita** e **Quantità fatturata** vengono aggiornati nell'ordine programmato correlato.</span><span class="sxs-lookup"><span data-stu-id="6fb1d-134">When the sales order is posted as shipped and/or invoiced, the **Quantity Shipped** and **Quantity Invoiced** fields are updated on the related blanket order.</span></span>  
- <span data-ttu-id="6fb1d-135">Quando l'ordine viene creato da un ordine programmato, il numero dell'ordine programmato e il numero di riga vengono registrati come proprietà delle righe di vendita.</span><span class="sxs-lookup"><span data-stu-id="6fb1d-135">The blanket order number and line number are recorded as properties of the sales lines when created from a blanket order.</span></span>  
- <span data-ttu-id="6fb1d-136">Quando gli ordini di vendita non vengono creati direttamente dall'ordine programmato, ma sono comunque correlati a esso, è possibile creare un collegamento tra un ordine di vendita e un ordine programmato immettendo il numero dell'ordine programmato associato nel campo **Nr. ordine programmato**</span><span class="sxs-lookup"><span data-stu-id="6fb1d-136">When sales orders are not created directly from the blanket order but still relate to it, a link between a sales order and a blanket order can be established by entering the associated blanket order number in the **Blanket Order No.**</span></span> <span data-ttu-id="6fb1d-137">nella riga dell'ordine di vendita.</span><span class="sxs-lookup"><span data-stu-id="6fb1d-137">field on the sales order line.</span></span>  
- <span data-ttu-id="6fb1d-138">Dopo avere creato un ordine di vendita per la quantità totale di una riga di ordine programmato, non è possibile creare altri ordini di vendita per la stessa riga.</span><span class="sxs-lookup"><span data-stu-id="6fb1d-138">After the sales order has been created for the total quantity of a blanket order line, no other sales order can be created for the same line.</span></span> <span data-ttu-id="6fb1d-139">Agli utenti non è consentito immettere una quantità nel campo **Qtà da spedire**.</span><span class="sxs-lookup"><span data-stu-id="6fb1d-139">Users are prevented from entering a quantity in the **Qty. to Ship** field.</span></span> <span data-ttu-id="6fb1d-140">Se, tuttavia, è necessario aggiungere ulteriori quantità a un ordine programmato, è possibile aumentare il valore del campo **Quantità**, quindi creare ulteriori ordini.</span><span class="sxs-lookup"><span data-stu-id="6fb1d-140">If, however, additional quantities need to be added to a blanket order, the value in the **Quantity** field can be increased and additional orders can then be created.</span></span>  
- <span data-ttu-id="6fb1d-141">L'ordine di vendita programmato fatturato rimane nel sistema fino a quando non viene eliminato, eliminando i singoli ordini programmati o eseguendo il processo batch **Elimina ord. ven. progr. fatt.**.</span><span class="sxs-lookup"><span data-stu-id="6fb1d-141">The invoiced blanket sales order remains in the system until it is deleted, either by deleting individual blanket orders or by running the **Delete Invoiced Blanket Sales Orders** batch job.</span></span>  
- <span data-ttu-id="6fb1d-142">Se un cliente è anche registrato come contatto nell'area di applicazione Marketing ed è stato specificato un codice modello di interazione per l'ordine di vendita programmato nella finestra **Setup marketing**, viene registrata un'interazione nella tabella Mov. log interazione quando si seleziona **Stampa** per stampare l'ordine di vendita programmato.</span><span class="sxs-lookup"><span data-stu-id="6fb1d-142">If a customer is also recorded as a contact in the Marketing application area, and if you have specified an interaction template code for blanket sales order in the **Marketing Setup** window, an interaction is recorded in the Interaction Log Entry table when you select **Print** to print the blanket sales order.</span></span>

## <a name="to-view-the-status-of-a-blanket-purchase-order"></a><span data-ttu-id="6fb1d-143">Per visualizzare lo stato di un ordine di acquisto programmato</span><span class="sxs-lookup"><span data-stu-id="6fb1d-143">To view the status of a blanket purchase order</span></span>  
<span data-ttu-id="6fb1d-144">È possibile visualizzare lo stato di un ordine di vendita programmato nella finestra **Statistiche Ordine Acquisto programmato**.</span><span class="sxs-lookup"><span data-stu-id="6fb1d-144">You can see the status of a blanket sales order in the **Purchase Blanket Order Statistics** window.</span></span> <span data-ttu-id="6fb1d-145">Ciò può risultare utile quando si avvia la fatturazione dell'ordine creato dall'ordine di acquisto programmato.</span><span class="sxs-lookup"><span data-stu-id="6fb1d-145">This may be relevant when you start to invoice the order that is created from the blanket purchase order.</span></span>  

1.  <span data-ttu-id="6fb1d-146">Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **Ordini di vendita programmati**, quindi scegliere il collegamento correlato.</span><span class="sxs-lookup"><span data-stu-id="6fb1d-146">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Blanket Purchase Orders**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="6fb1d-147">Selezionare un ordine di acquisto programmato quindi scegliere l'azione **Statistiche**.</span><span class="sxs-lookup"><span data-stu-id="6fb1d-147">Select a blanket purchase order, and then choose the **Statistics** action.</span></span>  
3.  <span data-ttu-id="6fb1d-148">Nella finestra **Statistiche ordine acquisto programmato**, nella Scheda dettaglio **Generale**, è possibile visualizzare le informazioni di riepilogo relative all'intero ordine in base alla quantità totale riportata nei vari **campi Quantità** delle righe dell'ordine di acquisto programmato.</span><span class="sxs-lookup"><span data-stu-id="6fb1d-148">In the **Purchase Blanket Order Statistics** window, on the **General** FastTab, you can see summary information about the entire order based on the total quantity in the various **Quantity fields** on the blanket purchase order lines.</span></span>  

    - <span data-ttu-id="6fb1d-149">Nella Scheda dettaglio **Fatturazione** è possibile visualizzare le informazioni di riepilogo in base alla quantità totale riportata nei campi **Qtà da fatturare** delle righe dell'ordine di acquisto programmato.</span><span class="sxs-lookup"><span data-stu-id="6fb1d-149">On the **Invoicing** FastTab, you can see summary information based on the total quantity in the **Qty. to Invoice** fields on the purchase blanket order lines.</span></span>  
    - <span data-ttu-id="6fb1d-150">Nella Scheda dettaglio **Spedizione** è possibile visualizzare le informazioni di riepilogo in base alla quantità totale riportata nei campi **Qtà da ricevere** delle righe dell'ordine di acquisto programmato.</span><span class="sxs-lookup"><span data-stu-id="6fb1d-150">On the **Shipping** FastTab, you can see summary information based on the total quantity in the **Qty. to Receive** fields on the purchase blanket order lines.</span></span>  
    - <span data-ttu-id="6fb1d-151">Nella Scheda dettaglio **Pagamento anticipato** è possibile visualizzare informazioni di riepilogo relative agli importi prepagati.</span><span class="sxs-lookup"><span data-stu-id="6fb1d-151">On the **Prepayment** FastTab, you can see summary information about any prepaid amounts.</span></span>  
    - <span data-ttu-id="6fb1d-152">Nella Scheda dettaglio **Fornitore** è possibile visualizzare le informazioni principali relative al fornitore.</span><span class="sxs-lookup"><span data-stu-id="6fb1d-152">On the **Vendor** FastTab, you can see certain basic information about the vendor.</span></span>    

## <a name="to-view-unposted-and-posted-blanket-sales-order-lines"></a><span data-ttu-id="6fb1d-153">Pere visualizzare le righe degli ordini di vendita programmati registrate e non registrate</span><span class="sxs-lookup"><span data-stu-id="6fb1d-153">To view unposted and posted blanket sales order lines</span></span>   
<span data-ttu-id="6fb1d-154">Il collegamento tra l'ordine di vendita programmato e l'ordine di vendita di origine ed eventuali altri documenti di vendita, viene mantenuto dopo la registrazione come lista delle righe della fattura di vendita registrate e non registrate.</span><span class="sxs-lookup"><span data-stu-id="6fb1d-154">The link between the blanket sales order and the originating sales order, and any other sales document, is retained after posting as a list of posted and unposted sales order invoice lines.</span></span>  

1. <span data-ttu-id="6fb1d-155">Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **Ordini di vendita programmati**, quindi scegliere il collegamento correlato.</span><span class="sxs-lookup"><span data-stu-id="6fb1d-155">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon enter **Blanket Sales Orders**, and then choose the related link.</span></span>
2. <span data-ttu-id="6fb1d-156">Aprire l'ordine di vendita programmato che si desidera visualizzare.</span><span class="sxs-lookup"><span data-stu-id="6fb1d-156">Open the blanket sales order you want to view.</span></span>
3. <span data-ttu-id="6fb1d-157">Per visualizzare i movimenti non registrati, selezionare la riga in questione, quindi scegliere l'azione **Riga** e l'azione **Righe non registrate**.</span><span class="sxs-lookup"><span data-stu-id="6fb1d-157">To view unposted entries, select the line in question, choose the **Line** action, and then choose the **Unposted Lines** action.</span></span> <span data-ttu-id="6fb1d-158">Selezionare una delle seguenti opzioni.</span><span class="sxs-lookup"><span data-stu-id="6fb1d-158">Choose one of the following options.</span></span>  

    <table>
    <tr>
    <th><span data-ttu-id="6fb1d-159">Opzione</span><span class="sxs-lookup"><span data-stu-id="6fb1d-159">Option</span></span></th>
    <th><span data-ttu-id="6fb1d-160">Description</span><span class="sxs-lookup"><span data-stu-id="6fb1d-160">Description</span></span></th>
    </tr>
    <tr>
    <td><span data-ttu-id="6fb1d-161">**Ordini**</span><span class="sxs-lookup"><span data-stu-id="6fb1d-161">**Orders**</span></span></td>
    <td><span data-ttu-id="6fb1d-162">Specifica ordini aperti associati alla riga selezionata.</span><span class="sxs-lookup"><span data-stu-id="6fb1d-162">Specifies open orders associated with the selected line.</span></span></td>
    </tr>
    <tr>
    <td><span data-ttu-id="6fb1d-163">**Fatture**</span><span class="sxs-lookup"><span data-stu-id="6fb1d-163">**Invoices**</span></span></td>
    <td><span data-ttu-id="6fb1d-164">Specifica fatture aperte associate alla riga selezionata.</span><span class="sxs-lookup"><span data-stu-id="6fb1d-164">Specifies open invoices that have been associated with the selected line.</span></span> <span data-ttu-id="6fb1d-165">È possibile associare manualmente le fatture aperte a un ordine programmato immettendo il numero dell'ordine programmato nella riga della fattura di vendita.</span><span class="sxs-lookup"><span data-stu-id="6fb1d-165">Open invoices are manually associated with a blanket order by entering the blanket order number on the sales invoice line.</span></span></td>
    </tr>
    <tr>
    <td><span data-ttu-id="6fb1d-166">**Ordini di reso**</span><span class="sxs-lookup"><span data-stu-id="6fb1d-166">**Return Orders**</span></span></td>
    <td><span data-ttu-id="6fb1d-167">Specifica ordini di reso aperti associati alla riga selezionata.</span><span class="sxs-lookup"><span data-stu-id="6fb1d-167">Specifies open return orders that have been associated with the selected line.</span></span></td>
    </tr>
    <tr>
    <td><span data-ttu-id="6fb1d-168">**Note di credito**</span><span class="sxs-lookup"><span data-stu-id="6fb1d-168">**Credit Memos**</span></span></td>
    <td><span data-ttu-id="6fb1d-169">Specifica note di credito aperte associate alla riga selezionata.</span><span class="sxs-lookup"><span data-stu-id="6fb1d-169">Specifies open credit memos that have been associated with the selected line.</span></span></td>
    </tr>
    </table><span data-ttu-id="6fb1d-170">
4. Per visualizzare i movimenti registrati, selezionare la riga in questione, quindi scegliere l'azione **Riga** e l'azione **Righe registrate**.</span><span class="sxs-lookup"><span data-stu-id="6fb1d-170">
4. To view posted entries, select the line in question, choose the **Line** action, and then choose the **Posted Lines** action.</span></span> <span data-ttu-id="6fb1d-171">Selezionare una delle seguenti opzioni.</span><span class="sxs-lookup"><span data-stu-id="6fb1d-171">Choose one of the following options.</span></span>  

    <table>
    <tr>
    <th><span data-ttu-id="6fb1d-172">Opzione</span><span class="sxs-lookup"><span data-stu-id="6fb1d-172">Option</span></span></th>
    <th><span data-ttu-id="6fb1d-173">Description</span><span class="sxs-lookup"><span data-stu-id="6fb1d-173">Description</span></span></th>
    </tr>
    <tr>
    <td><span data-ttu-id="6fb1d-174">**Spedizioni**</span><span class="sxs-lookup"><span data-stu-id="6fb1d-174">**Shipments**</span></span></td>
    <td><span data-ttu-id="6fb1d-175">spedizioni registrate associate alla riga selezionata.</span><span class="sxs-lookup"><span data-stu-id="6fb1d-175">Posted shipments associated with the selected line.</span></span></td>
    </tr>
    <tr>
    <td><span data-ttu-id="6fb1d-176">**Fatture**</span><span class="sxs-lookup"><span data-stu-id="6fb1d-176">**Invoices**</span></span></td>
    <td><span data-ttu-id="6fb1d-177">fatture registrate associate alla riga selezionata.</span><span class="sxs-lookup"><span data-stu-id="6fb1d-177">Posted invoices associated with the selected line.</span></span></td>
    </tr>
    <tr>
    <td><span data-ttu-id="6fb1d-178">**Carichi da reso**</span><span class="sxs-lookup"><span data-stu-id="6fb1d-178">**Return Receipts**</span></span></td>
    <td><span data-ttu-id="6fb1d-179">carichi da reso registrati associati alla riga selezionata.</span><span class="sxs-lookup"><span data-stu-id="6fb1d-179">Posted return receipts that have been associated with the selected line.</span></span></td>
    </tr>
    <tr>
    <td><span data-ttu-id="6fb1d-180">**Note di credito**</span><span class="sxs-lookup"><span data-stu-id="6fb1d-180">**Credit Memos**</span></span></td>
    <td><span data-ttu-id="6fb1d-181">note di credito registrate associate alla riga selezionata.</span><span class="sxs-lookup"><span data-stu-id="6fb1d-181">Posted credit memos that have been associated with the selected line.</span></span></td>
    </tr>
    </table><span data-ttu-id="6fb1d-182">
5. Nella finestra **Righe acquisto** scegliere l'azione **Mostra documento** per visualizzare il movimento.</span><span class="sxs-lookup"><span data-stu-id="6fb1d-182">
5. In the **Sales Lines** window, choose the **Show Document** action to view the entry.</span></span>

## <a name="see-also"></a><span data-ttu-id="6fb1d-183">Vedi anche</span><span class="sxs-lookup"><span data-stu-id="6fb1d-183">See Also</span></span>
[<span data-ttu-id="6fb1d-184">Vendite</span><span class="sxs-lookup"><span data-stu-id="6fb1d-184">Sales</span></span>](sales-manage-sales.md)  
[<span data-ttu-id="6fb1d-185">Setup Vendite</span><span class="sxs-lookup"><span data-stu-id="6fb1d-185">Setting Up Sales</span></span>](sales-setup-sales.md)  
<span data-ttu-id="6fb1d-186">[Utilizzo di [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="6fb1d-186">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
