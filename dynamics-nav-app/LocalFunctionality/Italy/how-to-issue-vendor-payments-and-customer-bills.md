---
title: 'Procedura: Emettere pagamenti fornitori ed effetti clienti'
description: "La funzionalità di pagamento degli effetti cliente e fornitore supporta i formati SEPA oltre ai formati di file italiani. È possibile pagare i fornitori in base al bonifico SEPA standard e riscuotere i pagamenti dai clienti in base al metodo di addebito diretto SEPA standard. Di seguito viene descritto il processo per l'invio del pagamento a un fornitore con bonifico SEPA. I passaggi sono simili per la riscossione del pagamento da un cliente."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: aa6d9ca868f3c580115975c128d7faa5ef40e43c
ms.contentlocale: it-it
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-issue-vendor-payments-and-customer-bills"></a><span data-ttu-id="bc558-106">Procedura: Emettere pagamenti fornitori ed effetti clienti</span><span class="sxs-lookup"><span data-stu-id="bc558-106">How to: Issue Vendor Payments and Customer Bills</span></span>
<span data-ttu-id="bc558-107">La funzionalità di pagamento degli effetti cliente e fornitore supporta i formati SEPA oltre ai formati di file italiani.</span><span class="sxs-lookup"><span data-stu-id="bc558-107">The vendor and customer bill pay feature supports SEPA-based formats in addition to Italian file formats.</span></span> <span data-ttu-id="bc558-108">È possibile pagare i fornitori in base al bonifico SEPA standard e riscuotere i pagamenti dai clienti in base al metodo di addebito diretto SEPA standard.</span><span class="sxs-lookup"><span data-stu-id="bc558-108">You can pay vendors according to the SEPA Credit Transfer standard and collect payment from customers according to the SEPA Direct Debit standard.</span></span> <span data-ttu-id="bc558-109">Di seguito viene descritto il processo per l'invio del pagamento a un fornitore con bonifico SEPA.</span><span class="sxs-lookup"><span data-stu-id="bc558-109">The following procedure describes the process for sending a SEPA-based payment to a vendor.</span></span> <span data-ttu-id="bc558-110">I passaggi sono simili per la riscossione del pagamento da un cliente.</span><span class="sxs-lookup"><span data-stu-id="bc558-110">The steps are similar for collecting payment from a customer.</span></span>  

 <span data-ttu-id="bc558-111">Prima di avviare la seguente procedura, controllare che le informazioni sulla banca della società siano state immesse nella finestra **Scheda conto corrente bancario**.</span><span class="sxs-lookup"><span data-stu-id="bc558-111">Before starting the following procedure, make sure that information for your company's bank has been provided in the **Bank Account Card** window.</span></span> <span data-ttu-id="bc558-112">Nella scheda. includere le informazioni per i seguenti campi:</span><span class="sxs-lookup"><span data-stu-id="bc558-112">On the card, include information for the following fields:</span></span>  

-   <span data-ttu-id="bc558-113">IBAN</span><span class="sxs-lookup"><span data-stu-id="bc558-113">IBAN</span></span>  

-   <span data-ttu-id="bc558-114">Codice SWIFT (facoltativo)</span><span class="sxs-lookup"><span data-stu-id="bc558-114">SWIFT Code (optional)</span></span>  

-   <span data-ttu-id="bc558-115">Formato esportazione pagamento</span><span class="sxs-lookup"><span data-stu-id="bc558-115">Payment Export Format</span></span>  

-   <span data-ttu-id="bc558-116">Nr serie ID msg CT SEPA</span><span class="sxs-lookup"><span data-stu-id="bc558-116">SEPA CT Msg. ID No.</span></span> <span data-ttu-id="bc558-117">Serie</span><span class="sxs-lookup"><span data-stu-id="bc558-117">Series</span></span>  

 <span data-ttu-id="bc558-118">Inoltre, occorre inserire una fattura di acquisito registrata e con cui è possibile inviare un pagamento.</span><span class="sxs-lookup"><span data-stu-id="bc558-118">In addition, there must be a posted purchased invoice against which you can send a payment.</span></span>  

### <a name="to-issue-payment-to-a-vendor"></a><span data-ttu-id="bc558-119">Per emettere il pagamento per un fornitore</span><span class="sxs-lookup"><span data-stu-id="bc558-119">To issue payment to a vendor</span></span>  

1.  <span data-ttu-id="bc558-120">Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **Fornitori**, quindi scegliere il collegamento correlato.</span><span class="sxs-lookup"><span data-stu-id="bc558-120">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Vendors**, and then choose the related link.</span></span>  

2.  <span data-ttu-id="bc558-121">Selezionare il fornitore al quale si desidera inviare il pagamento.</span><span class="sxs-lookup"><span data-stu-id="bc558-121">Select the vendor to which you want to send payment.</span></span> <span data-ttu-id="bc558-122">Nella Scheda dettaglio **Pagamento**, nel campo **Codice metodo di pagamento** scegliere **TRASFBANC**.</span><span class="sxs-lookup"><span data-stu-id="bc558-122">On the **Payment** FastTab, in the **Payment Method Code** field, choose, **TRASFBANC**.</span></span> <span data-ttu-id="bc558-123">Nel gruppo **Fornitore** della scheda **Naviga** selezionare **C/C bancari**.</span><span class="sxs-lookup"><span data-stu-id="bc558-123">On the **Navigate** tab, in the **Vendor** group, choose **Bank Accounts**.</span></span>  

3.  <span data-ttu-id="bc558-124">Nella **Lista C/C bancari fornitori**, selezionare il conto C/C bancari del fornitore e nella scheda **Pagina iniziale**, nel gruppo **Gestisci**, scegliere **Modifica**.</span><span class="sxs-lookup"><span data-stu-id="bc558-124">In the **Vendor Bank Account List**, select the vendor's bank account, and on the **Home** tab, in the **Manage** group, choose **Edit**.</span></span> <span data-ttu-id="bc558-125">Nella Scheda dettaglio **Trasferimento**, specificare le informazioni relative al campo **IBAN**.</span><span class="sxs-lookup"><span data-stu-id="bc558-125">On the **Transfer** FastTab, specify information for the **IBAN** field.</span></span>  

     <span data-ttu-id="bc558-126">Scegliere il pulsante **OK**.</span><span class="sxs-lookup"><span data-stu-id="bc558-126">Choose the **OK** button.</span></span>  

4.  <span data-ttu-id="bc558-127">Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "Cerca pagina o report"), immettere **Distinta fornitore**, quindi selezionare il collegamento correlato.</span><span class="sxs-lookup"><span data-stu-id="bc558-127">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Vendor Bill Card**, and then choose the related link.</span></span>  

5.  <span data-ttu-id="bc558-128">Nel gruppo **Gestisci** della scheda **Pagina iniziale** scegliere **Nuovo**.</span><span class="sxs-lookup"><span data-stu-id="bc558-128">On the **Home** tab, in the **Manage** group, choose **New**.</span></span>  

6.  <span data-ttu-id="bc558-129">Nella Scheda dettaglio **Generale**, immettere le informazioni nei seguenti campi: **Nr. conto bancario** del fornitore e **Codice metodo di pagamento**.</span><span class="sxs-lookup"><span data-stu-id="bc558-129">On the **General** FastTab, enter information for the following fields: **Bank Account No.** of the vendor and **Payment Method Code**.</span></span>  

7.  <span data-ttu-id="bc558-130">Nel gruppo **Processo** della scheda **Pagina iniziale** scegliere **Suggerisci pagamenti**.</span><span class="sxs-lookup"><span data-stu-id="bc558-130">On the **Home** tab, in the **Process** group, choose **Suggest Payment**.</span></span> <span data-ttu-id="bc558-131">Impostare i filtri appropriati e scegliere il pulsante **OK** per eseguire il processo batch.</span><span class="sxs-lookup"><span data-stu-id="bc558-131">Set filters, as appropriate, and then choose the **OK** button to run the batch job.</span></span>  

8.  <span data-ttu-id="bc558-132">Nel gruppo **Processo** della scheda **Pagina iniziale** scegliere **Crea distinta**.</span><span class="sxs-lookup"><span data-stu-id="bc558-132">On the **Home** tab, in the **Process** group, choose **Create List**.</span></span> <span data-ttu-id="bc558-133">Scegliere il pulsante **Sì** per inviare il pagamento dell'effetto.</span><span class="sxs-lookup"><span data-stu-id="bc558-133">Choose the **Yes** button to send the bill payment.</span></span>  

9. <span data-ttu-id="bc558-134">Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **Distinta effetti fornitore emessa** e selezionare il pagamento dell'effetto emesso dall'elenco.</span><span class="sxs-lookup"><span data-stu-id="bc558-134">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Vendor Bill List Issued**, and select bill payment that you issued from the list.</span></span> <span data-ttu-id="bc558-135">Nella scheda **Pagina iniziale** selezionare **Modifica**.</span><span class="sxs-lookup"><span data-stu-id="bc558-135">On the **Home** tab, choose **Edit**.</span></span> <span data-ttu-id="bc558-136">Verrà aperta la finestra **Distinta effetti forn. emessa**.</span><span class="sxs-lookup"><span data-stu-id="bc558-136">The **Vendor Bill List Sent Card** window opens.</span></span>  

10. <span data-ttu-id="bc558-137">Per esportare le informazioni di pagamento, nella scheda **Pagina iniziale**, nel gruppo **Report**, scegliere una delle seguenti opzioni: **Esporta distinta effetti su file**.</span><span class="sxs-lookup"><span data-stu-id="bc558-137">To export the payment information, on the **Home** tab, in the **Report** group, chose one of the following: **Export Bill List to File**.</span></span> <span data-ttu-id="bc558-138">È possibile visualizzare il file XML inviato.</span><span class="sxs-lookup"><span data-stu-id="bc558-138">You can review the xml file that was sent.</span></span>  

    1.  <span data-ttu-id="bc558-139">Esportare nel file (per file in formato SEPA standard)</span><span class="sxs-lookup"><span data-stu-id="bc558-139">Export to File (for standard SEPA format files)</span></span>  

    2.  <span data-ttu-id="bc558-140">Esporta distinta effetti su file</span><span class="sxs-lookup"><span data-stu-id="bc558-140">Export Bill List to File</span></span>  

     <span data-ttu-id="bc558-141">È possibile visualizzare il file XML prima di inviarlo.</span><span class="sxs-lookup"><span data-stu-id="bc558-141">You can review the .xml file before sending it.</span></span> <span data-ttu-id="bc558-142">Per esaminare e correggere gli errori, è possibile fare riferimento al riquadro dettaglio informazioni **Errori esportazione file** creato.</span><span class="sxs-lookup"><span data-stu-id="bc558-142">To review and fix errors, you can refer to the **File Export Errors** Fact Box.</span></span>  

## <a name="see-also"></a><span data-ttu-id="bc558-143">Vedi anche</span><span class="sxs-lookup"><span data-stu-id="bc558-143">See Also</span></span>  
 <span data-ttu-id="bc558-144">[Eseguire i pagamenti con il servizio di conversione dati bancari o bonifico SEPA](finance-make-payments-with-bank-data-conversion-service-or-sepa-credit-transfer.md) </span><span class="sxs-lookup"><span data-stu-id="bc558-144">[Make Payments with Bank Data Conversion Service or SEPA Credit Transfer](finance-make-payments-with-bank-data-conversion-service-or-sepa-credit-transfer.md) </span></span>  
 <span data-ttu-id="bc558-145">[Procedura: Impostare il trasferimento crediti SEPA](../../finance-how-to-set-up-sepa-credit-transfer.md) </span><span class="sxs-lookup"><span data-stu-id="bc558-145">[How to: Set Up SEPA Credit Transfer](../../finance-how-to-set-up-sepa-credit-transfer.md) </span></span>  
 [<span data-ttu-id="bc558-146">Riscuotere pagamenti con addebito diretto SEPA</span><span class="sxs-lookup"><span data-stu-id="bc558-146">Collecting Payments with SEPA Direct Debit</span></span>](../../finance-collect-payments-with-sepa-direct-debit.md)

