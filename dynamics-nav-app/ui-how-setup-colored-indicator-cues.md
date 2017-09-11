---
title: 'Procedura: Impostare un indicatore colorato nelle pile'
author: SusanneWindfeldPedersen
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 6b60b1344a1e18ad91863046110df880f75f7c04
ms.openlocfilehash: 38cd904d0cf22374eac430d035e6ea6d205bcab8
ms.contentlocale: it-it
ms.lasthandoff: 07/19/2017

---
    
# <a name="how-to-set-up-a-colored-indicator-on-cues"></a><span data-ttu-id="4d0ab-102">Procedura: Impostare un indicatore colorato nelle pile</span><span class="sxs-lookup"><span data-stu-id="4d0ab-102">How to: Set Up a Colored Indicator on Cues</span></span>
<span data-ttu-id="4d0ab-103">È possibile impostare delle pile che vengono visualizzate nella pagina **Home** in modo che includano un indicatore che cambia colore in base ai valori dei dati presenti nelle pile.</span><span class="sxs-lookup"><span data-stu-id="4d0ab-103">You can set up Cues that appear on the **Home** page to include an indicator that changes color based on the data values in the Cues.</span></span> 

<span data-ttu-id="4d0ab-104">L'indicatore viene visualizzato come una barra colorata lungo il bordo superiore della pila.</span><span class="sxs-lookup"><span data-stu-id="4d0ab-104">The indicator appears as a colored bar along the top border of the Cue tile.</span></span> <span data-ttu-id="4d0ab-105">Fornisce un segnale visivo dello stato dell'attività della pila, che può indicare le condizioni favorevoli o sfavorevoli per spingere l'utente a intraprendere un'azione.</span><span class="sxs-lookup"><span data-stu-id="4d0ab-105">It provides a visual signal of the status of the Cue's activity, which can indicate favorable or unfavorable conditions to prompt the user to take action.</span></span> <span data-ttu-id="4d0ab-106">Ad esempio, se una pila visualizza le fatture di vendita in corso, è possibile impostare l'indicatore in modo che appaia verde (favorevole) quando il totale delle fatture di vendita in corso è minore di 10 e rosso (sfavorevole) quando il totale è maggiore di 20.</span><span class="sxs-lookup"><span data-stu-id="4d0ab-106">For example, if a Cue displays ongoing sales invoices, you can set up the indicator to appear green (favorable) when total number of ongoing sales invoices is below 10, and appears red (unfavorable) when the total is greater than 20.</span></span>

<span data-ttu-id="4d0ab-107">Nella finestra **Setup pila**, si impostano gli indicatori di tutte le pile disponibili nel database della società.</span><span class="sxs-lookup"><span data-stu-id="4d0ab-107">From the **Cue Setup** window, you set up indicators for all the Cues that are available in the company database.</span></span>

<span data-ttu-id="4d0ab-108">Per impostare l'indicatore, specificare fino a due valori di soglia che definiscono tre intervalli dei valori dei dati (basso, medio e alto) e a cui è possibile applicare un colore diverso (o stile).</span><span class="sxs-lookup"><span data-stu-id="4d0ab-108">To set up the indicator, you specify up to two threshold values that define three ranges of data values (low, middle, and high) to which you can apply a different color (or style).</span></span>

## <a name="to-set-up-colored-indicators-on-cues"></a><span data-ttu-id="4d0ab-109">Per impostare indicatori colorati nelle pile</span><span class="sxs-lookup"><span data-stu-id="4d0ab-109">To set up colored indicators on Cues</span></span>
1. <span data-ttu-id="4d0ab-110">In **Attività**, nella pagina **Home**, scegliere **Imposta pile**.</span><span class="sxs-lookup"><span data-stu-id="4d0ab-110">Under **Activities** on your **Home** page, choose **Set Up Cues**.</span></span>  
<span data-ttu-id="4d0ab-111">Verrà visualizzata la finestra **Setup pila**.</span><span class="sxs-lookup"><span data-stu-id="4d0ab-111">The **Cue Setup** window appears.</span></span> <span data-ttu-id="4d0ab-112">Nella finestra sono elencati gli indicatori attualmente impostati nelle pile.</span><span class="sxs-lookup"><span data-stu-id="4d0ab-112">The window lists the indicators that are currently setup up on Cues.</span></span>
2. <span data-ttu-id="4d0ab-113">Per modificare un indicatore, modificare i campi e modificare, ad esempio, i valori per le diverse soglie.</span><span class="sxs-lookup"><span data-stu-id="4d0ab-113">To modify an indicator, edit the fields and modify, for example, the values for the different thresholds.</span></span>  

<span data-ttu-id="4d0ab-114">Nella tabella seguente sono elencati i colori corrispondenti alle opzioni dei campi **Stile intervallo inferiore**, **Stile intervallo medio** e **Stile intervallo superiore**.</span><span class="sxs-lookup"><span data-stu-id="4d0ab-114">The following table lists the colors that correspond to the options of the **Low Range Style**, **Middle Range Style**, and **High Range Style** fields.</span></span>

|<span data-ttu-id="4d0ab-115">Opzione</span><span class="sxs-lookup"><span data-stu-id="4d0ab-115">Option</span></span>|<span data-ttu-id="4d0ab-116">Colore</span><span class="sxs-lookup"><span data-stu-id="4d0ab-116">Color</span></span>|
|------|-----|
|<span data-ttu-id="4d0ab-117">**Nessuno**</span><span class="sxs-lookup"><span data-stu-id="4d0ab-117">**None**</span></span>|<span data-ttu-id="4d0ab-118">Nessun colore (lo stesso colore della sezione Pila</span><span class="sxs-lookup"><span data-stu-id="4d0ab-118">No color (same color as the Cue tile</span></span>|
|<span data-ttu-id="4d0ab-119">**Favorevole**</span><span class="sxs-lookup"><span data-stu-id="4d0ab-119">**Favorable**</span></span>|<span data-ttu-id="4d0ab-120">Verde</span><span class="sxs-lookup"><span data-stu-id="4d0ab-120">Green</span></span>|
|<span data-ttu-id="4d0ab-121">**Sfavorevole**</span><span class="sxs-lookup"><span data-stu-id="4d0ab-121">**Unfavorable**</span></span>|<span data-ttu-id="4d0ab-122">Rosso</span><span class="sxs-lookup"><span data-stu-id="4d0ab-122">Red</span></span>|
|<span data-ttu-id="4d0ab-123">**Ambiguo**</span><span class="sxs-lookup"><span data-stu-id="4d0ab-123">**Ambiguous**</span></span>|<span data-ttu-id="4d0ab-124">Giallo</span><span class="sxs-lookup"><span data-stu-id="4d0ab-124">Yellow</span></span>|
|<span data-ttu-id="4d0ab-125">**Subordinato**</span><span class="sxs-lookup"><span data-stu-id="4d0ab-125">**Subordinate**</span></span>|<span data-ttu-id="4d0ab-126">Grigio</span><span class="sxs-lookup"><span data-stu-id="4d0ab-126">Gray</span></span>|

## <a name="see-also"></a><span data-ttu-id="4d0ab-127">Vedi anche</span><span class="sxs-lookup"><span data-stu-id="4d0ab-127">See Also</span></span>
[<span data-ttu-id="4d0ab-128">Utilizzare Dynamics NAV</span><span class="sxs-lookup"><span data-stu-id="4d0ab-128">Work with Dynamics NAV</span></span>](ui-work-product.md)


