---
title: Come trasferire movimenti C/G ai movimenti di costi
description: I movimenti C/G possono essere trasferiti ai movimenti di costi.
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
ms.openlocfilehash: b7a78fb1023e8b664fd866eb1a8b5e42ff0de265
ms.contentlocale: it-it
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-transfer-general-ledger-entries-to-cost-entries"></a><span data-ttu-id="0b8d7-103">Procedura: Trasferire movimenti C/G ai movimenti di costi</span><span class="sxs-lookup"><span data-stu-id="0b8d7-103">How to: Transfer General Ledger Entries to Cost Entries</span></span>
<span data-ttu-id="0b8d7-104">I movimenti C/G possono essere trasferiti ai movimenti di costi.</span><span class="sxs-lookup"><span data-stu-id="0b8d7-104">You can transfer general ledger entries to cost entries.</span></span>  

<span data-ttu-id="0b8d7-105">Prima di eseguire il processo per il trasferimento dei movimenti C/G ai movimenti di costi, è necessario preparare il trasferimento per evitare la registrazione manuale della correzione.</span><span class="sxs-lookup"><span data-stu-id="0b8d7-105">Before you run the process for transferring general ledger entries to cost entries, you must prepare the transfer to avoid manual correction posting.</span></span>  

## <a name="to-prepare-the-transfer"></a><span data-ttu-id="0b8d7-106">Per preparare il trasferimento</span><span class="sxs-lookup"><span data-stu-id="0b8d7-106">To prepare the transfer</span></span>  

1.  <span data-ttu-id="0b8d7-107">Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **Setup contabilità industriale**, quindi scegliere il collegamento correlato.</span><span class="sxs-lookup"><span data-stu-id="0b8d7-107">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Cost Accounting Setup**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="0b8d7-108">Nella finestra **Setup contabilità industriale** controllare che il campo **Data inizio per trasferimento C/G** sia impostato sul valore corretto.</span><span class="sxs-lookup"><span data-stu-id="0b8d7-108">In the **Cost Accounting Setup** window, verify that the **Starting Date for G/L Transfer** field is set to the correct value.</span></span>  
3.  <span data-ttu-id="0b8d7-109">Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **Piano dei tipi di costo**, quindi scegliere il collegamento correlato.</span><span class="sxs-lookup"><span data-stu-id="0b8d7-109">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Chart of Cost Types**, and then choose the related link.</span></span>  
4.  <span data-ttu-id="0b8d7-110">Nella finestra **Scheda tipo costo** verificare che il campo **Intervallo conti C/G** sia collegato correttamente per ogni tipo di costo per prelevare i movimenti dalla contabilità generale.</span><span class="sxs-lookup"><span data-stu-id="0b8d7-110">In the **Cost Type Card** window, verify that the **G/L Account Range** field is linked correctly for each cost type to take entries from the general ledger.</span></span>  
5.  <span data-ttu-id="0b8d7-111">Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **Piano dei conti**, quindi scegliere il collegamento correlato.</span><span class="sxs-lookup"><span data-stu-id="0b8d7-111">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Chart of Accounts**, and then choose the related link.</span></span>  
6.  <span data-ttu-id="0b8d7-112">Per ogni conto di contabilità generale pertinente, nella finestra **Scheda conto C/G** verificare che il campo **Nr. tipo di costo**</span><span class="sxs-lookup"><span data-stu-id="0b8d7-112">For each relevant general ledger account, in the **G/L Account Card** window, verify that the **Cost Type No.**</span></span> <span data-ttu-id="0b8d7-113">sia collegato correttamente a un tipo di costo.</span><span class="sxs-lookup"><span data-stu-id="0b8d7-113">field is linked correctly to a cost type.</span></span> <span data-ttu-id="0b8d7-114">Per ulteriori informazioni, vedere [Definizione della relazione tra i tipi di costo e i conti di contabilità generale](finance-defining-the-relationship-between-cost-types-and-general-ledger-accounts.md).</span><span class="sxs-lookup"><span data-stu-id="0b8d7-114">For more information, see [Defining the Relationship Between Cost Types and General Ledger Accounts](finance-defining-the-relationship-between-cost-types-and-general-ledger-accounts.md).</span></span>  
7.  <span data-ttu-id="0b8d7-115">Verificare che a tutti i relativi movimenti C/G siano associati valori dimensioni che corrispondono a un centro di costo e a un oggetto di costo.</span><span class="sxs-lookup"><span data-stu-id="0b8d7-115">Verify that all relevant general ledger entries have dimension values that correspond to a cost center and a cost object.</span></span>  

## <a name="to-transfer-general-ledger-entries-to-cost-entries"></a><span data-ttu-id="0b8d7-116">Per trasferire movimenti C/G a movimenti di costi</span><span class="sxs-lookup"><span data-stu-id="0b8d7-116">To transfer general ledger entries to cost entries</span></span>  
1.  <span data-ttu-id="0b8d7-117">Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **Trasferisci movimenti C/G a CA**, quindi scegliere il collegamento correlato.</span><span class="sxs-lookup"><span data-stu-id="0b8d7-117">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Transfer GL Entries to CA**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="0b8d7-118">Scegliere **Sì** per avviare il trasferimento.</span><span class="sxs-lookup"><span data-stu-id="0b8d7-118">Choose the **Yes** button to start the transfer.</span></span> <span data-ttu-id="0b8d7-119">Con il processo vengono trasferiti tutti i movimenti C/G che non sono già stati trasferiti.</span><span class="sxs-lookup"><span data-stu-id="0b8d7-119">The process transfers all general ledger entries that have not already been transferred.</span></span>  

    <span data-ttu-id="0b8d7-120">Durante il trasferimento, con il processo vengono creati collegamenti nei movimenti nella tabella **Movimento di costo** e nella tabella **Registro costi**.</span><span class="sxs-lookup"><span data-stu-id="0b8d7-120">During the transfer, the process creates connections in the entries in the **Cost Entry** table and the **Cost Register** table.</span></span> <span data-ttu-id="0b8d7-121">In questo modo è possibile analizzare l'origine dei movimenti di costi.</span><span class="sxs-lookup"><span data-stu-id="0b8d7-121">This makes it possible to trace the source of cost entries.</span></span>  

## <a name="see-also"></a><span data-ttu-id="0b8d7-122">Vedi anche</span><span class="sxs-lookup"><span data-stu-id="0b8d7-122">See Also</span></span>  
 <span data-ttu-id="0b8d7-123">[Criteri per trasferire movimenti C/G ai movimenti di costi](finance-criteria-for-transferring-general-ledger-entries-to-cost-entries.md) </span><span class="sxs-lookup"><span data-stu-id="0b8d7-123">[Criteria for Transferring General Ledger Entries to Cost Entries](finance-criteria-for-transferring-general-ledger-entries-to-cost-entries.md) </span></span>  
 <span data-ttu-id="0b8d7-124">[Trasferimento automatico e movimenti combinati](finance-automatic-transfer-combined-entries.md) </span><span class="sxs-lookup"><span data-stu-id="0b8d7-124">[Automatic Transfer and Combined Entries](finance-automatic-transfer-combined-entries.md) </span></span>  
 <span data-ttu-id="0b8d7-125">[Risultati del trasferimento](finance-results-of-the-transfer.md) </span><span class="sxs-lookup"><span data-stu-id="0b8d7-125">[Results of the Transfer](finance-results-of-the-transfer.md) </span></span>  
 <span data-ttu-id="0b8d7-126">[Trasferimento e registrazione di movimenti di costi](finance-transfer-and-post-cost-entries.md) </span><span class="sxs-lookup"><span data-stu-id="0b8d7-126">[Transferring and Posting Cost Entries](finance-transfer-and-post-cost-entries.md) </span></span>  
 [<span data-ttu-id="0b8d7-127">Definizione della relazione tra i tipi di costo e i conti di contabilità generale</span><span class="sxs-lookup"><span data-stu-id="0b8d7-127">Defining the Relationship Between Cost Types and General Ledger Accounts</span></span>](finance-defining-the-relationship-between-cost-types-and-general-ledger-accounts.md)   
