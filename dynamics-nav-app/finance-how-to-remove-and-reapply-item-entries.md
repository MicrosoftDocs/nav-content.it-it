---
title: Come rimuovere e ricollegare movimenti articoli
description: "È possibile visualizzare e modificare manualmente alcuni movimenti di collegamento articoli creati automaticamente durante le transazioni di magazzino."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 09/07/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 400a30ab196d2015bd9caae3fcb38dfdceea53ca
ms.contentlocale: it-it
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-remove-and-reapply-item-ledger-entries"></a>Procedura: Rimuovere e ricollegare movimenti contabili articolo
Nella finestra **Prospetto collegamento** è possibile visualizzare e modificare manualmente alcuni movimenti di collegamento articoli creati automaticamente durante le transazioni di magazzino.  

Quando si registra una transazione in cui gli articoli vengono spostati in magazzino o fuori da esso, viene creato un collegamento articoli tra un aumento di magazzino a una riduzione di magazzino. Questi collegamenti determinano il flusso dei costi dalle merci ricevute in magazzino a quelle in uscita dal magazzino. A causa della modalità di calcolo del costo unitario, un collegamento articoli non corretto potrebbe portare a un costo medio o a un costo unitario non attendibile. Per ulteriori informazioni, vedere Dettagli di progettazione: Collegamento articoli.

Gli scenari seguenti potrebbero richiedere di annullare un collegamento o di ricollegare i movimenti contabili articolo:

- Ci si è dimenticati di creare un collegamento fisso.
- È stato creato un collegamento fisso non corretto.
- È necessario restituire un articolo a cui è stata già collegata una vendita.

Se possibile, utilizzare un documento per ricollegare un movimento contabile articolo. Se, ad esempio, è necessario effettuare un reso di acquisto di un articolo a cui è già stata collegata una vendita, è possibile creare il nuovo collegamento semplicemente creando e registrando il documento di reso di acquisto utilizzando il collegamento corretto nel campo **Collega-a mov. art.** della riga di reso di acquisto. Per semplificare questa operazione, è possibile utilizzare la funzione **Ottieni righe documento registrato da stornare** o **Copia documento** nel documento di reso di acquisto. Quando si registra il documento, il movimento contabile articolo viene ricollegato automaticamente. Per ulteriori informazioni vedere [Procedura: Elaborare i resi o gli annullamenti acquisti](purchasing-how-process-purchase-returns-cancellations.md).

Se non è possibile utilizzare un documento per ricollegare, ad esempio quando si deve correggere un collegamento fisso, utilizzare la finestra **Prospetto collegamento** per correggere un collegamento.

> [!Warning]  
> Quando si utilizza il Prospetto collegamento, è importante prendere in considerazione quanto indicato di seguito:
    - Non è consigliabile lasciare i movimenti di collegamento scollegati per lungi periodi di tempo poiché altri utenti non possono elaborare gli articoli finché non si ricollegano i movimenti di collegamento o si chiude la finestra **Prospetto collegamento**. Gli utenti che provano a realizzare le azioni che includono un movimento di collegamento manualmente scollegato ricevono il seguente messaggio di errore: “Impossibile eseguire questa azione perché i movimenti per l'articolo XXX non sono applicati in XXX dall'utente XXX".
    - È consigliabile collegare solo i movimenti contabili articoli durante le ore non lavorative per evitare conflitti con altri utenti che registrano transazioni con gli stessi articoli.
    - Quando si chiude il Prospetto collegamento, in [!INCLUDE[d365fin](includes/d365fin_md.md)] viene eseguito un controllo automatico per verificare che tutti i movimenti siano collegati. Se, ad esempio, si rimuove il collegamento a una quantità ma non si crea un nuovo collegamento, quindi si chiude il Prospetto collegamento, viene creato un nuovo collegamento. In questo modo, i costi rimangono intatti. Tuttavia, se si rimuove un collegamento fisso, al momento della chiusura del prospetto non ne viene creato automaticamente uno nuovo. È necessario eseguire questa operazione manualmente creando un nuovo collegamento nel prospetto.
    - Nel Prospetto collegamento è possibile rimuovere i collegamenti da più di un movimento per volta. Poiché, tuttavia, il collegamento di movimenti influenza l'insieme dei movimenti disponibili per il collegamento, non è possibile creare un collegamento per più di un movimento per volta.
    - Il Prospetto collegamento non consente di creare un collegamento nel seguente caso: se non è disponibile una quantità in stock sufficiente per il collegamento, il Prospetto collegamento non consente di creare un collegamento quando si tenta di collegare un movimento di riduzione di magazzino senza informazioni sulla tracciabilità articolo a un movimento di aumento di magazzino con informazioni sulla tracciabilità articolo.

## <a name="to-remove-an-item-application-by-using-the-application-worksheet"></a>Per rimuovere un collegamento articoli tramite il Prospetto collegamento  
1.  Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **Prospetto collegamento**, quindi scegliere il collegamento correlato.  
2.  La finestra **Prospetto collegamento** si apre visualizzando i movimenti contabili articoli esistenti per tutti gli articoli.  
3.  Immettere filtri nella Scheda dettaglio **Generale** per semplificare la ricerca del movimento contabile articolo per il quale si desidera modificare il collegamento.  
4.  Selezionare il movimento contabile articolo e scegliere l'azione **Movimenti collegati**. Verrà aperta la finestra **Visualizza movimenti collegati - Movimenti collegati** in cui saranno visualizzati uno o più movimenti contabili articoli attualmente collegati al movimento selezionato.  
5.  Selezionare il movimento per il quale si desidera rimuovere il collegamento.  
6.  Scegliere l'azione **Rimuovi collegamento**. In questo modo si rimuove il movimento di collegamento articolo che collega i due movimenti contabili articoli e lo si sposta nella finestra **Visualizza movimenti collegati - Movimenti scollegati** .  
7.  Chiudere la finestra **Visualizza movimenti collegati - Movimenti collegati** .  

 Il valore dei campi **Quantità residua** dei due movimenti contabili articoli viene aumentato della quantità che non è stata collegata. Il movimento contabile articolo rimosso è ora disponibile per il nuovo collegamento nella finestra **Visualizza movimenti collegati - Movimenti scollegati** .  

> [!IMPORTANT]  
>  Non è consigliabile lasciare i movimenti di collegamento scollegati per periodi di tempo più lunghi poiché altri utenti non possono elaborare gli articoli interessati finché non si ricollegano i movimenti di collegamento o si chiude la finestra **Prospetto collegamento**. Il seguente messaggio di errore viene visualizzato se si tenta di eseguire operazioni che includono un movimento di collegamento manualmente scollegato:  
>   
>  **Impossibile eseguire questa azione perché i movimenti per l'articolo <item> non sono applicati nel prospetto collegamento dall'utente <user>.**  

## <a name="to-reapply-an-item-application-by-using-the-application-worksheet"></a>Per riapplicare un collegamento articoli tramite il Prospetto collegamento  
1.  Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **Prospetto collegamento**, quindi scegliere il collegamento correlato.  
2.  La finestra **Prospetto collegamento** si apre visualizzando i movimenti contabili articoli esistenti per tutti gli articoli.  
3.  Per ricollegare i movimenti rimossi dopo l'apertura del prospetto, selezionare il movimento contabile articolo che si desidera ricollegare. Nel gruppo **Funzioni** della scheda **Azioni** scegliere **Ricollega**.  

    > [!NOTE]  
    >  Questo ricollegamento al saldo originale viene eseguito anche automaticamente quando si chiude la finestra **Prospetto collegamento**.  
4.  Per collegare un movimento contabile aperto disponibile a un altro movimento, selezionare il movimento contabile articolo che si desidera collegare. Scegliere l'azione **Movimenti scollegati**. Viene visualizzata la finestra **Visualizza movimenti collegati - Movimenti scollegati** .  
5.  Selezionare uno o più movimenti contabili articoli che si desidera collegare al movimento selezionato nella finestra **Prospetto collegamento**, quindi fare clic su **OK**.  

     Verrà creato un movimento collegamento articoli tra i due movimenti contabili articoli. I valori dei campi **Quantità residua** dei due movimenti verranno diminuiti della quantità collegata.  

    > [!NOTE]  
    >  Se si è scelto di creare un collegamento che provocherebbe la generazione di un ciclo infinito nel processo di rettifica del costo, il collegamento proposto non viene effettuato. Ciò può avvenire quando tramite i movimenti originali è stato creato uno stock negativo. Il collegamento non viene eseguito. Di conseguenza, è necessario selezionare un movimento diverso per il collegamento.  
6.  Se nella finestra **Setup magazzino** il campo **Rettifica costo automatica** è impostato su **Sempre**, il processo batch di rettifica del costo viene eseguito automaticamente dopo la creazione di un nuovo collegamento. In caso contrario, eseguire il processo batch **Rettifica costo - Movimenti articoli** per assicurarsi che tutti i costi siano aggiornati.  

## <a name="see-also"></a>Vedi anche  
[Procedura: Chiudere i movimenti contabili articoli aperti risultanti da un collegamento fisso nelle registrazioni magazzino](finance-how-to-close-open-item-ledger-entries-resulting-from-fixed-application-in-the-item-journal.md)  
 [Procedura: Elaborare i resi o gli annullamenti acquisti](purchasing-how-process-purchase-returns-cancellations.md)  
 [Gestione dei costi di magazzino](finance-manage-inventory-costs.md)   
 [Dettagli di progettazione: Collegamento articoli](design-details-item-application.md)  
 [Utilizzo di [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

