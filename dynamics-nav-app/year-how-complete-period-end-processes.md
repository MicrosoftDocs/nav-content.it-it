---
title: Chiudere i periodi
author: jswymer
ms.custom: na
ms.date: 09/16/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: ac1ed2d1dcf8bf780bda91fbf0a04e5c5e8d106a
ms.contentlocale: it-it
ms.lasthandoff: 06/26/2017

---
# <a name="close-periods"></a><span data-ttu-id="1c1d5-102">Chiudere i periodi</span><span class="sxs-lookup"><span data-stu-id="1c1d5-102">Close Periods</span></span>
<span data-ttu-id="1c1d5-103">Non è obbligatorio chiudere i periodi, tuttavia, se lo si desidera, vi sono numerose attività di chiusura del periodo (chiusura del mese) che è possibile svolgere.</span><span class="sxs-lookup"><span data-stu-id="1c1d5-103">The application does not force you to close periods, however, there are many period-end (month-end) activities that can be performed in the application if you want.</span></span> <span data-ttu-id="1c1d5-104">In questo argomento viene fornita una panoramica dei processi e delle attività che possono o non possono essere necessari per la società.</span><span class="sxs-lookup"><span data-stu-id="1c1d5-104">This topic provides an overview of these processes and activities, which may or may not be necessary for your company.</span></span>

## <a name="general-ledger"></a><span data-ttu-id="1c1d5-105">Contabilità generale</span><span class="sxs-lookup"><span data-stu-id="1c1d5-105">General Ledger</span></span>
* <span data-ttu-id="1c1d5-106">Specificare intervalli di date di registrazione a livello di sistema e specifici dell'utente.</span><span class="sxs-lookup"><span data-stu-id="1c1d5-106">Specify system-wide and user-specific posting period.</span></span>

    <span data-ttu-id="1c1d5-107">Ciò specifica le date tra cui le registrazioni sono ammesse.</span><span class="sxs-lookup"><span data-stu-id="1c1d5-107">This specifies the dates between which postings are allowed.</span></span> <span data-ttu-id="1c1d5-108">In base alle esigenze aziendali, è possibile limitare gli intervalli di date di registrazione all'inizio del processo di chiusura del periodo o in un secondo momento verso la fine del periodo.</span><span class="sxs-lookup"><span data-stu-id="1c1d5-108">Depending on your business needs, you may want to restrict user posting date ranges at the start of the period-end process or at later time towards the end of the period.</span></span> <span data-ttu-id="1c1d5-109">Per ulteriori informazioni, vedere [Procedura: Specificare i periodi di registrazione](finance-setup-how-specify-posting-periods.md).</span><span class="sxs-lookup"><span data-stu-id="1c1d5-109">For more information, see [How to: Specify Posting Periods](finance-setup-how-specify-posting-periods.md).</span></span>
* <span data-ttu-id="1c1d5-110">Apportare tutte le rettifiche C/G necessarie.</span><span class="sxs-lookup"><span data-stu-id="1c1d5-110">Make all necessary G/L adjustments.</span></span>
* <span data-ttu-id="1c1d5-111">Aggiornare e contabilizzare le registrazioni periodiche.</span><span class="sxs-lookup"><span data-stu-id="1c1d5-111">Update and post Recurring Journals.</span></span>
<!--* Process Consolidations-->
* <span data-ttu-id="1c1d5-112">Eseguire le situazioni contabili come segue:</span><span class="sxs-lookup"><span data-stu-id="1c1d5-112">Run account schedules as follows:</span></span>
  1. <span data-ttu-id="1c1d5-113">Aprire la finestra **Situazione contabile** e scegliere l'azione **Stampa**.</span><span class="sxs-lookup"><span data-stu-id="1c1d5-113">Open the **Account Schedule** window, and choose the **Print** action.</span></span>
  2. <span data-ttu-id="1c1d5-114">Compilare la finestra **Situazione contabile** e scegliere l'azione **Stampa**.</span><span class="sxs-lookup"><span data-stu-id="1c1d5-114">Fill the **Account Schedule** request window and choose the **Print** action.</span></span>

## <a name="sales--receivables"></a><span data-ttu-id="1c1d5-115">Contabilità clienti</span><span class="sxs-lookup"><span data-stu-id="1c1d5-115">Sales & Receivables</span></span>
* <span data-ttu-id="1c1d5-116">Registrare tutti gli ordini di vendita, le fatture, le note di credito e gli ordini di reso.</span><span class="sxs-lookup"><span data-stu-id="1c1d5-116">Post all sales orders, invoices, credit memos, and return orders.</span></span>
* <span data-ttu-id="1c1d5-117">Contabilizzare tutte le registrazioni incassi.</span><span class="sxs-lookup"><span data-stu-id="1c1d5-117">Post all cash receipt journals.</span></span>
* <span data-ttu-id="1c1d5-118">Aggiornare e contabilizzare le registrazioni periodiche correlate alla contabilità clienti.</span><span class="sxs-lookup"><span data-stu-id="1c1d5-118">Update and post recurring journals that are related to Sales & Receivables.</span></span>
* <span data-ttu-id="1c1d5-119">Riconciliare i crediti v/clienti nella contabilità generale.</span><span class="sxs-lookup"><span data-stu-id="1c1d5-119">Reconcile accounts receivable to the general ledger.</span></span>
* <span data-ttu-id="1c1d5-120">Eseguire il processo batch **Elimina ord. vendita fatturati**.</span><span class="sxs-lookup"><span data-stu-id="1c1d5-120">Run the **Delete Invoiced Sales Orders** batch job.</span></span>

## <a name="purchases--payables"></a><span data-ttu-id="1c1d5-121">Contabilità fornitori</span><span class="sxs-lookup"><span data-stu-id="1c1d5-121">Purchases & Payables</span></span>
* <span data-ttu-id="1c1d5-122">Contabilizzare tutti gli ordini di acquisto, le fatture, le note di credito e gli ordini di reso.</span><span class="sxs-lookup"><span data-stu-id="1c1d5-122">Post all purchase orders, invoices, credit memos, and return orders.</span></span>
* <span data-ttu-id="1c1d5-123">Contabilizzare tutte le registrazioni pagamenti.</span><span class="sxs-lookup"><span data-stu-id="1c1d5-123">Post all payment journals.</span></span>
* <span data-ttu-id="1c1d5-124">Aggiornare e contabilizzare le registrazioni periodiche correlate alla contabilità fornitori.</span><span class="sxs-lookup"><span data-stu-id="1c1d5-124">Update and post recurring journals that are related to purchases & payables.</span></span>
* <span data-ttu-id="1c1d5-125">Eseguire il report **Scadenziario fornitori** e riconciliare i debiti v/fornitori nella contabilità generale.</span><span class="sxs-lookup"><span data-stu-id="1c1d5-125">Run the **Aged Accounts Payable** report and reconcile accounts payable to the general ledger.</span></span>
* <span data-ttu-id="1c1d5-126">Eseguire il processo batch **Elimina ordini acquisto fatturati**.</span><span class="sxs-lookup"><span data-stu-id="1c1d5-126">Run the **Delete Invoiced Purchase Orders** batch job.</span></span>

<!-- ### Fixed Assets
* Post all maintenance costs have been posted through the fixed asset journals or invoices.
* Post adjustments.
* Post appreciation.
* Post depreciation.
* Update and post the recurring fixed asset journal.-->

<!--### Intercompany
* Process Intercompany Postings.-->

## <a name="calculate-and-process-sales-tax"></a><span data-ttu-id="1c1d5-127">Calcolare ed elaborare l'imposta di vendita.</span><span class="sxs-lookup"><span data-stu-id="1c1d5-127">Calculate and Process Sales Tax</span></span>
*  <span data-ttu-id="1c1d5-128">Completare le dichiarazioni fiscali.</span><span class="sxs-lookup"><span data-stu-id="1c1d5-128">Complete Tax Statements.</span></span>

## <a name="see-also"></a><span data-ttu-id="1c1d5-129">Vedi anche</span><span class="sxs-lookup"><span data-stu-id="1c1d5-129">See Also</span></span>
[<span data-ttu-id="1c1d5-130">Chiusura di anni e periodi</span><span class="sxs-lookup"><span data-stu-id="1c1d5-130">Closing Years and Periods</span></span>](year-close-years-periods.md)  
[<span data-ttu-id="1c1d5-131">Chiusura dei libri</span><span class="sxs-lookup"><span data-stu-id="1c1d5-131">Close Books</span></span>](year-close-books.md)

