---
title: 'Procedura: Utilizzare le chiavi di allocazione nelle registrazioni COGE'
author: edupont04
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 6b60b1344a1e18ad91863046110df880f75f7c04
ms.openlocfilehash: ca21d9d129dbc98d75371d1b2b7a0ffad4aa2848
ms.contentlocale: it-it
ms.lasthandoff: 07/19/2017

---

#  <a name="how-to-use-allocation-keys-in-general-journals"></a><span data-ttu-id="463d6-102">Procedura: Utilizzare le chiavi di allocazione nelle registrazioni COGE</span><span class="sxs-lookup"><span data-stu-id="463d6-102">How to: Use Allocation Keys in General Journals</span></span>
<span data-ttu-id="463d6-103">È possibile assegnare un movimento in una registrazione generale a più conti diversi, quando tale registrazione viene contabilizzata.</span><span class="sxs-lookup"><span data-stu-id="463d6-103">You can allocate an entry in a general journal to several different accounts when you post the journal.</span></span> <span data-ttu-id="463d6-104">L'allocazione può essere effettuata per quantità, percentuale o importo.</span><span class="sxs-lookup"><span data-stu-id="463d6-104">The allocation can be made by quantity, percentage, or amount.</span></span>

## <a name="to-set-up-allocation-keys"></a><span data-ttu-id="463d6-105">Per impostare le chiavi di allocazione</span><span class="sxs-lookup"><span data-stu-id="463d6-105">To set up allocation keys</span></span> 
1. <span data-ttu-id="463d6-106">Nell'angolo superiore destro, scegliere l'icona **Cerca pagina o report**, immettere **Reg. periodiche generali**, quindi scegliere il collegamento correlato.</span><span class="sxs-lookup"><span data-stu-id="463d6-106">In the top right corner, choose the **Search for Page or Report** icon, enter **Recurring General Journal**, and then choose the related link.</span></span>
2. <span data-ttu-id="463d6-107">Scegliere il campo **Nome batch** per aprire la finestra **Batch registrazioni COGE**.</span><span class="sxs-lookup"><span data-stu-id="463d6-107">Choose the **Batch Name** field to open the **General Journal Batches** window.</span></span>
3. <span data-ttu-id="463d6-108">È possibile modificare le allocazioni in un batch esistente nell'elenco o creare un nuovo batch con le allocazioni.</span><span class="sxs-lookup"><span data-stu-id="463d6-108">You can either modify allocations on an existing batch in the list or create a new batch with allocations.</span></span>
  * <span data-ttu-id="463d6-109">Per creare un nuovo batch, scegliere l'azione **Nuovo** e andare al passaggio successivo.</span><span class="sxs-lookup"><span data-stu-id="463d6-109">To create a new batch, choose the **New** action, and go to the next step.</span></span>
  * <span data-ttu-id="463d6-110">Per modificare le allocazioni di registrazioni esistenti, selezionare le registrazioni e andare al passaggio 7.</span><span class="sxs-lookup"><span data-stu-id="463d6-110">To change the allocations of an existing journal, select the journal and go to step 7.</span></span>    
4. <span data-ttu-id="463d6-111">Nel campo **Nome** immettere un nome per il batch, ad esempio PULIZIE.</span><span class="sxs-lookup"><span data-stu-id="463d6-111">In the **Name** field, enter a name for the batch, such as CLEANING.</span></span> <span data-ttu-id="463d6-112">Nel campo **Descrizione** immettere una descrizione, ad esempio Registrazioni spese pulizie.</span><span class="sxs-lookup"><span data-stu-id="463d6-112">In the **Description** field, enter a description, such as Cleaning Expenses Journal.</span></span>
5. <span data-ttu-id="463d6-113">Al termine, chiudere la finestra.</span><span class="sxs-lookup"><span data-stu-id="463d6-113">When you are done, close the window.</span></span> <span data-ttu-id="463d6-114">Verrà visualizzata una nuova registrazione periodica vuota.</span><span class="sxs-lookup"><span data-stu-id="463d6-114">A new, empty recurring journal opens.</span></span> 
6. <span data-ttu-id="463d6-115">Compilare i campi nella riga.</span><span class="sxs-lookup"><span data-stu-id="463d6-115">Fill in the fields in the line.</span></span>
7. <span data-ttu-id="463d6-116">Scegliere l'azione **Allocazioni**.</span><span class="sxs-lookup"><span data-stu-id="463d6-116">Choose the **Allocations** action.</span></span> 
8. <span data-ttu-id="463d6-117">Aggiungere una riga per ciascuna allocazione.</span><span class="sxs-lookup"><span data-stu-id="463d6-117">Add a line for each allocation.</span></span> <span data-ttu-id="463d6-118">È necessario compilare il campo **Allocazione %**, **Quantità allocazione** o **Importo**.</span><span class="sxs-lookup"><span data-stu-id="463d6-118">You must fill in either the **Allocation %**, **Allocation Quantity**, or **Amount** field.</span></span> <span data-ttu-id="463d6-119">È inoltre necessario compilare il campo **Nr. conto**</span><span class="sxs-lookup"><span data-stu-id="463d6-119">You must also fill in the **Account No.**</span></span> <span data-ttu-id="463d6-120">e, se si sta allocando la transazione tra dimensioni globali, anche i campi delle dimensioni globali.</span><span class="sxs-lookup"><span data-stu-id="463d6-120">field and, if you are allocating the transaction among global dimensions, the global dimension fields.</span></span>
9. <span data-ttu-id="463d6-121">Se in una riga è stata immessa una percentuale, il valore del campo **Importo** viene calcolato automaticamente.</span><span class="sxs-lookup"><span data-stu-id="463d6-121">If you enter a percentage on a line, the amount in the **Amount** field is calculated automatically.</span></span> <span data-ttu-id="463d6-122">Questi importi hanno il segno opposto rispetto all'importo totale nel campo **Importo** delle registrazioni periodiche.</span><span class="sxs-lookup"><span data-stu-id="463d6-122">These amounts have the opposite sign from the total amount in the **Amount** field in the recurring journal.</span></span>
10. <span data-ttu-id="463d6-123">Dopo aver immesso le righe di allocazione, scegliere **OK** per tornare alla finestra **Reg. periodiche generali**.</span><span class="sxs-lookup"><span data-stu-id="463d6-123">After entering the allocations lines, choose **OK** to return to the **Recurring General Journal** window.</span></span> <span data-ttu-id="463d6-124">Il campo **Importo allocato (VL)** viene compilato e corrisponde al campo **Importo**.</span><span class="sxs-lookup"><span data-stu-id="463d6-124">The **Allocated Amt. (USD)** field is filled in and matches the **Amount** field.</span></span>
11. <span data-ttu-id="463d6-125">Effettuare la registrazione.</span><span class="sxs-lookup"><span data-stu-id="463d6-125">Post the journal.</span></span>

## <a name="to-change-an-allocation-key-that-has-already-been-set-up"></a><span data-ttu-id="463d6-126">Per modificare una chiave di allocazione già impostata</span><span class="sxs-lookup"><span data-stu-id="463d6-126">To change an allocation key that has already been set up</span></span>
1. <span data-ttu-id="463d6-127">Nell'angolo superiore destro, scegliere l'icona **Cerca pagina o report**, immettere **Reg. periodiche generali**, quindi scegliere il collegamento correlato.</span><span class="sxs-lookup"><span data-stu-id="463d6-127">In the top right corner, choose the **Search for Page or Report** icon, enter **Recurring General Journal**, and then choose the related link.</span></span>
2. <span data-ttu-id="463d6-128">Nella finestra **Registrazioni periodiche generali** selezionare le registrazioni con l'allocazione.</span><span class="sxs-lookup"><span data-stu-id="463d6-128">In the **Recurring General Journal** window, select the journal with the allocation.</span></span>
3. <span data-ttu-id="463d6-129">Selezionare la riga con l'allocazione e scegliere l'azione **Allocazioni**.</span><span class="sxs-lookup"><span data-stu-id="463d6-129">Choose the line with the allocation, and then choose **Allocations** action.</span></span>
4. <span data-ttu-id="463d6-130">Modificare i campi pertinenti e chiudere la finestra.</span><span class="sxs-lookup"><span data-stu-id="463d6-130">Change the relevant fields, and close the window.</span></span>

## <a name="see-also"></a><span data-ttu-id="463d6-131">Vedi anche</span><span class="sxs-lookup"><span data-stu-id="463d6-131">See Also</span></span>
[<span data-ttu-id="463d6-132">Utilizzo delle registrazioni COGE</span><span class="sxs-lookup"><span data-stu-id="463d6-132">Work With General Journals</span></span>](ui-work-general-journals.md)  
[<span data-ttu-id="463d6-133">Contabilizzare documenti e registrazioni</span><span class="sxs-lookup"><span data-stu-id="463d6-133">Post Documents and Journals</span></span>](ui-post-documents-journals.md)




