---
title: Impostazione di valori suggeriti per i campi
description: "Per evitare i calcoli manuali e per completare i task in modo rapido e accurato, è possibile impostare l'immissione automatica dei dati in modo che Dynamics NAV compili i campi selezionati."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.date: 08/15/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 7c68019ff32d6fbe700975b0897dff9474da7bc1
ms.contentlocale: it-it
ms.lasthandoff: 10/16/2017

---
# <a name="letting-included365finincludesd365finmdmd-suggest-values"></a>Suggerimento automatico dei valori in [!INCLUDE[d365fin](includes/d365fin_md.md)]
[!INCLUDE[d365fin](includes/d365fin_md.md)] può aiutare a completare le attività in modo più rapido e più corretto precompilando campi o righe intere con dati che verrebbero altrimenti calcolati e immessi manualmente. Sebbene tale l'immissione dei dati automatica sia sempre corretta, è possibile modificarla in seguito se lo si desidera.

La funzionalità che fornisce in automatico i valori dei campi è in genere offerta per le attività in cui si devono immettere grandi volumi di dati transazionali e per cui si desidera evitare errori e risparmiare tempo. Questo argomento contiene una selezione di tale funzionalità. Nei futuri aggiornamenti di [!INCLUDE[d365fin](includes/d365fin_md.md)] verranno aggiunte altre sezioni.

## <a name="the-suggest-balancing-amount-check-box-in-the-general-journal-batches-window"></a>La casella di controllo **Suggerisci importo contropartita** nella finestra **Batch registrazioni COGE**
Se, ad esempio, si intende immettere delle righe di registrazione COGE per più spese che devono essere contabilizzate nello stesso conto bancario, ogni volta che si immette una riga di registrazione COGE per una spesa, è possibile fare in modo che il campo **Importo** del conto bancario venga aggiornato automaticamente all'importo che bilancia le spese. Per ulteriori informazioni sull'utilizzo delle registrazioni COGE, vedere [Utilizzo delle registrazioni COGE](ui-work-general-journals.md).

### <a name="to-have-the-amount-field-on-balancing-general-journal-lines-filled-automatically"></a>Per compilare automaticamente il campo **Importo** nelle righe di registrazione COGE di contropartita
1. Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "Cerca pagina o report"), immettere **Registrazioni COGE**, quindi scegliere il collegamento correlato.
2. Nella riga del batch delle registrazioni COGE preferito, selezionare la casella di controllo **Suggerisci importo contropartita**.
3. Aprire le registrazioni COGE e procedere a registrare e contabilizzare le transazioni utilizzando la funzionalità descritta per l'immissione automatica di un valore nel campo.       

Per informazioni su come impostare un batch registrazioni COGE personale, ad esempio per la gestione delle spese, vedere [Utilizzo delle registrazioni COGE](ui-work-general-journals.md).

## <a name="the-automatically-fill-date-received-field-in-the-payment-registration-window"></a>Il campo **Compila automaticamente data di ricezione** nella finestra **Registrazione pagamenti**
Nella finestra **Registrazione pagamenti** vengono mostrati i pagamenti in entrata inevasi come righe che rappresentano i documenti di vendita in cui è dovuto il pagamento di un importo. Per ulteriori informazioni sul collegamento dei pagamenti dei clienti, vedere [Procedura: Riconciliare i pagamenti dei clienti manualmente dall'elenco dei documenti di vendita non pagati](receivables-how-reconcile-customer-payments-list-unpaid-sales-documents.md).

Le principali azioni che deve effettuare l'utente nella finestra sono la selezione della casella di controllo **Pagamento effettuato** e la compilazione del campo **Data ricezione**. È possibile impostare [!INCLUDE[d365fin](includes/d365fin_md.md)] in modo che inserisca automaticamente la data di lavoro nel campo **Data ricezione** quando si seleziona la casella di controllo **Pagamento effettuato**.

### <a name="to-have-the-date-received-field-in-the-payment-registration-window-filled-automatically"></a>Per compilare automaticamente il campo **Data ricezione** nella finestra **Registrazione pagamenti**
1. Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "Cerca pagina o report"), immettere **Setup registrazione pagamenti**, quindi scegliere il collegamento correlato.
2. Selezionare la casella di controllo **Compila automaticamente data di ricezione**.
3. Aprire la finestra **Registrazione pagamenti** e procedere con l'elaborazione dei pagamenti clienti in entrata utilizzando la funzionalità descritta per l'immissione automatica di un valore di campo.

## <a name="see-also"></a>Vedi anche
[Utilizzo di [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)  
[Finanze](finance.md)

