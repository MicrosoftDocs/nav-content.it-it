---
title: Dettagli di progettazione - Ricerca delle combinazioni di dimensione
description: Quando si chiude la finestra dopo avere modificato un set di dimensioni, in [!INCLUDE[d365fin](includes/d365fin_md.md)] viene valutato se il set di dimensioni modificato esiste. Se il set non esiste, viene creato un nuovo set e viene restituito l'ID combinazione delle dimensioni.
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
ms.openlocfilehash: 1e3bbad5d5f809068b88f6bbf5d0deaa22b38427
ms.contentlocale: it-it
ms.lasthandoff: 10/16/2017

---
# <a name="design-details-searching-for-dimension-combinations"></a><span data-ttu-id="22d2d-104">Dettagli di progettazione: Ricerca delle combinazioni di dimensione</span><span class="sxs-lookup"><span data-stu-id="22d2d-104">Design Details: Searching for Dimension Combinations</span></span>
<span data-ttu-id="22d2d-105">Quando si chiude la finestra dopo avere modificato un set di dimensioni, in [!INCLUDE[d365fin](includes/d365fin_md.md)] viene valutato se il set di dimensioni modificato esiste.</span><span class="sxs-lookup"><span data-stu-id="22d2d-105">When you close a window after you edit a set of dimensions, [!INCLUDE[d365fin](includes/d365fin_md.md)] evaluates whether the edited set of dimensions exists.</span></span> <span data-ttu-id="22d2d-106">Se il set non esiste, viene creato un nuovo set e viene restituito l'ID combinazione delle dimensioni.</span><span class="sxs-lookup"><span data-stu-id="22d2d-106">If the set does not exist, a new set is created and the dimension combination ID is returned.</span></span>  

## <a name="building-search-tree"></a><span data-ttu-id="22d2d-107">Creazione albero di ricerca</span><span class="sxs-lookup"><span data-stu-id="22d2d-107">Building Search Tree</span></span>  
 <span data-ttu-id="22d2d-108">La tabella 481 **Nodo albero set di dimensioni** viene utilizzata quando [!INCLUDE[d365fin](includes/d365fin_md.md)] valuta se un set di dimensioni esiste già nella tabella 480 **Voce set di dimensioni**.</span><span class="sxs-lookup"><span data-stu-id="22d2d-108">Table 481 **Dimension Set Tree Node** is used when [!INCLUDE[d365fin](includes/d365fin_md.md)] evaluates whether a set of dimensions already exists in table 480 **Dimension Set Entry** table.</span></span> <span data-ttu-id="22d2d-109">La valutazione viene eseguita in modo ricorsivo lungo l'albero di ricerca a partire dal livello massimo con numero 0.</span><span class="sxs-lookup"><span data-stu-id="22d2d-109">The evaluation is performed by recursively traversing the search tree starting at the top level numbered 0.</span></span> <span data-ttu-id="22d2d-110">Il livello massimo 0 rappresenta un set di dimensioni senza movimenti di set di dimensioni.</span><span class="sxs-lookup"><span data-stu-id="22d2d-110">The top level 0 represents a dimension set with no dimension set entries.</span></span> <span data-ttu-id="22d2d-111">I figli di questo set di dimensioni rappresentano i set di dimensioni con un solo movimento set di dimensioni.</span><span class="sxs-lookup"><span data-stu-id="22d2d-111">The children of this dimension set represent dimension sets with only one dimension set entry.</span></span> <span data-ttu-id="22d2d-112">I figli di questi set di dimensioni rappresentano i set di dimensioni con due elementi figlio e così via.</span><span class="sxs-lookup"><span data-stu-id="22d2d-112">The children of these dimension sets represent dimension sets with two children, and so on.</span></span>  

### <a name="example-1"></a><span data-ttu-id="22d2d-113">Esempio 1</span><span class="sxs-lookup"><span data-stu-id="22d2d-113">Example 1</span></span>  
 <span data-ttu-id="22d2d-114">Nel seguente diagramma viene rappresentato un albero di ricerca con sei set di dimensioni.</span><span class="sxs-lookup"><span data-stu-id="22d2d-114">The following diagram represents a search tree with six dimension sets.</span></span> <span data-ttu-id="22d2d-115">Solo il movimento set di dimensioni distintivo viene visualizzato nel grafico.</span><span class="sxs-lookup"><span data-stu-id="22d2d-115">Only the distinguishing dimension set entry is displayed in the diagram.</span></span>  

 <span data-ttu-id="22d2d-116">![Struttura ad albero dimensioni](media/nav2013_dimension_tree.png "NAV2013_Dimension_Tree")</span><span class="sxs-lookup"><span data-stu-id="22d2d-116">![Dimension tree structure](media/nav2013_dimension_tree.png "NAV2013_Dimension_Tree")</span></span>  

 <span data-ttu-id="22d2d-117">Nella tabella seguente viene descritto un elenco di movimenti set di dimensioni che costituiscono ogni set di dimensioni.</span><span class="sxs-lookup"><span data-stu-id="22d2d-117">The following table describes a complete list of dimension set entries that make up each dimension set.</span></span>  

|<span data-ttu-id="22d2d-118">Set di dimensioni</span><span class="sxs-lookup"><span data-stu-id="22d2d-118">Dimension Sets</span></span>|<span data-ttu-id="22d2d-119">Movimenti set di dimensioni</span><span class="sxs-lookup"><span data-stu-id="22d2d-119">Dimension Set Entries</span></span>|  
|--------------------|---------------------------|  
|<span data-ttu-id="22d2d-120">Set 0</span><span class="sxs-lookup"><span data-stu-id="22d2d-120">Set 0</span></span>|<span data-ttu-id="22d2d-121">Nessuno</span><span class="sxs-lookup"><span data-stu-id="22d2d-121">None</span></span>|  
|<span data-ttu-id="22d2d-122">Set 1</span><span class="sxs-lookup"><span data-stu-id="22d2d-122">Set 1</span></span>|<span data-ttu-id="22d2d-123">AREA 30</span><span class="sxs-lookup"><span data-stu-id="22d2d-123">AREA 30</span></span>|  
|<span data-ttu-id="22d2d-124">Set 2</span><span class="sxs-lookup"><span data-stu-id="22d2d-124">Set 2</span></span>|<span data-ttu-id="22d2d-125">AREA 30, REPARTO ADM</span><span class="sxs-lookup"><span data-stu-id="22d2d-125">AREA 30, DEPT ADM</span></span>|  
|<span data-ttu-id="22d2d-126">Set 3</span><span class="sxs-lookup"><span data-stu-id="22d2d-126">Set 3</span></span>|<span data-ttu-id="22d2d-127">AREA 30, REPARTO PROD</span><span class="sxs-lookup"><span data-stu-id="22d2d-127">AREA 30, DEPT PROD</span></span>|  
|<span data-ttu-id="22d2d-128">Set 4</span><span class="sxs-lookup"><span data-stu-id="22d2d-128">Set 4</span></span>|<span data-ttu-id="22d2d-129">AREA 30, REPARTO ADM, PROJ VW</span><span class="sxs-lookup"><span data-stu-id="22d2d-129">AREA 30, DEPT ADM, PROJ VW</span></span>|  
|<span data-ttu-id="22d2d-130">Set 5</span><span class="sxs-lookup"><span data-stu-id="22d2d-130">Set 5</span></span>|<span data-ttu-id="22d2d-131">AREA 40</span><span class="sxs-lookup"><span data-stu-id="22d2d-131">AREA 40</span></span>|  
|<span data-ttu-id="22d2d-132">Set 6</span><span class="sxs-lookup"><span data-stu-id="22d2d-132">Set 6</span></span>|<span data-ttu-id="22d2d-133">AREA 40, PROJ VW</span><span class="sxs-lookup"><span data-stu-id="22d2d-133">AREA 40, PROJ VW</span></span>|  

### <a name="example-2"></a><span data-ttu-id="22d2d-134">Esempio 2</span><span class="sxs-lookup"><span data-stu-id="22d2d-134">Example 2</span></span>  
 <span data-ttu-id="22d2d-135">In questo esempio viene mostrato in che modo [!INCLUDE[d365fin](includes/d365fin_md.md)] valuta se è presente un set di dimensioni costituito da movimenti di set di dimensioni AREA 40, DEPT PROD.</span><span class="sxs-lookup"><span data-stu-id="22d2d-135">This example shows how [!INCLUDE[d365fin](includes/d365fin_md.md)] evaluates whether a dimension set that consists of the dimension set entries AREA 40, DEPT PROD exists.</span></span>  

 <span data-ttu-id="22d2d-136">[!INCLUDE[d365fin](includes/d365fin_md.md)] aggiorna prima di tutto anche la tabella **Nodo albero set di dimensioni** per assicurarsi che l'albero di ricerca somigli al diagramma seguente.</span><span class="sxs-lookup"><span data-stu-id="22d2d-136">First, [!INCLUDE[d365fin](includes/d365fin_md.md)] also updates the **Dimension Set Tree Node** table to make sure that the search tree looks like the following diagram.</span></span> <span data-ttu-id="22d2d-137">Pertanto il set di dimensioni 7 diventa un figlio del set di dimensioni 5.</span><span class="sxs-lookup"><span data-stu-id="22d2d-137">Thus dimension set 7 becomes a child of the dimension set 5.</span></span>  

 <span data-ttu-id="22d2d-138">![NAV2013&#95;Dimension&#95;Tree&#95;Example 2](media/nav2013_dimension_tree_example2.png "NAV2013_Dimension_Tree_Example2")</span><span class="sxs-lookup"><span data-stu-id="22d2d-138">![NAV2013&#95;Dimension&#95;Tree&#95;Example 2](media/nav2013_dimension_tree_example2.png "NAV2013_Dimension_Tree_Example2")</span></span>  

### <a name="finding-dimension-set-id"></a><span data-ttu-id="22d2d-139">Ricerca ID set di dimensioni</span><span class="sxs-lookup"><span data-stu-id="22d2d-139">Finding Dimension Set ID</span></span>  
 <span data-ttu-id="22d2d-140">A livello concettuale, i valori **ID padre**, **Dimensione** e **Valore dimensioni**, nell'albero di ricerca vengono combinati e utilizzati come chiave primaria perché [!INCLUDE[d365fin](includes/d365fin_md.md)] attraversa la struttura ad albero nello stesso ordine dei movimenti con dimensione.</span><span class="sxs-lookup"><span data-stu-id="22d2d-140">At a conceptual level, **Parent ID**, **Dimension**, and **Dimension Value**, in the search tree, are combined and used as the primary key because [!INCLUDE[d365fin](includes/d365fin_md.md)] traverses the tree in the same order as the dimension entries.</span></span> <span data-ttu-id="22d2d-141">La funzione Get (record) viene utilizzata per cercare l'ID set di dimensioni.</span><span class="sxs-lookup"><span data-stu-id="22d2d-141">The GET function (record) is used to search for dimension set ID.</span></span> <span data-ttu-id="22d2d-142">Nell'esempio di codice riportato di seguito viene illustrato come trovare l'ID set di dimensioni quando sono presenti tre valori di dimensione.</span><span class="sxs-lookup"><span data-stu-id="22d2d-142">The following code example shows how to find the dimension set ID when there are three dimension values.</span></span>  

```  
DimSet."Parent ID" := 0;  // 'root'  
IF UserDim.FINDSET THEN  
  REPEAT  
      DimSet.GET(DimSet."Parent ID",UserDim.DimCode,UserDim.DimValueCode);  
  UNTIL UserDim.NEXT = 0;  
EXIT(DimSet.ID);  

```  

 <span data-ttu-id="22d2d-143">Tuttavia, per mantenere la capacità di [!INCLUDE[d365fin](includes/d365fin_md.md)] di rinominare una dimensione e un valore di dimensione, la tabella 348 **Valore dimensioni** viene estesa con un campo di numero intero di **ID valore dimensioni**.</span><span class="sxs-lookup"><span data-stu-id="22d2d-143">However, to preserve the ability of [!INCLUDE[d365fin](includes/d365fin_md.md)] to rename a dimension and dimension value, table 348 **Dimension Value** is extended with an integer field of **Dimension Value ID**.</span></span> <span data-ttu-id="22d2d-144">Questa tabella converte la coppia di campi **Dimensione** e **Valore dimensioni** in un valore intero.</span><span class="sxs-lookup"><span data-stu-id="22d2d-144">This table converts the field pair **Dimension** and **Dimension Value** to an integer value.</span></span> <span data-ttu-id="22d2d-145">Quando si rinominano la dimensione e il valore di dimensione, il valore intero non viene modificato.</span><span class="sxs-lookup"><span data-stu-id="22d2d-145">When you rename the dimension and dimension value, the integer value is not changed.</span></span>  

```  
DimSet."Parent ID" := 0;  // 'root'  
IF UserDim.FINDSET THEN  
  REPEAT  
      DimSet.GET(DimSet.ParentID,UserDim."Dimension Value ID");  
  UNTIL UserDim.NEXT = 0;  
EXIT(DimSet.ID);  

```  

## <a name="see-also"></a><span data-ttu-id="22d2d-146">Vedi anche</span><span class="sxs-lookup"><span data-stu-id="22d2d-146">See Also</span></span>  
 <span data-ttu-id="22d2d-147">[Funzione GET (Record)](https://msdn.microsoft.com/en-us/library/dd301056.aspx)  </span><span class="sxs-lookup"><span data-stu-id="22d2d-147">[GET Function (Record)](https://msdn.microsoft.com/en-us/library/dd301056.aspx)  </span></span>  
 <span data-ttu-id="22d2d-148">[Dettagli di progettazione: Movimenti set di dimensioni](design-details-dimension-set-entries.md) </span><span class="sxs-lookup"><span data-stu-id="22d2d-148">[Design Details: Dimension Set Entries](design-details-dimension-set-entries.md) </span></span>  
 <span data-ttu-id="22d2d-149">[Sintesi movimenti set di dimensioni](design-details-dimension-set-entries-overview.md) </span><span class="sxs-lookup"><span data-stu-id="22d2d-149">[Dimension Set Entries Overview](design-details-dimension-set-entries-overview.md) </span></span>  
 <span data-ttu-id="22d2d-150">[Dettagli di progettazione: Struttura della tabella](design-details-table-structure.md) </span><span class="sxs-lookup"><span data-stu-id="22d2d-150">[Design Details: Table Structure](design-details-table-structure.md) </span></span>  
 <span data-ttu-id="22d2d-151">[Dettagli di progettazione: Gestione dimensioni della codeunit 408](design-details-codeunit-408-dimension-management.md) </span><span class="sxs-lookup"><span data-stu-id="22d2d-151">[Design Details: Codeunit 408 Dimension Management](design-details-codeunit-408-dimension-management.md) </span></span>  
 [<span data-ttu-id="22d2d-152">Dettagli di progettazione: Esempi di codice dei modelli modificati nelle modifiche</span><span class="sxs-lookup"><span data-stu-id="22d2d-152">Design Details: Code Examples of Changed Patterns in Modifications</span></span>](design-details-code-examples-of-changed-patterns-in-modifications.md)
