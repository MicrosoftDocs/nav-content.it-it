---
title: Impostazione di campagne di marketing in Dynamics NAV
description: Descrive come impostare e condurre le campagne di marketing in Dynamics NAV per identificare e coinvolgere prospect e fidelizzare i clienti.
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: marketing, campaign, promo, prospect
ms.date: 06/06/2017
ms.author: edupont
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 3f8fd64397161f00a289b0d0435ebcf2de76de80
ms.contentlocale: it-it
ms.lasthandoff: 10/16/2017

---
# <a name="managing-marketing-campaigns"></a><span data-ttu-id="dc818-103">Gestione di campagne di marketing</span><span class="sxs-lookup"><span data-stu-id="dc818-103">Managing Marketing Campaigns</span></span>
<span data-ttu-id="dc818-104">Per identificare, attirare e fidelizzare i clienti, è fondamentale mettere a punto un solido piano di marketing.</span><span class="sxs-lookup"><span data-stu-id="dc818-104">Having a strong marketing plan in place enables you to identify, attract, and retain customers.</span></span> <span data-ttu-id="dc818-105">Un piano di marketing comprende diverse campagne e altre interazioni correlate alle attività di marketing e di vendita.</span><span class="sxs-lookup"><span data-stu-id="dc818-105">A marketing plan consists of various campaigns and other interactions in connection with your sales and marketing activities.</span></span> <span data-ttu-id="dc818-106">Quando si pianifica una campagna, è necessario decidere a quali contatti rivolgersi, quale tipo di campagna creare (fiera commerciale o messaggi e-mail) e a quali agenti assegnare ogni task.</span><span class="sxs-lookup"><span data-stu-id="dc818-106">While planning a campaign, you need to decide which contacts to target, what type of campaign (such as trade show or direct mail), and what salespeople will perform each task.</span></span>

<span data-ttu-id="dc818-107">Ogni campagna deve prevedere diverse attività o task.</span><span class="sxs-lookup"><span data-stu-id="dc818-107">Each campaign consists of various activities or tasks.</span></span> <span data-ttu-id="dc818-108">È possibile combinare più task, ad esempio task che rappresentano un passaggio, nelle attività.</span><span class="sxs-lookup"><span data-stu-id="dc818-108">You can combine multiple task, for example tasks that each represent a step, in activities.</span></span> <span data-ttu-id="dc818-109">I task delle attività sono in relazione tra essi in base a una formula di date.</span><span class="sxs-lookup"><span data-stu-id="dc818-109">Activity tasks are related to each other by a date formula.</span></span> <span data-ttu-id="dc818-110">I singoli task possono essere assegnati solo agli agenti.</span><span class="sxs-lookup"><span data-stu-id="dc818-110">Individual tasks can only be assigned to salespeople.</span></span> <span data-ttu-id="dc818-111">Le attività possono essere assegnate a opportunità, agenti, gruppi di venditori e contatti.</span><span class="sxs-lookup"><span data-stu-id="dc818-111">Activities can be assigned to opportunities, salespeople, groups of sales people, and contacts.</span></span> <span data-ttu-id="dc818-112">Per ulteriori informazioni, vedere [Procedura: Impostare fasi ciclo e fasi di vendita delle opportunità](marketing-how-setup-opportunity-sales-cycles-stages.md).</span><span class="sxs-lookup"><span data-stu-id="dc818-112">For more information, see [How to: Set Up Opportunity Sales Cycles and Cycle Stages](marketing-how-setup-opportunity-sales-cycles-stages.md).</span></span>

## <a name="defining-individual-campaigns"></a><span data-ttu-id="dc818-113">Definizione di campagne singole</span><span class="sxs-lookup"><span data-stu-id="dc818-113">Defining individual campaigns</span></span>
<span data-ttu-id="dc818-114">Prima di creare una campagna, è necessario impostare *codici di stato campagna*.</span><span class="sxs-lookup"><span data-stu-id="dc818-114">Before you can create a campaign, you must set up *campaign status codes*.</span></span> <span data-ttu-id="dc818-115">L'utilizzo di questi codici consente di gestire le campagne assegnando ad esse uno stato.</span><span class="sxs-lookup"><span data-stu-id="dc818-115">Using these codes will help you manage your campaigns by assigning a status to the campaign.</span></span> <span data-ttu-id="dc818-116">Lavorando alle diverse fasi della campagna, sarà possibile sapere i passaggi completati e quelli ancora da iniziare.</span><span class="sxs-lookup"><span data-stu-id="dc818-116">As you work through the stages of a campaign, you are able to see what step a campaign is at and what step comes next.</span></span> <span data-ttu-id="dc818-117">I codici stato campagna vengono impostati nella finestra **Stato campagna**.</span><span class="sxs-lookup"><span data-stu-id="dc818-117">You set up campaign status codes in the **Campaign Status** window.</span></span>

<span data-ttu-id="dc818-118">È possibile creare una scheda campagna per ogni campagna di cui tenere traccia.</span><span class="sxs-lookup"><span data-stu-id="dc818-118">You can create a campaign card for each campaign that you want to keep track of.</span></span> <span data-ttu-id="dc818-119">È anche possibile visualizzare queste schede campagna per visualizzare informazioni generali su ogni campagna.</span><span class="sxs-lookup"><span data-stu-id="dc818-119">You can also view these campaign cards to view general information about your campaigns.</span></span>
<span data-ttu-id="dc818-120">È possibile eliminare movimenti campagna, come se il movimento registrasse un'azione che è stata annullata.</span><span class="sxs-lookup"><span data-stu-id="dc818-120">You can delete campaign entries, such as if the entry records an action that has been canceled.</span></span> <span data-ttu-id="dc818-121">È possibile eliminare solo movimenti campagna annullati.</span><span class="sxs-lookup"><span data-stu-id="dc818-121">Only canceled campaign entries can be deleted.</span></span>

### <a name="selecting-the-target-audience"></a><span data-ttu-id="dc818-122">Selezione del target</span><span class="sxs-lookup"><span data-stu-id="dc818-122">Selecting the target audience</span></span>
<span data-ttu-id="dc818-123">Dopo avere creato una campagna, è possibile iniziare a creare segmenti che specifichino il target della campagna.</span><span class="sxs-lookup"><span data-stu-id="dc818-123">After you have created a campaign, you can start creating segments that specify the target audience of the campaign.</span></span> <span data-ttu-id="dc818-124">Per ulteriori informazioni, vedere [Gestione dei segmenti](marketing-segments.md).</span><span class="sxs-lookup"><span data-stu-id="dc818-124">For more information, see [Managing Segments](marketing-segments.md).</span></span>

### <a name="registering-discount-percentages"></a><span data-ttu-id="dc818-125">Registrazione delle percentuali di sconto</span><span class="sxs-lookup"><span data-stu-id="dc818-125">Registering discount percentages</span></span>
<span data-ttu-id="dc818-126">Dopo avere impostato la campagna, avere stabilito quali segmenti coprirà la campagna e avere impostato la data di inizio e la data di fine, sarà possibile registrare la percentuale di sconto che verrà applicata al cliente per i singoli articoli nelle righe della finestra **Sconti riga vendita**.</span><span class="sxs-lookup"><span data-stu-id="dc818-126">When you have set up your campaign, decided what segments you want the campaign to cover, and set the starting and ending dates, you register the discount percentage that the customer will receive on the individual items on the lines in the **Sales Line Discounts** window.</span></span> <span data-ttu-id="dc818-127">È inoltre possibile registrare prezzi di vendita dei singoli articoli nelle righe della finestra **Prezzi vendita**.</span><span class="sxs-lookup"><span data-stu-id="dc818-127">You can also register the sales prices for the individual items on the lines in the **Sales Prices** window.</span></span> <span data-ttu-id="dc818-128">È possibile accedere a entrambe le finestre dalla scheda campagna.</span><span class="sxs-lookup"><span data-stu-id="dc818-128">You can access both windows from the campaign card.</span></span>

 <span data-ttu-id="dc818-129">Una volta impostati i prezzi di vendita e gli sconti riga, nonché i segmenti nella Scheda Campagna, è necessario attivarli in modo che i prezzi e gli sconti vengano riportati anche nelle righe.</span><span class="sxs-lookup"><span data-stu-id="dc818-129">When you have set up the sales prices/line discounts and the segments on the campaign card, you must activate them so that the campaign prices/discounts will be reflected on the lines.</span></span>

> [!NOTE]  
>   <span data-ttu-id="dc818-130">Per attivare i prezzi di vendita/ gli sconti riga, è necessario specificare se l'intero segmento o solo alcuni contatti sono obiettivi della campagna.</span><span class="sxs-lookup"><span data-stu-id="dc818-130">In order to activate the sales prices/line discounts, you must specify if the whole segment or only some contacts are targets of the campaign.</span></span> <span data-ttu-id="dc818-131">Se i prezzi di vendita e gli sconti riga riguardano tutti i contatti del segmento, selezionare il campo **Target campagna** disponibile nella Scheda dettaglio **Campagna** della scheda **Segmento**.</span><span class="sxs-lookup"><span data-stu-id="dc818-131">If the sales prices/line discounts covers all the contacts in the segment, select the **Campaign Target** field on the **Campaign** FastTab of the **Segment** card.</span></span>

<span data-ttu-id="dc818-132">Se i prezzi di vendita/gli sconti riga non vengono offerti a tutti i contatti del segmento, è possibile deselezionare il campo **Target campagna** per i contatti specifici.</span><span class="sxs-lookup"><span data-stu-id="dc818-132">If the sales prices/line discounts are not to be offered to all the contacts in the segment, you can clear the **Campaign Target** field for the relevant contacts.</span></span> <span data-ttu-id="dc818-133">Se non è possibile visualizzare questo campo, è possibile aggiungerlo alla vista.</span><span class="sxs-lookup"><span data-stu-id="dc818-133">If you cannot see this field, you can add it to your view.</span></span> <span data-ttu-id="dc818-134">Per ulteriori informazioni, vedere [Personalizzazione utente](ui-user-personalization.md).</span><span class="sxs-lookup"><span data-stu-id="dc818-134">For more information, see [User Personalization](ui-user-personalization.md).</span></span>

## <a name="conducting-campaigns"></a><span data-ttu-id="dc818-135">Esecuzione di campagne</span><span class="sxs-lookup"><span data-stu-id="dc818-135">Conducting campaigns</span></span>
<span data-ttu-id="dc818-136">Durante l'esecuzione di una campagna, vengono registrate tutte le interazioni con i contatti, o segmenti. In questo modo sarà possibile ottenere statistiche e altre informazioni sui costi e sulle probabilità di successo della campagna.</span><span class="sxs-lookup"><span data-stu-id="dc818-136">As a campaign runs, all interactions with your contacts, or segment, are recorded so that you can get statistics and other information about the costs and success rates of the campaign.</span></span>

<span data-ttu-id="dc818-137">Le campagne vengono eseguite dagli agenti ed è necessario creare attività per rappresentare ciascun task e per assegnarlo agli agenti pertinenti.</span><span class="sxs-lookup"><span data-stu-id="dc818-137">Campaigns are conducted by salespeople, and you must create activities to represent each task and assign them to the relevant salespeople.</span></span> <span data-ttu-id="dc818-138">Per ulteriori informazioni, vedere [Procedura: Impostare fasi ciclo e fasi di vendita delle opportunità](marketing-how-setup-opportunity-sales-cycles-stages.md).</span><span class="sxs-lookup"><span data-stu-id="dc818-138">For more information, see [How to: Set Up Opportunity Sales Cycles and Cycle Stages](marketing-how-setup-opportunity-sales-cycles-stages.md).</span></span>

## <a name="see-also"></a><span data-ttu-id="dc818-139">Vedi anche</span><span class="sxs-lookup"><span data-stu-id="dc818-139">See Also</span></span>
[<span data-ttu-id="dc818-140">Gestione dei contatti</span><span class="sxs-lookup"><span data-stu-id="dc818-140">Managing Contacts</span></span>](marketing-contacts.md)  
[<span data-ttu-id="dc818-141">Gestione dei segmenti</span><span class="sxs-lookup"><span data-stu-id="dc818-141">Managing Segments</span></span>](marketing-segments.md)  
[<span data-ttu-id="dc818-142">Gestione delle opportunità di vendita</span><span class="sxs-lookup"><span data-stu-id="dc818-142">Managing Sales Opportunities</span></span>](marketing-manage-sales-opportunities.md)  
[<span data-ttu-id="dc818-143">Utilizzo di Dynamics NAV</span><span class="sxs-lookup"><span data-stu-id="dc818-143">Working with Dynamics NAV</span></span>](ui-work-product.md)  
