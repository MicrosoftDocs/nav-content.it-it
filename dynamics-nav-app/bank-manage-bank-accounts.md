---
title: Gestire i conti correnti bancari
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
ms.openlocfilehash: d97c3afba0e899768bda1b637c4f288db210d38c
ms.contentlocale: it-it
ms.lasthandoff: 07/19/2017

---

# <a name="manage-bank-accounts"></a><span data-ttu-id="45711-102">Gestire i conti correnti bancari</span><span class="sxs-lookup"><span data-stu-id="45711-102">Manage Bank Accounts</span></span>
<span data-ttu-id="45711-103">A intervalli regolari, è necessario riconciliare i movimenti contabili bancari in Dynamics NAV con le transazioni bancarie relative nei conti bancari presso la banca e quindi registrare il saldo al conto corrente bancario.</span><span class="sxs-lookup"><span data-stu-id="45711-103">At regular intervals, you must reconcile your bank ledger entries in Dynamics NAV with the related bank transactions in bank accounts at your bank, and then post the balance to your bank account.</span></span> <span data-ttu-id="45711-104">È possibile eseguire questa attività come parte dell'elaborazione dei pagamenti rappresentati in un estratto conto bancario in **Registrazione riconciliazione pagamenti**.</span><span class="sxs-lookup"><span data-stu-id="45711-104">You can perform this task either as part of processing the payments represented on a bank statement in the **Payment Reconciliation Journal**.</span></span> <span data-ttu-id="45711-105">In alternativa, è possibile eseguire questa attività in modo distinto dall'elaborazione del pagamento, nella finestra **Riconciliazioni C/C bancari**, che supporta i movimenti contabili degli assegni.</span><span class="sxs-lookup"><span data-stu-id="45711-105">Alternatively, you can perform the task separately from payment processing, in the **Bank Acc. Reconciliation** window, which supports check ledger entries.</span></span> <span data-ttu-id="45711-106">In entrambi i casi, compilare le finestre importando l'estratto conto bancario in Dynamics NAV.</span><span class="sxs-lookup"><span data-stu-id="45711-106">In both cases, you fill the windows by importing the bank statement into Dynamics NAV.</span></span>

<span data-ttu-id="45711-107">Talvolta, è necessario trasferire gli importi tra il conto corrente bancario in Dynamics NAV per riflettere i trasferimenti alla banca.</span><span class="sxs-lookup"><span data-stu-id="45711-107">Sometimes, you need to transfer amounts between bank account in Dynamics NAV to reflect transfers at your bank.</span></span> <span data-ttu-id="45711-108">È possibile eseguire questa attività nella finestra **Registrazioni COGE** in modi diversi a seconda della valuta dei fondi.</span><span class="sxs-lookup"><span data-stu-id="45711-108">You perform this task in the **General Journal** window, in different ways depending on the currency of the funds.</span></span>

<span data-ttu-id="45711-109">Prima di poter gestire i conti correnti bancari, è necessario impostare ogni conto bancario come scheda conto corrente bancario.</span><span class="sxs-lookup"><span data-stu-id="45711-109">Before you can manage bank accounts, you must set each bank account up as a bank account card.</span></span> <span data-ttu-id="45711-110">Inoltre, è necessario impostare i servizi elettronici che è possibile utilizzare per l'importazione dell'estratto conto bancario e l'esportazione del file di pagamento.</span><span class="sxs-lookup"><span data-stu-id="45711-110">In addition, you must set up electronic services that you may use for bank statement import and payment file export.</span></span> <span data-ttu-id="45711-111">Per ulteriori informazioni, vedere [Impostare i conti correnti bancari](bank-setup-banking.md).</span><span class="sxs-lookup"><span data-stu-id="45711-111">For more information, see [Set Up Bank Accounts](bank-setup-banking.md).</span></span>

<span data-ttu-id="45711-112">Nella tabella seguente viene descritta una sequenza di task, con collegamenti agli argomenti che li descrivono.</span><span class="sxs-lookup"><span data-stu-id="45711-112">The following table describes a sequence of tasks, with links to the topics that describe them.</span></span>

|<span data-ttu-id="45711-113">Per</span><span class="sxs-lookup"><span data-stu-id="45711-113">To</span></span> |<span data-ttu-id="45711-114">Vedere</span><span class="sxs-lookup"><span data-stu-id="45711-114">See</span></span> |
|---|----|
|<span data-ttu-id="45711-115">Riconciliare i conti correnti bancari in relazione all'elaborazione dei pagamenti nella finestra **Registrazione riconciliazione pagamenti**.</span><span class="sxs-lookup"><span data-stu-id="45711-115">Reconcile bank accounts in connection with payment processing in the **Payment Reconciliation Journal** window.</span></span>|[<span data-ttu-id="45711-116">Collegare i pagamenti automaticamente e riconciliare i conti correnti bancari</span><span class="sxs-lookup"><span data-stu-id="45711-116">Apply Payments Automatically and Reconcile Bank Accounts</span></span>](receivables-apply-payments-auto-reconcile-bank-accounts.md)|
|<span data-ttu-id="45711-117">Riconciliare i conti bancari, inclusi i movimenti contabili assegni, come attività separata nella finestra **Riconciliazioni C/C bancari**.</span><span class="sxs-lookup"><span data-stu-id="45711-117">Reconcile bank accounts, including check ledger entries, as a separate task in the **Bank Acc. Reconciliation** window.</span></span>|[<span data-ttu-id="45711-118">Procedura: Riconciliare i conti correnti bancari separatamente</span><span class="sxs-lookup"><span data-stu-id="45711-118">How to: Reconcile Bank Accounts Separately</span></span>](bank-how-reconcile-bank-accounts-separately.md)|
|<span data-ttu-id="45711-119">Registrare i bonifici tra conti correnti bancari nella stessa valuta o in valute diverse.</span><span class="sxs-lookup"><span data-stu-id="45711-119">Post transfers between bank accounts in the same currency or in different currencies.</span></span>|[<span data-ttu-id="45711-120">Procedura: Trasferire fondi bancari</span><span class="sxs-lookup"><span data-stu-id="45711-120">How to: Transfer Bank Funds</span></span>](bank-how-transfer-bank-funds.md)
## <a name="see-also"></a><span data-ttu-id="45711-121">Vedi anche</span><span class="sxs-lookup"><span data-stu-id="45711-121">See Also</span></span>  
[<span data-ttu-id="45711-122">Impostare le attività bancarie</span><span class="sxs-lookup"><span data-stu-id="45711-122">Set Up Banking</span></span>](bank-setup-banking.md)  
[<span data-ttu-id="45711-123">Gestire la contabilità clienti</span><span class="sxs-lookup"><span data-stu-id="45711-123">Manage Receivables</span></span>](receivables-manage-receivables.md)  
<span data-ttu-id="45711-124">[Gestire la contabilità fornitori](payables-manage-payables.md)  </span><span class="sxs-lookup"><span data-stu-id="45711-124">[Manage Payables](payables-manage-payables.md)  </span></span>  
[<span data-ttu-id="45711-125">Utilizzare Dynamics NAV</span><span class="sxs-lookup"><span data-stu-id="45711-125">Work With Dynamics NAV</span></span>](ui-work-product.md)  
[<span data-ttu-id="45711-126">Tra le aree aziendali</span><span class="sxs-lookup"><span data-stu-id="45711-126">Across Business Areas</span></span>](ui-across-business-areas.md)

