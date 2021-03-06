---
title: Scambiare dati
description: "È possibile scambiare i dati tra [!INCLUDE[d365fin](includes/d365fin_md.md)] e flussi o file esterni in relazione alle attività aziendali, come l'invio e la ricezione di documenti elettronici e l'importazione e l'esportazione di file dalla banca."
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/18/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: b9b1f062ee6009f34698ea2cf33bc25bdd5b11e4
ms.openlocfilehash: d83e68f31edf2dee9e3e5bc5b73a4861cfe919d7
ms.contentlocale: it-it
ms.lasthandoff: 10/23/2017

---
# <a name="exchanging-data"></a>Scambio di dati
È possibile scambiare i dati tra [!INCLUDE[d365fin](includes/d365fin_md.md)] e flussi o file esterni in relazione alle attività aziendali, come l'invio e la ricezione di documenti elettronici e l'importazione e l'esportazione di file dalla banca.  

Prima di poter inviare e ricevere documenti elettronici o importare ed esportare file bancari, è necessario impostare il framework di scambio dati per elaborare i flussi o i file di dati interessati. Inoltre, è necessario impostare delle aree correlate. Sono inclusi i dati master per i clienti a cui si inviano fatture elettroniche e il servizio di conversione di dati bancari nel caso si distribuiscano traduzioni di file della banca a un provider di servizi esterno. Per ulteriori informazioni, vedere [Impostazione dello scambio di dati](across-set-up-data-exchange.md).  

 Nella tabella seguente viene descritta una sequenza di task, con collegamenti agli argomenti che li descrivono.  

|**Task**|**Vedere**|  
|------------|-------------|  
|Convertire i record del documento di vendita in [!INCLUDE[d365fin](includes/d365fin_md.md)] in un formato standardizzato e inviarli come documenti elettronici che i clienti possono ricevere nel proprio sistema.|[Procedura: Inviare documenti elettronici](sales-how-to-send-electronic-documents.md)|  
|Inviare PDF o file immagine a un provider di servizi OCR e riceverli come documenti elettronici che possono essere convertiti in record di documento in [!INCLUDE[d365fin](includes/d365fin_md.md)].|[Procedura: Utilizzare OCR per convertire PDF e file di immagine in documenti elettronici](across-how-use-ocr-pdf-images-files.md)|  
|Ricevere i documenti elettronici dal servizio OCR o dal servizio di scambio documenti in un formato standardizzato che viene convertito nei relativi record di documento in [!INCLUDE[d365fin](includes/d365fin_md.md)].|[Procedura: Ricevere e convertire documenti elettronici](purchasing-how-to-receive-and-convert-electronic-documents.md)|  
|Importare un file dell'estratto conto bancario nella finestra **Registrazione riconciliazione pagamenti** come primo passaggio della riconciliazione dei pagamenti o nella finestra **Riconciliazioni C/C bancari** come primo passaggio nella riconciliazione dei conti bancari.|[Collegare i pagamenti automaticamente e riconciliare i conti correnti bancari](receivables-apply-payments-auto-reconcile-bank-accounts.md)|  
|Esportare i pagamenti dalla finestra **Registrazioni pagamenti** in un file della banca da caricare sul conto corrente bancario elettronico per l'elaborazione.|[Procedura: esportare pagamenti in un file della banca](payables-how-export-payments-bank-file.md)|  
|Indicare alla propria banca di trasferire gli importi dei pagamenti dai conti bancari dei clienti a quello della propria società in base al setup dell'addebito diretto SEPA.|[Procedura: Creare movimenti riscossione addebiti diretti SEPA ed esportarli in un file della banca](finance-how-create-sepa-direct-debit-collection-entries-export-bank-file.md)|  
|Utilizzare un provider di servizi per i tassi di cambio valuta per aggiornare la finestra **Valute**.|[Procedura: Aggiornare i tassi di cambio delle valute](finance-how-update-currencies.md)|  
|Visualizzare di quali elementi del file viene eseguito il mapping ai campi in [!INCLUDE[d365fin](includes/d365fin_md.md)] durante l'importazione di file di estratto conto SEPA CAMT.|[Mapping dei campi durante l'importazione dei file SEPA CAMT](across-field-mapping-when-importing-sepa-camt-files.md)|  
|Visualizzare i campi in [!INCLUDE[d365fin](includes/d365fin_md.md)] di cui viene eseguito il mapping agli elementi del file durante l'esportazione dei file di pagamento tramite la funzionalità del servizio di conversione dati bancari.|[Mapping dei campi durante l'esportazione dei file di pagamento tramite il servizio di conversione dati bancari](across-field-mapping-when-exporting-payment-files-using-bank-data-conversion-service.md)|  

## <a name="see-also"></a>Vedi anche  
[Impostazione dello scambio di dati](across-set-up-data-exchange.md)  
[Scambio di dati in modalità elettronica](across-data-exchange.md)  
[Procedura: Fatturare le vendite](sales-how-invoice-sales.md)   
[Procedura: Registrare gli acquisti](purchasing-how-record-purchases.md)  
[Documenti in entrata](across-income-documents.md)  
[Funzionalità aziendali generali](ui-across-business-areas.md)  

