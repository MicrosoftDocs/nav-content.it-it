---
title: "Dettagli di progettazione - Qtà riordino fissa"
description: "Il criterio Qtà Riordino Fissa è correlato alla pianificazione di magazzino dei tipici articoli C (costo di magazzino basso, basso rischio di obsolescenza e/o molti articoli). Questo metodo viene in genere utilizzato in connessione con un punto di riordino che riflette la domanda anticipata durante il lead time dell'articolo."
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
ms.openlocfilehash: 6249f51415f46443eb0b528161da290aac25d202
ms.contentlocale: it-it
ms.lasthandoff: 10/16/2017

---
# <a name="design-details-fixed-reorder-qty"></a><span data-ttu-id="6d1d2-104">Dettagli di progettazione: Qtà riordino fissa</span><span class="sxs-lookup"><span data-stu-id="6d1d2-104">Design Details: Fixed Reorder Qty.</span></span>
<span data-ttu-id="6d1d2-105">Il criterio Qtà Riordino Fissa è correlato alla pianificazione di magazzino dei tipici articoli C (costo di magazzino basso, basso rischio di obsolescenza e/o molti articoli).</span><span class="sxs-lookup"><span data-stu-id="6d1d2-105">The Fixed Reorder Qty. policy is related to inventory planning of typical C-items (low inventory cost, low risk of obsolescence, and/or many items).</span></span> <span data-ttu-id="6d1d2-106">Questo metodo viene in genere utilizzato in connessione con un punto di riordino che riflette la domanda anticipata durante il lead time dell'articolo.</span><span class="sxs-lookup"><span data-stu-id="6d1d2-106">This policy is usually used in connection with a reorder point reflecting the anticipated demand during the lead time of the item.</span></span>  

## <a name="calculated-per-time-bucket"></a><span data-ttu-id="6d1d2-107">Calcolato per intervallo di tempo</span><span class="sxs-lookup"><span data-stu-id="6d1d2-107">Calculated per Time Bucket</span></span>  
 <span data-ttu-id="6d1d2-108">Se il sistema di pianificazione rileva che il punto di riordino è stato raggiunto o superato in un intervallo di tempo specificato (ciclo di riordino) - sopra o in corrispondenza del punto di riordino all'inizio del periodo e sotto o in corrispondenza del punto di riordino alla fine del periodo - verrà suggerito di creare un nuovo ordine di approvvigionamento della quantità di riordino specificata e di programmarlo dalla prima data successiva alla fine dell'intervallo di tempo.</span><span class="sxs-lookup"><span data-stu-id="6d1d2-108">If the planning system detects that the reorder point has been reached or crossed in a given time bucket (reorder cycle) – above or on the reorder point at the start of the period and below or on the reorder point at the end of the period – it will suggest to create a new supply order of the specified reorder quantity and forward schedule it from the first date after the end of the time bucket.</span></span>  

 <span data-ttu-id="6d1d2-109">Il concetto di punto di riordino programmato riduce il numero di suggerimenti di approvvigionamento.</span><span class="sxs-lookup"><span data-stu-id="6d1d2-109">The bucketed reorder point concept reduces the number of supply suggestions.</span></span> <span data-ttu-id="6d1d2-110">Ciò riflette un processo manuale di entrare nella warehouse spesso per controllare i contenuti effettivi nelle varie collocazioni.</span><span class="sxs-lookup"><span data-stu-id="6d1d2-110">This reflects a manual process of frequently walking through the warehouse to check the actual contents in the various bins.</span></span>  

## <a name="creates-only-necessary-supply"></a><span data-ttu-id="6d1d2-111">Crea solo l'approvvigionamento necessario</span><span class="sxs-lookup"><span data-stu-id="6d1d2-111">Creates only Necessary Supply</span></span>  
 <span data-ttu-id="6d1d2-112">Prima di suggerire un nuovo ordine di approvvigionamento per soddisfare un punto di riordino, il sistema di pianificazione controlla se l'approvvigionamento è già stato ordinato per essere ricevuto entro il lead time di un articolo.</span><span class="sxs-lookup"><span data-stu-id="6d1d2-112">Before suggesting a new supply order to meet a reorder point, the planning system checks if supply has already been ordered to be received within the item’s lead time.</span></span> <span data-ttu-id="6d1d2-113">Se un ordine di approvvigionamento esistente risolverà il problema portando la giacenza disponibile al punto di riordino o oltre nel lead time, il sistema non suggerirà un nuovo ordine di approvvigionamento.</span><span class="sxs-lookup"><span data-stu-id="6d1d2-113">If an existing supply order will solve the problem by bringing the projected inventory to or above the reorder point within the lead time, the system will not suggest a new supply order.</span></span>  

 <span data-ttu-id="6d1d2-114">Gli ordini di approvvigionamento che vengono creati specificamente per soddisfare un punto di riordino sono esclusi dal bilanciamento dell'approvvigionamento ordinario e non verranno in alcun modo modificati in seguito.</span><span class="sxs-lookup"><span data-stu-id="6d1d2-114">Supply orders that are created specifically to meet a reorder point is excluded from ordinary supply balancing, and will not in any way be changed afterwards.</span></span> <span data-ttu-id="6d1d2-115">Di conseguenza, se un articolo che utilizza il punto di riordino deve essere eliminato (non compilato), è consigliabile verificare gli ordini di approvvigionamento inevasi manualmente o modificare il metodo di riordino lotto-per-Lotto con cui il sistema ridurrà o annullerà l'approvvigionamento superfluo.</span><span class="sxs-lookup"><span data-stu-id="6d1d2-115">Consequently, if an item using reorder point is to be phased out (not replenished), it is advisable to review outstanding supply orders manually or change the reordering policy to Lot-for-Lot, whereby the system will reduce or cancel superfluous supply.</span></span>  

## <a name="combines-with-order-modifiers"></a><span data-ttu-id="6d1d2-116">Combina con i modificatori di ordine</span><span class="sxs-lookup"><span data-stu-id="6d1d2-116">Combines with Order Modifiers</span></span>  
 <span data-ttu-id="6d1d2-117">I modificatori di ordini, Quantità minima ordine, Quantità massima ordine e Molteplicità ordine, non devono svolgere un grande ruolo quando vengono utilizzati i criteri di quantità riordino fissa.</span><span class="sxs-lookup"><span data-stu-id="6d1d2-117">The order modifiers, Minimum Order Quantity, Maximum Order Quantity, and Order Multiple, should not play a big role when the fixed reorder quantity policy is used.</span></span> <span data-ttu-id="6d1d2-118">Tuttavia, il sistema di pianificazione prende ancora in considerazione questi modificatori e diminuirà la quantità alle quantità di ordine massime specificate (e creerà due o più approvvigionamenti per raggiungere la quantità di ordine totale), aumenterà la quantità di ordine minima o arrotonderà la quantità di ordine fino a soddisfare la molteplicità ordine specificata.</span><span class="sxs-lookup"><span data-stu-id="6d1d2-118">However, the planning system still takes these modifiers into account and will decrease the quantity to the specified maximum order quantity (and create two or more supplies in order to reach the total order quantity), increase the order to the specified minimum order quantity, or round the order quantity up to meet a specified order multiple.</span></span>  

## <a name="combines-with-calendars"></a><span data-ttu-id="6d1d2-119">Associazioni con i calendari</span><span class="sxs-lookup"><span data-stu-id="6d1d2-119">Combines with Calendars</span></span>  
 <span data-ttu-id="6d1d2-120">Prima di suggerire un nuovo ordine di approvvigionamento per soddisfare un punto di riordino, il sistema di pianificazione verifica che l'ordine sia programmato per un giorno non lavorativo, in base ai calendari definiti nel campo **Codice calendario base** delle finestre **Informazioni società** e **Scheda Ubicazione**.</span><span class="sxs-lookup"><span data-stu-id="6d1d2-120">Before suggesting a new supply order to meet a reorder point, the planning system checks if the order is scheduled for a non-working day, according to any calendars that are defined in the **Base Calendar Code** field in the **Company Information** and **Location Card** windows.</span></span>  

 <span data-ttu-id="6d1d2-121">Se la data prevista è un giorno non lavorativo, il sistema di pianificazione sposta l'ordine al giorno lavorativo più vicino.</span><span class="sxs-lookup"><span data-stu-id="6d1d2-121">If the scheduled date is a non-working day, the planning system moves the order forward to the nearest working date.</span></span> <span data-ttu-id="6d1d2-122">In questo modo, potrebbe verificarsi che un ordine soddisfi un punto di riordino ma non una richiesta specifica.</span><span class="sxs-lookup"><span data-stu-id="6d1d2-122">This may result in an order that meets a reorder point but does not meet some specific demand.</span></span> <span data-ttu-id="6d1d2-123">Per tale richiesta non bilanciata, il sistema di pianificazione crea un approvvigionamento aggiuntivo.</span><span class="sxs-lookup"><span data-stu-id="6d1d2-123">For such unbalanced demand, the planning system creates an extra supply.</span></span>  

## <a name="should-not-be-used-with-forecast"></a><span data-ttu-id="6d1d2-124">Non deve essere utilizzato con la previsione</span><span class="sxs-lookup"><span data-stu-id="6d1d2-124">Should Not be Used with Forecast</span></span>  
 <span data-ttu-id="6d1d2-125">Poiché la domanda prevista è già espressa nel livello del punto di riordino non è necessario includere una previsione nella pianificazione di un articolo utilizzando un punto di riordino.</span><span class="sxs-lookup"><span data-stu-id="6d1d2-125">Because the anticipated demand is already expressed in the reorder point level it is not necessary to include a forecast in the planning of an item using a reorder point.</span></span> <span data-ttu-id="6d1d2-126">Se è necessario basare il piano su una previsione, utilizzare il metodo lotto per lotto.</span><span class="sxs-lookup"><span data-stu-id="6d1d2-126">If it is relevant to base the plan on a forecast, use the lot-for-lot policy.</span></span>  

## <a name="must-not-be-used-with-reservations"></a><span data-ttu-id="6d1d2-127">Non deve essere utilizzato con gli impegni</span><span class="sxs-lookup"><span data-stu-id="6d1d2-127">Must Not be Used with Reservations</span></span>  
 <span data-ttu-id="6d1d2-128">Se l'utente ha impegnato una quantità, ad esempio una quantità in magazzino, per una domanda remota, la struttura della pianificazione rimarrà alterata.</span><span class="sxs-lookup"><span data-stu-id="6d1d2-128">If the user has reserved a quantity, for instance a quantity in inventory, for some distant demand, the planning foundation will be disturbed.</span></span> <span data-ttu-id="6d1d2-129">Anche se il livello della quantità scorte previste è ammesso relativamente al punto di riordino, le quantità potrebbero non essere disponibili.</span><span class="sxs-lookup"><span data-stu-id="6d1d2-129">Even if the projected inventory level is acceptable in relation to the reorder point, the quantities might not be available.</span></span> <span data-ttu-id="6d1d2-130">Il sistema può provare a compensare creando ordini di eccezione; tuttavia, è consigliabile che il campo Impegno sia impostato su Mai negli articoli che sono pianificati utilizzando un punto di riordino.</span><span class="sxs-lookup"><span data-stu-id="6d1d2-130">The system may try to compensate for that by creating exception orders; however, it is recommended that the Reserve field is set to Never on items that are planned using a reorder point.</span></span>  

## <a name="see-also"></a><span data-ttu-id="6d1d2-131">Vedi anche</span><span class="sxs-lookup"><span data-stu-id="6d1d2-131">See Also</span></span>  
 <span data-ttu-id="6d1d2-132">[Dettagli di progettazione: Criteri di riordino](design-details-reordering-policies.md) </span><span class="sxs-lookup"><span data-stu-id="6d1d2-132">[Design Details: Reordering Policies](design-details-reordering-policies.md) </span></span>  
 <span data-ttu-id="6d1d2-133">[Dettagli di progettazione: Qtà Massima](design-details-maximum-qty.md) </span><span class="sxs-lookup"><span data-stu-id="6d1d2-133">[Design Details: Maximum Qty.](design-details-maximum-qty.md) </span></span>  
 <span data-ttu-id="6d1d2-134">[Dettagli di progettazione: Parametri di pianificazione](design-details-planning-parameters.md) </span><span class="sxs-lookup"><span data-stu-id="6d1d2-134">[Design Details: Planning Parameters](design-details-planning-parameters.md) </span></span>  
 <span data-ttu-id="6d1d2-135">[Dettagli di progettazione: Gestione dei metodi di riordino](design-details-handling-reordering-policies.md) </span><span class="sxs-lookup"><span data-stu-id="6d1d2-135">[Design Details: Handling Reordering Policies](design-details-handling-reordering-policies.md) </span></span>  
 [<span data-ttu-id="6d1d2-136">Dettagli di progettazione: Pianificazione approvvigionamento</span><span class="sxs-lookup"><span data-stu-id="6d1d2-136">Design Details: Supply Planning</span></span>](design-details-supply-planning.md)
