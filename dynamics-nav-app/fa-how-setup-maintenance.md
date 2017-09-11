---
title: 'Procedura: Impostare la manutenzione cespiti'
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
ms.openlocfilehash: ace0fb13d2be71c7204f16f34f6b65b54ff98230
ms.contentlocale: it-it
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-set-up-fixed-asset-maintenance"></a><span data-ttu-id="62bb7-102">Procedura: Impostare la manutenzione cespiti</span><span class="sxs-lookup"><span data-stu-id="62bb7-102">How to: Set Up Fixed Asset Maintenance</span></span>
<span data-ttu-id="62bb7-103">Per gestire la manutenzione dei cespiti, è prima necessario impostare alcune informazioni generali di manutenzione, un conto analitico per i costi di manutenzione e i codici di manutenzione per i tipi di lavoro, ad esempio assistenza di routine o riparazione.</span><span class="sxs-lookup"><span data-stu-id="62bb7-103">To manage fixed asset maintenance, you must first set up some general maintenance information, a posting account for maintenance costs, and maintenance codes for types of work, such as Routine Service or Repair.</span></span>

## <a name="to-set-up-general-maintenance-information"></a><span data-ttu-id="62bb7-104">Per impostare le informazioni generali di manutenzione</span><span class="sxs-lookup"><span data-stu-id="62bb7-104">To set up general maintenance information</span></span>
<span data-ttu-id="62bb7-105">Se vengono impostati campi per la manutenzione è possibile registrare le spese di manutenzione dalla registrazione cespiti.</span><span class="sxs-lookup"><span data-stu-id="62bb7-105">If you set up the fields for maintenance, you can post maintenance expenses from the fixed asset journal.</span></span>
1. <span data-ttu-id="62bb7-106">Nell'angolo superiore destro, scegliere l'icona **Cerca pagina o report**, immettere **Cespiti**, quindi scegliere il collegamento correlato.</span><span class="sxs-lookup"><span data-stu-id="62bb7-106">In the top right corner, choose the **Search for Page or Report** icon, enter **Fixed Assets**, and then choose the related link.</span></span>
2. <span data-ttu-id="62bb7-107">Selezionare il cespite per cui si desidera definire la copertura assicurativa, quindi scegliere l'azione **Modifica**.</span><span class="sxs-lookup"><span data-stu-id="62bb7-107">Select the fixed asset that you to define insurance coverage for, and then choose the **Edit** action.</span></span>
3. <span data-ttu-id="62bb7-108">Compilare i campi appropriati nella Scheda dettaglio **Manutenzione**.</span><span class="sxs-lookup"><span data-stu-id="62bb7-108">On the **Maintenance** FastTab, fill in the fields as necessary.</span></span> <span data-ttu-id="62bb7-109">Selezionare il campo per visualizzare una breve descrizione del campo o il collegamento a ulteriori informazioni.</span><span class="sxs-lookup"><span data-stu-id="62bb7-109">Choose a field to read a short description of the field or link to more information.</span></span>

## <a name="to-set-up-maintenance-codes"></a><span data-ttu-id="62bb7-110">Per impostare i codici di manutenzione</span><span class="sxs-lookup"><span data-stu-id="62bb7-110">To set up maintenance codes</span></span>  
<span data-ttu-id="62bb7-111">Quando si registrano dei costi di manutenzione dalle registrazioni COGE, si compila il campo **Cod. manutenzione** per registrare il tipo di manutenzione eseguita, ad esempio assistenza di routine o riparazione.</span><span class="sxs-lookup"><span data-stu-id="62bb7-111">When you post maintenance costs from a general journal, you fill in the **Maintenance Code** field to record what kind of maintenance has been performed, such as routine service or repair.</span></span>
1. <span data-ttu-id="62bb7-112">Nell'angolo superiore destro, scegliere l'icona **Cerca pagina o report**, immettere **Manutenzione**, quindi scegliere il collegamento correlato.</span><span class="sxs-lookup"><span data-stu-id="62bb7-112">In the top right corner, choose the **Search for Page or Report** icon, enter **Maintenance**, and then choose the related link.</span></span>
2. <span data-ttu-id="62bb7-113">Nella finestra **Manutenzione**, impostare i codici per i diversi tipi di lavoro di manutenzione.</span><span class="sxs-lookup"><span data-stu-id="62bb7-113">In the **Maintenance** window, set up codes for different types of maintenance work.</span></span>

## <a name="to-set-up-maintenance-expense-accounts"></a><span data-ttu-id="62bb7-114">Per impostare i conti spesa manutenzione</span><span class="sxs-lookup"><span data-stu-id="62bb7-114">To set up maintenance expense accounts</span></span>  
<span data-ttu-id="62bb7-115">Per registrare i costi di manutenzione occorre prima immettere un numero di conto nella finestra **Cat. Reg. Cespite**.</span><span class="sxs-lookup"><span data-stu-id="62bb7-115">To post maintenance costs, you must first enter an account number in the **FA Posting Groups** window.</span></span>
1. <span data-ttu-id="62bb7-116">Nell'angolo superiore destro, scegliere l'icona **Cerca pagina o report**, immettere **Categorie registrazione cespiti**, quindi scegliere il collegamento correlato.</span><span class="sxs-lookup"><span data-stu-id="62bb7-116">In the top right corner, choose the **Search for Page or Report** icon, enter **FA Posting Groups**, and then choose the related link.</span></span>
2. <span data-ttu-id="62bb7-117">Compilare il campo **Conto Spesa Manutenzione** per ogni categoria di registrazione.</span><span class="sxs-lookup"><span data-stu-id="62bb7-117">Fill in the **Maintenance Expense Account** field for each posting group.</span></span>

<span data-ttu-id="62bb7-118">**Nota**: per definire che i costi di manutenzione vengano allocati ai reparti o ai progetti, impostare le chiavi di allocazione.</span><span class="sxs-lookup"><span data-stu-id="62bb7-118">**Note**: To define that maintenance costs are allocated to departments or projects, set up an allocation keys.</span></span> <span data-ttu-id="62bb7-119">Per ulteriori informazioni, vedere [Procedura: Impostare le funzionalità generali per i cespiti](fa-how-setup-general.md).</span><span class="sxs-lookup"><span data-stu-id="62bb7-119">For more information, see [How to: Set Up General Fixed Assets Features](fa-how-setup-general.md).</span></span>

## <a name="see-also"></a><span data-ttu-id="62bb7-120">Vedi anche</span><span class="sxs-lookup"><span data-stu-id="62bb7-120">See Also</span></span>
[<span data-ttu-id="62bb7-121">Impostazione cespiti</span><span class="sxs-lookup"><span data-stu-id="62bb7-121">Set Up Fixed Assets</span></span>](fa-setup.md)  
[<span data-ttu-id="62bb7-122">Gestione di cespiti</span><span class="sxs-lookup"><span data-stu-id="62bb7-122">Manage Fixed Assets</span></span>](fa-manage.md)  
[<span data-ttu-id="62bb7-123">Contabilità</span><span class="sxs-lookup"><span data-stu-id="62bb7-123">Finance</span></span>](finance-setup.md)  
[<span data-ttu-id="62bb7-124">Benvenuto in Dynamics NAV</span><span class="sxs-lookup"><span data-stu-id="62bb7-124">Welcome to Dynamics NAV</span></span>](across-get-started.md)

