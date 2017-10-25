---
title: "Perché la personalizzazione di una pagina è bloccata"
description: "Descrizione dei motivi per cui non è possibile personalizzare una pagina e delle azioni che è possibile intraprendere per sbloccare la pagina e personalizzarla."
author: jswymer
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: personalization locked, cannot personalize page
ms.date: 09/07/2017
ms.author: jswymer
ms.prod: dynamics-nav-2018
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: b365d14c199d36abebcae0b3ac86340fd59cf8ef
ms.contentlocale: it-it
ms.lasthandoff: 10/16/2017

---
# <a name="why-is-the-page-is-locked-from-personalizing"></a>Perché la personalizzazione di una pagina è bloccata
Un'icona di blocco nel banner **Personalizzazione** quando viene aperta una pagina (come mostrato) indica che attualmente non sono consentite ulteriori modifiche di personalizzazione nella pagina di [!INCLUDE[nav_web](includes/nav_web_md.md)].

![Blocco della personalizzazione](media/personalization-locked.png "Blocco della personalizzazione")

Questo può avvenire per due motivi:
1.  Finora, è stato utilizzato solo [!INCLUDE[nav_windows_md](includes/nav_windows_md.md)] per personalizzare la pagina.

2. In precedenza, la pagina è stata personalizzata tramite [!INCLUDE[nav_web](includes/nav_web_md.md)], ma utilizzando una versione di [!INCLUDE[nav2017](includes/nav2017.md)] o una versione precedente.   

Per continuare a personalizzare la pagina utilizzando [!INCLUDE[nav_web](includes/nav_web_md.md)], scegliere l'icona del blocco e quindi **Sblocca**.

## <a name="what-happens-when-you-unlock-the-page"></a>Cosa succede quando si sblocca la pagina
Se si sceglie di sbloccare la pagina, la personalizzazione della pagina in [!INCLUDE[nav_web](includes/nav_web_md.md)] verrà annullata, ovvero la pagina ritornerà al layout originale e sarà necessario ricominciare da zero.

In [!INCLUDE[nav_windows_md](includes/nav_windows_md.md)], la pagina verrà conservata come in precedenza e non verrà interessata dalle nuove modifiche in [!INCLUDE[nav_web](includes/nav_web_md.md)]. Le personalizzazioni in [!INCLUDE[nav_web](includes/nav_web_md.md)] e [!INCLUDE[nav_windows_md](includes/nav_windows_md.md)] rimangono distinte e si avrà una versione personalizzata diversa per ogni client. 

Pertanto, in futuro, si personalizzerà separatamente la pagina nei due client. Di conseguenza, la pagina può potenzialmente apparire diversa nei due client.

## <a name="see-also"></a>Vedi anche
[Sintesi della personalizzazione](ui-personalization-overview.md)  
[Utilizzo della personalizzazione nel client Windows e nel client Web di Dynamics NAV](ui-personalization-overview.md#PersonalizationWinWeb)  
[Personalizzazione dell'area di lavoro tramite il client Web](ui-personalization-user.md)  
[Personalizzazione dell'area di lavoro tramite il client Windows](ui-personalization-windows-client.md)  
[Gestione della personalizzazione](ui-personalization-manage.md)  
[Utilizzo di [!INCLUDE[navnow_md](includes/navnow_md.md)]](ui-work-product.md)  
[Procedura: Modificare la Gestione ruolo utente](change-role.md)  

