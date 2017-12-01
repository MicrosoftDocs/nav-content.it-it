---
title: Acquistare articoli o servizi per una commessa e gestire gli approvvigionamenti
description: Descrive come gestire gli approvvigionamenti e gli acquisti di materiale e servizi per le commesse.
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: project management, material, purchase
ms.date: 06/06/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 3405af0c06df0fb04c528cf114d4ef6326f7c0a9
ms.contentlocale: it-it
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-manage-job-supplies"></a>Procedura: Gestire gli approvvigionamenti delle commesse
La gestione degli approvvigionamenti di progetto di articoli, servizi e spese è un aspetto integrale e critico dell'esecuzione di tutte le commesse. È possibile utilizzare le giacenze o effettuare acquisti specifici per delle commesse utilizzando gli ordini di acquisto e/o le fatture di acquisto. Ad esempio, per completare una commessa relativa a un intervento di assistenza su un computer è richiesto un nuovo disco. Si crea quindi una fattura di acquisto per acquistare il nuovo disco e si registra la commessa in cui verrà utilizzato.

Se il processo di acquisto non richiede la registrazione separata della transazione fisica, è possibile elaborare un acquisto nella finestra **Registrazioni commesse in G/L**. Per ulteriori informazioni, vedere [Procedura: Registrare l'utilizzo nelle commesse](projects-how-record-job-usage.md).

## <a name="to-purchase-items-or-services-for-a-job"></a>Per acquistare articoli o servizi per una commessa
Nella procedura riportata di seguito viene illustrato come utilizzare una fattura di acquisto per acquistare i prodotti per una commessa. La stessa procedura vale anche quando si utilizza un ordine di acquisto.  

1. Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **Fatture di acquisto**, quindi scegliere il collegamento correlato.  
2. Scegliere l'azione **Nuovo** e compilare i campi necessari. Per ulteriori informazioni, vedere [Procedura: Registrare gli acquisti](purchasing-how-record-purchases.md).
3. Nei campi **Nr. commessa** e **Nr. task commessa** selezionare le informazioni della commessa per la quale si desidera acquistare articoli o servizi. Utilizzare la funzione **Scegli colonne** se il campo non è visualizzato. Per ulteriori informazioni, vedere [Personalizzazione utente](ui-user-personalization.md).

    Il valore che si seleziona nel campo **Tipo riga commessa** definisce se viene creata una riga di pianificazione quando si registra l'utilizzo dell'articolo. Se il campo contiene **Fatturabile**, vengono create le righe di pianificazione commessa che sono pronte per la fatturazione al cliente. Per ulteriori informazioni, vedere [Procedura: Fatturare commesse](projects-how-invoice-jobs.md).
4. Scegliere l'azione **Registra**.

## <a name="to-view-the-value-of-purchases-for-a-job"></a>Per visualizzare il valore degli acquisti per una commessa
1. Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **Commesse**, quindi scegliere il collegamento correlato.
2. Aprire una scheda commessa di interesse.

    Nella Scheda dettaglio **Task**, il campo **Ordini inevasi** mostra l'importo inevaso totale, in valuta locale, degli articoli a magazzino e dei servizi sui documenti di acquisto per la riga del task commessa.  

    Il campo **Importo carichi non fatt.** mostra il valore di articoli spediti su documenti di acquisto, ma non ancora fatturati.  
3. Scegliere uno dei campi per aprire la finestra **Righe acquisto** dove è possibile esaminare le informazioni sulle righe del documento di vendita correlate, inclusi gli articoli o i servizi che sono stati ricevuti.

## <a name="to-post-a-job-related-expense"></a>Per registrare una spesa correlata a una commessa
Se si incorre in spese di commessa straordinarie o eccezionali, è possibile utilizzare la finestra **Registrazioni commesse in G/L** per registrarle direttamente nel conto commessa correlato.

1. Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **Registrazioni commesse in C/G**, quindi scegliere il collegamento correlato.  
2. Creare una nuova riga e immettere le informazioni sulla spesa, tra cui le informazioni nei campi **Nr. commessa** e **Nr. task commessa**.  
3. Una volta completate le registrazioni, scegliere l'azione **Registra**.

## <a name="see-also"></a>Vedi anche
[Gestione progetti](projects-manage-projects.md)  
[Finanze](finance.md)  
[Acquisti](purchasing-manage-purchasing.md)         
[Vendite](sales-manage-sales.md)      
[Utilizzo di [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)  

