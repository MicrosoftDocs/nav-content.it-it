---
title: Scambiare dati
description: "È possibile scambiare i dati tra [!INCLUDE[d365fin](includes/d365fin_md.md)] e flussi o file esterni in relazione alle attività aziendali, come l'invio e la ricezione di documenti elettronici e l'importazione e l'esportazione di file dalla banca."
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/18/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: e41e0eb6dd10127a47b2b6545d0333db700586bc
ms.contentlocale: it-it
ms.lasthandoff: 10/16/2017

---
# <a name="exchanging-data"></a><span data-ttu-id="a6b57-103">Scambio di dati</span><span class="sxs-lookup"><span data-stu-id="a6b57-103">Exchanging Data</span></span>
<span data-ttu-id="a6b57-104">È possibile scambiare i dati tra [!INCLUDE[d365fin](includes/d365fin_md.md)] e flussi o file esterni in relazione alle attività aziendali, come l'invio e la ricezione di documenti elettronici e l'importazione e l'esportazione di file dalla banca.</span><span class="sxs-lookup"><span data-stu-id="a6b57-104">You can exchange data between [!INCLUDE[d365fin](includes/d365fin_md.md)] and external files or streams in connection with common business tasks, such as sending and receiving electronic documents and importing and exporting bank files.</span></span>  

<span data-ttu-id="a6b57-105">Prima di poter inviare e ricevere documenti elettronici o importare ed esportare file bancari, è necessario impostare il framework di scambio dati per elaborare i flussi o i file di dati interessati.</span><span class="sxs-lookup"><span data-stu-id="a6b57-105">Before you can send and receive electronic documents or import and export bank files, you must set up the data exchange framework to process the involved data files or streams.</span></span> <span data-ttu-id="a6b57-106">Inoltre, è necessario impostare delle aree correlate.</span><span class="sxs-lookup"><span data-stu-id="a6b57-106">In addition, you must set up related areas.</span></span> <span data-ttu-id="a6b57-107">Sono inclusi i dati master per i clienti a cui si inviano fatture elettroniche e il servizio di conversione di dati bancari nel caso si distribuiscano traduzioni di file della banca a un provider di servizi esterno.</span><span class="sxs-lookup"><span data-stu-id="a6b57-107">These include master data for customers that you send electronic invoices to and the bank data conversion service in case you distribute bank file conversions to an external service provider.</span></span> <span data-ttu-id="a6b57-108">Per ulteriori informazioni, vedere [Impostazione dello scambio di dati](across-set-up-data-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="a6b57-108">For more information, see [Setting Up Data Exchange](across-set-up-data-exchange.md).</span></span>  

 <span data-ttu-id="a6b57-109">Nella tabella seguente viene descritta una sequenza di task, con collegamenti agli argomenti che li descrivono.</span><span class="sxs-lookup"><span data-stu-id="a6b57-109">The following table describes a sequence of tasks, with links to the topics that describe them.</span></span>  

|<span data-ttu-id="a6b57-110">**Task**</span><span class="sxs-lookup"><span data-stu-id="a6b57-110">**To**</span></span>|<span data-ttu-id="a6b57-111">**Vedere**</span><span class="sxs-lookup"><span data-stu-id="a6b57-111">**See**</span></span>|  
|------------|-------------|  
|<span data-ttu-id="a6b57-112">Convertire i record del documento di vendita in [!INCLUDE[d365fin](includes/d365fin_md.md)] in un formato standardizzato e inviarli come documenti elettronici che i clienti possono ricevere nel proprio sistema.</span><span class="sxs-lookup"><span data-stu-id="a6b57-112">Convert sales document records in [!INCLUDE[d365fin](includes/d365fin_md.md)] to a standardized format and send them as electronic documents that your customers can receive into their system.</span></span>|[<span data-ttu-id="a6b57-113">Procedura: Inviare documenti elettronici</span><span class="sxs-lookup"><span data-stu-id="a6b57-113">How to: Send Electronic Documents</span></span>](sales-how-to-send-electronic-documents.md)|  
|<span data-ttu-id="a6b57-114">Inviare PDF o file immagine a un provider di servizi OCR e riceverli come documenti elettronici che possono essere convertiti in record di documento in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="a6b57-114">Send PDF or image files to a provider of OCR services, and receive them back as electronic documents that can be converted to document records in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span>|[<span data-ttu-id="a6b57-115">Procedura: Utilizzare OCR per convertire PDF e file di immagine in documenti elettronici</span><span class="sxs-lookup"><span data-stu-id="a6b57-115">How to: Use OCR to Turn PDF and Image Files into Electronic Documents</span></span>](across-how-use-ocr-pdf-images-files.md)|  
|<span data-ttu-id="a6b57-116">Ricevere i documenti elettronici dal servizio OCR o dal servizio di scambio documenti in un formato standardizzato che viene convertito nei relativi record di documento in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="a6b57-116">Receive electronic documents, either from the OCR service or the document exchange service, in a standardized format that you convert to the relevant document records in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span>|[<span data-ttu-id="a6b57-117">Procedura: Ricevere e convertire documenti elettronici</span><span class="sxs-lookup"><span data-stu-id="a6b57-117">How to: Receive and Convert Electronic Documents</span></span>](purchasing-how-to-receive-and-convert-electronic-documents.md)|  
|<span data-ttu-id="a6b57-118">Importare un file dell'estratto conto bancario nella finestra **Registrazione riconciliazione pagamenti** come primo passaggio della riconciliazione dei pagamenti o nella finestra **Riconciliazioni C/C bancari** come primo passaggio nella riconciliazione dei conti bancari.</span><span class="sxs-lookup"><span data-stu-id="a6b57-118">Import a bank statement file into the **Payment Reconciliation Journal** window as the first step in reconciling payments or into the **Bank Acc. Reconciliation** window as the first step in reconciling bank accounts.</span></span>|<span data-ttu-id="a6b57-119">[Collegare i pagamenti automaticamente e riconciliare i conti correnti bancari]([Collegare i pagamenti automaticamente e riconciliare i conti correnti bancari](receivables-apply-payments-auto-reconcile-bank-accounts.md)</span><span class="sxs-lookup"><span data-stu-id="a6b57-119">[Apply Payments Automatically and Reconcile Bank Accounts]([Applying Payments Automatically and Reconcile Bank Accounts](receivables-apply-payments-auto-reconcile-bank-accounts.md)</span></span>|  
|<span data-ttu-id="a6b57-120">Esportare i pagamenti dalla finestra **Registrazioni pagamenti** in un file della banca da caricare sul conto corrente bancario elettronico per l'elaborazione.</span><span class="sxs-lookup"><span data-stu-id="a6b57-120">Export payments from the **Payment Journal** window to a bank file that you upload to your electronic bank account for processing.</span></span>|[<span data-ttu-id="a6b57-121">Procedura: esportare pagamenti in un file della banca</span><span class="sxs-lookup"><span data-stu-id="a6b57-121">How to: Export Payments to a Bank File</span></span>](payables-how-export-payments-bank-file.md)|  
|<span data-ttu-id="a6b57-122">Indicare alla propria banca di trasferire gli importi dei pagamenti dai conti bancari dei clienti a quello della propria società in base al setup dell'addebito diretto SEPA.</span><span class="sxs-lookup"><span data-stu-id="a6b57-122">Instruct your bank to transfer payment amounts from your customers’ bank accounts to your company’s account according to your setup of SEPA direct debit.</span></span>|[<span data-ttu-id="a6b57-123">Procedura: Creare movimenti riscossione addebiti diretti SEPA ed esportarli in un file della banca</span><span class="sxs-lookup"><span data-stu-id="a6b57-123">How to: Create SEPA Direct Debit Collection Entries and Export to a Bank File</span></span>](finance-how-create-sepa-direct-debit-collection-entries-export-bank-file.md)|  
|<span data-ttu-id="a6b57-124">Utilizzare un provider di servizi per i tassi di cambio valuta per aggiornare la finestra **Valute**.</span><span class="sxs-lookup"><span data-stu-id="a6b57-124">Use a service provider of currency exchange rates to update the **Currencies** window.</span></span>|[<span data-ttu-id="a6b57-125">Procedura: Aggiornare i tassi di cambio delle valute</span><span class="sxs-lookup"><span data-stu-id="a6b57-125">How to: Update Currency Exchange Rates</span></span>](finance-how-update-currencies.md)|  
|<span data-ttu-id="a6b57-126">Visualizzare di quali elementi del file viene eseguito il mapping ai campi in [!INCLUDE[d365fin](includes/d365fin_md.md)] durante l'importazione di file di estratto conto SEPA CAMT.</span><span class="sxs-lookup"><span data-stu-id="a6b57-126">View which file elements are mapped to fields in [!INCLUDE[d365fin](includes/d365fin_md.md)] when importing SEPA CAMT statement files.</span></span>|[<span data-ttu-id="a6b57-127">Mapping dei campi durante l'importazione dei file SEPA CAMT</span><span class="sxs-lookup"><span data-stu-id="a6b57-127">Field Mapping When Importing SEPA CAMT Files</span></span>](across-field-mapping-when-importing-sepa-camt-files.md)|  
|<span data-ttu-id="a6b57-128">Visualizzare i campi in [!INCLUDE[d365fin](includes/d365fin_md.md)] di cui viene eseguito il mapping agli elementi del file durante l'esportazione dei file di pagamento tramite la funzionalità del servizio di conversione dati bancari.</span><span class="sxs-lookup"><span data-stu-id="a6b57-128">View which fields in [!INCLUDE[d365fin](includes/d365fin_md.md)] are mapped to file elements when exporting payment files by using the Bank Date Conversion Service feature.</span></span>|[<span data-ttu-id="a6b57-129">Mapping dei campi durante l'esportazione dei file di pagamento tramite il servizio di conversione dati bancari</span><span class="sxs-lookup"><span data-stu-id="a6b57-129">Field Mapping When Exporting Payment Files Using Bank Data Conversion Service</span></span>](across-field-mapping-when-exporting-payment-files-using-bank-data-conversion-service.md)|  

## <a name="see-also"></a><span data-ttu-id="a6b57-130">Vedi anche</span><span class="sxs-lookup"><span data-stu-id="a6b57-130">See Also</span></span>  
[<span data-ttu-id="a6b57-131">Impostazione dello scambio di dati</span><span class="sxs-lookup"><span data-stu-id="a6b57-131">Setting Up Data Exchange</span></span>](across-set-up-data-exchange.md)  
[<span data-ttu-id="a6b57-132">Scambio di dati in modalità elettronica</span><span class="sxs-lookup"><span data-stu-id="a6b57-132">Exchanging Data Electronically</span></span>](across-data-exchange.md)  
<span data-ttu-id="a6b57-133">[Procedura: Fatturare le vendite](sales-how-invoice-sales.md) </span><span class="sxs-lookup"><span data-stu-id="a6b57-133">[How to: Invoice Sales](sales-how-invoice-sales.md) </span></span>  
[<span data-ttu-id="a6b57-134">Procedura: Registrare gli acquisti</span><span class="sxs-lookup"><span data-stu-id="a6b57-134">How to: Record Purchases</span></span>](purchasing-how-record-purchases.md)  
[<span data-ttu-id="a6b57-135">Documenti in entrata</span><span class="sxs-lookup"><span data-stu-id="a6b57-135">Incoming Documents</span></span>](across-income-documents.md)  
[<span data-ttu-id="a6b57-136">Funzionalità aziendali generali</span><span class="sxs-lookup"><span data-stu-id="a6b57-136">General Business Functionality</span></span>](ui-across-business-areas.md)  
