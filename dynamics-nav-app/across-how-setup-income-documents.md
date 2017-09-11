---
title: 'Procedura: Impostare documenti in entrata'
author: SorenGP
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 6b60b1344a1e18ad91863046110df880f75f7c04
ms.openlocfilehash: d55329b571e4c59d4821a86a39362ea58480b86a
ms.contentlocale: it-it
ms.lasthandoff: 07/19/2017

---

# <a name="how-to-set-up-incoming-documents"></a><span data-ttu-id="877aa-102">Procedura: Impostare documenti in entrata</span><span class="sxs-lookup"><span data-stu-id="877aa-102">How to: Set Up Incoming Documents</span></span>
<span data-ttu-id="877aa-103">Se si creano righe registrazioni COGE da record di documenti in entrata, è necessario specificare nella finestra **Setup documenti in entrata** quale definizione registrazioni e quale batch contabile utilizzare.</span><span class="sxs-lookup"><span data-stu-id="877aa-103">If you create general journal lines from incoming document records, you must specify in the **Incoming Documents Setup** window which journal template and batch to use.</span></span>

<span data-ttu-id="877aa-104">Se non si desidera che gli utenti creino fatture o righe registrazioni COGE dai record di documenti in entrata prima che i documenti siano approvati, è necessario impostare i responsabili dell'approvazione nella finestra **Responsabili approvazione documenti in entrata**.</span><span class="sxs-lookup"><span data-stu-id="877aa-104">If you do not want users to create invoices or general journal lines from incoming document records unless the documents are first approved, you must set up approvers in the **Incoming Document Approvers** window.</span></span>

<span data-ttu-id="877aa-105">Per trasformare file PDF e file di immagine in documenti elettronici convertibili, ad esempio, in fatture di acquisto in Dynamics NAV, è necessario innanzitutto impostare la funzionalità OCR e abilitare il servizio.</span><span class="sxs-lookup"><span data-stu-id="877aa-105">To turn PDF and image files into electronic documents that you can convert to, for example, purchase invoices inside Dynamics NAV, you must first set up the OCR feature and enable the service.</span></span>

<span data-ttu-id="877aa-106">Se la funzionalità Documenti in entrata è impostata, è possibile utilizzare diverse funzioni per esaminare le ricevute relative alle spese, gestire le attività OCR e convertire i file dei documenti in entrata, manualmente o automaticamente, nei relativi documenti o in righe di registrazione.</span><span class="sxs-lookup"><span data-stu-id="877aa-106">When the Incoming Documents feature is set up, you can use different functions to review expense receipts, manage OCR tasks, and convert incoming document files, manually or automatically, to the relevant documents or journal lines.</span></span> <span data-ttu-id="877aa-107">I file esterni possono essere allegati in qualsiasi fase dell'elaborazione, ad esempio ai documenti registrati, nonché ai fornitori, clienti e movimenti di contabilità generale risultanti.</span><span class="sxs-lookup"><span data-stu-id="877aa-107">The external files can be attached at any process stage, including to posted documents and to the resulting vendor, customer, and general ledger entries.</span></span> <span data-ttu-id="877aa-108">Per ulteriori informazioni, vedere [Procedura: Elaborare i documenti in entrata](across-process-income-documents.md).</span><span class="sxs-lookup"><span data-stu-id="877aa-108">For more information, see [How to: Process Incoming Documents](across-process-income-documents.md).</span></span>

## <a name="to-set-up-the-incoming-documents-feature"></a><span data-ttu-id="877aa-109">Per impostare la funzione Documenti in entrata</span><span class="sxs-lookup"><span data-stu-id="877aa-109">To set up the Incoming Documents feature</span></span>
1. <span data-ttu-id="877aa-110">Nell'angolo superiore destro, scegliere l'icona **Cerca pagina o report**, immettere **Setup documenti in entrata**, quindi scegliere il collegamento correlato.</span><span class="sxs-lookup"><span data-stu-id="877aa-110">In the top right corner, choose the **Search for Page or Report** icon, enter **Incoming Document Setup**, and then choose the related link.</span></span>
2. <span data-ttu-id="877aa-111">Compilare i campi, se necessario.</span><span class="sxs-lookup"><span data-stu-id="877aa-111">Fill in the fields as necessary.</span></span> <span data-ttu-id="877aa-112">Selezionare il campo per visualizzare una breve descrizione del campo o il collegamento a ulteriori informazioni.</span><span class="sxs-lookup"><span data-stu-id="877aa-112">Choose a field to read a short description of the field or link to more information.</span></span>

## <a name="to-set-up-approvers-of-incoming-document-records"></a><span data-ttu-id="877aa-113">Per impostare i responsabili dell'approvazione dei record di documenti in entrata</span><span class="sxs-lookup"><span data-stu-id="877aa-113">To set up approvers of incoming document records</span></span>
1. <span data-ttu-id="877aa-114">Nell'angolo superiore destro, scegliere l'icona **Cerca pagina o report**, immettere **Setup documenti in entrata**, quindi scegliere il collegamento correlato.</span><span class="sxs-lookup"><span data-stu-id="877aa-114">In the top right corner, choose the **Search for Page or Report** icon, enter **Incoming Document Setup**, and then choose the related link.</span></span>  
2. <span data-ttu-id="877aa-115">In alternativa, nella finestra **Setup documenti in entrata** scegliere l'azione **Responsabili approvazione**.</span><span class="sxs-lookup"><span data-stu-id="877aa-115">In the **Incoming Documents Setup** window, choose the **Approvers** action.</span></span>

    <span data-ttu-id="877aa-116">Nella finestra **Responsabili approvazione documenti in entrata** vengono elencati tutti gli utenti impostati in Dynamics NAV.</span><span class="sxs-lookup"><span data-stu-id="877aa-116">The **Incoming Document Approvers** window shows all users that are set up in your Dynamics NAV .</span></span>  
3. <span data-ttu-id="877aa-117">Selezionare uno o più utenti che possono approvare un documento in entrata prima che possa essere creato un documento o una riga registrazioni correlata.</span><span class="sxs-lookup"><span data-stu-id="877aa-117">Select one or more users that can approve an incoming document before a related document or journal line can be created.</span></span>

<span data-ttu-id="877aa-118">Se vengono impostati i responsabili dell'approvazione nella finestra **Responsabile approvazione documento in entrata** solo questi utenti possono approvare un documento in entrata se la casella di controllo **Richiedi approvazione per creare** nella finestra **Setup documenti in entrata** è selezionata.</span><span class="sxs-lookup"><span data-stu-id="877aa-118">When approvers have been set up in the **Incoming Document Approvers** window, only those users can approve an incoming document if the **Require Approval To Create** check box in the **Incoming Documents Setup** window is selected.</span></span>

<span data-ttu-id="877aa-119">**Nota**: Questa impostazione di approvazione non è correlata ai workflow di approvazione.</span><span class="sxs-lookup"><span data-stu-id="877aa-119">**Note**: This approval setup is not related to approval workflows.</span></span> <span data-ttu-id="877aa-120">Per ulteriori informazioni, vedere [Procedura: Utilizzo dei workflow di approvazione](across-how-use-approval-workflows.md).</span><span class="sxs-lookup"><span data-stu-id="877aa-120">For more information, see [How to: Use Approval Workflows](across-how-use-approval-workflows.md).</span></span>

## <a name="to-set-up-an-ocr-service"></a><span data-ttu-id="877aa-121">Per impostare un servizio OCR</span><span class="sxs-lookup"><span data-stu-id="877aa-121">To set up an OCR service</span></span>
1. <span data-ttu-id="877aa-122">Nell'angolo superiore destro, scegliere l'icona **Cerca pagina o report**, immettere **Setup servizio OCR**, quindi scegliere il collegamento correlato.</span><span class="sxs-lookup"><span data-stu-id="877aa-122">In the top right corner, choose the **Search for Page or Report** icon, enter **OCR Service Setup**, and then choose the related link.</span></span>
2. <span data-ttu-id="877aa-123">Compilare i campi, se necessario.</span><span class="sxs-lookup"><span data-stu-id="877aa-123">Fill in the fields as necessary.</span></span> <span data-ttu-id="877aa-124">Selezionare il campo per visualizzare una breve descrizione del campo o il collegamento a ulteriori informazioni.</span><span class="sxs-lookup"><span data-stu-id="877aa-124">Choose a field to read a short description of the field or link to more information.</span></span>


## <a name="to-encrypt-your-login-information"></a><span data-ttu-id="877aa-125">Per crittografare le informazioni di accesso</span><span class="sxs-lookup"><span data-stu-id="877aa-125">To encrypt your login information</span></span>
<span data-ttu-id="877aa-126">Si consiglia di proteggere le informazioni di accesso immesse nella finestra **Setup servizio OCR**.</span><span class="sxs-lookup"><span data-stu-id="877aa-126">It is recommended that you protect the logon information that you enter in the **OCR Service Setup** window.</span></span> <span data-ttu-id="877aa-127">È possibile crittografare dati nel server generando nuove chiavi di crittografia o importando quelle esistenti che vengono abilitate nell'istanza del server che collega al database.</span><span class="sxs-lookup"><span data-stu-id="877aa-127">You can encrypt data on the server by generating new or importing existing encryption keys that you enable on the server instance that connects to the database.</span></span>

1. <span data-ttu-id="877aa-128">Nella finestra **Setup servizio OCR** scegliere l'azione **Gestione crittografia**.</span><span class="sxs-lookup"><span data-stu-id="877aa-128">In the **OCR Service Setup** window, choose the **Encryption Management** action.</span></span>
2. <span data-ttu-id="877aa-129">Nella finestra **Gestione crittografia dati** abilitare la crittografia dei dati.</span><span class="sxs-lookup"><span data-stu-id="877aa-129">In the **Data Encryption Management** window, enable encryption of your data.</span></span>

## <a name="see-also"></a><span data-ttu-id="877aa-130">Vedi anche</span><span class="sxs-lookup"><span data-stu-id="877aa-130">See Also</span></span>  
[<span data-ttu-id="877aa-131">Elaborare i documenti in entrata</span><span class="sxs-lookup"><span data-stu-id="877aa-131">Process Incoming Documents</span></span>](across-process-income-documents.md)  
[<span data-ttu-id="877aa-132">Documenti in entrata</span><span class="sxs-lookup"><span data-stu-id="877aa-132">Incoming Documents</span></span>](across-income-documents.md)  
[<span data-ttu-id="877aa-133">Gestire gli acquisti</span><span class="sxs-lookup"><span data-stu-id="877aa-133">Manage Purchasing</span></span>](purchasing-manage-purchasing.md)  
[<span data-ttu-id="877aa-134">Utilizzare Dynamics NAV</span><span class="sxs-lookup"><span data-stu-id="877aa-134">Work With Dynamics NAV</span></span>](ui-work-product.md)

