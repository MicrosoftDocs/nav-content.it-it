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
# <a name="how-to-issue-vendor-payments-and-customer-bills"></a>Procedura: Emettere pagamenti fornitori ed effetti clienti
La funzionalità di pagamento degli effetti cliente e fornitore supporta i formati SEPA oltre ai formati di file italiani. È possibile pagare i fornitori in base al bonifico SEPA standard e riscuotere i pagamenti dai clienti in base al metodo di addebito diretto SEPA standard. Di seguito viene descritto il processo per l'invio del pagamento a un fornitore con bonifico SEPA. I passaggi sono simili per la riscossione del pagamento da un cliente.  

 Prima di avviare la seguente procedura, controllare che le informazioni sulla banca della società siano state immesse nella finestra **Scheda conto corrente bancario**. Nella scheda. includere le informazioni per i seguenti campi:  

-   IBAN  

-   Codice SWIFT (facoltativo)  

-   Formato esportazione pagamento  

-   Nr serie ID msg CT SEPA Serie  

 Inoltre, occorre inserire una fattura di acquisito registrata e con cui è possibile inviare un pagamento.  

### <a name="to-issue-payment-to-a-vendor"></a>Per emettere il pagamento per un fornitore  

1.  Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **Fornitori**, quindi scegliere il collegamento correlato.  

2.  Selezionare il fornitore al quale si desidera inviare il pagamento. Nella Scheda dettaglio **Pagamento**, nel campo **Codice metodo di pagamento** scegliere **TRASFBANC**. Nel gruppo **Fornitore** della scheda **Naviga** selezionare **C/C bancari**.  

3.  Nella **Lista C/C bancari fornitori**, selezionare il conto C/C bancari del fornitore e nella scheda **Pagina iniziale**, nel gruppo **Gestisci**, scegliere **Modifica**. Nella Scheda dettaglio **Trasferimento**, specificare le informazioni relative al campo **IBAN**.  

     Scegliere il pulsante **OK**.  

4.  Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "Cerca pagina o report"), immettere **Distinta fornitore**, quindi selezionare il collegamento correlato.  

5.  Nel gruppo **Gestisci** della scheda **Pagina iniziale** scegliere **Nuovo**.  

6.  Nella Scheda dettaglio **Generale**, immettere le informazioni nei seguenti campi: **Nr. conto bancario** del fornitore e **Codice metodo di pagamento**.  

7.  Nel gruppo **Processo** della scheda **Pagina iniziale** scegliere **Suggerisci pagamenti**. Impostare i filtri appropriati e scegliere il pulsante **OK** per eseguire il processo batch.  

8.  Nel gruppo **Processo** della scheda **Pagina iniziale** scegliere **Crea distinta**. Scegliere il pulsante **Sì** per inviare il pagamento dell'effetto.  

9. Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **Distinta effetti fornitore emessa** e selezionare il pagamento dell'effetto emesso dall'elenco. Nella scheda **Pagina iniziale** selezionare **Modifica**. Verrà aperta la finestra **Distinta effetti forn. emessa**.  

10. Per esportare le informazioni di pagamento, nella scheda **Pagina iniziale**, nel gruppo **Report**, scegliere una delle seguenti opzioni: **Esporta distinta effetti su file**. È possibile visualizzare il file XML inviato.  

    1.  Esportare nel file (per file in formato SEPA standard)  

    2.  Esporta distinta effetti su file  

     È possibile visualizzare il file XML prima di inviarlo. Per esaminare e correggere gli errori, è possibile fare riferimento al riquadro dettaglio informazioni **Errori esportazione file** creato.  

## <a name="see-also"></a>Vedi anche  
 [Eseguire i pagamenti con il servizio di conversione dati bancari o bonifico SEPA](finance-make-payments-with-bank-data-conversion-service-or-sepa-credit-transfer.md)   
 [Procedura: Impostare il trasferimento crediti SEPA](../../finance-how-to-set-up-sepa-credit-transfer.md)   
 [Riscuotere pagamenti con addebito diretto SEPA](../../finance-collect-payments-with-sepa-direct-debit.md)

