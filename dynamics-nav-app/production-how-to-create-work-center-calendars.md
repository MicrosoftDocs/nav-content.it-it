---
title: Come impostare i calendari del reparto produzione
description: "In un calendario delle aree di produzione sono specificati i giorni e gli orari lavorativi, i turni, le ferie e le assenze che determinano la capacità lorda disponibile dell'area di produzione, misurata in tempo, sulla base dei valori definiti per l'efficienza e la capacità di tale area. Per la creazione e l'attivazione di un calendario delle aree di produzione sono necessarie diverse attività preliminari."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 09/14/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 59131cdded4bf854aed02a7d835e8160342adb36
ms.contentlocale: it-it
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-set-up-shop-calendars"></a><span data-ttu-id="616e1-104">Procedura: Impostare i calendari del reparto produzione</span><span class="sxs-lookup"><span data-stu-id="616e1-104">How to: Set Up Shop Calendars</span></span>
<span data-ttu-id="616e1-105">In un calendario delle aree di produzione o dei centri di lavoro sono specificati i giorni e gli orari lavorativi, i turni, le ferie e le assenze che determinano la capacità lorda disponibile dell'area o del centro, misurata in tempo, sulla base dei valori definiti per l'efficienza e la capacità di tale area o centro.</span><span class="sxs-lookup"><span data-stu-id="616e1-105">A work center or machine calendar specifies the working days and hours, shifts, holidays, and absences that determine the center’s gross available capacity, measured in time, according to its defined efficiency and capacity values.</span></span>

<span data-ttu-id="616e1-106">Come base per il calcolo di un calendario specifico delle aree di produzione o dei centri di lavoro è prima di tutto necessario configurare uno o più calendari del reparto produzione generali.</span><span class="sxs-lookup"><span data-stu-id="616e1-106">As a foundation for calculating a specific work or machine center calendar, you must first set up one or more general shop calendars.</span></span> <span data-ttu-id="616e1-107">In un calendario del reparto produzione viene definita una settimana lavorativa standard in termini di ora di inizio e di fine di ogni giorno lavorativo e di relazione di turni lavorativi.</span><span class="sxs-lookup"><span data-stu-id="616e1-107">A shop calendar defines a standard work week according to start and end times of each working day and the work shift relation.</span></span> <span data-ttu-id="616e1-108">In tale calendario sono inoltre disponibili le ferie fisse nel corso di un anno.</span><span class="sxs-lookup"><span data-stu-id="616e1-108">In addition, the shop calendar defines the fixed holidays during a year.</span></span>  

<span data-ttu-id="616e1-109">Di seguito viene descritto come impostare i calendari delle aree di produzione.</span><span class="sxs-lookup"><span data-stu-id="616e1-109">The following describes how to set up work center calendars.</span></span> <span data-ttu-id="616e1-110">I passaggi sono gli stessi della procedura per l'impostazione dei calendari dei centri di lavoro.</span><span class="sxs-lookup"><span data-stu-id="616e1-110">The steps are similar when setting up machine center calendars.</span></span>  

## <a name="to-create-work-shifts"></a><span data-ttu-id="616e1-111">Per creare turni lavorativi</span><span class="sxs-lookup"><span data-stu-id="616e1-111">To create work shifts</span></span>  
1.  <span data-ttu-id="616e1-112">Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **Turni lavorativi** e quindi scegliere il collegamento correlato.</span><span class="sxs-lookup"><span data-stu-id="616e1-112">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Work Shifts**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="616e1-113">In una riga vuota immettere un numero nel campo **Codice** per identificare il turno lavorativo, ad esempio **1**.</span><span class="sxs-lookup"><span data-stu-id="616e1-113">On a blank line, enter a number in the **Code** field to identify the work shift, for example, **1**.</span></span>  
3.  <span data-ttu-id="616e1-114">Descrivere il turno lavorativo nel campo **Descrizione**, ad esempio **1mo Turno**.</span><span class="sxs-lookup"><span data-stu-id="616e1-114">Describe the work shift in the **Description** field, for example, **1st shift**.</span></span>  
4.  <span data-ttu-id="616e1-115">Facoltativamente, compilare le righe relative a un secondo o terzo turno lavorativo.</span><span class="sxs-lookup"><span data-stu-id="616e1-115">Optionally, fill in lines for a second or third work shift.</span></span>  

<span data-ttu-id="616e1-116">Anche se nelle aree di produzione specificate non vengono effettuati turni diversi, immettere almeno un codice di turno lavorativo.</span><span class="sxs-lookup"><span data-stu-id="616e1-116">Even if your work centers do not work in different work shifts, enter at least one work shift code.</span></span>  

## <a name="to-set-up-a-shop-calendar"></a><span data-ttu-id="616e1-117">Per impostare un calendario reparto prod.</span><span class="sxs-lookup"><span data-stu-id="616e1-117">To set up a shop calendar</span></span>  
1.  <span data-ttu-id="616e1-118">Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **Calendari reparto prod.** e quindi scegliere il collegamento correlato.</span><span class="sxs-lookup"><span data-stu-id="616e1-118">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Shop Calendars**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="616e1-119">In una riga vuota immettere un numero nel campo **Codice** per identificare il calendario reparto prod.</span><span class="sxs-lookup"><span data-stu-id="616e1-119">On a blank line, enter a number in the **Code** field to identify the shop calendar.</span></span>  
3.  <span data-ttu-id="616e1-120">Nel campo **Descrizione** immettere una descrizione del calendario.</span><span class="sxs-lookup"><span data-stu-id="616e1-120">Describe the shop calendar in the **Description** field.</span></span>  
4.  <span data-ttu-id="616e1-121">Scegliere l'azione **Giorni lavorativi**.</span><span class="sxs-lookup"><span data-stu-id="616e1-121">Choose the **Working Days** action.</span></span>
5.  <span data-ttu-id="616e1-122">Nella finestra **Giorni lavorativi rep. prod.**, specificare una settimana lavorativa completa, con l'ora di inizio e di fine per ogni giorno.</span><span class="sxs-lookup"><span data-stu-id="616e1-122">In the **Shop Calendar Working Days** window, define a complete work week, with the start and end times for each day.</span></span>  

    <span data-ttu-id="616e1-123">Nel campo **Cod. turno lavorativo** , selezionare uno dei turni precedentemente definiti.</span><span class="sxs-lookup"><span data-stu-id="616e1-123">In the **Work Shift Code** field, select one of the shifts that you previously defined.</span></span> <span data-ttu-id="616e1-124">Aggiungere una riga per ogni giorno lavorativo e ogni turno.</span><span class="sxs-lookup"><span data-stu-id="616e1-124">Add a line for every working day and every shift.</span></span> <span data-ttu-id="616e1-125">Ad esempio:</span><span class="sxs-lookup"><span data-stu-id="616e1-125">For example:</span></span>  

    <span data-ttu-id="616e1-126">Lunedì 07.00 15.00 1</span><span class="sxs-lookup"><span data-stu-id="616e1-126">Monday  07:00 15:00 1</span></span>   
    <span data-ttu-id="616e1-127">Martedì 07.00 15.00 1</span><span class="sxs-lookup"><span data-stu-id="616e1-127">Tuesday 07:00 15:00 1</span></span>  

    <span data-ttu-id="616e1-128">Se è necessario un calendario reparto prod. con due turni lavorativi, occorre compilarlo come illustrato nell'esempio seguente:</span><span class="sxs-lookup"><span data-stu-id="616e1-128">If you need a shop calendar with two work shifts, you must fill it in in this manner:</span></span>  

    <span data-ttu-id="616e1-129">Lunedì 07.00 15.00 1</span><span class="sxs-lookup"><span data-stu-id="616e1-129">Monday 07:00 15:00 1</span></span>   
    <span data-ttu-id="616e1-130">Lunedì 15.00 23.00 2</span><span class="sxs-lookup"><span data-stu-id="616e1-130">Monday 15:00 23:00 2</span></span>  
    <span data-ttu-id="616e1-131">Martedì 07.00 15.00 1</span><span class="sxs-lookup"><span data-stu-id="616e1-131">Tuesday 07:00 15:00 1</span></span>  
    <span data-ttu-id="616e1-132">Martedì 15.00 23.00 2</span><span class="sxs-lookup"><span data-stu-id="616e1-132">Tuesday 15:00 23:00 2</span></span>  

    <span data-ttu-id="616e1-133">Eventuali giorni della settimana non definiti nel calendario reparto produz., ad esempio sabato e domenica, verranno semplicemente considerati giorni non lavorativi e la relativa capacità disponibile sarà pari a zero in un calendario aree di produzione.</span><span class="sxs-lookup"><span data-stu-id="616e1-133">Any week days that you do not define in the shop calendar, such as Saturday and Sunday, are considered non-working days and will have zero available capacity in a work center calendar.</span></span>  

    <span data-ttu-id="616e1-134">Dopo avere definito tutti i giorni lavorativi di una settimana, è possibile chiudere la finestra **Giorni Lavorativi Rep. Prod.** e procedere all'immissione delle ferie.</span><span class="sxs-lookup"><span data-stu-id="616e1-134">When all the working days of a week are defined, you can close the **Shop Calendar Working Days** window and proceed to enter holidays.</span></span>  

6.  <span data-ttu-id="616e1-135">Nella finestra **Calendari reparto prod.**, selezionare il calendario del reparto produzione, quindi scegliere l'azione **Ferie**.</span><span class="sxs-lookup"><span data-stu-id="616e1-135">In the **Shop Calendars** window, select the shop calendar, and then choose the **Holidays** action.</span></span>
7. <span data-ttu-id="616e1-136">Nella finestra **Cal. festività rep. prod.**, definire le ferie dell'anno specificando l'ora e la data di inizio e fine e la descrizione di ogni festività in righe distinte.</span><span class="sxs-lookup"><span data-stu-id="616e1-136">In the **Shop Calendar Holidays** window, define the holidays of the year by entering the start date and time, the end time, and description of each holiday on individual lines.</span></span> <span data-ttu-id="616e1-137">Ad esempio:</span><span class="sxs-lookup"><span data-stu-id="616e1-137">For example:</span></span>  

    <span data-ttu-id="616e1-138">04/07/14 0.00.00 23.59.00 Vacanze estive</span><span class="sxs-lookup"><span data-stu-id="616e1-138">04/07/14 0:00:00 23:59:00 Summer Holiday</span></span>  
    <span data-ttu-id="616e1-139">05/07/14 0.00.00 23.59.00 Vacanze estive</span><span class="sxs-lookup"><span data-stu-id="616e1-139">05/07/14 0:00:00 23:59:00 Summer Holiday</span></span>  
    <span data-ttu-id="616e1-140">06/07/14 0.00.00 23.59.00 Vacanze estive</span><span class="sxs-lookup"><span data-stu-id="616e1-140">06/07/14 0:00:00 23:59:00 Summer Holiday</span></span>  

<span data-ttu-id="616e1-141">La capacità disponibile per le ferie definite sarà pari a zero in un calendario delle aree di produzione.</span><span class="sxs-lookup"><span data-stu-id="616e1-141">The defined holidays will have zero available capacity in a work center calendar.</span></span>  

<span data-ttu-id="616e1-142">È ora possibile assegnare il calendario reparto prod. a un'area di produzione per calcolare il calendario reparto prod. su cui sarà basata la pianificazione di tutte le operazioni in tale area di produzione.</span><span class="sxs-lookup"><span data-stu-id="616e1-142">The shop calendar can now be assigned to a work center to calculate the work shop calendar that will govern all operation scheduling at that work center.</span></span>  

## <a name="to-calculate-a-work-center-calendar"></a><span data-ttu-id="616e1-143">Per calcolare un calendario aree di produzione</span><span class="sxs-lookup"><span data-stu-id="616e1-143">To calculate a work center calendar</span></span>  

1.  <span data-ttu-id="616e1-144">Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **Aree di produzione** e quindi scegliere il collegamento correlato.</span><span class="sxs-lookup"><span data-stu-id="616e1-144">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Work Centers**, and then choose the related link.</span></span>
2. <span data-ttu-id="616e1-145">Aprire l'area di produzione che si desidera aggiornare.</span><span class="sxs-lookup"><span data-stu-id="616e1-145">Open the work center that you want to update.</span></span>  
3. <span data-ttu-id="616e1-146">Nel campo **Cod. calendario reparto prod.**, selezionare il calendario del reparto produzione da utilizzare come base per un calendario delle aree di produzione.</span><span class="sxs-lookup"><span data-stu-id="616e1-146">In the **Shop Calendar Code** field, select which shop calendar to use as the foundation for a work center calendar.</span></span>  
4. <span data-ttu-id="616e1-147">Scegliere l'azione **Calendario**.</span><span class="sxs-lookup"><span data-stu-id="616e1-147">Choose the **Calendar** action.</span></span>  
5. <span data-ttu-id="616e1-148">Nella finestra **Calendario aree di prod.**, scegliere l'azione **Mostra matrice**.</span><span class="sxs-lookup"><span data-stu-id="616e1-148">In the **Work Center Calendar** window, choose the **Show Matrix** action.</span></span>  

    <span data-ttu-id="616e1-149">Nel lato sinistro della matrice sono elencate le aree di produzione configurate.</span><span class="sxs-lookup"><span data-stu-id="616e1-149">The left side of the matrix window lists the work centers that are set up.</span></span> <span data-ttu-id="616e1-150">Nella parte destra è disponibile un calendario, in cui vengono visualizzati i valori relativi alla capacità disponibile per giorno lavorativo nell'unità di misura specificata, ad esempio **480** minuti.</span><span class="sxs-lookup"><span data-stu-id="616e1-150">The right side shows a calendar displaying the available capacity values for each working day in the defined unit of measure, for example, **480** minutes.</span></span> <span data-ttu-id="616e1-151">Ogni riga rappresenta il calendario relativo a un'area di produzione.</span><span class="sxs-lookup"><span data-stu-id="616e1-151">Each line represents the calendar of one work center.</span></span>  

    > [!NOTE]  
    >  <span data-ttu-id="616e1-152">È anche possibile selezionare i valori di capacità per ogni settimana o mese cambiando l'opzione del campo **Visualizza per** nella finestra **Calendario aree di prod.**.</span><span class="sxs-lookup"><span data-stu-id="616e1-152">You can also select to view the capacity values for each week or month by changing the selection in the **View By** field in the **Work Center Calendar** window.</span></span>  

    <span data-ttu-id="616e1-153">Per riflettere il nuovo calendario di reparto come riga dell'area di produzione selezionata, è necessario prima calcolarlo.</span><span class="sxs-lookup"><span data-stu-id="616e1-153">To reflect the new shop calendar as a line on the selected work center, it must first be calculated.</span></span>  

6.  <span data-ttu-id="616e1-154">Scegliere l'azione **Calcola**.</span><span class="sxs-lookup"><span data-stu-id="616e1-154">Choose the **Calculate** action.</span></span>  
7.  <span data-ttu-id="616e1-155">Nella Scheda dettaglio **Area di produzione** è possibile impostare un filtro per eseguire il calcolo solo per un'area di produzione.</span><span class="sxs-lookup"><span data-stu-id="616e1-155">On the **Work Center** FastTab, you can set a filter to only calculate for one work center.</span></span> <span data-ttu-id="616e1-156">Se non si imposta alcun filtro, verranno calcolati tutti i calendari delle aree di produzione esistenti.</span><span class="sxs-lookup"><span data-stu-id="616e1-156">If you do not set a filter, all existing work center calendars will be calculated.</span></span>  
8.  <span data-ttu-id="616e1-157">Definire la data di inizio e di fine del periodo di calendario da calcolare, ad esempio un anno, dal giorno 01/01/14 al 31/12/14.</span><span class="sxs-lookup"><span data-stu-id="616e1-157">Define the starting and ending dates of the calendar period that should be calculated, for example, one year from 01/01/14 to 31/12/14.</span></span>
9. <span data-ttu-id="616e1-158">Scegliere **OK** per calcolare la capacità.</span><span class="sxs-lookup"><span data-stu-id="616e1-158">Choose the **OK** button to calculate capacity.</span></span>  

<span data-ttu-id="616e1-159">Vengono ora creati o aggiornati i movimenti di calendario, in cui viene visualizzata la capacità disponibile per ogni periodo sulla base dei tre gruppi seguenti di dati master:</span><span class="sxs-lookup"><span data-stu-id="616e1-159">Calendar entries are now created or updated displaying the available capacity for each period according to the following three sets of master data:</span></span>  

- <span data-ttu-id="616e1-160">Giorni e turni lavorativi definiti nel calendario reparto prod. assegnato.</span><span class="sxs-lookup"><span data-stu-id="616e1-160">The working days and shift defined in the assigned shop calendar.</span></span>  
- <span data-ttu-id="616e1-161">Valore specificato nel campo **Capacità** della scheda area di produzione.</span><span class="sxs-lookup"><span data-stu-id="616e1-161">The value in the **Capacity** field on the work center card.</span></span>  
- <span data-ttu-id="616e1-162">Valore specificato nel campo **Efficienza** della scheda dell'area di produzione.</span><span class="sxs-lookup"><span data-stu-id="616e1-162">The value in the **Efficiency** field on the work center card.</span></span>  

<span data-ttu-id="616e1-163">Il calendario calcolato dell'area di produzione definirà ora quando e quanta capacità è disponibile in quest'area di produzione.</span><span class="sxs-lookup"><span data-stu-id="616e1-163">The calculated work center calendar will now define when and how much capacity is available at this work center.</span></span> <span data-ttu-id="616e1-164">Ciò controlla la pianificazione dettagliata delle operazioni eseguite nell'area di produzione.</span><span class="sxs-lookup"><span data-stu-id="616e1-164">This controls the detailed scheduling of operations performed at the work center.</span></span>  

## <a name="to-record-work-center-absence"></a><span data-ttu-id="616e1-165">Per registrare un'assenza dell'area di produzione</span><span class="sxs-lookup"><span data-stu-id="616e1-165">To record work center absence</span></span>  
1.  <span data-ttu-id="616e1-166">Nella finestra **Calendario aree di prod.**, scegliere l'azione **Mostra matrice**.</span><span class="sxs-lookup"><span data-stu-id="616e1-166">In the **Work Center Calendar** window, choose the **Show Matrix** action.</span></span>
2. <span data-ttu-id="616e1-167">Nella finestra **Matrice calendario aree di prod.** selezionare l'area di produzione e il giornio di calendario in cui registrare l'orario di assenza, quindi scegliere l'azione **Assenze**.</span><span class="sxs-lookup"><span data-stu-id="616e1-167">In the **Work Center Calendar Matrix** window, select the work center and calendar day when the absence time should be recorded, and then choose the **Absence** action.</span></span>  
3.  <span data-ttu-id="616e1-168">Nella finestra **Assenze** definire l'ora di inizio, l'ora di fine e la descrizione dell'assenza relativa al giorno specificato.</span><span class="sxs-lookup"><span data-stu-id="616e1-168">In the **Absence** window, define the starting time, ending time, and description of that day’s absence.</span></span> <span data-ttu-id="616e1-169">Ad esempio:</span><span class="sxs-lookup"><span data-stu-id="616e1-169">For example:</span></span>  

    <span data-ttu-id="616e1-170">25/01/01 08.00 10.00 Manutenzione</span><span class="sxs-lookup"><span data-stu-id="616e1-170">25/01/01 08:00 10:00 Maintenance</span></span>  

4.  <span data-ttu-id="616e1-171">Scegliere l'azione **Aggiorna** e chiudere la finestra **Assenze**.</span><span class="sxs-lookup"><span data-stu-id="616e1-171">Choose the **Update** action, and then close the **Absence** window.</span></span>  

<span data-ttu-id="616e1-172">La capacità del giorno selezionato risulta ora diminuita in base al tempo di assenza registrato.</span><span class="sxs-lookup"><span data-stu-id="616e1-172">The capacity of the selected day has now decreased by the recorded absence time.</span></span>  

## <a name="see-also"></a><span data-ttu-id="616e1-173">Vedi anche</span><span class="sxs-lookup"><span data-stu-id="616e1-173">See Also</span></span>  
[<span data-ttu-id="616e1-174">Procedura: Impostare i calendari di base</span><span class="sxs-lookup"><span data-stu-id="616e1-174">How to: Set Up Base Calendars</span></span>](across-how-to-assign-base-calendars.md)  
[<span data-ttu-id="616e1-175">Procedura: Impostare aree di produzione e centri di lavoro</span><span class="sxs-lookup"><span data-stu-id="616e1-175">How to: Set Up Work Centers and Machine Centers</span></span>](production-how-to-set-up-work-and-machine-centers.md)  
[<span data-ttu-id="616e1-176">Impostazione della produzione</span><span class="sxs-lookup"><span data-stu-id="616e1-176">Setting Up Manufacturing</span></span>](production-configure-production-processes.md)  
[<span data-ttu-id="616e1-177">Manufacturing</span><span class="sxs-lookup"><span data-stu-id="616e1-177">Manufacturing</span></span>](production-manage-manufacturing.md)  
<span data-ttu-id="616e1-178">[Utilizzo di [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="616e1-178">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  
