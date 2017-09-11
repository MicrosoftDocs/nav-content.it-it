---
title: "Procedura: Impostare cicli e fasi di vendita dalle opportunità"
author: jswymer
ms.custom: na
ms.date: 09/16/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 6b60b1344a1e18ad91863046110df880f75f7c04
ms.openlocfilehash: 756e9b2f33fe66cd4c2b4e26ca4390683bd087af
ms.contentlocale: it-it
ms.lasthandoff: 07/19/2017

---
# <a name="how-to-set-up-opportunity-sales-cycles-and-cycle-stages"></a><span data-ttu-id="89f9a-102">Procedura: Impostare cicli e fasi di vendita dalle opportunità</span><span class="sxs-lookup"><span data-stu-id="89f9a-102">How to: Set Up Opportunity Sales Cycles and Cycle Stages</span></span>
<span data-ttu-id="89f9a-103">Prima di iniziare a utilizzare le opportunità di vendita, è necessario impostare cicli di vendita e fasi dei cicli di vendita.</span><span class="sxs-lookup"><span data-stu-id="89f9a-103">Before you can start using sales opportunities, you must set up sales cycles and sales cycle stages.</span></span> <span data-ttu-id="89f9a-104">Un ciclo di vendita è composto da una serie di fasi che vanno dal contatto iniziale alla chiusura della vendita.</span><span class="sxs-lookup"><span data-stu-id="89f9a-104">A sales cycle is made up of a series of stages that go from the initial contact to the closing of a sale.</span></span> <span data-ttu-id="89f9a-105">Per ogni fase possono essere previsti determinati requisiti che devono essere soddisfatti, ad esempio richiesta di un'offerta di vendita, prima che un'opportunità possa passare alla fase successiva.</span><span class="sxs-lookup"><span data-stu-id="89f9a-105">Each stage can have certain requirements that must be met, such as requiring a sales quote, before an opportunity can go to the next stage.</span></span> <span data-ttu-id="89f9a-106">È inoltre possibile specificare se una fase può essere ignorata.</span><span class="sxs-lookup"><span data-stu-id="89f9a-106">You can also specify whether a stage can be skipped.</span></span> <span data-ttu-id="89f9a-107">È possibile impostare il numero desiderato di cicli di vendita e di fasi all'interno di un ciclo.</span><span class="sxs-lookup"><span data-stu-id="89f9a-107">You can setup as many sales cycles as you need, and you can set up as many sales cycle stages as necessary within a sales cycle.</span></span>

<span data-ttu-id="89f9a-108">Implementare i cicli di vendita delle opportunità consiste nell'impostare il codice ciclo di vendita, definire le varie fasi del ciclo e quindi assegnare il ciclo alle opportunità.</span><span class="sxs-lookup"><span data-stu-id="89f9a-108">Implementing opportunity sales cycles involves setting up the sales cycle code, defining the different stages of the cycle, and then assigning the cycle to opportunities.</span></span>

## <a name="to-set-up-an-opportunity-sales-cycle-code"></a><span data-ttu-id="89f9a-109">Per impostare un codice ciclo di vendita delle opportunità</span><span class="sxs-lookup"><span data-stu-id="89f9a-109">To set up an opportunity sales cycle code</span></span>
1. <span data-ttu-id="89f9a-110">Nell'angolo superiore destro, scegliere l'icona **Cerca pagina o report**, immettere **Cicli di vendita**, quindi scegliere il collegamento correlato.</span><span class="sxs-lookup"><span data-stu-id="89f9a-110">In the top right corner, choose the **Search for Page or Report** icon, enter **Sales Cycles**, and then choose the related link.</span></span> <span data-ttu-id="89f9a-111">La finestra **Cicli di vendita** si apre e viene visualizzato un elenco di tutti i cicli di vendita esistenti.</span><span class="sxs-lookup"><span data-stu-id="89f9a-111">The **Sales Cycles** window opens, and lists all the existing sales cycles.</span></span>
2. <span data-ttu-id="89f9a-112">Scegliere l'azione **Nuovo** e compilare i campi.</span><span class="sxs-lookup"><span data-stu-id="89f9a-112">Choose the **New** action, and fill in the fields.</span></span>

<span data-ttu-id="89f9a-113">Ripetere tali passaggi per impostare altri cicli di vendita.</span><span class="sxs-lookup"><span data-stu-id="89f9a-113">Repeat these steps to set up as many sales cycles as you want.</span></span> <span data-ttu-id="89f9a-114">Dopo aver impostato i cicli delle opportunità di vendita, potrebbe essere necessario impostare le diverse fasi all'interno di ciascun ciclo.</span><span class="sxs-lookup"><span data-stu-id="89f9a-114">After you have set up opportunity sales cycles, you may want to set up the different stages within each cycle.</span></span>

## <a name="to-define-opportunity-sales-cycle-stages"></a><span data-ttu-id="89f9a-115">Per definire le fasi ciclo di vendita delle opportunità</span><span class="sxs-lookup"><span data-stu-id="89f9a-115">To define opportunity sales cycle stages</span></span>
1. <span data-ttu-id="89f9a-116">Nella finestra **Cicli di vendita** selezionare l'opportunità relativa al ciclo di vendita per la quale si desidera impostare le fasi, quindi fare clic sull'azione **Fasi**.</span><span class="sxs-lookup"><span data-stu-id="89f9a-116">In the **Sales Cycles** window, select the opportunity sales cycle for which you want to set up stages, and then choose the **Stages** action.</span></span> <span data-ttu-id="89f9a-117">Verrà aperta la finestra **Fasi ciclo di vendita**.</span><span class="sxs-lookup"><span data-stu-id="89f9a-117">The **Sales Cycle Stages** window opens.</span></span>
2. <span data-ttu-id="89f9a-118">Scegliere l'azione **Nuovo** per inserire una nuova fase nel ciclo di vendita.</span><span class="sxs-lookup"><span data-stu-id="89f9a-118">Choose the **New** action to enter a new stage in the sales cycle.</span></span>

<span data-ttu-id="89f9a-119">Ripetere tali passaggi per impostare altre fasi all'interno del ciclo di vendita.</span><span class="sxs-lookup"><span data-stu-id="89f9a-119">Repeat these steps to set up as many stages as you want within the sales cycle.</span></span>

## <a name="to-assign-stage-cycle-to-an-opportunity"></a><span data-ttu-id="89f9a-120">Per assegnare il ciclo della fase a un'opportunità</span><span class="sxs-lookup"><span data-stu-id="89f9a-120">To assign stage cycle to an opportunity</span></span>
<span data-ttu-id="89f9a-121">Una volta aggiunto il ciclo della fase delle opportunità, è possibile iniziare ad aggiungere le opportunità di vendita e quindi assegnare il ciclo della fase alle opportunità impostando il campo **Codice ciclo di vendita**.</span><span class="sxs-lookup"><span data-stu-id="89f9a-121">After you add the opportunities stage cycle, you can start to add sales opportunities, and then assign the stage cycle to opportunities by setting the **Sales Cycle Code** field.</span></span> <span data-ttu-id="89f9a-122">Per ulteriori informazioni, vedere [Procedura: Creare opportunità di vendita](marketing-how-create-opportunities.md).</span><span class="sxs-lookup"><span data-stu-id="89f9a-122">For more information, see [How to: Create Sales Opportunities](marketing-how-create-opportunities.md).</span></span>

##<a name="see-also"></a><span data-ttu-id="89f9a-123">Vedi anche</span><span class="sxs-lookup"><span data-stu-id="89f9a-123">See Also</span></span>  
[<span data-ttu-id="89f9a-124">Elaborazione delle opportunità di vendita</span><span class="sxs-lookup"><span data-stu-id="89f9a-124">Processing Sales Opportunities</span></span>](marketing-processing-sales-opportunities.md)  
[<span data-ttu-id="89f9a-125">Gestire le vendite</span><span class="sxs-lookup"><span data-stu-id="89f9a-125">Manage Sales</span></span>](sales-manage-sales.md)  
[<span data-ttu-id="89f9a-126">Utilizzo di Dynamics NAV</span><span class="sxs-lookup"><span data-stu-id="89f9a-126">Working with Dynamics NAV</span></span>](ui-work-product.md)

