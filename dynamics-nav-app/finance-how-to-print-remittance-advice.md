---
title: Come stampare l'avviso di rimessa
description: "È possibile aiutare i fornitori a eseguire le riconciliazioni stampando l'avviso di rimessa prima di effettuare una registrazione pagamenti e dopo la registrazione di un pagamento."
documentationcenter: 
author: bholtorf
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 10/26/2017
ms.author: bholtorf
ms.translationtype: HT
ms.sourcegitcommit: a16640e014e157d4dbcaabc53d0df2d3e063f8f9
ms.openlocfilehash: 71c84b4a7bad83e6008c0fa34f908e133b014a59
ms.contentlocale: it-it
ms.lasthandoff: 10/26/2017

---

#<a name="how-to-print-remittance-advice"></a><span data-ttu-id="82bd4-103">Procedura: Stampare l'avviso di rimessa</span><span class="sxs-lookup"><span data-stu-id="82bd4-103">How to: Print Remittance Advice</span></span>
<span data-ttu-id="82bd4-104">È possibile stampare l'avviso di rimessa prima di eseguire una registrazione pagamenti e dopo la registrazione di un pagamento.</span><span class="sxs-lookup"><span data-stu-id="82bd4-104">You can print remittance advice before posting a payment journal and after posting a payment.</span></span> <span data-ttu-id="82bd4-105">Questo avviso visualizza i numeri delle fatture fornitore e consente ai fornitori di eseguire le riconciliazioni.</span><span class="sxs-lookup"><span data-stu-id="82bd4-105">This advice displays vendor invoice numbers, which helps vendors to perform reconciliations.</span></span>

##<a name="to-print-remittance-advice"></a><span data-ttu-id="82bd4-106">Per stampare l'avviso di rimessa</span><span class="sxs-lookup"><span data-stu-id="82bd4-106">To print remittance advice</span></span>
1. <span data-ttu-id="82bd4-107">Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **Registrazioni pagamenti**, quindi scegliere il collegamento correlato.</span><span class="sxs-lookup"><span data-stu-id="82bd4-107">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Payment Journals**, and then choose the related link.</span></span>  
2. <span data-ttu-id="82bd4-108">Nella finestra **Registrazioni pagamenti**, selezionare il pagamento per il quale l'avviso di rimessa deve essere stampato.</span><span class="sxs-lookup"><span data-stu-id="82bd4-108">In the **Payment Journal** window, select the payment for which remittance advice must be printed.</span></span>  
3. <span data-ttu-id="82bd4-109">Scegliere l'azione **Stampa avviso di rimessa**.</span><span class="sxs-lookup"><span data-stu-id="82bd4-109">Choose the **Print Remittance Advice** action.</span></span>  
4. <span data-ttu-id="82bd4-110">Nel processo batch **Avviso di rimessa - Giornale di registrazione**, nella Scheda dettaglio **Righe registrazioni COGE**, scegliere i filtri appropriati.</span><span class="sxs-lookup"><span data-stu-id="82bd4-110">In the **Remittance Advice - Journal** batch job, on the **Fen. Journal Line** FastTab, choose the appropriate filters.</span></span>  
  
    >[!Note]
    > <span data-ttu-id="82bd4-111">È possibile filtrare utilizzando il numero di documento esterno del fornitore per la corrispondenza tra pagamenti e fatture.</span><span class="sxs-lookup"><span data-stu-id="82bd4-111">You can filter using the vendor's external document number to match payments with invoices.</span></span>

5. <span data-ttu-id="82bd4-112">Nella Scheda dettaglio **Fornitore**, scegliere i filtri appropriati.</span><span class="sxs-lookup"><span data-stu-id="82bd4-112">On the **Vendor** FastTab, choose the appropriate filters.</span></span>  
6. <span data-ttu-id="82bd4-113">Scegliere **Stampa** per stampare il report o **Anteprima** per visualizzarlo.</span><span class="sxs-lookup"><span data-stu-id="82bd4-113">Choose **Print** to print the report, or choose **Preview** to view it now.</span></span>  

## <a name="using-remittance-advice-reports"></a><span data-ttu-id="82bd4-114">Utilizzo dii report relativi agli avvisi di rimessa</span><span class="sxs-lookup"><span data-stu-id="82bd4-114">Using Remittance Advice Reports</span></span>
<span data-ttu-id="82bd4-115">Nella tabella seguente sono descritti i report utilizzabili con l'avviso di rimessa:</span><span class="sxs-lookup"><span data-stu-id="82bd4-115">The following table describes the reports that you can use with remittance advice:</span></span>

|<span data-ttu-id="82bd4-116">Report</span><span class="sxs-lookup"><span data-stu-id="82bd4-116">Report</span></span>|<span data-ttu-id="82bd4-117">Description</span><span class="sxs-lookup"><span data-stu-id="82bd4-117">Description</span></span>|
|----|----|
|<span data-ttu-id="82bd4-118">Report Avviso di rimessa - Giornale di registrazione</span><span class="sxs-lookup"><span data-stu-id="82bd4-118">Remittance Advice - Journal Report</span></span>|<span data-ttu-id="82bd4-119">In questo report sono indicati i documenti inclusi nel pagamento.</span><span class="sxs-lookup"><span data-stu-id="82bd4-119">This report indicates which documents are included in the payment.</span></span> <span data-ttu-id="82bd4-120">Per le righe delle registrazioni COGE, è possibile specificare il modello di registrazioni e il batch registrazioni da cui gli avvisi di rimessa verranno stampati, la data della prima attività da stampare e il filtro per un numero di documento.</span><span class="sxs-lookup"><span data-stu-id="82bd4-120">For general journal lines, you can specify the journal template and journal batch from which the remittance advices will be printed, the date of the first activity to print, and filter on a document number.</span></span> <span data-ttu-id="82bd4-121">Per i fornitori, è possibile immettere il numero dei fornitori da includere nel report.</span><span class="sxs-lookup"><span data-stu-id="82bd4-121">For vendors, you can enter the vendor numbers to include in the report.</span></span> |
|<span data-ttu-id="82bd4-122">Report Avviso di rimessa - Movimenti</span><span class="sxs-lookup"><span data-stu-id="82bd4-122">Remittance Advice - Entries Report</span></span>| <span data-ttu-id="82bd4-123">In questo report sono indicati i documenti inclusi nel pagamento.</span><span class="sxs-lookup"><span data-stu-id="82bd4-123">This report indicates which documents are included in the payment.</span></span> <span data-ttu-id="82bd4-124">È possibile definire il contenuto del report impostando dei filtri.</span><span class="sxs-lookup"><span data-stu-id="82bd4-124">You define the report contents by setting filters.</span></span> <span data-ttu-id="82bd4-125">È possibile impostare ulteriori campi nella scheda scegliendo il campo **Campo**.</span><span class="sxs-lookup"><span data-stu-id="82bd4-125">You can set additional fields on the tab by choosing the **Field** field.</span></span> <span data-ttu-id="82bd4-126">Per i movimenti contabili fornitori, è possibile specificare i fornitori da includere nel report, la data della prima attività da stampare, la valuta e il numero di movimento da includere.</span><span class="sxs-lookup"><span data-stu-id="82bd4-126">For vendor ledger entries, you can specify the vendors to include in the report, the date of the first activity to print, the currency, and the entry number to include.</span></span> |

> [!Note]
> <span data-ttu-id="82bd4-127">Il report Avviso di rimessa - Giornale di registrazione non supporta gli scenari di applicazione per valute o le tolleranze di pagamento.</span><span class="sxs-lookup"><span data-stu-id="82bd4-127">The Remittance Advice - Journal Report does not support cross currency application scenarios or payment tolerances.</span></span> <span data-ttu-id="82bd4-128">Per ulteriori informazioni, vedere [Procedura: Abilitare il collegamento dei movimenti contabili fornitore in valute diverse](finance-how-enable-application-ledger-entries-different-currencies.md).</span><span class="sxs-lookup"><span data-stu-id="82bd4-128">For more information, see [How to: Enable Application of Ledger Entries in Different Currencies](finance-how-enable-application-ledger-entries-different-currencies.md).</span></span>

> [!Tip]
> <span data-ttu-id="82bd4-129">Per ulteriori informazioni su come utilizzare i report, vedere, [Visualizzazione di report test prima della registrazione](ui-how-view-test-reports-posting.md), [Utilizzare i report](ui-work-report.md) e [Ricerca, filtro e ordinamento di dati](ui-enter-criteria-filters.md).</span><span class="sxs-lookup"><span data-stu-id="82bd4-129">For more information about how to work with reports, see [Viewing Test Reports before Posting](ui-how-view-test-reports-posting.md), [Work with Reports](ui-work-report.md), and [Searching, Filtering, and Sorting Data](ui-enter-criteria-filters.md).</span></span>

##<a name="see-also"></a><span data-ttu-id="82bd4-130">Vedi anche</span><span class="sxs-lookup"><span data-stu-id="82bd4-130">See Also</span></span>  
[<span data-ttu-id="82bd4-131">Benvenuto in Dynamics NAV</span><span class="sxs-lookup"><span data-stu-id="82bd4-131">Welcome to Dynamics NAV</span></span>](across-get-started.md)
