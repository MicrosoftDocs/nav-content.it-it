---
title: "Dettagli di progettazione - Movimenti di tracciabilità articolo storici e attivi"
description: "Quando vengono registrate parti di una quantità di una riga documento, solo quella quantità in questione viene trasferita ai movimenti contabili articoli e ai relativi numeri di tracciabilità articolo. Tuttavia, è opportuno accedere a tutte le informazioni rilevanti di tracciabilità articoli direttamente dalla riga del documento attivo. Ovvero non solo si desidererà vedere i movimenti che sono correlati alla quantità residua, ma si vorranno anche informazioni sulle unità che sono state registrate. Quando si visualizza o si modifica la finestra **Righe tracciabilità articolo**, i contenuti collettivi delle tabelle **Specifica tracciabilità** (T336) e **Movimenti impegni** (T337) vengono presentati in una versione temporanea di T336. In questo modo si garantisce l'accesso unico ai dati di tracciabilità articolo attivi e storici."
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
ms.openlocfilehash: 315b5317c2ac3e2cd6a56bd243e30d4e3445a6ec
ms.contentlocale: it-it
ms.lasthandoff: 10/16/2017

---
# <a name="design-details-active-versus-historic-item-tracking-entries"></a><span data-ttu-id="1e0c4-107">Dettagli di progettazione: Movimenti di tracciabilità articolo storici e attivi</span><span class="sxs-lookup"><span data-stu-id="1e0c4-107">Design Details: Active versus Historic Item Tracking Entries</span></span>
<span data-ttu-id="1e0c4-108">Quando vengono registrate parti di una quantità di una riga documento, solo quella quantità in questione viene trasferita ai movimenti contabili articoli e ai relativi numeri di tracciabilità articolo.</span><span class="sxs-lookup"><span data-stu-id="1e0c4-108">When parts of a document line quantity are posted, only that particular quantity is transferred to the item ledger entries and its item tracking numbers.</span></span> <span data-ttu-id="1e0c4-109">Tuttavia, è opportuno accedere a tutte le informazioni rilevanti di tracciabilità articoli direttamente dalla riga del documento attivo.</span><span class="sxs-lookup"><span data-stu-id="1e0c4-109">However, you will want to access all relevant item tracking information directly from the active document line.</span></span> <span data-ttu-id="1e0c4-110">Ovvero non solo si desidererà vedere i movimenti che sono correlati alla quantità residua, ma si vorranno anche informazioni sulle unità che sono state registrate.</span><span class="sxs-lookup"><span data-stu-id="1e0c4-110">That is, not only will you want to see the entries that are related to the remaining quantity, you will also want information about the units that have been posted.</span></span> <span data-ttu-id="1e0c4-111">Quando si visualizza o si modifica la finestra **Righe tracciabilità articolo**, i contenuti collettivi delle tabelle **Specifica tracciabilità** (T336) e **Movimenti impegni** (T337) vengono presentati in una versione temporanea di T336.</span><span class="sxs-lookup"><span data-stu-id="1e0c4-111">When you view or modify the **Item Tracking Lines** window, the collective contents of the **Tracking Specification** table (T336) and **Reservation Entry** table (T337) are presented in a temporary version of T336.</span></span> <span data-ttu-id="1e0c4-112">In questo modo si garantisce l'accesso unico ai dati di tracciabilità articolo attivi e storici.</span><span class="sxs-lookup"><span data-stu-id="1e0c4-112">This ensures that historic and active item tracking data is accessed as one.</span></span>  

 <span data-ttu-id="1e0c4-113">Nella seguente tabella viene mostrato come T336 e T337 vengono utilizzati in uno scenario di acquisto.</span><span class="sxs-lookup"><span data-stu-id="1e0c4-113">The following table shows how T336 and T337 are used in a purchase scenario.</span></span> <span data-ttu-id="1e0c4-114">Le cifre in grassetto rappresentano i valori che l'utente immette manualmente nella finestra **Righe tracciabilità articolo**.</span><span class="sxs-lookup"><span data-stu-id="1e0c4-114">The bold figures represent values that the user manually enters in the **Item Tracking Lines** window.</span></span>  

 <span data-ttu-id="1e0c4-115">Passaggio 1: Creare una riga di ordine di acquisto di sette pezzi con numeri di tracciabilità articolo.</span><span class="sxs-lookup"><span data-stu-id="1e0c4-115">Step 1: Create a purchase order line of seven pieces with item tracking numbers.</span></span>  

||<span data-ttu-id="1e0c4-116">**Quantità (base)**</span><span class="sxs-lookup"><span data-stu-id="1e0c4-116">**Quantity (Base)**</span></span>|<span data-ttu-id="1e0c4-117">**Qtà da gestire**</span><span class="sxs-lookup"><span data-stu-id="1e0c4-117">**Qty. to Handle**</span></span>|<span data-ttu-id="1e0c4-118">**Qtà da fatturare (base)**</span><span class="sxs-lookup"><span data-stu-id="1e0c4-118">**Qty. to Invoice (Base)**</span></span>|<span data-ttu-id="1e0c4-119">**Quantità gestita (base)**</span><span class="sxs-lookup"><span data-stu-id="1e0c4-119">**Quantity Handled (Base)**</span></span>|<span data-ttu-id="1e0c4-120">**Quantità fatturata (base)**</span><span class="sxs-lookup"><span data-stu-id="1e0c4-120">**Quantity Invoiced (Base)**</span></span>|  
|-|----------------------------------------------|--------------------------------------------|------------------------------------------------------|-------------------------------------------------------|--------------------------------------------------------|  
|<span data-ttu-id="1e0c4-121">**T337**</span><span class="sxs-lookup"><span data-stu-id="1e0c4-121">**T337**</span></span>|<span data-ttu-id="1e0c4-122">7</span><span class="sxs-lookup"><span data-stu-id="1e0c4-122">7</span></span>|<span data-ttu-id="1e0c4-123">0</span><span class="sxs-lookup"><span data-stu-id="1e0c4-123">0</span></span>|<span data-ttu-id="1e0c4-124">0</span><span class="sxs-lookup"><span data-stu-id="1e0c4-124">0</span></span>|<span data-ttu-id="1e0c4-125">0</span><span class="sxs-lookup"><span data-stu-id="1e0c4-125">0</span></span>|<span data-ttu-id="1e0c4-126">0</span><span class="sxs-lookup"><span data-stu-id="1e0c4-126">0</span></span>|  
|<span data-ttu-id="1e0c4-127">**T336**</span><span class="sxs-lookup"><span data-stu-id="1e0c4-127">**T336**</span></span>|<span data-ttu-id="1e0c4-128">0</span><span class="sxs-lookup"><span data-stu-id="1e0c4-128">0</span></span>|<span data-ttu-id="1e0c4-129">0</span><span class="sxs-lookup"><span data-stu-id="1e0c4-129">0</span></span>|<span data-ttu-id="1e0c4-130">0</span><span class="sxs-lookup"><span data-stu-id="1e0c4-130">0</span></span>|<span data-ttu-id="1e0c4-131">0</span><span class="sxs-lookup"><span data-stu-id="1e0c4-131">0</span></span>|<span data-ttu-id="1e0c4-132">0</span><span class="sxs-lookup"><span data-stu-id="1e0c4-132">0</span></span>|  

 <span data-ttu-id="1e0c4-133">Passaggio 2: Ricevere quattro pezzi.</span><span class="sxs-lookup"><span data-stu-id="1e0c4-133">Step 2: Receive four pieces.</span></span>  

||<span data-ttu-id="1e0c4-134">**Quantità (base)**</span><span class="sxs-lookup"><span data-stu-id="1e0c4-134">**Quantity (Base)**</span></span>|<span data-ttu-id="1e0c4-135">**Qtà da gestire**</span><span class="sxs-lookup"><span data-stu-id="1e0c4-135">**Qty. to Handle**</span></span>|<span data-ttu-id="1e0c4-136">**Qtà da fatturare (base)**</span><span class="sxs-lookup"><span data-stu-id="1e0c4-136">**Qty. to Invoice (Base)**</span></span>|<span data-ttu-id="1e0c4-137">**Quantità gestita (base)**</span><span class="sxs-lookup"><span data-stu-id="1e0c4-137">**Quantity Handled (Base)**</span></span>|<span data-ttu-id="1e0c4-138">**Quantità fatturata (base)**</span><span class="sxs-lookup"><span data-stu-id="1e0c4-138">**Quantity Invoiced (Base)**</span></span>|  
|-|----------------------------------------------|--------------------------------------------|------------------------------------------------------|-------------------------------------------------------|--------------------------------------------------------|  
|<span data-ttu-id="1e0c4-139">Finestra **Righe tracciabilità articolo**</span><span class="sxs-lookup"><span data-stu-id="1e0c4-139">**Item Tracking Lines** window</span></span>|<span data-ttu-id="1e0c4-140">7</span><span class="sxs-lookup"><span data-stu-id="1e0c4-140">7</span></span>|<span data-ttu-id="1e0c4-141">**4**</span><span class="sxs-lookup"><span data-stu-id="1e0c4-141">**4**</span></span>|<span data-ttu-id="1e0c4-142">**0**</span><span class="sxs-lookup"><span data-stu-id="1e0c4-142">**0**</span></span>|<span data-ttu-id="1e0c4-143">0</span><span class="sxs-lookup"><span data-stu-id="1e0c4-143">0</span></span>|<span data-ttu-id="1e0c4-144">0</span><span class="sxs-lookup"><span data-stu-id="1e0c4-144">0</span></span>|  
|<span data-ttu-id="1e0c4-145">**T337**</span><span class="sxs-lookup"><span data-stu-id="1e0c4-145">**T337**</span></span>|<span data-ttu-id="1e0c4-146">3</span><span class="sxs-lookup"><span data-stu-id="1e0c4-146">3</span></span>|<span data-ttu-id="1e0c4-147">0</span><span class="sxs-lookup"><span data-stu-id="1e0c4-147">0</span></span>|<span data-ttu-id="1e0c4-148">0</span><span class="sxs-lookup"><span data-stu-id="1e0c4-148">0</span></span>|<span data-ttu-id="1e0c4-149">0</span><span class="sxs-lookup"><span data-stu-id="1e0c4-149">0</span></span>|<span data-ttu-id="1e0c4-150">0</span><span class="sxs-lookup"><span data-stu-id="1e0c4-150">0</span></span>|  
|<span data-ttu-id="1e0c4-151">**T336**</span><span class="sxs-lookup"><span data-stu-id="1e0c4-151">**T336**</span></span>|<span data-ttu-id="1e0c4-152">4</span><span class="sxs-lookup"><span data-stu-id="1e0c4-152">4</span></span>|<span data-ttu-id="1e0c4-153">0</span><span class="sxs-lookup"><span data-stu-id="1e0c4-153">0</span></span>|<span data-ttu-id="1e0c4-154">0</span><span class="sxs-lookup"><span data-stu-id="1e0c4-154">0</span></span>|<span data-ttu-id="1e0c4-155">4</span><span class="sxs-lookup"><span data-stu-id="1e0c4-155">4</span></span>|<span data-ttu-id="1e0c4-156">0</span><span class="sxs-lookup"><span data-stu-id="1e0c4-156">0</span></span>|  

 <span data-ttu-id="1e0c4-157">Passaggio 3: Ricevere due pezzi e fatturare due pezzi.</span><span class="sxs-lookup"><span data-stu-id="1e0c4-157">Step 3: Receive two pieces and invoice two pieces.</span></span>  

||<span data-ttu-id="1e0c4-158">**Quantità (base)**</span><span class="sxs-lookup"><span data-stu-id="1e0c4-158">**Quantity (Base)**</span></span>|<span data-ttu-id="1e0c4-159">**Qtà da gestire**</span><span class="sxs-lookup"><span data-stu-id="1e0c4-159">**Qty. to Handle**</span></span>|<span data-ttu-id="1e0c4-160">**Qtà da fatturare (base)**</span><span class="sxs-lookup"><span data-stu-id="1e0c4-160">**Qty. to Invoice (Base)**</span></span>|<span data-ttu-id="1e0c4-161">**Quantità gestita (base)**</span><span class="sxs-lookup"><span data-stu-id="1e0c4-161">**Quantity Handled (Base)**</span></span>|<span data-ttu-id="1e0c4-162">**Quantità fatturata (base)**</span><span class="sxs-lookup"><span data-stu-id="1e0c4-162">**Quantity Invoiced (Base)**</span></span>|  
|-|----------------------------------------------|--------------------------------------------|------------------------------------------------------|-------------------------------------------------------|--------------------------------------------------------|  
|<span data-ttu-id="1e0c4-163">Finestra **Righe tracciabilità articolo**</span><span class="sxs-lookup"><span data-stu-id="1e0c4-163">**Item Tracking Lines** window</span></span>|<span data-ttu-id="1e0c4-164">7</span><span class="sxs-lookup"><span data-stu-id="1e0c4-164">7</span></span>|<span data-ttu-id="1e0c4-165">**2**</span><span class="sxs-lookup"><span data-stu-id="1e0c4-165">**2**</span></span>|<span data-ttu-id="1e0c4-166">**2**</span><span class="sxs-lookup"><span data-stu-id="1e0c4-166">**2**</span></span>|<span data-ttu-id="1e0c4-167">4</span><span class="sxs-lookup"><span data-stu-id="1e0c4-167">4</span></span>|<span data-ttu-id="1e0c4-168">0</span><span class="sxs-lookup"><span data-stu-id="1e0c4-168">0</span></span>|  
|<span data-ttu-id="1e0c4-169">**T337**</span><span class="sxs-lookup"><span data-stu-id="1e0c4-169">**T337**</span></span>|<span data-ttu-id="1e0c4-170">1</span><span class="sxs-lookup"><span data-stu-id="1e0c4-170">1</span></span>|<span data-ttu-id="1e0c4-171">0</span><span class="sxs-lookup"><span data-stu-id="1e0c4-171">0</span></span>|<span data-ttu-id="1e0c4-172">0</span><span class="sxs-lookup"><span data-stu-id="1e0c4-172">0</span></span>|<span data-ttu-id="1e0c4-173">0</span><span class="sxs-lookup"><span data-stu-id="1e0c4-173">0</span></span>|<span data-ttu-id="1e0c4-174">0</span><span class="sxs-lookup"><span data-stu-id="1e0c4-174">0</span></span>|  
|<span data-ttu-id="1e0c4-175">**T336**</span><span class="sxs-lookup"><span data-stu-id="1e0c4-175">**T336**</span></span>|<span data-ttu-id="1e0c4-176">6</span><span class="sxs-lookup"><span data-stu-id="1e0c4-176">6</span></span>|<span data-ttu-id="1e0c4-177">0</span><span class="sxs-lookup"><span data-stu-id="1e0c4-177">0</span></span>|<span data-ttu-id="1e0c4-178">0</span><span class="sxs-lookup"><span data-stu-id="1e0c4-178">0</span></span>|<span data-ttu-id="1e0c4-179">6</span><span class="sxs-lookup"><span data-stu-id="1e0c4-179">6</span></span>|<span data-ttu-id="1e0c4-180">2</span><span class="sxs-lookup"><span data-stu-id="1e0c4-180">2</span></span>|  

 <span data-ttu-id="1e0c4-181">Passaggio 4: Ricevere un pezzo.</span><span class="sxs-lookup"><span data-stu-id="1e0c4-181">Step 4: Receive one piece.</span></span>  

||<span data-ttu-id="1e0c4-182">**Quantità (base)**</span><span class="sxs-lookup"><span data-stu-id="1e0c4-182">**Quantity (Base)**</span></span>|<span data-ttu-id="1e0c4-183">**Qtà da gestire**</span><span class="sxs-lookup"><span data-stu-id="1e0c4-183">**Qty. to Handle**</span></span>|<span data-ttu-id="1e0c4-184">**Qtà da fatturare (base)**</span><span class="sxs-lookup"><span data-stu-id="1e0c4-184">**Qty. to Invoice (Base)**</span></span>|<span data-ttu-id="1e0c4-185">**Quantità gestita (base)**</span><span class="sxs-lookup"><span data-stu-id="1e0c4-185">**Quantity Handled (Base)**</span></span>|<span data-ttu-id="1e0c4-186">**Quantità fatturata (base)**</span><span class="sxs-lookup"><span data-stu-id="1e0c4-186">**Quantity Invoiced (Base)**</span></span>|  
|-|----------------------------------------------|--------------------------------------------|------------------------------------------------------|-------------------------------------------------------|--------------------------------------------------------|  
|<span data-ttu-id="1e0c4-187">Finestra **Righe tracciabilità articolo**</span><span class="sxs-lookup"><span data-stu-id="1e0c4-187">**Item Tracking Lines** window</span></span>|<span data-ttu-id="1e0c4-188">7</span><span class="sxs-lookup"><span data-stu-id="1e0c4-188">7</span></span>|<span data-ttu-id="1e0c4-189">**1**</span><span class="sxs-lookup"><span data-stu-id="1e0c4-189">**1**</span></span>|<span data-ttu-id="1e0c4-190">**0**</span><span class="sxs-lookup"><span data-stu-id="1e0c4-190">**0**</span></span>|<span data-ttu-id="1e0c4-191">6</span><span class="sxs-lookup"><span data-stu-id="1e0c4-191">6</span></span>|<span data-ttu-id="1e0c4-192">2</span><span class="sxs-lookup"><span data-stu-id="1e0c4-192">2</span></span>|  
|<span data-ttu-id="1e0c4-193">**T336**</span><span class="sxs-lookup"><span data-stu-id="1e0c4-193">**T336**</span></span>|<span data-ttu-id="1e0c4-194">7</span><span class="sxs-lookup"><span data-stu-id="1e0c4-194">7</span></span>|<span data-ttu-id="1e0c4-195">0</span><span class="sxs-lookup"><span data-stu-id="1e0c4-195">0</span></span>|<span data-ttu-id="1e0c4-196">0</span><span class="sxs-lookup"><span data-stu-id="1e0c4-196">0</span></span>|<span data-ttu-id="1e0c4-197">7</span><span class="sxs-lookup"><span data-stu-id="1e0c4-197">7</span></span>|<span data-ttu-id="1e0c4-198">2</span><span class="sxs-lookup"><span data-stu-id="1e0c4-198">2</span></span>|  

 <span data-ttu-id="1e0c4-199">Fatturare 5 pezzi.</span><span class="sxs-lookup"><span data-stu-id="1e0c4-199">Invoice 5 pieces.</span></span>  

||<span data-ttu-id="1e0c4-200">**Quantità (base)**</span><span class="sxs-lookup"><span data-stu-id="1e0c4-200">**Quantity (Base)**</span></span>|<span data-ttu-id="1e0c4-201">**Qtà da gestire**</span><span class="sxs-lookup"><span data-stu-id="1e0c4-201">**Qty. to Handle**</span></span>|<span data-ttu-id="1e0c4-202">**Qtà da fatturare (base)**</span><span class="sxs-lookup"><span data-stu-id="1e0c4-202">**Qty. to Invoice (Base)**</span></span>|<span data-ttu-id="1e0c4-203">**Quantità gestita (base)**</span><span class="sxs-lookup"><span data-stu-id="1e0c4-203">**Quantity Handled (Base)**</span></span>|<span data-ttu-id="1e0c4-204">**Quantità fatturata (base)**</span><span class="sxs-lookup"><span data-stu-id="1e0c4-204">**Quantity Invoiced (Base)**</span></span>|  
|-|----------------------------------------------|--------------------------------------------|------------------------------------------------------|-------------------------------------------------------|--------------------------------------------------------|  
|<span data-ttu-id="1e0c4-205">Finestra **Righe tracciabilità articolo**</span><span class="sxs-lookup"><span data-stu-id="1e0c4-205">**Item Tracking Lines** window</span></span>|<span data-ttu-id="1e0c4-206">7</span><span class="sxs-lookup"><span data-stu-id="1e0c4-206">7</span></span>|<span data-ttu-id="1e0c4-207">0</span><span class="sxs-lookup"><span data-stu-id="1e0c4-207">0</span></span>|<span data-ttu-id="1e0c4-208">**5**</span><span class="sxs-lookup"><span data-stu-id="1e0c4-208">**5**</span></span>|<span data-ttu-id="1e0c4-209">7</span><span class="sxs-lookup"><span data-stu-id="1e0c4-209">7</span></span>|<span data-ttu-id="1e0c4-210">2</span><span class="sxs-lookup"><span data-stu-id="1e0c4-210">2</span></span>|  
|<span data-ttu-id="1e0c4-211">**T336**</span><span class="sxs-lookup"><span data-stu-id="1e0c4-211">**T336**</span></span>|<span data-ttu-id="1e0c4-212">7</span><span class="sxs-lookup"><span data-stu-id="1e0c4-212">7</span></span>|<span data-ttu-id="1e0c4-213">0</span><span class="sxs-lookup"><span data-stu-id="1e0c4-213">0</span></span>|<span data-ttu-id="1e0c4-214">0</span><span class="sxs-lookup"><span data-stu-id="1e0c4-214">0</span></span>|<span data-ttu-id="1e0c4-215">7</span><span class="sxs-lookup"><span data-stu-id="1e0c4-215">7</span></span>|<span data-ttu-id="1e0c4-216">7</span><span class="sxs-lookup"><span data-stu-id="1e0c4-216">7</span></span>|  

## <a name="see-also"></a><span data-ttu-id="1e0c4-217">Vedi anche</span><span class="sxs-lookup"><span data-stu-id="1e0c4-217">See Also</span></span>  
 <span data-ttu-id="1e0c4-218">[Dettagli di progettazione: Tracciabilità articolo](design-details-item-tracking.md) </span><span class="sxs-lookup"><span data-stu-id="1e0c4-218">[Design Details: Item Tracking](design-details-item-tracking.md) </span></span>  
 [<span data-ttu-id="1e0c4-219">Dettagli di progettazione: Finestra righe tracciabilità articolo</span><span class="sxs-lookup"><span data-stu-id="1e0c4-219">Design Details: Item Tracking Lines Window</span></span>](design-details-item-tracking-lines-window.md)
