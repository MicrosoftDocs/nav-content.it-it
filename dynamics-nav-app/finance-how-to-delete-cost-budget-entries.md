---
title: Come eliminare i movimenti budget costi
description: Utilizzare il processo batch **Elimina mov. budget costi** per annullare i movimenti di budget costi dal registro budget costi.
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
ms.openlocfilehash: 16c471b7c03d8b53049ad2284dbe4fa058dd3ca9
ms.contentlocale: it-it
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-delete-cost-budget-entries"></a><span data-ttu-id="dfa71-103">Procedura: eliminare i mov. budget costi</span><span class="sxs-lookup"><span data-stu-id="dfa71-103">How to: Delete Cost Budget Entries</span></span>
<span data-ttu-id="dfa71-104">Utilizzare il processo batch **Elimina mov. budget costi** per annullare i movimenti di budget costi dal registro budget costi.</span><span class="sxs-lookup"><span data-stu-id="dfa71-104">You use the **Delete Cost Budget Entries** batch job to cancel cost budget entries from the cost budget register.</span></span>  

<span data-ttu-id="dfa71-105">Per evitare qualsiasi gap nei movimenti di budget costi e nei movimenti del registro dei costi, non è possibile eliminare un unico movimento o un batch di movimenti a metà della lista dei movimenti del registro.</span><span class="sxs-lookup"><span data-stu-id="dfa71-105">To prevent any gaps in the cost budget entries and cost register entries, you cannot delete a single entry or a batch of entries in the middle of the list of register entries.</span></span>  

### <a name="to-delete-a-cost-budget-entry"></a><span data-ttu-id="dfa71-106">Per eliminare un mov. budget costi</span><span class="sxs-lookup"><span data-stu-id="dfa71-106">To delete a cost budget entry</span></span>  

1.  <span data-ttu-id="dfa71-107">Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **Elimina mov. budget costi**, quindi scegliere il collegamento correlato.</span><span class="sxs-lookup"><span data-stu-id="dfa71-107">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Delete Cost Budget Entries**, and then choose the related link.</span></span>  

    <span data-ttu-id="dfa71-108">Nel campo **A nr. registro**</span><span class="sxs-lookup"><span data-stu-id="dfa71-108">The **To Register No.**</span></span> <span data-ttu-id="dfa71-109">è incluso l'ultimo numero del movimento del registro e non può essere modificato.</span><span class="sxs-lookup"><span data-stu-id="dfa71-109">field contains the last register entry number and cannot be changed.</span></span>  

    <span data-ttu-id="dfa71-110">È possibile utilizzare il campo **Da nr. registro**</span><span class="sxs-lookup"><span data-stu-id="dfa71-110">You can use the **From Register No.**</span></span> <span data-ttu-id="dfa71-111">per selezionare un numero di movimento del registro dal quale iniziare l'eliminazione.</span><span class="sxs-lookup"><span data-stu-id="dfa71-111">field to select a register entry number from which the deletion should begin.</span></span>  
2.  <span data-ttu-id="dfa71-112">Scegliere il pulsante **OK** per eliminare i movimenti di bugdet costi selezionati.</span><span class="sxs-lookup"><span data-stu-id="dfa71-112">Choose the **OK** button to delete the selected cost budget entries.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="dfa71-113">Per evitare un'eliminazione accidentale dei movimenti di budget costi, è possibile chiudere i movimenti del registro contrassegnando le righe come **Chiuso** nel campo **Chiuso** della finestra **Registri budget costi**.</span><span class="sxs-lookup"><span data-stu-id="dfa71-113">To avoid an accidental deletion of cost budget entries, you can close register entries by marking the lines as **Closed** in the **Closed** field in the **Cost Budget Registers** window.</span></span>  

## <a name="see-also"></a><span data-ttu-id="dfa71-114">Vedi anche</span><span class="sxs-lookup"><span data-stu-id="dfa71-114">See Also</span></span>  
<span data-ttu-id="dfa71-115">[Contabilizzazione dei costi](finance-manage-cost-accounting.md)
[Creazione di budget di costi](finance-create-cost-budgets.md)</span><span class="sxs-lookup"><span data-stu-id="dfa71-115">[Accounting for Costs](finance-manage-cost-accounting.md)
[Creating Cost Budgets](finance-create-cost-budgets.md)</span></span>  
<span data-ttu-id="dfa71-116">[Utilizzo di [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="dfa71-116">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
