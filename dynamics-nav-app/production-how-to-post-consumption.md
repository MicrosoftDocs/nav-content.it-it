---
title: Come registrare il consumo tramite processo batch
description: "Se il metodo di consuntivazione è **Manuale**, i componenti devono essere registrati manualmente nelle registrazioni consumi."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 09/06/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: bd4cedaf3fdb2d0f5627120836580fc82f4befa3
ms.contentlocale: it-it
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-batch-post-production-consumption"></a><span data-ttu-id="0caae-103">Procedura: Registrare il consumo produzione tramite processo batch</span><span class="sxs-lookup"><span data-stu-id="0caae-103">How to: Batch Post Production Consumption</span></span>
<span data-ttu-id="0caae-104">Se il metodo di consuntivazione è **Manuale**, i componenti devono essere registrati manualmente nelle registrazioni consumi.</span><span class="sxs-lookup"><span data-stu-id="0caae-104">If the flushing method is **Manual**, you must post the components manually, using a consumption journal.</span></span>

<span data-ttu-id="0caae-105">È inoltre possibile impostare il sistema sulla registrazione (*consuntivazione*) automatica dei componenti quando si avviano o si chiudono ordini di produzione.</span><span class="sxs-lookup"><span data-stu-id="0caae-105">You can also set the system up to automatically post (*flush*) components when you start or finish production orders.</span></span> <span data-ttu-id="0caae-106">Per ulteriori informazioni vedere [Attivare la consuntivazione dei componenti in base all'output dell'operazione](production-how-to-flush-components-according-to-operation-output.md).</span><span class="sxs-lookup"><span data-stu-id="0caae-106">For more information, see [Enable Flushing of Components According to Operation Output](production-how-to-flush-components-according-to-operation-output.md).</span></span>

## <a name="to-post-consumption-for-one-or-more-production-order-lines"></a><span data-ttu-id="0caae-107">Per registrare il consumo per una o più righe dell'ordine di produzione</span><span class="sxs-lookup"><span data-stu-id="0caae-107">To post consumption for one or more production order lines</span></span>  
1.  <span data-ttu-id="0caae-108">Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **Registrazioni consumi**, quindi scegliere il collegamento correlato.</span><span class="sxs-lookup"><span data-stu-id="0caae-108">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Consumption Journal**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="0caae-109">Compilare i campi inserendo i dati relativi agli ordini di produzione e al consumo.</span><span class="sxs-lookup"><span data-stu-id="0caae-109">Fill in the fields with the production order data and the consumption data.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  

    <span data-ttu-id="0caae-110">Se l'ubicazione della warehouse in cui sono immagazzinati i componenti prevede l'utilizzo di collocazioni, ma non richiede l'elaborazione dei prelievi, assegnare un codice collocazione alla riga delle registrazioni per indicare da dove dovranno essere prelevati gli articoli nella warehouse.</span><span class="sxs-lookup"><span data-stu-id="0caae-110">If the warehouse location where the components are stored is set up to use bins but does not require pick processing, assign a bin code to the journal line to indicate where the items should be taken from in the warehouse.</span></span> <span data-ttu-id="0caae-111">Per ulteriori informazioni, vedere [Procedura: Prelevare per la produzione o l'assemblaggio](warehouse-how-to-pick-for-production.md).</span><span class="sxs-lookup"><span data-stu-id="0caae-111">For more information, see [How to: Pick for Production or Assembly](warehouse-how-to-pick-for-production.md).</span></span>  
3.  <span data-ttu-id="0caae-112">Per registrare il consumo scegliere l'azione **Registra**.</span><span class="sxs-lookup"><span data-stu-id="0caae-112">Choose the **Post** action to post the consumption.</span></span> <span data-ttu-id="0caae-113">I movimenti articolo collegati vengono ridotti.</span><span class="sxs-lookup"><span data-stu-id="0caae-113">The related item ledger entries are reduced.</span></span>

## <a name="see-also"></a><span data-ttu-id="0caae-114">Vedi anche</span><span class="sxs-lookup"><span data-stu-id="0caae-114">See Also</span></span>  
<span data-ttu-id="0caae-115">[Manufacturing](production-manage-manufacturing.md)  </span><span class="sxs-lookup"><span data-stu-id="0caae-115">[Manufacturing](production-manage-manufacturing.md)  </span></span>  
[<span data-ttu-id="0caae-116">Impostazione della produzione</span><span class="sxs-lookup"><span data-stu-id="0caae-116">Setting Up Manufacturing</span></span>](production-configure-production-processes.md)  
<span data-ttu-id="0caae-117">[Pianif.](production-planning.md)    </span><span class="sxs-lookup"><span data-stu-id="0caae-117">[Planning](production-planning.md)    </span></span>  
[<span data-ttu-id="0caae-118">Magazzino</span><span class="sxs-lookup"><span data-stu-id="0caae-118">Inventory</span></span>](inventory-manage-inventory.md)  
[<span data-ttu-id="0caae-119">Acquisti</span><span class="sxs-lookup"><span data-stu-id="0caae-119">Purchasing</span></span>](purchasing-manage-purchasing.md)  
<span data-ttu-id="0caae-120">[Utilizzo di [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="0caae-120">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
