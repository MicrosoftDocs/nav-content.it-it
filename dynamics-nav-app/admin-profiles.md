---
title: Gestione di profili e Gestioni ruolo utente
description: Ottenere informazioni su come gestire gli utenti e le Gestioni ruolo utente in Dynamics NAV.
author: jswymer
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: profiles, roles, role centers, user roles
ms.date: 09/01/2017
ms.author: jswymer
ms.prod: dynamics-nav-2018
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: cd60cbc206b8e2cd6665b98ee49a5dc10c50fe08
ms.contentlocale: it-it
ms.lasthandoff: 10/16/2017

---
# <a name="managing-profiles-and-role-centers"></a>Gestione di profili e Gestioni ruolo utente
I profili sono raccolte di utenti [!INCLUDE[navnow_md](includes/navnow_md.md)] che condividono la stessa Gestione ruolo utente. La Gestione ruolo utente è un tipo di pagina nella quale è possibile inserire parti differenti. Ogni parte è un contenitore in cui è possibile ospitare altre pagine o parti di sistema di default, come, ad esempio, una parte Outlook o parti per l'aggiunta di task, notifiche o note.  

## <a name="about-profiles-and-role-centers"></a>Informazioni sui profili e sulle Gestioni ruolo utente
Utilizzare i profili per collegare gli utenti alle Gestioni ruolo utente predefinite. Una Gestione ruolo utente è una home page per tutti gli utenti di un profilo, configurata per riflettere i task e le priorità degli utenti del profilo. Ad esempio, la Gestione ruolo utente del gestore ordini è stata configurata per riflettere i task e le priorità di un gestore ordini. La Gestione ruolo utente consente di accedere facilmente alle informazioni necessarie agli utenti per svolgere le proprie attività quotidiane. Ad esempio, la Gestione ruolo utente determina le pile, o riquadri, che mostrano quando gli utenti accedono per la prima volta e i collegamenti dalla pagina di spostamento.

Il profilo utilizzato viene visualizzato nella testata dell'area di contenuto principale della Gestione ruolo utente. Un amministratore può personalizzare la Gestione ruolo utente in modo da soddisfare le esigenze di un ruolo specifico per una società specifica. La Gestione ruolo utente del gestore ordini può quindi essere ulteriormente personalizzata su un singolo computer per soddisfare le esigenze di una persona che sta portando avanti la commessa come gestore ordini. Questa persona può personalizzare la Gestione ruolo utente conservando le query, aggiungendo filtri e aggiungendo o rimuovendo campi.

I profili e le Gestioni ruolo utente sono allineati ai ruoli e alle responsabilità nell'organizzazione. [!INCLUDE[navnow_md](includes/navnow_md.md)] fornisce una serie di profili predefiniti, di cui ognuno corrisponde e collega a una Gestione ruolo utente. Gli amministratori possono modificare i profili esistenti o crearne di nuovi.  
  
> [!NOTE]  
>  i profili non sono esplicitamente collegati ai ruoli e ai permessi che costituiscono il sistema di protezione, ma gli utenti dei profili devono disporre dei permessi che allineano i loro ruoli nel sistema di protezione. Per ulteriori informazioni, vedere la pagina sulla [sicurezza nell'ambiente personalizzato in base al ruolo](http://go.microsoft.com/fwlink?LinkId=147633) in MSDN Library. 

## <a name="to-create-a-profile"></a>Per creare un profilo
1.  Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **Profili**, quindi scegliere il collegamento correlato.  
  
2.  Selezionare l'azione **Nuovo** per aprire la finestra **Scheda Nuovo profilo**.  
  
3.  Nel campo **ID profilo** immettere un nome che descriva il ruolo previsto dell'utente.  
  
4.  Nel campo **Descrizione** immettere una descrizione dell'ID profilo, ad esempio **Gestore ordini**.  
  
5.  Impostare il campo **ID Gestione ruolo utente** nella Gestione ruolo utente che si intende assegnare al profilo.  
  
6.  Per impostare questa Gestione ruolo utente come predefinita per il proflo, selezionare la casella di controllo **Gestione ruolo utente predefinita**.  
  
7.  Scegliere il pulsante **OK**. .  
  
La procedura per modificare un profilo esistente è identica, tranne che si seleziona un profilo esistente nella pagina Profili invece di fare clic su **Nuovo**.  


##<a name="copying-a-profile"></a>Copia di un profilo 
La copia di un profilo consente di risparmiare tempo se si desidera utilizzare impostazioni simili in un profilo e si desidera soltanto modificare poche impostazioni.

1.  Aprire il profilo che si desidera copiare, quindi scegliere l'azione **Copia profilo**.

2.  Nel campo **Nuovo ID profilo** immettere un nome per il profilo che si desidera copiare. 

3.  Impostare il campo **Nuovo ambito profilo** su una delle seguenti opzioni:

    - **Sistema** per rendere il nuovo profilo disponibile a tutti i database del tenant che utilizzano l'applicazione.
    - **Tenant** per rendere il nuovo profilo disponibile solo al database del tenant corrente. 
4. Al termine, scegliere il pulsante **OK**.

## <a name="ExportImportProfile"></a>Esportazione e importazione di profili

È possibile esportare e importare i profili come file XML a e da un database [!INCLUDE[d365fin](includes/d365fin_md.md)]. L'esportazione e l'importazione di un profilo consentono di risparmiare tempo quando si configura l'interfaccia utente perché si riutilizza una configurazione di profilo esistente anziché dover configurare un profilo da zero. Se si dispone di un profilo configurato in un database [!INCLUDE[d365fin](includes/d365fin_md.md)] e si desidera riutilizzare tutte o alcune delle stesse configurazioni del profilo in un database diverso, è possibile esportare il profilo in un file XML. Quindi, è possibile importare il file XML del profilo nel secondo database.

-   Per esportare un profilo, cercare e aprire la pagina **Esporta profili**, selezionare il profilo dall'elenco, quindi scegliere l'azione **Esporta**. Salvare il file XML in un'ubicazione sul computer o sulla rete. 
  
-   Per importare un profilo, cercare e aprire la pagina **Importa profili**, selezionare il file XML del profilo, quindi scegliere il pulsante **OK**. 

    > [!NOTE]  
    >  Non è possibile importare un profilo già esistente nel database, anche se il file XML è denominato in modo diverso o ha un contenuto diverso. È necessario eliminare il profilo esistente prima di importare quello nuovo. 



## <a name="see-also"></a>Vedi anche  
[Procedura: Gestire gli utenti e le autorizzazioni](ui-how-users-permissions.md)  
[Personalizzazione dell'interfaccia utente](ui-customizing-overview.md)   
<!--[Security Overview](../Security%20Overview.md)-->

