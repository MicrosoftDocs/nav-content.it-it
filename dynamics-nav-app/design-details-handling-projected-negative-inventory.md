---
title: Dettagli di progettazione - Gestione giacenze negative previste
description: "Il punto di riordino esprime la domanda prevista durante il lead time dell'articolo. Quando il punto di riordino viene superato, è tempo di ordinare quantità maggiori. Ma le scorte previste devono essere abbastanza grandi da coprire la domanda fino a che non viene ricevuto il nuovo ordine. Nel frattempo, la scorta di sicurezza deve coprire le fluttuazioni della domanda fino a un livello di servizio di destinazione."
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
ms.openlocfilehash: 66cf357ccd0489d789ec9c2036734ec9f04aad95
ms.contentlocale: it-it
ms.lasthandoff: 10/16/2017

---
# <a name="design-details-handling-projected-negative-inventory"></a><span data-ttu-id="bf030-106">Dettagli di progettazione: Gestione giacenze negative previste</span><span class="sxs-lookup"><span data-stu-id="bf030-106">Design Details: Handling Projected Negative Inventory</span></span>
<span data-ttu-id="bf030-107">Il punto di riordino esprime la domanda prevista durante il lead time dell'articolo.</span><span class="sxs-lookup"><span data-stu-id="bf030-107">The reorder point expresses the anticipated demand during the lead time of the item.</span></span> <span data-ttu-id="bf030-108">Quando il punto di riordino viene superato, è tempo di ordinare quantità maggiori.</span><span class="sxs-lookup"><span data-stu-id="bf030-108">When the reorder point is passed, it is time to order more.</span></span> <span data-ttu-id="bf030-109">Ma le scorte previste devono essere abbastanza grandi da coprire la domanda fino a che non viene ricevuto il nuovo ordine.</span><span class="sxs-lookup"><span data-stu-id="bf030-109">But the projected inventory must be large enough to cover the demand until the new order is received.</span></span> <span data-ttu-id="bf030-110">Nel frattempo, la scorta di sicurezza deve coprire le fluttuazioni della domanda fino a un livello di servizio di destinazione.</span><span class="sxs-lookup"><span data-stu-id="bf030-110">Meanwhile, the safety stock should take care of fluctuations in demand up to a targeted service level.</span></span>  

 <span data-ttu-id="bf030-111">Di conseguenza, se una domanda futura non può essere servita dalle scorte previste, oppure espressa in un altro modo, il sistema di pianificazione considera un'emergenza se la giacenza disponibile diventa negativa.</span><span class="sxs-lookup"><span data-stu-id="bf030-111">Consequently, the planning system considers it an emergency if a future demand cannot be served from the projected inventory, or expressed in another way, that the projected inventory goes negative.</span></span> <span data-ttu-id="bf030-112">Il sistema tratta questo tipo di eccezione suggerendo un nuovo ordine di approvvigionamento in modo da soddisfare la parte della domanda che non può essere soddisfatta dal magazzino o da un altro approvvigionamento.</span><span class="sxs-lookup"><span data-stu-id="bf030-112">The system deals with such an exception by suggesting a new supply order to meet the part of the demand that cannot be met by inventory or other supply.</span></span> <span data-ttu-id="bf030-113">Le dimensioni dell'ordine del nuovo ordine di approvvigionamento non prenderanno in considerazione la giacenza massima o la quantità di riordino, né prenderanno in considerazione i modificatori di ordine Quantità massima ordine, Quantità minima ordine e Molteplicità ordine.</span><span class="sxs-lookup"><span data-stu-id="bf030-113">The order size of the new supply order will not take the maximum inventory or the reorder quantity into consideration, nor will it take into consideration the order modifiers Maximum Order Quantity, Minimum Order Quantity, and Order Multiple.</span></span> <span data-ttu-id="bf030-114">In alternativa, rifletterà la carenza esatta.</span><span class="sxs-lookup"><span data-stu-id="bf030-114">Instead, it will reflect the exact deficiency.</span></span>  

 <span data-ttu-id="bf030-115">Nella riga di pianificazione per questo tipo ordine di approvvigionamento verrà visualizzata un'icona di avviso di emergenza. Verranno inoltre fornite informazioni aggiuntive su ricerca per informare l'utente della situazione.</span><span class="sxs-lookup"><span data-stu-id="bf030-115">The planning line for this type of supply order will display an Emergency warning icon, and additional information will be provided upon lookup to inform the user of the situation.</span></span>  

 <span data-ttu-id="bf030-116">Nella seguente illustrazione l'approvvigionamento D rappresenta un ordine di emergenza per la rettifica della giacenza negativa.</span><span class="sxs-lookup"><span data-stu-id="bf030-116">In the following illustration, supply D represents an emergency order to adjust for negative inventory.</span></span>  

 ![](media/nav_app_supply_planning_2_negative_inventory.png "NAV_APP_supply_planning_2_negative_inventory")  

1.  <span data-ttu-id="bf030-117">L'approvvigionamento **A**, la giacenza disponibile iniziale, è inferiore al punto di riordino.</span><span class="sxs-lookup"><span data-stu-id="bf030-117">Supply **A**, initial projected inventory, is below reorder point.</span></span>  

2.  <span data-ttu-id="bf030-118">Viene creato un nuovo approvvigionamento programmato in avanti (**C**).</span><span class="sxs-lookup"><span data-stu-id="bf030-118">A new forward-scheduled supply is created (**C**).</span></span>  

     <span data-ttu-id="bf030-119">(Quantità = Giacenza massima – Livello giacenza disponibile)</span><span class="sxs-lookup"><span data-stu-id="bf030-119">(Quantity = Maximum Inventory – Projected Inventory Level)</span></span>  

3.  <span data-ttu-id="bf030-120">L'approvvigionamento **A** viene chiuso dalla domanda **B**, che non viene coperta completamente.</span><span class="sxs-lookup"><span data-stu-id="bf030-120">Supply **A** is closed by demand **B**, which is not fully covered.</span></span>  

     <span data-ttu-id="bf030-121">La domanda **B** potrebbe provare a pianificare l'Approvvigionamento C ma ciò non accade in base al concetto dell'intervallo di tempo.</span><span class="sxs-lookup"><span data-stu-id="bf030-121">(Demand **B** could try to schedule Supply C in but that will not happen according to the time-bucket concept.)</span></span>  

4.  <span data-ttu-id="bf030-122">Un nuovo approvvigionamento (**D**) viene creato per coprire la quantità residua sulla domanda **B**.</span><span class="sxs-lookup"><span data-stu-id="bf030-122">New supply (**D**) is created to cover the remaining quantity on Demand **B**.</span></span>  

5.  <span data-ttu-id="bf030-123">La domanda **B** viene chiusa creando un sollecito alle scorte previste.</span><span class="sxs-lookup"><span data-stu-id="bf030-123">Demand **B** is closed (creating a reminder to the projected inventory).</span></span>  

6.  <span data-ttu-id="bf030-124">Il nuovo approvvigionamento **D** viene chiuso.</span><span class="sxs-lookup"><span data-stu-id="bf030-124">The new supply **D** is closed.</span></span>  

7.  <span data-ttu-id="bf030-125">La giacenza disponibile è controllata; il punto di riordino non è stato superato.</span><span class="sxs-lookup"><span data-stu-id="bf030-125">Projected Inventory is checked; reorder point has not been crossed.</span></span>  

8.  <span data-ttu-id="bf030-126">L'approvvigionamento **C** viene chiuso (non esiste più la domanda).</span><span class="sxs-lookup"><span data-stu-id="bf030-126">Supply **C** is closed (no more demand exists).</span></span>  

9. <span data-ttu-id="bf030-127">Controllo finale: non esistono solleciti di livello di magazzino in sospeso.</span><span class="sxs-lookup"><span data-stu-id="bf030-127">Final check: No outstanding inventory level reminders exist.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="bf030-128">Il passaggio 4 indica in che modo il sistema opera nelle versioni precedenti a Microsoft Dynamics NAV 2009 SP1.</span><span class="sxs-lookup"><span data-stu-id="bf030-128">Step 4 reflects how the system reacts in versions earlier than Microsoft Dynamics NAV 2009 SP1.</span></span>  

 <span data-ttu-id="bf030-129">Ciò conclude la descrizione dei principi centrali relativi alla pianificazione del magazzino basata sui metodi di riordino.</span><span class="sxs-lookup"><span data-stu-id="bf030-129">This concludes the description of central principles relating to inventory planning based on reordering policies.</span></span> <span data-ttu-id="bf030-130">Nella seguente sezione vengono illustrate le caratteristiche dei quattro metodi di riordino supportati.</span><span class="sxs-lookup"><span data-stu-id="bf030-130">The following section describes the characteristics of the four supported reordering policies.</span></span>  

## <a name="see-also"></a><span data-ttu-id="bf030-131">Vedi anche</span><span class="sxs-lookup"><span data-stu-id="bf030-131">See Also</span></span>  
 <span data-ttu-id="bf030-132">[Dettagli di progettazione: Criteri di riordino](design-details-reordering-policies.md) </span><span class="sxs-lookup"><span data-stu-id="bf030-132">[Design Details: Reordering Policies](design-details-reordering-policies.md) </span></span>  
 <span data-ttu-id="bf030-133">[Dettagli di progettazione: Parametri di pianificazione](design-details-planning-parameters.md) </span><span class="sxs-lookup"><span data-stu-id="bf030-133">[Design Details: Planning Parameters](design-details-planning-parameters.md) </span></span>  
 <span data-ttu-id="bf030-134">[Dettagli di progettazione: Gestione dei metodi di riordino](design-details-handling-reordering-policies.md) </span><span class="sxs-lookup"><span data-stu-id="bf030-134">[Design Details: Handling Reordering Policies](design-details-handling-reordering-policies.md) </span></span>  
 [<span data-ttu-id="bf030-135">Dettagli di progettazione: Pianificazione approvvigionamento</span><span class="sxs-lookup"><span data-stu-id="bf030-135">Design Details: Supply Planning</span></span>](design-details-supply-planning.md)
