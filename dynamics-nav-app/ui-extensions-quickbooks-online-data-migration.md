---
title: Utilizzo dell'estensione per la migrazione QuickBooks
description: Descrive come utilizzare l'estensione per migrare clienti, fornitori, articoli e conti da QuickBooks Online a Dynamics NAV.
documentationcenter: 
author: bholtorf
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms. search.keywords: extension, migrate, data, QuickBooks, import
ms.date: 05/24/2017
ms.author: bholtorf
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: ff8f8f0c529966fc108d2d4c86e2d0681b1fc005
ms.contentlocale: it-it
ms.lasthandoff: 10/16/2017

---

# <a name="the-quickbooks-online-data-migration-extension-for-dynamics-nav"></a><span data-ttu-id="7b335-103">Estensione di migrazione dei dati QuickBooks Online per Dynamics NAV</span><span class="sxs-lookup"><span data-stu-id="7b335-103">The QuickBooks Online Data Migration Extension for Dynamics NAV</span></span>
<span data-ttu-id="7b335-104">Questa estensione è inclusa nella Guida setup assistito **Migrazione dati** per semplificare la migrazione dei dati aziendali importanti da QuickBooks Online a [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="7b335-104">This extension is included in the **Data Migration** assisted setup guide to help you migrate important business data from QuickBooks Online to [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span> <span data-ttu-id="7b335-105">Ad esempio, può essere utile quando l'attività si sviluppa e si è deciso di aggiornare l'app di gestione aziendale cominciando a utilizzare [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="7b335-105">For example, this is useful when your business is growing, and you've decided to upgrade your business management app by starting to use [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span>

## <a name="what-data-can-i-import-from-quickbooks-online"></a><span data-ttu-id="7b335-106">Quali dati si possono importare da QuickBooks Online?</span><span class="sxs-lookup"><span data-stu-id="7b335-106">What data can I import from QuickBooks Online?</span></span>
<span data-ttu-id="7b335-107">È possibile importare i seguenti dati da QuickBooks Online a [!INCLUDE[d365fin](includes/d365fin_md.md)]:</span><span class="sxs-lookup"><span data-stu-id="7b335-107">You can import the following data from QuickBooks Online to [!INCLUDE[d365fin](includes/d365fin_md.md)]:</span></span>  

* <span data-ttu-id="7b335-108">Clienti</span><span class="sxs-lookup"><span data-stu-id="7b335-108">Customers</span></span>
* <span data-ttu-id="7b335-109">Fornitori</span><span class="sxs-lookup"><span data-stu-id="7b335-109">Vendors</span></span>
* <span data-ttu-id="7b335-110">Articoli</span><span class="sxs-lookup"><span data-stu-id="7b335-110">Items</span></span>
* <span data-ttu-id="7b335-111">Piano dei conti</span><span class="sxs-lookup"><span data-stu-id="7b335-111">Chart of accounts</span></span> 
* <span data-ttu-id="7b335-112">Transazioni di saldo iniziale di contabilità generale</span><span class="sxs-lookup"><span data-stu-id="7b335-112">Beginning balance transaction in the general ledger</span></span>
* <span data-ttu-id="7b335-113">Quantità disponibili per gli articoli di magazzino</span><span class="sxs-lookup"><span data-stu-id="7b335-113">On-hand quantities for inventory items</span></span>
* <span data-ttu-id="7b335-114">Documenti aperti per clienti e fornitori, quali fatture, note di credito e pagamenti</span><span class="sxs-lookup"><span data-stu-id="7b335-114">Open documents for customers and vendors, such as invoices, credit memos, and payments</span></span>

<span data-ttu-id="7b335-115">Verranno migrati solo gli importi complessivi relativi a documenti di vendita e acquisto.</span><span class="sxs-lookup"><span data-stu-id="7b335-115">We migrate only full amounts on sales and purchase documents.</span></span> <span data-ttu-id="7b335-116">Non vengono aggiornati gli importi parzialmente pagati.</span><span class="sxs-lookup"><span data-stu-id="7b335-116">We do not update partially paid amounts.</span></span> <span data-ttu-id="7b335-117">Ad esempio, se un cliente ha pagato 300 dollari su un totale di 500 dollari di una fattura di vendita, l'importo che verrà migrato è quello completo, ovvero 500 dollari.</span><span class="sxs-lookup"><span data-stu-id="7b335-117">For example, if a customer has paid 300 of a total of 500 dollars on a sales invoice, we migrate the full 500.</span></span> <span data-ttu-id="7b335-118">Se si ricevono pagamenti parziali, è necessario aggiornare manualmente questi valori, prima o dopo aver migrato i dati.</span><span class="sxs-lookup"><span data-stu-id="7b335-118">If you have received partial payments, you must update these manually, either before or after you migrate data.</span></span> <span data-ttu-id="7b335-119">Si consiglia di applicare le transazioni inevase prima della migrazione, per semplificare le attività successive alla migrazione.</span><span class="sxs-lookup"><span data-stu-id="7b335-119">We recommend that you apply outstanding transactions before you migrate, just to make things easier afterward.</span></span>

> [!NOTE]  
>   <span data-ttu-id="7b335-120">Non vengono migrati gli ordini di acquisto o di vendita.</span><span class="sxs-lookup"><span data-stu-id="7b335-120">We do not migrate purchase orders or sales orders.</span></span>

## <a name="before-you-start"></a><span data-ttu-id="7b335-121">Operazioni preliminari</span><span class="sxs-lookup"><span data-stu-id="7b335-121">Before you start</span></span>
<span data-ttu-id="7b335-122">Una parte importante del processo di migrazione consiste nello specificare i conti verso cui migrare le transazioni.</span><span class="sxs-lookup"><span data-stu-id="7b335-122">An important part of the migration process is to specify the accounts to migrate transactions to.</span></span> <span data-ttu-id="7b335-123">Si consiglia di pianificare questa mappatura che prima della migrazione dei dati.</span><span class="sxs-lookup"><span data-stu-id="7b335-123">It's a good idea to plan this mapping before you migrate data.</span></span> <span data-ttu-id="7b335-124">Ad esempio, i conti in cui vengono registrate le transazioni relative a:</span><span class="sxs-lookup"><span data-stu-id="7b335-124">For example, the accounts where you post transactions for:</span></span>  
  
* <span data-ttu-id="7b335-125">La vendita di articoli o servizi ai clienti.</span><span class="sxs-lookup"><span data-stu-id="7b335-125">The sale of items or services to customers.</span></span>
* <span data-ttu-id="7b335-126">L'acquisto di articoli o servizi dai fornitori.</span><span class="sxs-lookup"><span data-stu-id="7b335-126">The purchase of items or services from vendors.</span></span>  
* <span data-ttu-id="7b335-127">Rettifiche nella contabilità generale.</span><span class="sxs-lookup"><span data-stu-id="7b335-127">Adjustments in the general ledger.</span></span>  

[!INCLUDE[d365fin](includes/d365fin_md.md)]<span data-ttu-id="7b335-128"> richiede che i conti di contabilità generale abbaino numeri assegnati ad essi.</span><span class="sxs-lookup"><span data-stu-id="7b335-128"> requires that general ledger accounts have account numbers assigned to them.</span></span> <span data-ttu-id="7b335-129">Assicurarsi che i numeri vengano assegnati ai conti in QuickBooks Online.</span><span class="sxs-lookup"><span data-stu-id="7b335-129">Make sure that account numbers are assigned to your accounts in QuickBooks Online.</span></span>

<span data-ttu-id="7b335-130">Se le transazioni in QuickBooks Online includono importi di imposte, è necessario configurare un conto per le imposte in base alle giurisdizioni fiscali di [!INCLUDE[d365fin](includes/d365fin_md.md)] prima di registrare le transazioni.</span><span class="sxs-lookup"><span data-stu-id="7b335-130">If transactions in QuickBooks Online have tax amounts, you must set up a tax account for your tax jurisdictions in [!INCLUDE[d365fin](includes/d365fin_md.md)] before you can post transactions.</span></span>

## <a name="how-do-i-start-using-the-extension"></a><span data-ttu-id="7b335-131">Operazioni iniziali per l'utilizzo dell'estensione</span><span class="sxs-lookup"><span data-stu-id="7b335-131">How do I start using the extension?</span></span>
<span data-ttu-id="7b335-132">Iniziare è semplice.</span><span class="sxs-lookup"><span data-stu-id="7b335-132">Getting started is easy.</span></span> <span data-ttu-id="7b335-133">È necessario solo eseguire la Guida di setup assistito **Migrazione di dati**.</span><span class="sxs-lookup"><span data-stu-id="7b335-133">All you need to do is run the **Data Migration** assisted setup guide.</span></span> <span data-ttu-id="7b335-134">Ecco come:</span><span class="sxs-lookup"><span data-stu-id="7b335-134">Here's how:</span></span>

1. <span data-ttu-id="7b335-135">Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report") e immettere **Setup assistito**, quindi scegliere **Migra dati aziendali**.</span><span class="sxs-lookup"><span data-stu-id="7b335-135">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Assisted Setup**, and then choose **Migrate business data**.</span></span>
2. <span data-ttu-id="7b335-136">Seguire le istruzioni per ogni passaggio della Guida di setup assistito.</span><span class="sxs-lookup"><span data-stu-id="7b335-136">Follow the instructions on each step in the assisted setup guide.</span></span>

## <a name="what-do-i-do-after-i-migrate-data"></a><span data-ttu-id="7b335-137">Operazioni successive alla migrazione dei dati</span><span class="sxs-lookup"><span data-stu-id="7b335-137">What do I do after I migrate data?</span></span>
<span data-ttu-id="7b335-138">Dopo aver migrato i dati, le transazioni hanno come stato **Non registrata**, quindi è possibile esaminarle e apportare modifiche.</span><span class="sxs-lookup"><span data-stu-id="7b335-138">After you migrate data, transactions have the status **Unposted**, so you can review them and make adjustments.</span></span> <span data-ttu-id="7b335-139">Per verificare le transazioni, andare alla pagina in cui vengono in genere visualizzate.</span><span class="sxs-lookup"><span data-stu-id="7b335-139">To review the transactions, go to the page where you would normally find them.</span></span> <span data-ttu-id="7b335-140">Ad esempio, per esaminare le fatture di vendita non registrate, andare alla pagina **Fatture di vendita**.</span><span class="sxs-lookup"><span data-stu-id="7b335-140">For example, to review unposted sales invoices, go to the **Sales Invoices** page.</span></span> <span data-ttu-id="7b335-141">Per verificare le registrazioni pagamenti, andare alla pagina **Registrazioni pagamenti**.</span><span class="sxs-lookup"><span data-stu-id="7b335-141">To review payment journals, go to the **Payment Journals** page.</span></span>   

<span data-ttu-id="7b335-142">Esistono alcune operazioni consigliate:</span><span class="sxs-lookup"><span data-stu-id="7b335-142">There are a few things in particular that you should do:</span></span>

* <span data-ttu-id="7b335-143">Se le transazioni in QuickBooks Online presentano importi di markup o sconti, è necessario aggiungere manualmente gli importi alle transazioni relative in [!INCLUDE[d365fin](includes/d365fin_md.md)] prima di registrarle.</span><span class="sxs-lookup"><span data-stu-id="7b335-143">If the transactions in QuickBooks Online had markup or discount amounts, you must manually add the amounts to the related transactions in [!INCLUDE[d365fin](includes/d365fin_md.md)] before you post them.</span></span>
* <span data-ttu-id="7b335-144">Se si utilizza l'IVA, può essere necessario aggiungere una categoria di registrazione business e articoli/servizi nel Setup registrazione in modo che sia possibile registrare gli importi IVA.</span><span class="sxs-lookup"><span data-stu-id="7b335-144">If you are using value added tax (VAT), you may need to add a business posting group and a product posting group to the posting setup so that you can post VAT amounts.</span></span>
* <span data-ttu-id="7b335-145">Verificare i saldi iniziali per i conti della contabilità generale.</span><span class="sxs-lookup"><span data-stu-id="7b335-145">Verify the beginning balances for accounts in the general ledger.</span></span> <span data-ttu-id="7b335-146">QuickBooks Online non memorizza il saldo attuale per tutti i conti, potrebbe quindi essere necessario correggere i saldi iniziali.</span><span class="sxs-lookup"><span data-stu-id="7b335-146">QuickBooks Online does not store the current balance for all accounts, so you might need to correct beginning balances.</span></span>

## <a name="see-also"></a><span data-ttu-id="7b335-147">Vedi anche</span><span class="sxs-lookup"><span data-stu-id="7b335-147">See Also</span></span>
[<span data-ttu-id="7b335-148">Importazione dei dati aziendali da altri sistemi contabili</span><span class="sxs-lookup"><span data-stu-id="7b335-148">Importing Business Data from Other Finance Systems</span></span>](upload-data.md)  
<span data-ttu-id="7b335-149">[Personalizzazione di [!INCLUDE[d365fin](includes/d365fin_md.md)] utilizzando le estensioni](ui-extensions.md)</span><span class="sxs-lookup"><span data-stu-id="7b335-149">[Customizing [!INCLUDE[d365fin](includes/d365fin_md.md)] Using Extensions](ui-extensions.md)</span></span>  
