---
title: Configurazione dell'interfaccia utente (IU) per gli utenti
description: "L'amministratore configura le interfacce utente predefinite della società personalizzando i layout di pagina per i diversi profili utente nella società."
author: jswymer
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: customize pages, configure user interface, customize UI
ms.date: 07/01/2017
ms.author: jswymer
ms.prod: dynamics-nav-2018
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 7ba3d45a856eb38fe99fc5012b4e2f2d8609f9ce
ms.contentlocale: it-it
ms.lasthandoff: 10/16/2017

---
# <a name="configuring-the-user-interface-ui-for-users"></a>Configurazione dell'interfaccia utente (IU) per gli utenti
L'amministratore configura le interfacce utente predefinite della società personalizzando i layout di pagina per i diversi profili utente nella società. Per eseguire questa attività, è necessario essere un amministratore con il set di autorizzazioni SUPER. Inoltre, è necessario configurare i profili e assegnare gli utenti appropriati. Per ulteriori informazioni, vedere [Gestione di utenti, profili e Gestioni ruolo utente](admin-users-profiles-roles.md).  
  
È possibile configurare l'interfaccia utente per più utenti personalizzando le pagine per un profilo specifico a cui sono assegnati gli utenti. A tale scopo utilizzare [!INCLUDE[nav_windows](includes/nav_windows_md.md)] e personalizzare nello stesso modo in cui i singoli utenti personalizzano le proprie aree di lavoro, ovvero mediante la funzione **Personalizza**. La differenza è costituita dal fatto che si apre [!INCLUDE[nav_windows](includes/nav_windows_md.md)] in modalità configurazione. Le personalizzazioni standard includono le azioni da includere nella barra multifunzione, il posizionamento dei campi nelle Schede dettaglio o nei Dettaglio informazioni e le voci di menu da includere nel riquadro di spostamento. 

> [!TIP]  
>  È possibile implementare le configurazioni dell'interfaccia utente per un profilo in modo rapido se si dispone già di un profilo configurato in un database [!INCLUDE[d365fin](includes/d365fin_md.md)] diverso. È possibile esportare tale profilo, quindi importarlo nel database corrente. Per ulteriori informazioni, vedere [Esportazione e importazione di profili](admin-profiles.md#ExportImportProfile).  
  
## <a name="general-information"></a>Informazioni generali
Prendere in considerazione le seguenti informazioni prima di avviare la configurazione dell'interfaccia utente:
-   Prima di iniziare a configurare l'interfaccia utente, l'applicazione può essere configurata per visualizzare e nascondere gli elementi dell'interfaccia utente (ad esempio campi, Schede dettaglio e riquadri Dettaglio informazioni) in base alla licenza o alle autorizzazioni dell'utente. Per ulteriori informazioni su come effettuare tale operazione, vedere [Rimozione di elementi dall'interfaccia utente in base alle autorizzazioni](https://msdn.microsoft.com/en-us/dynamics-nav/removing-elements-from-the-user-interface-according-to-permissions).

    Per vedere l'effetto dell'opzione Rimozione degli elementi dell'interfaccia utente, è possibile accedere come utente di test con il set di autorizzazioni del profilo che si sta configurando. Il motivo è che in qualità di amministratore si dispone del set di autorizzazioni SUPER e pertanto non è possibile vedere l'interfaccia utente risultante durante l'accesso e tanto meno eseguire i test su questa interfaccia utente.    
-   Quando si effettuano le modifiche di configurazione dell'interfaccia utente per una pagina che un utente ha personalizzato, la personalizzazione dell'interfaccia utente viene mantenuta e non viene sovrascritta dalla nuova configurazione della pagina. Inoltre, quando si annulla la configurazione dell'interfaccia utente di una pagina che da allora un utente ha personalizzato, la personalizzazione dell'interfaccia utente non viene annullata.
-   L'unica situazione in cui la configurazione dell'interfaccia utente ignora la personalizzazione dell'interfaccia utente è quando un elemento all'interfaccia utente viene rimosso dalla configurazione. Ad esempio, se l'amministratore rimuove un campo che l'utente ha rinominato o spostato, allora il campo sarà eliminato dall'interfaccia utente.
-   È possibile registrare più configurazioni dell'interfaccia utente della stessa pagina in base a differenti punti di accesso alla pagina. Ad esempio, la finestra **Ordini vendita** può essere personalizzata e apparire diversa all'apertura dalla finestra **Scheda cliente** rispetto a quando viene aperta dalla Gestione ruolo utente **Gestore ordini vendite**. Il punto da cui è possibile accedere alla pagina da personalizzare viene registrato nella personalizzazione di quella specifica pagina. Di conseguenza, potrebbero esserci più record di personalizzazione della pagina nel database, come è possibile vedere nella finestra **Elimina configurazione profilo**.  
-   A differenza di quando gli utenti modificano le dimensioni delle finestre o la larghezza delle colonne nel proprio computer, eventuali modifiche di visualizzazione di base che si apportano durante la configurazione dell'interfaccia utente per un profilo non vengono salvate nel profilo e non saranno disponibili per gli utenti assegnati al profilo. Le modifiche di visualizzazione di base non sono specifiche del computer.   

## <a name="configure-a-profile-with-the-includenavwindowsincludesnavwindowsmdmd-in-configuration-mode"></a>Configurare un profilo con [!INCLUDE[nav_windows](includes/nav_windows_md.md)] in modalità configurazione
1.  Aprire un prompt dei comandi e digitare il seguente comando per passare alla cartella di installazione di [!INCLUDE[nav_windows](includes/nav_windows_md.md)]. Ad esempio:  
  
    ```  
    cd C:\Program Files\(x86)\Microsoft Dynamics NAV\110\RoleTailored Client  
    ```  
  
2.  Digitare il seguente comando per avviare [!INCLUDE[nav_windows](includes/nav_windows_md.md)] in modalità configurazione per un profilo specifico:  
  
    ```  
    Microsoft.Dynamics.Nav.Client.exe -configure -profile:"profileid"  
    ```  
  
     Sostituire **profileid** con il nome del profilo che si desidera configurare.  
  
     Ad esempio, per configurare il profilo Manager contabilità, utilizzare questo comando:  
  
    ```  
    Microsoft.Dynamics.Nav.Client.exe -configure -profile:"Accounting Manager"  
    ``` 

3. È ora possibile iniziare a configurare l'interfaccia utente nello stesso modo in cui i singoli utenti personalizzano le proprie aree di lavoro. Per ulteriori informazioni, vedere [Personalizzazione dell'area di lavoro in [!INCLUDE[nav_windows](includes/nav_windows_md.md)]](ui-personalization-windows-client.md). 

## <a name="cancel-ui-configuration"></a>Annullare la configurazione dell'interfaccia utente
È possibile annullare le personalizzazioni dell'interfaccia utente che sono state apportate come configurazione per un profilo in tre modi:  
  
-   Annullare tutte le personalizzazioni dell'interfaccia utente eseguite per un profilo con il pulsante **Cancella pagine configurate** nella finestra **Scheda profilo**.  
  
-   Annullare la personalizzazione dell'interfaccia utente eseguita per pagine specifiche di un profilo eliminando righe nella finestra **Elimina configurazione profilo**.  
  
-   Annullare la personalizzazione dell'interfaccia utente effettuata per un'area specifica dell'interfaccia utente per una pagina specifica per un profilo con il pulsante **Ripristina default** nella finestra **Personalizza**.  
  
### <a name="general-information"></a>Informazioni generali  
-   Gli utenti possono personalizzare la propria interfaccia utente utilizzando le proprie credenziali di accesso. Quando si annulla la configurazione dell'interfaccia utente di una pagina che da allora un utente ha personalizzato, la personalizzazione dell'interfaccia utente non viene annullata. Analogamente, quando si crea una nuova configurazione dell'interfaccia utente per una pagina che un utente ha personalizzato, la personalizzazione dell'interfaccia utente viene mantenuta e non viene sovrascritta dalla nuova configurazione della pagina.  

    L'unica situazione in cui la configurazione dell'interfaccia utente ignora la personalizzazione dell'interfaccia utente è quando un elemento all'interfaccia utente viene rimosso dalla configurazione. Ad esempio, se l'amministratore rimuove un campo che l'utente ha rinominato o spostato, allora il campo sarà eliminato dall'interfaccia utente.  
  
-   Nella finestra **Elimina personalizzazione utente** e con il pulsante **Ripristina default** nella finestra **Personalizza**, gli utenti possono annullare la personalizzazione dell'interfaccia utente che hanno apportato alle pagine accedendo con le proprie credenziali. In questo caso, il layout delle pagine viene reimpostato su una qualsiasi personalizzazione dell'interfaccia utente che l'amministratore ha configurato per il profilo. Se il profilo non è stato configurato, il layout delle pagine dell'utente viene reimpostato alla configurazione del profilo predefinito. Per ulteriori informazioni su come gli utenti possono annullare la personalizzazione, vedere [Annullamento della personalizzazione](ui-personalization-windows-client.md#CancelPersonalization).
  
### <a name="to-cancel-all-ui-customization-that-you-have-made-for-a-profile"></a>Per annullare tutta la personalizzazione dell'interfaccia utente apportata per un profilo  
  
1.  Nella casella **Cerca**, immettere **Profili**, quindi selezionare il collegamento correlato.  
  
2.  Selezionare il profilo per il quale si desidera annullare tutte le personalizzazioni dell'interfaccia utente, quindi, nella scheda **Pagina iniziale**, nel gruppo **Gestione**, fare clic su **Modifica**.  
  
3.  Nella finestra **Scheda profilo**, nella scheda **Azioni**, nel gruppo **Funzioni** scegliere **Cancella pagine configurate**.  
  
> [!NOTE]  
>  Eventuali personalizzazioni dell'interfaccia utente per il profilo, sia installate con l'applicazione che eseguite dall'amministratore, vengono annullate. Nessun layout di pagina specifico al profilo rimane nel database.  
  
### <a name="to-cancel-ui-customization-that-you-have-made-for-specific-page-for-a-profile"></a>Per annullare la personalizzazione dell'interfaccia utente apportata per una pagina specifica per un profilo  
  
1.  Nella casella **Cerca**, immettere **Elimina configurazione profilo**, quindi selezionare il collegamento correlato.  
  
2.  Selezionare il set di profili/pagine per cui si desidera annullare la personalizzazione dell'interfaccia utente, quindi, nella scheda **Pagina iniziale**, nel gruppo **Gestione**, fare clic su **Elimina**.  
  
    > [!IMPORTANT]  
    >  Se sono state configurate differenti personalizzazioni dell'interfaccia utente della stessa pagina in base ai percorsi di spostamento alla pagina, ogni personalizzazione della pagina verrà elencata nella finestra **Elimina configurazione profilo** con le stesse informazioni. Non sono disponibili informazioni che consentano di identificare quale riga è correlata a quale percorso di navigazione. Di conseguenza, è necessario o eliminare le righe singolarmente dopo i controlli visivi nella pagina oppure eliminare tutte le righe con le personalizzazioni dell'interfaccia utente per il profilo o la pagina.
    >    
    >  Tutte le personalizzazioni dell'interfaccia utente per la pagina per il profilo effettuate mai all'installazione o dall'ultimo utilizzo della finestra **Elimina configurazione profilo** verranno annullate. Il layout della pagina viene reimpostato sul layout standard dell'oggetto pagina.  
  
### <a name="to-cancel-ui-customization-that-you-have-made-for-a-specific-ui-area-for-a-specific-page-for-a-profile"></a>Per annullare la personalizzazione dell'interfaccia utente apportata per un'area specifica dell'interfaccia utente per una pagina specifica per un profilo  
  
È possibile annullare le modifiche apportate a singole aree dell'interfaccia, ad esempio una barra multifunzione, utilizzando il pulsante **Ripristina default** nella finestra **Personalizza**. In alternativa, è possibile annullare tutte le modifiche dell'interfaccia utente effettuate per un profilo mediante la finestra **Elimina configurazione profilo**.  
  
La personalizzazione dell'interfaccia utente per il profilo dell'area dell'interfaccia utente specifica nella determinata pagina viene annullata. Il layout dell'area dell'interfaccia utente nella pagina viene reimpostato sulla configurazione predefinita, così come è stato configurato dall'amministratore o installato con l'applicazione.  
  
## <a name="see-also"></a>Vedi anche  
[Personalizzazione di [!INCLUDE[navnow_md](includes/navnow_md.md)]](ui-customizing-overview.md)   
