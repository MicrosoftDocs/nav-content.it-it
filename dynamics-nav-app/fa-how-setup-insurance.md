---
title: 'Procedura: Impostare l''assicurazione cespiti'
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
ms.openlocfilehash: 44bb5f20702a01d9fbbc025889ec2bc3191813be
ms.contentlocale: it-it
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-set-up-fixed-asset-insurance"></a>Procedura: Impostare l'assicurazione cespiti
Per gestire la copertura assicurativa del cespite, è prima necessario impostare alcune informazioni generali sull'assicurazione e una scheda assicurazione per ogni polizza.

## <a name="to-set-up-general-insurance-information"></a>Per impostare le informazioni generali delle assicurazioni  
Per utilizzare le funzionalità dell'assicurazione in Dynamics NAV, occorre impostare alcune informazioni generali sull'assicurazione.  
1. Nell'angolo superiore destro, scegliere l'icona **Cerca pagina o report**, immettere **Setup cespiti**, quindi scegliere il collegamento correlato.  
2. Compilare i campi, se necessario. Selezionare il campo per visualizzare una breve descrizione del campo o il collegamento a ulteriori informazioni.  

## <a name="to-set-up-insurance-types"></a>Per impostare i tipi di assicurazione  
È possibile raggruppare le polizze assicurative in categorie, ad esempio assicurazione da furti o incendi. I tipi di assicurazione vengono utilizzati nella Scheda Assicurazione.
1. Nell'angolo superiore destro, scegliere l'icona **Cerca pagina o report**, immettere **Tipi di assicurazione**, quindi scegliere il collegamento correlato.  
2. Compilare i campi, se necessario.

## <a name="to-set-up-insurance-cards"></a>Per impostare le schede assicurazione  
È possibile raggruppare informazioni relative ad ogni polizza assicurativa nella scheda di assicurazione.  
1. Nell'angolo superiore destro, scegliere l'icona **Cerca pagina o report**, immettere **Assicurazione**, quindi scegliere il collegamento correlato.  
2. Scegliere l'azione **Nuovo** nella finestra **Assicurazione** per creare una nuova scheda per l'assicurazione.  
3. Compilare i campi, se necessario.

## <a name="to-set-up-insurance-journal-templates"></a>Per impostare le definizioni registrazioni assicurazioni  
Una definizione delle registrazioni assicurazioni viene creata automaticamente la prima volta che in Dynamics NAV si apre la finestra **Registrazioni assicurazioni**. È tuttavia possibile impostare definizioni delle registrazioni aggiuntive. Per ulteriori informazioni, vedere [Elaborazione delle registrazioni COGE](ui-work-general-journals.md).  
1. Nell'angolo superiore destro, scegliere l'icona **Cerca pagina o report**, immettere **Def. reg. assicurazioni**, quindi scegliere il collegamento correlato.  
2. Compilare i campi, se necessario.

## <a name="to-set-up-insurance-journal-batches"></a>Per impostare i batch registrazioni assicurazioni  
I batch possono essere impostati in una definizione registrazioni assicurazioni. I valori nel batch delle registrazioni vengono utilizzati come valori di default nel caso in cui i campi nelle righe delle registrazioni non siano compilati. Per ulteriori informazioni, vedere [Elaborazione delle registrazioni COGE](ui-work-general-journals.md)  
1. Nell'angolo superiore destro, scegliere l'icona **Cerca pagina o report**, immettere **Def. reg. assicurazioni**, quindi scegliere il collegamento correlato.  
2. Selezionare una definizione registrazioni assicurazione e quindi scegliere l'azione **Batch**.
3. Nella finestra **Batch registrazioni assicurazioni** compilare i campi in base alle esigenze.

**NOTA**: i numeri hanno una funzione speciale nei nomi delle registrazioni. Se il nome definizione registrazioni o un nome batch registrazioni contiene un numero, quest'ultimo viene automaticamente incrementato di una unità ogni volta che le registrazioni vengono contabilizzate. Se ad esempio si immette HH1 nel campo **Nome**, il nome della registrazione verrà modificato in HH2 dopo la contabilizzazione della registrazione denominata HH1.

## <a name="see-also"></a>Vedi anche
[Impostazione cespiti](fa-setup.md)  
[Gestione di cespiti](fa-manage.md)  
[Contabilità](finance-setup.md)  
[Benvenuto in Dynamics NAV](across-get-started.md)

