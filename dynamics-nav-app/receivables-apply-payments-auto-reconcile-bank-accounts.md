---
title: Collegare i pagamenti automaticamente e riconciliare i conti correnti bancari
author: SorenGP
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: 11df387c16e19421090531fd03c209103b9989d9
ms.contentlocale: it-it
ms.lasthandoff: 06/26/2017

---

# <a name="apply-payments-automatically-and-reconcile-bank-accounts"></a>Collegare i pagamenti automaticamente e riconciliare i conti correnti bancari
È necessario riconciliare periodicamente i conti debiti, crediti e bancari in Dynamics NAV collegando i pagamenti registrati nella banca alle relative fatture non pagate o note di credito o altri movimenti aperti in Dynamics NAV.

Questa operazione può essere eseguita nella finestra **Registrazione riconciliazione pagamenti** importando un file di rendiconto della banca o un feed per registrare rapidamente i pagamenti in Dynamics NAV. Una funzione di collegamento automatico collega i pagamenti ai relativi movimenti contabili clienti o fornitori aperti correlati in base alle corrispondenze tra il testo di pagamento e le informazioni del movimento. È possibile rivedere e modificare i collegamenti automatici prima di effettuare la registrazione. Quando si effettua la registrazione, è possibile scegliere di chiudere qualsiasi movimento contabile di conto corrente bancario aperto correlato ai movimenti contabili. Questo significa che il conto bancario viene automaticamente riconciliato una volta che tutti i pagamenti sono collegati.

Per abilitare l'importazione degli estratti conto bancari come feed bancario, è necessario innanzitutto abilitare il servizio Feed bancario di Envestnet Yodlee e successivamente collegare i conti correnti bancari ai conti bancari in linea correlati. Per ulteriori informazioni, vedere [Procedura: Impostare il servizio di Feed bancario di Envestnet Yodlee](bank-how-setup-bank-statement-service.md).

**Nota**: il servizio Feed bancari di Envestnet Yodlee o un altro servizio di feed bancari del fornitore potrebbe non essere disponibile nel sistema. Contattare il partner di Microsoft se si desidera utilizzare un servizio di feed bancari per importare gli estratti conto.

In alternativa, è possibile utilizzare il servizio di conversione di dati bancari per convertire un file di rendiconto bancario da un formato qualsiasi in un flusso di dati importabile in Dynamics NAV. Per ulteriori informazioni, vedere [Procedura: Impostare il servizio di conversione di dati bancari](bank-how-setup-bank-data-conversion-service.md).

Nella tabella seguente viene descritta una sequenza di task, con collegamenti agli argomenti che li descrivono.

|Per |Vedere |
|---|----|
|Collegare i pagamenti per aprire i movimenti contabili cliente o fornitore importando un rendiconto bancario e riconciliare il conto corrente bancario quando tutti i pagamenti sono collegati. | [Procedura: Riconciliare i pagamenti utilizzando il collegamento automatico](receivables-how-reconcile-payments-auto-application.md) |
|Collegare manualmente i pagamenti visualizzando le informazioni dettagliate sui dati corrispondenti e i suggerimenti sui movimenti aperti da collegare ai pagamenti. | [Procedura: Esaminare o collegare i pagamenti in seguito al collegamento automatico](receivables-how-review-apply-payments-auto-application.md)
|Risolvere i pagamenti che non possono essere collegati automaticamente ai relativi movimenti contabili aperti, ad esempio per differenze di importi o perché il movimento contabile corrispondente non esiste. | [Procedura: Riconciliare i pagamenti che non possono essere collegati automaticamente](receivables-how-reconcile-payments-cannot-apply-auto.md)
|Collegare il testo sui pagamenti a specifici conti cliente, fornitore o di contabilità generale per registrare sempre incassi o spese ricorrenti in tali conti quando non esistono documenti da applicare.| [Procedura: Mappatura del testo nei pagamenti ricorrenti a conti per la riconciliazione automatica](receivables-how-map-text-recurring-payments-accounts-auto-reconcilliation.md)|

## <a name="see-also"></a>Vedi anche
[Gestire la contabilità clienti](receivables-manage-receivables.md)  
[Gestire le vendite](sales-manage-sales.md)

