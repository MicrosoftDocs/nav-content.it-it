---
title: Esportare file Positive Pay
description: Assicurarsi che la banca compensi solo gli assegni e gli importi convalidati tramite l'esportazione di file Positive Pay che contengano informazioni sul fornitore e pagamento.
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: check, clearing
ms.date: 06/16/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: bf09817e318b5338da0358f829ea2ed1edde9d67
ms.contentlocale: it-it
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-export-a-positive-pay-file"></a><span data-ttu-id="58554-103">Procedura: Esportare un file Positive Pay</span><span class="sxs-lookup"><span data-stu-id="58554-103">How to: Export a Positive Pay file</span></span>
<span data-ttu-id="58554-104">Per assicurarsi che la banca compensi solo gli assegni e gli importi convalidati, è possibile esportare un file Positive Pay con informazioni su fornitore, numero di assegno e importo del pagamento da inviare alla banca per riferimento quando si elaborano i pagamenti.</span><span class="sxs-lookup"><span data-stu-id="58554-104">To make sure that your bank only clears validated checks and amounts, you can export a Positive Pay file that contains vendor information, check number, and payment amount, which you send to the bank for reference when you process payments.</span></span>

[!INCLUDE[d365fin](includes/d365fin_md.md)]<span data-ttu-id="58554-105"> è preconfigurato per supportare i file Positive Pay per Bank of America e City Bank.</span><span class="sxs-lookup"><span data-stu-id="58554-105"> is preconfigured to support Positive Pay files for Bank of America and City Bank.</span></span>

## <a name="to-set-up-a-bank-account-for-positive-pay"></a><span data-ttu-id="58554-106">Per impostare un conto bancario per i file Positive Pay</span><span class="sxs-lookup"><span data-stu-id="58554-106">To set up a bank account for Positive Pay</span></span>
1. <span data-ttu-id="58554-107">Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **C/C bancari**, quindi scegliere il collegamento correlato.</span><span class="sxs-lookup"><span data-stu-id="58554-107">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Bank Accounts**, and then choose the related link.</span></span>
2. <span data-ttu-id="58554-108">Aprire la scheda della banca per cui si desidera utilizzare il Positive Pay.</span><span class="sxs-lookup"><span data-stu-id="58554-108">Open the card for the bank that you want to use Positive Pay for.</span></span>
3. <span data-ttu-id="58554-109">Nel campo **Codice esportazione Positive Pay** immettere POSPAYBANK.</span><span class="sxs-lookup"><span data-stu-id="58554-109">In the **Positive Pay Export Code** field, enter POSPAYBANK.</span></span>
4. <span data-ttu-id="58554-110">Chiudere la finestra.</span><span class="sxs-lookup"><span data-stu-id="58554-110">Close the window.</span></span>

## <a name="to-export-a-positive-pay-file"></a><span data-ttu-id="58554-111">Per esportare un file Positive Pay</span><span class="sxs-lookup"><span data-stu-id="58554-111">To export a Positive Pay file</span></span>
1. <span data-ttu-id="58554-112">Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **C/C bancari**, quindi scegliere il collegamento correlato.</span><span class="sxs-lookup"><span data-stu-id="58554-112">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Bank Accounts**, and then choose the related link.</span></span>
2. <span data-ttu-id="58554-113">Selezionare il conto bancario per cui si desidera esportare un file Positive Pay.</span><span class="sxs-lookup"><span data-stu-id="58554-113">Select the bank account that you want to export a Positive Pay file for.</span></span>
3. <span data-ttu-id="58554-114">Scegliere l'opzione **Esportazione Positive Pay**.</span><span class="sxs-lookup"><span data-stu-id="58554-114">Choose **Positive Pay Export** action.</span></span>

    <span data-ttu-id="58554-115">Verrà visualizzata la finestra **Esportazione Positive Pay** che mostra i pagamenti che sono stati effettuati per il conto bancario dalla data dell'ultimo caricamento, come mostrato nei campi **Data ultimo caricamento** e **Data ultimo caricamento**.</span><span class="sxs-lookup"><span data-stu-id="58554-115">The **Positive Pay Export** window opens displaying payments that have been made for the bank account since the last upload date, as shown in the **Last Upload Date** and **Last Upload Time** fields.</span></span>
4. <span data-ttu-id="58554-116">Nel campo **Data limite caricamento** specificare una data prima della quale i pagamenti non sono inclusi nel file esportato.</span><span class="sxs-lookup"><span data-stu-id="58554-116">In the **Cutoff Upload Date** field, specify a date before which payments are not included in the exported file.</span></span>
5. <span data-ttu-id="58554-117">Scegliere l'azione **Esporta**.</span><span class="sxs-lookup"><span data-stu-id="58554-117">Choose the **Export** action.</span></span>
6. <span data-ttu-id="58554-118">Nella finestra **Esporta file** scegliere il pulsante **Salva**, quindi salvare il file in un percorso appropriato.</span><span class="sxs-lookup"><span data-stu-id="58554-118">In the **Export File** window, choose the **Save** button, and then save the file to a convenient location.</span></span>
7. <span data-ttu-id="58554-119">Caricare il file nel sito elettronico della banca.</span><span class="sxs-lookup"><span data-stu-id="58554-119">Upload the file to your electronic bank site.</span></span>
8. <span data-ttu-id="58554-120">Annotare o copiare il numero di conferma visualizzato quando il file viene caricato.</span><span class="sxs-lookup"><span data-stu-id="58554-120">Write down or copy the confirmation number that is displayed when the file upload is successful.</span></span>

<span data-ttu-id="58554-121">Per visualizzare i record Positive Pay esportati</span><span class="sxs-lookup"><span data-stu-id="58554-121">To view exported Positive Pay records</span></span>

1. <span data-ttu-id="58554-122">Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **C/C bancari**, quindi scegliere il collegamento correlato.</span><span class="sxs-lookup"><span data-stu-id="58554-122">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Bank Accounts**, and then choose the related link.</span></span>
2. <span data-ttu-id="58554-123">Selezionare il conto bancario per cui si desidera visualizzare i record di esportazione Positive Pay.</span><span class="sxs-lookup"><span data-stu-id="58554-123">Select the bank account that you want to view Positive Pay export records for.</span></span>
3. <span data-ttu-id="58554-124">Scegliere l'azione **Movimenti Positive Pay**.</span><span class="sxs-lookup"><span data-stu-id="58554-124">Choose the **Positive Pay Entries** action.</span></span>

    <span data-ttu-id="58554-125">Nella finestra **Movimenti Positive Pay** è possibile visualizzare tutti i record di esportazione Positive Pay per il conto corrente bancario.</span><span class="sxs-lookup"><span data-stu-id="58554-125">In the **Positive Pay Entries** window, you can see all the Positive Pay export records for the bank account.</span></span>
4. <span data-ttu-id="58554-126">Nel campo **Numero di conferma** immettere per ogni record esportare il numero di conferma che si riceve quando il caricamento del file alla banca è riuscito.</span><span class="sxs-lookup"><span data-stu-id="58554-126">In the **Confirmation Number** field, enter, for each export record, the confirmation number that you receive when the file upload to the bank is successful.</span></span>
5. <span data-ttu-id="58554-127">Per visualizzare le righe di pagamento, scegliere l'azione **Dettagli movimenti Positive Pay**.</span><span class="sxs-lookup"><span data-stu-id="58554-127">To view the related payment lines, choose the **Positive Pay Entry Details** action.</span></span>

<span data-ttu-id="58554-128">Per riesportare file Positive Pay</span><span class="sxs-lookup"><span data-stu-id="58554-128">To reexport Positive Pay files</span></span>

1. <span data-ttu-id="58554-129">Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **C/C bancari**, quindi scegliere il collegamento correlato.</span><span class="sxs-lookup"><span data-stu-id="58554-129">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Bank Accounts**, and then choose the related link.</span></span>
2. <span data-ttu-id="58554-130">Selezionare il conto bancario per cui si desidera riesportare i file Positive Pay.</span><span class="sxs-lookup"><span data-stu-id="58554-130">Select the bank account that you want to reexport Positive Pay files for.</span></span>
3. <span data-ttu-id="58554-131">Scegliere l'azione **Movimenti Positive Pay**.</span><span class="sxs-lookup"><span data-stu-id="58554-131">Choose the **Positive Pay Entries** action.</span></span>
4. <span data-ttu-id="58554-132">Selezionare la riga per il file di esportazione Positive Pay da riesportare.</span><span class="sxs-lookup"><span data-stu-id="58554-132">Select the line for the Positive Pay export file that you want to reexport.</span></span>
5. <span data-ttu-id="58554-133">Nella finestra **Movimenti Positive Pay** selezionare l'azione **Riesporta Positive Pay su file**.</span><span class="sxs-lookup"><span data-stu-id="58554-133">In the **Positive Pay Entries** window, choose the **Reexport Positive Pay to File** action.</span></span>

## <a name="see-also"></a><span data-ttu-id="58554-134">Vedi anche</span><span class="sxs-lookup"><span data-stu-id="58554-134">See Also</span></span>
[<span data-ttu-id="58554-135">Finanze</span><span class="sxs-lookup"><span data-stu-id="58554-135">Finance</span></span>](finance.md)  
[<span data-ttu-id="58554-136">Impostazione di dati finanziari</span><span class="sxs-lookup"><span data-stu-id="58554-136">Setting Up Finance</span></span>](finance-setup-finance.md)  
[<span data-ttu-id="58554-137">Utilizzo delle registrazioni COGE</span><span class="sxs-lookup"><span data-stu-id="58554-137">Working with General Journals</span></span>](ui-work-general-journals.md)  
<span data-ttu-id="58554-138">[Utilizzo di [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="58554-138">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
