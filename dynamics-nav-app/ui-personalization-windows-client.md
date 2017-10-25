---
title: Personalizzazione delle pagine nel client Windows di Dynamics
description: Informazioni su come personalizzare l'interfaccia utente in base alle esigenze professionali.
author: jswymer
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.date: 07/26/2017
ms.author: jswymer
ms.prod: dynamics-nav-2018
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 12aee74950066647f61639ec88c47e9be3c2f172
ms.contentlocale: it-it
ms.lasthandoff: 10/16/2017

---
# <a name="personalizing-your-workspace-in-the-dynamics-windows-client"></a>Personalizzazione dell'area di lavoro nel client Windows di Dynamics
È possibile personalizzare l'area di lavoro per adattarla alle esigenze professionali e alle preferenze modificando le pagine in modo da visualizzare solo le informazioni necessarie, quando necessario. Le modifiche di personalizzazione apportate influenzeranno solo ciò che vede l'utente che le ha effettuate, non quello che altri utenti vedono. È possibile personalizzare molte parti dell'interfaccia utente, incluse le azioni da includere nella barra multifunzione, il posizionamento dei campi nelle Schede dettaglio o nei riquadri Dettaglio e le voci di menu da includere nel riquadro di spostamento.

> [!NOTE]  
> È inoltre possibile personalizzare le pagine tramite [!INCLUDE[nav_web_md](includes/nav_web_md.md)]. Per informazioni sulla personalizzazione nei due client, vedere [Sintesi della personalizzazione](ui-personalization-overview.md).
 
## <a name="how-to-personalize-your-workspace"></a>Come personalizzare l'area di lavoro
La maggior parte delle attività di personalizzazione può essere effettuata utilizzando la funzione **Personalizza**, a cui si accede praticamente da tutti i tipi di pagine nel modo seguente:

1.  Aprire la pagina da personalizzare.
2.  In alto a sinistra scegliere l'icona del menu **Applicazione** ![Pulsante menu Applicazione nella barra dei menu](media/applicationmenuicon.png "ApplicationMenuIcon"), quindi **Personalizza** e infine selezionare una delle opzioni di personalizzazione.

Sono inoltre disponibili modifiche di base dell'interfaccia utente, come il ridimensionamento delle finestre o l'ampliamento della larghezza delle colonne, direttamente nella pagina, al di fuori dell'opzione **Personalizza**.

## <a name="general-information"></a>Informazioni generali
Durante la personalizzazione dell'interfaccia utente, si consiglia di tenere presente quanto segue: 

-   È possibile registrare più personalizzazioni della stessa pagina in base a differenti punti di accesso alla pagina. Ad esempio, la finestra Ordini vendita può essere personalizzata e apparire diversa all'apertura dalla finestra Scheda cliente rispetto a quando viene aperta dalla Gestione ruolo utente Gestore ordini vendite. Il punto da cui è possibile accedere alla pagina da personalizzare viene registrato nella personalizzazione di quella specifica pagina. Di conseguenza, potrebbero esserci più record di personalizzazione della pagina nel database, come è possibile vedere nella finestra **Elimina personalizzazione utente**.

-   L'applicazione può essere configurata per visualizzare e nascondere gli elementi dell'interfaccia utente (ad esempio campi, Schede dettaglio e riquadri Dettaglio informazioni) in base alla licenza o alle autorizzazioni dell'utente. Sarà possibile visualizzare e personalizzare i campi relativi ai campi di elementi per cui si dispone di autorizzazione.

## <a name="customize-ribbons"></a>Personalizzare la barra multifunzione
La barra multifunzione consente di accedere a diverse azioni. È possibile personalizzare la barra multifunzione in modo da ottimizzarla in base ai processi e alle preferenze del proprio lavoro. Ad esempio, se si utilizza più frequentemente la finestra **Dimensioni**, è possibile aggiungere l'azione **Dimensioni** al gruppo di operazioni **Processo**. È inoltre possibile rimuovere le azioni che non vengono mai utilizzate per ottenere una panoramica migliore.  
  
È possibile effettuare i seguenti task per personalizzare le barre multifunzione nelle pagine:  
  
-   Aggiungere, rinominare o rimuovere schede, gruppi, azioni e menu.  
-   Modificare l'ordine delle azioni.  
-   Ripristinare la barra multifunzione all'impostazione di default.  
  
### <a name="to-customize-a-ribbon"></a>Per personalizzare la barra multifunzione
1. Aprire la pagina da modificare.
2. In alto a sinistra scegliere l'icona del menu **Applicazione** ![Pulsante menu Applicazione nella barra dei menu](media/applicationmenuicon.png "ApplicationMenuIcon"), scegliere **Personalizza** quindi **Personalizza barra multifunzione**.

Viene visualizzata la finestra di dialogo **Organizzare le azioni nella barra multifunzione** divisa in due riquadri. Il riquadro **Azioni disponibili** elenca tutte le azioni che è possibile scegliere da aggiungere nella pagina. Il riquadro **Mostra le azioni nell'ordine seguente** mostra la struttura di tutte le azioni attualmente visualizzate nella pagina.

-   Gli elementi a livello di radice definiscono le schede.

    -   Gli elementi di secondo livello definiscono un gruppo in una scheda.

        -   L'elemento di terzo livello definisce un menu di azioni in un gruppo.

### <a name="add-a-group"></a>Aggiungere un gruppo
Selezionare la scheda in cui inserire il gruppo e selezionare **Crea gruppo**. Non è possibile aggiungere un gruppo all'interno di un menu.

### <a name="add-a-menu"></a>Aggiungere un menu
Selezionare il gruppo in cui inserire il menu e selezionare **Crea menu**. È possibile aggiungere solo un menu a un gruppo o a un altro menu. 

#### <a name="add-an-action"></a>Aggiungere un'azione
Selezionare l'azione nel riquadro **Azioni disponibili**, scegliere **Aggiungi** per aggiungerla nel riquadro **Mostra le azioni nell'ordine seguente**, quindi usare i pulsanti **Sposta su** e **Sposta giù** per disporla nella posizione desiderata.

Non è possibile aggiungere un'azione a una scheda; solo a un gruppo o a un menu.

###  <a name="limitations-and-recommendations"></a>Limiti e consigli 
Si notino le seguenti limitazioni quando si personalizza la barra multifunzione:  
  
-   Non è possibile spostare o rinominare le schede o i gruppi di sistema ad esempio **Pagina iniziale** o **Nuovo**. L'ubicazione di alcuni gruppi, ad esempio **Nuovo documento** è fissa.  
-   Le azioni o i gruppi con visibilità dinamica non possono aggiunti o eliminati. 
-   È possibile creare solo menu all'interno di gruppi, non all'interno di schede.  
-   È possibile annidare un menu all'interno di un altro menu, ma non è consigliabile.  
-   Se si verifica un comportamento imprevisto con i gruppi e le azioni dopo aver personalizzato la barra multifunzione, eseguire le seguenti operazioni:  
    
    1.  Svuotare, ma non eliminare, il gruppo in cui il problema si verifica.  
    2.  Chiudere la finestra di dialogo utilizzando il pulsante **OK**.  
    3.  Aprire di nuovo la finestra di dialogo e aggiungere nuovamente le azioni al gruppo.  

> [!IMPORTANT]  
>  Qualsiasi personalizzazione che alteri la barra multifunzione potrebbe influire sulle indicazioni offerte nella guida di [!INCLUDE[navnow_md](includes/navnow_md.md)], in quanto i passaggi di spostamento nella guida potrebbero fare riferimento a un layout diverso della barra multifunzione.

## <a name="customize-fasttabs"></a>Personalizzare le Schede dettaglio
Le schede dettaglio consentono di organizzare le informazioni sulle pagine in gruppi semplici e facilmente gestibili. È possibile personalizzare le Schede dettaglio nelle pagine in base al proprio flusso di lavoro. È ad esempio possibile decidere di visualizzare un minor numero di Schede dettaglio o nascondere campi specifici in una determinata Scheda dettaglio. È inoltre possibile fare in modo che i campi più importanti vengano inclusi nelle testate delle Schede dettaglio quando queste ultime vengono compresse.  

### <a name="to-customize-a-fasttab"></a>Per personalizzare una Scheda dettaglio  
  
1.  Aprire la pagina da modificare.
2.  Scegliere l'icona del menu **Applicazione** ![Pulsante menu Applicazione nella barra dei menu](media/applicationmenuicon.png "ApplicationMenuIcon"), selezionare **Personalizza** quindi scegliere **Personalizza pagina**.  
3.  Nella finestra di dialogo **Personalizza <Page Name>** scegliere **Schede dettaglio**.  
  
### <a name="add-move-or-remove-fasttabs"></a>Aggiungere, spostare o rimuovere le Schede dettaglio
La casella **Mostra le Schede dettaglio nell'ordine seguente:** contiene le Schede dettaglio che si trovano attualmente nella pagina e l'ordine in cui vengono visualizzate. Utilizzare i pulsanti **Aggiungi**, **Rimuovi** e **Sposta su** e **Sposta giù** per apportare modifiche.

### <a name="show-and-hide-fields-on-fasttabs"></a>Mostrare o nascondere i campi nelle Schede dettaglio
In **Mostra le Schede dettaglio nell'ordine seguente** selezionare la Scheda dettaglio che si desidera modificare, quindi scegliere **Personalizza Scheda dettaglio**. Utilizzare i pulsanti per personalizzare i campi che si desidera visualizzare e il relativo ordine nella pagina.

Impostare l'**Importanza** nel modo seguente:
-   Se si desidera visualizzare il campo nell'intestazione della Scheda dettaglio quando questa è compressa, impostare **Essenziale**.
- Se si desidera nascondere il campo a meno che l'utente non scelga l'azione **Mostra più campi** nella Scheda dettaglio, impostare **Aggiuntivo**.
-   **Standard** è l'impostazione predefinita o normale.

### <a name="set-up-field-for-quick-entry"></a>Impostare un campo per l'inserimento rapido 
Selezionare la casella di controllo **Inserimento rapido** per aggiungere il campo all'elenco dei campi con Inserimento rapido. Quando si lavora nella pagina e si preme il tasto INVIO in un campo, il puntatore salta al campo successivo impostato come campo di inserimento rapido. 

## <a name="customize-factboxes"></a>Personalizzare i riquadri Dettaglio informazioni
I riquadri Dettaglio informazioni consentono di visualizzare informazioni correlate al record selezionato dalla lista o aperto in una pagina di attività. È possibile selezionare i riquadri Dettaglio informazioni da visualizzare in un riquadro Dettaglio informazioni specifico. È inoltre possibile personalizzare i riquadri Dettaglio informazioni per visualizzare solo i campi necessari.  
  
### <a name="to-show-or-hide-the-factbox-pane"></a>Per mostrare o nascondere il riquadro Dettaglio informazioni
I dettagli informazioni sono contenuti in un riquadro Dettaglio informazioni, che può essere mostrato o nascosto in base alla pagina. Questo consente di nascondere facilmente più riquadri Dettaglio informazioni senza doverli rimuovere singolarmente. 

1.  Aprire la pagina da modificare. 
2.  Scegliere l'icona del menu **Applicazione** ![Pulsante menu Applicazione nella barra dei menu](media/applicationmenuicon.png "ApplicationMenuIcon"), selezionare **Personalizza** quindi scegliere **Riquadro Dettaglio informazioni**. Un segno di spunta indica se il riquadro Dettaglio informazioni viene visualizzato o meno.  

### <a name="to-customize-the-factbox-pane"></a>Per personalizzare il riquadro Dettaglio informazioni  
1.  Aprire la pagina da modificare. 
2.  Scegliere l'icona del menu **Applicazione** ![Pulsante menu Applicazione nella barra dei menu](media/applicationmenuicon.png "ApplicationMenuIcon"), selezionare **Personalizza** quindi scegliere **Scegli riquadri Dettaglio informazioni**.  
    
### <a name="add-a-factbox"></a>Aggiungere un riquadro Dettaglio informazioni  
  
Selezionare il Dettaglio informazioni da aggiungere al riquadro Dettaglio informazioni dalla casella **Riquadri Dettaglio informazioni disponibili**, quindi scegliere il pulsante **Aggiungi**.  
  
### <a name="remove-a-factbox"></a>Rimuovere un riquadro Dettaglio informazioni  
  
Nella casella **Mostra i riquadri Dettaglio informazioni nell'ordine seguente** scegliere il Dettaglio informazioni e quindi il pulsante **Rimuovi**.   
  
### <a name="change-the-order-of-the-factboxes"></a>Modificare l'ordine dei riquadri Dettaglio informazioni  
  
Nella casella **Mostra i riquadri Dettaglio informazioni nell'ordine seguente** selezionare il riquadro Dettaglio informazioni che si desidera spostare, quindi scegliere i pulsanti **Sposta su** o **Sposta giù** finché non si trova nella posizione desiderata.  
  
### <a name="change-the-fields-in-a-factbox"></a>Modificare i campi in un Dettaglio informazioni  
  
1.  Nella casella **Mostra i riquadri Dettaglio informazioni nell'ordine seguente** selezionare il Dettaglio informazioni e quindi scegliere **Personalizza parte**.  
  
2.   La casella **Campi disponibili** elenca tutti i campi disponibili per la scelta. La casella **Campi visualizzati** visualizza tutti i campi attualmente visualizzati nel riquadro Dettaglio informazioni. Utilizzare i pulsanti per aggiungere, rimuovere e spostare i campi.   


## <a name="customize-columns-in-a-list-or-on-document-lines"></a>Personalizzare le colonne in un elenco o nelle righe di un documento
Per ottenere una panoramica migliore delle informazioni necessarie, è possibile personalizzare le pagine elenco e le pagine scheda aggiungendo o rimuovendo colonne nelle griglie, modificando la disposizione delle colonne o aggiungendo un blocco riquadri.  
  
### <a name="to-add-remove-and-arrange-columns"></a>Per aggiungere, rimuovere e disporre le colonne  
  
1.  È possibile aggiungere, rimuovere o ridisporre le colonne due modi:

    -   Scegliere l'icona del menu **Applicazione** ![Pulsante menu Applicazione nella barra dei menu](media/applicationmenuicon.png "ApplicationMenuIcon"), scegliere **Personalizza** quindi **Scegli colonne**.
    -   Fare clic con il pulsante destro del mouse su un'intestazione di colonna e scegliere **Scegli colonne**.

2.  Nella finestra di dialogo **Scegliere le colonne da visualizzare nella lista**, il riquadro **Colonne disponibili** contiene le colonne nascoste. Il riquadro **Mostra colonne nell'ordine seguente** contiene le colonne visualizzate. Utilizzare i pulsanti **Aggiungi** e **Rimuovi** per spostare le colonne da un campo all'altro. Utilizzare i pulsanti **Vai su** e **Vai giù** per posizionare le colonne. 

>[!TIP]
>Selezionare la casella di controllo **Inserimento rapido** per aggiungere il campo all'elenco dei campi con Inserimento rapido. Quando si lavora nella pagina e si preme il tasto INVIO in un campo, il puntatore salta al campo successivo impostato come campo di inserimento rapido. 

### <a name="to-set-the-freeze-pane"></a>Per impostare il blocco riquadri
Un elenco può includere molte colonne e potrebbe essere necessario scorrere orizzontalmente per visualizzarle tutte. Potrebbero essere presenti alcune colonne che si desidera visualizzare sempre, anche mentre si scorre. A tale scopo, è possibile aggiungere un riquadro di blocco verticale per evitare lo scorrimento di alcune colonne. Questo consente di garantire che solo le colonne meno importanti si spostino quando si esegue lo scorrimento.

Per impostare il riquadro di blocco, selezionare la colonna dopo cui posizionare l'inizio del blocco, quindi scegliere **Aggiungi Blocca riquadro**.

## <a name="customizing-the-navigation-pane"></a>Personalizzazione del riquadro di spostamento.
Nel riquadro di spostamento viene visualizzato un menu dei collegamenti alle diverse pagine dell'elenco. Tali collegamenti vengono raggruppati nei pulsanti a livello di radice. 

### <a name="to-customize-the-navigation-pane"></a>Per personalizzare il riquadro di spostamento  
  
Scegliere l'icona del menu **Applicazione** ![Pulsante menu Applicazione nella barra dei menu](media/applicationmenuicon.png "ApplicationMenuIcon"), selezionare **Personalizza** quindi scegliere **Personalizza riquadro di spostamento**.  
  
### <a name="rename-or-rearrange-buttons-in-the-navigation-pane"></a>Ridenominare o riorganizzare i pulsanti nel riquadro di spostamento  
Nel riquadro sinistro della finestra di dialogo **Personalizza riquadro di spostamento** selezionare il pulsante che si desidera spostare, rinominare o rimuovere, quindi fare clic sul pulsante corrispondente al centro della finestra.

Non è possibile spostare, rinominare o rimuovere il pulsante **Pagina iniziale**. Il pulsante **Reparti** può essere rimosso dal riquadro di spostamento, ma non rinominato o spostato. 
  
### <a name="add-a-new-menu-button"></a>Aggiungere un nuovo pulsante di menu 
È possibile creare un nuovo pulsante a livello radice e quindi aggiungere un menu di collegamenti nel pulsante per aprire le diverse pagine.

1. Nella finestra di dialogo **Personalizza riquadro di spostamento** selezionare **Nuovo**, digitare un nome nel campo **Nome**.
2.  Scegliere il pulsante **OK**.

A questo punto è possibile aggiungere i collegamenti al pulsante.  
  
### <a name="add-a-link-to-a-button"></a>Aggiungere un collegamento a un pulsante   
Se si dispone dell'autorizzazione per visualizzare una lista, ad esempio la lista degli ordini di vendita, è possibile aggiungere un collegamento per la lista a uno dei pulsanti presenti nel riquadro di spostamento.  
  
1.  Nel campo **Pulsanti del riquadro di spostamento** della finestra di dialogo **Personalizza riquadro di spostamento** selezionare il menu a cui si desidera aggiungere il collegamento.  
  
2.  Scegliere il pulsante **Aggiungi**.  
  
3.  Selezionare il collegamento che si desidera aggiungere, quindi scegliere il pulsante **OK**.  
> [!TIP]
> Se nelle pagine di **Reparti** è presente un collegamento, è possibile aggiungerlo anche al riquadro di spostamento. Per ulteriori informazioni, vedere la sezione Aggiunta di un collegamento da Reparti alla Gestione ruolo utente.  
  
### <a name="move-or-copy-a-link-from-one-button-to-another"></a>Spostare o copiare un collegamento da un pulsante all'altro:  
  
1.  Nel campo **Pulsanti del riquadro di spostamento** della finestra di dialogo **Personalizza riquadro di spostamento** selezionare il menu in cui è attualmente visualizzato il collegamento.  
  
2.  Nel riquadro **Liste** selezionare il collegamento che si desidera spostare, quindi scegliere **Sposta in** o **Copia in**.  
  
3.  Selezionare il pulsante di spostamento a cui si desidera aggiungere il collegamento, quindi scegliere **OK**.  
  
### <a name="rearrange-the-order-of-a-links-under-a-button"></a>Riorganizzare l'ordine di collegamenti in un pulsante  
  
1.  Nel riquadro **Liste** selezionare il collegamento che si desidera spostare.  
  
2.  Utilizzare i pulsanti **Vai su** e **Vai giù** per posizionare il collegamento.

## <a name="adding-department-links-to-the-role-center"></a>Aggiungere collegamenti dei reparti alla Gestione ruolo utente
In una pagina di **Reparti** potrebbe essere presente un collegamento che si desidera aggiungere a Gestione ruolo utente per accedere facilmente. Il punto in cui posizionare il collegamento in Gestione ruolo utente dipende dalla categoria del collegamento nella pagina **Reparti**.

Nella seguente tabella sono descritti i tipi di collegamenti in ogni categoria nelle pagine di **Reparti** e la posizione di Gestione ruolo utente in cui è possibile aggiungerli.  
  
|**Categoria**|**Contiene**|**Aggiungere il collegamento a**|  
|------------------|------------------|---------------------|  
|Liste|Pagine di elenco|Pulsante **Pagina iniziale** del riquadro di spostamento|  
|Task|Pagine dei task, processi batch, prospetti, registrazioni|Scheda **Azioni** nella barra multifunzione|  
|Report e analisi|Report, processi batch, finestre di matrice|Scheda **Report** nella barra multifunzione|  
|Documenti|Documenti quali fatture e solleciti|**Report** nella barra multifunzione|  
|Archivio/Storico|Documenti registrati/completati, registri|Pulsante **Pagina iniziale** del riquadro di spostamento|  
|Setup|Finestre di setup|Scheda **Azioni** nella barra multifunzione|  
  
### <a name="to-copy-department-links-to-your-role-center"></a>Per copiare collegamenti di Reparti in Gestione ruolo utente  
  
1.  Apre la pagina **Reparti**.  
  
2.  Fare clic con il pulsante destro del mouse sul collegamento e scegliere una delle seguenti opzioni. Sarà disponibile solo una delle opzioni elencate.  
  
    |**Selezionare**|**Per aggiungere il collegamento a**|  
    |----------------|----------------------------|  
    |**Aggiungi al riquadro di spostamento**|Il pulsante **Pagina iniziale** nel riquadro di spostamento di Gestione ruolo utente.|  
    |**Aggiungi ad azioni nella barra multifunzione Gestione ruolo utente**|Il menu **Azioni** sulla barra multifunzione nella Gestione ruolo utente|  
    |**Aggiungi a report nella barra multifunzione Gestione ruolo utente**|Il menu **Report** sulla barra multifunzione nella Gestione ruolo utente|  
  
3.  Confermare il messaggio che viene visualizzato.  
  
 Il nuovo collegamento sarà visualizzato nel menu a cui è stato aggiunto. È tuttavia possibile, se lo si desidera, spostare il collegamento in un'altra posizione nel menu. Ad esempio, se il collegamento è stato aggiunto al riquadro di spostamento, verrà visualizzato nel menu **Home**, ma può essere spostato in un altro menu del riquadro di spostamento. Per ulteriori informazioni, vedere la sezione Personalizzazione del riquadro di spostamento. 

## <a name="adding-charts-to-role-centers-and-list-pages"></a>Aggiungere grafici alle pagine di elenchi e gestione ruolo utente
In presenza di informazioni complesse, è possibile visualizzare una rappresentazione visiva dei dati per individuare meglio le tendenze e prendere decisioni. È ad esempio possibile monitorare i saldi per conto corrente bancario della società in un grafico. Utilizzare il riquadro grafici per mostrare i dati da una lista nei tipi di pagine seguenti:  
  
-   In Gestione ruolo utente, dove è possibile scegliere tra grafici generici predefiniti.  
  
-   In una pagina elenco, dove è possibile scegliere di visualizzare un elenco come grafico.  
  
### <a name="to-add-a-generic-chart-to-your-role-center"></a>Per aggiungere un grafico generico in Gestione ruolo utente  
  
1.  In Gestione ruolo utente scegliere l'icona del menu **Applicazione** ![Pulsante menu Applicazione nella barra dei menu](media/applicationmenuicon.png "ApplicationMenuIcon"), selezionare **Personalizza** quindi **Personalizza pagina**.  
  
2.  Nel campo **Parti disponibili** della finestra **Personalizza Gestione ruolo utente** selezionare **Parte grafico**, quindi scegliere **Aggiungi**.  
  
3.  Utilizzare i pulsanti **Vai su**, **Vai giù**, **Sposta a sinistra** e **Sposta a destra** per posizionare la parte del grafico in Gestione ruolo utente.  
  
4.  Selezionare la parte del grafico, scegliere **Personalizzare parte**.  
  
5.  Nella finestra **Personalizza grafico** selezionare il grafico di default che si desidera visualizzare, quindi scegliere **OK**.  
  
### <a name="to-view-a-list-as-a-chart"></a>Per visualizzare una lista come grafico  
  
1.  Nella pagina elenco selezionare l'azione **Mostra come grafico**.  
  
2.  Selezionare una misura e una dimensione per creare un grafico personalizzato. Per visualizzare informazioni aggiuntive, selezionare una dimensione secondaria. Ad esempio, per creare un semplice grafico a barre, selezionare una dimensione sull'asse x e la dimensione **Conteggio dimensioni** sull'asse y.  
  
> [!NOTE]  
>  Per default, il riquadro Grafici è nascosto in quanto può rallentare le prestazioni. È consigliabile mostrare il grafico solo quando è necessario avere a disposizione le informazioni.  
    
## <a name="handling-external-files-and-automation-objects"></a>Gestione di file esterni e oggetti di automazione
Quando [!INCLUDE[navnow_md](includes/navnow_md.md)] riceve un file esterno, viene visualizzata una finestra di dialogo. Oltre a selezionare un'azione sul file, è possibile decidere come trattare quel tipo di file la volta successiva che sarà ricevuto.  
  
Quando [!INCLUDE[navnow_md](includes/navnow_md.md)] deve eseguire un oggetto di automazione, viene visualizzata una finestra di dialogo. È possibile decidere se quel tipo di oggetto deve sempre poter essere eseguito o mai.  
  
### <a name="to-specify-how-to-handle-external-files"></a>Per specificare come gestire i file esterni  
  
1.  Quando appare la finestra di dialogo, deselezionare la casella di controllo **Chiedi sempre prima di aprire questo tipo di file** se si desidera che [!INCLUDE[navnow_md](includes/navnow_md.md)] ricordi l'opzione selezionata nel passaggio 2. La volta successiva in cui il tipo file deve essere gestito, la finestra di dialogo non verrà visualizzata e il file verrà gestito come specificato nel passaggio 2.  
  
     In alternativa, selezionare la casella di controllo **Chiedi sempre prima di aprire questo tipo di file** da presentare sempre alla finestra di dialogo quando questo tipo di file è stato ricevuto.  
  
2.  Selezionare **Apri**, **Salva** o **Annulla**. Il file viene trattato in base alla selezione.  
  
### <a name="to-specify-how-to-handle-automation-objects"></a>Per specificare come gestire gli oggetti ActiveX  
  
Quando viene visualizzata la finestra di dialogo, selezionare la casella di controllo **Consenti sempre** se si desidera che in [!INCLUDE[navnow_md](includes/navnow_md.md)] venga sempre eseguito quel tipo di oggetto di automazione. La volta successiva che sarà richiesta l'esecuzione di quel tipo di oggetto ActiveX, la finestra di dialogo non apparirà e l'oggetto ActiveX verrà eseguito direttamente.  
  
In alternativa, selezionare la casella di controllo **Non consentire mai** su. La volta successiva che sarà richiesta l'esecuzione di quel tipo di oggetto ActiveX, la finestra di dialogo non apparirà e l'oggetto ActiveX non verrà eseguito.  

## <a name="CancelPersonalization"></a>Annullamento della personalizzazione
L'annullamento della personalizzazione può essere suddiviso in due categorie:

-   L'annullamento delle modifiche effettuate tramite la funzionalità **Personalizza**.
-   L'annullamento delle modifiche di base dell'interfaccia utente. 

### <a name="cancel-customization"></a>Annullare la personalizzazione
Per annullare tutte le personalizzazioni dell'interfaccia utente apportate a una pagina con le credenziali di accesso dell'utente corrente o dall'ultima volta che sono state annullate delle personalizzazioni dell'interfaccia utente, è possibile utilizzare la finestra **Elimina personalizzazione utente**. Il layout della pagina per la quale si elimina la personalizzazione viene reimpostato sulla configurazione predefinita per il profilo.  
  
Se si desidera annullare la personalizzazione dell'interfaccia utente apportata a un'area specifica dell'interfaccia utente in una pagina, ad esempio la barra multifunzione, è possibile utilizzare il pulsante **Ripristina default** nella finestra **Personalizza**. Il layout dell'area dell'interfaccia utente specifica in quella pagina viene quindi reimpostato sulla configurazione predefinita per il profilo.  
  
#### <a name="to-cancel-all-ui-customization-that-you-have-made-to-a-page"></a>Per annullare tutta la personalizzazione dell'interfaccia utente apportata a una pagina  
  
1.  Nella casella **Cerca** immettere **Elimina personalizzazione utente**, quindi selezionare il collegamento correlato.  
  
2.  Selezionare la pagina per la quale si desidera annullare la personalizzazione dell'interfaccia utente, quindi, nella scheda **Pagina iniziale**, nel gruppo **Visualizzazione**, fare clic su **Elimina**.  
  
> [!NOTE]  
>  Tutte le personalizzazioni dell'interfaccia utente della pagina eseguite con le credenziali di accesso correnti o dall'ultimo utilizzo della finestra **Elimina personalizzazione utente** vengono annullate. Il layout della pagina viene reimpostato sulla configurazione predefinita per il profilo, così come è stato configurato dall'amministratore o installato con Microsoft Dynamics NAV.  
  
#### <a name="to-cancel-ui-customization-that-you-have-made-to-a-ui-area-on-a-page"></a>Per annullare tutta la personalizzazione dell'interfaccia utente apportata a un'area dell'interfaccia utente in una pagina  
  
1.  Nella pagina in cui è stata personalizzata un'area dell'interfaccia utente, scegliere il menu **Applicazione** ![Pulsante menu Applicazione nella barra dei menu](media/applicationmenuicon.png "ApplicationMenuIcon"), scegliere **Personalizza**, quindi **Personalizza <UI area>**.  
  
2.  Infondo alla finestra **Personalizza** selezionare il pulsante **Ripristina default**.  
  
> [!NOTE]  
>  Tutte le personalizzazioni dell'area interfaccia utente eseguite per la pagina con le credenziali di accesso correnti o dall'ultimo utilizzo del pulsante **Ripristina default** vengono annullate. Il layout dell'area dell'interfaccia utente sulla pagina viene reimpostato sulla configurazione predefinita per il profilo, così come è stato configurato dall'amministratore o installato con Microsoft Dynamics NAV.

### <a name="cancel-basic-ui-changes"></a>Annullare le modifiche di base dell'interfaccia utente
È possibile annullare le modifiche di base dell'interfaccia utente aprendo la finestra **Ripristina impostazioni specifiche dell'utente** da Gestione ruolo utente.  
  
Le modifiche di base dell'interfaccia utente includono:
 -  Modifiche della dimensione e della posizione di qualsiasi finestra.
 -  Modifica della larghezza delle colonna.
 -  Modifica dell'altezza delle intestazioni di colonna.
 -  Ordinamento delle colonne di un elenco.
 -  Visualizzazione di elenchi come grafici.
 -  Specificare come gestire i file esterni e gli oggetti di automazione.  
 
#### <a name="to-cancel-basic-ui-changes"></a>Per annullare le modifiche di base dell'interfaccia utente
  
1.  Andare a Gestione ruolo utente personale.  
  
     Nel menu **Applicazione** ![Pulsante menu Applicazione nella barra dei menu](media/applicationmenuicon.png "ApplicationMenuIcon"), scegliere **Personalizza** e quindi **Ripristina impostazioni specifiche dell'utente**.  
  
2.  Selezionare il pulsante **Ripristina impostazioni dell'interfaccia utente**. In alternativa, fare clic sul pulsante **Ripristina tutto** per annullare le decisioni per la gestione dei file e gli oggetti di automazione.  
  
 Tutte le modifiche di base dell'interfaccia utente eseguite con le credenziali di accesso corrente a [!INCLUDE[navnow_md](includes/navnow_md.md)] o dall'ultima selezione del pulsante **Ripristina impostazioni dell'interfaccia utente** vengono annullate. L'interfaccia utente viene reimpostata sulla configurazione predefinita per il profilo.  
  
#### <a name="to-cancel-your-decision-for-running-or-saving-external-files"></a>Per annullare la propria decisione per l'esecuzione o il salvataggio di file esterni  
  
1.  Andare a Gestione ruolo utente personale.  
  
     Nel menu **Applicazione** ![Pulsante menu Applicazione nella barra dei menu](media/applicationmenuicon.png "ApplicationMenuIcon"), scegliere **Personalizza** e quindi **Ripristina impostazioni specifiche dell'utente**.  
  
2.  Selezionare il pulsante **Ripristina decisione di gestione dei file**. In alternativa, fare clic sul pulsante **Ripristina tutto** per annullare anche le modifiche alla vista e la decisione per la gestione degli oggetti di automazione.  
  
 Tutte le decisioni per la gestione predefinita dei tipi di file effettuate con le credenziali di accesso correnti o dall'ultima selezione del pulsante **Accesso ai file client** vengono annullate e reimpostate alla configurazione predefinita per il profilo. La volta successiva che [!INCLUDE[navnow_md](includes/navnow_md.md)] riceve un file esterno di qualsiasi tipo, viene visualizzata una finestra di dialogo con le opzioni **Salva**, **Esegui** e **Annulla**.  
  
### <a name="to-cancel-your-decision-for-handling-automation-objects"></a>Per annullare la propria decisione sulla gestione degli oggetti ActiveX  
  
1.  Andare a Gestione ruolo utente personale.  
  
     Nel menu **Applicazione** ![Pulsante menu Applicazione nella barra dei menu](media/applicationmenuicon.png "ApplicationMenuIcon"), scegliere **Personalizza** e quindi **Ripristina impostazioni specifiche dell'utente**.  
  
2.  Selezionare il pulsante **Ripristina decisioni di automazione**. In alternativa, fare clic sul pulsante **Ripristina tutto** per annullare anche le modifiche alla vista e la decisione per l'esecuzione o il salvataggio dei file esterni.  
  
 Tutte le decisioni su come eseguire gli oggetti automatici con le credenziali di accesso corrente o dall'ultima selezione del pulsante **Ripristina decisioni di automazione** vengono annullate. Il comportamento di gestione dei file viene reimpostato sulla configurazione predefinita per il profilo. La volta successiva che in [!INCLUDE[navnow_md](includes/navnow_md.md)] dovrà essere eseguito un oggetto ActiveX di qualsiasi tipo, verrà visualizzata una finestra di dialogo con le opzioni **Consenti sempre** e **Non consentire mai**.    

<!--Use the following table to get more information about customizing the different elements of the UI.

| To | See |
| --- | --- |
| Change which actions to show on the ribbon and how the actions are grouped. |[How to: Customize FastTabs](purchasing-how-record-purchases.md) |
|Change which FastTabs to show and which fields to include on the FastTabs.|[How to: Request Quotes](purchasing-how-request-quotes.md)|
|Add, remove, or arrange columns in a list or document-lines that represent fields in the underlying tables. |[ How to: Add or Remove Columns in a List or on Document Lines](purchasing-how-purchase-products-sale.md) |
| Rename or rearrange buttons, create a new menu button, add a link to a menu, or rearrange the order of a menu. |[ How to: Customize the Navigation Pane](purchasing-how-correct-cancel-unpaid-purchase-invoices.md) |
| Add a link from a department page to your Role Center. |[How to: Process Purchase Returns or Cancellations](purchasing-how-register-new-vendors.md) |
|Add a chart to your Role Center or to a list page.|[How to: Combine Receipts on a Single Invoice](purchasing-how-to-combine-receipts.md)|
| Unod personalization that you have made to your user interface, either for a specific area on a page, such as a ribbon, or for the whole page.|[How to: Cancel Personalization](ui-customization-cancel.md)|
-->


## <a name="see-also"></a>Vedi anche
[Personalizzazione dell'area di lavoro nel client Web di Dynamics](ui-personalization-user.md)  
[Sintesi della personalizzazione](ui-personalization-overview.md)  



