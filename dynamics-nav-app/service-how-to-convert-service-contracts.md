---
title: Come convertire i contratti di assistenza
description: "Dal momento che lo strumento di modifica dell'aliquota IVA non può convertire i contratti di assistenza, tali contratti devono essere convertiti manualmente. In questo argomento vengono descritti diversi metodi alternativi che è possibile utilizzare per la conversione del contratto di assistenza."
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
ms.openlocfilehash: 2ae15fef88b10072a5c1dffa8e2673fe9413dd27
ms.contentlocale: it-it
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-convert-service-contracts-that-include-vat-amounts"></a><span data-ttu-id="49414-104">Procedura: Convertire i contratti di assistenza che includono importi IVA</span><span class="sxs-lookup"><span data-stu-id="49414-104">How to: Convert Service Contracts that Include VAT Amounts</span></span>
<span data-ttu-id="49414-105">Dal momento che lo strumento di modifica dell'aliquota IVA non può convertire i contratti di assistenza, tali contratti devono essere convertiti manualmente.</span><span class="sxs-lookup"><span data-stu-id="49414-105">Because the VAT rate change tool cannot convert service contracts, these contracts must be converted manually.</span></span> <span data-ttu-id="49414-106">In questo argomento vengono descritti diversi metodi alternativi che è possibile utilizzare per la conversione del contratto di assistenza.</span><span class="sxs-lookup"><span data-stu-id="49414-106">This topic describes several alternative methods that you can use for service contract conversion.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="49414-107">In questo argomento viene fornito un flusso di lavoro dettagliato.</span><span class="sxs-lookup"><span data-stu-id="49414-107">This topic provides a high-level workflow.</span></span>  

 <span data-ttu-id="49414-108">Nella procedura riportata di seguito viene descritto come correggere una fattura per un contratto di assistenza prepagato creato un anno prima.</span><span class="sxs-lookup"><span data-stu-id="49414-108">The following procedure describes how to correct an invoice for a prepaid service contact that has been created a year in advance.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="49414-109">Per questo esempio, è necessario modificare la data di lavoro in 01.01.2017.</span><span class="sxs-lookup"><span data-stu-id="49414-109">For this example, you must change your work date to 01.01.2017.</span></span>  

### <a name="to-correct-an-invoice-for-a-prepaid-service-contract"></a><span data-ttu-id="49414-110">Per correggere una fattura per un contratto di assistenza prepagato</span><span class="sxs-lookup"><span data-stu-id="49414-110">To correct an invoice for a prepaid service contract</span></span>  
1. <span data-ttu-id="49414-111">Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **Gestione contratti**, quindi scegliere il collegamento correlato.</span><span class="sxs-lookup"><span data-stu-id="49414-111">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Contract Management**, and then choose the related link.</span></span>  
2. <span data-ttu-id="49414-112">In **Liste** selezionare **Contratti assistenza**.</span><span class="sxs-lookup"><span data-stu-id="49414-112">Under **Lists**, choose **Service Contracts**.</span></span>  
3. <span data-ttu-id="49414-113">Creare un nuovo contratto di assistenza prepagato.</span><span class="sxs-lookup"><span data-stu-id="49414-113">Create a new prepaid service contract.</span></span> <span data-ttu-id="49414-114">Immettere una data di inizio **01.01.2017** e un anno del periodo di fatturazione per il cliente **20000**.</span><span class="sxs-lookup"><span data-stu-id="49414-114">Enter a start date of **01.01.2017** and an invoice period year for customer **20000**.</span></span>  
4. <span data-ttu-id="49414-115">Questo contratto deve essere firmato.</span><span class="sxs-lookup"><span data-stu-id="49414-115">This contract must be signed.</span></span> <span data-ttu-id="49414-116">Nel gruppo **Processo** della scheda **Pagina iniziale** scegliere **Firma contratto**.</span><span class="sxs-lookup"><span data-stu-id="49414-116">On the **Home** tab, in the **Process** group, choose **Sign Contract**.</span></span>  
5. <span data-ttu-id="49414-117">Creare una fattura assistenza.</span><span class="sxs-lookup"><span data-stu-id="49414-117">Create a service invoice.</span></span>
6. <span data-ttu-id="49414-118">La fattura viene elencata come fattura di assistenza non registrata.</span><span class="sxs-lookup"><span data-stu-id="49414-118">The invoice is listed as an unposted service invoice.</span></span> <span data-ttu-id="49414-119">Per visualizzare la fattura di assistenza, fare clic su **Assistenza**, selezionare **Gestione contratti**, quindi scegliere **Fatture assistenza**.</span><span class="sxs-lookup"><span data-stu-id="49414-119">To view the service invoice, choose **Service**, choose **Contract Management**, and then choose **Service Invoices**.</span></span>  
7. <span data-ttu-id="49414-120">Registrare la fattura di assistenza.</span><span class="sxs-lookup"><span data-stu-id="49414-120">Post the service invoice.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="49414-121">Non modificare la fattura di assistenza non registrata.</span><span class="sxs-lookup"><span data-stu-id="49414-121">Do not change the unposted service invoice.</span></span> <span data-ttu-id="49414-122">Poiché i movimenti di assistenza vengono generati quando la fattura viene creata, una modifica della fattura non registrata non influenzerà i movimenti contabili di assistenza già creati.</span><span class="sxs-lookup"><span data-stu-id="49414-122">Since the service ledger entries are created when the invoice is created, a change in the unposted invoice will not change the already created service ledger entries.</span></span> <span data-ttu-id="49414-123">Tuttavia, i movimenti IVA vengono creati quando la fattura viene registrata.</span><span class="sxs-lookup"><span data-stu-id="49414-123">However, the VAT entries are created when the invoice is posted.</span></span> <span data-ttu-id="49414-124">In questo modo è possibile modificare la categoria di registrazione articoli/servizi e la categoria di registrazione articoli/servizi del sistema di preferenze generalizzate nella fattura di assistenza non registrata.</span><span class="sxs-lookup"><span data-stu-id="49414-124">This lets you change the general product posting group and the GSP product posting group on the unposted service invoice.</span></span>  

### <a name="to-create-a-credit-memo-for-vat-difference"></a><span data-ttu-id="49414-125">Per creare una nota di credito per la differenza IVA</span><span class="sxs-lookup"><span data-stu-id="49414-125">To create a credit memo for VAT difference</span></span>  
<span data-ttu-id="49414-126">Nella procedura riportata di seguito viene descritto come creare una nota di credito che includa solo la differenza IVA per un periodo già fatturato a partire da **01.07.2017**.</span><span class="sxs-lookup"><span data-stu-id="49414-126">The following procedure describes how to create a credit memo that only includes the VAT difference for the already invoiced period starting on **01.07.2017**.</span></span> <span data-ttu-id="49414-127">Nell'esempio l'importo IVA viene registrato solo nel modulo Gestione contabile, non in quello Gestione assistenza.</span><span class="sxs-lookup"><span data-stu-id="49414-127">In this example, the VAT amount is only posted to the Financial Management module, not to the Service Management module.</span></span> <span data-ttu-id="49414-128">I movimenti IVA collegati al movimento assistenza non verranno corretti.</span><span class="sxs-lookup"><span data-stu-id="49414-128">The VAT entries that are linked to the service ledger entry will not be corrected.</span></span>  

1. <span data-ttu-id="49414-129">Creare un nuovo conto di contabilità generale per la differenza IVA.</span><span class="sxs-lookup"><span data-stu-id="49414-129">Create a new general ledger account for the VAT difference.</span></span> <span data-ttu-id="49414-130">Questo conto verrà utilizzato per la registrazione diretta della correzione IVA.</span><span class="sxs-lookup"><span data-stu-id="49414-130">This account will be used for direct posting of the VAT correction.</span></span>  
2. <span data-ttu-id="49414-131">Aggiungere una nuova riga all'impostazione per le registrazioni IVA.</span><span class="sxs-lookup"><span data-stu-id="49414-131">Add a new line to the VAT posting setup.</span></span>  

### <a name="to-create-contract-expiration-dates-in-contract-lines"></a><span data-ttu-id="49414-132">Per creare le date di scadenza del contratto nelle righe di contratto</span><span class="sxs-lookup"><span data-stu-id="49414-132">To create contract expiration dates in contract lines</span></span>  
<span data-ttu-id="49414-133">Nella procedura riportata di seguito viene descritto come creare nuovi contratti utilizzando le date di scadenza del contratto nelle righe del contratto di assistenza.</span><span class="sxs-lookup"><span data-stu-id="49414-133">The following procedure describes how to create new contracts by working with contact expiration dates in service contract lines.</span></span>  

1. <span data-ttu-id="49414-134">Nella finestra **Contratto assistenza** impostare la data di scadenza del contratto su **30.06.2017**.</span><span class="sxs-lookup"><span data-stu-id="49414-134">In the **Service Contract** window, set the contract expiration date to **30.06.2017**.</span></span>  
2. <span data-ttu-id="49414-135">Scegliere l'azione **Crea nota credito** per creare automaticamente una nota di credito per il periodo compreso tra luglio 2017 e dicembre 2017.</span><span class="sxs-lookup"><span data-stu-id="49414-135">Choose the **Create Credit Memo** action to automatically create a credit memo for July 2017 to December 2017.</span></span>  
3. <span data-ttu-id="49414-136">Dal momento che il contratto è scaduto, è necessario creare un nuovo contratto con la nuova aliquota IVA per il periodo compreso tra il 1° luglio 2017 e 31 dicembre 2017.</span><span class="sxs-lookup"><span data-stu-id="49414-136">Because the contract has expired, you need to create a new contract for the period with the new VAT rate for July 1, 2017 to December 31, 2017.</span></span>  

### <a name="to-create-a-new-credit-memo"></a><span data-ttu-id="49414-137">Per creare una nuova nota di credito.</span><span class="sxs-lookup"><span data-stu-id="49414-137">To create a new credit memo</span></span>  
<span data-ttu-id="49414-138">Nella procedura riportata di seguito viene descritto come creare una nuova nota di credito mediante il processo batch **Prendi mov. contr. prepagati**.</span><span class="sxs-lookup"><span data-stu-id="49414-138">The following procedure describes how to create a new credit memo using the **Get Prepaid Contract Entries** batch job.</span></span> <span data-ttu-id="49414-139">I movimenti che non si desidera correggere da gennaio 2017 a giugno 2017 verranno eliminati.</span><span class="sxs-lookup"><span data-stu-id="49414-139">Entries that you do not want to correct from January 2017 to June 2017 will be deleted.</span></span>  

1. <span data-ttu-id="49414-140">Eseguire lo strumento per la modifica dell'aliquota IVA il 1° luglio 2017.</span><span class="sxs-lookup"><span data-stu-id="49414-140">Run the VAT rate change tool on July 1, 2017.</span></span> <span data-ttu-id="49414-141">La categoria di registrazione articoli/servizi o la categoria di registrazione articoli/servizi IVA è cambiata.</span><span class="sxs-lookup"><span data-stu-id="49414-141">The general product posting group or the VAT product posting group is changed.</span></span> <span data-ttu-id="49414-142">Per ulteriori informazioni, vedere [Procedura: Utilizzare l'IVA nelle vendite e negli acquisti](finance-work-with-vat.md).</span><span class="sxs-lookup"><span data-stu-id="49414-142">For more information, see [How to: Work with VAT on Sales and Purchases](finance-work-with-vat.md).</span></span>  
2. <span data-ttu-id="49414-143">Dopo aver eseguito lo strumento di modifica aliquota IVA, immettere una data di scadenza del contratto per il contratto di assistenza.</span><span class="sxs-lookup"><span data-stu-id="49414-143">After running the VAT rate change tool, enter a contract expiration date for the service contract.</span></span> <span data-ttu-id="49414-144">È ora possibile eliminare la riga del contratto di assistenza e creare una nuova riga identica a quella precedente.</span><span class="sxs-lookup"><span data-stu-id="49414-144">You can now delete the service contract line and create a new line that is identical to the old one.</span></span>  
3. <span data-ttu-id="49414-145">Creare una nuova fattura per il periodo compreso tra gennaio 2017 e dicembre 2012 utilizzando la nuova aliquota IVA.</span><span class="sxs-lookup"><span data-stu-id="49414-145">Create a new invoice for the period of January 2017 to December 2012 using the new VAT rate.</span></span>  
4. <span data-ttu-id="49414-146">Per creare un'altra nota di credito, selezionare **Nuovo** nella finestra **Note credito assistenza**.</span><span class="sxs-lookup"><span data-stu-id="49414-146">To create another credit memo, in the **Service Credit Memos** window, choose **New** to create a new service credit memo.</span></span>  
5. <span data-ttu-id="49414-147">Scegliere l'azione **Prendi mov. contr. prepagati**.</span><span class="sxs-lookup"><span data-stu-id="49414-147">Choose the **Get Prepaid Contract Entries** action.</span></span>  
6. <span data-ttu-id="49414-148">Dopo aver completato la conversione, l'IVA e i movimenti contabili verranno corretti.</span><span class="sxs-lookup"><span data-stu-id="49414-148">After the conversion is complete, VAT and service ledger entries will be correct.</span></span>  

## <a name="see-also"></a><span data-ttu-id="49414-149">Vedi anche</span><span class="sxs-lookup"><span data-stu-id="49414-149">See Also</span></span>  
[<span data-ttu-id="49414-150">Procedura: Utilizzare contratti e offerte di contratto di assistenza</span><span class="sxs-lookup"><span data-stu-id="49414-150">How to: Work with Service Contracts and Service Contract Quotes</span></span>](service-how-to-create-service-contracts-and-service-contract-quotes.md)  
[<span data-ttu-id="49414-151">Finanze</span><span class="sxs-lookup"><span data-stu-id="49414-151">Finance</span></span>](finance.md)  
[<span data-ttu-id="49414-152">Procedura: Dichiarare l'IVA all'autorità fiscale</span><span class="sxs-lookup"><span data-stu-id="49414-152">How to: Report VAT to Tax Authorities</span></span>](finance-how-report-vat.md)  
[<span data-ttu-id="49414-153">Procedura: Utilizzare l'IVA nelle vendite e negli acquisti</span><span class="sxs-lookup"><span data-stu-id="49414-153">How to: Work with VAT on Sales and Purchases</span></span>](finance-work-with-vat.md)  
