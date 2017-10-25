---
title: Gestione della personalizzazione come amministratore
description: Informazioni su come personalizzare l'interfaccia utente in base alle esigenze professionali.
documentationcenter: 
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
ms.openlocfilehash: e3d088c35efca4d62b7db1f0d44d5ef2958317d4
ms.contentlocale: it-it
ms.lasthandoff: 10/16/2017

---
# <a name="managing-personalization-as-an-administrator"></a>Gestione della personalizzazione come amministratore
Gli utenti possono personalizzare l'area di lavoro per adattarla alle proprie preferenze. In qualità di amministratore, è possibile controllare e gestire la personalizzazione disabilitando la possibilità per gli utenti di personalizzare le pagine e cancellando le personalizzazioni di pagina che gli utenti hanno effettuato.

## <a name="disable-personalization-for-a-profile"></a>Disabilitare la personalizzazione per un profilo
È possibile impedire a tutti gli utenti che appartengono a un profilo specifico di personalizzare le proprie pagine.
1.  Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **Profili**, quindi scegliere il collegamento correlato.
2.  Selezionare dall'elenco il profilo che si desidera modificare.
3.  Selezionare la casella di controllo **Disabilita personalizzazione** e quindi fare clic sul pulsante **OK**.

## <a name="clear-user-personalizations"></a>Cancellare le personalizzazioni dell'utente

La cancellazione delle modifiche di personalizzazione della pagina ripristina la pagina al layout originale prima che fosse apportata qualsiasi personalizzazione. Ci sono due modi per eliminare le personalizzazioni che gli utenti hanno apportato alle pagine: utilizzando la pagina **Elimina personalizzazione utente** o la pagina **Scheda personalizzazione utente**.

### <a name="clear-user-personalizations-by-using-the-delete-user-personalization-page"></a>Eliminare le personalizzazioni dell'utente tramite la pagina Elimina personalizzazione utente

La pagina **Elimina personalizzazione utente** consente di eliminare la personalizzazione in base alla pagina e all'utente.

1.  Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **Elimina personalizzazione utente**, quindi scegliere il collegamento correlato.

    Nella pagina vengono elencate tutte le pagine che sono state personalizzate e l'utente a cui appartengono.

    >[!NOTE]
    > Un segno di spunta nella colonna **Personalizzazione legacy** indica che una personalizzazione è stata effettuata solo tramite [!INCLUDE[nav_windows_md](includes/nav_windows_md.md)] e/o è stata effettuata in [!INCLUDE[nav_web_md](includes/nav_web_md.md)] precedentemente a [!INCLUDE[navnow_md](includes/navnow_md.md)]. Gli utenti che provano a personalizzare queste pagine utilizzando [!INCLUDE[nav_web_md](includes/nav_web_md.md)] vengono bloccati a meno che non scelgano di sbloccare la pagina. Per ulteriori informazioni, vedere [Perché la personalizzazione di una pagina è bloccata](ui-personalization-locked.md). Per ulteriori informazioni sulla personalizzazione in [!INCLUDE[nav_windows_md](includes/nav_windows_md.md)] e [!INCLUDE[nav_web_md](includes/nav_web_md.md)], vedere [Utilizzo della personalizzazione nel client Windows e nel client Web di Dynamics NAV](ui-personalization-overview.md#PersonalizationWinWeb).

2. Selezionare la voce che si desidera eliminare, quindi scegliere l'azione **Elimina**.

    L'utente visualizzerà le modifiche dopo l'accesso successivo.

### <a name="clear-user-personalizations-by-using-the-user-personalization-card-page"></a>Eliminare le personalizzazioni dell'utente tramite la pagina Scheda personalizzazione utente

La pagina **Scheda personalizzazione utente** consente di eliminare la personalizzazione in tutte le pagine per un utente specifico. Questa operazione richiede l'autorizzazione di scrittura per la tabella **Profilo** 2000000072.

1.  Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "Cerca pagina o report"), immettere **Personalizzazione utente**, quindi scegliere il collegamento correlato.

    Nella pagina **Personalizzazione utente** vengono elencati tutti gli utenti che potenzialmente dispongono di pagine personalizzate. Se non è presente un utente nell'elenco, significa che non dispone di pagine personalizzate.

2. Selezionare l'utente dalla lista, quindi scegliere l'azione **Modifica**.

3.  Nella scheda **Azioni**, scegliere **Cancella pagine personalizzate**.

    L'utente visualizzerà le modifiche dopo l'accesso successivo.

## <a name="see-also"></a>Vedi anche
[Sintesi della personalizzazione](ui-personalization-overview.md)  
[Personalizzazione dell'area di lavoro](ui-personalization-user.md)  
[Utilizzo di [!INCLUDE[navnow_md](includes/navnow_md.md)]](ui-work-product.md)  
[Procedura: Modificare la Gestione ruolo utente](change-role.md)  
