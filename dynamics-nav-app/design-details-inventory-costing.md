---
title: Dettagli di progettazione - Costing di magazzino
description: "In questa documentazione sono fornite informazioni tecniche dettagliate sui concetti e sui principi utilizzati nelle funzionalità di magazzino e costing in [!INCLUDE[d365fin](includes/d365fin_md.md)]."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: design, inventory, costing
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 1dfba8b14019991c95f40ffd5f7fbaed5df414eb
ms.openlocfilehash: 8403486a897a3031ad0f488b4eb7e415daa1b8a0
ms.contentlocale: it-it
ms.lasthandoff: 12/01/2017

---
# <a name="design-details-inventory-costing"></a><span data-ttu-id="f26d0-103">Dettagli di progettazione: Costing di magazzino</span><span class="sxs-lookup"><span data-stu-id="f26d0-103">Design Details: Inventory Costing</span></span>
<span data-ttu-id="f26d0-104">In questa documentazione sono fornite informazioni tecniche dettagliate sui concetti e sui principi utilizzati nelle funzionalità di magazzino e costing in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="f26d0-104">This documentation provides detailed technical insight to the concepts and principles that are used within the Inventory Costing features in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span>  

<span data-ttu-id="f26d0-105">Il costing di magazzino, detto anche gestione costing riguarda la registrazione e il reporting dei costi operativi business.</span><span class="sxs-lookup"><span data-stu-id="f26d0-105">Inventory costing, also referred to as cost management, is concerned with recording and reporting business operating costs.</span></span>  

## <a name="in-this-section"></a><span data-ttu-id="f26d0-106">In questa sezione</span><span class="sxs-lookup"><span data-stu-id="f26d0-106">In This Section</span></span>  
[<span data-ttu-id="f26d0-107">Dettagli di progettazione: Metodi di costing</span><span class="sxs-lookup"><span data-stu-id="f26d0-107">Design Details: Costing Methods</span></span>](design-details-costing-methods.md)  
[<span data-ttu-id="f26d0-108">Dettagli di progettazione: Collegamento articoli</span><span class="sxs-lookup"><span data-stu-id="f26d0-108">Design Details: Item Application</span></span>](design-details-item-application.md)  
[<span data-ttu-id="f26d0-109">Dettagli di progettazione: Rettifica costo</span><span class="sxs-lookup"><span data-stu-id="f26d0-109">Design Details: Cost Adjustment</span></span>](design-details-cost-adjustment.md)  
[<span data-ttu-id="f26d0-110">Dettagli di progettazione: Registrazione del costo previsto</span><span class="sxs-lookup"><span data-stu-id="f26d0-110">Design Details: Expected Cost Posting</span></span>](design-details-expected-cost-posting.md)  
[<span data-ttu-id="f26d0-111">Dettagli di progettazione: Costo medio</span><span class="sxs-lookup"><span data-stu-id="f26d0-111">Design Details: Average Cost</span></span>](design-details-average-cost.md)  
[<span data-ttu-id="f26d0-112">Dettagli di progettazione: Scostamento</span><span class="sxs-lookup"><span data-stu-id="f26d0-112">Design Details: Variance</span></span>](design-details-variance.md)  
[<span data-ttu-id="f26d0-113">Dettagli di progettazione: Arrotondamento</span><span class="sxs-lookup"><span data-stu-id="f26d0-113">Design Details: Rounding</span></span>](design-details-rounding.md)  
[<span data-ttu-id="f26d0-114">Dettagli di progettazione: Componenti costo</span><span class="sxs-lookup"><span data-stu-id="f26d0-114">Design Details: Cost Components</span></span>](design-details-cost-components.md)  
[<span data-ttu-id="f26d0-115">Dettagli di progettazione: Periodi di magazzino</span><span class="sxs-lookup"><span data-stu-id="f26d0-115">Design Details: Inventory Periods</span></span>](design-details-inventory-periods.md)  
[<span data-ttu-id="f26d0-116">Dettagli di progettazione: Registrazione di magazzino</span><span class="sxs-lookup"><span data-stu-id="f26d0-116">Design Details: Inventory Posting</span></span>](design-details-inventory-posting.md)  
[<span data-ttu-id="f26d0-117">Dettagli di progettazione: Registrazione dell'ordine di produzione</span><span class="sxs-lookup"><span data-stu-id="f26d0-117">Design Details: Production Order Posting</span></span>](design-details-production-order-posting.md)  
[<span data-ttu-id="f26d0-118">Dettagli di progettazione: Registrazione dell'ordine di assemblaggio</span><span class="sxs-lookup"><span data-stu-id="f26d0-118">Design Details: Assembly Order Posting</span></span>](design-details-assembly-order-posting.md)  
[<span data-ttu-id="f26d0-119">Dettagli di progettazione: Riconciliazione con la contabilità generale</span><span class="sxs-lookup"><span data-stu-id="f26d0-119">Design Details: Reconciliation with the General Ledger</span></span>](design-details-reconciliation-with-the-general-ledger.md)  
[<span data-ttu-id="f26d0-120">Dettagli di progettazione: Conti nella contabilità generale</span><span class="sxs-lookup"><span data-stu-id="f26d0-120">Design Details: Accounts in the General Ledger</span></span>](design-details-accounts-in-the-general-ledger.md)  
[<span data-ttu-id="f26d0-121">Dettagli di progettazione: Rivalutazione</span><span class="sxs-lookup"><span data-stu-id="f26d0-121">Design Details: Revaluation</span></span>](design-details-revaluation.md)

