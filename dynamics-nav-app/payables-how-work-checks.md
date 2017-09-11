---
title: 'Procedura: Utilizzo degli assegni'
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
ms.openlocfilehash: 421516a7580a90d6eabc8ecfcc841215839994c9
ms.contentlocale: it-it
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-work-with-checks"></a><span data-ttu-id="7f4d9-102">Procedura: Utilizzo degli assegni</span><span class="sxs-lookup"><span data-stu-id="7f4d9-102">How to: Work With Checks</span></span>
<span data-ttu-id="7f4d9-103">Dynamics NAV supporta l'emissione elettronica e manuale di assegni.</span><span class="sxs-lookup"><span data-stu-id="7f4d9-103">Dynamics NAV supports electronic and manual check issuance.</span></span> <span data-ttu-id="7f4d9-104">In entrambi i metodi vengono utilizzate le registrazioni pagamenti per emettere assegni ai fornitori.</span><span class="sxs-lookup"><span data-stu-id="7f4d9-104">Both methods use the payment journal to issue checks to vendors.</span></span> <span data-ttu-id="7f4d9-105">È inoltre possibile annullare assegni e visualizzare movimenti contabili assegni.</span><span class="sxs-lookup"><span data-stu-id="7f4d9-105">You can also void checks and view check ledger entries.</span></span>

<span data-ttu-id="7f4d9-106">Il processo di emissione degli assegni comporta il suggerimento di pagamenti, la creazione di movimenti contabili e la stampa di assegni automatici.</span><span class="sxs-lookup"><span data-stu-id="7f4d9-106">The process of issuing checks suggests payments, creates ledger entries, and prints the computer checks.</span></span>

<span data-ttu-id="7f4d9-107">La stampante deve essere configurata per i moduli di assegni e deve essere definito il layout dell'assegno da utilizzare.</span><span class="sxs-lookup"><span data-stu-id="7f4d9-107">Your printer must be correctly set up with the check forms, and you must define which check layout to use.</span></span> <span data-ttu-id="7f4d9-108">Per ulteriori informazioni, vedere [Procedura: Definire i layout degli assegni](finance-setup-how-define-check-layouts.md)</span><span class="sxs-lookup"><span data-stu-id="7f4d9-108">For more information, see [How to: Define Check Layouts](finance-setup-how-define-check-layouts.md)</span></span>

## <a name="to-issue-checks"></a><span data-ttu-id="7f4d9-109">Per emettere assegni</span><span class="sxs-lookup"><span data-stu-id="7f4d9-109">To issue checks</span></span>
1. <span data-ttu-id="7f4d9-110">Nell'angolo superiore destro, scegliere l'icona **Cerca pagina o report**, immettere **Registrazioni pagamenti**, quindi scegliere il collegamento correlato.</span><span class="sxs-lookup"><span data-stu-id="7f4d9-110">In the top right corner, choose the **Search for Page or Report** icon, enter **Payment Journals**, and then choose the related link.</span></span>
2. <span data-ttu-id="7f4d9-111">Compilare le registrazioni con pagamenti rilevanti, ad esempio utilizzando la funzione Sugg. pagamenti fornitore.</span><span class="sxs-lookup"><span data-stu-id="7f4d9-111">Fill in the journal with relevant payments, for example by using the Suggest Vendor Payments function.</span></span> <span data-ttu-id="7f4d9-112">Per ulteriori informazioni, vedere [Procedura: Suggerire i pagamenti ai fornitori](payables-how-suggest-vendor-payments.md).</span><span class="sxs-lookup"><span data-stu-id="7f4d9-112">For more information, see [How to: Suggest Vendor Payments](payables-how-suggest-vendor-payments.md).</span></span>
3. <span data-ttu-id="7f4d9-113">Nel campo **Tipo pagamento banca** nelle righe di registrazione per il pagamento che si desidera effettuare con assegni, selezionare una delle seguenti opzioni:</span><span class="sxs-lookup"><span data-stu-id="7f4d9-113">In the **Bank Payment Type** field on journal lines for payment that you want to make with checks, select one of the following options:</span></span>

 - <span data-ttu-id="7f4d9-114">**Assegno automatico**: selezionare questa opzione per stampare un assegno relativo all'importo specificato nella riga di registrazione pagamenti.</span><span class="sxs-lookup"><span data-stu-id="7f4d9-114">**Computer Check**: Select this option if you want to print a check for the amount on the payment journal line.</span></span> <span data-ttu-id="7f4d9-115">È necessario stampare gli assegni prima di poter registrare le righe di registrazione.</span><span class="sxs-lookup"><span data-stu-id="7f4d9-115">You must print the checks before you can post the journal lines.</span></span> <span data-ttu-id="7f4d9-116">È possibile selezionare **Assegno automatico** solo se il campo **Tipo contropartita** o il campo **Tipo conto** è impostato su **Conto bancario**.</span><span class="sxs-lookup"><span data-stu-id="7f4d9-116">You can only select **Computer Check** if the **Bal. Account Type** or the **Account Type** is **Bank Account**.</span></span>

 - <span data-ttu-id="7f4d9-117">**Assegno manuale**: selezionare questa opzione se è stato creato un assegno manualmente e si desidera creare un corrispondente movimento contabile per questo importo.</span><span class="sxs-lookup"><span data-stu-id="7f4d9-117">**Manual Check**: Select this option if you have created a check manually and want to create a corresponding check ledger entry for this amount.</span></span> <span data-ttu-id="7f4d9-118">Non è possibile stampare assegni tramite questa opzione da Dynamics NAV.</span><span class="sxs-lookup"><span data-stu-id="7f4d9-118">By using this option, you cannot print checks from Dynamics NAV.</span></span> <span data-ttu-id="7f4d9-119">È possibile selezionare **Assegno manuale** solo se il campo **Tipo contropartita** o il campo **Tipo conto** è impostato su **Conto bancario**.</span><span class="sxs-lookup"><span data-stu-id="7f4d9-119">You can only select **Manual Check** if the **Bal. Account Type** or the **Account Type** is **Bank Account**.</span></span>

    <span data-ttu-id="7f4d9-120">**Nota**: è necessario stampare gli assegni automatici prima di poter registrare le righe di registrazione correlate.</span><span class="sxs-lookup"><span data-stu-id="7f4d9-120">**Note**: You must print computer checks before you post the related journal lines.</span></span>
4. <span data-ttu-id="7f4d9-121">In caso di assegni automatici, scegliere **Stampa assegno**.</span><span class="sxs-lookup"><span data-stu-id="7f4d9-121">In case of computer checks, choose **Print Check**.</span></span>
5. <span data-ttu-id="7f4d9-122">Nella finestra **Assegno** compilare i campi secondo le proprie necessità.</span><span class="sxs-lookup"><span data-stu-id="7f4d9-122">In the **Check** window, fill in the fields as necessary.</span></span> <span data-ttu-id="7f4d9-123">Selezionare il campo per visualizzare una breve descrizione del campo o il collegamento a ulteriori informazioni.</span><span class="sxs-lookup"><span data-stu-id="7f4d9-123">Choose a field to read a short description of the field or link to more information.</span></span>
6. <span data-ttu-id="7f4d9-124">Selezionare il pulsante **Stampa**.</span><span class="sxs-lookup"><span data-stu-id="7f4d9-124">Choose the **Print** button.</span></span>

<span data-ttu-id="7f4d9-125">**Nota**: se è necessario stampare automaticamente gli assegni provenienti da vari conti correnti bancari utilizzando più di una valuta, eseguire un singolo processo batch **Stampa assegno** per ogni valuta, specificando il conto corrente bancario appropriato.</span><span class="sxs-lookup"><span data-stu-id="7f4d9-125">**Note**: If you want to print checks in more than one currency from different bank accounts, you must run the **Print Check** batch job separately for each currency and specify the appropriate bank account.</span></span>

## <a name="to-cancel-printed-checks-that-are-not-posted"></a><span data-ttu-id="7f4d9-126">Per annullare assegni stampati che non sono registrati</span><span class="sxs-lookup"><span data-stu-id="7f4d9-126">To cancel printed checks that are not posted</span></span>
<span data-ttu-id="7f4d9-127">È possibile annullare gli assegni non registrati dopo che sono stati stampati utilizzando l'azione **Annullo assegno** della finestra **Registrazioni pagamenti**.</span><span class="sxs-lookup"><span data-stu-id="7f4d9-127">You can cancel non-posted checks after they have been printed by using the **Void Check** action in the **Payment Journal** window.</span></span>
1. <span data-ttu-id="7f4d9-128">Nella finestra **Registrazioni pagamenti** scegliere **Annullo assegno**, quindi scegliere gli assegni da annullare.</span><span class="sxs-lookup"><span data-stu-id="7f4d9-128">In the **Payment Journal** window, choose the **Void Check**, and then choose which checks to cancel.</span></span>

## <a name="to-void-checks"></a><span data-ttu-id="7f4d9-129">Per annullare gli assegni</span><span class="sxs-lookup"><span data-stu-id="7f4d9-129">To void checks</span></span>
<span data-ttu-id="7f4d9-130">Una volta che i pagamenti tramite assegno sono stati registrati, è possibile annullare gli assegni dai movimenti contabili bancari risultanti.</span><span class="sxs-lookup"><span data-stu-id="7f4d9-130">When check payment have been posted, you can only cancel (void) checks from the resulting bank ledger entries.</span></span>

1. <span data-ttu-id="7f4d9-131">Nell'angolo superiore destro, scegliere l'icona **Cerca pagina o report**, immettere **C/C bancari**, quindi scegliere il collegamento correlato.</span><span class="sxs-lookup"><span data-stu-id="7f4d9-131">In the top right corner, choose the **Search for Page or Report** icon, enter **Bank Accounts**, and then choose the related link.</span></span>
2. <span data-ttu-id="7f4d9-132">Selezionare il conto corrente bancario appropriato, scegliere l'azione **Modifica**, quindi scegliere l'azione **Mov. contabili assegni**.</span><span class="sxs-lookup"><span data-stu-id="7f4d9-132">Select the relevant bank account, choose the **Edit** action, and then choose the **Check Ledger Entries** action.</span></span>
3. <span data-ttu-id="7f4d9-133">Nella finestra **Mov. contabili assegni** scegliere l'azione **Annullo assegno**.</span><span class="sxs-lookup"><span data-stu-id="7f4d9-133">In the **Check Ledger Entries** window, choose the **Void Check** action.</span></span>
4. <span data-ttu-id="7f4d9-134">Selezionare la casella di controllo **Annullo solo assegno**.</span><span class="sxs-lookup"><span data-stu-id="7f4d9-134">Select the **Void Check Only** check box.</span></span>
5. <span data-ttu-id="7f4d9-135">Scegliere **OK**.</span><span class="sxs-lookup"><span data-stu-id="7f4d9-135">Choose the **OK**button.</span></span>

## <a name="see-also"></a><span data-ttu-id="7f4d9-136">Vedi anche</span><span class="sxs-lookup"><span data-stu-id="7f4d9-136">See Also</span></span>
[<span data-ttu-id="7f4d9-137">Gestire la contabilità fornitori</span><span class="sxs-lookup"><span data-stu-id="7f4d9-137">Manage Payables</span></span>](payables-manage-payables.md)  
[<span data-ttu-id="7f4d9-138">Impostare le attività bancarie</span><span class="sxs-lookup"><span data-stu-id="7f4d9-138">Set Up Banking</span></span>](bank-setup-banking.md)  

