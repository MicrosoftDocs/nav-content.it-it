---
title: 'Procedura: Creare report elettronici di transazioni IVA'
description: "È necessario creare una lista di transazioni che includono l'IVA con importi oltre la soglia corrente effettuati entro la data specificata. Inviare il report alle autorità fiscali."
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
ms.openlocfilehash: 20bce3e89d70ffc1a21fc647ff98aeca50e4f64a
ms.contentlocale: it-it
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-create-electronic-vat-transactions-reports"></a><span data-ttu-id="de9df-104">Procedura: Creare report elettronici di transazioni IVA</span><span class="sxs-lookup"><span data-stu-id="de9df-104">How to: Create Electronic VAT Transactions Reports</span></span>
<span data-ttu-id="de9df-105">È necessario creare una lista di transazioni che includono l'IVA con importi oltre la soglia corrente effettuati entro la data specificata.</span><span class="sxs-lookup"><span data-stu-id="de9df-105">You must create a list of transactions that include VAT with amounts over the current threshold on or before the specified occurrence date.</span></span> <span data-ttu-id="de9df-106">Inviare il report alle autorità fiscali.</span><span class="sxs-lookup"><span data-stu-id="de9df-106">You submit this report to the tax authorities.</span></span>  

### <a name="to-create-a-vat-transactions-report"></a><span data-ttu-id="de9df-107">Per creare un report di transazioni IVA</span><span class="sxs-lookup"><span data-stu-id="de9df-107">To create a VAT transactions report</span></span>  

1.  <span data-ttu-id="de9df-108">Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **Report IVA**, quindi scegliere il collegamento correlato.</span><span class="sxs-lookup"><span data-stu-id="de9df-108">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **VAT Report**, and then choose the related link.</span></span>  

2.  <span data-ttu-id="de9df-109">Compilare i campi come indicato nella tabella seguente.</span><span class="sxs-lookup"><span data-stu-id="de9df-109">Fill in the fields as described in the following table.</span></span>  

    |<span data-ttu-id="de9df-110">Campo</span><span class="sxs-lookup"><span data-stu-id="de9df-110">Field</span></span>|<span data-ttu-id="de9df-111">Description</span><span class="sxs-lookup"><span data-stu-id="de9df-111">Description</span></span>|  
    |---
    <span data-ttu-id="de9df-112">titolo: Procedura: Creare report elettronici di transazioni IVA descrizione: È necessario creare una lista di transazioni che includono l'IVA con importi oltre la soglia corrente effettuati entro la data specificata.</span><span class="sxs-lookup"><span data-stu-id="de9df-112">title: How to Create Electronic VAT Transactions Reports description: You must create a list of transactions that include VAT with amounts over the current threshold on or before the specified occurrence date.</span></span> <span data-ttu-id="de9df-113">Inviare il report alle autorità fiscali.</span><span class="sxs-lookup"><span data-stu-id="de9df-113">You submit this report to the tax authorities.</span></span>

    <span data-ttu-id="de9df-114">documentationcenter: '' author: SorenGP</span><span class="sxs-lookup"><span data-stu-id="de9df-114">documentationcenter: '' author: SorenGP</span></span>

    <span data-ttu-id="de9df-115">ms.prod: "dynamics-nav-2017" ms.topic: article ms.devlang: na ms.tgt_pltfrm: na ms.workload: na ms.search.keywords: ms.date: 07/01/2017 ms.author: sgroespe</span><span class="sxs-lookup"><span data-stu-id="de9df-115">ms.prod: "dynamics-nav-2017" ms.topic: article ms.devlang: na ms.tgt_pltfrm: na ms.workload: na ms.search.keywords: ms.date: 07/01/2017 ms.author: sgroespe</span></span>

----------------------------------|---------------------------------------|  
    <span data-ttu-id="de9df-116">|**Senza contratto**|I movimenti IVA che hanno generato questa riga non sono associati a un contratto.|</span><span class="sxs-lookup"><span data-stu-id="de9df-116">|**Without Contract**|The VAT entries that resulted in this line are not associated with a contract.|</span></span>  
    <span data-ttu-id="de9df-117">|**Contratto**|I movimenti IVA che hanno generato questa riga sono associati a un contratto.|</span><span class="sxs-lookup"><span data-stu-id="de9df-117">|**Contract**|The VAT entries that resulted in this line are associated with a contract.|</span></span>  
    <span data-ttu-id="de9df-118">|**Altro**| I movimenti IVA che hanno generato questa riga non sono associati a un contratto speciale, ad esempio per manutenzione in corso o altre eccezioni.|</span><span class="sxs-lookup"><span data-stu-id="de9df-118">|**Other**|The VAT entries that resulted in this line are not associated with a special contract, such as ongoing maintenance or other exceptions.|</span></span>  

    > [!TIP]  
    >  In [!INCLUDE[navnow](../../includes/navnow_md.md)], the contract that the tax authorities are looking for can be blanket orders or service contracts. To identify if the VAT report line belongs to a blanket order or service contract, you can drill down to see the underlying VAT entries from the **Amount** field.  

     Credit memos are included in the VAT transaction report if the customer or vendor is from a country/region that is outside the EU and not black-listed. For more information, see [Italian VAT](italian-vat.md).  

 <span data-ttu-id="de9df-119">Dopo avere creato il report IVA, è necessario inviarlo alle autorità fiscali.</span><span class="sxs-lookup"><span data-stu-id="de9df-119">Now that you have created the VAT report, you must submit it to the tax authorities.</span></span> <span data-ttu-id="de9df-120">Per ulteriori informazioni, vedere [Procedura: Esportare i report di transazioni IVA](how-to-export-vat-transactions-reports.md).</span><span class="sxs-lookup"><span data-stu-id="de9df-120">For more information, see [How to: Export VAT Transactions Reports](how-to-export-vat-transactions-reports.md).</span></span>  

## <a name="see-also"></a><span data-ttu-id="de9df-121">Vedi anche</span><span class="sxs-lookup"><span data-stu-id="de9df-121">See Also</span></span>  
 [<span data-ttu-id="de9df-122">IVA italiana</span><span class="sxs-lookup"><span data-stu-id="de9df-122">Italian VAT</span></span>](italian-vat.md)

