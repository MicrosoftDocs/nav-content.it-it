---
title: 'Procedura: Abilitare i pagamenti clienti attraverso PayPal'
author: SorenGP
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2017
ms.translationtype: HT
ms.sourcegitcommit: 6b60b1344a1e18ad91863046110df880f75f7c04
ms.openlocfilehash: 15f30a03c3e7ccc865ef527a707794c2c6428b2f
ms.contentlocale: it-it
ms.lasthandoff: 10/16/2017

---

# <a name="how-to-enable-customer-payments-through-paypal"></a><span data-ttu-id="28487-102">Procedura: Abilitare i pagamenti clienti attraverso PayPal#</span><span class="sxs-lookup"><span data-stu-id="28487-102">How to: Enable Customer Payments Through PayPal#</span></span>
<span data-ttu-id="28487-103">Come alternativa alla riscossione dei pagamenti tramite bonifico o carte di credito, è possibile offrire ai clienti di pagare tramite il conto PayPal.</span><span class="sxs-lookup"><span data-stu-id="28487-103">As an alternative to collecting payments through bank transfer or credit cards, you can offer your customers to pay you through their PayPal account.</span></span>

<span data-ttu-id="28487-104">Quando un cliente sceglie il collegamento a PayPal in una fattura di vendita o in un documento ordine di vendita, viene visualizzata la pagina di assistenza per il conto PayPal nella quale sono disponibili i dettagli di pagamento per la vendita.</span><span class="sxs-lookup"><span data-stu-id="28487-104">When a customer chooses the PayPal link on a sales invoice or sales order document, the service page for their PayPal account appears showing the payment details for the sale.</span></span> <span data-ttu-id="28487-105">Il cliente può quindi pagare la fattura con la stessa modalità di un qualsiasi altro pagamento PayPal.</span><span class="sxs-lookup"><span data-stu-id="28487-105">The customer can then pay the invoice as any other PayPal payment.</span></span>

<span data-ttu-id="28487-106">Per abilitare i pagamenti dei clienti attraverso PayPal, è necessario attenersi alla seguente procedura:</span><span class="sxs-lookup"><span data-stu-id="28487-106">To enable customer payments through PayPal, you must do the following:</span></span>

1. <span data-ttu-id="28487-107">Impostare PayPal Payments Standard come servizio di pagamento nella finestra **Servizi di pagamento**.</span><span class="sxs-lookup"><span data-stu-id="28487-107">Set up PayPal Payments Standard as a payment service in the **Payments Services** window.</span></span>
2. <span data-ttu-id="28487-108">Selezionare PayPal Payments Standard nel campo **Servizio di pagamento** nel documento di vendita in questione.</span><span class="sxs-lookup"><span data-stu-id="28487-108">Select PayPal Payments Standard in the **Payment Service** field on the sales document in question.</span></span>

<span data-ttu-id="28487-109">Il servizio PayPal Payments Standard verrà installato come estensione di Dynamics NAV e sarà pronto per essere abilitato.</span><span class="sxs-lookup"><span data-stu-id="28487-109">The PayPal Payments Standard service is installed as an extension to Dynamics NAV and ready to enabled.</span></span> <span data-ttu-id="28487-110">Per maggiori informazioni, vedere [Personalizzazione di Dynamics NAV utilizzando le estensioni](ui-extensions.md).</span><span class="sxs-lookup"><span data-stu-id="28487-110">For more information, see [Customizing Dynamics NAV Using Extensions ](ui-extensions.md).</span></span>

## <a name="to-enable-the-paypal-payments-standard-service"></a><span data-ttu-id="28487-111">Per abilitare il servizio PayPal Payments Standard</span><span class="sxs-lookup"><span data-stu-id="28487-111">To enable the PayPal Payments Standard service</span></span>
1. <span data-ttu-id="28487-112">Nell'angolo superiore destro, scegliere l'icona **Cerca pagina o report**, immettere **Servizi di pagamento**, quindi scegliere il collegamento correlato.</span><span class="sxs-lookup"><span data-stu-id="28487-112">In the top right corner, choose the **Search for Page or Report** icon, **Payment Services**, and then choose the related link.</span></span>  
2. <span data-ttu-id="28487-113">Nella finestra **Servizi di pagamento** scegliere l'azione **Nuovo**.</span><span class="sxs-lookup"><span data-stu-id="28487-113">In the **Payment Services** window, choose the **New** action.</span></span>
3. <span data-ttu-id="28487-114">Selezionare **PayPal Standard**, quindi chiudere la finestra.</span><span class="sxs-lookup"><span data-stu-id="28487-114">Select **PayPal Standard**, and then close the window.</span></span>
4. <span data-ttu-id="28487-115">Nella finestra **Servizi di pagamento** scegliere l'azione **Setup**.</span><span class="sxs-lookup"><span data-stu-id="28487-115">In the **Payment Services** window, choose the **Setup** action.</span></span>
5. <span data-ttu-id="28487-116">Compilare i campi, se necessario.</span><span class="sxs-lookup"><span data-stu-id="28487-116">Fill in the fields as necessary.</span></span> <span data-ttu-id="28487-117">Selezionare il campo per visualizzare una breve descrizione del campo o il collegamento a ulteriori informazioni.</span><span class="sxs-lookup"><span data-stu-id="28487-117">Choose a field to read a short description of the field or link to more information.</span></span>

    <span data-ttu-id="28487-118">**Nota**: selezionare la casella di controllo **Includi sempre in documenti** se il collegamento ipertestuale per il servizio di pagamento PayPal deve essere sempre visibile nei documenti di vendita laddove il pagamento tramite PayPal è abilitato.</span><span class="sxs-lookup"><span data-stu-id="28487-118">**Note**: Select the **Always Include on Documents** check box if the hyperlink for the PayPal payment service should always be visible on sales documents where payment through PayPal is enabled.</span></span>

6. <span data-ttu-id="28487-119">Chiudere la finestra.</span><span class="sxs-lookup"><span data-stu-id="28487-119">Close the window.</span></span>

## <a name="to-select-paypal-payments-standard-on-a-sales-invoice"></a><span data-ttu-id="28487-120">Per selezionare PayPal Payments Standard in una fattura di vendita</span><span class="sxs-lookup"><span data-stu-id="28487-120">To select PayPal Payments Standard on a sales invoice</span></span>
1. <span data-ttu-id="28487-121">Nella home page scegliere **Fatture vendite**.</span><span class="sxs-lookup"><span data-stu-id="28487-121">On the Home page, choose **Sales Invoices**.</span></span>
2. <span data-ttu-id="28487-122">Aprire la fattura di vendita per cui si desidera abilitare i pagamenti tramite PayPal.</span><span class="sxs-lookup"><span data-stu-id="28487-122">Open the sales invoice that you want to enable PayPal payments for.</span></span>
3. <span data-ttu-id="28487-123">Nel campo **Servizio di pagamento** scegliere PayPal Payments Standard.</span><span class="sxs-lookup"><span data-stu-id="28487-123">In the **Payment Service** field, choose PayPal Payments Standard.</span></span>

<span data-ttu-id="28487-124">**Nota**: il campo **Servizio di pagamento** è visibile solo se il servizio PayPal Payments Standard è abilitato.</span><span class="sxs-lookup"><span data-stu-id="28487-124">**Note**: The **Payment Service** field is only visible if the PayPal Payments Standard service is enabled.</span></span>   

## <a name="see-also"></a><span data-ttu-id="28487-125">Vedi anche</span><span class="sxs-lookup"><span data-stu-id="28487-125">See Also</span></span>  
[<span data-ttu-id="28487-126">Impostare le vendite</span><span class="sxs-lookup"><span data-stu-id="28487-126">Set Up Sales</span></span>](sales-setup-sales.md)  
[<span data-ttu-id="28487-127">Gestire le vendite</span><span class="sxs-lookup"><span data-stu-id="28487-127">Manage Sales</span></span>](sales-manage-sales.md)  
[<span data-ttu-id="28487-128">Personalizzazione di Dynamics NAV utilizzando le estensioni</span><span class="sxs-lookup"><span data-stu-id="28487-128">Customizing Dynamics NAV Using Extensions</span></span>](ui-extensions.md)

