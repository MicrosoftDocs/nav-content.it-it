---
title: Dettagli di progettazione - Monitoraggio del livello di giacenza disponibile e del punto di riordino
description: Informazioni sulla distinzione tra il livello di scorte disponibili previste e il livello di giacenza disponibile per la pianificazione del magazzino.
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: design, supply, inventory, planning
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: ef99b84a635a8403c62c38b8a66e77166bbf2883
ms.contentlocale: it-it
ms.lasthandoff: 10/16/2017

---
# <a name="design-details-monitoring-the-projected-inventory-level-and-the-reorder-point"></a><span data-ttu-id="b87f2-103">Dettagli di progettazione: Monitoraggio del livello di giacenza disponibile e del punto di riordino</span><span class="sxs-lookup"><span data-stu-id="b87f2-103">Design Details: Monitoring the Projected Inventory Level and the Reorder Point</span></span>
<span data-ttu-id="b87f2-104">Il magazzino è un tipo di approvvigionamento, ma per la pianificazione del magazzino, il sistema di pianificazione distingue tra due livelli di magazzino:</span><span class="sxs-lookup"><span data-stu-id="b87f2-104">Inventory is a type of supply, but for inventory planning, the planning system distinguishes between two inventory levels:</span></span>  

* <span data-ttu-id="b87f2-105">Quantità scorte previste</span><span class="sxs-lookup"><span data-stu-id="b87f2-105">Projected inventory</span></span>  
* <span data-ttu-id="b87f2-106">Scorte disponibili previste</span><span class="sxs-lookup"><span data-stu-id="b87f2-106">Projected available inventory</span></span>  

## <a name="projected-inventory"></a><span data-ttu-id="b87f2-107">Quantità scorte previste</span><span class="sxs-lookup"><span data-stu-id="b87f2-107">Projected Inventory</span></span>  
<span data-ttu-id="b87f2-108">Inizialmente, la giacenza disponibile corrisponde alla quantità di giacenza lorda, inclusi approvvigionamento e domanda passati anche se non registrati, all'avvio del processo di pianificazione.</span><span class="sxs-lookup"><span data-stu-id="b87f2-108">Initially, projected inventory is the quantity of gross inventory, including supply and demand in the past even if not posted, when starting the planning process.</span></span> <span data-ttu-id="b87f2-109">In futuro, diventa un livello di giacenza disponibile mobile che viene mantenuto dalle quantità lorde di approvvigionamenti e domande futuri perché sono introdotte seguendo la linea del tempo (se impegnate o allocate in altri modi).</span><span class="sxs-lookup"><span data-stu-id="b87f2-109">In the future, this becomes a moving projected inventory level that is maintained by gross quantities from future supply and demand because those are introduced along the time line (whether reserved or in other ways allocated).</span></span>  

<span data-ttu-id="b87f2-110">La giacenza disponibile viene utilizzata dal sistema di pianificazione per monitorare il punto di riordino e per determinare la quantità di riordino quando viene utilizzato il metodo di riordino Qtà Massima.</span><span class="sxs-lookup"><span data-stu-id="b87f2-110">The projected inventory is used by the planning system to monitor the reorder point and to determine the reorder quantity when using the Maximum Qty. reordering policy.</span></span>  

## <a name="projected-available-inventory"></a><span data-ttu-id="b87f2-111">Scorte disponibili previste</span><span class="sxs-lookup"><span data-stu-id="b87f2-111">Projected Available Inventory</span></span>  
<span data-ttu-id="b87f2-112">Le scorte disponibili previste sono la parte della giacenza disponibile che in un dato momento è disponibile per soddisfare la domanda.</span><span class="sxs-lookup"><span data-stu-id="b87f2-112">The projected available inventory is the part of the projected inventory that at a given point in time is available to fulfill demand.</span></span> <span data-ttu-id="b87f2-113">Le scorte disponibili previste vengono utilizzate dal motore di pianificazione durante il monitoraggio del livello della scorta di sicurezza.</span><span class="sxs-lookup"><span data-stu-id="b87f2-113">The projected available inventory is used by the planning engine when monitoring the safety stock level.</span></span>  

<span data-ttu-id="b87f2-114">Le scorte disponibili previste vengono utilizzate dal sistema di pianificazione per monitorare il livello di scorta di sicurezza, dal momento che la scorta di sicurezza deve essere sempre disponibile per servire la domanda imprevista.</span><span class="sxs-lookup"><span data-stu-id="b87f2-114">The projected available inventory is used by the planning system to monitor the safety stock level, since the safety stock must always be available to serve unexpected demand.</span></span>  

## <a name="time-buckets"></a><span data-ttu-id="b87f2-115">Intervalli di tempo</span><span class="sxs-lookup"><span data-stu-id="b87f2-115">Time Buckets</span></span>  
<span data-ttu-id="b87f2-116">È importante disporre di un controllo stretto delle scorte previste per rilevare quando viene raggiunto il punto di riordino e per calcolare le giuste quantità dell'ordine quando si utilizza il metodo di riordino Qtà massima.</span><span class="sxs-lookup"><span data-stu-id="b87f2-116">Having a tight control of the projected inventory is crucial to detect when the reorder point is reached or crossed and to calculate the right order quantity when using the Maximum Qty. reordering policy.</span></span>  

<span data-ttu-id="b87f2-117">Come dichiarato in precedenza, il livello di magazzino previsto viene calcolato all'inizio del periodo di pianificazione.</span><span class="sxs-lookup"><span data-stu-id="b87f2-117">As stated earlier, the projected inventory level is calculated at the start of the planning period.</span></span> <span data-ttu-id="b87f2-118">È un livello lordo che non considera gli impegni e le allocazioni simili.</span><span class="sxs-lookup"><span data-stu-id="b87f2-118">It is a gross level that does not consider reservations and similar allocations.</span></span> <span data-ttu-id="b87f2-119">Per monitorare il livello di magazzino durante la sequenza di pianificazione, le modifiche aggregate vengono monitorate dal sistema nell'arco di un intervallo di tempo.</span><span class="sxs-lookup"><span data-stu-id="b87f2-119">To monitor this inventory level during the planning sequence, the system monitors the aggregated changes over a period of time, a time bucket.</span></span> <span data-ttu-id="b87f2-120">Il sistema garantisce che l'intervallo di tempo sia almeno di un giorno perché è l'unità di tempo più precisa in caso di un evento di approvvigionamento o di domanda.</span><span class="sxs-lookup"><span data-stu-id="b87f2-120">The system ensures that the time bucket is at least one day since it is the most precise unit of time for a demand or supply event.</span></span>  

## <a name="determining-the-projected-inventory-level"></a><span data-ttu-id="b87f2-121">Determinazione del livello di magazzino previsto</span><span class="sxs-lookup"><span data-stu-id="b87f2-121">Determining the Projected Inventory Level</span></span>  
<span data-ttu-id="b87f2-122">Nella seguente sequenza viene descritto in che modo viene determinato il livello di giacenza disponibile:</span><span class="sxs-lookup"><span data-stu-id="b87f2-122">The following sequence describes how the projected inventory level is determined:</span></span>  

* <span data-ttu-id="b87f2-123">Quando un evento di approvvigionamento, ad esempio un ordine di acquisto, è stato completamente pianificato, la giacenza disponibile verrà aumentata alla data di scadenza.</span><span class="sxs-lookup"><span data-stu-id="b87f2-123">When a supply event, such as a purchase order has been totally planned, it will increase the projected inventory on its due date.</span></span>  
* <span data-ttu-id="b87f2-124">Una volta che un evento di domanda è stato completamente soddisfatto, la giacenza disponibile non diminuirà immediatamente.</span><span class="sxs-lookup"><span data-stu-id="b87f2-124">When a demand event has been fully satisfied, it will not decrease the projected inventory right away.</span></span> <span data-ttu-id="b87f2-125">In alternativa, registra un sollecito di diminuzione, ovvero un record interno che contiene la data e la quantità di contributo alla giacenza disponibile.</span><span class="sxs-lookup"><span data-stu-id="b87f2-125">Instead, it posts a decrease reminder, which is an internal record that holds the date and quantity of the contribution to the projected inventory.</span></span>  
* <span data-ttu-id="b87f2-126">Quando un evento di approvvigionamento successivo viene pianificato e collocato nella sequenza temporale, i solleciti di riduzione registrati vengono analizzati singolarmente fino alla data di approvvigionamento pianificata durante l'aggiornamento della giacenza disponibile.</span><span class="sxs-lookup"><span data-stu-id="b87f2-126">When a subsequent supply event is planned and placed on the time line, the posted decrease reminders are investigated one by one up until the planned date of the supply while updating the projected inventory.</span></span> <span data-ttu-id="b87f2-127">Durante il processo, potrebbe essere raggiunto o superato il livello del punto di riordino del sollecito di incremento interno.</span><span class="sxs-lookup"><span data-stu-id="b87f2-127">During this process, the reorder point level of the internal increase reminder may be reached or crossed.</span></span>  
* <span data-ttu-id="b87f2-128">Se viene immesso un nuovo ordine di approvvigionamento, nel sistema viene controllato se tale ordine viene immesso prima dell'approvvigionamento corrente.</span><span class="sxs-lookup"><span data-stu-id="b87f2-128">If a new supply order is introduced, the system checks if it is entered before the current supply.</span></span> <span data-ttu-id="b87f2-129">In questo caso, il nuovo approvvigionamento diventa l'approvvigionamento corrente e la procedura di contropartita rincomincia.</span><span class="sxs-lookup"><span data-stu-id="b87f2-129">If it is, the new supply becomes current supply and the balancing procedure starts over.</span></span>  

<span data-ttu-id="b87f2-130">Di seguito viene illustrato questo principio:</span><span class="sxs-lookup"><span data-stu-id="b87f2-130">The following shows a graphical illustration of this principle:</span></span>  

![](media/nav_app_supply_planning_2_projected_inventory.png "NAV_APP_supply_planning_2_projected_inventory")  

1. <span data-ttu-id="b87f2-131">L'approvvigionamento **Sa** di 4 (fisso) chiude la domanda **Da** di -3.</span><span class="sxs-lookup"><span data-stu-id="b87f2-131">Supply **Sa** of 4 (fixed) closes Demand **Da** of -3.</span></span>  
2. <span data-ttu-id="b87f2-132">CloseDemand: Creare un sollecito di riduzione di -3 (non visualizzato).</span><span class="sxs-lookup"><span data-stu-id="b87f2-132">CloseDemand: Create a decrease reminder of -3 (not shown).</span></span>  
3. <span data-ttu-id="b87f2-133">L'approvvigionamento **Sa** viene chiuso con un surplus di 1 (non esiste più domanda).</span><span class="sxs-lookup"><span data-stu-id="b87f2-133">Supply **Sa** is closed with a surplus of 1 (no more demand exists).</span></span>  

     <span data-ttu-id="b87f2-134">Ciò aumenta il livello di scorte previste a +4, mentre la giacenza **disponibile** diventa -1.</span><span class="sxs-lookup"><span data-stu-id="b87f2-134">This increases the projected inventory level to +4, while the projected **available** inventory becomes -1.</span></span>  

4. <span data-ttu-id="b87f2-135">Il successivo approvvigionamento **Sb** di 2 (un altro ordine) è già stato immesso nella sequenza temporale.</span><span class="sxs-lookup"><span data-stu-id="b87f2-135">The next supply **Sb** of 2 (another order) has already been placed on the timeline.</span></span>  
5. <span data-ttu-id="b87f2-136">Il sistema controlla se esiste un sollecito di riduzione precedente a **Sb**; in caso negativo, non viene intrapresa alcuna azione.</span><span class="sxs-lookup"><span data-stu-id="b87f2-136">System checks if there is any decrease reminder preceding **Sb** (there is not, so no action is taken).</span></span>  
6. <span data-ttu-id="b87f2-137">Il sistema chiude l'approvvigionamento **Sb** (non esiste più domanda) riducendolo a 0 (annullamento) o lasciandolo invariato.</span><span class="sxs-lookup"><span data-stu-id="b87f2-137">System closes supply **Sb** (no more demand exists)—either A: by reducing it to 0 (cancel) or B: by leaving as is.</span></span>  

     <span data-ttu-id="b87f2-138">Ciò aumenta il livello del magazzino previsto (A: +0 => +4 o B: +2 = +6).</span><span class="sxs-lookup"><span data-stu-id="b87f2-138">This increases the projected inventory level (A: +0 => +4 or B: +2 = +6).</span></span>  

7. <span data-ttu-id="b87f2-139">Il sistema esegue un controllo finale: è presente un sollecito di riduzione?</span><span class="sxs-lookup"><span data-stu-id="b87f2-139">System makes a final check: Is there any decrease reminder?</span></span> <span data-ttu-id="b87f2-140">Sì, ne esiste uno alla data di **Da**.</span><span class="sxs-lookup"><span data-stu-id="b87f2-140">Yes, there is one on the date of **Da**.</span></span>  
8. <span data-ttu-id="b87f2-141">Viene aggiunto un sollecito di diminuzione dal sistema di -3 al livello di giacenza disponibile, A: +4 -3 = 1 o B: +6 -3 = +3.</span><span class="sxs-lookup"><span data-stu-id="b87f2-141">System adds the decrease reminder of -3 reminder to the projected inventory level, either A: +4 -3 = 1 or B: +6 -3 = +3.</span></span>  
9. <span data-ttu-id="b87f2-142">Nel caso di A, il sistema crea un ordine programmato in avanti che inizia alla data indicata di **Da**.</span><span class="sxs-lookup"><span data-stu-id="b87f2-142">In case of A, the system creates a forward-scheduled order starting on date **Da**.</span></span>  

     <span data-ttu-id="b87f2-143">Nel caso di B, viene raggiunto il punto di riordino e viene creato un nuovo ordine.</span><span class="sxs-lookup"><span data-stu-id="b87f2-143">In case of B, the reorder point is reached and a new order is created.</span></span>  

## <a name="see-also"></a><span data-ttu-id="b87f2-144">Vedi anche</span><span class="sxs-lookup"><span data-stu-id="b87f2-144">See Also</span></span>  
<span data-ttu-id="b87f2-145">[Dettagli di progettazione: Criteri di riordino](design-details-reordering-policies.md) </span><span class="sxs-lookup"><span data-stu-id="b87f2-145">[Design Details: Reordering Policies](design-details-reordering-policies.md) </span></span>  
<span data-ttu-id="b87f2-146">[Dettagli di progettazione: Parametri di pianificazione](design-details-planning-parameters.md) </span><span class="sxs-lookup"><span data-stu-id="b87f2-146">[Design Details: Planning Parameters](design-details-planning-parameters.md) </span></span>  
<span data-ttu-id="b87f2-147">[Dettagli di progettazione: Gestione dei metodi di riordino](design-details-handling-reordering-policies.md) </span><span class="sxs-lookup"><span data-stu-id="b87f2-147">[Design Details: Handling Reordering Policies](design-details-handling-reordering-policies.md) </span></span>  
[<span data-ttu-id="b87f2-148">Dettagli di progettazione: Pianificazione approvvigionamento</span><span class="sxs-lookup"><span data-stu-id="b87f2-148">Design Details: Supply Planning</span></span>](design-details-supply-planning.md)
