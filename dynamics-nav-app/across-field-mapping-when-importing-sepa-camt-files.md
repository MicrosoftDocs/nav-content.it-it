---
title: Mapping dei campi durante l'importazione dei file SEPA CAMT
description: "Nei mercati europei è possibile importare i file del rendiconto bancario negli standard SEPA (Single Euro Payments Area) locali."
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/18/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 88f949bb211845a1c3c0e5f0b364d4ea26cfd13f
ms.contentlocale: it-it
ms.lasthandoff: 10/16/2017

---
# <a name="field-mapping-when-importing-sepa-camt-files"></a><span data-ttu-id="a8eb8-103">Mapping dei campi durante l'importazione dei file SEPA CAMT</span><span class="sxs-lookup"><span data-stu-id="a8eb8-103">Field Mapping When Importing SEPA CAMT Files</span></span>
<span data-ttu-id="a8eb8-104">La versione generica di [!INCLUDE[d365fin](includes/d365fin_md.md)] supporta gli standard SEPA (Single Euro Payments Area)per l'importazione dei rendiconti bancari SEPA (formato CAMT).</span><span class="sxs-lookup"><span data-stu-id="a8eb8-104">[!INCLUDE[d365fin](includes/d365fin_md.md)] supports the regional SEPA standards (Single Euro Payments Area) for importing SEPA bank statements (CAMT format).</span></span> <span data-ttu-id="a8eb8-105">Per ulteriori informazioni, vedere [Procedura: Impostare il servizio di conversione di dati bancari](bank-how-setup-bank-data-conversion-service.md).</span><span class="sxs-lookup"><span data-stu-id="a8eb8-105">For more information, see [How to: Set Up the Bank Data Conversion Service](bank-how-setup-bank-data-conversion-service.md).</span></span>  

 <span data-ttu-id="a8eb8-106">Lo standard SEPA CAMT include di per sé variazioni locali.</span><span class="sxs-lookup"><span data-stu-id="a8eb8-106">The SEPA CAMT standard itself has local variations.</span></span> <span data-ttu-id="a8eb8-107">Di conseguenza, è possibile che si debba modificare la definizione di scambio dati generica rappresentata dal codice **SEPA CAMT** nella finestra **Registrazione definizioni di scambio** per adattarla a una variazione locale dello standard.</span><span class="sxs-lookup"><span data-stu-id="a8eb8-107">Therefore, you may have to modify the generic data exchange definition (represented by the **SEPA CAMT** code in the **Posting Exchange Definitions** window to adapt it to a local variation of the standard.</span></span> <span data-ttu-id="a8eb8-108">Nelle seguenti tabelle viene mostrato il mapping tra elementi e campi per le tabelle 81, 273 e 274 nell'implementazione SEPA CAMT in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="a8eb8-108">The following tables show the element-to-field mapping for tables 81, 273, and 274 in the SEPA CAMT implementation in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span>  

 <span data-ttu-id="a8eb8-109">Per informazioni sulla creazione o la modifica della definizione di scambio dati, vedere [Procedura: Impostare le definizioni di scambio dati](across-how-to-set-up-data-exchange-definitions.md).</span><span class="sxs-lookup"><span data-stu-id="a8eb8-109">For information about creating or adjusting a data exchange definition, see [How to: Set Up Data Exchange Definitions](across-how-to-set-up-data-exchange-definitions.md).</span></span>  

## <a name="camt-data-mapping-to-fields-in-the-general-journal-table-81"></a><span data-ttu-id="a8eb8-110">Mapping dei dati CAMT ai campi nella tabella Contabilità generale (81)</span><span class="sxs-lookup"><span data-stu-id="a8eb8-110">CAMT data mapping to fields in the General Journal table (81)</span></span>  

|<span data-ttu-id="a8eb8-111">Percorso dell'articolo</span><span class="sxs-lookup"><span data-stu-id="a8eb8-111">Element Path</span></span>|<span data-ttu-id="a8eb8-112">Elemento messaggio</span><span class="sxs-lookup"><span data-stu-id="a8eb8-112">Message Element</span></span>|<span data-ttu-id="a8eb8-113">Tipo di dati</span><span class="sxs-lookup"><span data-stu-id="a8eb8-113">Data Type</span></span>|<span data-ttu-id="a8eb8-114">Descrizione</span><span class="sxs-lookup"><span data-stu-id="a8eb8-114">Description</span></span>|<span data-ttu-id="a8eb8-115">Identificatore segno negativo</span><span class="sxs-lookup"><span data-stu-id="a8eb8-115">Negative-Sign Identifier</span></span>|<span data-ttu-id="a8eb8-116">Nr. campo</span><span class="sxs-lookup"><span data-stu-id="a8eb8-116">Field No.</span></span>|<span data-ttu-id="a8eb8-117">Nome campo</span><span class="sxs-lookup"><span data-stu-id="a8eb8-117">Field Name</span></span>|  
|------------------|---------------------|---------------|-----------------|-------------------------------|---------------|----------------|  
|<span data-ttu-id="a8eb8-118">Stmt/Ntry/Amt</span><span class="sxs-lookup"><span data-stu-id="a8eb8-118">Stmt/Ntry/Amt</span></span>|<span data-ttu-id="a8eb8-119">Importo</span><span class="sxs-lookup"><span data-stu-id="a8eb8-119">Amount</span></span>|<span data-ttu-id="a8eb8-120">Decimale</span><span class="sxs-lookup"><span data-stu-id="a8eb8-120">Decimal</span></span>|<span data-ttu-id="a8eb8-121">Specifica l'importo di denaro nel movimento cassa.</span><span class="sxs-lookup"><span data-stu-id="a8eb8-121">The amount of money in the cash entry</span></span>||<span data-ttu-id="a8eb8-122">13</span><span class="sxs-lookup"><span data-stu-id="a8eb8-122">13</span></span>|<span data-ttu-id="a8eb8-123">Importo</span><span class="sxs-lookup"><span data-stu-id="a8eb8-123">Amount</span></span>|  
|<span data-ttu-id="a8eb8-124">Stmt/Ntry/CdtDbtInd</span><span class="sxs-lookup"><span data-stu-id="a8eb8-124">Stmt/Ntry/CdtDbtInd</span></span>|<span data-ttu-id="a8eb8-125">CreditDebitIndicator</span><span class="sxs-lookup"><span data-stu-id="a8eb8-125">CreditDebitIndicator</span></span>|<span data-ttu-id="a8eb8-126">Testo</span><span class="sxs-lookup"><span data-stu-id="a8eb8-126">Text</span></span>|<span data-ttu-id="a8eb8-127">Indica se il movimento è un credito o un debito</span><span class="sxs-lookup"><span data-stu-id="a8eb8-127">Indicates whether the entry is a credit or a debit entry</span></span>|<span data-ttu-id="a8eb8-128">DBIT</span><span class="sxs-lookup"><span data-stu-id="a8eb8-128">DBIT</span></span>|<span data-ttu-id="a8eb8-129">13</span><span class="sxs-lookup"><span data-stu-id="a8eb8-129">13</span></span>|<span data-ttu-id="a8eb8-130">Importo</span><span class="sxs-lookup"><span data-stu-id="a8eb8-130">Amount</span></span>|  
|<span data-ttu-id="a8eb8-131">Stmt/Ntry/BookgDt/Dt</span><span class="sxs-lookup"><span data-stu-id="a8eb8-131">Stmt/Ntry/BookgDt/Dt</span></span>|<span data-ttu-id="a8eb8-132">Data</span><span class="sxs-lookup"><span data-stu-id="a8eb8-132">Date</span></span>|<span data-ttu-id="a8eb8-133">Data</span><span class="sxs-lookup"><span data-stu-id="a8eb8-133">Date</span></span>|<span data-ttu-id="a8eb8-134">Data in cui un movimento viene registrato in un conto nei registri di chi utilizza il conto</span><span class="sxs-lookup"><span data-stu-id="a8eb8-134">The date when an entry is posted to an account on the account servicer's books</span></span>||<span data-ttu-id="a8eb8-135">5</span><span class="sxs-lookup"><span data-stu-id="a8eb8-135">5</span></span>|<span data-ttu-id="a8eb8-136">Data di registrazione:</span><span class="sxs-lookup"><span data-stu-id="a8eb8-136">Posting Date</span></span>|  
|<span data-ttu-id="a8eb8-137">Stmt/Ntry/BookgDt/DtTm</span><span class="sxs-lookup"><span data-stu-id="a8eb8-137">Stmt/Ntry/BookgDt/DtTm</span></span>|<span data-ttu-id="a8eb8-138">DataOra</span><span class="sxs-lookup"><span data-stu-id="a8eb8-138">DateTime</span></span>|<span data-ttu-id="a8eb8-139">DataOra</span><span class="sxs-lookup"><span data-stu-id="a8eb8-139">DateTime</span></span>|<span data-ttu-id="a8eb8-140">Data e ora in cui un movimento viene registrato in un conto nei registri di chi utilizza il conto</span><span class="sxs-lookup"><span data-stu-id="a8eb8-140">The date and time when an entry is posted to an account on the account servicer's books</span></span>||<span data-ttu-id="a8eb8-141">5</span><span class="sxs-lookup"><span data-stu-id="a8eb8-141">5</span></span>|<span data-ttu-id="a8eb8-142">Data di registrazione:</span><span class="sxs-lookup"><span data-stu-id="a8eb8-142">Posting Date</span></span>|  
|<span data-ttu-id="a8eb8-143">Stmt/Ntry/NtryDtls/TxDtls/RltdPties/Dbtr/Nm</span><span class="sxs-lookup"><span data-stu-id="a8eb8-143">Stmt/Ntry/NtryDtls/TxDtls/RltdPties/Dbtr/Nm</span></span>|<span data-ttu-id="a8eb8-144">Nome</span><span class="sxs-lookup"><span data-stu-id="a8eb8-144">Name</span></span>|<span data-ttu-id="a8eb8-145">Testo</span><span class="sxs-lookup"><span data-stu-id="a8eb8-145">Text</span></span>|<span data-ttu-id="a8eb8-146">Nome della parte che deve una somma di denaro al creditore (finale)</span><span class="sxs-lookup"><span data-stu-id="a8eb8-146">The name of the party that owes an amount of money to the (ultimate) creditor</span></span>||<span data-ttu-id="a8eb8-147">1221</span><span class="sxs-lookup"><span data-stu-id="a8eb8-147">1221</span></span>|<span data-ttu-id="a8eb8-148">Informazioni sul pagante</span><span class="sxs-lookup"><span data-stu-id="a8eb8-148">Payer Information</span></span>|  
|<span data-ttu-id="a8eb8-149">Stmt/Ntry/NtryDtls/TxDtls/RmtInf/Ustrd</span><span class="sxs-lookup"><span data-stu-id="a8eb8-149">Stmt/Ntry/NtryDtls/TxDtls/RmtInf/Ustrd</span></span>|<span data-ttu-id="a8eb8-150">Non strutturato</span><span class="sxs-lookup"><span data-stu-id="a8eb8-150">Unstructured</span></span>|<span data-ttu-id="a8eb8-151">Testo</span><span class="sxs-lookup"><span data-stu-id="a8eb8-151">Text</span></span>|<span data-ttu-id="a8eb8-152">Informazioni fornite per consentire la corrispondenza o riconciliazione di un movimento con gli articoli oggetto del pagamento, come le fatture aziendali in un sistema conto clienti, in un form non strutturato</span><span class="sxs-lookup"><span data-stu-id="a8eb8-152">Information supplied to enable the matching/reconciliation of an entry with the items that the payment is intended to settle, such as commercial invoices in an accounts-receivable system, in an unstructured form</span></span>||<span data-ttu-id="a8eb8-153">8</span><span class="sxs-lookup"><span data-stu-id="a8eb8-153">8</span></span>|<span data-ttu-id="a8eb8-154">Descrizione</span><span class="sxs-lookup"><span data-stu-id="a8eb8-154">Description</span></span>|  
|<span data-ttu-id="a8eb8-155">Stmt/Ntry/AddtlNtryInf</span><span class="sxs-lookup"><span data-stu-id="a8eb8-155">Stmt/Ntry/AddtlNtryInf</span></span>|<span data-ttu-id="a8eb8-156">AdditionalEntryInformation</span><span class="sxs-lookup"><span data-stu-id="a8eb8-156">AdditionalEntryInformation</span></span>|<span data-ttu-id="a8eb8-157">Testo</span><span class="sxs-lookup"><span data-stu-id="a8eb8-157">Text</span></span>|<span data-ttu-id="a8eb8-158">Informazioni aggiuntive relative al movimento</span><span class="sxs-lookup"><span data-stu-id="a8eb8-158">Additional information about the entry</span></span>||<span data-ttu-id="a8eb8-159">1222</span><span class="sxs-lookup"><span data-stu-id="a8eb8-159">1222</span></span>|<span data-ttu-id="a8eb8-160">Informazioni sulla transazione</span><span class="sxs-lookup"><span data-stu-id="a8eb8-160">Transaction Information</span></span>|  

## <a name="camt-data-mapping-to-fields-in-the-bank-acc-reconciliation-table-273"></a><span data-ttu-id="a8eb8-161">Mapping dei dati CAMT ai campi nella tabella Riconc. C/C bancari (273)</span><span class="sxs-lookup"><span data-stu-id="a8eb8-161">CAMT data mapping to fields in the Bank Acc. Reconciliation table (273)</span></span>  

|<span data-ttu-id="a8eb8-162">Percorso dell'articolo</span><span class="sxs-lookup"><span data-stu-id="a8eb8-162">Element Path</span></span>|<span data-ttu-id="a8eb8-163">Elemento messaggio</span><span class="sxs-lookup"><span data-stu-id="a8eb8-163">Message Element</span></span>|<span data-ttu-id="a8eb8-164">Tipo di dati</span><span class="sxs-lookup"><span data-stu-id="a8eb8-164">Data Type</span></span>|<span data-ttu-id="a8eb8-165">Descrizione</span><span class="sxs-lookup"><span data-stu-id="a8eb8-165">Description</span></span>|<span data-ttu-id="a8eb8-166">Identificatore segno negativo</span><span class="sxs-lookup"><span data-stu-id="a8eb8-166">Negative-Sign Identifier</span></span>|<span data-ttu-id="a8eb8-167">Nr. campo</span><span class="sxs-lookup"><span data-stu-id="a8eb8-167">Field No.</span></span>|<span data-ttu-id="a8eb8-168">Nome campo</span><span class="sxs-lookup"><span data-stu-id="a8eb8-168">Field Name</span></span>|  
|------------------|---------------------|---------------|-----------------|-------------------------------|---------------|----------------|  
|<span data-ttu-id="a8eb8-169">Stmt/CreDtTm</span><span class="sxs-lookup"><span data-stu-id="a8eb8-169">Stmt/CreDtTm</span></span>|<span data-ttu-id="a8eb8-170">CreationDateTime</span><span class="sxs-lookup"><span data-stu-id="a8eb8-170">CreationDateTime</span></span>|<span data-ttu-id="a8eb8-171">Data</span><span class="sxs-lookup"><span data-stu-id="a8eb8-171">Date</span></span>|<span data-ttu-id="a8eb8-172">Data e ora di creazione del messaggio</span><span class="sxs-lookup"><span data-stu-id="a8eb8-172">The date and time when the message was created</span></span>||<span data-ttu-id="a8eb8-173">3</span><span class="sxs-lookup"><span data-stu-id="a8eb8-173">3</span></span>|<span data-ttu-id="a8eb8-174">Data estratto conto</span><span class="sxs-lookup"><span data-stu-id="a8eb8-174">Statement Date</span></span>|  
|<span data-ttu-id="a8eb8-175">Stmt/Bal/Amt</span><span class="sxs-lookup"><span data-stu-id="a8eb8-175">Stmt/Bal/Amt</span></span>|<span data-ttu-id="a8eb8-176">Importo</span><span class="sxs-lookup"><span data-stu-id="a8eb8-176">Amount</span></span>|<span data-ttu-id="a8eb8-177">Decimale</span><span class="sxs-lookup"><span data-stu-id="a8eb8-177">Decimal</span></span>|<span data-ttu-id="a8eb8-178">Importo risultante dagli importi al netto per tutti i movimenti dare e avere</span><span class="sxs-lookup"><span data-stu-id="a8eb8-178">The amount resulting from the netted amounts for all debit and credit entries</span></span>||<span data-ttu-id="a8eb8-179">4</span><span class="sxs-lookup"><span data-stu-id="a8eb8-179">4</span></span>|<span data-ttu-id="a8eb8-180">Saldo finale estratto conto</span><span class="sxs-lookup"><span data-stu-id="a8eb8-180">Statement Ending Balance</span></span>|  

## <a name="camt-data-mapping-to-fields-in-the-bank-acc-reconciliation-line-table-274"></a><span data-ttu-id="a8eb8-181">Mapping dei dati CAMT ai campi nella tabella Righe riconc. C/C bancari (274)</span><span class="sxs-lookup"><span data-stu-id="a8eb8-181">CAMT data mapping to fields in the Bank Acc. Reconciliation Line table (274)</span></span>  

|<span data-ttu-id="a8eb8-182">Percorso dell'articolo</span><span class="sxs-lookup"><span data-stu-id="a8eb8-182">Element Path</span></span>|<span data-ttu-id="a8eb8-183">Elemento messaggio</span><span class="sxs-lookup"><span data-stu-id="a8eb8-183">Message Element</span></span>|<span data-ttu-id="a8eb8-184">Tipo di dati</span><span class="sxs-lookup"><span data-stu-id="a8eb8-184">Data Type</span></span>|<span data-ttu-id="a8eb8-185">Descrizione</span><span class="sxs-lookup"><span data-stu-id="a8eb8-185">Description</span></span>|<span data-ttu-id="a8eb8-186">Identificatore segno negativo</span><span class="sxs-lookup"><span data-stu-id="a8eb8-186">Negative-Sign Identifier</span></span>|<span data-ttu-id="a8eb8-187">Nr. campo</span><span class="sxs-lookup"><span data-stu-id="a8eb8-187">Field No.</span></span>|<span data-ttu-id="a8eb8-188">Nome campo</span><span class="sxs-lookup"><span data-stu-id="a8eb8-188">Field Name</span></span>|  
|------------------|---------------------|---------------|-----------------|-------------------------------|---------------|----------------|  
|<span data-ttu-id="a8eb8-189">Stmt/Ntry/Amt</span><span class="sxs-lookup"><span data-stu-id="a8eb8-189">Stmt/Ntry/Amt</span></span>|<span data-ttu-id="a8eb8-190">Importo</span><span class="sxs-lookup"><span data-stu-id="a8eb8-190">Amount</span></span>|<span data-ttu-id="a8eb8-191">Decimale</span><span class="sxs-lookup"><span data-stu-id="a8eb8-191">Decimal</span></span>|<span data-ttu-id="a8eb8-192">Specifica l'importo di denaro nel movimento cassa.</span><span class="sxs-lookup"><span data-stu-id="a8eb8-192">The amount of money in the cash entry</span></span>||<span data-ttu-id="a8eb8-193">7</span><span class="sxs-lookup"><span data-stu-id="a8eb8-193">7</span></span>|<span data-ttu-id="a8eb8-194">Importo estratto conto</span><span class="sxs-lookup"><span data-stu-id="a8eb8-194">Statement Amount</span></span>|  
|<span data-ttu-id="a8eb8-195">Stmt/Ntry/CdtDbtInd</span><span class="sxs-lookup"><span data-stu-id="a8eb8-195">Stmt/Ntry/CdtDbtInd</span></span>|<span data-ttu-id="a8eb8-196">CreditDebitIndicator</span><span class="sxs-lookup"><span data-stu-id="a8eb8-196">CreditDebitIndicator</span></span>|<span data-ttu-id="a8eb8-197">Testo</span><span class="sxs-lookup"><span data-stu-id="a8eb8-197">Text</span></span>|<span data-ttu-id="a8eb8-198">Indica se il movimento è un credito o un debito</span><span class="sxs-lookup"><span data-stu-id="a8eb8-198">Indicates whether the entry is a credit or a debit entry</span></span>|<span data-ttu-id="a8eb8-199">DBIT</span><span class="sxs-lookup"><span data-stu-id="a8eb8-199">DBIT</span></span>|<span data-ttu-id="a8eb8-200">7</span><span class="sxs-lookup"><span data-stu-id="a8eb8-200">7</span></span>|<span data-ttu-id="a8eb8-201">Importo estratto conto</span><span class="sxs-lookup"><span data-stu-id="a8eb8-201">Statement Amount</span></span>|  
|<span data-ttu-id="a8eb8-202">Stmt/Ntry/BookgDt/Dt</span><span class="sxs-lookup"><span data-stu-id="a8eb8-202">Stmt/Ntry/BookgDt/Dt</span></span>|<span data-ttu-id="a8eb8-203">Data</span><span class="sxs-lookup"><span data-stu-id="a8eb8-203">Date</span></span>|<span data-ttu-id="a8eb8-204">Data</span><span class="sxs-lookup"><span data-stu-id="a8eb8-204">Date</span></span>|<span data-ttu-id="a8eb8-205">Data in cui un movimento viene registrato in un conto nei registri di chi utilizza il conto</span><span class="sxs-lookup"><span data-stu-id="a8eb8-205">The date when an entry is posted to an account on the account servicer's books</span></span>||<span data-ttu-id="a8eb8-206">5</span><span class="sxs-lookup"><span data-stu-id="a8eb8-206">5</span></span>|<span data-ttu-id="a8eb8-207">Data transazione</span><span class="sxs-lookup"><span data-stu-id="a8eb8-207">Transaction Date</span></span>|  
|<span data-ttu-id="a8eb8-208">Stmt/Ntry/BookgDt/DtTm</span><span class="sxs-lookup"><span data-stu-id="a8eb8-208">Stmt/Ntry/BookgDt/DtTm</span></span>|<span data-ttu-id="a8eb8-209">DataOra</span><span class="sxs-lookup"><span data-stu-id="a8eb8-209">DateTime</span></span>|<span data-ttu-id="a8eb8-210">DataOra</span><span class="sxs-lookup"><span data-stu-id="a8eb8-210">DateTime</span></span>|<span data-ttu-id="a8eb8-211">Data e ora in cui un movimento viene registrato in un conto nei registri di chi utilizza il conto</span><span class="sxs-lookup"><span data-stu-id="a8eb8-211">The date and time when an entry is posted to an account on the account servicer's books</span></span>||<span data-ttu-id="a8eb8-212">5</span><span class="sxs-lookup"><span data-stu-id="a8eb8-212">5</span></span>|<span data-ttu-id="a8eb8-213">Data transazione</span><span class="sxs-lookup"><span data-stu-id="a8eb8-213">Transaction Date</span></span>|  
|<span data-ttu-id="a8eb8-214">Stmt/Ntry/ValDt/Dt</span><span class="sxs-lookup"><span data-stu-id="a8eb8-214">Stmt/Ntry/ValDt/Dt</span></span>|<span data-ttu-id="a8eb8-215">Data</span><span class="sxs-lookup"><span data-stu-id="a8eb8-215">Date</span></span>|<span data-ttu-id="a8eb8-216">Data</span><span class="sxs-lookup"><span data-stu-id="a8eb8-216">Date</span></span>|<span data-ttu-id="a8eb8-217">Data in cui i cespiti diventano disponibili al proprietario del conto nel caso di un movimento in avere o cessano di essere disponibili nel caso di un movimento in dare</span><span class="sxs-lookup"><span data-stu-id="a8eb8-217">The date when assets become available to the account owner in case of a credit entry, or cease to be available to the account owner in case of a debit entry</span></span>||<span data-ttu-id="a8eb8-218">12</span><span class="sxs-lookup"><span data-stu-id="a8eb8-218">12</span></span>|<span data-ttu-id="a8eb8-219">Data valuta</span><span class="sxs-lookup"><span data-stu-id="a8eb8-219">Value Date</span></span>|  
|<span data-ttu-id="a8eb8-220">Stmt/Ntry/ValDt/DtTm</span><span class="sxs-lookup"><span data-stu-id="a8eb8-220">Stmt/Ntry/ValDt/DtTm</span></span>|<span data-ttu-id="a8eb8-221">DataOra</span><span class="sxs-lookup"><span data-stu-id="a8eb8-221">DateTime</span></span>|<span data-ttu-id="a8eb8-222">DataOra</span><span class="sxs-lookup"><span data-stu-id="a8eb8-222">DateTime</span></span>|<span data-ttu-id="a8eb8-223">Data e ora in cui i cespiti diventano disponibili al proprietario del conto nel caso di un movimento in avere o cessano di essere disponibili nel caso di un movimento in dare</span><span class="sxs-lookup"><span data-stu-id="a8eb8-223">The date and time when assets become available to the account owner in case of a credit entry, or cease to be available to the account owner in case of a debit entry</span></span>||<span data-ttu-id="a8eb8-224">12</span><span class="sxs-lookup"><span data-stu-id="a8eb8-224">12</span></span>|<span data-ttu-id="a8eb8-225">Data valuta</span><span class="sxs-lookup"><span data-stu-id="a8eb8-225">Value Date</span></span>|  
|<span data-ttu-id="a8eb8-226">Stmt/Ntry/NtryDtls/TxDtls/RltdPties/Dbtr/Nm</span><span class="sxs-lookup"><span data-stu-id="a8eb8-226">Stmt/Ntry/NtryDtls/TxDtls/RltdPties/Dbtr/Nm</span></span>|<span data-ttu-id="a8eb8-227">Nome</span><span class="sxs-lookup"><span data-stu-id="a8eb8-227">Name</span></span>|<span data-ttu-id="a8eb8-228">Testo</span><span class="sxs-lookup"><span data-stu-id="a8eb8-228">Text</span></span>|<span data-ttu-id="a8eb8-229">Nome della parte che deve una somma di denaro al creditore (finale)</span><span class="sxs-lookup"><span data-stu-id="a8eb8-229">The name of the party that owes an amount of money to the (ultimate) creditor</span></span>||<span data-ttu-id="a8eb8-230">15</span><span class="sxs-lookup"><span data-stu-id="a8eb8-230">15</span></span>|<span data-ttu-id="a8eb8-231">Informazioni sul pagante</span><span class="sxs-lookup"><span data-stu-id="a8eb8-231">Payer Information</span></span>|  
|<span data-ttu-id="a8eb8-232">Stmt/Ntry/NtryDtls/TxDtls/RmtInf/Ustrd</span><span class="sxs-lookup"><span data-stu-id="a8eb8-232">Stmt/Ntry/NtryDtls/TxDtls/RmtInf/Ustrd</span></span>|<span data-ttu-id="a8eb8-233">Non strutturato</span><span class="sxs-lookup"><span data-stu-id="a8eb8-233">Unstructured</span></span>|<span data-ttu-id="a8eb8-234">Testo</span><span class="sxs-lookup"><span data-stu-id="a8eb8-234">Text</span></span>|<span data-ttu-id="a8eb8-235">Informazioni fornite per consentire la corrispondenza o riconciliazione di un movimento con gli articoli oggetto del pagamento, come le fatture aziendali in un sistema conto clienti, in un form non strutturato</span><span class="sxs-lookup"><span data-stu-id="a8eb8-235">Information supplied to enable the matching/reconciliation of an entry with the items that the payment is intended to settle, such as commercial invoices in an accounts-receivable system, in an unstructured form</span></span>||<span data-ttu-id="a8eb8-236">6</span><span class="sxs-lookup"><span data-stu-id="a8eb8-236">6</span></span>|<span data-ttu-id="a8eb8-237">Descrizione</span><span class="sxs-lookup"><span data-stu-id="a8eb8-237">Description</span></span>|  
|<span data-ttu-id="a8eb8-238">Stmt/Ntry/AddtlNtryInf</span><span class="sxs-lookup"><span data-stu-id="a8eb8-238">Stmt/Ntry/AddtlNtryInf</span></span>|<span data-ttu-id="a8eb8-239">AdditionalEntryInformation</span><span class="sxs-lookup"><span data-stu-id="a8eb8-239">AdditionalEntryInformation</span></span>|<span data-ttu-id="a8eb8-240">Testo</span><span class="sxs-lookup"><span data-stu-id="a8eb8-240">Text</span></span>|<span data-ttu-id="a8eb8-241">Informazioni aggiuntive relative al movimento</span><span class="sxs-lookup"><span data-stu-id="a8eb8-241">Additional information about the entry</span></span>||<span data-ttu-id="a8eb8-242">16</span><span class="sxs-lookup"><span data-stu-id="a8eb8-242">16</span></span>|<span data-ttu-id="a8eb8-243">Informazioni sulla transazione</span><span class="sxs-lookup"><span data-stu-id="a8eb8-243">Transaction Information</span></span>|  

 <span data-ttu-id="a8eb8-244">Gli elementi nel nodo **Ntry** importati in [!INCLUDE[d365fin](includes/d365fin_md.md)], ma di cui non è stato eseguito il mapping ad alcun campo, vengono memorizzati nella tabella **Registrazione definizione colonna scambio dati**.</span><span class="sxs-lookup"><span data-stu-id="a8eb8-244">Elements in the **Ntry** node that are imported into [!INCLUDE[d365fin](includes/d365fin_md.md)] but not mapped to any fields are stored in the **Posting Exch. Column Def** table.</span></span> <span data-ttu-id="a8eb8-245">Gli utenti possono vedere gli elementi nelle finestre **Registrazione riconciliazione pagamenti**, **Collegamento pagamenti** e **Riconciliazioni C/C bancari** scegliendo l'azione **Dettagli riga rendiconto bancario**.</span><span class="sxs-lookup"><span data-stu-id="a8eb8-245">Users can view these elements from the **Payment Reconciliation Journal**, **Payment Application**, and **Bank Acc. Reconciliation** windows by choosing the **Bank Statement Line Details** action.</span></span> <span data-ttu-id="a8eb8-246">Per ulteriori informazioni, vedere [Procedura: Riconciliare i pagamenti utilizzando il collegamento automatico](receivables-how-reconcile-payments-auto-application.md).</span><span class="sxs-lookup"><span data-stu-id="a8eb8-246">For more information, see [How to: Reconcile Payments Using Automatic Application](receivables-how-reconcile-payments-auto-application.md).</span></span>  
## <a name="see-also"></a><span data-ttu-id="a8eb8-247">Vedi anche</span><span class="sxs-lookup"><span data-stu-id="a8eb8-247">See Also</span></span>  
[<span data-ttu-id="a8eb8-248">Impostazione dello scambio di dati</span><span class="sxs-lookup"><span data-stu-id="a8eb8-248">Setting Up Data Exchange</span></span>](across-set-up-data-exchange.md)  
[<span data-ttu-id="a8eb8-249">Scambio di dati in modalità elettronica</span><span class="sxs-lookup"><span data-stu-id="a8eb8-249">Exchanging Data Electronically</span></span>](across-data-exchange.md)  
<span data-ttu-id="a8eb8-250">[Procedura: Impostare il servizio di conversione di dati bancari](bank-how-setup-bank-data-conversion-service.md) </span><span class="sxs-lookup"><span data-stu-id="a8eb8-250">[How to: Set Up the Bank Data Conversion Service](bank-how-setup-bank-data-conversion-service.md) </span></span>  
[<span data-ttu-id="a8eb8-251">Procedura: Utilizzare gli schemi XML per preparare le definizioni di scambio dati</span><span class="sxs-lookup"><span data-stu-id="a8eb8-251">How to: Use XML Schemas to Prepare Data Exchange Definitions</span></span>](across-how-to-use-xml-schemas-to-prepare-data-exchange-definitions.md)  
[<span data-ttu-id="a8eb8-252">Procedura: Riconciliare i pagamenti utilizzando il collegamento automatico</span><span class="sxs-lookup"><span data-stu-id="a8eb8-252">How to: Reconcile Payments Using Automatic Application</span></span>](receivables-how-reconcile-payments-auto-application.md)  
