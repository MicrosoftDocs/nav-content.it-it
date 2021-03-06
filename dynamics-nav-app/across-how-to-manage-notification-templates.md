---
title: Come gestire i modelli di notifica
description: "Le notifiche vengono inviate agli utenti del workflow per informarli sui passaggi che devono eseguire o sullo stato delle fasi del workflow. È possibile impostare gli utenti che ricevono la notifica e il momento in cui la ricevono configurando gli utenti di approvazione, la pianificazione della notifica agli utenti e le risposte del flusso di lavoro interessato per definire il destinatario della notifica. Per ulteriori informazioni, vedere [Impostazione delle notifiche del workflow](across-setting-up-workflow-notifications.md)."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: b9b1f062ee6009f34698ea2cf33bc25bdd5b11e4
ms.openlocfilehash: 4180eeabe2e81aabcfc54642e656fc8ef37157a7
ms.contentlocale: it-it
ms.lasthandoff: 10/23/2017

---
# <a name="how-to-manage-notification-templates"></a>Procedura: Gestire i modelli di notifica
Le notifiche vengono inviate agli utenti del workflow per informarli sui passaggi che devono eseguire o sullo stato delle fasi del workflow. È possibile impostare gli utenti che ricevono la notifica e il momento in cui la ricevono configurando gli utenti di approvazione, la pianificazione della notifica agli utenti e le risposte del workflow interessato per definire il destinatario della notifica. Per ulteriori informazioni, vedere [Impostazione delle notifiche del workflow](across-setting-up-workflow-notifications.md).  

 Le notifiche si basano sui modelli che ne definiscono il contenuto e il layout. Il contenuto di un modello di notifica può essere esportato, modificato e, successivamente, importato nello stesso modello di notifica o in uno nuovo. Questa funzionalità è descritta nelle procedure seguenti.  

 Nella versione generica di [!INCLUDE[d365fin](includes/d365fin_md.md)] sono inclusi tre modelli di notifica per informare sulle richieste di approvazione, sui nuovi record e sulle richieste di approvazione scadute. I tre modelli di notifica predefiniti supportano **E-mail** e **Nota** come metodo di notifica. Per visualizzare il contenuto dei tre modelli di notifica, vedere la sezione "Contenuto dei modelli di notifica" in questo argomento.

## <a name="to-create-a-new-notification-template"></a>Per creare un nuovo modello di notifica  
1.  Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **Modelli di notifica**, quindi scegliere il collegamento correlato.  
2.  Nella finestra **Modelli di notifica** scegliere l'azione **Nuovo**.  
3.  Compilare i campi come indicato nella tabella seguente.  

    |Campo|Description|  
    |---------------------------------|---------------------------------------|  
    |**Codice**|Identificare il modello di notifica.|  
    |**Description**|Descrivere il modello di notifica.|  
    |**Metodo di notifica**|Specificare se la notifica viene inviata come messaggio di posta elettronica o nota.|  
    |**Tipo**|Specificare il processo commerciale per cui sarà utilizzata la notifica.<br /><br /> Selezionare uno dei tipi seguenti:<br /><br /> -   **Approvazione** specifica che il modello è utilizzato per informare gli utenti durante i workflow di approvazione.<br />-   **Nuovo record** specifica che il modello viene utilizzato per notificare ai responsabili dell'approvazione il momento in cui un nuovo record, ad esempio una scheda cliente, deve essere approvato.<br />-   **Scaduto** specifica che il modello è utilizzato per notificare agli utenti le richieste di approvazione scadute.|  
    |**Default**|Specificare se il modello di notifica sarà utilizzato per impostazione predefinita.|  

## <a name="to-modify-a-notification-template"></a>Per modificare un modello di notifica  
1.  Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **Modelli di notifica**, quindi scegliere il collegamento correlato.  
2.  Nella finestra **Modelli di notifica** selezionare il modello di notifica che si desidera modificare.  
3.  Scegliere l'azione **Esporta contenuto modello**.  
4.  Nella finestra **Esporta file** scegliere il pulsante **Salva**, quindi denominare e salvare il file HTML in un percorso appropriato.  
5.  Fare clic con il pulsante destro del mouse sul file, scegliere **Apri con**, quindi scegliere il programma appropriato.  

    > [!NOTE]  
    >  Il contenuto dei modelli di notifica di tipo messaggio di posta elettronica è in formato HTML. Il contenuto dei modelli di notifica di tipo nota è in formato TXT.  
6.  Modificare il contenuto del modello di notifica aggiungendo, modificando o rimuovendo le variabili dei parametri per definire il contenuto desiderato, quindi salvarlo. Per ulteriori informazioni, vedere la sezione "Contenuto dei modelli di notifica".  

    Continuare a importare il contenuto modificato nello stesso modello di notifica o in uno nuovo.  
7.  Per modificare il modello di notifica esportato, nella finestra **Modelli di notifica** selezionare il modello scelto nel passaggio 2.  

    In alternativa, per importare il contenuto del modello modificato in un nuovo modello di notifica, attenersi alla procedura "Per creare un nuovo modello di notifica" e, successivamente, selezionare il nuovo modello di notifica.  
8.  Scegliere l'azione **Importa contenuto modello**.  
9. Se si sta modificando un modello di notifica esistente, scegliere il pulsante **Sì** nel messaggio relativo alla sovrascrittura del modello esistente.  
10. Nella finestra **Seleziona un file da importare** scegliere il file HTML modificato nel passaggio 6, quindi selezionare il pulsante **Apri**.  

Il modello di notifica nuovo o esistente nella finestra **Modelli di notifica** è ora aggiornato con il contenuto modificato.  

### <a name="content-of-the-notification-templates"></a>Contenuto dei modelli di notifica  
Nei tre tipi di modelli di notifica, **Nuovo record**, **Approvazione** e **Scaduto** sono presenti contenuti diversi.  

I valori dei parametri vengono inseriti automaticamente nelle notifiche in base al tipo del modello di notifica.  

#### <a name="new-record"></a>Nuovo record  
 ![NAV&#95;notification&#95;template&#95;new&#95;record&#95;type](media/nav_notification_template_new_record.png "NAV_notification_template_new_record")  

#### <a name="approval"></a>Approvazione  
 ![NAV&#95;notification&#95;template&#95;approval&#95;type](media/nav_notification_template_approval_type.png "NAV_notification_template_approval_type")  

#### <a name="overdue"></a>Scaduto  
 ![NAV&#95;notification&#95;overdue&#95;type](media/nav_notification_overdue_type.png "NAV_notification_overdue_type")  

## <a name="see-also"></a>Vedi anche  
 [Impostazione delle notifiche del workflow](across-setting-up-workflow-notifications.md)   
 [Procedura: Impostare la posta elettronica](madeira-how-setup-email.md)   
 [Procedura: Impostare gli utenti del workflow](across-how-to-set-up-workflow-users.md)   
 [Procedura: Impostare gli utenti per l'approvazione](across-how-to-set-up-approval-users.md)   
 [Procedura: Creare workflow](across-how-to-create-workflows.md)   
 [Utilizzare le code processi per pianificare i task](admin-job-queues-schedule-tasks.md)   
 [Workflow](across-workflow.md)   

