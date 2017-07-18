---
title: Specificare la selezione della stampante per i report
author: SusanneWindfeldPedersen
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: 55b48aef2bc108ced7f581f0ff6c11263ee467df
ms.contentlocale: it-it
ms.lasthandoff: 06/26/2017

---
    
# <a name="specify-printer-selection-for-reports"></a>Specificare la selezione della stampante per i report
È possibile impostare i report in modo vengano stampati su una stampante specifica. Di seguito sono descritti alcuni utilizzi della selezione stampante: 

- È possibile stampare report sulla carta intestata speciale della società.
- È possibile stampare i report su formati carta diversi.
- È possibile stampare report sulla stampante di default di un impiegato specificato.

Utilizzare la finestra **Selezioni stampante** per impostare valori differenti al fine di ottenere un output differente. Se si imposta una selezione stampante specifica, questa ha la precedenza su una selezione stampante generale. Ad esempio, è possibile impostare una selezione stampante che dispone di valori nei campi **ID utente**, **ID report** e **Nome stampante**. Questa selezione stampante ha la precedenza su una selezione stampante che ha movimenti vuoti nei campi **ID report** o **ID utente**. 

Nella seguente tabella viene descritta la combinazione dei valori da specificare quando si impostano le selezioni stampante per un report.

|Per                                                 |Impostare i seguenti valori                                             |
|---------------------------------------------------|---------------------------------------------------------------------|
|Stampare un report su una stampante specifica per tutti gli utenti |Specificare i valori nei campi **Nome stampante** e **ID report** e lasciare vuoto il campo **ID utente**.|
|Stampare tutti i report su una stampante specifica per un utente specifico|Specificare i valori nei campi **ID utente** e **Nome stampante** e lasciare vuoto il campo **ID utente**.|
|Impostare la stampante di default per tutti i report|Specificare un valore nel campo **Nome stampante** e lasciare vuoti i campi **ID utente** e **ID report**.|
|Stampare un report specifico sulla stampante di default dell'utente|Specificare un valore nel campo **ID report** e lasciare vuoti i campi **Nome stampante** e **ID utente**.|
|Stampare un report specifico su una stampante specifica per un utente specifico|Specificare i valori in tutti e tre i campi.|

## <a name="see-also"></a>Vedi anche
[Utilizzare Dynamics NAV](ui-work-product.md)

