---
title: Impostazione dei workflow
description: "È possibile impostare e utilizzare i workflow che collegano task di processi aziendali eseguiti da utenti diversi. I task di sistema, ad esempio la registrazione automatica, possono essere inclusi come passaggi nei flussi di lavoro e preceduti o seguiti da task degli utenti. La richiesta e la concessione dell'approvazione per creare nuovi record sono passaggi tipici del workflow."
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
ms.openlocfilehash: 060a402b54fa59110986907de2d6c64ba079db30
ms.contentlocale: it-it
ms.lasthandoff: 10/16/2017

---
# <a name="setting-up-workflows"></a><span data-ttu-id="07242-105">Impostazione dei workflow</span><span class="sxs-lookup"><span data-stu-id="07242-105">Setting Up Workflows</span></span>
<span data-ttu-id="07242-106">È possibile impostare e utilizzare i workflow che collegano task di processi aziendali eseguiti da utenti diversi.</span><span class="sxs-lookup"><span data-stu-id="07242-106">You can set up and use workflows that connect business-process tasks performed by different users.</span></span> <span data-ttu-id="07242-107">I task di sistema, ad esempio la registrazione automatica, possono essere inclusi come passaggi nei flussi di lavoro e preceduti o seguiti da task degli utenti.</span><span class="sxs-lookup"><span data-stu-id="07242-107">System tasks, such as automatic posting, can be included as steps in workflows, preceded or followed by user tasks.</span></span> <span data-ttu-id="07242-108">La richiesta e la concessione dell'approvazione per creare nuovi record sono passaggi tipici del workflow.</span><span class="sxs-lookup"><span data-stu-id="07242-108">Requesting and granting approval to create new records are typical workflow steps.</span></span> <span data-ttu-id="07242-109">Per ulteriori informazioni, vedere [Utilizzo dei workflow](across-use-workflows.md).</span><span class="sxs-lookup"><span data-stu-id="07242-109">For more information, see [Using Workflows](across-use-workflows.md).</span></span>  

 <span data-ttu-id="07242-110">Prima di poter iniziare a utilizzare i flussi di lavoro, è necessario impostare gli utenti del flusso di lavoro e gli utenti dell'approvazione, specificare la modalità di ricezione delle notifiche sui passaggi del flusso di lavoro e successivamente creare i flussi di lavoro, potenzialmente preceduti dalla personalizzazione del codice.</span><span class="sxs-lookup"><span data-stu-id="07242-110">Before you begin to use workflows, you must set up workflow users and approval users, specify how users receive notifications about workflow steps, and then create the workflows, potentially preceded by code customization.</span></span>  

 <span data-ttu-id="07242-111">Nella finestra **Workflow** creare un workflow elencando le fasi interessate nelle righe.</span><span class="sxs-lookup"><span data-stu-id="07242-111">In the **Workflow** window, you create a workflow by listing the involved steps on the lines.</span></span> <span data-ttu-id="07242-112">Ogni fase consiste in un evento del flusso di lavoro, moderato dalle condizioni di evento, e in una risposta del flusso di lavoro, moderata dalle opzioni di risposta.</span><span class="sxs-lookup"><span data-stu-id="07242-112">Each step consists of a workflow event, moderated by event conditions, and a workflow response, moderated by response options.</span></span> <span data-ttu-id="07242-113">È possibile definire le fasi workflow compilando i campi delle righe del workflow in base a elenchi fissi di valori di evento e di risposta che rappresentano gli scenari supportati dal codice dell'applicazione.</span><span class="sxs-lookup"><span data-stu-id="07242-113">You define workflow steps by filling fields on workflow lines from fixed lists of event and response values representing scenarios that are supported by the application code.</span></span>  

 <span data-ttu-id="07242-114">Se uno scenario aziendale richiede un evento o una risposta del flusso di lavoro non supportati, il partner Microsoft deve implementarli tramite la personalizzazione del codice dell'applicazione.</span><span class="sxs-lookup"><span data-stu-id="07242-114">If a business scenario requires a workflow event or response that is not supported, a Microsoft partner must implement them by customizing the application code.</span></span> <span data-ttu-id="07242-115">Per ulteriori informazioni, vedere [Procedura dettagliata: Implementazione di nuovi eventi e risposte workflow](https://msdn.microsoft.com/en-us/library/mt574349.aspx) su MSDN.</span><span class="sxs-lookup"><span data-stu-id="07242-115">For more information, see [Walkthrough: Implementing New Workflow Events and Responses](https://msdn.microsoft.com/en-us/library/mt574349.aspx) on MSDN.</span></span>

 <span data-ttu-id="07242-116">Nella tabella seguente viene descritta una sequenza di task, con collegamenti agli argomenti che li descrivono.</span><span class="sxs-lookup"><span data-stu-id="07242-116">The following table describes a sequence of tasks, with links to the topics that describe them.</span></span>  

|<span data-ttu-id="07242-117">**Per**</span><span class="sxs-lookup"><span data-stu-id="07242-117">**To**</span></span>|<span data-ttu-id="07242-118">**Vedere**</span><span class="sxs-lookup"><span data-stu-id="07242-118">**See**</span></span>|  
|------------|-------------|  
|<span data-ttu-id="07242-119">Impostare gli utenti e i gruppi di utenti del flusso di lavoro.</span><span class="sxs-lookup"><span data-stu-id="07242-119">Set up workflow users and user groups.</span></span>|[<span data-ttu-id="07242-120">Procedura: Impostare gli utenti del workflow</span><span class="sxs-lookup"><span data-stu-id="07242-120">How to: Set Up Workflow Users</span></span>](across-how-to-set-up-workflow-users.md)|  
|<span data-ttu-id="07242-121">Impostare gli utenti del flusso di lavoro che partecipano ai flussi di approvazione.</span><span class="sxs-lookup"><span data-stu-id="07242-121">Set up workflow users who take part in approval workflows.</span></span>|[<span data-ttu-id="07242-122">Procedura: Impostare gli utenti per l'approvazione</span><span class="sxs-lookup"><span data-stu-id="07242-122">How to: Set Up Approval Users</span></span>](across-how-to-set-up-approval-users.md)|  
|<span data-ttu-id="07242-123">Specificare in che modo gli utenti ricevono le notifiche dei passaggi del flusso di lavoro, incluse le richieste di approvazione.</span><span class="sxs-lookup"><span data-stu-id="07242-123">Specify how workflow users are notified of workflow steps, including approval requests.</span></span>|[<span data-ttu-id="07242-124">Impostazione delle notifiche del workflow</span><span class="sxs-lookup"><span data-stu-id="07242-124">Setting Up Workflow Notifications</span></span>](across-setting-up-workflow-notifications.md)|  
|<span data-ttu-id="07242-125">Specificare quando gli utenti ricevono le notifiche e se aggregare le notifiche in un unico periodo per ridurne il numero.</span><span class="sxs-lookup"><span data-stu-id="07242-125">Specify when users receive notifications and whether to aggregate notifications in a period to minimize the number of notifications.</span></span>|[<span data-ttu-id="07242-126">Procedura: Specificare come e quando ricevere le notifiche</span><span class="sxs-lookup"><span data-stu-id="07242-126">How to: Specify When and How to Receive Notifications</span></span>](across-how-to-specify-when-and-how-to-receive-notifications.md)|  
|<span data-ttu-id="07242-127">Impostare il layout e il contenuto generale di nuovi messaggi di notifica relativi al workflow o esportare, modificare e importare nuovamente i modelli esistenti.</span><span class="sxs-lookup"><span data-stu-id="07242-127">Set up the layout and general content of new workflow notifications emails, or export, modify, and reimport existing templates.</span></span>|[<span data-ttu-id="07242-128">Procedura: Gestire i modelli di notifica</span><span class="sxs-lookup"><span data-stu-id="07242-128">How to: Manage Notification Templates</span></span>](across-how-to-manage-notification-templates.md)|  
|<span data-ttu-id="07242-129">Impostare un server SMTP per consentire la comunicazione e-mail in entrata e in uscita di [!INCLUDE[d365fin](includes/d365fin_md.md)]</span><span class="sxs-lookup"><span data-stu-id="07242-129">Set up an SMTP server to enable email communication in and out of [!INCLUDE[d365fin](includes/d365fin_md.md)]</span></span>|[<span data-ttu-id="07242-130">Procedura: Impostare la posta elettronica</span><span class="sxs-lookup"><span data-stu-id="07242-130">How to: Set up Email</span></span>](madeira-how-setup-email.md)|
|<span data-ttu-id="07242-131">Specificare i diversi passaggi di un flusso di lavoro in base al collegamento tra gli eventi del flusso di lavoro e le risposte del flusso di lavoro.</span><span class="sxs-lookup"><span data-stu-id="07242-131">Specify the different steps of a workflow by connection workflow events with workflow responses.</span></span>|[<span data-ttu-id="07242-132">Procedura: Creare flussi di lavoro</span><span class="sxs-lookup"><span data-stu-id="07242-132">How to: Create Workflows</span></span>](across-how-to-create-workflows.md)|  
|<span data-ttu-id="07242-133">Usare i modelli di flussi di lavoro per creare nuovi flussi di lavoro.</span><span class="sxs-lookup"><span data-stu-id="07242-133">Use workflow templates to create new workflows.</span></span>|[<span data-ttu-id="07242-134">Procedura: Creare flussi di lavoro da modelli di flusso di lavoro</span><span class="sxs-lookup"><span data-stu-id="07242-134">How to: Create Workflows from Workflow Templates</span></span>](across-how-to-create-workflows-from-workflow-templates.md)|  
|<span data-ttu-id="07242-135">Condividere workflow con altri database [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="07242-135">Share workflows with other [!INCLUDE[d365fin](includes/d365fin_md.md)] databases.</span></span>|[<span data-ttu-id="07242-136">Procedura: Esportare e importare workflow</span><span class="sxs-lookup"><span data-stu-id="07242-136">How to: Export and Import Workflows</span></span>](across-how-to-export-and-import-workflows.md)|  
|<span data-ttu-id="07242-137">Come impostare un flusso di lavoro per approvare documenti di vendita seguendo una procedura end-to-end.</span><span class="sxs-lookup"><span data-stu-id="07242-137">Learn how to set up a workflow for approving sales documents by following an end-to-end procedure.</span></span>|[<span data-ttu-id="07242-138">Procedura dettagliata: Impostazione e utilizzo di un flusso di lavoro di approvazione di acquisto</span><span class="sxs-lookup"><span data-stu-id="07242-138">Walkthrough: Setting Up and Using a Purchase Approval Workflow</span></span>](walkthrough-setting-up-and-using-a-purchase-approval-workflow.md)|  
|<span data-ttu-id="07242-139">Aggiungere supporto per uno scenario aziendale che richiede nuovi eventi o risposte del flusso di lavoro personalizzando il codice dell'applicazione.</span><span class="sxs-lookup"><span data-stu-id="07242-139">Add support for a business scenario that requires new workflow events or responses by customizing the application code.</span></span>|<span data-ttu-id="07242-140">[Procedura dettagliata: Implementazione di nuovi eventi e risposte workflow](https://msdn.microsoft.com/en-us/library/mt574349.aspx) su MSDN.</span><span class="sxs-lookup"><span data-stu-id="07242-140">[Walkthrough: Implementing New Workflow Events and Responses](https://msdn.microsoft.com/en-us/library/mt574349.aspx) on MSDN.</span></span>|  

## <a name="see-also"></a><span data-ttu-id="07242-141">Vedi anche</span><span class="sxs-lookup"><span data-stu-id="07242-141">See Also</span></span>  
 <span data-ttu-id="07242-142">[Utilizzo dei workflow](across-use-workflows.md) </span><span class="sxs-lookup"><span data-stu-id="07242-142">[Using Workflows](across-use-workflows.md) </span></span>  
 <span data-ttu-id="07242-143">[Workflow](across-workflow.md) </span><span class="sxs-lookup"><span data-stu-id="07242-143">[Workflow](across-workflow.md) </span></span>  
 [<span data-ttu-id="07242-144">Procedura dettagliata: Impostazione e utilizzo di un flusso di lavoro di approvazione di acquisto</span><span class="sxs-lookup"><span data-stu-id="07242-144">Walkthrough: Setting Up and Using a Purchase Approval Workflow</span></span>](walkthrough-setting-up-and-using-a-purchase-approval-workflow.md)  
 [<span data-ttu-id="07242-145">Utilizzo di Dynamics NAV</span><span class="sxs-lookup"><span data-stu-id="07242-145">Working with Dynamics NAV</span></span>](ui-work-product.md)
