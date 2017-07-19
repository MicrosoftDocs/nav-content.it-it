---
title: Risoluzione dei problemi relativi all'iscrizione self-service
author: SusanneWindfeldPedersen
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: 931c427518694cbd0003ea82735292a019b388d5
ms.contentlocale: it-it
ms.lasthandoff: 06/26/2017

---

# <a name="troubleshooting-self-service-sign-up"></a>Risoluzione dei problemi relativi all'iscrizione self-service
L'iscrizione a Dynamics NAV è facile e può essere effettuata molto rapidamente. È possibile creare un account gratuito anche se si è un'organizzazione esistente. Questo articolo illustra i problemi che è possibile incontrare durante l'iscrizione.

## <a name="what-email-address-can-i-use-with-dynamics-nav"></a>Quale indirizzo e-mail posso utilizzare con Dynamics NAV?
Per l'iscrizione a Dynamics NAV è necessario utilizzare un indirizzo e-mail di lavoro o della scuola. Dynamics NAV non supporta gli indirizzi e-mail forniti dai servizi di posta elettronica di tipo consumer o dai provider di telecomunicazione. Questo include indirizzi di outlook.com, hotmail.com, gmail.com e altri simili.

Se si prova a effettuare l'iscrizione con un indirizzo e-mail personale, si riceve un messaggio che richiede di utilizzare un indirizzo e-mail un lavoro o di scuola.

## <a name="troubleshooting"></a>Troubleshooting
In molti casi, la registrazione a Dynamics NAV si ottiene seguendo il processo di iscrizione. Tuttavia, esistono diverse motivi per i quali non è possibile completare l'iscrizione self service. La tabella sottostante riepiloga alcuni dei motivi più comuni per cui non è possibile completare l'iscrizione e i modi in cui è possibile ovviare ai problemi.

|Sintomo/Messaggio di errore                                                                             |Causa e soluzione alternativa|
|--------------------------------------------------------------------------------------------------|--------------------|
|Per gli indirizzi e-mail Office 365 che non sono registrati negli Stati Uniti, durante l'iscrizione si riceve un messaggio simile al seguente: <br>**Impossibile eseguire l'iscrizione. Il paese non è ancora supportato.**<br> |Dynamics NAV attualmente supporta solo gli account e-mail di Office 365 registrati negli Stati Uniti.|
|Gli indirizzi e-mail personali come nancy@gmail.com non sono supportati. Durante l'iscrizione viene visualizzato un messaggio simile al seguente: <br>**È stato immesso un indirizzo e-mail personale. Immettere l'indirizzo e-mail di lavoro per consentirci di archiviare in modo sicuro i dati della società.**<br> oppure <br> **È possibile che sia stato utilizzato un indirizzo di posta elettronica personale. Immettere l'indirizzo di lavoro per connettersi agli altri utenti nella società. Nessuna preoccupazione. L'indirizzo immesso non verrà condiviso con nessuno.** | Dynamics NAV non supporta gli indirizzi e-mail forniti dai servizi di posta elettronica di tipo consumer o dai provider di telecomunicazioni. Per completare l'iscrizione, provare a utilizzare un indirizzo e-mail assegnato dall'organizzazione o dalla scuola. Se non è ancora possibile effettuare l'iscrizione e si desidera completare un processo di setup più avanzato, è possibile registrare una nuova sottoscrizione di prova di Office 365 e utilizzare tale indirizzo e-mail per effettuare l'iscrizione.
|Indirizzi e-mail .gov o .mil. Durante l'iscrizione è possibile ricevere un messaggio simile al seguente: <br>**Dynamics NAV non disponibili. Attualmente Dynamics NAV non è disponibile per gli utenti con indirizzi e-mail .gov o .mil. Utilizzare un altro indirizzo e-mail di lavoro o riprovare più tardi.** <br>oppure <br>**Impossibile completare l'iscrizione. Dynamics NAV non risulta disponibile per l'organizzazione o la scuola indicata.**|Al momento Dynamics NAV non supporta indirizzi e-mail .gov o .mil.|
|L'iscrizione self-service non è abilitata. Durante l'iscrizione viene visualizzato un messaggio simile al seguente: <br>**Impossibile completare l'iscrizione. Il reparto IT ha disattivato l'iscrizione a Dynamics VAN. Contattare il proprio reparto IT per completare l'iscrizione.** <br>oppure <br> **È possibile che sia stato utilizzato un indirizzo di posta elettronica personale. Immettere l'indirizzo di lavoro per connettersi agli altri utenti nella società. Nessuna preoccupazione. L'indirizzo immesso non verrà condiviso con nessuno.**|L'amministratore IT dell'organizzazione ha disabilitato l'iscrizione self service a Dynamics NAV. Per completare l'iscrizione, contattare l'amministratore IT e chiedergli di seguire le istruzioni indicate nella pagina sottostante per consentire agli utenti esistenti di iscriversi a Dynamics NAV e consentire a nuovi utenti di accedere al tenant esistente. Questo problema può verificarsi anche se è stato sottoscritto Office 365 tramite un partner.|
|L'indirizzo e-mail non è un ID di Office 365. Durante l'iscrizione viene visualizzato un messaggio simile al seguente: <br>**Impossibile individuare l'utente su contoso.com. Probabilmente utilizza un ID diverso al lavoro o a scuola. Provare ad accedere con quell'account e se non funziona contattare il proprio reparto IT.**|Per accedere a Office 365 e altri servizi Microsoft, l'organizzazione utilizza degli ID che sono diversi dall'indirizzo e-mail. Ad esempio, se l'indirizzo e-mail è Nancy.Smith@contoso.com, l'ID potrebbe essere  nancys@contoso.com. Per completare l'iscrizione, utilizzare l'ID assegnato dall'organizzazione per accedere a Office 365 o ad altri servizi Microsoft. Per ulteriori informazioni sull'ID, contattare l'amministratore IT. Se non è ancora possibile effettuare l'iscrizione e si può completare un processo di setup più avanzato, è possibile registrare una nuova sottoscrizione di prova di Office 365 e utilizzare tale indirizzo e-mail per effettuare l'iscrizione.|


## <a name="see-also"></a>Vedi anche
[Benvenuto in Dynamics NAV](across-get-started.md)  
[Utilizzare Dynamics NAV](ui-work-product.md)




