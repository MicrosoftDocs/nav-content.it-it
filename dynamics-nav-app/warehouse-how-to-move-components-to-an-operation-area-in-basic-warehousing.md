---
title: Come spostare componenti in un'area di operazione nelle configurazioni della warehouse di base
description: Se le operazioni di elaborazione dell'articolo si verificano nell'ubicazione della warehouse, potrebbe essere necessario spostare gli articoli tra le collocazioni interne in modo che corrispondano ai documenti di origine interni, ad esempio produzione, assemblaggio o ordini di assistenza per l'ubicazione.
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/16/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: c1ee0394b835827eee3394a4bea3171d9294208c
ms.contentlocale: it-it
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-move-components-to-an-operation-area-in-basic-warehouse-configurations"></a><span data-ttu-id="32148-103">Procedura: Spostare componenti in un'area di operazione nelle configurazioni della warehouse di base</span><span class="sxs-lookup"><span data-stu-id="32148-103">How to: Move Components to an Operation Area in Basic Warehouse Configurations</span></span>
<span data-ttu-id="32148-104">Se le operazioni di elaborazione dell'articolo si verificano nell'ubicazione della warehouse, potrebbe essere necessario spostare gli articoli tra le collocazioni interne in modo che corrispondano ai documenti di origine interni, ad esempio produzione, assemblaggio o ordini di assistenza per l'ubicazione.</span><span class="sxs-lookup"><span data-stu-id="32148-104">If item processing operations occur at your warehouse location, then you may have to move items between internal bins to respond to internal source documents, such as production, assembly, or service orders at the location.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="32148-105">Per informazioni sullo spostamento di articoli tra collocazioni senza documenti di origine, vedere Movimentazione interna.</span><span class="sxs-lookup"><span data-stu-id="32148-105">For information about moving items between bins without source documents, see Internal Movement.</span></span>  

<span data-ttu-id="32148-106">Nelle configurazioni warehouse avanzate, ovvero ubicazioni che utilizzano il campo di setup **Stoccaggi e prelievi guidati**, è possibile utilizzare la finestra **Prospetto movimentazioni** per spostare gli articoli tra le collocazioni. Per ulteriori informazioni, vedere [Procedura: Spostare articoli nelle configurazioni della warehouse di base](warehouse-how-to-move-items-in-advanced-warehousing.md).</span><span class="sxs-lookup"><span data-stu-id="32148-106">In advanced warehouse configurations, which are locations that use the **Directed Put-away and Pick** setup field, you can use the **Movement Worksheet** window to move items between bins. For more information, see [How to: Move Items in Advanced warehouse Configurations](warehouse-how-to-move-items-in-advanced-warehousing.md).</span></span>  

<span data-ttu-id="32148-107">Nelle configurazioni di warehouse di base, ovvero ubicazioni che utilizzano il campo di setup **Collocazione obbligatoria** e il campo di setup **Richiesto prelievo**, è possibile registrare le movimentazioni di articoli nelle aree delle operazioni interne in base ai documenti di origine interni nei seguenti modi:</span><span class="sxs-lookup"><span data-stu-id="32148-107">In basic warehouse configurations, which are locations that use the **Bin Mandatory** setup field and the **Require Pick** setup field, you can register movement of items to internal operation areas based on internal source documents in the following ways:</span></span>  

-   <span data-ttu-id="32148-108">Tramite la finestra **Movimento di magazzino**.</span><span class="sxs-lookup"><span data-stu-id="32148-108">With the **Inventory Movement** window.</span></span>  
-   <span data-ttu-id="32148-109">Con la finestra **Prelievi magazzino**.</span><span class="sxs-lookup"><span data-stu-id="32148-109">With the **Inventory Pick** window.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="32148-110">I prelievi magazzino registrano inoltre i movimenti contabili articoli negativi come consumo e sono supportati solo per i componenti di produzione.</span><span class="sxs-lookup"><span data-stu-id="32148-110">Inventory picks also post negative item ledger entries as consumption and are only supported for production components.</span></span> <span data-ttu-id="32148-111">Per ulteriori informazioni, vedere la finestra Prelievo magazzino.</span><span class="sxs-lookup"><span data-stu-id="32148-111">For more information, see the Inventory Pick window.</span></span>  

<span data-ttu-id="32148-112">Per informazioni dettagliate sui movimenti di magazzino, vedere la finestra Movimento di magazzino.</span><span class="sxs-lookup"><span data-stu-id="32148-112">For detailed information about inventory movements, see the Inventory Movement window.</span></span>  

<span data-ttu-id="32148-113">Due diversi ruoli possono creare il movimento di magazzino iniziale.</span><span class="sxs-lookup"><span data-stu-id="32148-113">Two different roles can create the initial inventory movement.</span></span> <span data-ttu-id="32148-114">Un addetto all'assemblaggio, ad esempio, può crearlo da un ordine di assemblaggio rilasciato in modo che venga visualizzato nell'elenco dell'addetto warehouse relativo al lavoro da svolgere.</span><span class="sxs-lookup"><span data-stu-id="32148-114">An assembly worker, for example, can create it from a released assembly order so that it shows up in the warehouse worker’s list of work to do.</span></span> <span data-ttu-id="32148-115">Per creare un movimento di magazzino per le righe ordini di assemblaggio i cui componenti sono pronti per essere spostati nelle relative collocazioni specificate, l'addetto all'assemblaggio utilizza la funzione **Crea movimento di magazzino**.</span><span class="sxs-lookup"><span data-stu-id="32148-115">To create an inventory movement for assembly order lines that are ready to have components moved to their specified bins, the assembly worker uses the **Create Inventory Movement** function.</span></span>  

<span data-ttu-id="32148-116">In alternativa, un lavoratore warehouse può crearlo scegliendo l'ordine di assemblaggio rilasciato in questione.</span><span class="sxs-lookup"><span data-stu-id="32148-116">Alternatively, a warehouse worker can create it by pointing to the released assembly order in question.</span></span> <span data-ttu-id="32148-117">Questa funzionalità è descritta nella procedura seguente.</span><span class="sxs-lookup"><span data-stu-id="32148-117">This is described in the following procedure.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="32148-118">Se la movimentazione riguarda un ordine di assemblaggio in cui l'articolo è assemblato in base a un ordine di vendita, è possibile definire che il documento di movimento di magazzino viene creato automaticamente quando si crea il documento di prelievo magazzino che accetta l'articolo di assemblaggio completato e registra la spedizione.</span><span class="sxs-lookup"><span data-stu-id="32148-118">If the movement is for an assembly order where the item is assembled to a sales order, then you can define that the inventory movement document is automatically created when you create the inventory pick document that takes the finished assembly item and posts the shipment.</span></span> <span data-ttu-id="32148-119">Per impostare questa operazione, selezionare il campo **Crea movimenti automaticamente** nella finestra **Setup assemblaggio**.</span><span class="sxs-lookup"><span data-stu-id="32148-119">To set this up, select the **Create Movements Automatically** field in the **Assembly Setup** window</span></span>  
>   
>  <span data-ttu-id="32148-120">Per ulteriori informazioni sugli ordini di assemblaggio e nelle configurazioni di base della warehouse, vedere la sezione "Gestione di articoli da assemblare su ordine con prelievi magazzino" in [Procedura: Prelevare per la produzione o l'assemblaggio](warehouse-how-to-pick-for-production.md).</span><span class="sxs-lookup"><span data-stu-id="32148-120">For more information about assembly orders and basic warehouse configurations, see the "Handling Assemble-to-Order Items with Inventory Picks" section in [How to: Pick for Production or Assembly](warehouse-how-to-pick-for-production.md).</span></span>  

<span data-ttu-id="32148-121">La procedura seguente mostra come creare un movimento di magazzino nella finestra **Movimento di magazzino** facendo riferimento a un ordine di assemblaggio rilasciato come documento di origine.</span><span class="sxs-lookup"><span data-stu-id="32148-121">This procedure shows how to create an inventory movement from the **Inventory Movement** window by referencing a released assembly order as a source document.</span></span> <span data-ttu-id="32148-122">La procedura è la stessa quando si spostano componenti per gli ordini di produzione e gli ordini di assistenza.</span><span class="sxs-lookup"><span data-stu-id="32148-122">The procedure is the same when you move components for production orders and service orders.</span></span>  

## <a name="to-move-components-to-an-operation-area-in-basic-warehouse-configurations"></a><span data-ttu-id="32148-123">Per spostare componenti in un'area di operazione nelle configurazioni di warehouse di base</span><span class="sxs-lookup"><span data-stu-id="32148-123">To move components to an operation area in basic warehouse configurations</span></span>  
1.  <span data-ttu-id="32148-124">Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "Cerca pagina o report"), immettere **Movimento di magazzino**, quindi scegliere il collegamento pertinente.</span><span class="sxs-lookup"><span data-stu-id="32148-124">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Inventory Movement**, and choose the relevant link.</span></span>  
2.  <span data-ttu-id="32148-125">Nella Scheda dettaglio **Generale** compilare il campo **Nr.**</span><span class="sxs-lookup"><span data-stu-id="32148-125">On the **General** FastTab, fill in the **No.**</span></span> <span data-ttu-id="32148-126">.</span><span class="sxs-lookup"><span data-stu-id="32148-126">field.</span></span> <span data-ttu-id="32148-127">È possibile premere INVIO per selezionare la numerazione.</span><span class="sxs-lookup"><span data-stu-id="32148-127">You can press the Enter key  to select from the number series.</span></span>  
3.  <span data-ttu-id="32148-128">Nel campo **Cod. ubicazione** immettere l'ubicazione in cui si verifica la movimentazione.</span><span class="sxs-lookup"><span data-stu-id="32148-128">In the **Location Code** field, enter the location where the movement occurs.</span></span>  
4.  <span data-ttu-id="32148-129">Scegliere l'azione **Prendi documenti origine**.</span><span class="sxs-lookup"><span data-stu-id="32148-129">Choose the **Get Source Documents** action.</span></span> <span data-ttu-id="32148-130">In alternativa, compilare il campo **Documento origine**, quindi fare clic sul pulsante **AssistEdit** nel campo **Nr. origine**.</span><span class="sxs-lookup"><span data-stu-id="32148-130">Alternatively, fill in the **Source Document** field, and then choose the **AssistEdit** button in the **Source No.** field.</span></span>  
5.  <span data-ttu-id="32148-131">Nella finestra **Documenti origine** selezionare l'ordine di assemblaggio per cui si desidera spostare i componenti, quindi fare clic sul pulsante **OK**.</span><span class="sxs-lookup"><span data-stu-id="32148-131">In the **Source Documents** window, select the assembly order that you want to move components for, and then choose the **OK** button.</span></span>  

    <span data-ttu-id="32148-132">Per ogni componente necessario che può essere spostato, viene generata una riga Prendere e una riga Mettere nella finestra **Movimenti di magazzino**.</span><span class="sxs-lookup"><span data-stu-id="32148-132">For each needed component that can be moved, one Take line and one Place line are generated in the **Inventory Movements** window.</span></span> <span data-ttu-id="32148-133">Tutti i campi tranne il campo **Qtà da gestire** sono precompilati in base alle righe del documento di origine.</span><span class="sxs-lookup"><span data-stu-id="32148-133">All fields except the **Qty. to Handle** field are prefilled according to the source document lines.</span></span> <span data-ttu-id="32148-134">Il campo **Qtà da gestire** è uguale a zero fino a quando non si immette la quantità effettivamente spostata.</span><span class="sxs-lookup"><span data-stu-id="32148-134">The **Qty. to Handle** field is set to zero until you enter the quantity that you have actually moved.</span></span>  

    <span data-ttu-id="32148-135">È possibile modificare il codice collocazione in una riga Prendere, ma solo in base alla disponibilità.</span><span class="sxs-lookup"><span data-stu-id="32148-135">You can change the bin code on a Take line but only according to availability.</span></span> <span data-ttu-id="32148-136">Scegliendo il pulsante **AssistEdit** nel campo **Cod. collocazione** in una riga Prendere, la finestra **Contenuto collocazioni** viene aperta e mostra solo le collocazioni in cui il componente è disponibile.</span><span class="sxs-lookup"><span data-stu-id="32148-136">If you choose the **AssistEdit** button in the **Bin Code** field on a Take line, then the **Bin Contents** window opens and only shows bins where the component is available.</span></span>  

    <span data-ttu-id="32148-137">Non è possibile modificare il codice collocazione in una riga Mettere.</span><span class="sxs-lookup"><span data-stu-id="32148-137">You cannot change the bin code on a Place line.</span></span> <span data-ttu-id="32148-138">Solo il codice collocazione definito nella riga componente del documento di origine viene accettato.</span><span class="sxs-lookup"><span data-stu-id="32148-138">Only the bin code that is defined on the component line of the source document is accepted.</span></span> <span data-ttu-id="32148-139">Ciò supporta il principio secondo cui il ruolo che richiede un componente, ovvero un addetto all'assemblaggio in questa procedura, sa dove deve essere inserito il componente.</span><span class="sxs-lookup"><span data-stu-id="32148-139">This supports the principle that the role who requests a component, which is an assembly worker in this procedure, knows where the component must be placed.</span></span> <span data-ttu-id="32148-140">Se si desidera inserire i componenti in una collocazione diversa, è necessario innanzitutto modificare il codice collocazione specificato nella riga componenti, quindi ricreare le righe movimenti di magazzino.</span><span class="sxs-lookup"><span data-stu-id="32148-140">If you want to place the components in a different bin, then you must first change the bin code on the component line and then re-create the inventory movement lines.</span></span>  
6.  <span data-ttu-id="32148-141">Nel campo **Qtà da gestire** immettere la quantità parziale o completa effettivamente spostata.</span><span class="sxs-lookup"><span data-stu-id="32148-141">In the **Qty. to Handle** field, enter the full or partial quantity that you have actually moved.</span></span> <span data-ttu-id="32148-142">Il valore nelle righe Prendere e Mettere deve essere identico.</span><span class="sxs-lookup"><span data-stu-id="32148-142">The value on the Take and the Place lines must be the same.</span></span> <span data-ttu-id="32148-143">In caso contrario, non è possibile registrare la movimentazione.</span><span class="sxs-lookup"><span data-stu-id="32148-143">Otherwise, you cannot register the movement.</span></span>  

    > [!NOTE]  
    >  <span data-ttu-id="32148-144">Come in altre attività di warehouse, è possibile suddividere la riga Posizione selezionando l'azione **Azioni** e scegliendo l'azione **Dividi riga**.</span><span class="sxs-lookup"><span data-stu-id="32148-144">As in other warehouse activities, you can split the Place line by selecting the **Actions** action and then choosing the **Split Line** action.</span></span> <span data-ttu-id="32148-145">In questo caso, la somma delle due righe divise Mettere deve essere uguale alla quantità nella riga Prendere.</span><span class="sxs-lookup"><span data-stu-id="32148-145">In that case, the sum of the two split Place lines must equal the quantity on the Take line.</span></span>  

7.  <span data-ttu-id="32148-146">Al momento di registrare le movimentazioni effettuate, scegliere l'azione **Registra movimentazioni inv.**.</span><span class="sxs-lookup"><span data-stu-id="32148-146">When you are ready to register the movements that you have performed, choose the **Register Invt. Movement** action.</span></span>  

    <span data-ttu-id="32148-147">I movimenti warehouse vengono creati in modo da riflettere la presenza dei componenti nelle collocazioni specificate nelle righe ordine di assemblaggio.</span><span class="sxs-lookup"><span data-stu-id="32148-147">Warehouse entries are created reflecting that the components now exist in the bins specified on the assembly order lines.</span></span>  

    > [!NOTE]  
    >  <span data-ttu-id="32148-148">A differenza di quando si spostano componenti con un prelievo magazzino, il consumo non viene registrato quando si registra un movimento di magazzino.</span><span class="sxs-lookup"><span data-stu-id="32148-148">Unlike when you move components with an inventory pick, consumption is not posted when you register an inventory movement.</span></span> <span data-ttu-id="32148-149">Tale passaggio deve essere eseguito separatamente registrando l'output e il consumo dell'ordine di assemblaggio.</span><span class="sxs-lookup"><span data-stu-id="32148-149">That step must be performed separately by posting the assembly order output and consumption.</span></span> <span data-ttu-id="32148-150">Per ulteriori informazioni, vedere Ordine di assemblaggio.</span><span class="sxs-lookup"><span data-stu-id="32148-150">For more information, see Assembly Order.</span></span>  

## <a name="see-also"></a><span data-ttu-id="32148-151">Vedi anche</span><span class="sxs-lookup"><span data-stu-id="32148-151">See Also</span></span>  
[<span data-ttu-id="32148-152">Gestione warehouse</span><span class="sxs-lookup"><span data-stu-id="32148-152">Warehouse Management</span></span>](warehouse-manage-warehouse.md)  
[<span data-ttu-id="32148-153">Magazzino</span><span class="sxs-lookup"><span data-stu-id="32148-153">Inventory</span></span>](inventory-manage-inventory.md)  
<span data-ttu-id="32148-154">[Impostazione gestione warehouse](warehouse-setup-warehouse.md)   </span><span class="sxs-lookup"><span data-stu-id="32148-154">[Setting Up Warehouse Management](warehouse-setup-warehouse.md)   </span></span>  
<span data-ttu-id="32148-155">[Gestione assemblaggio](assembly-assemble-items.md)  </span><span class="sxs-lookup"><span data-stu-id="32148-155">[Assembly Management](assembly-assemble-items.md)  </span></span>  
[<span data-ttu-id="32148-156">Dettagli di progettazione: Gestione warehouse</span><span class="sxs-lookup"><span data-stu-id="32148-156">Design Details: Warehouse Management</span></span>](design-details-warehouse-management.md)  
<span data-ttu-id="32148-157">[Utilizzo di [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="32148-157">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
