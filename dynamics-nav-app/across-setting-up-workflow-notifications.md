---
title: Impostazione delle notifiche del workflow
description: "Molte risposte workflow riguardano la comunicazione, a un utente, di un evento che si è verificato e la relativa necessità di intervento. Ad esempio, in un passaggio del flusso di lavoro, l'evento potrebbe essere che l'utente 1 richiede l'approvazione di un nuovo record e la risposta riguarda l'invio di una notifica all'utente 2, cioè il responsabile dell'approvazione. Nel passaggio successivo del flusso di lavoro, l'evento potrebbe essere che l'utente 2 approva il record e la risposta riguarda l'invio di una notifica all'utente 3 per iniziare un'elaborazione correlata del record approvato. Per le fasi del workflow che riguardano l'approvazione, ogni notifica è collegata a un movimento di approvazione."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 2c3e64a5d343bad026ba5417f18861ef6417dae3
ms.contentlocale: it-it
ms.lasthandoff: 10/16/2017

---
# <a name="setting-up-workflow-notifications"></a><span data-ttu-id="a22a3-106">Impostazione delle notifiche del workflow</span><span class="sxs-lookup"><span data-stu-id="a22a3-106">Setting Up Workflow Notifications</span></span>
<span data-ttu-id="a22a3-107">Molte risposte workflow riguardano la comunicazione, a un utente, di un evento che si è verificato e la relativa necessità di intervento.</span><span class="sxs-lookup"><span data-stu-id="a22a3-107">Many workflow responses are about notifying a user that an event has occurred that they must act on.</span></span> <span data-ttu-id="a22a3-108">Ad esempio, in un passaggio del flusso di lavoro, l'evento potrebbe essere che l'utente 1 richiede l'approvazione di un nuovo record e la risposta riguarda l'invio di una notifica all'utente 2, cioè il responsabile dell'approvazione.</span><span class="sxs-lookup"><span data-stu-id="a22a3-108">For example, on one workflow step, the event can be that User 1 requests approval of a new record, and the response is that a notification is sent to User 2, the approver.</span></span> <span data-ttu-id="a22a3-109">Nel passaggio successivo del flusso di lavoro, l'evento potrebbe essere che l'utente 2 approva il record e la risposta riguarda l'invio di una notifica all'utente 3 per iniziare un'elaborazione correlata del record approvato.</span><span class="sxs-lookup"><span data-stu-id="a22a3-109">On the next workflow step, the event can be that User 2 approves the record, and the response is that a notification is sent to User 3 to start a related processing of the approved record.</span></span> <span data-ttu-id="a22a3-110">Per le fasi del workflow che riguardano l'approvazione, ogni notifica è collegata a un movimento di approvazione.</span><span class="sxs-lookup"><span data-stu-id="a22a3-110">For workflow steps that are about approval, each notification is tied to an approval entry.</span></span> <span data-ttu-id="a22a3-111">Per ulteriori informazioni, vedere [Workflow](across-workflow.md).</span><span class="sxs-lookup"><span data-stu-id="a22a3-111">For more information, see [Workflow](across-workflow.md).</span></span>  

> [!NOTE]  
>  <span data-ttu-id="a22a3-112">La versione generica di [!INCLUDE[d365fin](includes/d365fin_md.md)] supporta le notifiche come messaggi e-mail e note interne.</span><span class="sxs-lookup"><span data-stu-id="a22a3-112">The generic version of [!INCLUDE[d365fin](includes/d365fin_md.md)] supports notifications as email and as internal notes.</span></span>  

> [!IMPORTANT]  
>  <span data-ttu-id="a22a3-113">Tutte le notifiche del flusso di lavoro vengono inviate tramite una coda processi.</span><span class="sxs-lookup"><span data-stu-id="a22a3-113">All workflow notifications are sent through a job queue.</span></span> <span data-ttu-id="a22a3-114">Assicurarsi che la coda processi sia presente nella soluzione.</span><span class="sxs-lookup"><span data-stu-id="a22a3-114">Make sure that the job queue in your solution.</span></span> <span data-ttu-id="a22a3-115">Per ulteriori informazioni, vedere [Utilizzare le code processi per pianificare i task](admin-job-queues-schedule-tasks.md).</span><span class="sxs-lookup"><span data-stu-id="a22a3-115">For more information, see [Use Job Queues to Schedule Tasks](admin-job-queues-schedule-tasks.md).</span></span>

<span data-ttu-id="a22a3-116">È possibile impostare diversi aspetti delle notifiche del flusso di lavoro nelle aree seguenti:</span><span class="sxs-lookup"><span data-stu-id="a22a3-116">You set up different aspects of workflow notifications in the following places:</span></span>  

1.  <span data-ttu-id="a22a3-117">Per i workflow di approvazione, è possibile impostare i destinatari delle notifiche del workflow compilando una riga nella finestra **Setup utente approvazione** per ogni utente che fa parte del workflow.</span><span class="sxs-lookup"><span data-stu-id="a22a3-117">For approval workflows, you set up the recipients of workflow notifications by filling a line in the **Approval User Setup** window for each user that takes part in the workflow.</span></span> <span data-ttu-id="a22a3-118">Ad esempio, se l'utente 2 è specificato nel campo **ID resp. approvazione** nella riga per l'utente 1, la notifica di richiesta dell'approvazione viene inviata all'utente 1.</span><span class="sxs-lookup"><span data-stu-id="a22a3-118">For example, if User 2 is specified in the **Approver ID** field on the line for User 1, then the approval request notification is sent to User 1.</span></span> <span data-ttu-id="a22a3-119">Per ulteriori informazioni, vedere [Procedura: Impostare utenti per l'approvazione](across-how-to-set-up-approval-users.md).</span><span class="sxs-lookup"><span data-stu-id="a22a3-119">For more information, see [How to: Set Up Approval Users](across-how-to-set-up-approval-users.md).</span></span>  
2.  <span data-ttu-id="a22a3-120">È possibile impostare il momento e la modalità di ricezione delle notifiche del workflow da parte degli utenti compilando la finestra **Programmazione notifica**  per ogni utente del workflow.</span><span class="sxs-lookup"><span data-stu-id="a22a3-120">You set when and how users receive workflow notifications by filling the **Notification Schedule** window for each workflow user.</span></span> <span data-ttu-id="a22a3-121">Per ulteriori informazioni, vedere [Procedura: Specificare come e quando ricevere le notifiche](across-how-to-specify-when-and-how-to-receive-notifications.md).</span><span class="sxs-lookup"><span data-stu-id="a22a3-121">For more information, see [How to: Specify When and How to Receive Notifications](across-how-to-specify-when-and-how-to-receive-notifications.md).</span></span>  
3.  <span data-ttu-id="a22a3-122">È possibile impostare il contenuto e il layout generali delle notifiche, incluse le notifiche relative alle risposte del workflow scadute, impostando i modelli di notifica nella finestra **Modelli di notifica**.</span><span class="sxs-lookup"><span data-stu-id="a22a3-122">You set up the general content and layout of notifications, including notifications about overdue workflow responses, by setting up notification templates in the **Notification Templates** window.</span></span> <span data-ttu-id="a22a3-123">È possibile utilizzare i modelli di default forniti con [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="a22a3-123">You can use the default templates provided with [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span>  
4.  <span data-ttu-id="a22a3-124">È possibile impostare le regole e il contenuto specifici della notifica di un flusso di lavoro durante la creazione del flusso di lavoro in questione.</span><span class="sxs-lookup"><span data-stu-id="a22a3-124">You set up specific content and rules of a workflow notification when you create the workflow in question.</span></span> <span data-ttu-id="a22a3-125">Questa operazione può essere eseguita selezionando le opzioni nella finestra **Opzioni di risposta workflow** per la risposta workflow che rappresenta la notifica.</span><span class="sxs-lookup"><span data-stu-id="a22a3-125">You do this by selecting options in the **Workflow Response Options** window for the workflow response that represents the notification.</span></span> <span data-ttu-id="a22a3-126">Per ulteriori informazioni, vedere il passaggio 9 in [Procedura: Creare workflow](across-how-to-create-workflows.md).</span><span class="sxs-lookup"><span data-stu-id="a22a3-126">For more information, see step 9 in [How to: Create Workflows](across-how-to-create-workflows.md).</span></span>  

## <a name="see-also"></a><span data-ttu-id="a22a3-127">Vedi anche</span><span class="sxs-lookup"><span data-stu-id="a22a3-127">See Also</span></span>  
 <span data-ttu-id="a22a3-128">[Procedura: Impostare gli utenti per l'approvazione](across-how-to-set-up-approval-users.md) </span><span class="sxs-lookup"><span data-stu-id="a22a3-128">[How to: Set Up Approval Users](across-how-to-set-up-approval-users.md) </span></span>  
 <span data-ttu-id="a22a3-129">[Procedura: Impostare gli utenti del workflow](across-how-to-set-up-workflow-users.md) </span><span class="sxs-lookup"><span data-stu-id="a22a3-129">[How to: Set Up Workflow Users](across-how-to-set-up-workflow-users.md) </span></span>  
 <span data-ttu-id="a22a3-130">[Procedura: Specificare come e quando ricevere le notifiche](across-how-to-specify-when-and-how-to-receive-notifications.md) </span><span class="sxs-lookup"><span data-stu-id="a22a3-130">[How to: Specify When and How to Receive Notifications](across-how-to-specify-when-and-how-to-receive-notifications.md) </span></span>  
 <span data-ttu-id="a22a3-131">[Procedura: Creare workflow](across-how-to-create-workflows.md) </span><span class="sxs-lookup"><span data-stu-id="a22a3-131">[How to: Create Workflows](across-how-to-create-workflows.md) </span></span>  
 <span data-ttu-id="a22a3-132">[Procedura: Gestire i modelli di notifica](across-how-to-manage-notification-templates.md) </span><span class="sxs-lookup"><span data-stu-id="a22a3-132">[How to: Manage Notification Templates](across-how-to-manage-notification-templates.md) </span></span>  
 <span data-ttu-id="a22a3-133">[Utilizzare le code processi per pianificare i task](admin-job-queues-schedule-tasks.md) </span><span class="sxs-lookup"><span data-stu-id="a22a3-133">[Use Job Queues to Schedule Tasks](admin-job-queues-schedule-tasks.md) </span></span>  
 <span data-ttu-id="a22a3-134">[Procedura: Impostare la posta elettronica](madeira-how-setup-email.md) </span><span class="sxs-lookup"><span data-stu-id="a22a3-134">[How to: Set up Email](madeira-how-setup-email.md) </span></span>  
 <span data-ttu-id="a22a3-135">[Procedura dettagliata: Impostazione e utilizzo di un workflow di approvazione di acquisto](walkthrough-setting-up-and-using-a-purchase-approval-workflow.md) </span><span class="sxs-lookup"><span data-stu-id="a22a3-135">[Walkthrough: Setting Up and Using a Purchase Approval Workflow](walkthrough-setting-up-and-using-a-purchase-approval-workflow.md) </span></span>  
 [<span data-ttu-id="a22a3-136">Workflow</span><span class="sxs-lookup"><span data-stu-id="a22a3-136">Workflow</span></span>](across-workflow.md)   
