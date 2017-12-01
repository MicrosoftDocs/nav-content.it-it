---
title: 'Procedura: Creare report elettronici di transazioni IVA'
description: "È necessario creare una lista di transazioni che includono l'IVA con importi oltre la soglia corrente effettuati entro la data specificata. Inviare il report alle autorità fiscali."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 1dfba8b14019991c95f40ffd5f7fbaed5df414eb
ms.openlocfilehash: 8bcc217ab8e88632bfd29e41c8d2f554bc4d9db3
ms.contentlocale: it-it
ms.lasthandoff: 12/01/2017

---
# <a name="how-to-create-electronic-vat-transactions-reports"></a><span data-ttu-id="82313-104">Procedura: Creare report elettronici di transazioni IVA</span><span class="sxs-lookup"><span data-stu-id="82313-104">How to: Create Electronic VAT Transactions Reports</span></span>
<span data-ttu-id="82313-105">È necessario creare una lista di transazioni che includono l'IVA con importi oltre la soglia corrente effettuati entro la data specificata.</span><span class="sxs-lookup"><span data-stu-id="82313-105">You must create a list of transactions that include VAT with amounts over the current threshold on or before the specified occurrence date.</span></span> <span data-ttu-id="82313-106">Inviare il report alle autorità fiscali.</span><span class="sxs-lookup"><span data-stu-id="82313-106">You submit this report to the tax authorities.</span></span>  

## <a name="to-create-a-vat-transactions-report"></a><span data-ttu-id="82313-107">Per creare un report di transazioni IVA</span><span class="sxs-lookup"><span data-stu-id="82313-107">To create a VAT transactions report</span></span>  

1.  <span data-ttu-id="82313-108">Scegliere l'icona ![Cerca pagina o report](../../media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **Report IVA**, quindi scegliere il collegamento correlato.</span><span class="sxs-lookup"><span data-stu-id="82313-108">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **VAT Report**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="82313-109">Compilare i campi come indicato nella tabella seguente.</span><span class="sxs-lookup"><span data-stu-id="82313-109">Fill in the fields as described in the following table.</span></span>  

    |<span data-ttu-id="82313-110">Campo</span><span class="sxs-lookup"><span data-stu-id="82313-110">Field</span></span>|<span data-ttu-id="82313-111">Description</span><span class="sxs-lookup"><span data-stu-id="82313-111">Description</span></span>|  
    |-------------------------------------|---------------------------------------|  
    |<span data-ttu-id="82313-112">**Senza contratto**</span><span class="sxs-lookup"><span data-stu-id="82313-112">**Without Contract**</span></span>|<span data-ttu-id="82313-113">I movimenti IVA che hanno generato questa riga non sono associati a un contratto.</span><span class="sxs-lookup"><span data-stu-id="82313-113">The VAT entries that resulted in this line are not associated with a contract.</span></span>|  
    |<span data-ttu-id="82313-114">**Contratto**</span><span class="sxs-lookup"><span data-stu-id="82313-114">**Contract**</span></span>|<span data-ttu-id="82313-115">I movimenti IVA che hanno generato questa riga sono associati a un contratto.</span><span class="sxs-lookup"><span data-stu-id="82313-115">The VAT entries that resulted in this line are associated with a contract.</span></span>|  
    |<span data-ttu-id="82313-116">**Altro**</span><span class="sxs-lookup"><span data-stu-id="82313-116">**Other**</span></span>|<span data-ttu-id="82313-117">I movimenti IVA che hanno generato questa riga non sono associati a un contratto speciale, ad esempio per manutenzione in corso o altre eccezioni.</span><span class="sxs-lookup"><span data-stu-id="82313-117">The VAT entries that resulted in this line are not associated with a special contract, such as ongoing maintenance or other exceptions.</span></span>|  

    > [!TIP]  
    >  <span data-ttu-id="82313-118">In [!INCLUDE[navnow](../../includes/navnow_md.md)], il contratto che le autorità fiscali cercano può essere ordini programmati oppure contratti di assistenza.</span><span class="sxs-lookup"><span data-stu-id="82313-118">In [!INCLUDE[navnow](../../includes/navnow_md.md)], the contract that the tax authorities are looking for can be blanket orders or service contracts.</span></span> <span data-ttu-id="82313-119">Per identificare se la riga del report IVA appartiene a un ordine programmato o a un contratto di assistenza, è possibile eseguire il drill-down per visualizzare i movimenti IVA sottostanti dal campo **Importo**.</span><span class="sxs-lookup"><span data-stu-id="82313-119">To identify if the VAT report line belongs to a blanket order or service contract, you can drill down to see the underlying VAT entries from the **Amount** field.</span></span>  

<span data-ttu-id="82313-120">Le note di credito vengono incluse nel report transazioni IVA se il cliente o il fornitore è di un paese esterno all'UE e non incluso nella blacklist.</span><span class="sxs-lookup"><span data-stu-id="82313-120">Credit memos are included in the VAT transaction report if the customer or vendor is from a country/region that is outside the EU and not black-listed.</span></span> <span data-ttu-id="82313-121">Per ulteriori informazioni, vedere [IVA italiana](italian-vat.md).</span><span class="sxs-lookup"><span data-stu-id="82313-121">For more information, see [Italian VAT](italian-vat.md).</span></span>  

<span data-ttu-id="82313-122">Dopo avere creato il report IVA, è necessario inviarlo alle autorità fiscali.</span><span class="sxs-lookup"><span data-stu-id="82313-122">Now that you have created the VAT report, you must submit it to the tax authorities.</span></span> <span data-ttu-id="82313-123">Per ulteriori informazioni, vedere [Procedura: Esportare i report di transazioni IVA](how-to-export-vat-transactions-reports.md).</span><span class="sxs-lookup"><span data-stu-id="82313-123">For more information, see [How to: Export VAT Transactions Reports](how-to-export-vat-transactions-reports.md).</span></span>  

## <a name="see-also"></a><span data-ttu-id="82313-124">Vedi anche</span><span class="sxs-lookup"><span data-stu-id="82313-124">See Also</span></span>  
 [<span data-ttu-id="82313-125">IVA italiana</span><span class="sxs-lookup"><span data-stu-id="82313-125">Italian VAT</span></span>](italian-vat.md)

