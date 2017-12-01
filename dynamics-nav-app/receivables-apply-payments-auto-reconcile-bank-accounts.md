---
title: Task per la riconciliazione dei conti correnti bancari e il collegamento dei pagamenti ai relativi movimenti
description: "Descrive i task per riconciliare conti correnti bancari, conti di contabilità clienti, fornitori, registrazione incassi o spese e per applicare i pagamenti automaticamente."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: payment process, direct payment posting, reconcile payment, expenses, cash receipts
ms.date: 03/29/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: b9b1f062ee6009f34698ea2cf33bc25bdd5b11e4
ms.openlocfilehash: 33c0661a2ebf9b8d9b817c026a8c9abf0f0eff91
ms.contentlocale: it-it
ms.lasthandoff: 10/23/2017

---
# <a name="applying-payments-automatically-and-reconciling-bank-accounts"></a>Collegare i pagamenti automaticamente e riconciliare i conti correnti bancari
È necessario riconciliare periodicamente i conti debiti, crediti e bancari collegando i pagamenti registrati nella banca alle relative fatture non pagate e note di credito o altri movimenti aperti in [!INCLUDE[d365fin](includes/d365fin_long_md.md)].  

Questa operazione può essere eseguita nella finestra **Registrazione riconciliazione pagamenti** importando un file di rendiconto della banca o un feed per registrare rapidamente i pagamenti. I pagamenti sono collegati ai movimenti contabili aperti per clienti o fornitori in base alle corrispondenze tra il testo di pagamento e le informazioni del movimento. È possibile rivedere e modificare i collegamenti automatici prima di effettuare la registrazione. Quando si effettua la registrazione, è possibile scegliere di chiudere qualsiasi movimento contabile di conto corrente bancario aperto correlato ai movimenti contabili. Il conto bancario viene automaticamente riconciliato una volta che tutti i pagamenti sono collegati.  

Per importare rendiconti bancari come un feed bancari, è necessario innanzitutto impostare e abilitare il servizio di conversione dati bancari. Per ulteriori informazioni, vedere [Procedura: Impostare il servizio di conversione di dati bancari](bank-how-setup-bank-data-conversion-service.md).  

Nella tabella seguente viene descritta una sequenza di task, con collegamenti agli argomenti che li descrivono.  

| Per | Vedere |
| --- | --- |
| Collegare i pagamenti per aprire i movimenti contabili cliente o fornitore importando un rendiconto bancario e riconciliare il conto corrente bancario quando tutti i pagamenti sono collegati. |[Procedura: Riconciliare i pagamenti utilizzando il collegamento automatico](receivables-how-reconcile-payments-auto-application.md) |
| Collegare manualmente i pagamenti visualizzando le informazioni dettagliate sui dati corrispondenti e i suggerimenti sui movimenti aperti da collegare ai pagamenti. |[Procedura: Esaminare o collegare i pagamenti in seguito al collegamento automatico](receivables-how-review-apply-payments-auto-application.md) |
| Risolvere i pagamenti che non possono essere collegati automaticamente ai movimenti contabili aperti correlati. Ad esempio perché gli importi differiscono o perché non esiste un movimento contabile correlato. |[Procedura: Riconciliare i pagamenti che non possono essere collegati automaticamente](receivables-how-reconcile-payments-cannot-apply-auto.md) |
| Collegare il testo sui pagamenti a specifici conti cliente, fornitore o di contabilità generale per registrare sempre incassi o spese ricorrenti in tali conti quando non esistono documenti da applicare. |[Procedura: Mappatura del testo nei pagamenti ricorrenti a conti per la riconciliazione automatica](receivables-how-map-text-recurring-payments-accounts-auto-reconcilliation.md) |

## <a name="see-also"></a>Vedi anche
[Gestione della contabilità clienti](receivables-manage-receivables.md)  
[Vendite](sales-manage-sales.md)  
[Utilizzo di [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

