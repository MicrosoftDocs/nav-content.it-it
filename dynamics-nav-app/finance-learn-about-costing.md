---
title: Informazioni sul costing di magazzino
description: La gestione dei costi di magazzino include la registrazione e il reporting dei costi operativi business. Comprende inoltre il reporting dei costi di produzione e di magazzino, ovvero il valore degli articoli.
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 3b265e86751060b75b9f37580923469612cd1b56
ms.contentlocale: it-it
ms.lasthandoff: 10/16/2017

---
# <a name="about-inventory-costing"></a><span data-ttu-id="9b08f-104">Informazioni sul costing di magazzino</span><span class="sxs-lookup"><span data-stu-id="9b08f-104">About Inventory Costing</span></span>
<span data-ttu-id="9b08f-105">La gestione dei costi di magazzino include la registrazione e il reporting dei costi operativi business.</span><span class="sxs-lookup"><span data-stu-id="9b08f-105">Managing inventory costs is concerned with recording and reporting business operating costs.</span></span> <span data-ttu-id="9b08f-106">Comprende inoltre il reporting dei costi di produzione e di magazzino, ovvero il valore degli articoli.</span><span class="sxs-lookup"><span data-stu-id="9b08f-106">It includes the reporting of manufacturing costs and inventory costs, that is, the value of items.</span></span>  

 <span data-ttu-id="9b08f-107">Di seguito sono elencati i principi fondamentali di questa materia: i metodi di costing definiscono il modo in cui gli articoli vengono valutati quando escono dal magazzino, la rettifica dei costi aggiorna il costo della merce venduta con costi di acquisto correlati registrati dopo la vendita e infine il valore di magazzino deve essere registrato in appositi conti C/G con periodicità regolare.</span><span class="sxs-lookup"><span data-stu-id="9b08f-107">Central principles to understand are that costing methods define how items are valued when they leave inventory, that cost adjustment updates the cost of goods sold with related purchase costs posted after the sale, and that inventory values must be posted to dedicated G/L accounts at regular intervals.</span></span>  

 <span data-ttu-id="9b08f-108">Nella tabella seguente viene descritta una sequenza di task, con collegamenti agli argomenti che li descrivono.</span><span class="sxs-lookup"><span data-stu-id="9b08f-108">The following table describes a sequence of tasks, with links to the topics that describe them.</span></span>   

|<span data-ttu-id="9b08f-109">**Per**</span><span class="sxs-lookup"><span data-stu-id="9b08f-109">**To**</span></span>|<span data-ttu-id="9b08f-110">**Vedere**</span><span class="sxs-lookup"><span data-stu-id="9b08f-110">**See**</span></span>|  
|------------|-------------|  
|<span data-ttu-id="9b08f-111">Distinguere i diversi metodi di costing e il relativo effetto sui flussi dei costi.</span><span class="sxs-lookup"><span data-stu-id="9b08f-111">Distinguish the five different costing methods and their effect on cost flows.</span></span>|[<span data-ttu-id="9b08f-112">Dettagli di progettazione: Metodi di costing</span><span class="sxs-lookup"><span data-stu-id="9b08f-112">Design Details: Costing Methods</span></span>](design-details-costing-methods.md)|  
|<span data-ttu-id="9b08f-113">Ottenere informazioni sul modo in cui i movimenti di collegamento articoli collegano dinamicamente le riduzioni con gli aumenti di magazzino per mantenere il controllo dei flussi dei costi.</span><span class="sxs-lookup"><span data-stu-id="9b08f-113">Learn how item application entries dynamically link inventory decreases with increases to keep control of cost flows.</span></span>|[<span data-ttu-id="9b08f-114">Dettagli di progettazione: Collegamento articoli</span><span class="sxs-lookup"><span data-stu-id="9b08f-114">Design Details: Item Application</span></span>](design-details-item-application.md)|  
|<span data-ttu-id="9b08f-115">Ottenere informazioni sul modo in cui il costo unitario di un articolo viene continuamente aggiornato con il costo dell'ultima transazione in base al metodo di costing dell'articolo.</span><span class="sxs-lookup"><span data-stu-id="9b08f-115">Learn how an item's unit cost is continuously updated with the cost of its latest transaction according to the item's costing method.</span></span>|[<span data-ttu-id="9b08f-116">Dettagli di progettazione: Rettifica costo</span><span class="sxs-lookup"><span data-stu-id="9b08f-116">Design Details: Cost Adjustment</span></span>](design-details-cost-adjustment.md)|  
|<span data-ttu-id="9b08f-117">Ottenere informazioni sul modo in cui il costo medio di un articolo viene calcolato dinamicamente in base al costo medio del periodo selezionato.</span><span class="sxs-lookup"><span data-stu-id="9b08f-117">Learn how an item's average cost is dynamically calculated according to the selected average cost period.</span></span>|[<span data-ttu-id="9b08f-118">Dettagli di progettazione: Costo medio</span><span class="sxs-lookup"><span data-stu-id="9b08f-118">Design Details: Average Cost</span></span>](design-details-average-cost.md)|  
|<span data-ttu-id="9b08f-119">Distinguere il costo previsto (non ancora fatturato) dal costo effettivo e apprendere come viene gestito nella contabilità generale.</span><span class="sxs-lookup"><span data-stu-id="9b08f-119">Distinguish expected cost (not yet invoiced) from actual cost and learn how it is managed in the general ledger.</span></span>|[<span data-ttu-id="9b08f-120">Dettagli di progettazione: Registrazione del costo previsto</span><span class="sxs-lookup"><span data-stu-id="9b08f-120">Design Details: Expected Cost Posting</span></span>](design-details-expected-cost-posting.md)|  
|<span data-ttu-id="9b08f-121">Comprendere il meccanismo di rettifica dei costi, che assicura il riporto dei costi anche se le transazioni di magazzino avvengono in modo casuale.</span><span class="sxs-lookup"><span data-stu-id="9b08f-121">Understand the cost adjustment mechanism, which ensures that costs are brought forward even if inventory transactions happen in a random manner.</span></span>|[<span data-ttu-id="9b08f-122">Dettagli di progettazione: Rettifica costo</span><span class="sxs-lookup"><span data-stu-id="9b08f-122">Design Details: Cost Adjustment</span></span>](design-details-cost-adjustment.md)|  
|<span data-ttu-id="9b08f-123">Apprendere per quale motivo i costi standard vengono spesso utilizzati dalle aziende manifatturiere come base di valutazione per componenti e articoli finali.</span><span class="sxs-lookup"><span data-stu-id="9b08f-123">Read why standard costs are often used by manufacturing companies as a valuation base for components and end items.</span></span>|[<span data-ttu-id="9b08f-124">Informazioni sul calcolo del costo standard</span><span class="sxs-lookup"><span data-stu-id="9b08f-124">About Calculating Standard Cost</span></span>](finance-about-calculating-standard-cost.md)|  
|<span data-ttu-id="9b08f-125">Comprendere il modo in cui il valore di magazzino viene riflesso nella contabilità generale.</span><span class="sxs-lookup"><span data-stu-id="9b08f-125">Understand how the value of inventory is reflected in the general ledger.</span></span>|[<span data-ttu-id="9b08f-126">Creazione di report dei costi e riconciliazione con la contabilità generale</span><span class="sxs-lookup"><span data-stu-id="9b08f-126">Reporting Costs and Reconciling with the General Ledger</span></span>](finance-report-costs-and-reconcile-with-the-general-ledger.md)|  
|<span data-ttu-id="9b08f-127">Ottenere informazioni sul modo in cui gli addebiti articoli, come le spese di trasposto e l'assicurazione, possono attribuire componenti di costo supplementari al costo unitario di un articolo.</span><span class="sxs-lookup"><span data-stu-id="9b08f-127">Learn how item charges, such as freight and insurance, can assign additional cost components to an item's unit cost.</span></span>|[<span data-ttu-id="9b08f-128">Procedura: Utilizzare gli addebiti articolo al conto per i costi aggiuntivi commerciali</span><span class="sxs-lookup"><span data-stu-id="9b08f-128">How to: Use Item Charges to Account for Additional Trade Costs</span></span>](payables-how-assign-item-charges.md)|  
|<span data-ttu-id="9b08f-129">Apprendere come i periodi di magazzino consentano a una società di controllare il valore di magazzino nel tempo mediante la definizione di periodi più brevi, che possono essere chiusi per la registrazione con l'avanzamento dell'anno fiscale.</span><span class="sxs-lookup"><span data-stu-id="9b08f-129">Read how inventory periods help a company to control inventory value over time by defining shorter periods that can be closed for posting as the fiscal year progresses.</span></span>|[<span data-ttu-id="9b08f-130">Procedura: Utilizzare periodi di magazzino</span><span class="sxs-lookup"><span data-stu-id="9b08f-130">How to: Work with Inventory Periods</span></span>](finance-how-to-work-with-inventory-periods.md)|  
|<span data-ttu-id="9b08f-131">Comprendere tutti i meccanismi del motore di costing, incluso quanto accade quando si registrano transazioni di produzione e di assemblaggio.</span><span class="sxs-lookup"><span data-stu-id="9b08f-131">Understand all mechanisms in the costing engine, including what happens when you post assembly and production transactions.</span></span>|[<span data-ttu-id="9b08f-132">Dettagli di progettazione: Costing di magazzino</span><span class="sxs-lookup"><span data-stu-id="9b08f-132">Design Details: Inventory Costing</span></span>](design-details-inventory-costing.md)|

## <a name="see-also"></a><span data-ttu-id="9b08f-133">Vedi anche</span><span class="sxs-lookup"><span data-stu-id="9b08f-133">See Also</span></span>
<span data-ttu-id="9b08f-134">[Gestione dei costi di magazzino](finance-manage-inventory-costs.md)  </span><span class="sxs-lookup"><span data-stu-id="9b08f-134">[Managing Inventory Costs](finance-manage-inventory-costs.md)  </span></span>  
<span data-ttu-id="9b08f-135">[Utilizzo di [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="9b08f-135">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
