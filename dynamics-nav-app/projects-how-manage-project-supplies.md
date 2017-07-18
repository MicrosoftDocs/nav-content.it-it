---
title: 'Procedura: Gestire gli approvvigionamenti per un progetto'
author: SorenGP
ms.custom: na
ms.date: 11/01/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: 00b9ed8480f6b5ab9265beb0fe2dc0060b1c3192
ms.contentlocale: it-it
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-manage-job-supplies"></a>Procedura: Gestire gli approvvigionamenti delle commesse
La gestione degli approvvigionamenti di progetto di articoli, servizi e spese è un aspetto integrale e critico dell'esecuzione di tutte le commesse. È possibile utilizzare le giacenze o effettuare acquisti specifici per delle commesse utilizzando gli ordini di acquisto e/o le fatture di acquisto. Ad esempio, per completare una commessa relativa a un intervento di assistenza su un computer è richiesto un nuovo disco. Si crea quindi una fattura di acquisto per acquistare il nuovo disco e si registra la commessa in cui verrà utilizzato.

Se il processo di acquisto non richiede la registrazione separata della transazione fisica, è possibile elaborare un acquisto nella finestra **Registrazioni commesse in G/L**. Per ulteriori informazioni, vedere [Procedura: Registrare l'utilizzo nelle commesse](projects-how-record-job-usage.md).

## <a name="to-purchase-items-or-services-for-a-job"></a>Per acquistare articoli o servizi per una commessa
Nella procedura riportata di seguito viene illustrato come utilizzare una fattura di acquisto per acquistare i prodotti per una commessa. La stessa procedura vale anche quando si utilizza un ordine di acquisto.  

1. Nell'angolo superiore destro, scegliere l'icona **Cerca pagina o report**, immettere **Fatture acquisto**, quindi scegliere il collegamento correlato.  
2. Scegliere l'azione **Nuovo** e compilare i campi necessari. Per ulteriori informazioni, vedere [Procedura: Registrare gli acquisti](purchasing-how-record-purchases.md).
3. Nei campi **Nr. commessa** e **Nr. task commessa**, selezionare le informazioni della commessa per la quale si desidera acquistare articoli o servizi.  

    Il valore che si seleziona nel campo **Tipo riga commessa** definisce se viene creata una riga di pianificazione quando si registra l'utilizzo dell'articolo. Se il campo contiene **Fatturabile**, vengono create le righe di pianificazione commessa che sono pronte per la fatturazione al cliente. Per ulteriori informazioni, vedere [Procedura: Fatturare commesse](projects-how-invoice-jobs.md).

4. Scegliere l'azione **Registra**.

## <a name="to-view-the-value-of-purchases-for-a-job"></a>Per visualizzare il valore degli acquisti per una commessa  

1. Nell'angolo superiore destro, scegliere l'icona **Cerca pagina o report**, immettere **Commesse**, quindi scegliere il collegamento correlato.
2. Aprire una scheda commessa di interesse.

    Nella Scheda dettaglio **Task**, il campo **Ordini inevasi** mostra l'importo inevaso totale, in valuta locale, degli articoli a magazzino e dei servizi sui documenti di acquisto per la riga del task commessa.  

    Il campo **Importo carichi non fatt.** mostra il valore di articoli spediti su documenti di acquisto, ma non ancora fatturati.  

3. Scegliere uno dei campi per aprire la finestra **Righe acquisto** dove è possibile esaminare le informazioni sulle righe del documento di vendita correlate, inclusi gli articoli o i servizi che sono stati ricevuti.

## <a name="to-post-a-job-related-expense"></a>Per registrare una spesa correlata a una commessa  
Se si incorre in spese di commessa straordinarie o eccezionali, è possibile utilizzare la finestra **Registrazioni commesse in G/L** per registrarle direttamente nel conto commessa correlato.

1. Nell'angolo superiore destro, scegliere l'icona **Cerca pagina o report**, immettere **Registrazioni commesse in C/G**, quindi scegliere il collegamento correlato.  
2. Creare una nuova riga e immettere le informazioni sulla spesa, incluse le informazioni nei campi **Nr. commessa** e **Nr. task commessa**.  
3. Una volta completate le registrazioni, scegliere l'azione **Registra**.


## <a name="see-also"></a>Vedi anche
[Gestione di progetti](projects-manage-projects.md)  
[Contabilità](finance-setup.md)  
[Gestire gli acquisti](purchasing-manage-purchasing.md)         
[Gestire le vendite](sales-manage-sales.md)      
[Utilizzare Dynamics NAV](ui-work-product.md)  

