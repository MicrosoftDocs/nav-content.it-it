---
title: 'Procedura: Impostare documenti in entrata'
author: SorenGP
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: 2bce97c76876c86a576ec6a281a306a46881027c
ms.contentlocale: it-it
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-set-up-incoming-documents"></a>Procedura: Impostare documenti in entrata
Se si creano righe registrazioni COGE da record di documenti in entrata, è necessario specificare nella finestra **Setup documenti in entrata** quale definizione registrazioni e quale batch contabile utilizzare.

Se non si desidera che gli utenti creino fatture o righe registrazioni COGE dai record di documenti in entrata prima che i documenti siano approvati, è necessario impostare i responsabili dell'approvazione nella finestra **Responsabili approvazione documenti in entrata**.

Per trasformare file PDF e file di immagine in documenti elettronici convertibili, ad esempio, in fatture di acquisto in Dynamics NAV, è necessario innanzitutto impostare la funzionalità OCR e abilitare il servizio.

Se la funzionalità Documenti in entrata è impostata, è possibile utilizzare diverse funzioni per esaminare le ricevute relative alle spese, gestire le attività OCR e convertire i file dei documenti in entrata, manualmente o automaticamente, nei relativi documenti o in righe di registrazione. I file esterni possono essere allegati in qualsiasi fase dell'elaborazione, ad esempio ai documenti registrati, nonché ai fornitori, clienti e movimenti di contabilità generale risultanti. Per ulteriori informazioni, vedere [Procedura: Elaborare i documenti in entrata](across-process-income-documents.md).

## <a name="to-set-up-the-incoming-documents-feature"></a>Per impostare la funzione Documenti in entrata
1. Nell'angolo superiore destro, scegliere l'icona **Cerca pagina o report**, immettere **Setup documenti in entrata**, quindi scegliere il collegamento correlato.
2. Compilare i campi, se necessario. Selezionare il campo per visualizzare una breve descrizione del campo o il collegamento a ulteriori informazioni.

## <a name="to-set-up-approvers-of-incoming-document-records"></a>Per impostare i responsabili dell'approvazione dei record di documenti in entrata
1. Nell'angolo superiore destro, scegliere l'icona **Cerca pagina o report**, immettere **Setup documenti in entrata**, quindi scegliere il collegamento correlato.  
2. In alternativa, nella finestra **Setup documenti in entrata** scegliere l'azione **Responsabili approvazione**.

    Nella finestra **Responsabili approvazione documenti in entrata** vengono elencati tutti gli utenti impostati in Dynamics NAV.  
3. Selezionare uno o più utenti che possono approvare un documento in entrata prima che possa essere creato un documento o una riga registrazioni correlata.

Se vengono impostati i responsabili dell'approvazione nella finestra **Responsabile approvazione documento in entrata** solo questi utenti possono approvare un documento in entrata se la casella di controllo **Richiedi approvazione per creare** nella finestra **Setup documenti in entrata** è selezionata.

**Nota**: Questa impostazione di approvazione non è correlata ai workflow di approvazione. Per ulteriori informazioni, vedere [Procedura: Utilizzo dei workflow di approvazione](across-how-use-approval-workflows.md).

## <a name="to-set-up-an-ocr-service"></a>Per impostare un servizio OCR
1. Nell'angolo superiore destro, scegliere l'icona **Cerca pagina o report**, immettere **Setup servizio OCR**, quindi scegliere il collegamento correlato.
2. Compilare i campi, se necessario. Selezionare il campo per visualizzare una breve descrizione del campo o il collegamento a ulteriori informazioni.


## <a name="to-encrypt-your-login-information"></a>Per crittografare le informazioni di accesso
Si consiglia di proteggere le informazioni di accesso immesse nella finestra **Setup servizio OCR**. È possibile crittografare dati nel server generando nuove chiavi di crittografia o importando quelle esistenti che vengono abilitate nell'istanza del server che collega al database.

1. Nella finestra **Setup servizio OCR** scegliere l'azione **Gestione crittografia**.
2. Nella finestra **Gestione crittografia dati** abilitare la crittografia dei dati.

## <a name="see-also"></a>Vedi anche  
[Elaborare i documenti in entrata](across-process-income-documents.md)  
[Documenti in entrata](across-income-documents.md)  
[Gestire gli acquisti](purchasing-manage-purchasing.md)  
[Utilizzare Dynamics NAV](ui-work-product.md)

