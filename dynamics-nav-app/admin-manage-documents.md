---
title: Gestire, eliminare o comprimere documenti
description: Conservare i dati storici o eliminarli.
author: edupont04
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 09/01/2017
ms.author: edupont
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 89e541c7d38d26204c403636e4df11b7468bffa9
ms.contentlocale: it-it
ms.lasthandoff: 10/16/2017

---
# <a name="manage-documents"></a><span data-ttu-id="d59fd-103">Gestione dei documenti</span><span class="sxs-lookup"><span data-stu-id="d59fd-103">Manage Documents</span></span>
<span data-ttu-id="d59fd-104">Un ruolo centrale, ad esempio l'amministratore dell'applicazione, deve occuparsi regolarmente dell'accumularsi dei documenti storici, eliminandoli o comprimendoli.</span><span class="sxs-lookup"><span data-stu-id="d59fd-104">A central role, such as the application administrator, must regularly deal with accumulating historic documents by deleting or compressing them.</span></span>  

## <a name="delete-documents"></a><span data-ttu-id="d59fd-105">Eliminare documenti</span><span class="sxs-lookup"><span data-stu-id="d59fd-105">Delete Documents</span></span>
<span data-ttu-id="d59fd-106">In certe situazioni, si ha la necessità di eliminare degli ordini di acquisto fatturati.</span><span class="sxs-lookup"><span data-stu-id="d59fd-106">In certain situations, you may need to delete invoiced purchase orders that have not been deleted.</span></span> [!INCLUDE[d365fin](includes/d365fin_md.md)]<span data-ttu-id="d59fd-107"> verifica che gli ordini di acquisto eliminati siano stati completamente fatturati.</span><span class="sxs-lookup"><span data-stu-id="d59fd-107"> checks that you have fully invoiced the deleted purchase orders.</span></span> <span data-ttu-id="d59fd-108">Non è possibile eliminare ordini che non siano stati completamente fatturati e ricevuti.</span><span class="sxs-lookup"><span data-stu-id="d59fd-108">You cannot delete orders that you have not fully invoiced and received.</span></span>  

<span data-ttu-id="d59fd-109">Gli ordini di reso sono in genere eliminati dopo la fatturazione.</span><span class="sxs-lookup"><span data-stu-id="d59fd-109">Return orders are usually deleted after they are invoiced.</span></span> <span data-ttu-id="d59fd-110">Quando si registra una fattura, viene trasferita nella finestra **Note credito acq. registrate** .</span><span class="sxs-lookup"><span data-stu-id="d59fd-110">When you post an invoice, it is transferred to the **Posted Purchase Credit Memo** window.</span></span> <span data-ttu-id="d59fd-111">Se si seleziona la casella di controllo **Spediz. resi in nota credito** nella finestra **Setup contabilità fornitori**, la fattura viene trasferita nella finestra **spedizione reso registrata**.</span><span class="sxs-lookup"><span data-stu-id="d59fd-111">If you selected the **Return Shipment on Credit Memo** check box in the **Purchases & Payable Setup** window, then the invoice is transferred to the **Posted Return Shipment** window.</span></span> <span data-ttu-id="d59fd-112">È possibile eliminare i documenti mediante il processo batch **Rimuovi ordini resi acq. fatt.** .</span><span class="sxs-lookup"><span data-stu-id="d59fd-112">You can delete the documents using the **Delete Invd Purch. Ret. Orders** batch job.</span></span> <span data-ttu-id="d59fd-113">Prima di eliminarli, il processo batch verifica se gli ordini di reso acquisto sono completamente spediti e fatturati.</span><span class="sxs-lookup"><span data-stu-id="d59fd-113">Before deleting, the batch job checks if the purchase return orders are fully shipped and invoiced.</span></span>  

<span data-ttu-id="d59fd-114">Gli ordini di acquisto programmati non vengono eliminati dopo aver elaborato e fatturato tutti gli ordini di acquisto correlati.</span><span class="sxs-lookup"><span data-stu-id="d59fd-114">Blanket purchase orders are not deleted after you have processed and invoiced all the related purchase orders.</span></span> <span data-ttu-id="d59fd-115">È possibile eliminare ordini programmati tramite il processo batch **Elimina ordini acq. progr. fatturati**.</span><span class="sxs-lookup"><span data-stu-id="d59fd-115">You can delete blanket orders with the **Delete Invoiced Blanket Purchase Orders** batch job.</span></span>  

<span data-ttu-id="d59fd-116">Gli ordini di assistenza fatturati vengono in genere eliminati automaticamente dopo che sono stati completamente fatturati.</span><span class="sxs-lookup"><span data-stu-id="d59fd-116">Invoiced service orders are usually deleted automatically after having been fully invoiced.</span></span> <span data-ttu-id="d59fd-117">Quando si registra una fattura, viene creato un movimento corrispondente nella finestra **Fatture assistenza registrate**.</span><span class="sxs-lookup"><span data-stu-id="d59fd-117">When an invoice is posted, a corresponding entry is created in the **Posted Service Invoices** window.</span></span> <span data-ttu-id="d59fd-118">Il documento registrato può essere visualizzato nella finestra **Fattura assistenza registrata**.</span><span class="sxs-lookup"><span data-stu-id="d59fd-118">The posted document can be viewed in the **Posted Service Invoice** window.</span></span>  

<span data-ttu-id="d59fd-119">Gli ordini di assistenza non vengono, tuttavia, eliminati automaticamente se la quantità totale indicata nell'ordine è stata registrata non dall'ordine stesso, ma dalla finestra **Fattura assistenza**.</span><span class="sxs-lookup"><span data-stu-id="d59fd-119">Service orders are not deleted automatically, however, if the total quantity on the order has been posted not from the service order itself, but from the **Service Invoice** window.</span></span> <span data-ttu-id="d59fd-120">In questo caso può essere necessario eliminare ordini fatturati che non sono stati eliminati.</span><span class="sxs-lookup"><span data-stu-id="d59fd-120">Then you may need to delete invoiced orders that were not deleted.</span></span> <span data-ttu-id="d59fd-121">Per eseguire questa operazione, utilizzare il processo batch **Elimina ordini assistenza fatturati**.</span><span class="sxs-lookup"><span data-stu-id="d59fd-121">You can do this by running the **Delete Invoiced Service Orders** batch job.</span></span>  

## <a name="see-also"></a><span data-ttu-id="d59fd-122">Vedi anche</span><span class="sxs-lookup"><span data-stu-id="d59fd-122">See Also</span></span>  
[<span data-ttu-id="d59fd-123">Impostazione e amministrazione in Dynamics NAV</span><span class="sxs-lookup"><span data-stu-id="d59fd-123">Setup and Administration in Dynamics NAV</span></span>](admin-setup-and-administration.md)  
