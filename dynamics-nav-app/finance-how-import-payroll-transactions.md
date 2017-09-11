---
title: 'Procedura: Importare transazioni retributive '
author: SorenGP
ms.custom: na
ms.date: 09/29/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: d5e70a0a1659c7facdeec3f0971eda43ff8a03cc
ms.contentlocale: it-it
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-import-payroll-transactions"></a><span data-ttu-id="4412b-102">Procedura: Importare transazioni retributive </span><span class="sxs-lookup"><span data-stu-id="4412b-102">How to: Import Payroll Transactions</span></span>
<span data-ttu-id="4412b-103">Per indicare i pagamenti di stipendio e le transazioni correlate, è necessario importare e registrare in contabilità generale le transazioni finanziarie trasformate dal provider di retribuzioni.</span><span class="sxs-lookup"><span data-stu-id="4412b-103">To account for salary payments and related transactions, you must import and post financial transactions made by your payroll provider to the general ledger.</span></span> <span data-ttu-id="4412b-104">A tale scopo, è necessario innanzitutto importare un file csv</span><span class="sxs-lookup"><span data-stu-id="4412b-104">To do this, you first import a csv.</span></span> <span data-ttu-id="4412b-105">che si riceve dal provider di retribuzioni nella finestra **Contabilità generale**.</span><span class="sxs-lookup"><span data-stu-id="4412b-105">file that you receive from the payroll provider into the **General Journal** window.</span></span> <span data-ttu-id="4412b-106">Successivamente si esegue il mapping tra i conti esterni nel file retribuzioni e i conti C/G pertinenti.</span><span class="sxs-lookup"><span data-stu-id="4412b-106">Then you map the external accounts in the payroll file to the relevant G/L accounts.</span></span> <span data-ttu-id="4412b-107">Infine, si registrano le transazioni retribuzioni in base alla mappatura dei conti.</span><span class="sxs-lookup"><span data-stu-id="4412b-107">Lastly, you post the payroll transactions according to the account mapping.</span></span>

## <a name="to-import-a-payroll-file"></a><span data-ttu-id="4412b-108">Per importare un file delle retribuzioni</span><span class="sxs-lookup"><span data-stu-id="4412b-108">To import a payroll file</span></span>
1. <span data-ttu-id="4412b-109">Nell'angolo superiore destro, scegliere l'icona **Cerca pagina o report**, immettere **Registrazioni COGE**, quindi scegliere il collegamento correlato.</span><span class="sxs-lookup"><span data-stu-id="4412b-109">In the top right corner, choose the **Search for Page or Report** icon, enter **General Journals**, and then choose the related link.</span></span>
2. <span data-ttu-id="4412b-110">Nel batch registrazioni COGE appropriato scegliere l'azione **Importa transazioni retribuzioni**.</span><span class="sxs-lookup"><span data-stu-id="4412b-110">In the relevant general journal batch, choose the **Import Payroll Transactions** action.</span></span>
3. <span data-ttu-id="4412b-111">Nella finestra **Importa** selezionare il file retribuzioni interessato, quindi scegliere **OK**.</span><span class="sxs-lookup"><span data-stu-id="4412b-111">In the **Import** window, select the relevant payroll file, and then choose the **OK** button.</span></span> <span data-ttu-id="4412b-112">Il file deve essere in formato CSV.</span><span class="sxs-lookup"><span data-stu-id="4412b-112">The file must be in CSV format.</span></span> 
4. <span data-ttu-id="4412b-113">Seguire i passaggi indicati nella finestra **Importa transazioni retribuzioni** per importare le transazioni e mappare i conti, quindi scegliere il pulsante **Fine**.</span><span class="sxs-lookup"><span data-stu-id="4412b-113">Follow the steps in the **Import Payroll Transactions** window to import transactions and map accounts, and then choose the **Finish** button.</span></span>

    <span data-ttu-id="4412b-114">Le registrazioni COGE vengono completate con le righe che rappresentano le transazioni contenute nel file retribuzioni e con i relativi conti nella colonna **Conto C/G**.</span><span class="sxs-lookup"><span data-stu-id="4412b-114">The general journal is filled with lines representing the transactions that the payroll file contains and with the relevant accounts in the **G/L Account** column.</span></span>
4. <span data-ttu-id="4412b-115">Modificare o registrare le righe delle registrazioni relative a tutte le altre le transazioni della contabilità generale.</span><span class="sxs-lookup"><span data-stu-id="4412b-115">Edit or post the journal lines as for any other general ledger transactions.</span></span> <span data-ttu-id="4412b-116">Per ulteriori informazioni, vedere [Procedura: Elaborazione delle registrazioni COGE](ui-work-general-journals.md).</span><span class="sxs-lookup"><span data-stu-id="4412b-116">For more information, see [How to: Work With General Journals](ui-work-general-journals.md).</span></span>   

## <a name="see-also"></a><span data-ttu-id="4412b-117">Vedi anche</span><span class="sxs-lookup"><span data-stu-id="4412b-117">See Also</span></span>
[<span data-ttu-id="4412b-118">Contabilità</span><span class="sxs-lookup"><span data-stu-id="4412b-118">Finance</span></span>](finance-setup.md)  
[<span data-ttu-id="4412b-119">Procedura: Utilizzare le registrazioni di contabilità generale</span><span class="sxs-lookup"><span data-stu-id="4412b-119">How to: Work With General Journals</span></span>](ui-work-general-journals.md)  

