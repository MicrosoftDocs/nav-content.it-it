---
title: Procedura dettagliata - Calcolo del valore WIP per una commessa
description: Le commesse consentono di pianificare l'impiego delle risorse dell'azienda e di tenere traccia dei vari costi connessi all'impiego delle risorse in un progetto specifico. Le commesse implicano il consumo di ore di lavoro del personale, di ore macchina, degli articoli a magazzino e altri consumi che vanno monitorati man mano che la commessa progredisce.
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 09/06/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: ea0953192454302a83a9187cd6569905723fd150
ms.contentlocale: it-it
ms.lasthandoff: 10/16/2017

---
# <a name="walkthrough-calculating-work-in-process-for-a-job"></a><span data-ttu-id="513d9-104">Procedura dettagliata: Calcolo del valore WIP per una commessa</span><span class="sxs-lookup"><span data-stu-id="513d9-104">Walkthrough: Calculating Work in Process for a Job</span></span>
<span data-ttu-id="513d9-105">Le commesse consentono di pianificare l'impiego delle risorse dell'azienda e di tenere traccia dei vari costi connessi all'impiego delle risorse in un progetto specifico.</span><span class="sxs-lookup"><span data-stu-id="513d9-105">With jobs, you can schedule the usage of your company's resources and keep track of the various costs associated with the usage of resources on a specific project.</span></span> <span data-ttu-id="513d9-106">Le commesse implicano il consumo di ore di lavoro del personale, di ore macchina, degli articoli a magazzino e altri consumi che vanno monitorati man mano che la commessa progredisce.</span><span class="sxs-lookup"><span data-stu-id="513d9-106">Jobs involve the consumption of employee hours, machine hours, inventory items, and other types of usage that have to be tracked as a job progresses.</span></span> <span data-ttu-id="513d9-107">Se una commessa si protrae per lungo tempo, può essere opportuno trasferire questi costi a un conto WIP (Work in Process, ovvero semilavorati) nel conto patrimoniale fino al completamento della commessa.</span><span class="sxs-lookup"><span data-stu-id="513d9-107">If a job runs over a long period, you may want to transfer these costs to a Work in Process (WIP) account on the balance sheet while the job is being completed.</span></span> <span data-ttu-id="513d9-108">Sarà possibile riconoscere conti e vendite nel conto economico quando opportuno.</span><span class="sxs-lookup"><span data-stu-id="513d9-108">You can then recognize the costs and sales in your income statement accounts when it is appropriate.</span></span>  

## <a name="about-this-walkthrough"></a><span data-ttu-id="513d9-109">Informazioni sulla procedura dettagliata</span><span class="sxs-lookup"><span data-stu-id="513d9-109">About This Walkthrough</span></span>  
 <span data-ttu-id="513d9-110">In questa procedura dettagliata sono illustrati i task seguenti:</span><span class="sxs-lookup"><span data-stu-id="513d9-110">This walkthrough illustrates the following tasks:</span></span>  

-   <span data-ttu-id="513d9-111">Calcolo del WIP</span><span class="sxs-lookup"><span data-stu-id="513d9-111">Calculating WIP.</span></span>  
-   <span data-ttu-id="513d9-112">Selezione di un metodo di calcolo del WIP</span><span class="sxs-lookup"><span data-stu-id="513d9-112">Selecting a WIP calculation method.</span></span>  
-   <span data-ttu-id="513d9-113">Esclusione dal WIP di parte di una commessa.</span><span class="sxs-lookup"><span data-stu-id="513d9-113">Excluding part of a job from the WIP.</span></span>  
-   <span data-ttu-id="513d9-114">Registrazione del WIP nella contabilità generale.</span><span class="sxs-lookup"><span data-stu-id="513d9-114">Posting the WIP to the general ledger.</span></span>  
-   <span data-ttu-id="513d9-115">Storno di una registrazione WIP</span><span class="sxs-lookup"><span data-stu-id="513d9-115">Reversing a WIP posting.</span></span>  

 <span data-ttu-id="513d9-116">In ogni fase della procedura viene calcolato il valore del WIP e le transazioni della commessa sono trasferite alla contabilità generale.</span><span class="sxs-lookup"><span data-stu-id="513d9-116">Each step of the process calculates the value and moves the job transactions to the general ledger.</span></span> <span data-ttu-id="513d9-117">Le fasi di calcolo e registrazione sono state separate per consentire all'utente di rivedere i dati e apportarvi modifiche prima di procedere alla registrazione nella contabilità generale.</span><span class="sxs-lookup"><span data-stu-id="513d9-117">The calculation and posting steps are separated to help you review your data and to make modifications before posting to the general ledger.</span></span> <span data-ttu-id="513d9-118">Pertanto, dopo aver eseguito i processi batch di calcolo e prima di effettuare i processi batch di registrazione, è necessario controllare che tutti i dati siano corretti.</span><span class="sxs-lookup"><span data-stu-id="513d9-118">Therefore, you should make sure that all information is correct after you run the calculation batch jobs and before you run the posting batch jobs.</span></span>  

## <a name="roles"></a><span data-ttu-id="513d9-119">Ruoli</span><span class="sxs-lookup"><span data-stu-id="513d9-119">Roles</span></span>  
 <span data-ttu-id="513d9-120">Questa procedura dettagliata è svolta da un membro del team (Cinzia Di Marco).</span><span class="sxs-lookup"><span data-stu-id="513d9-120">This walkthrough uses the project team member (Tricia) as the persona.</span></span>  

## <a name="prerequisites"></a><span data-ttu-id="513d9-121">Prerequisiti</span><span class="sxs-lookup"><span data-stu-id="513d9-121">Prerequisites</span></span>  
 <span data-ttu-id="513d9-122">Prima di svolgere le attività di questa procedura dettagliata, è necessario installare [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="513d9-122">Before you can perform the tasks in the walkthrough, the [!INCLUDE[d365fin](includes/d365fin_md.md)] must be installed on your computer.</span></span>  

## <a name="story"></a><span data-ttu-id="513d9-123">Scenario</span><span class="sxs-lookup"><span data-stu-id="513d9-123">Story</span></span>  
 <span data-ttu-id="513d9-124">Questa procedura dettagliata è incentrata su CRONUS International Ltd., una società che si occupa di progettazione, consulenza e installazione di nuove infrastrutture, ad esempio aule conferenze e uffici, complete di mobilia e accessori.</span><span class="sxs-lookup"><span data-stu-id="513d9-124">This walkthrough focuses on CRONUS International Ltd., a design and consultancy firm that designs and fits new infrastructures, such as conference halls and offices, with furniture, accessories, and storage units.</span></span> <span data-ttu-id="513d9-125">La maggior parte di lavoro in CRONUS è svolto sulla base di un progetto e Cinzia, un membro del team di progetto, utilizza le commesse per avere una panoramica delle commesse in corso avviate da CRONUS e di quelle completate.</span><span class="sxs-lookup"><span data-stu-id="513d9-125">Most of the work at CRONUS is project-oriented and Tricia, a project team member, uses jobs to have an overview of each ongoing job that CRONUS has started and also the jobs that are completed.</span></span> <span data-ttu-id="513d9-126">Alcune commesse risultano estremamente lunghe e possono durare mesi.</span><span class="sxs-lookup"><span data-stu-id="513d9-126">Some of the jobs can be very lengthy and can run over months.</span></span> <span data-ttu-id="513d9-127">Cinzia può utilizzare un conto WIP per registrare i semilavorati e per tenere traccia dei costi in varie parti della commessa.</span><span class="sxs-lookup"><span data-stu-id="513d9-127">Tricia can use a WIP account to record the work in process and to track the costs throughout the job.</span></span>  

## <a name="calculating-wip"></a><span data-ttu-id="513d9-128">Calcolo del WIP</span><span class="sxs-lookup"><span data-stu-id="513d9-128">Calculating WIP</span></span>  
 <span data-ttu-id="513d9-129">CRONUS ha preso in carico un lungo progetto che si sta estendendo su più periodi contabili.</span><span class="sxs-lookup"><span data-stu-id="513d9-129">CRONUS has taken on a lengthy project that has now extended across reporting periods.</span></span> <span data-ttu-id="513d9-130">Cinzia, un membro del team di progetto, calcola il WIP per garantire l'accuratezza del rendiconto finanziario della società.</span><span class="sxs-lookup"><span data-stu-id="513d9-130">Tricia, a project team member, calculates the work in process (WIP) to make sure that the financial statement of the company will be accurate.</span></span>  

 <span data-ttu-id="513d9-131">Durante la procedura, Cinzia selezionerà uno specifico gruppo di task da includere nel calcolo del WIP.</span><span class="sxs-lookup"><span data-stu-id="513d9-131">During this procedure, Tricia will select a specific group of tasks that will be included in the WIP calculation.</span></span> <span data-ttu-id="513d9-132">Nella finestra **Righe task commessa** può specificare queste righe nella colonna **WIP-Totale**.</span><span class="sxs-lookup"><span data-stu-id="513d9-132">In the **Job Task Lines** window, she can specify these lines in the **WIP-Total** column.</span></span>  

 <span data-ttu-id="513d9-133">Nella seguente tabella vengono illustrate tre opzioni.</span><span class="sxs-lookup"><span data-stu-id="513d9-133">The following table describes the three options.</span></span>  

|<span data-ttu-id="513d9-134">Campo</span><span class="sxs-lookup"><span data-stu-id="513d9-134">Field</span></span>|<span data-ttu-id="513d9-135">Description</span><span class="sxs-lookup"><span data-stu-id="513d9-135">Description</span></span>|  
|-------------------------------------|---------------------------------------|  
|**<blank>**|<span data-ttu-id="513d9-136">Lasciare vuota se il task commessa fa parte di un gruppo di task.</span><span class="sxs-lookup"><span data-stu-id="513d9-136">Leave blank if the job task is a part of a group of tasks.</span></span>|  
|<span data-ttu-id="513d9-137">**Totale**</span><span class="sxs-lookup"><span data-stu-id="513d9-137">**Total**</span></span>|<span data-ttu-id="513d9-138">Definisce l'intervallo o il gruppo di task incluso nel calcolo di WIP e corrispettivo.</span><span class="sxs-lookup"><span data-stu-id="513d9-138">Defines the range or group of tasks that are included in the WIP and recognition calculation.</span></span> <span data-ttu-id="513d9-139">Qualsiasi task commessa all'interno del gruppo con **Tipo task commessa** impostato su **Registrazione** verrà incluso nel totale WIP, a meno che il relativo campo **WIP-Totale** sia impostato su **Escluso**.</span><span class="sxs-lookup"><span data-stu-id="513d9-139">Within the group, any job task with **Job Task Type** set to **Posting** will be included in the WIP Total, unless its **WIP-Total** field is set to **Excluded**.</span></span>|  
|<span data-ttu-id="513d9-140">**Escluso**</span><span class="sxs-lookup"><span data-stu-id="513d9-140">**Excluded**</span></span>|<span data-ttu-id="513d9-141">Si applica solo a un task con **Tipo task commessa** impostato su **Registrazione**.</span><span class="sxs-lookup"><span data-stu-id="513d9-141">Applies only to a task with **Job Task Type** of **Posting**.</span></span> <span data-ttu-id="513d9-142">Il task non viene incluso in caso di calcolo di WIP e corrispettivo.</span><span class="sxs-lookup"><span data-stu-id="513d9-142">The task is not included when WIP and recognition are calculated.</span></span>|  

 <span data-ttu-id="513d9-143">Nella seguente procedura dettagliata, Cinzia applica il metodo Valore costo, lo standard della società, per calcolare il WIP.</span><span class="sxs-lookup"><span data-stu-id="513d9-143">In the following walkthrough, Tricia applies the Cost Value method, her company standard, to calculate WIP.</span></span> <span data-ttu-id="513d9-144">Specifica quale parte della commessa sarà inclusa nel calcolo WIP assegnando dei valori WIP-Totale a varie righe task commessa.</span><span class="sxs-lookup"><span data-stu-id="513d9-144">She specifies what part of the job will be included in the WIP calculation by assigning WIP-Total values to various job task lines.</span></span>  

### <a name="to-calculate-wip"></a><span data-ttu-id="513d9-145">Per calcolare il WIP</span><span class="sxs-lookup"><span data-stu-id="513d9-145">To calculate WIP</span></span>  

1.  <span data-ttu-id="513d9-146">Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "Cerca pagina o report"), immettere **Commesse**, quindi scegliere il collegamento correlato.</span><span class="sxs-lookup"><span data-stu-id="513d9-146">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Jobs**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="513d9-147">Nell'elenco **Commesse** selezionare la commessa **Chernelli**, quindi scegliere l'azione **Modifica**.</span><span class="sxs-lookup"><span data-stu-id="513d9-147">In the **Jobs** list, select the **Deerfield** job, and then choose the **Edit** action.</span></span> <span data-ttu-id="513d9-148">Verrà visualizzata la scheda commessa in modalità di modifica.</span><span class="sxs-lookup"><span data-stu-id="513d9-148">This will open the job card in edit mode.</span></span>  

     <span data-ttu-id="513d9-149">Il WIP può essere calcolato sulla base di valore del costo, valore delle vendite, costo del venduto, percentuale di completamento o contratto completato.</span><span class="sxs-lookup"><span data-stu-id="513d9-149">WIP can be calculated based on Cost Value, Sales Value, Cost of Sales, Percentage of Completion, or Completed Contract.</span></span> <span data-ttu-id="513d9-150">Nell'esempio, CRONUS utilizza il metodo Valore costo.</span><span class="sxs-lookup"><span data-stu-id="513d9-150">In this example, CRONUS uses the Cost Value method.</span></span>  

3.  <span data-ttu-id="513d9-151">Selezionare il campo **Metodo WIP** della Scheda dettaglio **Registrazione**, quindi **Valore costo**.</span><span class="sxs-lookup"><span data-stu-id="513d9-151">On the **Posting** FastTab, choose the **WIP Method** field, and then select **Cost Value**.</span></span>  
4.  <span data-ttu-id="513d9-152">Scegliere l'azione **Righe task commessa** e impostare i valori elencati di seguito nel campo **WIP-Totale**.</span><span class="sxs-lookup"><span data-stu-id="513d9-152">Choose the **Job Task Lines** action and set the following values in the **WIP-Total** field.</span></span>  

     <span data-ttu-id="513d9-153">Nella seguente tabella vengono illustrati i valori.</span><span class="sxs-lookup"><span data-stu-id="513d9-153">The following table describes the values.</span></span>  

    |<span data-ttu-id="513d9-154">Nr. task commessa</span><span class="sxs-lookup"><span data-stu-id="513d9-154">Job Task No.</span></span>|<span data-ttu-id="513d9-155">Campo WIP-Totale</span><span class="sxs-lookup"><span data-stu-id="513d9-155">WIP-Total Field</span></span>|  
    |------------------|----------------------|  
    |<span data-ttu-id="513d9-156">1130</span><span class="sxs-lookup"><span data-stu-id="513d9-156">1130</span></span>|<span data-ttu-id="513d9-157">Escluso</span><span class="sxs-lookup"><span data-stu-id="513d9-157">Excluded</span></span>|  
    |<span data-ttu-id="513d9-158">1190</span><span class="sxs-lookup"><span data-stu-id="513d9-158">1190</span></span>|<span data-ttu-id="513d9-159">Totale</span><span class="sxs-lookup"><span data-stu-id="513d9-159">Total</span></span>|  
    |<span data-ttu-id="513d9-160">1210</span><span class="sxs-lookup"><span data-stu-id="513d9-160">1210</span></span>|<span data-ttu-id="513d9-161">Escluso</span><span class="sxs-lookup"><span data-stu-id="513d9-161">Excluded</span></span>|  
    |<span data-ttu-id="513d9-162">1310</span><span class="sxs-lookup"><span data-stu-id="513d9-162">1310</span></span>|<span data-ttu-id="513d9-163">Escluso</span><span class="sxs-lookup"><span data-stu-id="513d9-163">Excluded</span></span>|  

5.  <span data-ttu-id="513d9-164">Scegliere l'azione **WIP**, quindi scegliere l'azione **Calcola WIP**.</span><span class="sxs-lookup"><span data-stu-id="513d9-164">Choose the **WIP** action, and then choose the **Calculate WIP** action.</span></span>  
6.  <span data-ttu-id="513d9-165">Nella finestra **Commessa - Calcola WIP** è possibile selezionare la commessa per la quale calcolare il WIP.</span><span class="sxs-lookup"><span data-stu-id="513d9-165">In the **Job Calculate WIP** window, you can select a job that you want to calculate WIP.</span></span> <span data-ttu-id="513d9-166">Nella Scheda dettaglio **Commessa** selezionare **Chernelli** nel campo **Nr.**</span><span class="sxs-lookup"><span data-stu-id="513d9-166">On the **Job** FastTab, select **Deerfield** in the **No.**</span></span> <span data-ttu-id="513d9-167">.</span><span class="sxs-lookup"><span data-stu-id="513d9-167">field.</span></span>  
7.  <span data-ttu-id="513d9-168">Nel campo **Data di registrazione** immettere una data successiva alla data di lavoro.</span><span class="sxs-lookup"><span data-stu-id="513d9-168">In the **Posting Date** field, enter a date that is later than the work date.</span></span>
8.  <span data-ttu-id="513d9-169">Nel campo **Nr. documento** , immettere **1**.</span><span class="sxs-lookup"><span data-stu-id="513d9-169">In the **Document No.** field, enter **1**.</span></span> <span data-ttu-id="513d9-170">Viene quindi creato un documento a cui è possibile fare riferimento in seguito per la tracciabilità.</span><span class="sxs-lookup"><span data-stu-id="513d9-170">This creates a document that you can refer to later for traceability.</span></span>  
9. <span data-ttu-id="513d9-171">Scegliere **OK** per eseguire il processo batch.</span><span class="sxs-lookup"><span data-stu-id="513d9-171">Choose the **OK** button to run the batch job.</span></span> <span data-ttu-id="513d9-172">Viene visualizzato un messaggio.</span><span class="sxs-lookup"><span data-stu-id="513d9-172">A message is displayed.</span></span> <span data-ttu-id="513d9-173">Fare clic sul pulsante **OK** per continuare.</span><span class="sxs-lookup"><span data-stu-id="513d9-173">Choose the **OK** button to continue.</span></span> <span data-ttu-id="513d9-174">Chiudere la finestra **Righe task commessa**.</span><span class="sxs-lookup"><span data-stu-id="513d9-174">Close the **Job Task Lines** window.</span></span>  

    > [!NOTE]  
    >  <span data-ttu-id="513d9-175">Il messaggio indica che sono presenti avvisi associati al calcolo WIP.</span><span class="sxs-lookup"><span data-stu-id="513d9-175">The message states that there are warnings associated with the WIP calculation.</span></span> <span data-ttu-id="513d9-176">Gli avvisi verranno esaminati nella procedura successiva.</span><span class="sxs-lookup"><span data-stu-id="513d9-176">You will review the warnings in the next procedure.</span></span>  

10. <span data-ttu-id="513d9-177">Nella scheda **Commessa**, espandere la Scheda dettaglio **WIP e corrispettivo** per vedere i valori calcolati.</span><span class="sxs-lookup"><span data-stu-id="513d9-177">On the **Job** card, expand the **WIP and Recognition** FastTab to see the calculated values.</span></span> <span data-ttu-id="513d9-178">È inoltre possibile visualizzare la **Data di registrazione WIP** e i valori che sono stati registrati nella contabilità generale, se disponibile.</span><span class="sxs-lookup"><span data-stu-id="513d9-178">You can also see the **WIP Posting Date** and the values that have been posted to the general ledger, if any.</span></span>  

 <span data-ttu-id="513d9-179">Si noti che il valore **Importo costi ricon.** è 215,60 nella colonna **Da registrare**.</span><span class="sxs-lookup"><span data-stu-id="513d9-179">Notice that the value for **Recog. Costs Amount** is 215.60 in the **To Post** column.</span></span> <span data-ttu-id="513d9-180">Ciò riflette i costi totali di due degli articoli nel gruppo di task 1110 a 1130 della commessa.</span><span class="sxs-lookup"><span data-stu-id="513d9-180">This reflects the total costs of two of the items in the group of job tasks 1110 – 1130.</span></span> <span data-ttu-id="513d9-181">Il terzo articolo è stato impostato su **Escluso** e quindi non è incluso nel calcolo del WIP.</span><span class="sxs-lookup"><span data-stu-id="513d9-181">The third item was set to **Excluded**, and therefore is not included in the WIP calculation.</span></span>  

### <a name="to-review-wip-warnings"></a><span data-ttu-id="513d9-182">Per esaminare gli avvisi WIP</span><span class="sxs-lookup"><span data-stu-id="513d9-182">To review WIP warnings</span></span>  

1.  <span data-ttu-id="513d9-183">Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **Pannello di controllo WIP commessa**, quindi scegliere il collegamento correlato.</span><span class="sxs-lookup"><span data-stu-id="513d9-183">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Job WIP Cockpit**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="513d9-184">Selezionare la commessa **Chernelli**, quindi scegliere l'azione **Mostra avvisi**.</span><span class="sxs-lookup"><span data-stu-id="513d9-184">Select the **Deerfield** job, and then choose the **Show Warnings** action.</span></span>  
3.  <span data-ttu-id="513d9-185">Nella finestra **Avvisi WIP commessa** analizzare l'avviso associato alla commessa.</span><span class="sxs-lookup"><span data-stu-id="513d9-185">In the **Job WIP Warnings** window, review the warning associated with the job.</span></span>  

 <span data-ttu-id="513d9-186">Dopo il periodo contabile, Cinzia deve ricalcolare il WIP per includervi il lavoro completato finora.</span><span class="sxs-lookup"><span data-stu-id="513d9-186">After the accounting period ends, Tricia has to recalculate the WIP to include completed work to this point.</span></span>  

### <a name="to-recalculate-wip"></a><span data-ttu-id="513d9-187">Per ricalcolare il WIP</span><span class="sxs-lookup"><span data-stu-id="513d9-187">To recalculate WIP</span></span>  

1.  <span data-ttu-id="513d9-188">Nella scheda **Commessa**, scegliere l'azione **Movimenti WIP** per visualizzare il calcolo del WIP.</span><span class="sxs-lookup"><span data-stu-id="513d9-188">On the **Job** card, choose the **WIP Entries** action to view the WIP calculation.</span></span>  

     <span data-ttu-id="513d9-189">La finestra **Movimenti WIP commessa** riporta gli ultimi movimenti WIP calcolati per una commessa, anche se il WIP non è ancora stato registrato nella contabilità generale.</span><span class="sxs-lookup"><span data-stu-id="513d9-189">The **Job WIP Entries** window shows the WIP entries that were last calculated on a job, even if WIP has not yet been posted to the general ledger.</span></span>  

2.  <span data-ttu-id="513d9-190">È possibile utilizzare i passaggi nella procedura relativa a come calcolare il WIP per ricalcolare il WIP.</span><span class="sxs-lookup"><span data-stu-id="513d9-190">You can follow the steps in the procedure that explains how to calculate WIP to recalculate WIP.</span></span> <span data-ttu-id="513d9-191">Ogni volta che si ricalcola il WIP, viene creato un movimento nella finestra **Movimenti WIP commessa**.</span><span class="sxs-lookup"><span data-stu-id="513d9-191">Every time WIP is calculated, an entry is created in the **Job WIP Entries** window.</span></span>  
3.  <span data-ttu-id="513d9-192">Chiudere la finestra.</span><span class="sxs-lookup"><span data-stu-id="513d9-192">Close the window.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="513d9-193">Il WIP e il corrispettivo vengono solo calcolati.</span><span class="sxs-lookup"><span data-stu-id="513d9-193">Work in Process and Recognition is only calculated.</span></span> <span data-ttu-id="513d9-194">ma non registrato nella contabilità generale.</span><span class="sxs-lookup"><span data-stu-id="513d9-194">It is not posted to the general ledger.</span></span> <span data-ttu-id="513d9-195">A tale scopo, è necessario eseguire il processo batch **Registra WIP in C/G** dopo aver calcolato il WIP e il corrispettivo.</span><span class="sxs-lookup"><span data-stu-id="513d9-195">To do so, you must run **Post WIP to G/L** batch job after you have calculated the WIP and Recognition.</span></span>

## <a name="posting-wip-to-general-ledger"></a><span data-ttu-id="513d9-196">Registrazione del WIP nella contabilità generale</span><span class="sxs-lookup"><span data-stu-id="513d9-196">Posting WIP to General Ledger</span></span>  
 <span data-ttu-id="513d9-197">Ora che il WIP per la commessa è stato calcolato, è possibile registrarlo nella contabilità generale.</span><span class="sxs-lookup"><span data-stu-id="513d9-197">Now that Tricia has calculated WIP for this job, she can post it to the general ledger.</span></span>  

### <a name="to-post-wip-to-general-ledger"></a><span data-ttu-id="513d9-198">Per registrare il WIP nella contabilità generale</span><span class="sxs-lookup"><span data-stu-id="513d9-198">To post WIP to general ledger</span></span>  

1.  <span data-ttu-id="513d9-199">Nell'elenco **Commesse** selezionare la commessa **Chernelli**.</span><span class="sxs-lookup"><span data-stu-id="513d9-199">From the **Jobs** list, select the **Deerfield** job.</span></span>  
2.  <span data-ttu-id="513d9-200">Scegliere l'azione **WIP**, quindi scegliere l'azione **Registra WIP in C/G**.</span><span class="sxs-lookup"><span data-stu-id="513d9-200">Choose the **WIP** action, and then choose the **Post WIP to G/L** action.</span></span>  
3.  <span data-ttu-id="513d9-201">Nella finestra **Commessa - Registra WIP in C/G**, nella Scheda dettaglio **Commessa** selezionare **Chernelli** nel campo **Nr.**.</span><span class="sxs-lookup"><span data-stu-id="513d9-201">In the **Job Post WIP to G/L** window, on the **Job** FastTab, select **Deerfield** in the **No.**</span></span> <span data-ttu-id="513d9-202"> </span><span class="sxs-lookup"><span data-stu-id="513d9-202">field.</span></span>  
4.  <span data-ttu-id="513d9-203">Inserire **1** nel campo **Nr. documento storno** della Scheda dettaglio **Opzioni**.</span><span class="sxs-lookup"><span data-stu-id="513d9-203">On the **Options** FastTab, in the **Reversal Document No.** field, enter **1**.</span></span>  
5.  <span data-ttu-id="513d9-204">Scegliere **OK** per registrare il WIP nella contabilità generale.</span><span class="sxs-lookup"><span data-stu-id="513d9-204">Choose the **OK** button to post WIP to the general ledger.</span></span>  
6.  <span data-ttu-id="513d9-205">Fare clic sul pulsante **OK** per chiudere la finestra di conferma.</span><span class="sxs-lookup"><span data-stu-id="513d9-205">Choose the **OK** button to close the confirmation window.</span></span>  

     <span data-ttu-id="513d9-206">Dopo avere completato la registrazione, è possibile visualizzare le informazioni di registrazione nella finestra **Movimenti C/G WIP** .</span><span class="sxs-lookup"><span data-stu-id="513d9-206">After you have completed the posting, you can view the posting information in the **WIP G/L Entries** window.</span></span>  

7.  <span data-ttu-id="513d9-207">Nell'elenco **Commesse** selezionare la commessa **Chernelli**, quindi scegliere l'azione **Movimenti C/G WIP**.</span><span class="sxs-lookup"><span data-stu-id="513d9-207">In the **Jobs** list, select the **Deerfield** job, and then choose the **WIP G/L Entries** action.</span></span>  

     <span data-ttu-id="513d9-208">Nella finestra **Movimenti C/G WIP commessa** verificare che il WIP sia stato registrato nella contabilità generale.</span><span class="sxs-lookup"><span data-stu-id="513d9-208">In the **Job WIP G/L Entries** window, verify that the WIP has been posted to the general ledger.</span></span>  

8.  <span data-ttu-id="513d9-209">Chiudere la finestra.</span><span class="sxs-lookup"><span data-stu-id="513d9-209">Close the window.</span></span>  
9. <span data-ttu-id="513d9-210">Aprire la scheda **Commessa** per la commessa **Chernelli**.</span><span class="sxs-lookup"><span data-stu-id="513d9-210">Open the **Job** card for the **Deerfield** job.</span></span>  
10. <span data-ttu-id="513d9-211">Nella Scheda dettaglio **WIP e corrispettivo**, si noti che nella colonna **Registrato** il campo **Importo C/G costi ricon.** ora è compilato, il che indica che il WIP è stato correttamente registrato nella contabilità generale.</span><span class="sxs-lookup"><span data-stu-id="513d9-211">On the **WIP and Recognition** FastTab, notice that in the **Posted** column, the **Recog. Costs G/L Amount** field is now filled in, which indicates that WIP was posted to the general ledger successfully.</span></span>  
11. <span data-ttu-id="513d9-212">Scegliere il pulsante **OK** per chiudere la scheda.</span><span class="sxs-lookup"><span data-stu-id="513d9-212">Choose the **OK** button to close the card.</span></span>  

## <a name="reversing-a-wip-posting"></a><span data-ttu-id="513d9-213">Storno di una registrazione WIP</span><span class="sxs-lookup"><span data-stu-id="513d9-213">Reversing a WIP Posting</span></span>  
 <span data-ttu-id="513d9-214">Cinzia si accorge che i task commessa esclusi dal calcolo del WIP avrebbero dovuto essere calcolati nel WIP.</span><span class="sxs-lookup"><span data-stu-id="513d9-214">Tricia determines that the job tasks that were excluded from the calculation of WIP should have been calculated in WIP.</span></span> <span data-ttu-id="513d9-215">Il programma consente di stornare le registrazioni errate senza dover contabilizzare nuove registrazioni WIP.</span><span class="sxs-lookup"><span data-stu-id="513d9-215">She can reverse the incorrect postings without having to post new WIP postings.</span></span>  

### <a name="to-reverse-a-wip-posting"></a><span data-ttu-id="513d9-216">Per stornare una registrazione WIP</span><span class="sxs-lookup"><span data-stu-id="513d9-216">To reverse a WIP posting</span></span>  

1.  <span data-ttu-id="513d9-217">Nell'elenco **Commesse** selezionare la commessa **Chernelli**.</span><span class="sxs-lookup"><span data-stu-id="513d9-217">From the **Jobs** list, select the **Deerfield** job.</span></span>  
2.  <span data-ttu-id="513d9-218">Scegliere l'azione **WIP**, quindi scegliere l'azione **Registra WIP in C/G**.</span><span class="sxs-lookup"><span data-stu-id="513d9-218">Choose the **WIP** action, and then choose the **Post WIP to G/L** action.</span></span>  
3.  <span data-ttu-id="513d9-219">Nella Scheda dettaglio **Commessa** della finestra **Commessa - Registra WIP in C/G** selezionare **Chernelli** nel campo **Nr.**.</span><span class="sxs-lookup"><span data-stu-id="513d9-219">In the **Job Post to WIP to G/L** window, on the **Job** FastTab, select **Deerfield** in the **No.**</span></span> <span data-ttu-id="513d9-220"> </span><span class="sxs-lookup"><span data-stu-id="513d9-220">field.</span></span>  
4.  <span data-ttu-id="513d9-221">Inserire **1** nel campo **Nr. documento storno** della Scheda dettaglio **Opzioni**.</span><span class="sxs-lookup"><span data-stu-id="513d9-221">On the **Options** FastTab, in the **Reversal Document No.** field, enter **1**.</span></span>  
5.  <span data-ttu-id="513d9-222">Nel campo **Data registrazione storno**, inserire la data di registrazione originale.</span><span class="sxs-lookup"><span data-stu-id="513d9-222">In the **Reversal Posting Date** field, enter the original posting date.</span></span> <span data-ttu-id="513d9-223">I dati dovrebbero essere gli stessi utilizzati per calcolare il WIP la prima volta.</span><span class="sxs-lookup"><span data-stu-id="513d9-223">It should be the same date that you used to calculate WIP the first time.</span></span>  
6.  <span data-ttu-id="513d9-224">Selezionare la casella di controllo **Storna solo**.</span><span class="sxs-lookup"><span data-stu-id="513d9-224">Select the **Reverse Only** check box.</span></span> <span data-ttu-id="513d9-225">In questo modo il WIP precedentemente registrato viene stornato senza una nuova registrazione nella contabilità generale.</span><span class="sxs-lookup"><span data-stu-id="513d9-225">This will reverse previously posted WIP, but does post new WIP to the general ledger.</span></span>  
7.  <span data-ttu-id="513d9-226">Selezionare il pulsante **OK** per eseguire il processo batch e fare clic sul pulsante **OK** per chiudere la finestra di conferma.</span><span class="sxs-lookup"><span data-stu-id="513d9-226">Choose the **OK** button to run the batch job, and choose the **OK** button to close the confirmation window.</span></span>  
8.  <span data-ttu-id="513d9-227">Aprire la scheda **Commessa** per **Chernelli**.</span><span class="sxs-lookup"><span data-stu-id="513d9-227">Open the **Job** card for **Deerfield**.</span></span>  
9. <span data-ttu-id="513d9-228">Nella Scheda dettaglio **WIP e corrispettivo** verificare che non vi siano movimenti WIP registrati.</span><span class="sxs-lookup"><span data-stu-id="513d9-228">On the **WIP and Recognition** FastTab, verify that there are no posted WIP entries.</span></span>  
10. <span data-ttu-id="513d9-229">Chiudere questa finestra.</span><span class="sxs-lookup"><span data-stu-id="513d9-229">Close this window.</span></span>  
11. <span data-ttu-id="513d9-230">Nell'elenco **Commesse** selezionare la commessa **Chernelli**, scegliere l'azione **WIP**, quindi scegliere l'azione **Movimenti C/G WIP**.</span><span class="sxs-lookup"><span data-stu-id="513d9-230">In the **Jobs** list, select the **Deerfield** job, choose the **WIP** action, and then choose the **WIP G/L Entries** action.</span></span> <span data-ttu-id="513d9-231">I movimenti WIP hanno la casella di controllo **Stornato** selezionata.</span><span class="sxs-lookup"><span data-stu-id="513d9-231">The WIP entries have the **Reversed** check box selected.</span></span>  
12. <span data-ttu-id="513d9-232">Chiudere questa finestra.</span><span class="sxs-lookup"><span data-stu-id="513d9-232">Close this window.</span></span>  
13. <span data-ttu-id="513d9-233">Aprire **Righe task commessa** per la commessa, includere nel calcolo del WIP le parti della commessa necessarie, ricalcolare il WIP e registrare il nuovo valore nella contabilità generale.</span><span class="sxs-lookup"><span data-stu-id="513d9-233">Open **Job Task Lines** for the job, include the parts of the job that should be in the WIP calculation, and then recalculate and post the new value to the general ledger.</span></span>  

    > [!NOTE]  
    >  <span data-ttu-id="513d9-234">Si supponga che Cinzia abbia calcolato e registrato il WIP per una commessa con date errate.</span><span class="sxs-lookup"><span data-stu-id="513d9-234">Suppose Tricia calculated and posted WIP for a job with incorrect dates.</span></span> <span data-ttu-id="513d9-235">Seguendo il metodo che è stato discusso in precedenza, il programma consente di stornare le registrazioni errate, correggerne le date e registrarle nuovamente nella contabilità generale.</span><span class="sxs-lookup"><span data-stu-id="513d9-235">Following the method that was discussed earlier, she can reverse the incorrect postings, correct the dates, and repost to the general ledger.</span></span>  

## <a name="next-steps"></a><span data-ttu-id="513d9-236">Passaggi successivi</span><span class="sxs-lookup"><span data-stu-id="513d9-236">Next Steps</span></span>  
 <span data-ttu-id="513d9-237">In questa procedura dettagliata sono stati svolti i passaggi del calcolo del WIP in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="513d9-237">This walkthrough has taken you through the steps of calculating WIP in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span> <span data-ttu-id="513d9-238">In commesse più grandi, può essere utile trasferire periodicamente i costi a un conto WIP fino al completamento della commessa.</span><span class="sxs-lookup"><span data-stu-id="513d9-238">In larger jobs, it may be useful to transfer the costs to a WIP account periodically while the job is being completed.</span></span> <span data-ttu-id="513d9-239">In questa procedura dettagliata è stato illustrato come escludere le righe di task dal calcolo.</span><span class="sxs-lookup"><span data-stu-id="513d9-239">This walkthrough has shown you how to exclude task lines from a calculation.</span></span> <span data-ttu-id="513d9-240">È stato inoltre illustrato quando è necessario ricalcolare.</span><span class="sxs-lookup"><span data-stu-id="513d9-240">It also shows you when you would have to recalculate.</span></span> <span data-ttu-id="513d9-241">Infine, è stato descritto come registrare il WIP nella contabilità generale.</span><span class="sxs-lookup"><span data-stu-id="513d9-241">And finally, this walkthrough demonstrates how to post the WIP to the general ledger.</span></span> <span data-ttu-id="513d9-242">Inoltre è incluso un esempio di come stornare una registrazione WIP nella contabilità generale.</span><span class="sxs-lookup"><span data-stu-id="513d9-242">An example of how to reverse a WIP posting to the general ledger is also included.</span></span>  

## <a name="see-also"></a><span data-ttu-id="513d9-243">Vedi anche</span><span class="sxs-lookup"><span data-stu-id="513d9-243">See Also</span></span>  
 [<span data-ttu-id="513d9-244">Procedure dettagliate per i processi aziendali</span><span class="sxs-lookup"><span data-stu-id="513d9-244">Business Process Walkthroughs</span></span>](walkthrough-business-process-walkthroughs.md)  
 <span data-ttu-id="513d9-245">[Procedura dettagliata: Gestione dei progetti con le commesse](walkthrough-managing-projects-with-jobs.md) </span><span class="sxs-lookup"><span data-stu-id="513d9-245">[Walkthrough: Managing Projects with Jobs](walkthrough-managing-projects-with-jobs.md) </span></span>  
 <span data-ttu-id="513d9-246">[Metodi WIP](projects-understanding-wip.md) </span><span class="sxs-lookup"><span data-stu-id="513d9-246">[Understanding WIP Methods](projects-understanding-wip.md) </span></span>  
 [<span data-ttu-id="513d9-247">Monitoraggio di progressi e performance</span><span class="sxs-lookup"><span data-stu-id="513d9-247">Monitor Progress and Performance</span></span>](projects-how-monitor-progress-performance.md)  
 <span data-ttu-id="513d9-248">[Utilizzo di [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="513d9-248">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
