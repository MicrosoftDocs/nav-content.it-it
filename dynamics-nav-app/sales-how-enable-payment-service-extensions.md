---
title: Abilitare i pagamenti clienti tramite i servizi di pagamento
description: Facilitare ai clienti il pagamento delle fatture abilitando i servizi di pagamento.
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: online payment
ms.date: 07/07/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 71ff4af2fa3c0d1020a24de4325aafe17978f715
ms.contentlocale: it-it
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-enable-customer-payments-through-payment-services"></a><span data-ttu-id="04d07-103">Procedura: Abilitare i pagamenti clienti tramite i servizi di pagamento</span><span class="sxs-lookup"><span data-stu-id="04d07-103">How to: Enable Customer Payments Through Payment Services</span></span>
<span data-ttu-id="04d07-104">Come alternativa alla riscossione dei pagamenti tramite bonifico o carte di credito, i clienti possono pagare utilizzando il conto personale e servizi di pagamento, quali Microsoft Pay, PayPal o WorldPay.</span><span class="sxs-lookup"><span data-stu-id="04d07-104">As an alternative to collecting payments through bank transfer or credit cards, your customers can pay you through their account with payment services, such as Microsoft Pay, PayPal, or WorldPay.</span></span>  

<span data-ttu-id="04d07-105">Dopo che viene abilitato un servizio di pagamento in [!INCLUDE[d365fin](includes/d365fin_md.md)], un collegamento all'assistenza è disponibile nei documenti di vendita inviati tramite e-mail ai clienti.</span><span class="sxs-lookup"><span data-stu-id="04d07-105">After you enable a payment service in [!INCLUDE[d365fin](includes/d365fin_md.md)], a link to the service is available on sales documents that you send by email to your customers.</span></span> <span data-ttu-id="04d07-106">I clienti possono utilizzare il collegamento per andare al servizio di pagamento e per pagare la fattura, direttamente dal documento di vendita.</span><span class="sxs-lookup"><span data-stu-id="04d07-106">Customers can use the link to go to the payment service and pay the bill, directly from the sales document.</span></span> <span data-ttu-id="04d07-107">Se non si desidera includere il collegamento, ad esempio, se un cliente pagherà in contanti, è possibile rimuovere il servizio di pagamento dalla fattura prima della registrazione.</span><span class="sxs-lookup"><span data-stu-id="04d07-107">If you don't want to include the link, for example, if a customer will pay with cash, you can remove the payment service from the invoice before posting.</span></span>  

<span data-ttu-id="04d07-108">Le estensioni Microsoft Pay, PayPal Payments Standard e WorldPay Payments Standard vengono installate in [!INCLUDE[d365fin](includes/d365fin_md.md)] e sono pronte per essere abilitate.</span><span class="sxs-lookup"><span data-stu-id="04d07-108">The Microsoft Pay, PayPal Payments Standard, and WorldPay Payments Standard extensions are installed in [!INCLUDE[d365fin](includes/d365fin_md.md)], and are ready for you to enable.</span></span>  

## <a name="to-enable-a-payment-service-in-included365finincludesd365finmdmd"></a><span data-ttu-id="04d07-109">Per abilitare un servizio di pagamento in [!INCLUDE[d365fin](includes/d365fin_md.md)]</span><span class="sxs-lookup"><span data-stu-id="04d07-109">To enable a payment service in [!INCLUDE[d365fin](includes/d365fin_md.md)]</span></span>
1. <span data-ttu-id="04d07-110">Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **Servizi di pagamento**, quindi scegliere il collegamento correlato.</span><span class="sxs-lookup"><span data-stu-id="04d07-110">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Payment Services**, and then choose the related link.</span></span>  
2. <span data-ttu-id="04d07-111">Nella finestra **Servizi di pagamento** scegliere l'azione **Nuovo**.</span><span class="sxs-lookup"><span data-stu-id="04d07-111">In the **Payment Services** window, choose the **New** action.</span></span>  
3. <span data-ttu-id="04d07-112">Selezionare il servizio di pagamento e chiudere la finestra.</span><span class="sxs-lookup"><span data-stu-id="04d07-112">Select the payment service, and then close the window.</span></span>  
4. <span data-ttu-id="04d07-113">Nella finestra **Servizi di pagamento** scegliere l'azione **Setup**.</span><span class="sxs-lookup"><span data-stu-id="04d07-113">In the **Payment Services** window, choose the **Setup** action.</span></span>  
5. <span data-ttu-id="04d07-114">Compilare i campi, se necessario.</span><span class="sxs-lookup"><span data-stu-id="04d07-114">Fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  
6. <span data-ttu-id="04d07-115">Chiudere la finestra.</span><span class="sxs-lookup"><span data-stu-id="04d07-115">Close the window.</span></span>  

## <a name="to-select-a-payment-service-on-a-sales-invoice"></a><span data-ttu-id="04d07-116">Per selezionare un servizio di pagamento di una fattura di vendita</span><span class="sxs-lookup"><span data-stu-id="04d07-116">To select a payment service on a sales invoice</span></span>
1. <span data-ttu-id="04d07-117">Nella home page scegliere **Fatture vendite**.</span><span class="sxs-lookup"><span data-stu-id="04d07-117">On the Home page, choose **Sales Invoices**.</span></span>  
2. <span data-ttu-id="04d07-118">Aprire una fattura di vendita che si desidera pagare utilizzando il servizio di pagamento.</span><span class="sxs-lookup"><span data-stu-id="04d07-118">Open the sales invoice that you want to pay by using the payment service.</span></span>  
3. <span data-ttu-id="04d07-119">Nel campo **Servizio di pagamento** scegliere il servizio di pagamento.</span><span class="sxs-lookup"><span data-stu-id="04d07-119">In the **Payment Service** field, choose the payment service.</span></span>  

    > [!NOTE]  
>   <span data-ttu-id="04d07-120">Il campo **Servizio di pagamento** è disponibile solo se è stato abilitato il servizio di pagamento.</span><span class="sxs-lookup"><span data-stu-id="04d07-120">The **Payment Service** field is available only if you've enabled the payment service.</span></span>  

## <a name="see-also"></a><span data-ttu-id="04d07-121">Vedi anche</span><span class="sxs-lookup"><span data-stu-id="04d07-121">See Also</span></span>  
[<span data-ttu-id="04d07-122">Setup Vendite</span><span class="sxs-lookup"><span data-stu-id="04d07-122">Setting Up Sales</span></span>](sales-setup-sales.md)  
[<span data-ttu-id="04d07-123">Vendite</span><span class="sxs-lookup"><span data-stu-id="04d07-123">Sales</span></span>](sales-manage-sales.md)  
<span data-ttu-id="04d07-124">[Personalizzazione di [!INCLUDE[d365fin](includes/d365fin_md.md)] utilizzando le estensioni](ui-extensions.md)</span><span class="sxs-lookup"><span data-stu-id="04d07-124">[Customizing [!INCLUDE[d365fin](includes/d365fin_md.md)] Using Extensions](ui-extensions.md)</span></span>  
<span data-ttu-id="04d07-125">[Utilizzo di [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="04d07-125">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  
