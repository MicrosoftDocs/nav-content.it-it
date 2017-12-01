---
title: Valutazione magazzino fiscale
description: "È necessario inviare un report annuale che indichi il valore monetario degli articoli di magazzino per l'anno fiscale."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 1dfba8b14019991c95f40ffd5f7fbaed5df414eb
ms.openlocfilehash: bbceb4d57981b4c5ce213eadf8381294f21065e1
ms.contentlocale: it-it
ms.lasthandoff: 12/01/2017

---
# <a name="fiscal-inventory-valuation"></a><span data-ttu-id="77503-103">Valutazione magazzino fiscale</span><span class="sxs-lookup"><span data-stu-id="77503-103">Fiscal Inventory Valuation</span></span>
<span data-ttu-id="77503-104">È necessario inviare un report annuale che indichi il valore monetario degli articoli di magazzino per l'anno fiscale.</span><span class="sxs-lookup"><span data-stu-id="77503-104">You must submit an annual report that shows the monetary value of inventory items for the fiscal year.</span></span> <span data-ttu-id="77503-105">A seconda dei requisiti italiani per la valutazione del magazzino fiscale, è necessario calcolare i seguenti tipi di costi:</span><span class="sxs-lookup"><span data-stu-id="77503-105">According to the Italian requirements for fiscal inventory valuation, you must calculate the following cost types:</span></span>  

- <span data-ttu-id="77503-106">Costo medio annuale</span><span class="sxs-lookup"><span data-stu-id="77503-106">Year average cost</span></span>  
- <span data-ttu-id="77503-107">Costo medio ponderato</span><span class="sxs-lookup"><span data-stu-id="77503-107">Weighted average cost</span></span>  
- <span data-ttu-id="77503-108">Costo FIFO (First-In-First-Out)</span><span class="sxs-lookup"><span data-stu-id="77503-108">First in, First Out (FIFO) cost</span></span>  
- <span data-ttu-id="77503-109">Costo LIFO (Last-In-First-Out)</span><span class="sxs-lookup"><span data-stu-id="77503-109">Last in, First Out (LIFO) cost</span></span>  
- <span data-ttu-id="77503-110">Costo LIFO discreto</span><span class="sxs-lookup"><span data-stu-id="77503-110">Discrete LIFO cost</span></span>  

## <a name="fiscal-inventory-valuation-in-includenavnowincludesnavnowmdmd"></a><span data-ttu-id="77503-111">Valutazione magazzino fiscale in [!INCLUDE[navnow](../../includes/navnow_md.md)]</span><span class="sxs-lookup"><span data-stu-id="77503-111">Fiscal Inventory Valuation in [!INCLUDE[navnow](../../includes/navnow_md.md)]</span></span>  
<span data-ttu-id="77503-112">Inizialmente, è necessario impostare la valutazione magazzino fiscale per tutti i tipi di costo nella finestra **Setup costing articolo** e nella finestra **Scheda articolo**.</span><span class="sxs-lookup"><span data-stu-id="77503-112">Initially, you must set up the fiscal inventory valuation for all cost types in the **Item Costing Setup** window and the **Item Card** window.</span></span> <span data-ttu-id="77503-113">Per ulteriori informazioni, vedere [Procedura: Impostare la valutazione magazzino fiscale](how-to-set-up-fiscal-inventory-valuation.md).</span><span class="sxs-lookup"><span data-stu-id="77503-113">For more information, see [How to: Set Up Fiscal Inventory Valuation](how-to-set-up-fiscal-inventory-valuation.md).</span></span>  

<span data-ttu-id="77503-114">Quando si imposta [!INCLUDE[navnow](../../includes/navnow_md.md)], è necessario immettere i movimenti contabili del magazzino per il primo anno per calcolare la valutazione dell'articolo.</span><span class="sxs-lookup"><span data-stu-id="77503-114">When you set up [!INCLUDE[navnow](../../includes/navnow_md.md)], you must enter the inventory item ledger entries for the first year in order to calculate the item’s valuation.</span></span> <span data-ttu-id="77503-115">È possibile effettuare questa operazione nella finestra Costo articolo prima dell'inizio.</span><span class="sxs-lookup"><span data-stu-id="77503-115">You can do this in the Before Start Item Cost window.</span></span>  

<span data-ttu-id="77503-116">Per calcolare il costo LIFO discreto, è necessario impostare le informazioni nella finestra **Scheda articolo** e nella finestra **Prezzi Conto Lavoro**.</span><span class="sxs-lookup"><span data-stu-id="77503-116">To calculate discrete LIFO cost, you must set up information in the **Item Card** window and the **Subcontracting Prices** window.</span></span>

> [!NOTE]  
>  <span data-ttu-id="77503-117">Il costo LIFO discreto può essere calcolato solo per gli articoli per i quali il campo **Valutazione magazzino** è impostato su **LIFO discreto** nella finestra **Scheda articolo**.</span><span class="sxs-lookup"><span data-stu-id="77503-117">The discrete LIFO cost can only be calculated for items for which the **Inventory Valuation** field is set to **Discrete LIFO** in the **Item Card** window.</span></span>

<span data-ttu-id="77503-118">Dopo aver impostato il calcolo del costo LIFO discreto, è possibile registrare le transazioni di vendita e acquisto basate sui costi di fine anno.</span><span class="sxs-lookup"><span data-stu-id="77503-118">After you set up the discrete LIFO cost calculation, you can post sales and purchase transactions based on year-end costs.</span></span>  

## <a name="end-of-year"></a><span data-ttu-id="77503-119">Fine anno</span><span class="sxs-lookup"><span data-stu-id="77503-119">End of Year</span></span>  
 <span data-ttu-id="77503-120">Alla fine dell'anno fiscale, è possibile eseguire il processo batch Calcola costi fine anno per calcolare il valore del magazzino fiscale di ogni articolo di magazzino in base ai metodi di valutazione richiesti.</span><span class="sxs-lookup"><span data-stu-id="77503-120">At the end of the fiscal year, you can run the Calculate End Year Costs batch job to calculate the fiscal inventory value of each inventory item according to the required valuation methods.</span></span> <span data-ttu-id="77503-121">I risultati sono visualizzati nella finestra Lista storico costo articolo.</span><span class="sxs-lookup"><span data-stu-id="77503-121">The results are shown in the Item Cost History List window.</span></span> <span data-ttu-id="77503-122">Quindi, è possibile eseguire il report **Valutazione fiscale magazzino** e il report **Valutazione LIFO** per visualizzare la valutazione del magazzino.</span><span class="sxs-lookup"><span data-stu-id="77503-122">Then, you can run the **Fiscal Inventory Valuation** report and the **LIFO Valuation** report to show the inventory valuation.</span></span>  

 <span data-ttu-id="77503-123">Per le operazioni di fine anno, come il calcolo di profitti e delle perdite in un anno fiscale, esiste un periodo definitivo e un periodo non definitivo.</span><span class="sxs-lookup"><span data-stu-id="77503-123">For year-end operations, such as calculating the profit and loss during a fiscal year, there is a definitive period and a non-definitive period.</span></span> <span data-ttu-id="77503-124">Se il campo **Anno di competenza** della finestra **Lista storico costo articolo** è uguale alla data di fine dell'anno fiscale, è un periodo definitivo e non è possibile ricalcolare i dati per un periodo definitivo.</span><span class="sxs-lookup"><span data-stu-id="77503-124">If the **Competence Year** field in the **Item Cost History List** window is equal to the fiscal year end date, it is a definitive period, and you cannot recalculate data for a definitive period.</span></span> <span data-ttu-id="77503-125">Se i dati definitivi differiscono dalla data di fine dell'anno fiscale, si tratta di un periodo non definitivo.</span><span class="sxs-lookup"><span data-stu-id="77503-125">If the definitive data differs from the fiscal year end date, then it is a non-definitive period.</span></span> <span data-ttu-id="77503-126">Per eseguire calcoli o calcoli parziali è necessario disporre dei dati relativi ad almeno un periodo non definitivo.</span><span class="sxs-lookup"><span data-stu-id="77503-126">There should be data for at least one non-definitive period to perform calculations or partial calculations.</span></span>

## <a name="see-also"></a><span data-ttu-id="77503-127">Vedi anche</span><span class="sxs-lookup"><span data-stu-id="77503-127">See Also</span></span>  
 <span data-ttu-id="77503-128">[Funzionalità locale per l'Italia](italy-local-functionality.md) </span><span class="sxs-lookup"><span data-stu-id="77503-128">[Italy Local Functionality](italy-local-functionality.md) </span></span>  
 <span data-ttu-id="77503-129">[Procedura: Impostare la valutazione magazzino fiscale](how-to-set-up-fiscal-inventory-valuation.md) </span><span class="sxs-lookup"><span data-stu-id="77503-129">[How to: Set Up Fiscal Inventory Valuation](how-to-set-up-fiscal-inventory-valuation.md) </span></span>  
 [<span data-ttu-id="77503-130">Procedura: Impostare i costi iniziali per gli articoli</span><span class="sxs-lookup"><span data-stu-id="77503-130">How to: Set Up Initial Item Costs</span></span>](how-to-set-up-initial-item-costs.md)

