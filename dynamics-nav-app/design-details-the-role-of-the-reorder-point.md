---
title: Dettagli di progettazione - Il ruolo del punto di riordino
description: "In questo argomento viene evidenziata l'importanza di impostare un punto di riordino, in modo da sapere quando è necessario approvvigionare il magazzino."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: desigh, reorder, demand, supply
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 8035a670077e53981e9c366d22bdb20df06d8c1b
ms.contentlocale: it-it
ms.lasthandoff: 10/16/2017

---
# <a name="design-details-the-role-of-the-reorder-point"></a><span data-ttu-id="4e89f-103">Dettagli di progettazione: Il ruolo del punto di riordino</span><span class="sxs-lookup"><span data-stu-id="4e89f-103">Design Details: The Role of the Reorder Point</span></span>
<span data-ttu-id="4e89f-104">Oltre alla contropartita generale di approvvigionamento e domanda, il sistema di pianificazione deve inoltre monitorare i livelli di magazzino per gli articoli interessati in modo che siano rispettati i metodi di riordino definiti:</span><span class="sxs-lookup"><span data-stu-id="4e89f-104">In addition to the general balancing of supply and demand, the planning system must also monitor inventory levels for the affected items to respect the defined reordering policies.</span></span>  
  
<span data-ttu-id="4e89f-105">Un punto di riordino rappresenta la domanda durante il lead time.</span><span class="sxs-lookup"><span data-stu-id="4e89f-105">A reorder point represents demand during lead time.</span></span> <span data-ttu-id="4e89f-106">Quando la giacenza disponibile scende sotto il livello di magazzino definito dal punto di riordino, è tempo di ordinare una maggiore quantità.</span><span class="sxs-lookup"><span data-stu-id="4e89f-106">When the projected inventory passes below the inventory level defined by the reorder point, it is time to order more quantity.</span></span> <span data-ttu-id="4e89f-107">Nel frattempo, si prevede una diminuzione graduale della giacenza, che possibilmente raggiunge lo zero (o il livello di scorta di sicurezza), finché non arriva il rifornimento.</span><span class="sxs-lookup"><span data-stu-id="4e89f-107">Meanwhile, the inventory is expected to decrease gradually and possibly reach zero (or the safety stock level), until the replenishment arrives.</span></span>  
  
<span data-ttu-id="4e89f-108">Di conseguenza, il sistema di pianificazione suggerirà un ordine di approvvigionamento programmato in avanti alla fase in cui la giacenza prevista passa al di sotto del punto di riordino.</span><span class="sxs-lookup"><span data-stu-id="4e89f-108">Accordingly, the planning system will suggest a forward-scheduled supply order at the point when the projected inventory passes below the reorder point.</span></span>  
  
<span data-ttu-id="4e89f-109">Il punto di riordino riflette un determinato livello di magazzino.</span><span class="sxs-lookup"><span data-stu-id="4e89f-109">The reorder point reflects a certain inventory level.</span></span> <span data-ttu-id="4e89f-110">Tuttavia, i livelli di magazzino possono spostarsi in modo significativo nell'intervallo di tempo e, pertanto, il sistema di pianificazione deve costantemente monitorare le scorte disponibili previste.</span><span class="sxs-lookup"><span data-stu-id="4e89f-110">However, inventory levels can move significantly during the time bucket and, therefore, the planning system must constantly monitor the projected available inventory.</span></span>  
  
## <a name="see-also"></a><span data-ttu-id="4e89f-111">Vedi anche</span><span class="sxs-lookup"><span data-stu-id="4e89f-111">See Also</span></span>  
<span data-ttu-id="4e89f-112">[Dettagli di progettazione: Criteri di riordino](design-details-reordering-policies.md) </span><span class="sxs-lookup"><span data-stu-id="4e89f-112">[Design Details: Reordering Policies](design-details-reordering-policies.md) </span></span>  
<span data-ttu-id="4e89f-113">[Dettagli di progettazione: Parametri di pianificazione](design-details-planning-parameters.md) </span><span class="sxs-lookup"><span data-stu-id="4e89f-113">[Design Details: Planning Parameters](design-details-planning-parameters.md) </span></span>  
<span data-ttu-id="4e89f-114">[Dettagli di progettazione: Gestione dei metodi di riordino](design-details-handling-reordering-policies.md) </span><span class="sxs-lookup"><span data-stu-id="4e89f-114">[Design Details: Handling Reordering Policies](design-details-handling-reordering-policies.md) </span></span>  
[<span data-ttu-id="4e89f-115">Dettagli di progettazione: Pianificazione approvvigionamento</span><span class="sxs-lookup"><span data-stu-id="4e89f-115">Design Details: Supply Planning</span></span>](design-details-supply-planning.md)