---
title: Come utilizzare famiglie di articoli nella produzione
description: "L'operazione principale da eseguire per personalizzare un calendario di base per la propria società, o per uno dei partner commerciali, è la modifica dello stato dei giorni lavorativi e non lavorativi."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 09/05/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 4ad54585baef119db06bf69476739174af1209bb
ms.contentlocale: it-it
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-work-with-production-families"></a><span data-ttu-id="b2c75-103">Procedura: Utilizzare famiglie di prodotti</span><span class="sxs-lookup"><span data-stu-id="b2c75-103">How to: Work with Production Families</span></span>
<span data-ttu-id="b2c75-104">Una famiglia di prodotti consiste in un gruppo di articoli individuali la cui relazione si basa sulla similarità dei rispettivi processi di lavorazione.</span><span class="sxs-lookup"><span data-stu-id="b2c75-104">A production family is a group of individual items whose relationship is based on the similarity of their manufacturing processes.</span></span> <span data-ttu-id="b2c75-105">Formando delle famiglie di produzione, è possibile che alcuni articoli siano lavorati due o più volte nel corso di una produzione; questa operazione ottimizzerà il consumo di materiale.</span><span class="sxs-lookup"><span data-stu-id="b2c75-105">By forming production families, some items can be manufactured twice or more in one production, which will optimize material consumption.</span></span>

<span data-ttu-id="b2c75-106">Nel campo **Quantità** della finestra **Famiglie di prodotti**, immettere la quantità che sarà prodotta quando l'intera famiglia sarà stata lavorata una volta.</span><span class="sxs-lookup"><span data-stu-id="b2c75-106">In the **Quantity** field in the **Family** window, you enter the quantity that will be produced when the whole family has been manufactured once.</span></span>

## <a name="example"></a><span data-ttu-id="b2c75-107">Esempio</span><span class="sxs-lookup"><span data-stu-id="b2c75-107">Example</span></span>
<span data-ttu-id="b2c75-108">Nei processi di perforazione, è possibile che da una lamina vengano prodotti contemporaneamente quattro pezzi di un articolo e 10 pezzi di un altro articolo differente.</span><span class="sxs-lookup"><span data-stu-id="b2c75-108">In punching processes, four pieces of the same item can be produced from one sheet and 10 pieces of another, different, item at the same time.</span></span> <span data-ttu-id="b2c75-109">La perforatrice perforerà tutti i 14 pezzi in un'unica fase.</span><span class="sxs-lookup"><span data-stu-id="b2c75-109">The punching machine will punch all 14 pieces in one step.</span></span>

<span data-ttu-id="b2c75-110">La creazione di famiglie di produzione riduce le quantità di scarto perché ciò che generalmente costituisce gli scarti rimanenti dalla produzione di pezzi di grandi dimensioni viene utilizzato per produrre i pezzi di piccole dimensioni.</span><span class="sxs-lookup"><span data-stu-id="b2c75-110">Forming production families reduces the scrap quantity because what would normally be leftover scrap, when producing big pieces, will be used instead to produce small items.</span></span>

## <a name="to-set-up-a-production-family"></a><span data-ttu-id="b2c75-111">Per impostare una famiglia di prodotti</span><span class="sxs-lookup"><span data-stu-id="b2c75-111">To set up a production family</span></span>
1. <span data-ttu-id="b2c75-112">Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **Famiglie di prodotti**, quindi scegliere il collegamento correlato.</span><span class="sxs-lookup"><span data-stu-id="b2c75-112">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Families**, and then choose the related link.</span></span>
2. <span data-ttu-id="b2c75-113">Compilare i campi come necessario.</span><span class="sxs-lookup"><span data-stu-id="b2c75-113">Fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

## <a name="to-produce-based-on-a-production-familily"></a><span data-ttu-id="b2c75-114">Per produrre in base a una famiglia di prodotti</span><span class="sxs-lookup"><span data-stu-id="b2c75-114">To produce based on a production familily</span></span>
1. <span data-ttu-id="b2c75-115">Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **Ord. produzione confermato**, quindi scegliere il collegamento correlato.</span><span class="sxs-lookup"><span data-stu-id="b2c75-115">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Firm Planned Prod. Orders**, and then choose the related link.</span></span>
2. <span data-ttu-id="b2c75-116">Creare un nuovo ordine di produzione.</span><span class="sxs-lookup"><span data-stu-id="b2c75-116">Create a new production order.</span></span> <span data-ttu-id="b2c75-117">Per ulteriori informazioni, vedere [Procedura: Creare ordini di produzione](production-how-to-create-production-orders.md).</span><span class="sxs-lookup"><span data-stu-id="b2c75-117">For more information, see [How to: Create Production orders](production-how-to-create-production-orders.md).</span></span>
3. <span data-ttu-id="b2c75-118">Nel campo **Tipo origine**, selezionare **Famiglie di prodotti**.</span><span class="sxs-lookup"><span data-stu-id="b2c75-118">In the **Source Type** field, select **Family**.</span></span>  
4. <span data-ttu-id="b2c75-119">Nel campo **Nr. risorsa**, selezionare la famiglia di prodotti pertinente.</span><span class="sxs-lookup"><span data-stu-id="b2c75-119">In the **Source No.** field, select the relevant production family.</span></span>

## <a name="see-also"></a><span data-ttu-id="b2c75-120">Vedi anche</span><span class="sxs-lookup"><span data-stu-id="b2c75-120">See Also</span></span>
[<span data-ttu-id="b2c75-121">Procedura: Creare distinte base di produzione</span><span class="sxs-lookup"><span data-stu-id="b2c75-121">How to: Create Production BOMs</span></span>](production-how-to-create-production-boms.md)  
[<span data-ttu-id="b2c75-122">Impostazione della produzione</span><span class="sxs-lookup"><span data-stu-id="b2c75-122">Setting Up Manufacturing</span></span>](production-configure-production-processes.md)  
<span data-ttu-id="b2c75-123">[Manufacturing](production-manage-manufacturing.md)  </span><span class="sxs-lookup"><span data-stu-id="b2c75-123">[Manufacturing](production-manage-manufacturing.md)  </span></span>  
<span data-ttu-id="b2c75-124">[Pianif.](production-planning.md) </span><span class="sxs-lookup"><span data-stu-id="b2c75-124">[Planning](production-planning.md) </span></span>  
[<span data-ttu-id="b2c75-125">Magazzino</span><span class="sxs-lookup"><span data-stu-id="b2c75-125">Inventory</span></span>](inventory-manage-inventory.md)  
[<span data-ttu-id="b2c75-126">Acquisti</span><span class="sxs-lookup"><span data-stu-id="b2c75-126">Purchasing</span></span>](purchasing-manage-purchasing.md)  
<span data-ttu-id="b2c75-127">[Utilizzo di [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="b2c75-127">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
