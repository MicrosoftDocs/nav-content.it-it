---
title: 'Procedura: Effettuare spedizioni dirette'
author: SorenGP
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 6b60b1344a1e18ad91863046110df880f75f7c04
ms.openlocfilehash: a726c8c24d8f843b33b4df4d85ad2b5eab3790e7
ms.contentlocale: it-it
ms.lasthandoff: 07/19/2017

---

# <a name="how-to-make-drop-shipments"></a><span data-ttu-id="7573f-102">Procedura: Effettuare spedizioni dirette</span><span class="sxs-lookup"><span data-stu-id="7573f-102">How to: Make Drop Shipments</span></span>
<span data-ttu-id="7573f-103">Una spedizione diretta è costituita dalla spedizione di articoli direttamente da un fornitore a un cliente.</span><span class="sxs-lookup"><span data-stu-id="7573f-103">A drop shipment is the shipment of items from one of your vendors directly to one of your customers.</span></span>

<span data-ttu-id="7573f-104">Quando un ordine di vendita è contrassegnato per la spedizione diretta e si crea un ordine di acquisto specificando il cliente nel campo **Vendere a - Nr. cliente**,</span><span class="sxs-lookup"><span data-stu-id="7573f-104">When a sales order is marked for drop shipment, and you create a purchase order specifying the customer in the **Sell-to Customer No.**</span></span> <span data-ttu-id="7573f-105">è possibile collegare due documenti e istruire il fornitore di spedire direttamente al cliente.</span><span class="sxs-lookup"><span data-stu-id="7573f-105">field, then you can link the two documents and thereby instruct the vendor to ship directly to the customer.</span></span>

## <a name="to-create-a-sales-order-for-drop-shipment"></a><span data-ttu-id="7573f-106">Per creare un ordine di vendita per una spedizione diretta</span><span class="sxs-lookup"><span data-stu-id="7573f-106">To create a sales order for drop shipment</span></span>
<span data-ttu-id="7573f-107">Per preparare una spedizione diretta, si crea un ordine di vendita per un articolo come al solito, ad eccezione del fatto che è necessario indicare sulla riga di vendita che la vendita richiede la spedizione diretta.</span><span class="sxs-lookup"><span data-stu-id="7573f-107">To prepare a drop shipment, you create a sales order for an item as normal, except you must indicate on the sales line that the sale requires drop shipment.</span></span>

1. <span data-ttu-id="7573f-108">Creare un ordine cliente per un articolo.</span><span class="sxs-lookup"><span data-stu-id="7573f-108">Create a sales order for an item.</span></span> <span data-ttu-id="7573f-109">Per ulteriori informazioni, vedere [Procedura: Vendere prodotti](sales-how-sell-products.md).</span><span class="sxs-lookup"><span data-stu-id="7573f-109">For more information, see [How to: Sell Products](sales-how-sell-products.md).</span></span>
2. <span data-ttu-id="7573f-110">Nella riga ordine di vendita dell'articolo con spedizione diretta, selezionare la casella di controllo **Spedizione diretta**.</span><span class="sxs-lookup"><span data-stu-id="7573f-110">On the sales order line for the drop-shipment item, select the **Drop Shipment** check box.</span></span>

## <a name="to-create-the-purchase-order-for-drop-shipment"></a><span data-ttu-id="7573f-111">Per creare l'ordine di acquisto per la spedizione diretta</span><span class="sxs-lookup"><span data-stu-id="7573f-111">To create the purchase order for drop shipment</span></span>
<span data-ttu-id="7573f-112">Per preparare una spedizione diretta per l'articolo da vendere, si crea un ordine di acquisto come al solito, ad eccezione del fatto che è necessario indicare nell'ordine di acquisto che deve essere spedito al cliente e non a se stessi.</span><span class="sxs-lookup"><span data-stu-id="7573f-112">To prepare a drop shipment for the item to be sold, you create a purchase order as normal, except you must indicate on the purchase order that it must be shipped to your customer, not to yourself.</span></span>

1. <span data-ttu-id="7573f-113">Creare un ordine di acquisto.</span><span class="sxs-lookup"><span data-stu-id="7573f-113">Create a purchase order.</span></span> <span data-ttu-id="7573f-114">Non compilare i campi nelle righe.</span><span class="sxs-lookup"><span data-stu-id="7573f-114">Do not fill any fields on the lines.</span></span> <span data-ttu-id="7573f-115">Per ulteriori informazioni, vedere [Procedura: Registrare gli acquisti](purchasing-how-record-purchases.md).</span><span class="sxs-lookup"><span data-stu-id="7573f-115">For more information, see [How to: Record Purchases](purchasing-how-record-purchases.md).</span></span>
2. <span data-ttu-id="7573f-116">Nel campo **Vendere a - Nr. cliente**</span><span class="sxs-lookup"><span data-stu-id="7573f-116">In the **Sell-to Customer No.**</span></span> <span data-ttu-id="7573f-117">selezionare il cliente a cui si sta vendendo.</span><span class="sxs-lookup"><span data-stu-id="7573f-117">field, select the customer that you are selling to.</span></span>
3. <span data-ttu-id="7573f-118">Scegliere l'azione **Spedizioni dirette** e scegliere l'azione **Ottieni ordini vendite**.</span><span class="sxs-lookup"><span data-stu-id="7573f-118">Choose the **Drop Shipments** action, and then choose the **Get Sales Order** action.</span></span>
4. <span data-ttu-id="7573f-119">Nella finestra **Lista vendite**, selezionare l'ordine di vendita che è stato preparato nella sezione "Per creare un ordine di vendita per una spedizione diretta".</span><span class="sxs-lookup"><span data-stu-id="7573f-119">In the **Sales List** window, select the sales order that you prepared in the "To create a sales order for drop shipment" section.</span></span>
5. <span data-ttu-id="7573f-120">Scegliere il pulsante **OK**.</span><span class="sxs-lookup"><span data-stu-id="7573f-120">Choose the **OK** button.</span></span>

<span data-ttu-id="7573f-121">Le informazioni di riga dall'ordine di vendita vengono inserite nelle righe dell'ordine di acquisto.</span><span class="sxs-lookup"><span data-stu-id="7573f-121">The line information from the sales order is inserted on the purchase order line(s).</span></span>

<span data-ttu-id="7573f-122">È possibile istruire il fornitore di spedire gli articoli al cliente, ad esempio spedendo l'ordine di acquisto come PDF.</span><span class="sxs-lookup"><span data-stu-id="7573f-122">You can now instruct the vendor to ship the items to your customer, for example, by mailing the purchase order as a PDF.</span></span>     

## <a name="to-view-the-linked-purchase-order-from-the-sales-order"></a><span data-ttu-id="7573f-123">Per visualizzare l'ordine di acquisto collegato dall'ordine di vendita</span><span class="sxs-lookup"><span data-stu-id="7573f-123">To view the linked purchase order from the sales order</span></span>
1. <span data-ttu-id="7573f-124">Selezionare la riga dell'ordine di vendita con spedizione diretta, scegliere l'azione **Ordine**, scegliere l'azione **Spedizione diretta** e quindi scegliere l'azione **Ordine acquisto**.</span><span class="sxs-lookup"><span data-stu-id="7573f-124">Select the drop-shipment sales order line, choose the **Order** action, choose the **Drop Shipment** action, and then choose the **Purchase Order** action.</span></span>

<span data-ttu-id="7573f-125">L'ordine di acquisto collegato viene aperto.</span><span class="sxs-lookup"><span data-stu-id="7573f-125">The linked purchase order opens.</span></span>

## <a name="to-post-a-drop-shipment"></a><span data-ttu-id="7573f-126">Per registrare una spedizione diretta</span><span class="sxs-lookup"><span data-stu-id="7573f-126">To post a drop shipment</span></span>
<span data-ttu-id="7573f-127">Quando il fornitore ha spedito gli articoli, è possibile registrare l'ordine di vendita come spedito.</span><span class="sxs-lookup"><span data-stu-id="7573f-127">When the vendor has shipped the items, you can post the sales order as shipped.</span></span> <span data-ttu-id="7573f-128">È possibile registrare anche l'ordine di acquisto, ma solo con l'opzione **Ricevi** finché l'ordine di vendita non viene fatturato.</span><span class="sxs-lookup"><span data-stu-id="7573f-128">You can also post the purchase order, but only with the **Receive** option until the sales order has been invoiced.</span></span>
1. <span data-ttu-id="7573f-129">Nell'angolo superiore destro, scegliere l'icona **Cerca pagina o report**, immettere **Ordini di vendita**, quindi scegliere il collegamento correlato.</span><span class="sxs-lookup"><span data-stu-id="7573f-129">In the top right corner, choose the **Search for Page or Report** icon, enter **Sales orders**, and then choose the related link.</span></span>
2. <span data-ttu-id="7573f-130">Aprire l'ordine di vendita creato nella sezione "Per creare un ordine di vendita per una spedizione diretta".</span><span class="sxs-lookup"><span data-stu-id="7573f-130">Open the sales order that you created in the "To create a sales order for a drop shipment" section.</span></span>
3. <span data-ttu-id="7573f-131">Nel campo **Qtà da spedire**, specificare la quantità dell'ordine da spedire, la quantità dell'ordine completa o parziale.</span><span class="sxs-lookup"><span data-stu-id="7573f-131">In the **Qty. to Ship** field, specify how many of the order quantity to ship, the full or a partial order quantity.</span></span>
3. <span data-ttu-id="7573f-132">Scegliere l'azione **Registra** o **Registra e invia**.</span><span class="sxs-lookup"><span data-stu-id="7573f-132">Choose the **Post** or **Post and Send** action.</span></span>
4. <span data-ttu-id="7573f-133">Selezionare l'opzione **Spedizione** per fatturare in seguito oppure l'opzione **Spedisci e fattura** per fatturare immediatamente.</span><span class="sxs-lookup"><span data-stu-id="7573f-133">Choose either the **Ship** option to invoice later, or the **Ship and Invoice** option to invoice immediately.</span></span>

## <a name="see-also"></a><span data-ttu-id="7573f-134">Vedi anche</span><span class="sxs-lookup"><span data-stu-id="7573f-134">See Also</span></span>
<span data-ttu-id="7573f-135">[Procedura: vendere prodotti](sales-how-sell-products.md)  </span><span class="sxs-lookup"><span data-stu-id="7573f-135">[How to: Sell Products](sales-how-sell-products.md)  </span></span>  
[<span data-ttu-id="7573f-136">Procedura: Registrare gli acquisti</span><span class="sxs-lookup"><span data-stu-id="7573f-136">How to: Record Purchases</span></span>](purchasing-how-record-purchases.md)  
[<span data-ttu-id="7573f-137">Gestire le vendite</span><span class="sxs-lookup"><span data-stu-id="7573f-137">Manage Sales</span></span>](sales-manage-sales.md)  
<span data-ttu-id="7573f-138">[Gestire i costi del magazzino](inventory-manage-inventory.md)    </span><span class="sxs-lookup"><span data-stu-id="7573f-138">[Manage Inventory](inventory-manage-inventory.md)    </span></span>  
[<span data-ttu-id="7573f-139">Utilizzare Dynamics NAV</span><span class="sxs-lookup"><span data-stu-id="7573f-139">Work with Dynamics NAV</span></span>](ui-work-product.md)

