---
title: Come impostare le warehouse di base con aree di operazioni
description: "Se le aree delle operazioni interne, ad esempio produzione o assemblaggio, sono presenti nelle configurazioni di warehouse di base in cui le ubicazioni utilizzano il campo di setup **Collocazione obbligatoria** ed eventualmente i campi di setup **Richiesto prelievo** e **Richiesto stoccaggio**, è possibile utilizzare tre documenti warehouse di base per registrare le attività di warehouse per le aree delle operazioni interne."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 09/08/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: d141fcb9f5357355272f6a34d71b88f50129985b
ms.contentlocale: it-it
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-set-up-basic-warehouses-with-operations-areas"></a><span data-ttu-id="55717-103">Procedura: Impostare le warehouse di base con aree di operazioni</span><span class="sxs-lookup"><span data-stu-id="55717-103">How to: Set Up Basic Warehouses with Operations Areas</span></span>
<span data-ttu-id="55717-104">Se le aree delle operazioni interne, ad esempio produzione o assemblaggio, sono presenti nelle configurazioni di base della warehouse in cui le ubicazioni utilizzano il campo di setup **Collocazione obbligatoria** ed eventualmente i campi di setup **Richiesto prelievo** e **Richiesto stoccaggio**, è possibile utilizzare i seguenti documenti warehouse di base per registrare le attività di warehouse per le aree delle operazioni interne:</span><span class="sxs-lookup"><span data-stu-id="55717-104">If internal operation areas such as production or assembly exist in basic warehouse configurations where locations use the **Bin Mandatory** setup field and possibly the **Require Pick** and **Require Put-away** setup fields, then you can use the following basic warehouse documents to record your warehouse activities for internal operation areas:</span></span>  

- <span data-ttu-id="55717-105">Finestra **Movimento di magazzino**.</span><span class="sxs-lookup"><span data-stu-id="55717-105">**Inventory Movement** window.</span></span>  
- <span data-ttu-id="55717-106">Finestra **Prelievi magazzino**.</span><span class="sxs-lookup"><span data-stu-id="55717-106">**Inventory Pick** window.</span></span>  
- <span data-ttu-id="55717-107">Finestra **Stoccaggio magazzino**.</span><span class="sxs-lookup"><span data-stu-id="55717-107">**Inventory Put-away** window.</span></span>

> [!NOTE]
> <span data-ttu-id="55717-108">Anche se le impostazioni sono definite **Richiesto prelievo** e **Richiesto stoccaggio**, è possibile registrare carichi e spedizioni direttamente dai documenti commerciali di origine nelle ubicazioni in cui si selezionano queste caselle di controllo.</span><span class="sxs-lookup"><span data-stu-id="55717-108">Even though the settings are called **Require Pick** and **Require Put-away**, you can still post receipts and shipments directly from the source business documents at locations where you select these check boxes.</span></span>  

<span data-ttu-id="55717-109">Per utilizzare queste finestre con le operazioni interne, ad esempio prelevare e spostare componenti in produzione, è necessario impostare alcune o tutte le seguenti procedure di setup in base al livello di controllo richiesto:</span><span class="sxs-lookup"><span data-stu-id="55717-109">To use these windows with internal operations, such as to pick and move components to production, you must make some or all the following setup steps depending on how much control you need:</span></span>  

- <span data-ttu-id="55717-110">Abilitare i documenti relativi a prelievi magazzino, spostamento e stoccaggio.</span><span class="sxs-lookup"><span data-stu-id="55717-110">Enable the inventory pick, move, and put-away documents.</span></span>  
- <span data-ttu-id="55717-111">Definire le strutture di collocazione di default per i componenti e gli articoli finali trasferiti da e verso le risorse dell'operazione.</span><span class="sxs-lookup"><span data-stu-id="55717-111">Define default bin structures for components and end items flowing to and from operation resources.</span></span>  
- <span data-ttu-id="55717-112">Creare collocazioni di provenienza e destinazione dedicate alle risorse specifiche dell'operazione per evitare il prelievo degli articoli per i documenti in uscita.</span><span class="sxs-lookup"><span data-stu-id="55717-112">Make to- and from- bins that are dedicated to specific operation resources to prevent the items from being picked for outbound documents.</span></span>

<span data-ttu-id="55717-113">I codici di collocazione impostati nelle schede ubicazione consentono di definire un flusso di warehouse di default per determinate attività, come i componenti di un reparto di assemblaggio.</span><span class="sxs-lookup"><span data-stu-id="55717-113">Bin codes that are set up on location cards define a default warehouse flow for certain activities, such as components in an assembly department.</span></span> <span data-ttu-id="55717-114">La funzionalità aggiuntiva consente di garantire che quando gli articoli si trovano in una determinata collocazione, non possono essere spostati o prelevati per altre attività.</span><span class="sxs-lookup"><span data-stu-id="55717-114">Additional functionality exists to make sure that when items are placed in a certain bin, they cannot be moved or picked to other activities.</span></span> <span data-ttu-id="55717-115">Per ulteriori informazioni, vedere la sezione "Per creare collocazioni componenti dedicate".</span><span class="sxs-lookup"><span data-stu-id="55717-115">For more information, see the "To create dedicated component bins" section.</span></span>

<span data-ttu-id="55717-116">Le procedure riportate di seguito sono basate sull'impostazione di attività di warehouse di base relative a un'area di produzione.</span><span class="sxs-lookup"><span data-stu-id="55717-116">The following procedures are based on setting up basic warehouse activities around a production area.</span></span> <span data-ttu-id="55717-117">I passaggi sono simili ad altre aree dell'operazione, come assemblaggio, gestione assistenza e commesse.</span><span class="sxs-lookup"><span data-stu-id="55717-117">The steps are similar for other operation areas, such as assembly, service management, and jobs.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="55717-118">Nella procedura riportata di seguito, il campo di setup **Collocazione obbligatoria** nelle schede ubicazione è selezionato come condizione preliminare perché è considerato la base di qualsiasi livello di gestione warehouse.</span><span class="sxs-lookup"><span data-stu-id="55717-118">In the following procedure, the **Bin Mandatory** setup field on location cards is selected as a precondition because that is considered the foundation for any level of warehouse management.</span></span>  

## <a name="to-enable-inventory-documents-for-internal-operation-activities"></a><span data-ttu-id="55717-119">Per abilitare i documenti di magazzino per le attività delle operazioni interne</span><span class="sxs-lookup"><span data-stu-id="55717-119">To enable inventory documents for internal operation activities</span></span>  
1.  <span data-ttu-id="55717-120">Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "Cerca pagina o report"), immettere **Ubicazioni**, quindi scegliere il collegamento correlato.</span><span class="sxs-lookup"><span data-stu-id="55717-120">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Locations**, and then choose the related link.</span></span>
2. <span data-ttu-id="55717-121">Aprire la scheda Ubicazione che si desidera configurare.</span><span class="sxs-lookup"><span data-stu-id="55717-121">Open the location card you want to set up.</span></span>  
3.  <span data-ttu-id="55717-122">Nella Scheda Dettaglio **Warehouse** selezionare la casella di controllo **Richiesto stoccaggio** per indicare che quando viene rilasciato un documento di origine in entrata o interno con un codice collocazione, può essere creato un documento di stoccaggio magazzino o di movimento di magazzino.</span><span class="sxs-lookup"><span data-stu-id="55717-122">On the **Warehouse** FastTab, select the **Require Put-away** check box to indicate that, when an inbound or internal source document with a bin code is released, an inventory put-away or an inventory movement document can be created.</span></span>  
4.  <span data-ttu-id="55717-123">Selezionare la casella di controllo **Richiesto prelievo** per indicare che quando viene creato un documento di origine in uscita o interno con un codice collocazione, deve essere creato un documento di prelievi magazzino o di movimento di magazzino.</span><span class="sxs-lookup"><span data-stu-id="55717-123">Select the **Require Pick** check box to indicate that when an outbound or internal source document with a bin code is created, an inventory pick or an inventory movement document must be created.</span></span>  

## <a name="to-define-a-default-bin-structure-in-the-production-area"></a><span data-ttu-id="55717-124">Per definire una struttura di collocazione di default nell'area di produzione</span><span class="sxs-lookup"><span data-stu-id="55717-124">To define a default bin structure in the production area</span></span>  
1.  <span data-ttu-id="55717-125">Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "Cerca pagina o report"), immettere **Ubicazioni**, quindi scegliere il collegamento correlato.</span><span class="sxs-lookup"><span data-stu-id="55717-125">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Locations**, and then choose the related link.</span></span>
2. <span data-ttu-id="55717-126">Aprire l'ubicazione che si desidera configurare.</span><span class="sxs-lookup"><span data-stu-id="55717-126">Open the Location you want to set up.</span></span>  
3.  <span data-ttu-id="55717-127">Nel campo **Codice coll. produzione aperta** della Scheda Dettaglio **Collocazioni** immettere il codice della collocazione nell'area di produzione con tutti i componenti che l'operatore macchina può consumare senza richiedere un'attività di warehouse per portarli alla collocazione.</span><span class="sxs-lookup"><span data-stu-id="55717-127">On the **Bins** FastTab, in the **Open Shop Floor Bin Code** field, enter the code of the bin in the production area with plenty of components that the machine operator can consume from without requesting a warehouse activity to bring them to the bin.</span></span> <span data-ttu-id="55717-128">Gli articoli che si trovano in questa collocazione vengono in genere impostati per la registrazione automatica o la consuntivazione.</span><span class="sxs-lookup"><span data-stu-id="55717-128">Items that are placed in this bin are typically set up for automatic posting, or flushing.</span></span> <span data-ttu-id="55717-129">Ciò significa che il campo **Metodo consuntivazione** contiene **Avanti** o **Indietro**.</span><span class="sxs-lookup"><span data-stu-id="55717-129">This means that the **Flushing Method** field contains **Forward** or **Backward**.</span></span>  
4. <span data-ttu-id="55717-130">Nel campo **Cod. coll. art. per produzione** immettere il codice della collocazione nell'area di produzione in cui i componenti prelevati per la produzione in questa ubicazione vengono inseriti per default prima di poter essere consumati.</span><span class="sxs-lookup"><span data-stu-id="55717-130">In the **To-Production Bin Code** field, enter the code of the bin in the production area where components that are picked for production at this location are placed by default before they can be consumed.</span></span> <span data-ttu-id="55717-131">Gli articoli che si trovano in questa collocazione vengono in genere impostati per la registrazione del consumo manuale.</span><span class="sxs-lookup"><span data-stu-id="55717-131">Items that are placed in this bin are typically set up for manual consumption posting.</span></span> <span data-ttu-id="55717-132">Ciò significa che il campo **Metodo consuntivazione** contiene **Manuale** o **Prelievo+Aut.Inizio** o **Prelievo+Aut.Fine** per i prelievi warehouse e i movimenti di magazzino.</span><span class="sxs-lookup"><span data-stu-id="55717-132">This means that the **Flushing Method** field contains **Manual** or **Pick + Forward** or **Pick + Backward** for warehouse picks and inventory movements.</span></span>  

    > [!NOTE]  
    >  <span data-ttu-id="55717-133">Quando si utilizzano prelievi da magazzino, il campo **Cod. collocazione** nella riga di componente di un ordine di produzione definisce la collocazione *prendere* da dove vengono diminuiti i componenti quando viene registrato il consumo.</span><span class="sxs-lookup"><span data-stu-id="55717-133">When you use inventory picks, the **Bin Code** field on a production order component line defines the *take* bin from where components are decreased when posting consumption.</span></span> <span data-ttu-id="55717-134">Quando si utilizzano i movimenti di magazzino, il campo **Cod. collocazione** nelle righe di componenti dell'ordine di produzione definisce la collocazione *mettere* nell'area di operazione in cui l'addetto alla warehouse deve posizionare i componenti.</span><span class="sxs-lookup"><span data-stu-id="55717-134">When you use inventory movements, the **Bin Code** field on production order component lines defines the *place* bin in the operation area where the warehouse worker must place the components.</span></span>  

5. <span data-ttu-id="55717-135">Nel campo **Cod. coll. art. da produzione** della Scheda Dettaglio **Collocazioni** immettere il codice della collocazione nell'area di produzione da cui gli articoli finali completati vengono prelevati per default quando il processo comporta un'attività di warehouse.</span><span class="sxs-lookup"><span data-stu-id="55717-135">On the **Bins** FastTab, in the **From-Production Bin Code** field, enter the code of the bin in the production area where finished end items are taken from by default when the process involves a warehouse activity.</span></span> <span data-ttu-id="55717-136">Nelle configurazioni di warehouse di base, l'attività viene registrata come uno stoccaggio o un movimento di magazzino.</span><span class="sxs-lookup"><span data-stu-id="55717-136">In basic warehouse configurations, the activity is recorded as an inventory put-away or an inventory movement.</span></span>  

<span data-ttu-id="55717-137">A questo punto, le righe dei componenti dell'ordine di produzione con il codice collocazione di default che necessitano di componenti prelevati a priori vengono posizionate in quel punto.</span><span class="sxs-lookup"><span data-stu-id="55717-137">Now, production order component lines with the default bin code require that forward-flushed components are placed there.</span></span> <span data-ttu-id="55717-138">Tuttavia, fino a quando i componenti vengono utilizzati da tale collocazione, in seguito alle domande di altri componenti è possibile prelevare o utilizzare questi ultimi da tale collocazione perché sono ancora considerati contenuti della collocazione disponibili.</span><span class="sxs-lookup"><span data-stu-id="55717-138">However, until the components are consumed from that bin, other component demands may pick or consume from that bin because they are still considered available bin contents.</span></span> <span data-ttu-id="55717-139">Per verificare che il contenuto della collocazione sia disponibile solo per la domanda di componenti che utilizza la collocazione articoli per produzione, è necessario selezionare il campo **Dedicata** sulla riga per tale codice collocazione nella finestra **Collocazioni** aperta dalla scheda ubicazione.</span><span class="sxs-lookup"><span data-stu-id="55717-139">To make sure that bin content is only available to component demand that uses that to-production bin, you must select the **Dedicated** field on the line for that bin code in the **Bins** window that you open from the location card.</span></span>

<span data-ttu-id="55717-140">Questo diagramma di flusso illustra in che modo il campo **Cod. collocazione** nelle righe del componente dell'ordine di produzione viene compilato in base al setup.</span><span class="sxs-lookup"><span data-stu-id="55717-140">This flow chart shows how the **Bin Code** field on production order component lines is filled according to your setup.</span></span>  

<span data-ttu-id="55717-141">![Diagramma di flusso collocazione](media/binflow.png "BinFlow")</span><span class="sxs-lookup"><span data-stu-id="55717-141">![Bin flow chart](media/binflow.png "BinFlow")</span></span>    

## <a name="to-define-a-default-bin-structure-in-the-assembly-area"></a><span data-ttu-id="55717-142">Per definire una struttura di collocazione di default nell'area di assemblaggio</span><span class="sxs-lookup"><span data-stu-id="55717-142">To define a default bin structure in the assembly area</span></span>
<span data-ttu-id="55717-143">I componenti per gli ordini di assemblaggio non possono essere prelevati o registrati con i prelievi da magazzino.</span><span class="sxs-lookup"><span data-stu-id="55717-143">Components for assembly orders cannot be picked or posted with inventory picks.</span></span> <span data-ttu-id="55717-144">Pertanto, utilizzare la finestra **Movimento di magazzino**.</span><span class="sxs-lookup"><span data-stu-id="55717-144">Instead, use the **Inventory Movement** window.</span></span> <span data-ttu-id="55717-145">Per ulteriori informazioni, vedere [Procedura: Spostare componenti in un'area di operazione nella gestione warehouse di base](warehouse-how-to-move-components-to-an-operation-area-in-basic-warehousing.md).</span><span class="sxs-lookup"><span data-stu-id="55717-145">For more information, see [How to: Move Components to an Operation Area in Basic Warehousing](warehouse-how-to-move-components-to-an-operation-area-in-basic-warehousing.md).</span></span>

<span data-ttu-id="55717-146">Durante il prelievo e la spedizione di quantità righe di vendita assemblate sull'ordine, è necessario seguire determinate regole per la creazione di righe di prelievo magazzino.</span><span class="sxs-lookup"><span data-stu-id="55717-146">When picking and shipping sales line quantities that are assembled to the order, you must follow certain rules when creating the inventory pick lines.</span></span> <span data-ttu-id="55717-147">Per altre informazioni, vedere la sezione "Gestione di articoli da assemblare su ordine in prelievi magazzino" in [Procedura: Prelevare articoli con prelievi magazzino](warehouse-how-to-pick-items-with-inventory-picks.md).</span><span class="sxs-lookup"><span data-stu-id="55717-147">For more information, see the “Handling Assemble-to-Order Items in Inventory Picks” section in [How to: Pick Items with Inventory Picks](warehouse-how-to-pick-items-with-inventory-picks.md).</span></span>

<span data-ttu-id="55717-148">Per ulteriori informazioni, vedere [Gestione assemblaggio](assembly-assemble-items.md).</span><span class="sxs-lookup"><span data-stu-id="55717-148">For more information, see [Assembly Management](assembly-assemble-items.md).</span></span>

### <a name="to-set-up-that-an-inventory-movement-is-automatically-created-when-the-inventory-pick-for-the-assembly-item-is-created"></a><span data-ttu-id="55717-149">Per impostare la creazione automatica di un movimento di magazzino quando viene creato il prelievo magazzino per l'articolo di assemblaggio</span><span class="sxs-lookup"><span data-stu-id="55717-149">To set up that an inventory movement is automatically created when the inventory pick for the assembly item is created</span></span>
1. <span data-ttu-id="55717-150">Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "Cerca pagina o report"), immettere **Setup assemblaggio**, quindi scegliere il collegamento correlato.</span><span class="sxs-lookup"><span data-stu-id="55717-150">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Assembly Setup**, and then choose the related link.</span></span>
2. <span data-ttu-id="55717-151">Selezionare la casella di controllo **Crea movimenti automaticamente**.</span><span class="sxs-lookup"><span data-stu-id="55717-151">Select the **Create Movements Automatically** check box.</span></span>

### <a name="to-set-up-the-bin-in-the-assembly-area-where-components-are-placed-by-default-before-they-can-be-consumed-in-assembly"></a><span data-ttu-id="55717-152">Per impostare la collocazione nell'area di assemblaggio in cui i componenti vengono inseriti per default prima di poter essere consumati in fase di assemblaggio</span><span class="sxs-lookup"><span data-stu-id="55717-152">To set up the bin in the assembly area where components are placed by default before they can be consumed in assembly</span></span>
<span data-ttu-id="55717-153">Il valore in questo campo viene automaticamente inserito nel campo **Codice collocazione** nelle righe ordine di assemblaggio quando questa ubicazione viene immessa nel campo **Codice ubicazione** nella riga di ordine di assemblaggio.</span><span class="sxs-lookup"><span data-stu-id="55717-153">The value in this field is automatically inserted in the **Bin Code** field on assembly order lines when this location is entered in the **Location Code** field on the assembly order line.</span></span>

1. <span data-ttu-id="55717-154">Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "Cerca pagina o report"), immettere **Ubicazioni**, quindi scegliere il collegamento correlato.</span><span class="sxs-lookup"><span data-stu-id="55717-154">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Locations**, and then choose the related link.</span></span>
2. <span data-ttu-id="55717-155">Aprire l'ubicazione che si desidera configurare.</span><span class="sxs-lookup"><span data-stu-id="55717-155">Open the Location you want to set up.</span></span>
3. <span data-ttu-id="55717-156">Compilare il campo **Cod. coll. art. per assembl.**.</span><span class="sxs-lookup"><span data-stu-id="55717-156">Fill in the **To-Assembly Bin Code** field.</span></span>

### <a name="to-set-up-the-bin-in-the-assembly-area-where-finished-assembly-items-are-posted-to-when-they-are-assembled-to-stock"></a><span data-ttu-id="55717-157">Per impostare la collocazione nell'area di assemblaggio in cui gli articoli di assemblaggio completati sono registrati quando vengono assemblati per magazzino</span><span class="sxs-lookup"><span data-stu-id="55717-157">To set up the bin in the assembly area where finished assembly items are posted to when they are assembled to stock</span></span>
<span data-ttu-id="55717-158">Il valore in questo campo viene automaticamente inserito nel campo **Codice collocazione** nelle testate degli ordini di assemblaggio quando questo codice ubicazione viene immesso nel campo **Codice ubicazione** nella testata dell'ordine di assemblaggio.</span><span class="sxs-lookup"><span data-stu-id="55717-158">The value in this field is automatically inserted in the **Bin Code** field on assembly order headers when this location code is filled into the **Location Code** field on the assembly order header.</span></span>

<span data-ttu-id="55717-159">I codici collocazione impostati nelle schede ubicazione consentono di definire un flusso di warehouse di default per determinate attività di warehouse, come il consumo di componenti in un'area di assemblaggio.</span><span class="sxs-lookup"><span data-stu-id="55717-159">Bin codes that are set up on location cards define a default warehouse flow for specific warehouse activities, such as consumption of components in an assembly area.</span></span> <span data-ttu-id="55717-160">La funzionalità aggiuntiva consente di garantire che quando gli articoli si trovano in una collocazione di default, non possono essere spostati o prelevati per altre attività.</span><span class="sxs-lookup"><span data-stu-id="55717-160">Additional functionality exists to make sure that when items are placed in a default bin, they cannot be moved or picked to other activities.</span></span>

> [!NOTE]
> <span data-ttu-id="55717-161">Questo setup è possibile soltanto per le ubicazioni in cui è selezionato il campo Collocazione obbligatoria.</span><span class="sxs-lookup"><span data-stu-id="55717-161">This setup is only possible for locations where the Bin Mandatory field is selected.</span></span>

1. <span data-ttu-id="55717-162">Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "Cerca pagina o report"), immettere **Ubicazioni**, quindi scegliere il collegamento correlato.</span><span class="sxs-lookup"><span data-stu-id="55717-162">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Locations**, and then choose the related link.</span></span>
2. <span data-ttu-id="55717-163">Aprire l'ubicazione che si desidera configurare.</span><span class="sxs-lookup"><span data-stu-id="55717-163">Open the Location you want to set up.</span></span>
3. <span data-ttu-id="55717-164">Compilare il campo **Cod. coll. art. da assembl.**.</span><span class="sxs-lookup"><span data-stu-id="55717-164">Fill in the **From-Assembly Bin Code** field.</span></span>

### <a name="to-set-up-the-bin-where-finished-assembly-items-are-posted-to-when-they-are-assembled-to-a-linked-sales-order"></a><span data-ttu-id="55717-165">Per impostare la collocazione in cui gli articoli di assemblaggio completati sono registrati quando vengono assemblati per ordine di vendita collegato</span><span class="sxs-lookup"><span data-stu-id="55717-165">To set up the bin where finished assembly items are posted to when they are assembled to a linked sales order</span></span>
<span data-ttu-id="55717-166">Da questa collocazione gli articoli di assemblaggio sono spediti immediatamente, tramite un prelievo di magazzino, per evadere l'ordine di vendita.</span><span class="sxs-lookup"><span data-stu-id="55717-166">From this bin, the assembly items are shipped immediately, via an inventory pick, to fulfill the sales order.</span></span>

> [!NOTE]
> <span data-ttu-id="55717-167">Questo campo non può essere utilizzato se l'ubicazione prevede l'uso di prelievi e stoccaggi guidati.</span><span class="sxs-lookup"><span data-stu-id="55717-167">This field cannot be used if the location is set up to use directed pick and put-away.</span></span>

<span data-ttu-id="55717-168">Il codice collocazione viene copiato dalla riga di ordine di vendita nella testata ordine di assemblaggio per comunicare agli addetti all'assemblaggio dove posizionare l'output per prepararlo alla spedizione.</span><span class="sxs-lookup"><span data-stu-id="55717-168">The bin code is copied from the sales order line to the assembly order header to communicate to assembly workers where to place the output to ready it for shipping.</span></span> <span data-ttu-id="55717-169">Viene copiato anche nella riga di prelievo magazzino per comunicare agli addetti alla warehouse da dove effettuare il prelievo per la spedizione.</span><span class="sxs-lookup"><span data-stu-id="55717-169">It is also copied to the inventory pick line to communicate to warehouse workers where to take it from to ship it.</span></span>

> [!NOTE]
> <span data-ttu-id="55717-170">La collocazione di spedizione Assemblaggio su ordine è sempre vuota.</span><span class="sxs-lookup"><span data-stu-id="55717-170">The Assemble-to-Order Shipment bin is always empty.</span></span> <span data-ttu-id="55717-171">Quando si registra una riga vendite di assemblaggio su ordine, il contenuto della collocazione viene prima rettificato positivamente con l'output di assemblaggio.</span><span class="sxs-lookup"><span data-stu-id="55717-171">When you post an assemble-to-order sales line, then the bin content is first positively adjusted with the assembly output.</span></span> <span data-ttu-id="55717-172">Subito dopo viene rettificato negativamente con la quantità spedita.</span><span class="sxs-lookup"><span data-stu-id="55717-172">Immediately after, it is negatively adjusted with the shipped quantity.</span></span>

<span data-ttu-id="55717-173">Il valore in questo campo viene automaticamente inserito nel campo Codice collocazione nelle righe ordine di vendita che contengono una quantità nel campo **Qtà per assemblaggio su ordine** o se per l'articolo da vendere è impostato **Assemblaggio su ordine** nel campo **Sistema di rifornimento**.</span><span class="sxs-lookup"><span data-stu-id="55717-173">The value in this field is automatically inserted in the Bin Code field on sales order lines that contain a quantity in the **Qty. to Assemble to Order** field or if the item to be sold has **Assemble-to-Order** in the **Replenishment System** field.</span></span>

<span data-ttu-id="55717-174">Se **Cod. coll. sp. ass. su ordine** è vuoto, viene utilizzato il campo **Cod. coll. art. da assembl.**.</span><span class="sxs-lookup"><span data-stu-id="55717-174">If the **Asm.-to-Order Shpt. Bin Code** is blank, then the **From-Assembly Bin Code** field is used instead.</span></span> <span data-ttu-id="55717-175">Se entrambi i campi di setup sono vuoti, la collocazione con contenuto utilizzata per ultima viene utilizzata nel campo **Codice collocazione** nelle righe ordine di vendita.</span><span class="sxs-lookup"><span data-stu-id="55717-175">If both setup fields are blank, then the last used bin with content is used in the **Bin Code** field on sales order lines.</span></span>

<span data-ttu-id="55717-176">Lo stesso codice collocazione a sua volta viene copiato nel campo **Codice collocazione** sulla riga di prelievo magazzino che gestisce la spedizione della quantità per l'assemblaggio su ordine.</span><span class="sxs-lookup"><span data-stu-id="55717-176">The same bin code is in turn copied to the **Bin Code** field on the inventory pick line that manages the shipment of the assemble-to-order quantity.</span></span> <span data-ttu-id="55717-177">Per altre informazioni, vedere la sezione "Gestione di articoli da assemblare su ordine in prelievi magazzino" in [Procedura: Prelevare articoli con prelievi magazzino](warehouse-how-to-pick-items-with-inventory-picks.md).</span><span class="sxs-lookup"><span data-stu-id="55717-177">For more information, see the “Handling Assemble-to-Order Items in Inventory Picks” section in [How to: Pick Items with Inventory Picks](warehouse-how-to-pick-items-with-inventory-picks.md).</span></span>

1. <span data-ttu-id="55717-178">Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "Cerca pagina o report"), immettere **Ubicazioni**, quindi scegliere il collegamento correlato.</span><span class="sxs-lookup"><span data-stu-id="55717-178">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Locations**, and then choose the related link.</span></span>
2. <span data-ttu-id="55717-179">Aprire l'ubicazione che si desidera configurare.</span><span class="sxs-lookup"><span data-stu-id="55717-179">Open the Location you want to set up.</span></span>
3. <span data-ttu-id="55717-180">Compilare il campo **Cod. coll. sp. ass. su ordine**.</span><span class="sxs-lookup"><span data-stu-id="55717-180">Fill in the **Asm.-to-Order Shpt. Bin Code** field.</span></span>

## <a name="to-create-dedicated-component-bins"></a><span data-ttu-id="55717-181">Per creare collocazioni di componenti dedicate</span><span class="sxs-lookup"><span data-stu-id="55717-181">To create dedicated component bins</span></span>
<span data-ttu-id="55717-182">È possibile specificare che le quantità in una collocazione siano protette dal prelievo per domande diverse da quella corrente.</span><span class="sxs-lookup"><span data-stu-id="55717-182">You can specify that quantities in a bin are protected from being picked for other demands than demand from their current purpose.</span></span>

<span data-ttu-id="55717-183">Le quantità nelle collocazioni dedicate possono comunque essere impegnate.</span><span class="sxs-lookup"><span data-stu-id="55717-183">Quantities in dedicated bins can still be reserved.</span></span> <span data-ttu-id="55717-184">Di conseguenza, le quantità nelle collocazioni dedicate sono incluse nel campo **Quantità totale disponibile** della finestra **Impegno**.</span><span class="sxs-lookup"><span data-stu-id="55717-184">Accordingly, the quantities in dedicated bins are included in the **Total Available Quantity** field in the **Reservation** window.</span></span>

<span data-ttu-id="55717-185">Ad esempio, un'area di produzione impostata con un codice collocazione nel campo **Cod. coll. art. per produzione**.</span><span class="sxs-lookup"><span data-stu-id="55717-185">For example, is a work center is set up with a bin code in the **To-Production Bin Code** field.</span></span> <span data-ttu-id="55717-186">Le righe componenti di ordini di produzione con il codice collocazione che necessitano di componenti prelevati a priori vengono posizionate in quel punto.</span><span class="sxs-lookup"><span data-stu-id="55717-186">Production order component lines with that bin code require that forward-flushed components are placed there.</span></span> <span data-ttu-id="55717-187">Tuttavia, fino a quando i componenti vengono utilizzati da tale collocazione, in seguito alle domande di altri componenti è possibile prelevare o utilizzare questi ultimi da tale collocazione perché sono ancora considerati contenuti della collocazione disponibili.</span><span class="sxs-lookup"><span data-stu-id="55717-187">However, until the components are consumed from that bin, other component demands may pick or consume from that bin because they are still considered available bin contents.</span></span> <span data-ttu-id="55717-188">Per verificare che il contenuto della collocazione sia disponibile solo per la domanda di componenti che utilizza la collocazione articoli per produzione, è necessario selezionare il campo **Dedicata** sulla riga per tale codice collocazione nella finestra **Collocazioni** aperta dalla scheda ubicazione.</span><span class="sxs-lookup"><span data-stu-id="55717-188">To make sure that bin content is only available to component demand that uses that to-production bin, you must select the **Dedicated** field on the line for that bin code in the **Bins** window that you open from the location card.</span></span>

<span data-ttu-id="55717-189">La creazione di una collocazione dedicata fornisce una funzionalità simile all'utilizzo di tipi di collocazione, disponibile solo nella gestione warehouse avanzata.</span><span class="sxs-lookup"><span data-stu-id="55717-189">Making a bin dedicated provides similar functionality to using bin types, which is only available in advanced warehousing.</span></span> <span data-ttu-id="55717-190">Per ulteriori informazioni, vedere [Procedura: Impostare i tipi di collocazioni](warehouse-how-to-set-up-bin-types.md).</span><span class="sxs-lookup"><span data-stu-id="55717-190">For more information, see [How to: Set Up Bin Types](warehouse-how-to-set-up-bin-types.md).</span></span>

> [!Caution]
> <span data-ttu-id="55717-191">Gli articoli nelle collocazioni dedicate non sono protetti quando vengono prelevati e utilizzati come componenti di produzione tramite la finestra Prelievo magazzino.</span><span class="sxs-lookup"><span data-stu-id="55717-191">Items in dedicated bins are not protected when they are picked and consumed as production components with the Inventory Pick window.</span></span>

1.  <span data-ttu-id="55717-192">Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "Cerca pagina o report"), immettere **Ubicazioni**, quindi scegliere il collegamento correlato.</span><span class="sxs-lookup"><span data-stu-id="55717-192">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Locations**, and then choose the related link.</span></span> <span data-ttu-id="55717-193">Selezionare l'ubicazione che si desidera aggiornare.</span><span class="sxs-lookup"><span data-stu-id="55717-193">Select the location that you want to update.</span></span>  
2.  <span data-ttu-id="55717-194">Scegliere l'azione **Collocazioni**.</span><span class="sxs-lookup"><span data-stu-id="55717-194">Choose the **Bins** action.</span></span>  
3.  <span data-ttu-id="55717-195">Selezionare il campo **Dedicata** per ogni collocazione che si desidera utilizzare in modo esclusivo per determinate operazioni interne e in cui si desidera impegnare quantità per tale operazione interna, una volta inserite.</span><span class="sxs-lookup"><span data-stu-id="55717-195">Select the **Dedicated** field for each bin that you want to use exclusively for certain internal operations and where you want quantities to be reserved for that internal operation once placed there.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="55717-196">La collocazione deve essere vuota prima di poter selezionare o deselezionare il campo **Dedicata**.</span><span class="sxs-lookup"><span data-stu-id="55717-196">The bin must be empty before you can select or clear the **Dedicated** field.</span></span>

## <a name="see-also"></a><span data-ttu-id="55717-197">Vedi anche</span><span class="sxs-lookup"><span data-stu-id="55717-197">See Also</span></span>  
[<span data-ttu-id="55717-198">Gestione warehouse</span><span class="sxs-lookup"><span data-stu-id="55717-198">Warehouse Management</span></span>](warehouse-manage-warehouse.md)  
[<span data-ttu-id="55717-199">Magazzino</span><span class="sxs-lookup"><span data-stu-id="55717-199">Inventory</span></span>](inventory-manage-inventory.md)  
<span data-ttu-id="55717-200">[Impostazione gestione warehouse](warehouse-setup-warehouse.md)   </span><span class="sxs-lookup"><span data-stu-id="55717-200">[Setting Up Warehouse Management](warehouse-setup-warehouse.md)   </span></span>  
<span data-ttu-id="55717-201">[Gestione assemblaggio](assembly-assemble-items.md)  </span><span class="sxs-lookup"><span data-stu-id="55717-201">[Assembly Management](assembly-assemble-items.md)  </span></span>  
[<span data-ttu-id="55717-202">Dettagli di progettazione: Gestione warehouse</span><span class="sxs-lookup"><span data-stu-id="55717-202">Design Details: Warehouse Management</span></span>](design-details-warehouse-management.md)  
<span data-ttu-id="55717-203">[Utilizzo di [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="55717-203">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  
