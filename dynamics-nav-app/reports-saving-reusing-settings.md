---
title: Impostazioni salvate nei report
author: jswymer
ms.custom: na
ms.date: 09/26/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: 0f11d862315c8ecd160cd18afb0a72a2d684b9b2
ms.contentlocale: it-it
ms.lasthandoff: 06/26/2017

---
# <a name="saved-settings-on-reports"></a>Impostazioni salvate nei report
A seconda del report che viene eseguito, potrebbe apparire una pagina che consente di impostare determinate opzioni e filtri per variare i dati inclusi nel report generato. Questa pagina è nota come la pagina di richiesta report. Un report può includere uno o più *impostazioni salvate* che è possibile applicare al report dalla pagina di richiesta. Le *impostazioni salvate* sono fondamentalmente opzioni e filtri predefiniti. L'utilizzo delle impostazioni salvate è un metodo rapido e affidabile di generare coerentemente report contenenti dati corretti.

È possibile visualizzare le impostazioni salvate a disposizione dell'utente per un report nella sezione **Impostazioni salvate** della pagina di richiesta report.

## <a name="to-apply-saved-settings-to-a-report"></a>Per applicare le impostazioni salvate a un report
1.  Aprire il report.

    Viene visualizzata la pagina di richiesta report.    
2.  Nella sezione **Impostazioni salvate** della pagina impostare il campo **Nome** sulle impostazioni salvate che si desidera utilizzare.

    La sezione **Impostazioni salvate** viene visualizzata solo se il report è già stato eseguito in precedenza o se esistono movimenti salvati delle impostazioni. Esiste sempre una voce Impostazioni salvate, che viene chiamata **Filtri e opzioni utilizzati di recente**. Queste impostazioni sono i valori delle opzioni e dei filtri che sono stati utilizzati l'ultima volta che è stato eseguito il report.

## <a name="administer-saved-report-settings-for-users"></a>L'amministratore ha salvato le impostazioni dei report per gli utenti
Se si dispone delle autorizzazioni appropriate, è possibile visualizzare, creare e modificare le impostazioni salvate per tutti i report di tutti gli utenti nella società. È possibile assegnare le impostazioni salvate per un report ai singoli utenti o a tutti gli utenti della società.

È possibile gestire le impostazioni salvate nella pagina 1506 **Impostazioni report**. Per aprire questa pagina, nell'angolo superiore destro scegliere l'icona **Cerca pagina o report**, immettere **Impostazioni report**, quindi scegliere il collegamento correlato. 

Nella pagina **Impostazioni report** è possibile creare impostazioni ex novo o duplicarle e modificare le impostazioni esistenti. Per modificare le opzioni e i filtri di un'impostazione, scegliere l'azione **Modifica**.

**Note**:
-    La funzionalità Impostazioni salvate nei report è rilevante solo quando la proprietà SaveValues della pagina di richiesta è impostata su Sì. La proprietà SaveValues è impostata nell'ambiente di sviluppo.
-    Se si crea un articolo impostazioni salvato per tutti gli utenti con lo stesso nome di un'impostazione salvata esistente per un utente specifico, tale utente non potrà utilizzare le impostazioni salvate assegnata a tutti gli utenti.  Nel campo Impostazioni salvate nella pagina di richiesta del report, l'utente vedrà due opzioni delle impostazioni salvate con lo stesso nome. Tuttavia, indipendentemente dall'opzione che sceglie, verranno usate le impostazioni salvate specifiche dell'utente.

## <a name="see-also"></a>Vedi anche
[Programmare l'esecuzione di un report](ui-schedule-report.md)

