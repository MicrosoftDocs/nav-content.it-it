---
title: Impostare prezzi e costi per servizi assistenza
description: Informazioni su come impostare prezzi e costi aggiuntivi per i servizi assistenza.
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: service, cost, service order
ms.date: 08/22/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 014445360336ac00e00e5569a48e4866fc843afb
ms.contentlocale: it-it
ms.lasthandoff: 10/16/2017

---

# <a name="how-to-set-up-pricing-and-additional-costs-for-services"></a><span data-ttu-id="c74d1-103">Procedura: Impostare prezzi e costi aggiuntivi per i servizi assistenza</span><span class="sxs-lookup"><span data-stu-id="c74d1-103">How to: Set Up Pricing and Additional Costs for Services</span></span>
<span data-ttu-id="c74d1-104">È possibile utilizzare le funzionalità di definizione dei prezzi di [!INCLUDE[d365fin](includes/d365fin_md.md)] per impostare e personalizzare l'applicazione in modo da poter applicare e rettificare i prezzi per articoli in assistenza, riparazioni e ordini.</span><span class="sxs-lookup"><span data-stu-id="c74d1-104">You can use the [!INCLUDE[d365fin](includes/d365fin_md.md)] pricing features to set up and customize your application so that you apply and adjust pricing on service items, repairs, and orders.</span></span> <span data-ttu-id="c74d1-105">Queste decisioni relative ai prezzi potranno essere in seguito agevolmente trasmesse al processo di fatturazione.</span><span class="sxs-lookup"><span data-stu-id="c74d1-105">These pricing decisions are then easily transmitted to the invoicing process.</span></span>  
  
<span data-ttu-id="c74d1-106">Come previsto dall'implementazione, si possono impostare gruppi di prezzi associandoli a specifici periodi di tempo, clienti o valute.</span><span class="sxs-lookup"><span data-stu-id="c74d1-106">As your implementation requires, you can set up pricing groups and map them to specific time periods, customers, or currency.</span></span> <span data-ttu-id="c74d1-107">È anche possibile impostare prezzi fissi, minimi o massimi, a seconda dei contratti di assistenza in atto con i vari clienti.</span><span class="sxs-lookup"><span data-stu-id="c74d1-107">You can set up fixed, minimum, or maximum pricing, depending on the service contracts that you have with customers.</span></span> <span data-ttu-id="c74d1-108">Infine, in fase di rettifica dei prezzi, è possibile visualizzare e approvare le modifiche prima di applicarle alla contabilità.</span><span class="sxs-lookup"><span data-stu-id="c74d1-108">Finally, as you adjust your prices, you can view and approve the changes before committing them to the ledger.</span></span>  

## <a name="to-set-up-a-service-price-group"></a><span data-ttu-id="c74d1-109">Per impostare un gruppo di prezzi in assistenza</span><span class="sxs-lookup"><span data-stu-id="c74d1-109">To set up a service price group</span></span>
<span data-ttu-id="c74d1-110">È possibile impostare gruppi contenenti articoli in assistenza a cui si desidera vengano applicate le stesse definizioni speciali del prezzo di assistenza.</span><span class="sxs-lookup"><span data-stu-id="c74d1-110">You can set up groups containing service items that you want to receive the same special service pricing.</span></span> <span data-ttu-id="c74d1-111">I gruppi dei prezzi di assistenza vengono assegnati ad articoli in assistenza nelle righe di articoli in assistenza.</span><span class="sxs-lookup"><span data-stu-id="c74d1-111">You assign service price groups to service items on service item lines.</span></span> <span data-ttu-id="c74d1-112">È inoltre possibile assegnare gruppi di prezzi di assistenza ai gruppi di articoli in assistenza.</span><span class="sxs-lookup"><span data-stu-id="c74d1-112">You can also assign service price groups to service item groups.</span></span>  

1. <span data-ttu-id="c74d1-113">Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **Gruppi prezzo assistenza**, quindi scegliere il collegamento correlato.</span><span class="sxs-lookup"><span data-stu-id="c74d1-113">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Service Price Groups**, and then choose the related link.</span></span>  
2. <span data-ttu-id="c74d1-114">Creare un nuovo gruppo di prezzi di assistenza.</span><span class="sxs-lookup"><span data-stu-id="c74d1-114">Create a new service price group.</span></span>  
3. <span data-ttu-id="c74d1-115">Compilare i campi **Codice** e **Descrizione**.</span><span class="sxs-lookup"><span data-stu-id="c74d1-115">Fill in the **Code** and **Description** fields.</span></span>  
4. <span data-ttu-id="c74d1-116">Scegliere l'azione **Setup**.</span><span class="sxs-lookup"><span data-stu-id="c74d1-116">Choose the **Setup** action.</span></span>  
2. <span data-ttu-id="c74d1-117">Compilare i campi come necessario.</span><span class="sxs-lookup"><span data-stu-id="c74d1-117">Fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  

 > [!Tip]
 > <span data-ttu-id="c74d1-118">Con i campi **Tipo rettifica** e **Importo**, è possibile specificare se una rettifica riguarderà un importo fisso oppure verrà applicata esclusivamente ai prezzi totali di assistenza che supereranno o saranno inferiori all'importo specificato nel campo **Importo**.</span><span class="sxs-lookup"><span data-stu-id="c74d1-118">The **Adjustment Type** and **Amount** fields work together to specify whether an adjustment concerns a fixed amount, or applies only when the total service price exceeds or is lower than the amount in the **Amount** field.</span></span>  

## <a name="to-set-up-a-service-price-adjustment-group"></a><span data-ttu-id="c74d1-119">Per impostare un gruppo di rettifica dei prezzi di assistenza</span><span class="sxs-lookup"><span data-stu-id="c74d1-119">To set up a service price adjustment group</span></span>  
<span data-ttu-id="c74d1-120">È possibile impostare i gruppi di rettifica del prezzo per rettificare il prezzo di assistenza degli articoli in assistenza.</span><span class="sxs-lookup"><span data-stu-id="c74d1-120">You can set up price adjustment groups to adjust service pricing of service items.</span></span> <span data-ttu-id="c74d1-121">Ad esempio, è possibile impostare gruppi di rettifica del prezzo per modificare il costo di spedizione o dei pezzi di ricambio.</span><span class="sxs-lookup"><span data-stu-id="c74d1-121">For example, you can set up price adjustment groups that adjust price of freight or spare parts.</span></span>  
  
1. <span data-ttu-id="c74d1-122">Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **Gruppi rettifica prezzo assistenza**, quindi scegliere il collegamento correlato.</span><span class="sxs-lookup"><span data-stu-id="c74d1-122">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Service Price Adjustment Groups**, and then choose the related link.</span></span>  
2. <span data-ttu-id="c74d1-123">Creare un nuovo gruppo di rettifica dei prezzi di assistenza.</span><span class="sxs-lookup"><span data-stu-id="c74d1-123">Create a new service price adjustment group.</span></span>  
3. <span data-ttu-id="c74d1-124">Compilare i campi **Codice** e **Descrizione**.</span><span class="sxs-lookup"><span data-stu-id="c74d1-124">Fill in the **Code** and **Description** fields.</span></span>  
4. <span data-ttu-id="c74d1-125">Nel campo **Tipo** immettere il tipo del movimento da rettificare.</span><span class="sxs-lookup"><span data-stu-id="c74d1-125">In the **Type** field, enter the type of the entry that you want to adjust.</span></span>  
  
    * <span data-ttu-id="c74d1-126">Per rettificare un solo movimento specifico, immettere il numero di tale movimento nel campo **Nr.**</span><span class="sxs-lookup"><span data-stu-id="c74d1-126">To adjust only one specific entry, enter the number of this entry in the **No.**</span></span> <span data-ttu-id="c74d1-127"> </span><span class="sxs-lookup"><span data-stu-id="c74d1-127">field.</span></span> <span data-ttu-id="c74d1-128">Se questo campo viene lasciato vuoto, il gruppo di rettifica andrà a rettificare tutti i movimenti del tipo definito nel campo **Tipo**.</span><span class="sxs-lookup"><span data-stu-id="c74d1-128">When you leave this field blank, your adjustment group will adjust all entries of the type defined in the **Type** field.</span></span>  
    * <span data-ttu-id="c74d1-129">Per rettificare i prezzi di assistenza in base a un determinato servizio di assistenza, compilare il campo **Tipo di lavoro**.</span><span class="sxs-lookup"><span data-stu-id="c74d1-129">To adjust service prices related to only one specific service, fill in the **Work Type** field.</span></span> <span data-ttu-id="c74d1-130">Se questo campo viene lasciato vuoto, l'impostazione verrà ignorata.</span><span class="sxs-lookup"><span data-stu-id="c74d1-130">When you leave this field blank, it will just be ignored.</span></span>  
  
5. <span data-ttu-id="c74d1-131">Nel campo **Descrizione** immettere una breve descrizione della rettifica dei prezzi di assistenza.</span><span class="sxs-lookup"><span data-stu-id="c74d1-131">In the **Description** field, enter a short description of the service price adjustment.</span></span>  
6. <span data-ttu-id="c74d1-132">Per rettificare i prezzi di assistenza relativi a una determinata categoria di registrazione articoli/servizi, compilare il campo **Cat. reg. articolo/servizio**.</span><span class="sxs-lookup"><span data-stu-id="c74d1-132">To adjust service prices related to only one specific general product posting group, fill in the **Gen. Prod. Posting Group** field.</span></span>

> [!Tip]
> <span data-ttu-id="c74d1-133">È possibile scegliere **Dettagli** per aggiungere altre informazioni relative al gruppo di rettifica.</span><span class="sxs-lookup"><span data-stu-id="c74d1-133">You can choose **Details** to add additional information about the adjustment group.</span></span> <span data-ttu-id="c74d1-134">Ad esempio, specificare quale articolo appartiene al gruppo di rettifica dei prezzi di assistenza e se si tratta di un articolo, una risorsa, un gruppo di risorse o un addebito di assistenza.</span><span class="sxs-lookup"><span data-stu-id="c74d1-134">For example, you can specify which item belongs to the service price adjustment group, and whether this is an item, a resource, a resource group, or a service charge.</span></span>  

## <a name="to-set-up-additional-costs-for-services"></a><span data-ttu-id="c74d1-135">Per impostare costi aggiuntivi per i servizi assistenza</span><span class="sxs-lookup"><span data-stu-id="c74d1-135">To set up additional costs for services</span></span>
<span data-ttu-id="c74d1-136">Quando si utilizzano articoli in assistenza e ordini di assistenza, potrebbe essere necessario registrare costi aggiuntivi, quali le spese di viaggio in determinate zone di assistenza o le spese iniziali.</span><span class="sxs-lookup"><span data-stu-id="c74d1-136">When you work with service items and service orders, you may need to register additional costs, such as travel costs to particular service zones or starting fees.</span></span> <span data-ttu-id="c74d1-137">Quando si crea un ordine di assistenza, è possibile inserire tali costi e verrà aggiunta una riga con il tipo **Costo**.</span><span class="sxs-lookup"><span data-stu-id="c74d1-137">When you create a service order, you can insert these costs and a line with the type **Cost** will be added to the order.</span></span> <span data-ttu-id="c74d1-138">In alternativa, se si desidera applicare il costo a tutti gli ordini di assistenza, è possibile impostare un costo di default.</span><span class="sxs-lookup"><span data-stu-id="c74d1-138">Alternatively, if you want to apply the cost to all service orders, you can set up a default cost.</span></span> <span data-ttu-id="c74d1-139">Ad esempio, se si desidera applicare sempre una spesa iniziale.</span><span class="sxs-lookup"><span data-stu-id="c74d1-139">For example, if you always want to apply a starting fee.</span></span>
  
### <a name="to-set-up-service-costs"></a><span data-ttu-id="c74d1-140">Per impostare i costi di assistenza</span><span class="sxs-lookup"><span data-stu-id="c74d1-140">To set up service costs</span></span>
1. <span data-ttu-id="c74d1-141">Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **Costi assistenza**, quindi scegliere il collegamento correlato.</span><span class="sxs-lookup"><span data-stu-id="c74d1-141">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Service Costs**, and then choose the related link.</span></span> 
2. <span data-ttu-id="c74d1-142">Compilare i campi in base alle esigenze.</span><span class="sxs-lookup"><span data-stu-id="c74d1-142">Fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  

### <a name="to-specify-a-default-cost-for-service-orders"></a><span data-ttu-id="c74d1-143">Per specificare un costo di default per gli ordini di assistenza</span><span class="sxs-lookup"><span data-stu-id="c74d1-143">To specify a default cost for service orders</span></span>
1. <span data-ttu-id="c74d1-144">Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **Setup assistenza**, quindi scegliere il collegamento correlato.</span><span class="sxs-lookup"><span data-stu-id="c74d1-144">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Service Setup**, and then choose the related link.</span></span> 
2. <span data-ttu-id="c74d1-145">Nel campo **Tariffa iniziale ordine assistenza** selezionare il costo di assistenza appropriato.</span><span class="sxs-lookup"><span data-stu-id="c74d1-145">In the **Service Order Starting Fee** field, choose the appropriate service cost.</span></span>

## <a name="see-also"></a><span data-ttu-id="c74d1-146">Vedi anche</span><span class="sxs-lookup"><span data-stu-id="c74d1-146">See Also</span></span>
[<span data-ttu-id="c74d1-147">Impostazione della gestione assistenza</span><span class="sxs-lookup"><span data-stu-id="c74d1-147">Setting Up Service Management</span></span>](service-setup-service.md)  
[<span data-ttu-id="c74d1-148">Gestione assistenza</span><span class="sxs-lookup"><span data-stu-id="c74d1-148">Service Management</span></span>](service-service.md)  
