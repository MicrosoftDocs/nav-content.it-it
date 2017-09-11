---
title: 'Procedura: Registrare il movimento di chiusura di fine anno'
author: jswymer
ms.custom: na
ms.date: 09/16/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 6b60b1344a1e18ad91863046110df880f75f7c04
ms.openlocfilehash: fe32ee973c90ba857852ae092acf03db09e648ee
ms.contentlocale: it-it
ms.lasthandoff: 07/19/2017

---
# <a name="how-to-post-year-end-closing-entry"></a><span data-ttu-id="b88c2-102">Procedura: Registrare il movimento di chiusura di fine anno</span><span class="sxs-lookup"><span data-stu-id="b88c2-102">How to: Post Year-End Closing Entry</span></span>
<span data-ttu-id="b88c2-103">Nell'ambito della chiusura dei registri contabili relativi a un anno fiscale verrà eseguito il processo batch Chiudi conto economico per trasferire i risultati dell'anno su un conto dello stato patrimoniale e chiudere i conti economici.</span><span class="sxs-lookup"><span data-stu-id="b88c2-103">As part of closing the books for a fiscal year, you will run the Close Income Statement batch job to transfer the year's result to an account in the balance sheet and close the income statement accounts.</span></span> <span data-ttu-id="b88c2-104">Dopo avere eseguito il processo batch Chiudi conto economico, è necessario aprire le registrazioni specificate nel processo batch, quindi analizzare e registrare i movimenti.</span><span class="sxs-lookup"><span data-stu-id="b88c2-104">After you run the Close Income Statement batch job, you must open the journal you specified in the batch job, and then review and post the entries.</span></span>

## <a name="to-post-the-year-end-closing-entry"></a><span data-ttu-id="b88c2-105">Per registrare il movimento di chiusura di fine anno</span><span class="sxs-lookup"><span data-stu-id="b88c2-105">To post the year end closing entry</span></span>
1. <span data-ttu-id="b88c2-106">Nell'angolo superiore destro, scegliere l'icona **Cerca pagina o report**, immettere **Registrazioni COGE**, quindi scegliere il collegamento correlato.</span><span class="sxs-lookup"><span data-stu-id="b88c2-106">In the top right corner, choose the **Search for Page or Report** icon, enter **General Journal**, and then choose the related link.</span></span>
2. <span data-ttu-id="b88c2-107">Nella finestra **Registrazione COGE**, nel campo **Nome batch**, selezionare il batch contenente i movimenti di chiusura.</span><span class="sxs-lookup"><span data-stu-id="b88c2-107">In the **General Journal** window, in the **Batch Name** field, select the batch that contains the closing entries.</span></span>
3. <span data-ttu-id="b88c2-108">Analizzare i movimenti.</span><span class="sxs-lookup"><span data-stu-id="b88c2-108">Review the entries.</span></span>
4. <span data-ttu-id="b88c2-109">Per contabilizzare le registrazioni, scegliere l'azione **Registra**.</span><span class="sxs-lookup"><span data-stu-id="b88c2-109">To post the journal, choose the **Post** action.</span></span>

<span data-ttu-id="b88c2-110">**Nota**: se viene rilevato un errore, viene visualizzato un messaggio di errore.</span><span class="sxs-lookup"><span data-stu-id="b88c2-110">**Note**: If an error is detected, an error message is displayed.</span></span> <span data-ttu-id="b88c2-111">Se la registrazione avviene correttamente, i movimenti registrati vengono rimossi dalle registrazioni.</span><span class="sxs-lookup"><span data-stu-id="b88c2-111">If the posting is successful, the posted entries are removed from the journal.</span></span> <span data-ttu-id="b88c2-112">Dopo il completamento della registrazione, in ogni conto economico viene registrato un movimento in modo che il relativo saldo sia uguale a zero, e il risultato dell'anno viene trasferito al conto patrimoniale.</span><span class="sxs-lookup"><span data-stu-id="b88c2-112">After posting is complete, an entry is posted to each income statement account so that its balance becomes zero and the year's result is transferred to the balance sheet.</span></span>

## <a name="see-also"></a><span data-ttu-id="b88c2-113">Vedi anche</span><span class="sxs-lookup"><span data-stu-id="b88c2-113">See Also</span></span>
[<span data-ttu-id="b88c2-114">Chiusura dei libri</span><span class="sxs-lookup"><span data-stu-id="b88c2-114">Close Books</span></span>](year-close-books.md)  
[<span data-ttu-id="b88c2-115">Chiusura del conto economico</span><span class="sxs-lookup"><span data-stu-id="b88c2-115">Close Income Statement</span></span>](year-close-income-statement.md)  
[<span data-ttu-id="b88c2-116">Procedura: Chiudere i periodi contabili</span><span class="sxs-lookup"><span data-stu-id="b88c2-116">How to: Close Accounting Periods</span></span>](year-close-account-periods.md)  
