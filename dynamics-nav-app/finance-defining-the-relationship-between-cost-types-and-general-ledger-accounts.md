---
title: "Definizione della relazione tra i tipi di costo e i conti di contabilità generale"
description: "Informazioni su come definire la relazione tra il tipo di costo e il conto di contabilità generale."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: cost types, general ledger
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 6bedd251aad7f15f40a255e5b44c6080bbb73bdb
ms.contentlocale: it-it
ms.lasthandoff: 10/16/2017

---
# <a name="defining-the-relationship-between-cost-types-and-general-ledger-accounts"></a><span data-ttu-id="c4f0f-103">Definizione della relazione tra i tipi di costo e i conti di contabilità generale</span><span class="sxs-lookup"><span data-stu-id="c4f0f-103">Defining the Relationship Between Cost Types and General Ledger Accounts</span></span>
<span data-ttu-id="c4f0f-104">La relazione tra il tipo di costo e il conto di contabilità generale viene creata nel tipo di costo e nel conto di contabilità generale.</span><span class="sxs-lookup"><span data-stu-id="c4f0f-104">The relationship between the cost type and the general ledger account is created in the cost type and in the general ledger account.</span></span>  

* <span data-ttu-id="c4f0f-105">Tramite il campo **Intervallo conti CG** della tabella **Tipo costo** è possibile stabilire quali conti di contabilità generale appartengono a un tipo di costo.</span><span class="sxs-lookup"><span data-stu-id="c4f0f-105">The **G/L Account Range** field in the **Cost Type** table establishes which general ledger accounts belong to a cost type.</span></span>  
* <span data-ttu-id="c4f0f-106">Con il campo **Nr. tipo di costo**</span><span class="sxs-lookup"><span data-stu-id="c4f0f-106">The **Cost Type No.**</span></span> <span data-ttu-id="c4f0f-107">nel piano dei conti è possibile stabilire il tipo di costo a cui appartiene un conto di contabilità generale.</span><span class="sxs-lookup"><span data-stu-id="c4f0f-107">field in the chart of accounts establishes which cost type a general ledger account belongs to.</span></span>  

<span data-ttu-id="c4f0f-108">Questi due campi vengono compilati automaticamente quando si utilizza la funzione **Ottieni tipi costo da piano dei conti**.</span><span class="sxs-lookup"><span data-stu-id="c4f0f-108">These two fields are filled automatically when you use the **Get Cost Types from Chart of Accounts** function.</span></span>  

## <a name="relationship-between-general-ledger-accounts-and-cost-types"></a><span data-ttu-id="c4f0f-109">Relazione tra i conti di contabilità generale e i tipi di costo</span><span class="sxs-lookup"><span data-stu-id="c4f0f-109">Relationship Between General Ledger Accounts and Cost Types</span></span>  
<span data-ttu-id="c4f0f-110">Tra i conti di contabilità generale e i tipi di costo esiste una relazione n:1.</span><span class="sxs-lookup"><span data-stu-id="c4f0f-110">There is an n:1 relationship between general ledger accounts and cost types.</span></span> <span data-ttu-id="c4f0f-111">A un tipo di costo possono appartenere più conti di contabilità generale, ma ognuno di questi appartiene a un solo tipo di costo.</span><span class="sxs-lookup"><span data-stu-id="c4f0f-111">Several general ledger accounts can belong to one cost type, but each general ledger account belongs to only one cost type.</span></span> <span data-ttu-id="c4f0f-112">Nella seguente tabella vengono descritti i dettagli delle relazioni.</span><span class="sxs-lookup"><span data-stu-id="c4f0f-112">The following table describes the details in the relationship.</span></span>  

|<span data-ttu-id="c4f0f-113">Relazione</span><span class="sxs-lookup"><span data-stu-id="c4f0f-113">Relationship</span></span>|<span data-ttu-id="c4f0f-114">**Intervallo conti C/G**</span><span class="sxs-lookup"><span data-stu-id="c4f0f-114">**G/L Account Range**</span></span>|<span data-ttu-id="c4f0f-115">**Nr. tipo di costo**</span><span class="sxs-lookup"><span data-stu-id="c4f0f-115">**Cost Type No.**</span></span>|  
|------------------|------------------------------------------------|-------------------------------------------|  
|<span data-ttu-id="c4f0f-116">Un conto di contabilità generale per ogni tipo di costo</span><span class="sxs-lookup"><span data-stu-id="c4f0f-116">One general ledger account for each cost type</span></span>|<span data-ttu-id="c4f0f-117">Un conto di contabilità generale</span><span class="sxs-lookup"><span data-stu-id="c4f0f-117">One general ledger account</span></span>|<span data-ttu-id="c4f0f-118">Un tipo di costo</span><span class="sxs-lookup"><span data-stu-id="c4f0f-118">One cost type</span></span>|  
|<span data-ttu-id="c4f0f-119">Più conti di contabilità generale per un tipo di costo</span><span class="sxs-lookup"><span data-stu-id="c4f0f-119">Several general ledger accounts for one cost type</span></span>|<span data-ttu-id="c4f0f-120">Intervallo di conti di contabilità generale, ad esempio da 7110 a 7193, per ciascun conto di contabilità generale</span><span class="sxs-lookup"><span data-stu-id="c4f0f-120">General ledger account range, for example, 7110..7193 for each general ledger account</span></span>|<span data-ttu-id="c4f0f-121">Per ciascun conto di contabilità generale nell'intervallo, esiste un solo tipo di costo</span><span class="sxs-lookup"><span data-stu-id="c4f0f-121">For each general ledger account in the range, there is only one cost type</span></span>|  
|<span data-ttu-id="c4f0f-122">Tipi di costo senza conti di contabilità generale corrispondenti</span><span class="sxs-lookup"><span data-stu-id="c4f0f-122">Cost types without corresponding general ledger accounts</span></span>|<Empty>||  
|<span data-ttu-id="c4f0f-123">Conti di contabilità generale i cui movimenti non saranno trasferiti</span><span class="sxs-lookup"><span data-stu-id="c4f0f-123">General ledger accounts whose entries will not be transferred</span></span>||<Empty>|  

## <a name="cost-types-without-a-relationship-to-the-general-ledger"></a><span data-ttu-id="c4f0f-124">Tipi di costo senza una relazione con la contabilità generale</span><span class="sxs-lookup"><span data-stu-id="c4f0f-124">Cost Types Without a Relationship to the General Ledger</span></span>  
<span data-ttu-id="c4f0f-125">Un tipo di costo non può avere una relazione con i conti di contabilità generale se una delle seguenti condizioni è vera:</span><span class="sxs-lookup"><span data-stu-id="c4f0f-125">A cost type may not have a relationship to general ledger accounts if one of the following conditions is true:</span></span>  

* <span data-ttu-id="c4f0f-126">I conti per la contabilità operativa, ad esempio il calcolo interessi e l'ammortamento, vengono ricavati solo dalla contabilità operativa.</span><span class="sxs-lookup"><span data-stu-id="c4f0f-126">Accounts for operational accounting, such as Calc. Interest and Depreciation, only take costs from the operational accounting.</span></span>  
* <span data-ttu-id="c4f0f-127">I tipi di costo di supporto, ad esempio i tipi 9901, 9902 e 9903 nel database di [!INCLUDE[d365fin](includes/d365fin_md.md)], vengono utilizzati come dare e avere per le allocazioni.</span><span class="sxs-lookup"><span data-stu-id="c4f0f-127">Helping cost types, such as cost types 9901, 9902, and 9903 in the [!INCLUDE[d365fin](includes/d365fin_md.md)] database, are used as credit and debit accounts for allocations.</span></span>  
* <span data-ttu-id="c4f0f-128">Il conto di supporto, 9920 nel database di [!INCLUDE[d365fin](includes/d365fin_md.md)], contiene i ratei effettivi che mostrano la differenza tra i costi e le spese della contabilità generale.</span><span class="sxs-lookup"><span data-stu-id="c4f0f-128">The helping account, 9920 in the [!INCLUDE[d365fin](includes/d365fin_md.md)] database, contains actual accruals that show the difference between costs and the expense from the general ledger.</span></span>  

## <a name="see-also"></a><span data-ttu-id="c4f0f-129">Vedi anche</span><span class="sxs-lookup"><span data-stu-id="c4f0f-129">See Also</span></span>  
[<span data-ttu-id="c4f0f-130">Contabilizzazione dei costi</span><span class="sxs-lookup"><span data-stu-id="c4f0f-130">Accounting for Costs</span></span>](finance-manage-cost-accounting.md)  
<span data-ttu-id="c4f0f-131">[Impostazione della contabilità industriale](finance-set-up-cost-accounting.md) </span><span class="sxs-lookup"><span data-stu-id="c4f0f-131">[Setting Up Cost Accounting](finance-set-up-cost-accounting.md) </span></span>  
[<span data-ttu-id="c4f0f-132">Informazioni sulla contabilità industriale</span><span class="sxs-lookup"><span data-stu-id="c4f0f-132">About Cost Accounting</span></span>](finance-about-cost-accounting.md)  
<span data-ttu-id="c4f0f-133">[Utilizzo di [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="c4f0f-133">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
