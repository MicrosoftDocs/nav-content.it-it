---
title: Impostare documenti in entrata
description: "Utilizzare la funzione Documenti in entrata per creare documenti elettronici, gestire le attività OCR, importare le fatture e convertire i file immagine."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: electronic document, e-invoice, incoming document, OCR, ecommerce, document exchange, import invoice
ms.date: 06/02/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 1dfba8b14019991c95f40ffd5f7fbaed5df414eb
ms.openlocfilehash: f973b85066f657d1bd932659f3a538a0e471c80d
ms.contentlocale: it-it
ms.lasthandoff: 12/01/2017

---
# <a name="how-to-set-up-incoming-documents"></a><span data-ttu-id="f3403-103">Procedura: Impostare documenti in entrata</span><span class="sxs-lookup"><span data-stu-id="f3403-103">How to: Set Up Incoming Documents</span></span>
<span data-ttu-id="f3403-104">Se si creano righe registrazioni COGE da record di documenti in entrata, è necessario specificare nella finestra **Setup documenti in entrata** quale definizione registrazioni e quale batch contabile utilizzare.</span><span class="sxs-lookup"><span data-stu-id="f3403-104">If you create general journal lines from incoming document records, you must specify in the **Incoming Documents Setup** window which journal template and batch to use.</span></span>

<span data-ttu-id="f3403-105">Se non si desidera che gli utenti creino fatture o righe registrazioni COGE dai record di documenti in entrata prima che i documenti siano approvati, è necessario impostare i responsabili dell'approvazione nella finestra **Responsabili approvazione documenti in entrata**.</span><span class="sxs-lookup"><span data-stu-id="f3403-105">If you do not want users to create invoices or general journal lines from incoming document records unless the documents are first approved, you must set up approvers in the **Incoming Document Approvers** window.</span></span>

<span data-ttu-id="f3403-106">Per trasformare file PDF e file di immagine in documenti elettronici convertibili, ad esempio, in fatture di acquisto [!INCLUDE[d365fin](includes/d365fin_md.md)]', è necessario innanzitutto impostare la funzionalità OCR e abilitare il servizio.</span><span class="sxs-lookup"><span data-stu-id="f3403-106">To turn PDF and image files into electronic documents that you can convert to, for example, purchase invoices inside [!INCLUDE[d365fin](includes/d365fin_md.md)], you must first set up the OCR feature and enable the service.</span></span>

<span data-ttu-id="f3403-107">Se la funzionalità Documenti in entrata è impostata, è possibile utilizzare diverse funzioni per esaminare le ricevute relative alle spese, gestire le attività OCR e convertire i file dei documenti in entrata, manualmente o automaticamente, nei relativi documenti o in righe di registrazione.</span><span class="sxs-lookup"><span data-stu-id="f3403-107">When the Incoming Documents feature is set up, you can use different functions to review expense receipts, manage OCR tasks, and convert incoming document files, manually or automatically, to the relevant documents or journal lines.</span></span> <span data-ttu-id="f3403-108">I file esterni possono essere allegati in qualsiasi fase dell'elaborazione, ad esempio ai documenti registrati, nonché ai fornitori, clienti e movimenti di contabilità generale risultanti.</span><span class="sxs-lookup"><span data-stu-id="f3403-108">The external files can be attached at any process stage, including to posted documents and to the resulting vendor, customer, and general ledger entries.</span></span> <span data-ttu-id="f3403-109">Per ulteriori informazioni, vedere [Elaborazione di documenti in entrata](across-process-income-documents.md).</span><span class="sxs-lookup"><span data-stu-id="f3403-109">For more information, see [Processing Incoming Documents](across-process-income-documents.md).</span></span>

## <a name="to-set-up-the-incoming-documents-feature"></a><span data-ttu-id="f3403-110">Per impostare la funzione Documenti in entrata</span><span class="sxs-lookup"><span data-stu-id="f3403-110">To set up the Incoming Documents feature</span></span>
1. <span data-ttu-id="f3403-111">Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **Setup documenti in entrata**, quindi scegliere il collegamento correlato.</span><span class="sxs-lookup"><span data-stu-id="f3403-111">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Incoming Document Setup**, and then choose the related link.</span></span>
2. <span data-ttu-id="f3403-112">Compilare i campi, se necessario.</span><span class="sxs-lookup"><span data-stu-id="f3403-112">Fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

## <a name="to-set-up-approvers-of-incoming-document-records"></a><span data-ttu-id="f3403-113">Per impostare i responsabili dell'approvazione dei record di documenti in entrata</span><span class="sxs-lookup"><span data-stu-id="f3403-113">To set up approvers of incoming document records</span></span>
1. <span data-ttu-id="f3403-114">Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **Setup documenti in entrata**, quindi scegliere il collegamento correlato.</span><span class="sxs-lookup"><span data-stu-id="f3403-114">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Incoming Document Setup**, and then choose the related link.</span></span>  
2. <span data-ttu-id="f3403-115">In alternativa, nella finestra **Setup documenti in entrata** scegliere l'azione **Responsabili approvazione**.</span><span class="sxs-lookup"><span data-stu-id="f3403-115">In the **Incoming Documents Setup** window, choose the **Approvers** action.</span></span>

    <span data-ttu-id="f3403-116">Nella finestra **Responsabili approvazione documenti in entrata** vengono elencati tutti gli utenti impostati in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="f3403-116">The **Incoming Document Approvers** window shows all users that are set up in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span>  
3. <span data-ttu-id="f3403-117">Selezionare uno o più utenti che possono approvare un documento in entrata prima che possa essere creato un documento o una riga registrazioni correlata.</span><span class="sxs-lookup"><span data-stu-id="f3403-117">Select one or more users that can approve an incoming document before a related document or journal line can be created.</span></span>

<span data-ttu-id="f3403-118">Se vengono impostati i responsabili dell'approvazione nella finestra **Responsabile approvazione documento in entrata** solo questi utenti possono approvare un documento in entrata se la casella di controllo **Richiedi approvazione per creare** nella finestra **Setup documenti in entrata** è selezionata.</span><span class="sxs-lookup"><span data-stu-id="f3403-118">When approvers have been set up in the **Incoming Document Approvers** window, only those users can approve an incoming document if the **Require Approval To Create** check box in the **Incoming Documents Setup** window is selected.</span></span>

> [!NOTE]  
>   <span data-ttu-id="f3403-119">Questa impostazione di approvazione non è correlata ai workflow di approvazione.</span><span class="sxs-lookup"><span data-stu-id="f3403-119">This approval setup is not related to approval workflows.</span></span> <span data-ttu-id="f3403-120">Per ulteriori informazioni, vedere [Procedura: Utilizzo dei workflow di approvazione](across-how-use-approval-workflows.md).</span><span class="sxs-lookup"><span data-stu-id="f3403-120">For more information, see [How to: Use Approval Workflows](across-how-use-approval-workflows.md).</span></span>

## <a name="to-set-up-an-ocr-service"></a><span data-ttu-id="f3403-121">Per impostare un servizio OCR</span><span class="sxs-lookup"><span data-stu-id="f3403-121">To set up an OCR service</span></span>
1. <span data-ttu-id="f3403-122">Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **Setup servizio OCR**, quindi scegliere il collegamento correlato.</span><span class="sxs-lookup"><span data-stu-id="f3403-122">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **OCR Service Setup**, and then choose the related link.</span></span>
2. <span data-ttu-id="f3403-123">Compilare i campi, se necessario.</span><span class="sxs-lookup"><span data-stu-id="f3403-123">Fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

## <a name="to-encrypt-your-login-information"></a><span data-ttu-id="f3403-124">Per crittografare le informazioni di accesso</span><span class="sxs-lookup"><span data-stu-id="f3403-124">To encrypt your login information</span></span>
<span data-ttu-id="f3403-125">Si consiglia di proteggere le informazioni di accesso immesse nella finestra **Setup servizio OCR**.</span><span class="sxs-lookup"><span data-stu-id="f3403-125">It is recommended that you protect the logon information that you enter in the **OCR Service Setup** window.</span></span> <span data-ttu-id="f3403-126">È possibile crittografare dati nel server generando nuove chiavi di crittografia o importando quelle esistenti che vengono abilitate nell'istanza del server che collega al database.</span><span class="sxs-lookup"><span data-stu-id="f3403-126">You can encrypt data on the server by generating new or importing existing encryption keys that you enable on the server instance that connects to the database.</span></span>

1. <span data-ttu-id="f3403-127">Nella finestra **Setup servizio OCR** scegliere l'azione **Gestione crittografia**.</span><span class="sxs-lookup"><span data-stu-id="f3403-127">In the **OCR Service Setup** window, choose the **Encryption Management** action.</span></span>
2. <span data-ttu-id="f3403-128">Nella finestra **Gestione crittografia dati** abilitare la crittografia dei dati.</span><span class="sxs-lookup"><span data-stu-id="f3403-128">In the **Data Encryption Management** window, enable encryption of your data.</span></span>

## <a name="see-also"></a><span data-ttu-id="f3403-129">Vedi anche</span><span class="sxs-lookup"><span data-stu-id="f3403-129">See Also</span></span>
[<span data-ttu-id="f3403-130">Elaborare i documenti in entrata</span><span class="sxs-lookup"><span data-stu-id="f3403-130">Process Incoming Documents</span></span>](across-process-income-documents.md)  
[<span data-ttu-id="f3403-131">Documenti in entrata</span><span class="sxs-lookup"><span data-stu-id="f3403-131">Incoming Documents</span></span>](across-income-documents.md)  
[<span data-ttu-id="f3403-132">Acquisti</span><span class="sxs-lookup"><span data-stu-id="f3403-132">Purchasing</span></span>](purchasing-manage-purchasing.md)  
<span data-ttu-id="f3403-133">[Utilizzo di [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="f3403-133">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

