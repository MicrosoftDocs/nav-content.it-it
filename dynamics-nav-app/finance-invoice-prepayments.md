---
title: Fatturare i pagamenti anticipati
description: "I pagamenti anticipati sono pagamenti che vengono fatturati e registrati in un ordine di pagamento anticipato di vendita o di acquisto prima della fatturazione finale. Potrebbe essere necessario richiedere un deposito prima di iniziare la produzione di articoli su ordine oppure richiedere il pagamento prima della spedizione degli articoli a un cliente. La funzionalità di pagamento anticipato consente di fatturare e riscuotere i depositi richiesti dai clienti o di rimettere i depositi ai fornitori. In questo modo è possibile assicurarsi che tutti i pagamenti siano registrati a fronte di una fattura."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/07/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: e21a831a4ac96ae646c864f6dfeb38a32467593a
ms.contentlocale: it-it
ms.lasthandoff: 10/16/2017

---
# <a name="invoicing-prepayments"></a><span data-ttu-id="e15ac-106">Fatturazione dei pagamenti anticipati</span><span class="sxs-lookup"><span data-stu-id="e15ac-106">Invoicing Prepayments</span></span>
<span data-ttu-id="e15ac-107">I pagamenti anticipati sono pagamenti che vengono fatturati e registrati in un ordine di pagamento anticipato di vendita o di acquisto prima della fatturazione finale.</span><span class="sxs-lookup"><span data-stu-id="e15ac-107">Prepayments are payments that are invoiced and posted to a sales or purchase prepayment order before final invoicing.</span></span> <span data-ttu-id="e15ac-108">Potrebbe essere necessario richiedere un deposito prima di iniziare la produzione di articoli su ordine oppure richiedere il pagamento prima della spedizione degli articoli a un cliente.</span><span class="sxs-lookup"><span data-stu-id="e15ac-108">You might require a deposit before you manufacture items to order, or you might require payment before you ship items to a customer.</span></span> <span data-ttu-id="e15ac-109">La funzionalità di pagamento anticipato consente di fatturare e riscuotere i depositi richiesti dai clienti o di rimettere i depositi ai fornitori.</span><span class="sxs-lookup"><span data-stu-id="e15ac-109">The prepayments functionality enables you to invoice and collect deposits required from customers or to remit deposits to vendors.</span></span> <span data-ttu-id="e15ac-110">In questo modo è possibile assicurarsi che tutti i pagamenti siano registrati a fronte di una fattura.</span><span class="sxs-lookup"><span data-stu-id="e15ac-110">Thus, you can ensure that all payments are posted against an invoice.</span></span>  

 <span data-ttu-id="e15ac-111">I requisiti del pagamento anticipato possono essere definiti per un cliente o un fornitore per tutti gli articoli o solo per alcuni.</span><span class="sxs-lookup"><span data-stu-id="e15ac-111">Prepayment requirements can be defined for a customer or vendor for all items or selected items.</span></span> <span data-ttu-id="e15ac-112">Una volta definite le impostazioni necessarie, è possibile generare fatture di pagamento anticipato da ordini di vendita o di acquisto per l'importo calcolato.</span><span class="sxs-lookup"><span data-stu-id="e15ac-112">After you complete the required setup, you can generate prepayment invoices from sales and purchase orders for the calculated prepayment amount.</span></span> <span data-ttu-id="e15ac-113">È possibile modificare gli importi nella fattura in base alle esigenze.</span><span class="sxs-lookup"><span data-stu-id="e15ac-113">You can change the amounts on the invoice as needed.</span></span> <span data-ttu-id="e15ac-114">È ad esempio possibile specificare un importo totale per l'intero ordine.</span><span class="sxs-lookup"><span data-stu-id="e15ac-114">For example, you can specify a total amount for the entire order.</span></span> <span data-ttu-id="e15ac-115">È inoltre possibile inviare ulteriori fatture di pagamento anticipato se, ad esempio, vengono aggiunti altri articoli all'ordine.</span><span class="sxs-lookup"><span data-stu-id="e15ac-115">You can also send additional prepayment invoices if, for example, additional items are added to the order.</span></span> <span data-ttu-id="e15ac-116">È possibile aumentare le quantità o aggiungere nuove righe a un ordine dopo aver emesso un pagamento anticipato, quindi registrare un'altra fattura di pagamento anticipato.</span><span class="sxs-lookup"><span data-stu-id="e15ac-116">You can increase quantities or add new lines to an order after issuing a prepayment, and then you can post another prepayment invoice.</span></span> <span data-ttu-id="e15ac-117">Se si desidera eliminare una riga per la quale è già stato fatturato un pagamento anticipato, è necessario emettere una nota di credito di pagamento anticipato prima di poter eliminare la riga.</span><span class="sxs-lookup"><span data-stu-id="e15ac-117">If you want to delete a line for which a prepayment has already been invoiced, you must issue a prepayment credit memo before you can delete the line.</span></span>  

 <span data-ttu-id="e15ac-118">Nella tabella seguente viene descritta una sequenza di task, con collegamenti agli argomenti che li descrivono.</span><span class="sxs-lookup"><span data-stu-id="e15ac-118">The following table describes a sequence of tasks, with links to the topics that describe them.</span></span>

|<span data-ttu-id="e15ac-119">**Per**</span><span class="sxs-lookup"><span data-stu-id="e15ac-119">**To**</span></span>|<span data-ttu-id="e15ac-120">**Vedere**</span><span class="sxs-lookup"><span data-stu-id="e15ac-120">**See**</span></span>|  
|------------|-------------|  
|<span data-ttu-id="e15ac-121">Impostare le categorie di registrazione dei pagamenti anticipati e la numerazione e impostare le percentuali pagamento anticipato di default per clienti, fornitori e articoli.</span><span class="sxs-lookup"><span data-stu-id="e15ac-121">Set up prepayment posting groups and number series, and set up default prepayment percentages for customers, vendors, and items.</span></span>|[<span data-ttu-id="e15ac-122">Procedura: Impostare i pagamenti anticipati</span><span class="sxs-lookup"><span data-stu-id="e15ac-122">How to: Set Up Prepayments</span></span>](finance-set-up-prepayments.md)|
|<span data-ttu-id="e15ac-123">Creare un ordine, rettificare gli importi di pagamento anticipato ed emettere una fattura per gli importi di pagamento anticipato.</span><span class="sxs-lookup"><span data-stu-id="e15ac-123">Create an order, adjust the prepayment amounts, and issue an invoice for prepayment amounts.</span></span>|[<span data-ttu-id="e15ac-124">Procedura: Creare fatture di pagamenti anticipati</span><span class="sxs-lookup"><span data-stu-id="e15ac-124">How to: Create Prepayment Invoices</span></span>](finance-how-to-create-prepayment-invoices.md)|  
|<span data-ttu-id="e15ac-125">Emettere una fattura di pagamento anticipato supplementare, per articoli aggiuntivi o per un deposito aggiuntivo rispetto all'ordine originale, oppure emettere una nota di credito di pagamento anticipato.</span><span class="sxs-lookup"><span data-stu-id="e15ac-125">Issue an additional prepayment invoice, either for additional items or for an additional deposit on the original order, or issue a prepayment credit memo.</span></span>|[<span data-ttu-id="e15ac-126">Procedura: Rettificare i pagamenti anticipati</span><span class="sxs-lookup"><span data-stu-id="e15ac-126">How to: Correct Prepayments</span></span>](finance-how-to-correct-prepayments.md)|  

## <a name="see-also"></a><span data-ttu-id="e15ac-127">Vedi anche</span><span class="sxs-lookup"><span data-stu-id="e15ac-127">See Also</span></span>  
[<span data-ttu-id="e15ac-128">Procedura dettagliata: impostazione e fatturazione dei pagamenti anticipati vendite</span><span class="sxs-lookup"><span data-stu-id="e15ac-128">Walkthrough: Setting Up and Invoicing Sales Prepayments</span></span>](walkthrough-setting-up-and-invoicing-sales-prepayments.md)  
[<span data-ttu-id="e15ac-129">Finanze</span><span class="sxs-lookup"><span data-stu-id="e15ac-129">Finance</span></span>](finance.md)  
<span data-ttu-id="e15ac-130">[Utilizzo di [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="e15ac-130">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
