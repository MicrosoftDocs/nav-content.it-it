---
title: Come esportare e importare workflow
description: "Per trasferire i workflow ad altri database di [!INCLUDE[d365fin](includes/d365fin_md.md)], ad esempio per risparmiare tempo durante la creazione di nuovi workflow, è possibile esportare e importare i workflow."
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
ms.openlocfilehash: 7ce7c6bd83efaacaed53f5d5ca5c2eb1521c0e6e
ms.contentlocale: it-it
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-export-and-import-workflows"></a><span data-ttu-id="596fb-103">Procedura: Esportare e importare workflow</span><span class="sxs-lookup"><span data-stu-id="596fb-103">How to: Export and Import Workflows</span></span>
<span data-ttu-id="596fb-104">Per trasferire i workflow ad altri database di [!INCLUDE[d365fin](includes/d365fin_md.md)], ad esempio per risparmiare tempo durante la creazione di nuovi workflow, è possibile esportare e importare i workflow.</span><span class="sxs-lookup"><span data-stu-id="596fb-104">To transfer workflows to other [!INCLUDE[d365fin](includes/d365fin_md.md)] databases, for example to save time when creating new workflows, you can export and import workflows.</span></span>  

 <span data-ttu-id="596fb-105">Un altro modo per creare rapidamente i flussi di lavoro prevede la creazione dei flussi di lavoro dai modelli di flusso di lavoro.</span><span class="sxs-lookup"><span data-stu-id="596fb-105">Another way to quickly create workflows is to create workflows from workflow templates.</span></span> <span data-ttu-id="596fb-106">Per ulteriori informazioni, vedere [Procedura: Creare workflow da modelli di workflow](across-how-to-create-workflows-from-workflow-templates.md).</span><span class="sxs-lookup"><span data-stu-id="596fb-106">For more information, see [How to: Create Workflows from Workflow Templates](across-how-to-create-workflows-from-workflow-templates.md).</span></span>  

 <span data-ttu-id="596fb-107">Nella finestra **Workflow** creare un workflow elencando le fasi interessate nelle righe.</span><span class="sxs-lookup"><span data-stu-id="596fb-107">In the **Workflow** window, you create a workflow by listing the involved steps on the lines.</span></span> <span data-ttu-id="596fb-108">Ogni fase consiste in un evento del flusso di lavoro, moderato dalle condizioni di evento, e in una risposta del flusso di lavoro, moderata dalle opzioni di risposta.</span><span class="sxs-lookup"><span data-stu-id="596fb-108">Each step consists of a workflow event, moderated by event conditions, and a workflow response, moderated by response options.</span></span> <span data-ttu-id="596fb-109">È possibile definire le fasi workflow compilando i campi delle righe del workflow in base a elenchi fissi di valori di evento e di risposta che rappresentano gli scenari supportati dal codice dell'applicazione.</span><span class="sxs-lookup"><span data-stu-id="596fb-109">You define workflow steps by filling fields on workflow lines from fixed lists of event and response values representing scenarios that are supported by the application code.</span></span> <span data-ttu-id="596fb-110">Per ulteriori informazioni, vedere [Procedura: Creare workflow](across-how-to-create-workflows.md).</span><span class="sxs-lookup"><span data-stu-id="596fb-110">For more information, see [How to: Create Workflows](across-how-to-create-workflows.md).</span></span>  

## <a name="to-export-a-workflow"></a><span data-ttu-id="596fb-111">Per esportare un flusso di lavoro</span><span class="sxs-lookup"><span data-stu-id="596fb-111">To export a workflow</span></span>  
1.  <span data-ttu-id="596fb-112">Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **Workflow** e quindi scegliere il collegamento correlato.</span><span class="sxs-lookup"><span data-stu-id="596fb-112">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Workflows**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="596fb-113">Selezionare un workflow e scegliere l'azione **Esporta in file**.</span><span class="sxs-lookup"><span data-stu-id="596fb-113">Select a workflow, and then choose the **Export to File** action.</span></span>  
3.  <span data-ttu-id="596fb-114">Nella finestra **Esporta file** fare clic sul pulsante **Salva**.</span><span class="sxs-lookup"><span data-stu-id="596fb-114">In the **Export File** window, choose the **Save** button.</span></span>  
4.  <span data-ttu-id="596fb-115">Nella finestra **Esporta** selezionare un percorso per il file e scegliere il pulsante **Salva**.</span><span class="sxs-lookup"><span data-stu-id="596fb-115">In the **Export** window, select a file location, and then choose the **Save** button.</span></span>  

## <a name="to-import-a-workflow"></a><span data-ttu-id="596fb-116">Per importare un flusso di lavoro</span><span class="sxs-lookup"><span data-stu-id="596fb-116">To import a workflow</span></span>  
1.  <span data-ttu-id="596fb-117">Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **Workflow** e quindi scegliere il collegamento correlato.</span><span class="sxs-lookup"><span data-stu-id="596fb-117">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Workflows**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="596fb-118">Selezionare l'azione **Importa da file**.</span><span class="sxs-lookup"><span data-stu-id="596fb-118">Choose the **Import from File** action.</span></span>  
3.  <span data-ttu-id="596fb-119">Nella finestra **Importa** selezionare il file XML contenente il flusso di lavoro e quindi scegliere il pulsante **Apri**.</span><span class="sxs-lookup"><span data-stu-id="596fb-119">In the **Import** window, choose the XML file that contains the workflow, and then choose the **Open** button.</span></span>  

> [!CAUTION]  
>  <span data-ttu-id="596fb-120">Se il codice del flusso di lavoro è già esistente nel database, i passaggi del flusso di lavoro verranno sovrascritti dai passaggi il flusso di lavoro importato.</span><span class="sxs-lookup"><span data-stu-id="596fb-120">If the workflow code already exists in the database, the workflow steps will be overwritten with the steps in the imported workflow.</span></span>  

## <a name="see-also"></a><span data-ttu-id="596fb-121">Vedi anche</span><span class="sxs-lookup"><span data-stu-id="596fb-121">See Also</span></span>  
 <span data-ttu-id="596fb-122">[Procedura: Creare workflow](across-how-to-create-workflows.md) </span><span class="sxs-lookup"><span data-stu-id="596fb-122">[How to: Create Workflows](across-how-to-create-workflows.md) </span></span>  
 <span data-ttu-id="596fb-123">[Procedura: Creare workflow da modelli di workflow](across-how-to-create-workflows-from-workflow-templates.md) </span><span class="sxs-lookup"><span data-stu-id="596fb-123">[How to: Create Workflows from Workflow Templates](across-how-to-create-workflows-from-workflow-templates.md) </span></span>  
 <span data-ttu-id="596fb-124">[Procedura: Visualizzare le istanze di fasi workflow archiviate](across-how-to-view-archived-workflow-step-instances.md) </span><span class="sxs-lookup"><span data-stu-id="596fb-124">[How to: View Archived Workflow Step Instances](across-how-to-view-archived-workflow-step-instances.md) </span></span>  
 <span data-ttu-id="596fb-125">[Procedura: Eliminare i workflow](across-how-to-delete-workflows.md) </span><span class="sxs-lookup"><span data-stu-id="596fb-125">[How to: Delete Workflows](across-how-to-delete-workflows.md) </span></span>  
 <span data-ttu-id="596fb-126">[Procedura dettagliata: Impostazione e utilizzo di un workflow di approvazione di acquisto](walkthrough-setting-up-and-using-a-purchase-approval-workflow.md) </span><span class="sxs-lookup"><span data-stu-id="596fb-126">[Walkthrough: Setting Up and Using a Purchase Approval Workflow](walkthrough-setting-up-and-using-a-purchase-approval-workflow.md) </span></span>  
 <span data-ttu-id="596fb-127">[Impostazione dei workflow](across-set-up-workflows.md) </span><span class="sxs-lookup"><span data-stu-id="596fb-127">[Setting Up Workflows](across-set-up-workflows.md) </span></span>  
 <span data-ttu-id="596fb-128">[Utilizzo dei workflow](across-use-workflows.md) </span><span class="sxs-lookup"><span data-stu-id="596fb-128">[Using Workflows](across-use-workflows.md) </span></span>  
 [<span data-ttu-id="596fb-129">Workflow</span><span class="sxs-lookup"><span data-stu-id="596fb-129">Workflow</span></span>](across-workflow.md)   
