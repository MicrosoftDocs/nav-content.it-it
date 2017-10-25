---
title: Personalizzazione dell'area di lavoro - Sintesi
description: Informazioni su come personalizzare l'interfaccia utente in base alle esigenze professionali.
documentationcenter: 
author: jswymer
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.date: 07/26/2017
ms.author: jswymer
ms.prod: dynamics-nav-2018
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 04334d3bb50b37b9643b848ca4f59b015f03ad04
ms.contentlocale: it-it
ms.lasthandoff: 10/16/2017

---
# <a name="personalizing-your-workspace---overview"></a>Personalizzazione dell'area di lavoro - Sintesi
È possibile *personalizzare* l'area di lavoro per adattarla alle esigenze professionali e alle preferenze modificando il layout delle pagine in modo da visualizzare solo le informazioni necessarie, quando necessario. Le modifiche di personalizzazione apportate influenzeranno solo ciò che vede l'utente che le ha effettuate, non quello che altri utenti vedono.

È possibile personalizzare l'area di lavoro tramite [!INCLUDE[nav_windows_md](includes/nav_windows_md.md)] e [!INCLUDE[nav_web_md](includes/nav_web_md.md)]. Le modifiche di personalizzazione effettuate verranno visualizzate anche in [!INCLUDE[nav_phone_md](includes/nav_phone_md.md)] e [!INCLUDE[nav_web_md](includes/nav_phone_md.md)].
  
> [!NOTE]  
> L'amministratore della società potrebbe aver già personalizzato l'interfaccia utente di un utente con un layout specifico del ruolo per tutti gli utenti che hanno lo stesso profilo di quell'utente e utilizzano la stessa Gestione ruolo utente. Le personalizzazioni effettuate nell'area di lavoro vengono salvate nell'account utente, in modo che siano conservate anche se un amministratore rilascia un nuovo set di layout specifici per i ruoli dell'azienda. Per ulteriori informazioni, vedere [Configurazione dell'interfaccia utente](admin-configure-user-interface.md).

## <a name="comparing-personalization-in-the-dynamics-nav-windows-and-web-clients"></a>Confronto tra la personalizzazione nel client Windows e nel client Web di Dynamics NAV
A seconda della pagina, è possibile personalizzare molte parti dell'interfaccia utente, ad esempio quali campi o colonne vengono mostrati e dove sono posizionati, quali azioni sono incluse sulla barra multifunzione e molto altro ancora. Molte di queste operazioni possono essere effettuate sia nel client Windows che nel client Web. La tabella seguente fornisce una panoramica delle funzionalità di personalizzazione in ogni client.

|  Personalizza  ||  Client Windows  |  Client Web  |
|---------------|-|------------------|--------------|
|Campi delle Schede dettaglio||||
||Aggiungere, spostare, rimuovere |x|x|
||Visualizzazione nell'intestazione compressa|x||
||Nascondi nell'azione **Mostra più campi**|x||
|Elenchi o righe documento ||||
||Aggiungere, spostare, rimuovere colonne  |x|x|
||Aggiungere, spostare, rimuovere il riquadro di blocco  |x|x|
|Riquadri Dettaglio informazioni|||
||Spostare, rimuovere|x|x|
||Aggiungi|x||
||Aggiungere, spostare e rimuovere campi|x|x|
|Pile||||
||Spostare, rimuovere|x|x|
||Aggiungi |x||
|Grafici||||
||Spostare, rimuovere|x|x|
||Aggiungi|x| |
|Barra multifunzione e azioni||x||
|Riquadro di spostamento||x||

Un'altra differenza consiste nel fatto che quando si utilizza il client Windows, è possibile avere diverse versioni personalizzate della stessa pagina, basate su diversi punti di accesso alla pagina. Ad esempio, la pagina **Ordini vendita** può essere personalizzata per apparire diversa all'apertura dalla pagina **Scheda cliente** rispetto a quando viene aperta dalla pagina **Gestione ruolo utente Gestore ordini vendite**. Quando si personalizza una pagina utilizzando il client Web, esiste solo una versione personalizzata per pagina, pertanto le stesse modifiche verranno sempre visualizzate nella pagina, a prescindere dal punto in cui la si apre.

##  <a name="PersonalizationWinWeb"></a>Utilizzo della personalizzazione nel client Windows e nel client Web di Dynamics NAV
Prima di iniziare a personalizzare le pagine, è importante capire come funziona la personalizzazione nel client Windows e nel client Web. Se si utilizza solo il client Windows o il client Web, queste informazioni non sono così rilevanti. Tuttavia, le informazioni diventano importanti se si inizia a personalizzare le pagine utilizzando entrambi i client o se si passa dall'utilizzo del client Windows all'utilizzo permanente del client Web.  

-   Se si utilizza il client Windows per personalizzare una pagina specifica fin dall'inizio, le modifiche di personalizzazione della pagina verranno visualizzate anche nella pagina nel [!INCLUDE[nav_web_md](includes/nav_web_md.md)].

-   Finché si continua a utilizzare il client Windows per personalizzare la pagina, le modifiche di personalizzazione che si apportano avranno effetto anche sulla pagina del client Web.

-   Tuttavia, non appena si inizia a personalizzare la pagina utilizzando il client Web, la personalizzazione per quella pagina diventerà distinta per i due client e si avrà una versione personalizzata per ogni client. Nel client Web, le personalizzazioni precedenti della pagina verranno annullate, il che significa che la pagina tornerà al layout originale ed essenzialmente si inizierà la personalizzazione della pagina da zero. Le personalizzazione precedenti nel client Windows rimangono inalterate.

- Da questo punto in avanti, si personalizzerà la pagina del client Windows e del client Web indipendentemente l'una dall'altra, il che significa che la pagina può potenzialmente apparire diversa in ogni client. I client per telefono e tablet mostreranno le stesse personalizzazioni della pagina del client Web.  

> [!Tip]  
>Se si apre la pagina **Elimina personalizzazione utente**, è possibile visualizzare tutte le pagine che sono state personalizzate da ogni utente. La colonna **Personalizzazione legacy** indica se una personalizzazione è stata effettuata nel client Windows o nel client Web. Se è presente un segno di spunta nella colonna, la personalizzazione è stata effettuata nel client Windows (o nel client Web prima di [!INCLUDE[navnow_md](includes/navnow_md.md)]).

## <a name="see-also"></a>Vedi anche
[Personalizzazione dell'area di lavoro nel client Windows di Dynamics NAV](ui-personalization-windows-client.md)  
[Personalizzazione dell'area di lavoro nel client Web di Dynamics NAV](ui-personalization-user.md)  
[Gestione della personalizzazione](ui-personalization-manage.md)  
[Personalizzazione di Dynamics NAV](ui-customizing-overview.md)  

