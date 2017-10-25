---
title: Dettagli di progettazione - Domanda e approvvigionamento
description: Questo argomento introduce il concetto di domanda, ovvero il termine comune utilizzato per tutti i tipi di domanda lorda, ad esempio un ordine di vendita e un componente necessario da un ordine di produzione.
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: design, demand, supply, inventory, planning
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: d744b55835f5553e249a536e0fca0eb0046fda7b
ms.contentlocale: it-it
ms.lasthandoff: 10/16/2017

---
# <a name="design-details-demand-and-supply"></a><span data-ttu-id="db918-103">Dettagli di progettazione: Domanda e approvvigionamento</span><span class="sxs-lookup"><span data-stu-id="db918-103">Design Details: Demand and Supply</span></span>
<span data-ttu-id="db918-104">La domanda è il termine comune utilizzato per tutti i tipi di domanda lorda, ad esempio un ordine di vendita e un componente necessario da un ordine di produzione.</span><span class="sxs-lookup"><span data-stu-id="db918-104">Demand is the common term used for any kind of gross demand, such as a sales order and component need from a production order.</span></span> <span data-ttu-id="db918-105">Inoltre, il programma consente i tipi di domanda più tecnici, ad esempio resi di acquisto e delle giacenze negative.</span><span class="sxs-lookup"><span data-stu-id="db918-105">In addition, the program allows more technical types of demand, such as negative inventory and purchase returns.</span></span>  
  
<span data-ttu-id="db918-106">Approvvigionamento è il termine comune utilizzato per indicare qualsiasi genere di quantità in entrata o positiva, quale il magazzino, gli acquisti, l'assemblaggio, la produzione o i trasferimenti in entrata.</span><span class="sxs-lookup"><span data-stu-id="db918-106">Supply is the common term used for any kind of positive or inbound quantity, such as inventory, purchases, assembly, production, or inbound transfers.</span></span> <span data-ttu-id="db918-107">Inoltre, anche un reso di vendita può rappresentare un approvvigionamento.</span><span class="sxs-lookup"><span data-stu-id="db918-107">In addition, a sales return may also represent supply.</span></span>  
  
<span data-ttu-id="db918-108">Per ordinare le numerose origini di approvvigionamento e di domanda, il sistema di pianificazione le organizza su due righe chiamate profili di magazzino.</span><span class="sxs-lookup"><span data-stu-id="db918-108">To sort out the many sources of demand and supply, the planning system organizes them on two time lines called inventory profiles.</span></span> <span data-ttu-id="db918-109">Un profilo conserva gli eventi di domanda e l'altro conserva i corrispondenti eventi di approvvigionamento.</span><span class="sxs-lookup"><span data-stu-id="db918-109">One profile holds demand events, and the other holds the corresponding supply events.</span></span> <span data-ttu-id="db918-110">Ogni evento rappresenta un'entità di rete di ordini, ad esempio una riga ordine di vendita, un movimento contabile di magazzino o una riga di ordine di produzione.</span><span class="sxs-lookup"><span data-stu-id="db918-110">Each event represents one order network entity, such as a sales order line, an item ledger entry, or a production order line.</span></span>  
  
<span data-ttu-id="db918-111">Quando vengono caricati i profili di magazzino, i differenti set di domanda-approvvigionamento vengono bilanciati in modo da fornire un piano di approvvigionamento che soddisfi gli obiettivi elencati.</span><span class="sxs-lookup"><span data-stu-id="db918-111">When inventory profiles are loaded, the different demand-supply sets are balanced to output a supply plan that fulfills the listed goals.</span></span>  
  
<span data-ttu-id="db918-112">I parametri di pianificazione e i livelli di magazzino sono altri tipi rispettivamente di domanda e di approvvigionamento, che subiscono la contropartita integrata per rifornire gli articoli in stock.</span><span class="sxs-lookup"><span data-stu-id="db918-112">Planning parameters and inventory levels are other types of demand and supply respectively, which undergo integrated balancing to replenish stock items.</span></span> <span data-ttu-id="db918-113">Per ulteriori informazioni, vedere [Dettagli di programmazione: Gestione dei metodi di riordino](design-details-handling-reordering-policies.md).</span><span class="sxs-lookup"><span data-stu-id="db918-113">For more information, see [Design Details: Handling Reordering Policies](design-details-handling-reordering-policies.md).</span></span>  
  
## <a name="see-also"></a><span data-ttu-id="db918-114">Vedi anche</span><span class="sxs-lookup"><span data-stu-id="db918-114">See Also</span></span>  
<span data-ttu-id="db918-115">[Dettagli di progettazione: Bilanciamento domanda e approvvigionamento](design-details-balancing-demand-and-supply.md) </span><span class="sxs-lookup"><span data-stu-id="db918-115">[Design Details: Balancing Demand and Supply](design-details-balancing-demand-and-supply.md) </span></span>  
<span data-ttu-id="db918-116">[Dettagli di progettazione: Concetti centrali del sistema di pianificazione](design-details-central-concepts-of-the-planning-system.md) </span><span class="sxs-lookup"><span data-stu-id="db918-116">[Design Details: Central Concepts of the Planning System](design-details-central-concepts-of-the-planning-system.md) </span></span>  
[<span data-ttu-id="db918-117">Dettagli di progettazione: Pianificazione approvvigionamento</span><span class="sxs-lookup"><span data-stu-id="db918-117">Design Details: Supply Planning</span></span>](design-details-supply-planning.md)
