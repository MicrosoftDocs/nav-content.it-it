---
title: Conteggio, adeguamento e riclassificazione dell'inventario
description: "Descrive come eseguire attività di conteggio fisico, rettifiche positive o negative e modificare le informazioni, quali ubicazione o numero di lotto, nei movimenti contabili articoli o nei movimenti warehouse."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: adjustment, negative, positive, increase, decrease
ms.date: 08/16/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 4d53e6e9b64e0f5c790abb0f62f66a2b28c12c50
ms.contentlocale: it-it
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-count-adjust-and-reclassify-inventory"></a>Procedura: Conteggio, rettifica e riclassificazione dell'inventario
Almeno una volta durante l'anno fiscale, è necessario procedere a un inventario fisico, ovvero conteggiare tutti gli articoli in magazzino, per verificare se la quantità registrata nel database corrisponde alla quantità fisica presente nelle warehouse. Se non si conosce la quantità fisica effettiva, è necessario registrarla nella contabilità generale come parte di una valutazione di magazzino di fine periodo.

Sebbene tutti gli articoli a magazzino vengano conteggiati almeno una volta l'anno, potrebbe essere necessario eseguire il conteggio di determinati articoli con maggiore frequenza, ad esempio nel caso in cui abbiano acquisito maggiore valore o siano prodotti a rapido assorbimento e costituiscano buona parte dell'attività commerciale. A questo scopo, è possibile assegnare speciali periodi di conteggio agli articoli. Per ulteriori informazioni, vedere la sezione "Per eseguire il conteggio ciclico".

Se è necessario rettificare le quantità di magazzino registrate, in relazione al conteggio o per altri scopi, è possibile utilizzare una registrazione di magazzino per modificare i movimenti contabili di inventario direttamente senza registrare transazioni aziendali. In alternativa, è possibile rettificare un singolo articolo nella scheda articolo.

Se è necessario modificare gli attributi dei movimenti contabili articoli oltre alle quantità, è possibile utilizzare le registrazioni di riclassificazione articoli. In genere tra gli attributi da riclassificare vi sono i numeri di serie o di lotto, le date di scadenza e le dimensioni.

> [!NOTE]
> Nelle configurazioni di warehouse avanzate gli articoli sono registrati nelle collocazioni come movimenti warehouse e non come movimenti contabili articoli. Di conseguenza, eseguire il conteggio, la rettifica e la riclassificazione in registrazioni di warehouse speciali che supportano le collocazioni. Quindi, utilizzare le funzioni speciali per sincronizzare i movimenti warehouse nuovi o modificati con i movimenti contabili articoli correlati per riflettere le modifiche nelle quantità e nei valori di magazzino. Questa operazione è descritta in procedure specifiche riportate di seguito laddove è opportuno.

## <a name="to-perform-a-physical-inventory"></a>Per eseguire un inventario fisico
Al termine di un anno finanziario, ma anche più spesso, è necessario elaborare un inventario fisico (ovvero conteggiare gli articoli attualmente in magazzino) per controllare se le quantità registrate corrispondono alle quantità fisiche presenti in magazzino. Se esistono differenze, queste devono essere registrate nei conti articoli prima di eseguire la valutazione di inventario.

Oltre al task di conteggio fisico, il processo completo include i tre task seguenti:

- Calcolo delle giacenze previste.
- Stampa del report da utilizzare nel conteggio.
- Immissione e registrazione delle giacenze effettive conteggiate.

È possibile eseguire l'inventario fisico in uno dei seguenti modi, in base al setup della warehouse. Per ulteriori informazioni, vedere [Impostazione gestione warehouse](warehouse-setup-warehouse.md).  

-   Se l'ubicazione non prevede l'utilizzo di stoccaggi e prelievi guidati (configurazione di warehouse di base), utilizzare la finestra **Registrazioni inventario fis.** nel menu **Magazzino**. La procedura da seguire è molto simile a quella utilizzata per l'elaborazione di un inventario fisico senza conteggio ciclico.  
-   Se l'ubicazione prevede l'utilizzo di stoccaggi e prelievi guidati (configurazione di warehouse avanzata), utilizzare innanzitutto la finestra **Registrazioni inventario whse.** quindi la finestra **Registrazioni magazzino** per eseguire la funzione **Calcola rettifica whse.**.

### <a name="to-calculate-the-expected-inventory-in-basic-warehouse-configurations"></a>Per calcolare le giacenze previste nelle configurazioni di warehouse di base
1. Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **Registrazioni inventario fisico**, quindi scegliere il collegamento correlato.
2. Scegliere l'azione **Calcola giacenze**.
3. Nella finestra **Calcola giacenze** specificare le condizioni da utilizzare per creare le righe registrazioni, ad esempio se includere gli articoli che non hanno inventario registrato.
4. Impostare i filtri se si desidera soltanto calcolare le giacenze per determinati articoli, collocazioni, ubicazioni o dimensioni.
5. Scegliere il pulsante **OK**.

> [!NOTE]  
>   I movimenti articoli vengono elaborati in base alle informazioni inserite e le righe vengono create in registrazioni inventario fisico. Si noti che il campo **Qtà (inv. fisico)** viene compilato automaticamente con la stessa quantità del campo **Qtà (calcolata)** . Con questa funzionalità non è necessario immettere le giacenze conteggiate disponibili per gli articoli quando sono corrispondenti alla quantità calcolata. Tuttavia, se la quantità conteggiata è diversa da quella immessa nel campo **Qtà (calcolata)** , è necessario sovrascriverla con la quantità effettivamente conteggiata.

### <a name="to-calculate-the-expected-inventory-in-advanced-warehouse-configurations"></a>Per calcolare le giacenze previste nelle configurazioni di warehouse avanzate
1.  Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **Registraz. magazzino**, quindi scegliere il collegamento correlato.  
2.  Scegliere l'azione **Calcola rettifica whse.**.  
3.  Compilare i campi nella finestra di richiesta del processo batch specificando i numeri degli articoli che si desidera conteggiare e l'ubicazione.
4. Scegliere il pulsante **OK** e registrare le eventuali rettifiche.

    Se non si esegue questa operazione prima di eseguire l'inventario fisico della warehouse, i risultati registrati nelle registrazioni di inventario fisico e nei movimenti contabili magazzino nella seconda parte del processo corrispondono ai risultati dell'inventario fisico combinati con altre rettifiche di warehouse precedenti relative agli articoli conteggiati.  
5.  Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **Registr. invent. whse.**, quindi scegliere il collegamento correlato.  
6. Scegliere l'azione **Calcola giacenze**. Verrà visualizzata la finestra di richiesta del processo batch **Calcola inventario whse.**.  
7.  Impostare i filtri per limitare gli articoli che verranno conteggiati nelle registrazioni e fare clic sul pulsante **OK**.

    Verrà automaticamente creata una riga per ciascuna collocazione che soddisfa i requisiti del filtro. A questo punto, è possibile eliminare alcune righe. Tuttavia, se si desidera registrare i risultati come inventario fisico, è necessario conteggiare l'articolo in tutte le collocazioni in cui è contenuto.  

     Se si sceglie di conteggiare l'articolo solo in alcune collocazioni, è possibile rilevare le eventuali discrepanze, registrarle e successivamente contabilizzarle nelle registrazioni di magazzino utilizzando la funzione **Calcola rettifica whse.**  
8.  Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **Lista inventari fis. whse.**, quindi scegliere il collegamento correlato.  
9.  Aprire la pagina di richiesta del report e stampare le liste in cui si desidera che gli addetti annotino la quantità di articoli da loro conteggiata in ciascuna collocazione.  
10. Una volta completato il conteggio manuale, immettere le quantità conteggiate nel campo **Qtà (inv. fisico)** nelle registrazioni di inventario fisico della warehouse.  

    > [!NOTE]  
    >  Nelle registrazioni di inventario fisico della warehouse il campo **Qtà (calcolata)** viene compilato automaticamente in base ai record delle collocazioni warehouse e tali quantità vengono copiate nel campo **Qtà (inv. fisico)** in ogni riga. Se la quantità conteggiata dagli impiegati warehouse risulta differente dalla quantità copiata automaticamente nel campo Qtà (inv. fisico), è necessario immettere la quantità effettivamente conteggiata.  

11. Dopo avere immesso tutte le quantità conteggiate, scegliere l'azione **Registra**.  

    Quando si effettua la registrazione, nel registro warehouse vengono automaticamente creati due movimenti di warehouse per ogni riga conteggiata e registrata, nel modo descritto di seguito.  

    -   Se le quantità fisiche e le quantità calcolate risultano differenti, viene registrata una quantità positiva o negativa per la collocazione e viene contabilizzata una quantità di compensazione nella collocazione di rettifica dell'ubicazione.  
    -   Se la quantità calcolata è uguale alla quantità fisica, viene automaticamente registrato un movimento pari a 0 sia per la collocazione che per la collocazione di rettifica. I movimenti forniscono pertanto un record indicante che in una data specifica, ovvero quella di registrazione, è stato eseguito un inventario fisico della warehouse e non sono state rilevate discrepanze nelle giacenze per tale articolo.  

Quando si registra l'inventario fisico della warehouse, la registrazione non viene eseguita nei movimenti magazzino, nei movimenti di inventario fisico o nei movimenti di valorizzazione, tuttavia i record sono disponibili per eseguire una riconciliazione immediata qualora necessario. Se tuttavia si desidera conservare record precisi sulla situazione della warehouse e si è proceduto al conteggio di tutte le collocazioni in cui gli articoli erano registrati, si consiglia di registrare immediatamente i risultati della warehouse come inventario fisico. Per ulteriori informazioni, vedere la sezione "Per immettere e registrare le giacenze effettive conteggiate nelle configurazioni di warehouse avanzate".

### <a name="to-print-the-report-to-be-used-when-counting"></a>Per stampare il report da utilizzare nel conteggio
1. Nella finestra **Registrazioni inventario fis.** contenente le giacenze previste calcolate, scegliere l'azione **Stampa**.
2. Nella finestra **Lista inventario fisico** specificare se nel report deve essere inclusa la quantità calcolata e se elencare gli articoli di magazzino per numeri seriali/di lotto.
3. Impostare i filtri se si desidera stampare il report solo per determinati articoli, collocazioni, ubicazioni o dimensioni.
4. Selezionare il pulsante **Stampa**.

Gli addetti al magazzino potranno quindi eseguire l'inventario e registrare tutte le differenze nel report stampato.

### <a name="to-enter-and-post-the-actual-counted-inventory-in-basic-warehouse-configurations"></a>Per immettere e registrare le giacenze effettive conteggiate nelle configurazioni di warehouse di base
1. In ogni riga della finestra **Registrazioni inventario fis.** in cui le giacenze effettive, determinate dal conteggio fisico, sono diverse dalla quantità calcolata, immettere le giacenze effettive nel campo **Qtà (inv. fisico)**.

    I campi correlati vengono aggiornati di conseguenza.

    > [!NOTE]  
   >   Se dal conteggio fisico risultano differenze determinate dalla registrazione degli articoli con codici ubicazione non corretti, le differenze non devono essere inserite nelle registrazioni inventario fisico. In alternativa, utilizzare le registrazioni di riclassificazione o un ordine di trasferimento per reindirizzare gli articoli alle ubicazioni corrette. Per ulteriori informazioni, vedere Reg. ricl. articoli o Procedura: Creare ordini di trasferimento.

2. Per rettificare le quantità calcolate con le quantità effettive conteggiate, scegliere l'azione **Registra**.

    Vengono creati sia i movimenti contabili articoli che i movimenti contabili di inventario fisico. Aprire la scheda articolo per visualizzare i movimenti contabili di inventario fisico risultanti.

3. Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **Articoli**, quindi scegliere il collegamento correlato.
4. Per verificare il conteggio dell'inventario, aprire la scheda articolo in questione e quindi scegliere l'azione **Mov. contabili inventario fis.**.

### <a name="to-enter-and-post-the-actual-counted-inventory-in-advanced-warehouse-configurations"></a>Per immettere e registrare le giacenze effettive conteggiate nelle configurazioni di warehouse avanzate

1.  Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **Registraz. magazzino**, quindi scegliere il collegamento correlato.  
2.  Scegliere l'azione **Calcola rettifica whse.**.  
3.  Selezionare gli stessi articoli conteggiati per l'inventario fisico nel ciclo di conteggio appena eseguito e tutti gli altri articoli che richiedono la rettifica, quindi fare clic sul pulsante **OK**.  

     Viene visualizzata la finestra **Registrazioni magazzino** e vengono create le righe per tali articoli. Si noti che le quantità nette appena conteggiate e registrate collocazione per collocazione sono pronte per essere consolidate e sincronizzate come movimenti contabili articoli.  

4.  Registrare la registrazioni senza apportare alcuna modifica alle quantità.  

La corrispondenza tra le quantità nei movimenti contabili magazzino (movimenti articoli) e le quantità nella warehouse (movimenti warehouse) relative agli articoli è stata ristabilita e la data dell'ultimo conteggio dell'articolo o dell'unità di stockkeeping è stata automaticamente aggiornata.  

## <a name="to-perform-cycle-counting"></a>Per eseguire un conteggio ciclico
Sebbene tutti gli articoli a magazzino vengano conteggiati almeno una volta l'anno, potrebbe essere necessario eseguire il conteggio di determinati articoli con maggiore frequenza, ad esempio nel caso in cui abbiano acquisito maggiore valore o siano prodotti a rapido assorbimento e costituiscano buona parte dell'attività commerciale. A questo scopo, è possibile assegnare speciali periodi di conteggio agli articoli.

È possibile eseguire il conteggio ciclico in uno dei seguenti modi, in base al setup della warehouse. Per ulteriori informazioni, vedere [Impostazione gestione warehouse](warehouse-setup-warehouse.md).  

-   Se l'ubicazione non prevede l'utilizzo di stoccaggi e prelievi guidati (configurazione di warehouse di base), utilizzare la finestra **Registrazioni inventario fis.** nel menu **Magazzino**. La procedura da seguire è molto simile a quella utilizzata per l'elaborazione di un inventario fisico senza conteggio ciclico.  
-   Se l'ubicazione prevede l'utilizzo di stoccaggi e prelievi guidati (configurazione di warehouse avanzata), utilizzare innanzitutto la finestra **Registrazioni inventario whse.** quindi la finestra **Registrazioni magazzino** per eseguire la funzione **Calcola rettifica whse.**.  

### <a name="to-set-up-counting-periods"></a>Per impostare i periodi di conteggio
L'inventario fisico viene in genere eseguito ad intervalli regolari, ad esempio con frequenza mensile, trimestrale o annuale. È possibile impostare i periodi di conteggio dell'inventario necessari.

È innanzitutto necessario impostare i periodi di conteggio dell'inventario da utilizzare, quindi assegnarne uno a ciascun articolo. Quando si esegue un inventario fisico e si utilizza la funzione **Calcola conteggio periodo** nelle registrazioni di inventario fisico, le righe relative agli articoli vengono create automaticamente.

1. Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **Periodi di conteggio inventario fisico**, quindi scegliere il collegamento correlato.  
2. Compilare i campi, se necessario. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

### <a name="to-assign-a-counting-period-to-an-item"></a>Per assegnare un periodo di conteggio a un articolo  
1. Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **Articoli**, quindi scegliere il collegamento correlato.  
2. Selezionare l'articolo a cui si desidera assegnare un periodo di conteggio.  
3. Nel campo **Cod. cont. periodo inv. fis.**, selezionare il periodo di conteggio appropriato.  
4. Scegliere il pulsante **Sì** per modificare il codice e calcolare il primo periodo di conteggio per l'articolo. Alla successiva scelta di calcolare un periodo di conteggio nelle registrazioni di inventario fisico, l'articolo verrà visualizzato come riga nella finestra **Selez. articoli inv. fis.**. A questo punto è possibile iniziare a conteggiare l'articolo su base periodica.

### <a name="to-initiate-a-count-based-on-counting-periods-in-basic-warehouse-configurations"></a>Per avviare un conteggio basato sui periodi di conteggio nelle configurazioni di warehouse di base
1. Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **Registrazioni inventario fisico**, quindi scegliere il collegamento correlato.
2. Scegliere l'azione **Calcola conteggio periodo**.

    Viene visualizzata la finestra **Selez. articoli inv. fis.** contenente gli articoli da conteggiare in base ai periodi di conteggio precedentemente assegnati.
3. Eseguire l'inventario fisico. Per ulteriori informazioni, vedere la sezione "Per eseguire un inventario fisico".

### <a name="to-initiate-a-count-based-on-counting-periods-in-advanced-warehouse-configurations"></a>Per avviare un conteggio basato sui periodi di conteggio nelle configurazioni di warehouse avanzate
1.  Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **Registr. invent. whse.**, quindi scegliere il collegamento correlato.  
2. Scegliere l'azione **Calcola conteggio periodo**.

    Viene visualizzata la finestra **Selez. articoli inv. fis.** contenente gli articoli da conteggiare in base ai periodi di conteggio precedentemente assegnati.
3. Eseguire l'inventario fisico. Per ulteriori informazioni, vedere la sezione "Per eseguire un inventario fisico".  

    > [!NOTE]  
    >  È necessario conteggiare l'articolo in tutte le collocazioni contenenti l'articolo in questione. Se si eliminano alcune righe relative alle collocazioni automaticamente recuperate per il conteggio nella finestra **Inventario fis. whse.**, il conteggio non include tutti gli articoli presenti nella warehouse. Se successivamente si procede alla contabilizzazione di tali risultati incompleti in Registrazioni inventario fis., le quantità registrate non saranno corrette.  

## <a name="to-adjust-the-inventory-of-one-item"></a>Per rettificare l'inventario di un articolo
Dopo aver effettuato un conteggio fisico di un articolo nell'area magazzino, è possibile utilizzare la funzione **Rettifica magazzino** per registrare l'effettiva quantità di magazzino.

1. Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **Articoli**, quindi scegliere il collegamento correlato.
2. Selezionare l'articolo per cui si desidera rettificare il magazzino e scegliere l'azione **Rettifica magazzino**.
3. Nel campo **Nuovo inventario** immettere la quantità di magazzino che si desidera registrare per l'articolo.
4. Scegliere il pulsante **OK**.

Il magazzino dell'articolo è ora rettificato. La nuova quantità viene mostrata nel campo **Inventario corrente** nella finestra **Rettifica magazzino** e nel campo **Magazzino** nella finestra **Scheda articolo**.

È inoltre possibile utilizzare la funzione **Rettifica magazzino** come semplice mezzo per collocare articoli acquistati nel magazzino se non si utilizzano fatture o ordini di acquisto per registrare gli acquisti. Per ulteriori informazioni, vedere [Procedura: Registrare gli acquisti](purchasing-how-record-purchases.md).

> [!NOTE]  
>   Dopo aver rettificato il magazzino, è necessario aggiornarlo con il valore corrente calcolato. Per ulteriori informazioni, vedere [Procedura: Rivalutare il magazzino](inventory-how-revalue-inventory.md).

### <a name="to-adjust-the-inventory-quantity-of-multiple-items-in-basic-warehouse-configurations"></a>Per rettificare la quantità in giacenza di più articoli nelle configurazioni di warehouse di base
Nella finestra **Registrazioni magazzino**, è possibile registrare direttamente la transazione dell'articolo per rettificare il magazzino in relazione a rettifiche positive o negative di agli acquisti o vendite senza utilizzare i documenti.

Se le registrazioni magazzino sono spesso utilizzate per la stessa riga di registrazione o per righe di registrazione simili, ad esempio in relazione al consumo di materiale, è possibile utilizzare la finestra **Registrazioni Magazzino Standard** per rendere più semplice questo tipo di lavoro ricorrente. Per ulteriori informazioni, vedere la sezione "Registrazioni standard" in [Utilizzo delle registrazioni COGE](ui-work-general-journals.md).

1. Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **Registrazioni inventario fisico**, quindi scegliere il collegamento correlato.
2. Compilare i campi, se necessario. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
3. Scegliere l'azione **Registra** per procedere con le rettifiche di magazzino.

> [!NOTE]  
>   Dopo aver rettificato il magazzino, è necessario aggiornarlo con il valore corrente calcolato. Per ulteriori informazioni, vedere [Procedura: Rivalutare il magazzino](inventory-how-revalue-inventory.md).

### <a name="to-adjust-bin-quantities-in-advanced-warehouse-configurations"></a>Per rettificare le quantità di collocazioni nelle configurazioni di warehouse avanzate  
Se l'ubicazione utilizza stoccaggi e prelievi guidati, utilizzare **Registrazioni articoli whse.** per registrare, fuori dall'ambito dell'inventario fisico, tutte le rettifiche positive e negative della quantità degli articoli note come guadagni effettivi, ad esempio, articoli registrati in precedenza come mancanti che ricompaiono improvvisamente, o come perdite effettive, ad esempio, articoli danneggiati.  

Diversamente dalla registrazione delle rettifiche nelle registrazioni di magazzino, le registrazioni degli articoli di warehouse consentono un ulteriore livello di rettifica che offre una maggiore precisione dei record sulle quantità. In questo modo la warehouse conterrà sempre un record completo del numero di articoli disponibili e della relativa ubicazione, tuttavia le rettifiche non verranno registrate immediatamente nei movimenti contabili magazzino. Nel processo di registrazione vengono effettuati accrediti o addebiti alla collocazione effettiva con la rettifica della quantità e viene creato un movimento di compensazione nella collocazione rettifica, una collocazione virtuale che non contiene articoli reali. La collocazione viene definita nel **Codice collocazione rettifica magazzino** della scheda ubicazione.

1.  Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **Registrazioni articoli whse.**, quindi scegliere il collegamento correlato.  
2.  Compilare le informazioni di testata.  
3.  Compilare il campo **Nr. articolo** della riga.  
4.  Immettere la collocazione in cui inserire gli articoli extra o la posizione in cui sono stati rilevati articoli mancanti.  
5.  Immettere la quantità osservata come discrepanza nel campo **Quantità**. Se sono stati rilevati articoli extra, immettere una quantità positiva. In caso di articoli mancanti, immettere una quantità negativa.  
6.  Scegliere l'azione **Registra**.

## <a name="to-synchronize-the-adjusted-warehouse-entries-with-the-related-item-ledger-entries"></a>Per sincronizzare i movimenti warehouse rettificati con i movimenti contabili articoli correlati
A intervalli appropriati in base a quanto definito dalla politica aziendale, è necessario registrare i record delle collocazioni warehouse nei movimenti contabili magazzino. Alcune società ritengono che sia più appropriato registrare le rettifiche nei movimenti contabili magazzino ogni giorno, mentre altre ritengono più opportuno effettuare una riconciliazione con minore frequenza.

1.  Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **Registraz. magazzino**, quindi scegliere il collegamento correlato.  
2.  Compilare i campi di ogni riga di registrazione.  
3.  Scegliere l'azione **Calcola rettifica whse.** e definire i filtri in modo appropriato nella finestra di richiesta del processo batch. Le rettifiche vengono calcolate solo per i movimenti nella collocazione rettifica che soddisfano i criteri dei filtri.  
4.  Nella Scheda dettaglio **Opzioni** immettere un numero nel campo **Nr. documento**. Poiché non è stata impostata alcuna numerazione per questo processo batch, utilizzare lo schema di numerazione impostato dalla warehouse oppure immettere la data seguita dalle proprie iniziali.  
5.  Scegliere il pulsante **OK**. Le rettifiche positive e vengono sommati per ogni articolo e le righe create nelle registrazioni magazzino per tutti gli articoli in cui la somma è una quantità positiva o negativa.  
6.  Registrare le righe di registrazione per immettere le differenze di quantità nei movimenti contabili magazzino. A questo punto, le giacenze nelle collocazioni warehouse corrisponderanno esattamente alle giacenze nei movimenti contabili magazzino.  

## <a name="to-reclassify-an-items-lot-number"></a>Per riclassificare il numero di lotto di un articolo
1. Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **Registrazioni riclassificazioni articoli**, quindi scegliere il collegamento correlato.
2. Nella finestra **Batch reg. riclass. articoli** compilare i campi in base alle esigenze.
3. Nel campo **Nr. lotto** immettere il numero del lotto corrente dell'articolo.
4. Nel campo **Nuovo nr. lotto** immettere il nuovo numero del lotto dell'articolo.
5. Scegliere l'azione **Registra**.

Vengono applicati dei passaggi speciali per riclassificare i numeri di serie o di lotto. Per ulteriori informazioni, vedere [Procedura: Utilizzo dei numeri di serie e di lotto](inventory-how-work-item-tracking.md).

## <a name="see-also"></a>Vedi anche
[Magazzino](inventory-manage-inventory.md)
[Gestione warehouse](warehouse-manage-warehouse.md)    
[Vendite](sales-manage-sales.md)  
[Acquisti](purchasing-manage-purchasing.md)  
[Utilizzo di [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

