---
title: 'Procedura: Creare i record di documenti in entrata'
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
ms.openlocfilehash: e91c4570ff60d991974ac6afd16ba3bc3e73e44f
ms.contentlocale: it-it
ms.lasthandoff: 07/19/2017

---

# <a name="how-to-create-incoming-document-records"></a><span data-ttu-id="5e561-102">Procedura: Creare i record di documenti in entrata</span><span class="sxs-lookup"><span data-stu-id="5e561-102">How to: Create Incoming Document Records</span></span>
<span data-ttu-id="5e561-103">Nella finestra **Documenti in entrata** è possibile utilizzare diverse funzioni per esaminare le ricevute relative alle spese, gestire le attività OCR e convertire i file dei documenti in entrata, manualmente o automaticamente, nei relativi documenti o in righe di registrazione.</span><span class="sxs-lookup"><span data-stu-id="5e561-103">In the **Incoming Documents** window, you can use different functions to review expense receipts, manage OCR tasks, and convert incoming document files, manually or automatically, to the relevant documents or journal lines.</span></span> <span data-ttu-id="5e561-104">I file esterni possono essere allegati in qualsiasi fase dell'elaborazione, ad esempio ai documenti registrati, nonché ai fornitori, clienti e movimenti di contabilità generale risultanti.</span><span class="sxs-lookup"><span data-stu-id="5e561-104">The external files can be attached at any process stage, including to posted documents and to the resulting vendor, customer, and general ledger entries.</span></span>

<span data-ttu-id="5e561-105">Per registrare un documento esterno in Dynamics NAV, è necessario prima creare o completare un record di documento in entrata.</span><span class="sxs-lookup"><span data-stu-id="5e561-105">To record an external document in Dynamics NAV, you must first create or complete an incoming document record.</span></span> <span data-ttu-id="5e561-106">Questa operazione può essere eseguita manualmente oppure scattando una foto del documento e quindi creando un record del documento in entrata con il file immagine allegato.</span><span class="sxs-lookup"><span data-stu-id="5e561-106">You can do this manually, or you can take a photo of the external document and then create the incoming document record with the image file attached.</span></span>

<span data-ttu-id="5e561-107">Per poter utilizzare la funzionalità Documenti in entrata, è necessario eseguire l'impostazione necessaria.</span><span class="sxs-lookup"><span data-stu-id="5e561-107">Before you can use the Incoming Documents feature, you must perform the required setup.</span></span> <span data-ttu-id="5e561-108">Per ulteriori informazioni, vedere [Procedura: Impostare Documenti in entrata](across-how-setup-income-documents.md).</span><span class="sxs-lookup"><span data-stu-id="5e561-108">For more information, see [How to: Set Up Incoming Documents](across-how-setup-income-documents.md).</span></span>

## <a name="to-approve-or-reject-an-incoming-document"></a><span data-ttu-id="5e561-109">Per approvare o rifiutare un documento in entrata</span><span class="sxs-lookup"><span data-stu-id="5e561-109">To approve or reject an incoming document</span></span>
<span data-ttu-id="5e561-110">Se non si desidera consentire agli utenti di creare fatture o righe registrazioni COGE da record di documenti in entrata prima che vengano approvati, è possibile impostare dei responsabili che devono approvare i record prima che possano essere elaborati.</span><span class="sxs-lookup"><span data-stu-id="5e561-110">If you do want to allow users to create invoices or general journal lines from incoming document records unless they are approved, you can set up approvers who must approve the records before they can be processed.</span></span>

1. <span data-ttu-id="5e561-111">Nell'angolo superiore destro, scegliere l'icona **Cerca pagina o report**, immettere **Documenti in entrata**, quindi scegliere il collegamento correlato.</span><span class="sxs-lookup"><span data-stu-id="5e561-111">In the top right corner, choose the **Search for Page or Report** icon, enter **Incoming Documents**, and then choose the related link.</span></span>
2. <span data-ttu-id="5e561-112">Selezionare la riga con il documento che si desidera approvare o rifiutare quindi selezionare l'azione **Approva** o **Rifiuta**.</span><span class="sxs-lookup"><span data-stu-id="5e561-112">Select the line with the document that you want to approve or reject, and then choose the **Approve** or **Reject** actions.</span></span>

<span data-ttu-id="5e561-113">Se si approva il record del documento in entrata, la casella di controllo **Rilasciato** nella riga del documento in entrata è selezionata.</span><span class="sxs-lookup"><span data-stu-id="5e561-113">If you approve the incoming document record, the **Released** check box on the incoming document line is selected.</span></span> <span data-ttu-id="5e561-114">L'utente incaricato di creare, ad esempio, le fatture di acquisto può procedere all'elaborazione del record.</span><span class="sxs-lookup"><span data-stu-id="5e561-114">The user in charge of creating, for example, purchase invoices can proceed to process the record.</span></span>

## <a name="to-create-an-incoming-document-record-by-taking-a-photo"></a><span data-ttu-id="5e561-115">Per creare un record di documento in entrata facendo una foto</span><span class="sxs-lookup"><span data-stu-id="5e561-115">To create an incoming document record by taking a photo</span></span>
<span data-ttu-id="5e561-116">**Nota**: la seguente procedura si applica solo ai client di Dynamics NAV per tablet e telefono.</span><span class="sxs-lookup"><span data-stu-id="5e561-116">**Note**: The following procedure only applies to the Dynamics NAV Tablet and Phone clients.</span></span>

1. <span data-ttu-id="5e561-117">Sulla barra delle applicazioni, scegliere il riquadro **Crea documento in entrata da fotocamera** e andare al passaggio 4.</span><span class="sxs-lookup"><span data-stu-id="5e561-117">On the app bar, choose the **Create Incoming Document from Camera** tile, and then go to step 4.</span></span>
2. <span data-ttu-id="5e561-118">In alternativa, nella barra delle applicazioni, fare clic sul pulsante di opzione, selezionare **Documenti in entrata** e scegliere **Tutto**.</span><span class="sxs-lookup"><span data-stu-id="5e561-118">Alternatively, on the app bar, choose the options button, choose **Incoming Documents**, and then choose **All**.</span></span>
3. <span data-ttu-id="5e561-119">Nella finestra **Documenti in entrata** scegliere il pulsante con i puntini di sospensione e selezionare **Crea da fotocamera**.</span><span class="sxs-lookup"><span data-stu-id="5e561-119">In the **Incoming Documents** window, choose the ellipsis button, and then choose **Create from Camera**.</span></span> <span data-ttu-id="5e561-120">La fotocamera del tablet o del telefono è attivata.</span><span class="sxs-lookup"><span data-stu-id="5e561-120">The camera on the tablet or phone is activated.</span></span>
4. <span data-ttu-id="5e561-121">Scattare la foto di un documento, ad esempio una ricevuta di acquisto, che si desidera elaborare come documento in entrata e fare clic sul pulsante **OK**.</span><span class="sxs-lookup"><span data-stu-id="5e561-121">Take a photo of a document, such as a purchase receipt, that you want to process as an incoming document, and then choose the **OK** button.</span></span>

<span data-ttu-id="5e561-122">Viene creato un nuovo record di documento in entrata con l'immagine allegata.</span><span class="sxs-lookup"><span data-stu-id="5e561-122">A new incoming document record is created, with the image attached.</span></span>

## <a name="to-attach-an-image-to-an-incoming-document-record-by-taking-a-photo"></a><span data-ttu-id="5e561-123">Per allegare un'immagine a un record di documento in entrata facendo una foto</span><span class="sxs-lookup"><span data-stu-id="5e561-123">To attach an image to an incoming document record by taking a photo</span></span>
<span data-ttu-id="5e561-124">**Nota**: la seguente procedura si applica solo ai client di Dynamics NAV per tablet e telefono.</span><span class="sxs-lookup"><span data-stu-id="5e561-124">**Note**: The following procedure only applies to the Dynamics NAV Tablet and Phone clients.</span></span>

1. <span data-ttu-id="5e561-125">Nella barra delle applicazioni, fare clic sul pulsante di opzione, selezionare **Documenti in entrata** e scegliere **Tutto**.</span><span class="sxs-lookup"><span data-stu-id="5e561-125">On the app bar, choose the options button, choose **Incoming Documents**, and then choose **All**.</span></span>
2. <span data-ttu-id="5e561-126">Aprire la scheda di un record di documento in entrata esistente.</span><span class="sxs-lookup"><span data-stu-id="5e561-126">Open the card for an existing incoming document record.</span></span>
3. <span data-ttu-id="5e561-127">Nella finestra **Documento in entrata** scegliere il pulsante con i puntini di sospensione e selezionare **Allega immagine da fotocamera**.</span><span class="sxs-lookup"><span data-stu-id="5e561-127">In the **Incoming Document** window, choose the ellipsis button, and then choose **Attach Image from Camera**.</span></span> <span data-ttu-id="5e561-128">La fotocamera del tablet o del telefono è attivata.</span><span class="sxs-lookup"><span data-stu-id="5e561-128">The camera on the tablet or phone is activated.</span></span>
4. <span data-ttu-id="5e561-129">Scattare la foto di un documento, ad esempio una ricevuta di acquisto, che si desidera elaborare come documento in entrata e fare clic sul pulsante **OK**.</span><span class="sxs-lookup"><span data-stu-id="5e561-129">Take a photo of a document, such as a purchase receipt, that you want to process as an incoming document, and then choose the **OK** button.</span></span>

<span data-ttu-id="5e561-130">L'immagine viene allegata al record di documento in entrata.</span><span class="sxs-lookup"><span data-stu-id="5e561-130">The image is attached to the incoming document record.</span></span>

## <a name="to-create-an-incoming-document-record-manually"></a><span data-ttu-id="5e561-131">Per creare manualmente il record di un documento in entrata</span><span class="sxs-lookup"><span data-stu-id="5e561-131">To create an incoming document record manually</span></span>
1. <span data-ttu-id="5e561-132">Nell'angolo superiore destro, scegliere l'icona **Cerca pagina o report**, immettere **Documenti in entrata**, quindi scegliere il collegamento correlato.</span><span class="sxs-lookup"><span data-stu-id="5e561-132">In the top right corner, choose the **Search for Page or Report** icon, enter **Incoming Documents**, and then choose the related link.</span></span>
2. <span data-ttu-id="5e561-133">Selezionare l'azione **Crea da file**.</span><span class="sxs-lookup"><span data-stu-id="5e561-133">Choose the **Create from File** action.</span></span>  
3. <span data-ttu-id="5e561-134">Nella finestra **Inserisci file** selezionare un file e scegliere **Apri**.</span><span class="sxs-lookup"><span data-stu-id="5e561-134">In the **Insert File** window, select a file, and then choose **Open**.</span></span>

    <span data-ttu-id="5e561-135">Il file viene automaticamente allegato.</span><span class="sxs-lookup"><span data-stu-id="5e561-135">The file is automatically attached.</span></span>
4. <span data-ttu-id="5e561-136">In alternativa, selezionare l'azione **Nuovo**.</span><span class="sxs-lookup"><span data-stu-id="5e561-136">Alternatively, choose the **New** action.</span></span>
5. <span data-ttu-id="5e561-137">Per allegare un file, selezionare l'azione **Allega file**.</span><span class="sxs-lookup"><span data-stu-id="5e561-137">To attach a file, choose the **Attach File** action.</span></span>
6. <span data-ttu-id="5e561-138">Nella finestra **Inserisci file** selezionare il file che rappresenta il documento in entrata in questione, quindi scegliere il pulsante **Apri**.</span><span class="sxs-lookup"><span data-stu-id="5e561-138">In the **Insert File** window, select the file that represents the incoming document in question, and then choose the **Open** button.</span></span>
7. <span data-ttu-id="5e561-139">Nella finestra **Documento in entrata** compilare i campi secondo le proprie necessità.</span><span class="sxs-lookup"><span data-stu-id="5e561-139">In the **Incoming Document** window, fill in the fields as necessary.</span></span> <span data-ttu-id="5e561-140">Selezionare il campo per visualizzare una breve descrizione del campo o il collegamento a ulteriori informazioni.</span><span class="sxs-lookup"><span data-stu-id="5e561-140">Choose a field to read a short description of the field or link to more information.</span></span>

##<a name="see-also"></a><span data-ttu-id="5e561-141">Vedi anche</span><span class="sxs-lookup"><span data-stu-id="5e561-141">See Also</span></span>  
[<span data-ttu-id="5e561-142">Elaborare i documenti in entrata</span><span class="sxs-lookup"><span data-stu-id="5e561-142">Process Incoming Documents</span></span>](across-process-income-documents.md)  
[<span data-ttu-id="5e561-143">Documenti in entrata</span><span class="sxs-lookup"><span data-stu-id="5e561-143">Incoming Documents</span></span>](across-income-documents.md)  
[<span data-ttu-id="5e561-144">Gestire gli acquisti</span><span class="sxs-lookup"><span data-stu-id="5e561-144">Manage Purchasing</span></span>](purchasing-manage-purchasing.md)  
[<span data-ttu-id="5e561-145">Utilizzare Dynamics NAV</span><span class="sxs-lookup"><span data-stu-id="5e561-145">Work With Dynamics NAV</span></span>](ui-work-product.md)

