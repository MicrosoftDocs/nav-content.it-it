---
title: Immissione di criteri di filtro
author: SusanneWindfeldPedersen
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 6b60b1344a1e18ad91863046110df880f75f7c04
ms.openlocfilehash: df386e1195db385ee053b69fec0f5082d8df4116
ms.contentlocale: it-it
ms.lasthandoff: 07/19/2017

---

# <a name="entering-criteria-in-filters"></a><span data-ttu-id="62267-102">Immissione di criteri di filtro</span><span class="sxs-lookup"><span data-stu-id="62267-102">Entering Criteria in Filters</span></span>
<span data-ttu-id="62267-103">Quando si desidera cercare dei dati, ad esempio nomi e indirizzi dei clienti o gruppi di prodotti, si immettono dei criteri.</span><span class="sxs-lookup"><span data-stu-id="62267-103">When you want to search for data, such as customer names, addresses, or product groups, you enter criteria.</span></span> <span data-ttu-id="62267-104">Nei criteri di ricerca è possibile utilizzare nel campo specificato tutti i numeri e le lettere che normalmente si utilizzano.</span><span class="sxs-lookup"><span data-stu-id="62267-104">In search criteria you can use all the numbers and letters that you normally use in the specific field.</span></span> <span data-ttu-id="62267-105">È inoltre possibile utilizzare alcuni simboli speciali per filtrare ulteriormente i risultati.</span><span class="sxs-lookup"><span data-stu-id="62267-105">In addition, you can use special symbols to further filter the results.</span></span>

## <a name="searching-using-the-quick-filter"></a><span data-ttu-id="62267-106">Ricerca con l'utilizzo di Filtro rapido</span><span class="sxs-lookup"><span data-stu-id="62267-106">Searching using the Quick Filter</span></span>
<span data-ttu-id="62267-107">È possibile aggiungere filtri a tutte le pagine, utilizzando la funzione Filtro rapido.</span><span class="sxs-lookup"><span data-stu-id="62267-107">You can add filters to all pages by using the Quick Filter.</span></span> <span data-ttu-id="62267-108">Questa funzione viene abilitata scegliendo l'icona della lente di ingrandimento che si trova nell'angolo superiore destro di una pagina.</span><span class="sxs-lookup"><span data-stu-id="62267-108">The Quick Filter is enabled by choosing the magnifier icon in the top right corner of a page.</span></span> <span data-ttu-id="62267-109">Questo tipo di filtro viene utilizzato per una rapida immissione dei criteri.</span><span class="sxs-lookup"><span data-stu-id="62267-109">This filtering type is used for a fast entry of criteria.</span></span>

<span data-ttu-id="62267-110">**Importante**: la funzione Filtro rapido consente di filtrare i dati facilmente immettendo testo normale, ma non offre molte opzioni di criteri di ricerca.</span><span class="sxs-lookup"><span data-stu-id="62267-110">**Important**: The Quick Filter provides an easy access to filter data by entering plain text, but does also provide a lot of search criteria options.</span></span> <span data-ttu-id="62267-111">A seconda se si immette il testo normale o il testo con i simboli, il filtro rapido funziona in modo diverso.</span><span class="sxs-lookup"><span data-stu-id="62267-111">Depending on whether you enter plain text or text including symbols, the Quick Filter behaves differently.</span></span>  
- <span data-ttu-id="62267-112">Se si immette testo normale nei criteri di ricerca, i criteri di ricerca vengono interpretati come una ricerca senza distinzione tra maiuscole e minuscole contenente un determinato testo.</span><span class="sxs-lookup"><span data-stu-id="62267-112">If you enter plain text in the search criteria, the search criteria is interpreted as a case insensitive search that contains certain text.</span></span>  
- <span data-ttu-id="62267-113">Se si immette del testo includendo dei simboli nei criteri di ricerca, i criteri di ricerca vengono interpretati esattamente così come sono stati immessi e la ricerca rileva la differenza tra maiuscole e minuscole.</span><span class="sxs-lookup"><span data-stu-id="62267-113">If you enter text including symbols in the search criteria, the search criteria is interpreted exactly as you entered it, and the search is case sensitive.</span></span>

### <a name="quick-filter-criteria"></a><span data-ttu-id="62267-114">Criteri di Filtro rapido</span><span class="sxs-lookup"><span data-stu-id="62267-114">Quick filter criteria</span></span>
<!-- html syntax because symbols conflict with MarkDown syntax -->
<TABLE>
  <TR>
    <TH><span data-ttu-id="62267-115">Criteri di ricerca</span><span class="sxs-lookup"><span data-stu-id="62267-115">Search Criteria</span></span></TH>
    <TH><span data-ttu-id="62267-116">Interpretato come...</span><span class="sxs-lookup"><span data-stu-id="62267-116">Interpreted as...</span></span></TH>
    <TH><span data-ttu-id="62267-117">Reso come...</span><span class="sxs-lookup"><span data-stu-id="62267-117">Returns...</span></span></TH>
  </TR>
  <TR>
    <TD><span data-ttu-id="62267-118">>man</span><span class="sxs-lookup"><span data-stu-id="62267-118">>man</span></span></TD>
    <TD><span data-ttu-id="62267-119">@*man*</span><span class="sxs-lookup"><span data-stu-id="62267-119">@*man*</span></span></TD>
    <TD><span data-ttu-id="62267-120">Tutti i record che contengono il testo man e senza distinzione tra maiuscole e minuscole.</span><span class="sxs-lookup"><span data-stu-id="62267-120">All records that contain the text man and case insensitive.</span></span></TD>
  </TR>
  <TR>
    <TD><span data-ttu-id="62267-121">>se</span><span class="sxs-lookup"><span data-stu-id="62267-121">>se</span></span></TD>
    <TD><span data-ttu-id="62267-122">@*se*</span><span class="sxs-lookup"><span data-stu-id="62267-122">@*se*</span></span></TD>
    <TD><span data-ttu-id="62267-123">Tutti i record che contengono il testo e e senza distinzione tra maiuscole e minuscole.</span><span class="sxs-lookup"><span data-stu-id="62267-123">All records that contain the text se and case insensitive.</span></span></TD>
  </TR>
  <TR>
    <TD><span data-ttu-id="62267-124">>Man*</span><span class="sxs-lookup"><span data-stu-id="62267-124">>Man*</span></span></TD>
    <TD><span data-ttu-id="62267-125">Inizia con Man e con distinzione tra maiuscole e minuscole.</span><span class="sxs-lookup"><span data-stu-id="62267-125">Starts with Man and case sensitive.</span></span></TD>
    <TD><span data-ttu-id="62267-126">Tutti i record che iniziano con il testo Man.</span><span class="sxs-lookup"><span data-stu-id="62267-126">All records that start with the text Man.</span></span></TD>
  </TR>
  <TR>
    <TD><span data-ttu-id="62267-127">'man'</span><span class="sxs-lookup"><span data-stu-id="62267-127">'man'</span></span></TD>
    <TD><span data-ttu-id="62267-128">Un testo esatto e con distinzione tra maiuscole e minuscole.</span><span class="sxs-lookup"><span data-stu-id="62267-128">An exact text and case sensitive.</span></span></TD>
    <TD><span data-ttu-id="62267-129">Tutti i record che corrispondono esattamente a man.</span><span class="sxs-lookup"><span data-stu-id="62267-129">All records that match man exactly.</span></span></TD>
  </TR>
  <TR>
    <TD><span data-ttu-id="62267-130">@*man</span><span class="sxs-lookup"><span data-stu-id="62267-130">@*man</span></span></TD>
    <TD><span data-ttu-id="62267-131">Termina con e senza distinzione tra maiuscole e minuscole.</span><span class="sxs-lookup"><span data-stu-id="62267-131">Ends with and case insensitive.</span></span></TD>
    <TD><span data-ttu-id="62267-132">Tutti i record che terminano con man.</span><span class="sxs-lookup"><span data-stu-id="62267-132">All records that end with man.</span></span></TD>
  </TR>
  <TR>
    <TD><span data-ttu-id="62267-133">@man*</span><span class="sxs-lookup"><span data-stu-id="62267-133">@man*</span></span></TD>
    <TD><span data-ttu-id="62267-134">Inizia con e senza distinzione tra maiuscole e minuscole.</span><span class="sxs-lookup"><span data-stu-id="62267-134">Starts with and case insensitive.</span></span></TD>
    <TD><span data-ttu-id="62267-135">Tutti i record che iniziano con man.</span><span class="sxs-lookup"><span data-stu-id="62267-135">All records that start with man.</span></span></TD>
  </TR>
</TABLE>

<span data-ttu-id="62267-136">**Nota**: non è possibile utilizzare i carattere jolly quando si filtrano i campi di enumerazione, come il campo **Stato** negli ordini di vendita.</span><span class="sxs-lookup"><span data-stu-id="62267-136">**Note**: You cannot use a wildcard when filtering on enumeration fields, such as the **Status** field on sales orders.</span></span> <span data-ttu-id="62267-137">Per immettere un filtro per il tipo di campo, è possibile immettere il valore numerico come parametro di filtro.</span><span class="sxs-lookup"><span data-stu-id="62267-137">To enter a filter for this type of field, you can enter the numeric value as a filtering parameter.</span></span> <span data-ttu-id="62267-138">Ad esempio, nel campo **Stato** in un ordine di vendita con i valori **Aperto**, **Rilasciato**, **In attesa di approvazione**e **Pagamento anticipato in sospeso**, utilizzare i valori **0**, **1**, **2**e **3** per filtrare in base a queste opzioni.</span><span class="sxs-lookup"><span data-stu-id="62267-138">For example, in the **Status** field on a sales order that has the values **Open**, **Released**, **Pending Approval**, and **Pending Prepayment**, use the values **0**, **1**, **2**, and **3** to filter for these options.</span></span>  

## <a name="see-also"></a><span data-ttu-id="62267-139">Vedi anche</span><span class="sxs-lookup"><span data-stu-id="62267-139">See Also</span></span>
[<span data-ttu-id="62267-140">Utilizzare Dynamics NAV</span><span class="sxs-lookup"><span data-stu-id="62267-140">Work with Dynamics NAV</span></span>](ui-work-product.md)

