---
title: 'Procedura: Gestire gli approvvigionamenti per un progetto'
author: SorenGP
ms.custom: na
ms.date: 11/01/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: 00b9ed8480f6b5ab9265beb0fe2dc0060b1c3192
ms.contentlocale: it-it
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-manage-job-supplies"></a><span data-ttu-id="ee11d-102">Procedura: Gestire gli approvvigionamenti delle commesse</span><span class="sxs-lookup"><span data-stu-id="ee11d-102">How to: Manage Job Supplies</span></span>
<span data-ttu-id="ee11d-103">La gestione degli approvvigionamenti di progetto di articoli, servizi e spese è un aspetto integrale e critico dell'esecuzione di tutte le commesse.</span><span class="sxs-lookup"><span data-stu-id="ee11d-103">Managing project supplies of items, services, and expenses is an integral and critical aspect of the execution of all jobs.</span></span> <span data-ttu-id="ee11d-104">È possibile utilizzare le giacenze o effettuare acquisti specifici per delle commesse utilizzando gli ordini di acquisto e/o le fatture di acquisto.</span><span class="sxs-lookup"><span data-stu-id="ee11d-104">You can use inventory quantities or make job-specific purchases using purchase orders or purchase invoices.</span></span> <span data-ttu-id="ee11d-105">Ad esempio, per completare una commessa relativa a un intervento di assistenza su un computer è richiesto un nuovo disco.</span><span class="sxs-lookup"><span data-stu-id="ee11d-105">For example, a service job on a computer requires a new disk.</span></span> <span data-ttu-id="ee11d-106">Si crea quindi una fattura di acquisto per acquistare il nuovo disco e si registra la commessa in cui verrà utilizzato.</span><span class="sxs-lookup"><span data-stu-id="ee11d-106">You create a purchase invoice to buy a new disk and record the job that it will be used on.</span></span>

<span data-ttu-id="ee11d-107">Se il processo di acquisto non richiede la registrazione separata della transazione fisica, è possibile elaborare un acquisto nella finestra **Registrazioni commesse in G/L**.</span><span class="sxs-lookup"><span data-stu-id="ee11d-107">If the purchase process does not require that the physical transaction be recorded separately, then a purchase may be processed in the **Job G/L Journal** window.</span></span> <span data-ttu-id="ee11d-108">Per ulteriori informazioni, vedere [Procedura: Registrare l'utilizzo nelle commesse](projects-how-record-job-usage.md).</span><span class="sxs-lookup"><span data-stu-id="ee11d-108">For more information, see [How to: Record Usage for Jobs](projects-how-record-job-usage.md).</span></span>

## <a name="to-purchase-items-or-services-for-a-job"></a><span data-ttu-id="ee11d-109">Per acquistare articoli o servizi per una commessa</span><span class="sxs-lookup"><span data-stu-id="ee11d-109">To purchase items or services for a job</span></span>
<span data-ttu-id="ee11d-110">Nella procedura riportata di seguito viene illustrato come utilizzare una fattura di acquisto per acquistare i prodotti per una commessa.</span><span class="sxs-lookup"><span data-stu-id="ee11d-110">The following procedure shows how to use a purchase invoice to purchase products for a job.</span></span> <span data-ttu-id="ee11d-111">La stessa procedura vale anche quando si utilizza un ordine di acquisto.</span><span class="sxs-lookup"><span data-stu-id="ee11d-111">The same steps apply when using a purchase order.</span></span>  

1. <span data-ttu-id="ee11d-112">Nell'angolo superiore destro, scegliere l'icona **Cerca pagina o report**, immettere **Fatture acquisto**, quindi scegliere il collegamento correlato.</span><span class="sxs-lookup"><span data-stu-id="ee11d-112">In the top right corner, choose the **Search for Page or Report** icon, enter **Purchase Invoices**, and then choose the related link.</span></span>  
2. <span data-ttu-id="ee11d-113">Scegliere l'azione **Nuovo** e compilare i campi necessari.</span><span class="sxs-lookup"><span data-stu-id="ee11d-113">Choose the **New** action and fill in the fields as necessary.</span></span> <span data-ttu-id="ee11d-114">Per ulteriori informazioni, vedere [Procedura: Registrare gli acquisti](purchasing-how-record-purchases.md).</span><span class="sxs-lookup"><span data-stu-id="ee11d-114">For more information, see [How to: Record Purchases](purchasing-how-record-purchases.md).</span></span>
3. <span data-ttu-id="ee11d-115">Nei campi **Nr. commessa**</span><span class="sxs-lookup"><span data-stu-id="ee11d-115">In the **Job No.**</span></span> <span data-ttu-id="ee11d-116">e **Nr. task commessa**,</span><span class="sxs-lookup"><span data-stu-id="ee11d-116">and **Job Task No.**</span></span> <span data-ttu-id="ee11d-117">selezionare le informazioni della commessa per la quale si desidera acquistare articoli o servizi.</span><span class="sxs-lookup"><span data-stu-id="ee11d-117">fields, select the information of the job that you want to purchase items or services for.</span></span>  

    <span data-ttu-id="ee11d-118">Il valore che si seleziona nel campo **Tipo riga commessa** definisce se viene creata una riga di pianificazione quando si registra l'utilizzo dell'articolo.</span><span class="sxs-lookup"><span data-stu-id="ee11d-118">The value that you select in the **Job Line Type** field defines whether a planning line is created when you post the usage of the item.</span></span> <span data-ttu-id="ee11d-119">Se il campo contiene **Fatturabile**, vengono create le righe di pianificazione commessa che sono pronte per la fatturazione al cliente.</span><span class="sxs-lookup"><span data-stu-id="ee11d-119">If the field contains **Billable**, then job planning lines that are ready to be invoiced to the customer are created.</span></span> <span data-ttu-id="ee11d-120">Per ulteriori informazioni, vedere [Procedura: Fatturare commesse](projects-how-invoice-jobs.md).</span><span class="sxs-lookup"><span data-stu-id="ee11d-120">For more information, see [How to: Invoice Jobs](projects-how-invoice-jobs.md).</span></span>

4. <span data-ttu-id="ee11d-121">Scegliere l'azione **Registra**.</span><span class="sxs-lookup"><span data-stu-id="ee11d-121">Choose the **Post** action.</span></span>

## <a name="to-view-the-value-of-purchases-for-a-job"></a><span data-ttu-id="ee11d-122">Per visualizzare il valore degli acquisti per una commessa</span><span class="sxs-lookup"><span data-stu-id="ee11d-122">To view the value of purchases for a job</span></span>  

1. <span data-ttu-id="ee11d-123">Nell'angolo superiore destro, scegliere l'icona **Cerca pagina o report**, immettere **Commesse**, quindi scegliere il collegamento correlato.</span><span class="sxs-lookup"><span data-stu-id="ee11d-123">In the top right corner, choose the **Search for Page or Report** icon, enter **Jobs**, and then choose the related link.</span></span>
2. <span data-ttu-id="ee11d-124">Aprire una scheda commessa di interesse.</span><span class="sxs-lookup"><span data-stu-id="ee11d-124">Open a relevant job card.</span></span>

    <span data-ttu-id="ee11d-125">Nella Scheda dettaglio **Task**, il campo **Ordini inevasi** mostra l'importo inevaso totale, in valuta locale, degli articoli a magazzino e dei servizi sui documenti di acquisto per la riga del task commessa.</span><span class="sxs-lookup"><span data-stu-id="ee11d-125">On the **Tasks** FastTab, the **Outstanding Orders** field shows the total outstanding amount, in local currency, of inventory items and services on purchase documents for the job task line.</span></span>  

    <span data-ttu-id="ee11d-126">Il campo **Importo carichi non fatt.** mostra il valore di articoli spediti su documenti di acquisto, ma non ancora fatturati.</span><span class="sxs-lookup"><span data-stu-id="ee11d-126">The **Amt. Rec. Not Invoiced** field shows the value of items delivered on purchase documents, but not yet invoiced.</span></span>  

3. <span data-ttu-id="ee11d-127">Scegliere uno dei campi per aprire la finestra **Righe acquisto** dove è possibile esaminare le informazioni sulle righe del documento di vendita correlate, inclusi gli articoli o i servizi che sono stati ricevuti.</span><span class="sxs-lookup"><span data-stu-id="ee11d-127">Choose either of the fields to open the **Purchase Lines** window where you can review information about the related purchase document lines, including which items or services have been received.</span></span>

## <a name="to-post-a-job-related-expense"></a><span data-ttu-id="ee11d-128">Per registrare una spesa correlata a una commessa</span><span class="sxs-lookup"><span data-stu-id="ee11d-128">To post a job-related expense</span></span>  
<span data-ttu-id="ee11d-129">Se si incorre in spese di commessa straordinarie o eccezionali, è possibile utilizzare la finestra **Registrazioni commesse in G/L** per registrarle direttamente nel conto commessa correlato.</span><span class="sxs-lookup"><span data-stu-id="ee11d-129">If you incur extraordinary or one-time job expenses, you can use the **Job G/L Journal** window to post them directly to the relevant job account.</span></span>

1. <span data-ttu-id="ee11d-130">Nell'angolo superiore destro, scegliere l'icona **Cerca pagina o report**, immettere **Registrazioni commesse in C/G**, quindi scegliere il collegamento correlato.</span><span class="sxs-lookup"><span data-stu-id="ee11d-130">In the top right corner, choose the **Search for Page or Report** icon, enter **Job G/L Journals**, and then choose the related link.</span></span>  
2. <span data-ttu-id="ee11d-131">Creare una nuova riga e immettere le informazioni sulla spesa, incluse le informazioni nei campi **Nr. commessa**</span><span class="sxs-lookup"><span data-stu-id="ee11d-131">Create a new line and enter information about the expense, including information in the **Job No.**</span></span> <span data-ttu-id="ee11d-132">e **Nr. task commessa**.</span><span class="sxs-lookup"><span data-stu-id="ee11d-132">and **Job Task No** fields.</span></span>  
3. <span data-ttu-id="ee11d-133">Una volta completate le registrazioni, scegliere l'azione **Registra**.</span><span class="sxs-lookup"><span data-stu-id="ee11d-133">When the journal is complete, choose the **Post** action.</span></span>


## <a name="see-also"></a><span data-ttu-id="ee11d-134">Vedi anche</span><span class="sxs-lookup"><span data-stu-id="ee11d-134">See Also</span></span>
[<span data-ttu-id="ee11d-135">Gestione di progetti</span><span class="sxs-lookup"><span data-stu-id="ee11d-135">Manage Projects</span></span>](projects-manage-projects.md)  
[<span data-ttu-id="ee11d-136">Contabilità</span><span class="sxs-lookup"><span data-stu-id="ee11d-136">Finance</span></span>](finance-setup.md)  
<span data-ttu-id="ee11d-137">[Gestire gli acquisti](purchasing-manage-purchasing.md)       </span><span class="sxs-lookup"><span data-stu-id="ee11d-137">[Manage Purchasing](purchasing-manage-purchasing.md)       </span></span>  
<span data-ttu-id="ee11d-138">[Gestire le vendite](sales-manage-sales.md)    </span><span class="sxs-lookup"><span data-stu-id="ee11d-138">[Manage Sales](sales-manage-sales.md)    </span></span>  
[<span data-ttu-id="ee11d-139">Utilizzare Dynamics NAV</span><span class="sxs-lookup"><span data-stu-id="ee11d-139">Work With Dynamics NAV</span></span>](ui-work-product.md)  

