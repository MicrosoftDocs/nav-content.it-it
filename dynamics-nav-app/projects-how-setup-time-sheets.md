---
title: 'Procedura: Impostare fogli presenze'
author: SorenGP
ms.custom: na
ms.date: 11/01/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: 6cbacce79ce185d6ed00ea8383259d1b28f9e11b
ms.contentlocale: it-it
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-set-up-time-sheets"></a>Procedura: Impostare fogli presenze
I fogli presenze di Dynamics NAV consentono di gestire la registrazione del tempo in incrementi settimanali di sette giorni. Questi fogli possono essere usati per tenere traccia del tempo utilizzato nelle commesse e per registrare la semplice registrazione del tempo risorsa. Prima di poter utilizzare i fogli presenze, è necessario specificare come si desidera impostarli e configurarli.

Dopo aver impostato la modalità con cui l'organizzazione utilizzerà i fogli presenze, è possibile specificare se e come approvarli. In base alle esigenze dell'organizzazione, è possibile indicare:

- Uno o più utenti come amministratore dei fogli presenze e come responsabile approvazione di tutti i fogli presenze.
- Un responsabile approvazione del foglio presenze di ogni risorsa.

Una volta impostati dei fogli presenze, è possibile creare fogli presenze per le risorse, assegnarli alle righe di pianificazione commessa e registrare le righe dei fogli presenze. Per ulteriori informazioni, vedere [Procedura: Utilizzare i fogli presenze](projects-how-use-time-sheets.md).

## <a name="to-set-up-general-information-for-time-sheets"></a>Per impostare le informazioni generali relative ai fogli presenze  

1. Nell'angolo superiore destro, scegliere l'icona **Cerca pagina o report**, immettere **Setup risorse**, quindi scegliere il collegamento correlato.  
2. Compilare i campi, se necessario. Selezionare il campo per visualizzare una breve descrizione del campo o il collegamento a ulteriori informazioni.
3. Per il campo **Foglio presenze per approvazione commesse** selezionare una delle opzioni indicate di seguito.

|Opzione |Descrizione|
|---|---|
|**Mai**|Il foglio presenze viene approvato dall'utente indicato nel campo **ID utente resp. approvazione foglio presenze** nella scheda risorsa.|
|**Sempre**|Il foglio presenze viene approvato dall'utente indicato nel campo **Persona responsabile** nella scheda commessa.|
|**Solo macchina**|Se il foglio presenze della macchina è collegato a una commessa, il foglio presenze viene approvato dall'utente indicato nel campo **Persona responsabile** della scheda commessa. Se il foglio presenze della macchina è collegato a una risorsa, il foglio presenze viene approvato dall'utente indicato nel campo **ID utente resp. approvazione foglio presenze** della scheda risorsa.

## <a name="to-assign-a-time-sheet-administrator"></a>Per assegnare un amministratore per il foglio presenze  

1. Nell'angolo superiore destro, scegliere l'icona **Cerca pagina o report**, immettere **Setup utente**, quindi scegliere il collegamento correlato.  
2.  Aggiungere un nuovo utente, se la lista degli utenti non include la persona che si desidera nominare come amministratore del foglio presenze. Per ulteriori informazioni, contattare l'amministratore.  
3. Selezionare un utente come amministratore del foglio presenze, quindi selezionare la casella di controllo **Amministratore foglio presenze** .  

**Suggerimento**: si consiglia di designare un solo utente come amministratore del foglio presenze di un'azienda. Nella procedura riportata di seguito, si impostano un proprietario e un responsabile approvazione del foglio presenze dove il responsabile approvazione è assegnato a ciascuna risorsa.  

## <a name="to-assign-a-time-sheets-owner-and-approver"></a>Per assegnare un proprietario e un responsabile approvazione dei fogli presenze  

1. Nell'angolo superiore destro, scegliere l'icona **Cerca pagina o report**, immettere **Risorse**, quindi scegliere il collegamento correlato.
2. Selezionare la risorsa per cui si desidera impostare la possibilità di utilizzare i fogli presenze, quindi selezionare la casella di controllo **Usa foglio presenze**.  
3. Nel campo **ID utente proprietario foglio presenze** immettere l'ID del proprietario del foglio presenze. Il proprietario può immettere l'utilizzo del tempo in un foglio presenze e inviarlo per l'approvazione. In generale quando la risorsa è una persona, è anche il proprietario.  
4. Nel campo **ID utente resp. approvazione foglio presenze** immettere l'ID del responsabile approvazione del foglio presenze. Il responsabile approvazione può approvare, rifiutare o riaprire un foglio presenze.  

**Nota**: non è possibile modificare l'ID del responsabile approvazione del foglio presenze se vi sono dei fogli presenze che non sono stati ancora elaborati e il cui stato è **Inviato** o **Aperto**.

## <a name="see-also"></a>Vedi anche
[Impostare Gestione progetti](projects-setup-projects.md)  
[Gestione di progetti](projects-manage-projects.md)  
[Contabilità](finance-setup.md)  
[Gestire gli acquisti](purchasing-manage-purchasing.md)         
[Gestire le vendite](sales-manage-sales.md)      
[Utilizzare Dynamics NAV](ui-work-product.md)  

