---
title: Impostare lo scambio di dati
description: Impostare il framework di scambio dati in Dynamics NAV.
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/21/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: bd45b6a3d0a611154828a0c9b6a8e39fe1c14635
ms.contentlocale: it-it
ms.lasthandoff: 10/16/2017

---
# <a name="setting-up-data-exchange"></a><span data-ttu-id="dd382-103">Impostazione dello scambio di dati</span><span class="sxs-lookup"><span data-stu-id="dd382-103">Setting Up Data Exchange</span></span>
<span data-ttu-id="dd382-104">Prima di poter inviare e ricevere documenti elettronici o importare ed esportare file della banca, è necessario impostare il framework di scambio dati per elaborare i file interessati.</span><span class="sxs-lookup"><span data-stu-id="dd382-104">Before you can send and receive electronic documents or import and export bank files, you must set up the data exchange framework to process the involved files.</span></span> <span data-ttu-id="dd382-105">Inoltre, è necessario impostare le aree correlate, ad esempio i dati principali per i clienti a cui si inviano fatture elettroniche o il servizio di conversione dati bancari nel caso in cui si utilizzi il provider di servizi esterno per convertire i propri file bancari.</span><span class="sxs-lookup"><span data-stu-id="dd382-105">In addition, you must set up related areas, such as master data for customers that you send electronic invoices to or the bank data conversion service in case you use the external service provider to convert your bank files.</span></span> <span data-ttu-id="dd382-106">Per ulteriori informazioni, vedere [Scambio di dati in modalità elettronica](across-data-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="dd382-106">For more information, see [Exchanging Data Electronically](across-data-exchange.md).</span></span>  

 <span data-ttu-id="dd382-107">Se [!INCLUDE[d365fin](includes/d365fin_md.md)] è impostato per scambiare i dati con file esterni, gli utenti possono utilizzare l'impostazione in task aziendali comuni, ad esempio l'invio e la ricezione di documenti elettronici, nonché l'importazione e l'esportazione di file bancari.</span><span class="sxs-lookup"><span data-stu-id="dd382-107">When [!INCLUDE[d365fin](includes/d365fin_md.md)] is set up to exchange data with external files, users can use the setup in common business tasks, such as sending and receiving electronic documents and importing and exporting bank files.</span></span>  

 <span data-ttu-id="dd382-108">Nella tabella seguente viene descritta una sequenza di task, con collegamenti agli argomenti che li descrivono.</span><span class="sxs-lookup"><span data-stu-id="dd382-108">The following table describes a sequence of tasks, with links to the topics that describe them.</span></span>  

|<span data-ttu-id="dd382-109">**Task**</span><span class="sxs-lookup"><span data-stu-id="dd382-109">**To**</span></span>|<span data-ttu-id="dd382-110">**Vedere**</span><span class="sxs-lookup"><span data-stu-id="dd382-110">**See**</span></span>|  
|------------|-------------|  
|<span data-ttu-id="dd382-111">Impostare il servizio di scambio documenti preconfigurato per abilitare l'invio e la ricezione dei documenti elettronici da e a [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="dd382-111">Set up the preconfigured document exchange service to enable sending and receiving electronic documents from and to [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span>|[<span data-ttu-id="dd382-112">Procedura: Impostare un servizio di scambio documenti</span><span class="sxs-lookup"><span data-stu-id="dd382-112">How to: Set Up a Document Exchange Service</span></span>](across-how-to-set-up-a-document-exchange-service.md)|  
|<span data-ttu-id="dd382-113">Configurare il servizio OCR preconfigurato per convertire i file PDF o di immagine in documenti elettronici che possono essere convertiti in record di documento in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="dd382-113">Set up the preconfigured OCR service to turn PDF or image files into electronic documents that can be converted to document records in [!INCLUDE[d365fin](includes/d365fin_md.md)]</span></span>|[<span data-ttu-id="dd382-114">Procedura: Impostare documenti in entrata</span><span class="sxs-lookup"><span data-stu-id="dd382-114">How to: Set Up Incoming Documents</span></span>](across-how-setup-income-documents.md)|  
|<span data-ttu-id="dd382-115">Configurare uno dei due servizi preconfigurati per i tassi di cambio aggiornati in modo da ottenere i tassi di cambio valuta più recenti nella finestra **Valute**.</span><span class="sxs-lookup"><span data-stu-id="dd382-115">Set up one of two preconfigured services for updated exchange rates to get the latest currency exchange rates into the **Currencies** window.</span></span>|[<span data-ttu-id="dd382-116">Procedura: Aggiornare i tassi di cambio delle valute</span><span class="sxs-lookup"><span data-stu-id="dd382-116">How to: Update Currency Exchange Rates</span></span>](finance-how-update-currencies.md)|  
|<span data-ttu-id="dd382-117">È necessario impostare diversi dati master, ad esempio le informazioni sulla società, i clienti, i fornitori, gli articoli e le unità di misura correlati ai dati di mapping in [!INCLUDE[d365fin](includes/d365fin_md.md)]</span><span class="sxs-lookup"><span data-stu-id="dd382-117">Set up various master data, such as company information, customers, vendors, items, and units of measure, related to mapping data in [!INCLUDE[d365fin](includes/d365fin_md.md)]</span></span>|[<span data-ttu-id="dd382-118">Procedura: Impostare l'invio e la ricezione di documenti elettronici</span><span class="sxs-lookup"><span data-stu-id="dd382-118">How to: Set Up Electronic Document Sending and Receiving</span></span>](across-how-to-set-up-electronic-document-sending-and-receiving.md)|  
|<span data-ttu-id="dd382-119">Impostare un conto corrente bancario, un fornitore e le registrazioni pagamenti per bonifici SEPA.</span><span class="sxs-lookup"><span data-stu-id="dd382-119">Set up a bank account, a vendor, and a payment journal for SEPA credit transfer.</span></span>|[<span data-ttu-id="dd382-120">Procedura: Impostare il bonifico SEPA</span><span class="sxs-lookup"><span data-stu-id="dd382-120">How to: Set Up SEPA Credit Transfer</span></span>](finance-how-to-set-up-sepa-credit-transfer.md)|  
|<span data-ttu-id="dd382-121">Preparare i formati dei conti bancari, i metodi di pagamento e gli accordi con i clienti per l'addebito diretto SEPA.</span><span class="sxs-lookup"><span data-stu-id="dd382-121">Prepare bank account formats, payment methods, and customer agreements for SEPA direct debit.</span></span>|[<span data-ttu-id="dd382-122">Procedura: Impostare gli addebiti diretti SEPA</span><span class="sxs-lookup"><span data-stu-id="dd382-122">How to: Set Up SEPA Direct Debit</span></span>](finance-how-to-set-up-sepa-direct-debit.md)|  
|<span data-ttu-id="dd382-123">Impostare l'autenticazione utente e l'URL del provider di servizi di conversione di dati bancari che è necessario per convertire i file della banca nel formato della banca in uso.</span><span class="sxs-lookup"><span data-stu-id="dd382-123">Set up user authentication and the URL of the bank data conversion service provider that is required to have bank files converted to your bank’s format.</span></span>|[<span data-ttu-id="dd382-124">Procedura: Impostare il servizio di conversione di dati bancari</span><span class="sxs-lookup"><span data-stu-id="dd382-124">How to: Set Up the Bank Data Conversion Service</span></span>](bank-how-setup-bank-data-conversion-service.md)|  
|<span data-ttu-id="dd382-125">Impostare e abilitare un servizio esterno che consente di importare gli estratti conto bancari direttamente come feed bancari.</span><span class="sxs-lookup"><span data-stu-id="dd382-125">Set up and enable an external service that enables you to import bank statements directly as bank feeds.</span></span>|[<span data-ttu-id="dd382-126">Procedura: Impostare il servizio di conversione di dati bancari</span><span class="sxs-lookup"><span data-stu-id="dd382-126">How to: Set Up the Bank Data Conversion Service</span></span>](bank-how-setup-bank-data-conversion-service.md)|  
|<span data-ttu-id="dd382-127">Una volta abilitato il servizio di conversione dati bancari, collegare i conti correnti bancari in [!INCLUDE[d365fin](includes/d365fin_md.md)]</span><span class="sxs-lookup"><span data-stu-id="dd382-127">After the bank data conversion service is enabled, link bank accounts in [!INCLUDE[d365fin](includes/d365fin_md.md)]</span></span>|[<span data-ttu-id="dd382-128">Procedura: Impostare i conti correnti bancari</span><span class="sxs-lookup"><span data-stu-id="dd382-128">How to: Set Up Bank Accounts</span></span>](bank-how-setup-bank-accounts.md)|  
|<span data-ttu-id="dd382-129">Preparare l'impostazione di una nuova definizione di scambio di dati per un file o un flusso di dati utilizzando lo schema XML del file per precompilare la Scheda dettaglio **Definizioni colonne** nella finestra **Registrazione definizioni di scambio**.</span><span class="sxs-lookup"><span data-stu-id="dd382-129">Prepare to set up a new data exchange definition for a data file or stream by using the file’s XML schema to prefill the **Column Definitions** FastTab in the **Posting Exchange Definition** window.</span></span>|[<span data-ttu-id="dd382-130">Procedura: Utilizzare gli schemi XML per preparare le definizioni di scambio dati</span><span class="sxs-lookup"><span data-stu-id="dd382-130">How to: Use XML Schemas to Prepare Data Exchange Definitions</span></span>](across-how-to-use-xml-schemas-to-prepare-data-exchange-definitions.md)|  
|<span data-ttu-id="dd382-131">Impostare il framework di scambio dei dati per consentire agli utenti di ricevere un nuovo formato di documenti di acquisto, inviare un nuovo formato di documenti di vendita, importare un nuovo file bancario o altri tipi di scambio di dati.</span><span class="sxs-lookup"><span data-stu-id="dd382-131">Set up the Data Exchange Framework to enable users to receive a new purchase document format, send a new sales document format, import a new bank file, or other data exchange.</span></span>|[<span data-ttu-id="dd382-132">Procedura: Impostare le definizioni di scambio di dati</span><span class="sxs-lookup"><span data-stu-id="dd382-132">How to: Set Up Data Exchange Definitions</span></span>](across-how-to-set-up-data-exchange-definitions.md)|  

## <a name="see-also"></a><span data-ttu-id="dd382-133">Vedi anche</span><span class="sxs-lookup"><span data-stu-id="dd382-133">See Also</span></span>  
[<span data-ttu-id="dd382-134">Scambio di dati in modalità elettronica</span><span class="sxs-lookup"><span data-stu-id="dd382-134">Exchanging Data Electronically</span></span>](across-data-exchange.md)  
<span data-ttu-id="dd382-135">[Scambio di dati](across-exchange-data.md) </span><span class="sxs-lookup"><span data-stu-id="dd382-135">[Exchanging Data](across-exchange-data.md) </span></span>  
[<span data-ttu-id="dd382-136">Documenti in entrata</span><span class="sxs-lookup"><span data-stu-id="dd382-136">Incoming Documents</span></span>](across-income-documents.md)  
[<span data-ttu-id="dd382-137">Funzionalità aziendali generali</span><span class="sxs-lookup"><span data-stu-id="dd382-137">General Business Functionality</span></span>](ui-across-business-areas.md)  
