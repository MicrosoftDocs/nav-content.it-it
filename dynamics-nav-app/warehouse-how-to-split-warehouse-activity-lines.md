---
title: "Come suddividere le righe attività di warehouse"
description: "Nei prelievi, nei movimenti o negli stoccaggi warehouse, nonché nei prelievi e negli stoccaggi magazzino, vengono forniti suggerimenti circa le collocazioni per il prelievo o lo stoccaggio di articoli. Nella collocazione suggerita la quantità effettiva può non essere sufficiente o non vi è abbastanza spazio per stoccare la quantità richiesta. In questi casi è necessario suddividere la riga in modo che gli articoli ad essa corrispondenti vengano prelevati da o posti in più collocazioni."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/16/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: d113b83d2c4d21463e1a015e7015bc1f566652f9
ms.contentlocale: it-it
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-split-warehouse-activity-lines"></a><span data-ttu-id="8302a-105">Procedura: Suddividere le righe attività warehouse</span><span class="sxs-lookup"><span data-stu-id="8302a-105">How to: Split Warehouse Activity Lines</span></span>
<span data-ttu-id="8302a-106">Nei prelievi, nei movimenti o negli stoccaggi warehouse, nonché nei prelievi e negli stoccaggi magazzino, vengono forniti suggerimenti circa le collocazioni per il prelievo o lo stoccaggio di articoli.</span><span class="sxs-lookup"><span data-stu-id="8302a-106">In warehouse put-aways, movements, or picks, and in inventory put-aways and inventory picks, bins are suggested for the picking or putting away of items.</span></span> <span data-ttu-id="8302a-107">Nella collocazione suggerita la quantità effettiva può non essere sufficiente o non vi è abbastanza spazio per stoccare la quantità richiesta.</span><span class="sxs-lookup"><span data-stu-id="8302a-107">The actual quantity in the bin suggested may not be sufficient, or there is not enough room in the suggested bin to put away the required quantity.</span></span> <span data-ttu-id="8302a-108">In questi casi è necessario suddividere la riga in modo che gli articoli ad essa corrispondenti vengano prelevati da o posti in più collocazioni.</span><span class="sxs-lookup"><span data-stu-id="8302a-108">In these cases, you need to split the line, so that the items for one line are either taken from or placed into more than one bin.</span></span>  

<span data-ttu-id="8302a-109">La seguente procedura si applica ai documenti warehouse, ad esempio stoccaggio warehouse, movimentazione e righe prelievo oppure stoccaggio magazzino, movimentazione e righe prelievo.</span><span class="sxs-lookup"><span data-stu-id="8302a-109">The following procedure applies to warehouse documents, such as warehouse put-away, movement, and pick lines, or inventory put-away, movement, and pick lines.</span></span>  

## <a name="to-split-warehouse-activity-lines"></a><span data-ttu-id="8302a-110">Per suddividere righe attività warehouse</span><span class="sxs-lookup"><span data-stu-id="8302a-110">To split warehouse activity lines</span></span>  
1.  <span data-ttu-id="8302a-111">Aprire una riga attività warehouse in cui si sta tentando di gestire una quantità insufficiente.</span><span class="sxs-lookup"><span data-stu-id="8302a-111">Open a warehouse activity line where you are trying to handle an insufficient quantity.</span></span>  
2.  <span data-ttu-id="8302a-112">Nel campo **Qtà da gestire** immettere la quantità ridotta che si è in grado di gestire.</span><span class="sxs-lookup"><span data-stu-id="8302a-112">In the **Qty. to Handle** field, enter the reduced quantity that you are able to handle.</span></span>  
3.  <span data-ttu-id="8302a-113">Nella Scheda dettaglio **Righe** scegliere le azioni **Azioni**, **Funzioni** e **Dividi riga**.</span><span class="sxs-lookup"><span data-stu-id="8302a-113">On the **Lines** FastTab, choose the **Actions** action, choose the **Functions** action, and then choose the **Split Line** action.</span></span> <span data-ttu-id="8302a-114">Verrà visualizzata una nuova riga, costituita da una copia di quella originale tranne per il fatto che il campo **Qtà da gestire** contiene il valore sottratto dalla riga originale.</span><span class="sxs-lookup"><span data-stu-id="8302a-114">A new line appears, which is a copy of the original line, except that the **Qty. to Handle** field contains the quantity that you removed from the original line.</span></span>  
4.  <span data-ttu-id="8302a-115">Assegnare una collocazione appropriata alla nuova riga, nonché una zona se si utilizzano stoccaggi e prelievi guidati, oppure continuare a suddividere la riga fino a quando non si trovano le collocazioni appropriate per gestire l'intera quantità.</span><span class="sxs-lookup"><span data-stu-id="8302a-115">Assign an appropriate bin and, if you are using directed put-away and pick, a zone, to this new line, or continue splitting the line as necessary until you find appropriate bins for all of the quantity.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="8302a-116">Se per l'ubicazione vengono utilizzati stoccaggi e prelievi guidati e si procede alla suddivisione delle righe, è necessario avere familiarità con la warehouse ed essere in grado di scegliere una collocazione che corrisponda ai requisiti di immagazzinamento dell'articolo e che soddisfi i requisiti generali del documento di warehouse.</span><span class="sxs-lookup"><span data-stu-id="8302a-116">If the location uses directed put-away and pick and you split the lines, you must be familiar with the warehouse and be able to choose a bin that matches the storage requirements of the item and that fulfills the general requirements of the warehouse document.</span></span> <span data-ttu-id="8302a-117">Ad esempio, non è consigliabile suddividere una riga in un documento di prelievo e posizionare alcuni articoli nell'area di immagazzinamento a massa.</span><span class="sxs-lookup"><span data-stu-id="8302a-117">For example, you would not split a line on a pick document and place some items in the bulk storage.</span></span>  

## <a name="see-also"></a><span data-ttu-id="8302a-118">Vedi anche</span><span class="sxs-lookup"><span data-stu-id="8302a-118">See Also</span></span>  
[<span data-ttu-id="8302a-119">Gestione warehouse</span><span class="sxs-lookup"><span data-stu-id="8302a-119">Warehouse Management</span></span>](warehouse-manage-warehouse.md)  
[<span data-ttu-id="8302a-120">Magazzino</span><span class="sxs-lookup"><span data-stu-id="8302a-120">Inventory</span></span>](inventory-manage-inventory.md)  
<span data-ttu-id="8302a-121">[Impostazione gestione warehouse](warehouse-setup-warehouse.md)   </span><span class="sxs-lookup"><span data-stu-id="8302a-121">[Setting Up Warehouse Management](warehouse-setup-warehouse.md)   </span></span>  
<span data-ttu-id="8302a-122">[Gestione assemblaggio](assembly-assemble-items.md)  </span><span class="sxs-lookup"><span data-stu-id="8302a-122">[Assembly Management](assembly-assemble-items.md)  </span></span>  
[<span data-ttu-id="8302a-123">Dettagli di progettazione: Gestione warehouse</span><span class="sxs-lookup"><span data-stu-id="8302a-123">Design Details: Warehouse Management</span></span>](design-details-warehouse-management.md)  
<span data-ttu-id="8302a-124">[Utilizzo di [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="8302a-124">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
