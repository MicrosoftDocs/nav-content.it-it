---
title: 'Procedura: Aggiornare i dati delle transazioni IVA'
description: "Prima di creare il primo report transazioni IVA, è necessario preparare i dati esistenti eseguendo il report **Aggiorna data transazione IVA**. È inoltre necessario eseguire questo report se sono state apportate modifiche al setup in base ai nuovi requisiti delle autorità fiscali."
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
ms.openlocfilehash: a0b051adf9bc3eeb60db5fcd789b6c692b74565e
ms.contentlocale: it-it
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-update-vat-transactions-data"></a><span data-ttu-id="b88bf-104">Procedura: Aggiornare i dati delle transazioni IVA</span><span class="sxs-lookup"><span data-stu-id="b88bf-104">How to: Update VAT Transactions Data</span></span>
<span data-ttu-id="b88bf-105">Prima di creare il primo report transazioni IVA, è necessario preparare i dati esistenti eseguendo il report **Aggiorna data transazione IVA**.</span><span class="sxs-lookup"><span data-stu-id="b88bf-105">Before you create the first VAT transaction report, you should prepare the existing data by running the **Update VAT Transaction Data** report.</span></span> <span data-ttu-id="b88bf-106">È inoltre necessario eseguire questo report se sono state apportate modifiche al setup in base ai nuovi requisiti delle autorità fiscali.</span><span class="sxs-lookup"><span data-stu-id="b88bf-106">You should also run this report if you have made changes to the setup based on new requirements from the tax authorities.</span></span>  

 <span data-ttu-id="b88bf-107">È possibile eseguire il report **Aggiorna data transazione IVA** come test prima di modificare i dati.</span><span class="sxs-lookup"><span data-stu-id="b88bf-107">You can run the **Update VAT Transaction Data** report as a test before you change any data.</span></span> <span data-ttu-id="b88bf-108">Dopo avere verificato che i filtri soddisfano le previsioni e le richieste delle autorità fiscali, eseguire nuovamente il report per apportare le modifiche appropriate ai dati.</span><span class="sxs-lookup"><span data-stu-id="b88bf-108">When you have verified that the filters meet your expectations and the requirements of the tax authorities, you should run the report again to make the appropriate changes to data.</span></span>  

> [!CAUTION]  
>  <span data-ttu-id="b88bf-109">Prima di eseguire il report **Aggiorna data transazione IVA**, è necessario attivare il log delle modifiche nella finestra **Setup log modifiche**.</span><span class="sxs-lookup"><span data-stu-id="b88bf-109">Before you run the **Update VAT Transaction Data** report, you should activate the change log in the **Change Log Setup** window.</span></span> <span data-ttu-id="b88bf-110">Inoltre, è necessario attivare la registrazione delle modifiche nel campo **Includi in report transazioni IVA** nella tabella **Movimenti IVA**.</span><span class="sxs-lookup"><span data-stu-id="b88bf-110">Also, you should enable logging for modifications to the **Include in VAT Transac. Report** field on the **VAT Entry** table.</span></span>  

### <a name="to-update-vat-transaction-data"></a><span data-ttu-id="b88bf-111">Per aggiornare i dati delle transazioni IVA</span><span class="sxs-lookup"><span data-stu-id="b88bf-111">To update VAT transaction data</span></span>  

1.  <span data-ttu-id="b88bf-112">Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **Aggiorna data transazione IVA**, quindi scegliere il collegamento correlato.</span><span class="sxs-lookup"><span data-stu-id="b88bf-112">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Update VAT Transaction Data**, and then choose the related link.</span></span>  

2.  <span data-ttu-id="b88bf-113">Facoltativamente, nella Scheda dettaglio **Movimenti IVA** impostare i filtri appropriati.</span><span class="sxs-lookup"><span data-stu-id="b88bf-113">Optionally, on the **VAT Entry** FastTab, set the appropriate filters.</span></span>  

3.  <span data-ttu-id="b88bf-114">Nella Scheda dettaglio **Opzioni** compilare i campi come descritto nella tabella riportata di seguito.</span><span class="sxs-lookup"><span data-stu-id="b88bf-114">On the **Options** FastTab, fill in the fields as described in the following table.</span></span>  

    |<span data-ttu-id="b88bf-115">Campo</span><span class="sxs-lookup"><span data-stu-id="b88bf-115">Field</span></span>|<span data-ttu-id="b88bf-116">Description</span><span class="sxs-lookup"><span data-stu-id="b88bf-116">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="b88bf-117">**Confronta con soglia**</span><span class="sxs-lookup"><span data-stu-id="b88bf-117">**Compare against Threshold**</span></span>|<span data-ttu-id="b88bf-118">Selezionare per confrontare i movimenti IVA rispetto agli importi di soglia specificati nel setup registrazioni IVA.</span><span class="sxs-lookup"><span data-stu-id="b88bf-118">Select to compare VAT entries against the threshold amounts that are specified in the VAT posting setup.</span></span>|  
    |<span data-ttu-id="b88bf-119">**Mostra solo elenco**</span><span class="sxs-lookup"><span data-stu-id="b88bf-119">**Show List Only**</span></span>|<span data-ttu-id="b88bf-120">Selezionare se non si desidera aggiornare i dati.</span><span class="sxs-lookup"><span data-stu-id="b88bf-120">Select if you do not want to update data.</span></span><br /><br /> <span data-ttu-id="b88bf-121">Se si seleziona questo campo, [!INCLUDE[navnow](../../includes/navnow_md.md)] stampa un report in modo da poter verificare le modifiche prima che i dati vengano modificati.</span><span class="sxs-lookup"><span data-stu-id="b88bf-121">If you select this field, [!INCLUDE[navnow](../../includes/navnow_md.md)] prints a report so that you can verify the changes before data is modified.</span></span> <span data-ttu-id="b88bf-122">Il report contiene una riga per ogni documento in cui l'imponibile IVA sia uguale o maggiore degli importi di soglia.</span><span class="sxs-lookup"><span data-stu-id="b88bf-122">The report contains a line for each document where the VAT base is equal to or greater than the threshold amounts.</span></span> <span data-ttu-id="b88bf-123">**Avviso:** Non selezionare questo campo e il campo **Imposta Includi in report transazioni IVA**.</span><span class="sxs-lookup"><span data-stu-id="b88bf-123">**Warning:**  Do not select both this field and the **Set Include in VAT Transaction Report** field.</span></span>|  
    |<span data-ttu-id="b88bf-124">**Imposta Includi in report transazioni IVA**</span><span class="sxs-lookup"><span data-stu-id="b88bf-124">**Set Include in VAT Transaction Report**</span></span>|<span data-ttu-id="b88bf-125">Selezionare per impostare **Imposta Includi in report transazioni IVA** su **Sì** in tutti i movimenti IVA in cui gli importi soddisfano gli importi di soglia specificati nel setup registrazioni IVA.</span><span class="sxs-lookup"><span data-stu-id="b88bf-125">Select to set the **Include in VAT Trans. Report** to **Yes** on all VAT entries where the amounts meet the threshold amounts that are specified in the VAT posting setup.</span></span> <span data-ttu-id="b88bf-126">**Avviso:** Se si seleziona questo campo, i dati vengono aggiornati.</span><span class="sxs-lookup"><span data-stu-id="b88bf-126">**Warning:**  If you select this field, your data is updated.</span></span> <span data-ttu-id="b88bf-127">È consigliabile eseguire il report come test prima di eseguirlo per modificare i dati.</span><span class="sxs-lookup"><span data-stu-id="b88bf-127">You should run the report as a test before you run it to change data.</span></span>|  

4.  <span data-ttu-id="b88bf-128">Scegliere il pulsante **Stampa** per aggiornare i dati delle transazioni IVA oppure scegliere il pulsante **Anteprima** per visualizzare le modifiche.</span><span class="sxs-lookup"><span data-stu-id="b88bf-128">Choose the **Print** button to update VAT transaction data, or choose the **Preview** button to view the changes.</span></span>  

 <span data-ttu-id="b88bf-129">Quando si esegue il report, [!INCLUDE[navnow](../../includes/navnow_md.md)] elabora i movimenti IVA in base ai filtri impostati.</span><span class="sxs-lookup"><span data-stu-id="b88bf-129">When you run the report, [!INCLUDE[navnow](../../includes/navnow_md.md)] processes VAT entries based on the filters that you set.</span></span> <span data-ttu-id="b88bf-130">Le seguenti regole sono applicabili:</span><span class="sxs-lookup"><span data-stu-id="b88bf-130">The following rules are also applied:</span></span>  

-   <span data-ttu-id="b88bf-131">Il campo **In blacklist** per il movimento IVA deve essere vuoto.</span><span class="sxs-lookup"><span data-stu-id="b88bf-131">The **Blacklisted** field for the VAT entry must be blank.</span></span>  

-   <span data-ttu-id="b88bf-132">Il campo **Tipo** del movimento IVA non deve essere **Liquidazione**.</span><span class="sxs-lookup"><span data-stu-id="b88bf-132">The **Type** field for the VAT entry must not be **Settlement**.</span></span>  

## <a name="see-also"></a><span data-ttu-id="b88bf-133">Vedi anche</span><span class="sxs-lookup"><span data-stu-id="b88bf-133">See Also</span></span>  
 <span data-ttu-id="b88bf-134">[Procedura: Preparare i report di transazioni IVA](how-to-prepare-for-vat-transactions-reports.md) </span><span class="sxs-lookup"><span data-stu-id="b88bf-134">[How to: Prepare for VAT Transactions Reports](how-to-prepare-for-vat-transactions-reports.md) </span></span>  
 [<span data-ttu-id="b88bf-135">IVA italiana</span><span class="sxs-lookup"><span data-stu-id="b88bf-135">Italian VAT</span></span>](italian-vat.md)   
 

