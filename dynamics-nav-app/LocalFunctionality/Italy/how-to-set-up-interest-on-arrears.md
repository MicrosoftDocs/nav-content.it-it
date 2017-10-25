---
title: 'Procedura: Impostare gli interessi di mora'
description: "Per ciascuna condizione di addebito degli interessi, è possibile specificare come gli interessi di mora devono essere calcolati. È possibile impostare i calcoli di addebito degli interessi con diversi tassi di interesse per diversi periodi."
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
ms.openlocfilehash: d797a14ceab382f652e2a528ede01c8bbc13609c
ms.contentlocale: it-it
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-set-up-interest-on-arrears"></a><span data-ttu-id="1ab11-104">Procedura: Impostare gli interessi di mora</span><span class="sxs-lookup"><span data-stu-id="1ab11-104">How to: Set Up Interest on Arrears</span></span>
<span data-ttu-id="1ab11-105">Per ciascuna condizione di addebito degli interessi, è possibile specificare come gli interessi di mora devono essere calcolati.</span><span class="sxs-lookup"><span data-stu-id="1ab11-105">For each finance charge term, you can specify how interest on arrears must be calculated.</span></span> <span data-ttu-id="1ab11-106">È possibile impostare i calcoli di addebito degli interessi con diversi tassi di interesse per diversi periodi.</span><span class="sxs-lookup"><span data-stu-id="1ab11-106">You can set up finance charge calculations with different interest rates for different periods.</span></span>  

 <span data-ttu-id="1ab11-107">Quando si collega una condizione di addebito degli interessi con gli interessi di mora a un cliente o a un fornitore, gli interessi di mora vengono calcolati.</span><span class="sxs-lookup"><span data-stu-id="1ab11-107">When you apply a finance charge term with interest on arrears to a customer or vendor, interest on arrears will be calculated.</span></span> <span data-ttu-id="1ab11-108">Quindi, è possibile eseguire il report Calcolo interessi di mora per visualizzare i dettagli degli interessi di mora per clienti o fornitori.</span><span class="sxs-lookup"><span data-stu-id="1ab11-108">Then, you can run the Calculate Interest on Arrears report to view details about interest on arrears for customers or vendors.</span></span>  

 <span data-ttu-id="1ab11-109">Una volta eseguito il report, se un cliente deve gli interessi di mora, le informazioni sulla quantità degli interessi di mora da pagare vengono aggiunte al rendiconto cliente.</span><span class="sxs-lookup"><span data-stu-id="1ab11-109">After you run the report, if a customer owes interest on arrears, the information about the amount of interest on arrears to pay is added to the customer statement.</span></span>  

### <a name="to-set-up-interest-on-arrears"></a><span data-ttu-id="1ab11-110">Per impostare gli interessi di mora</span><span class="sxs-lookup"><span data-stu-id="1ab11-110">To set up interest on arrears</span></span>  

1.  <span data-ttu-id="1ab11-111">Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **Condiz. interessi finanziari**, quindi scegliere il collegamento correlato.</span><span class="sxs-lookup"><span data-stu-id="1ab11-111">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Finance Charge Terms**, and then choose the related link.</span></span>  

2.  <span data-ttu-id="1ab11-112">Nella finestra **Condiz. interessi finanziari**, selezionare il movimento richiesto della condizione di addebito degli interessi, quindi nella scheda **Azioni**, scegliere **Int. di mora**.</span><span class="sxs-lookup"><span data-stu-id="1ab11-112">In the **Finance Charge Terms** window, select the required finance charge term entry, and then, on the **Actions** tab, choose **Int. on Arrears**.</span></span>  

3.  <span data-ttu-id="1ab11-113">Nella finestra **Interessi di mora** nella scheda **Pagina iniziale** scegliere **Nuovo**.</span><span class="sxs-lookup"><span data-stu-id="1ab11-113">In the **Interest on Arrears** window, on the **Home** tab, choose **New**.</span></span>  

4.  <span data-ttu-id="1ab11-114">Compilare i campi come indicato nella tabella seguente.</span><span class="sxs-lookup"><span data-stu-id="1ab11-114">Fill in the fields as described in the following table.</span></span>  

    |<span data-ttu-id="1ab11-115">Campo</span><span class="sxs-lookup"><span data-stu-id="1ab11-115">Field</span></span>|<span data-ttu-id="1ab11-116">Description</span><span class="sxs-lookup"><span data-stu-id="1ab11-116">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="1ab11-117">**Data Inizio**</span><span class="sxs-lookup"><span data-stu-id="1ab11-117">**Starting Date**</span></span>|<span data-ttu-id="1ab11-118">Specificare la data a partire dalla quale si desidera calcolare gli interessi di mora.</span><span class="sxs-lookup"><span data-stu-id="1ab11-118">Specify the date from which you want to calculate interest on arrears.</span></span> <span data-ttu-id="1ab11-119">**Importante:** La data di inizio per la prima transazione degli interessi non può essere successiva alla data di registrazione più recente delle transazioni finanziarie.</span><span class="sxs-lookup"><span data-stu-id="1ab11-119">**Important:**  The start date for the first interest transaction cannot be later than the earliest posting date for the finance transactions.</span></span>|  
    |<span data-ttu-id="1ab11-120">**Tasso di interesse**</span><span class="sxs-lookup"><span data-stu-id="1ab11-120">**Interest Rate**</span></span>|<span data-ttu-id="1ab11-121">Specificare il tasso di interesse che deve essere calcolato per la mora.</span><span class="sxs-lookup"><span data-stu-id="1ab11-121">Specify the rate of interest to be calculated for the arrears.</span></span>|  
    |<span data-ttu-id="1ab11-122">**Description**</span><span class="sxs-lookup"><span data-stu-id="1ab11-122">**Description**</span></span>|<span data-ttu-id="1ab11-123">Specificare la descrizione per gli interessi di mora.</span><span class="sxs-lookup"><span data-stu-id="1ab11-123">Specify the description for the interest on arrears.</span></span>|  

5.  <span data-ttu-id="1ab11-124">Scegliere il pulsante **OK**.</span><span class="sxs-lookup"><span data-stu-id="1ab11-124">Choose the **OK** button.</span></span>  

 <span data-ttu-id="1ab11-125">Di seguito viene descritto come collegare gli interessi mora a un cliente, ma gli stessi passaggi si applicano anche per gli interessi di mora di un fornitore.</span><span class="sxs-lookup"><span data-stu-id="1ab11-125">The following procedure describes how to apply interest on arrears to a customer, but the same steps also apply for interest on arrears to a vendor.</span></span>  

### <a name="to-apply-interest-on-arrears-to-a-customer"></a><span data-ttu-id="1ab11-126">Per collegare gli interessi di mora a un cliente</span><span class="sxs-lookup"><span data-stu-id="1ab11-126">To apply interest on arrears to a customer</span></span>  

1.  <span data-ttu-id="1ab11-127">Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **Clienti**, quindi scegliere il collegamento correlato.</span><span class="sxs-lookup"><span data-stu-id="1ab11-127">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Customers**, and then choose the related link.</span></span>  

2.  <span data-ttu-id="1ab11-128">Selezionare il cliente a cui devono essere collegati gli interessi di mora e nella scheda **Pagina iniziale**, nel gruppo **Gestisci**, scegliere **Modifica**.</span><span class="sxs-lookup"><span data-stu-id="1ab11-128">Select the customer to whom interest on arrears must be applied, and then, on the **Home** tab, in the **Manage** group, choose **Edit**.</span></span>  

3.  <span data-ttu-id="1ab11-129">Nella Scheda dettaglio **Pagamenti**, nel campo **Codice int. di mora**, selezionare la condizione di addebito degli interessi appropriata che include gli interessi di mora.</span><span class="sxs-lookup"><span data-stu-id="1ab11-129">On the **Payments** FastTab, in the **Int. on Arrears Code** field, select the appropriate finance charge term that includes interest on arrears.</span></span>  

4.  <span data-ttu-id="1ab11-130">Scegliere il pulsante **OK**.</span><span class="sxs-lookup"><span data-stu-id="1ab11-130">Choose the **OK** button.</span></span>  

## <a name="see-also"></a><span data-ttu-id="1ab11-131">Vedi anche</span><span class="sxs-lookup"><span data-stu-id="1ab11-131">See Also</span></span>  
 [<span data-ttu-id="1ab11-132">Panoramica degli interessi di mora</span><span class="sxs-lookup"><span data-stu-id="1ab11-132">Interest on Arrears Overview</span></span>](interest-on-arrears-overview.md)   

