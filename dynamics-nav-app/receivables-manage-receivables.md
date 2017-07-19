---
title: "Gestire la contabilità clienti"
author: SorenGP
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: 3f2be627dfda9720e9f31fd227164d1c27116d2c
ms.contentlocale: it-it
ms.lasthandoff: 06/26/2017

---

# <a name="manage-receivables"></a>Gestire la contabilità clienti#
Un'attività centrale nella gestione della contabilità clienti è il collegamento dei pagamenti in entrata ai relativi movimenti contabili clienti o fornitori e la conseguente chiusura delle fatture di vendita o delle note di credito di acquisto come pagate. Una volta che tutti i pagamenti sono collegati, è possibile riconciliare il conto corrente bancario.  

Questa operazione può essere eseguita nella finestra **Registrazione riconciliazione pagamenti** importando un file di rendiconto della banca o un feed per registrare rapidamente i pagamenti in Dynamics NAV. Una funzione di collegamento automatico collega i pagamenti ai relativi movimenti contabili clienti o fornitori aperti correlati in base alle corrispondenze tra il testo di pagamento e le informazioni del movimento. È possibile rivedere e modificare i collegamenti automatici prima di effettuare la registrazione. Quando si effettua la registrazione, è possibile scegliere di chiudere qualsiasi movimento contabile di conto corrente bancario aperto correlato ai movimenti contabili. Questo significa che il conto bancario viene automaticamente riconciliato una volta che tutti i pagamenti sono collegati.

**Nota**: è possibile riconciliare i conti bancari come attività separata nella finestra **Riconciliazioni C/C bancari** che supporta anche i movimenti contabili assegni. Per ulteriori informazioni, vedere [Procedura: Riconciliare i conti bancari separatamente](bank-how-reconcile-bank-accounts-separately.md).

In alternativa, è possibile collegare i pagamenti nella finestra **Registrazione pagamenti** spuntando manualmente i pagamenti ricevuti come contante, assegno o transazione bancaria rispetto a una lista generata di documenti di vendita non pagati. Notare che questa funzionalità è disponibile solo per i documenti di vendita.

Un'altra modalità di riconciliazione manuale dei pagamenti prevede che si registri ogni ricezione nel relativo conto COGE, cliente o altro immettendo una riga di pagamento nella finestra **Registrazioni incassi**. In questo caso, è possibile collegare la ricezione o il rimborso a uno o più movimenti aperti prima di contabilizzare le registrazioni incassi oppure è possibile eseguire il collegamento dai movimenti contabili clienti creati.

Un'altra attività di gestione della contabilità clienti riguarda la riscossione dei saldi inevasi, inclusa la gestione degli addebiti interessi e l'emissione dei solleciti.

Nella tabella seguente viene descritta una sequenza di task, con collegamenti agli argomenti che li descrivono.

|Per |Vedere |
|---|----|
|Collegare i pagamenti a movimenti contabili cliente o fornitore aperti in base a un feed bancario o un file di rendiconto bancario importato e riconciliare il conto bancario una volta che tutti i pagamenti sono collegati.|[Collegare i pagamenti automaticamente e riconciliare i conti correnti bancari](receivables-apply-payments-auto-reconcile-bank-accounts.md)|
|Collegare i pagamenti a movimenti contabili clienti aperti in base all'immissione manuale in una lista di documenti di vendita non pagati. | [Procedura: Riconciliare i pagamenti dei clienti manualmente dall'elenco dei documenti di vendita non pagati](receivables-how-reconcile-customer-payments-list-unpaid-sales-documents.md)|
|Registrare gli incassi o i rimborsi per i clienti nelle registrazioni incassi e collegare ai movimenti contabili clienti, dalle registrazioni o dai movimenti contabili registrati. | [Procedura: Riconciliare manualmente i pagamenti dei clienti](receivables-how-apply-sales-transactions-manually.md) |
|Inviare solleciti ai clienti per gli importi insoluti, calcolare interessi e addebiti interessi e gestire i crediti verso i clienti. | [Procedura: Riscuotere i saldi inevasi](receivables-collect-outstanding-balances.md) |

## <a name="see-also"></a>Vedi anche
[Gestire le vendite](sales-manage-sales.md)  
[Gestire la contabilità fornitori](payables-manage-payables.md)  
[Utilizzare Dynamics NAV](ui-work-product.md)  
[Tra le aree aziendali](ui-across-business-areas.md)

