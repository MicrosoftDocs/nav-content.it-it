---
title: Creazione di numerazioni
author: SusanneWindfeldPedersen
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 6b60b1344a1e18ad91863046110df880f75f7c04
ms.openlocfilehash: e42e5ed139b2487fea13ef0fd57757035764addd
ms.contentlocale: it-it
ms.lasthandoff: 07/19/2017

---

# <a name="create-number-series"></a><span data-ttu-id="1cb8e-102">Creazione di numerazioni</span><span class="sxs-lookup"><span data-stu-id="1cb8e-102">Create Number Series</span></span>

<span data-ttu-id="1cb8e-103">Per ogni società impostata, è necessario assegnare codici di identificazione univoci a elementi quali i conti di contabilità generale, i conti clienti e i conti fornitori, le fatture e i documenti.</span><span class="sxs-lookup"><span data-stu-id="1cb8e-103">For each company that you set up, you need to assign unique identification codes to things such as general ledger accounts, customer and vendor accounts, invoices, and documents.</span></span> <span data-ttu-id="1cb8e-104">La numerazione è importante non solo ai fini dell'identificazione.</span><span class="sxs-lookup"><span data-stu-id="1cb8e-104">Numbering is important not only for identification.</span></span> <span data-ttu-id="1cb8e-105">Un sistema di numerazione progettato correttamente semplifica la gestione e l'analisi della società e può ridurre il numero di errori correlati all'immissione dei dati.</span><span class="sxs-lookup"><span data-stu-id="1cb8e-105">A well-designed numbering system also makes the company more manageable and easy to analyze, and can reduce the number of errors that occur in data entry.</span></span>

<span data-ttu-id="1cb8e-106">È possibile impostare un sistema con una quantità illimitata di numerazioni.</span><span class="sxs-lookup"><span data-stu-id="1cb8e-106">You can set up a complete numbering system with an unlimited number of number series.</span></span> <span data-ttu-id="1cb8e-107">È possibile utilizzare le numerazioni per tutti i tipi di documenti e di registrazioni, nonché per l'anagrafica, ad esempio per clienti, articoli e commesse.</span><span class="sxs-lookup"><span data-stu-id="1cb8e-107">You can use number series for all types of documents and journals, as well as for master data such as customers, items, and jobs.</span></span>

<span data-ttu-id="1cb8e-108">È possibile combinare l'utilizzo delle numerazioni con la numerazione manuale.</span><span class="sxs-lookup"><span data-stu-id="1cb8e-108">You can combine the use of number series with manual numbering.</span></span>

<span data-ttu-id="1cb8e-109">Per creare un sistema di numerazione, è necessario impostare uno o più codici per ogni tipo di anagrafica o documento.</span><span class="sxs-lookup"><span data-stu-id="1cb8e-109">You create a numbering system by setting up one or more codes for each type of master data or document.</span></span> <span data-ttu-id="1cb8e-110">È possibile, ad esempio, impostare un codice per la numerazione dei clienti, un altro per la numerazione delle fatture di vendita e un altro ancora per la numerazione di documenti in registrazioni COGE.</span><span class="sxs-lookup"><span data-stu-id="1cb8e-110">For example, you can set up one code for numbering customers, another code for numbering sales invoices, and another code for numbering documents in general journals.</span></span>

<span data-ttu-id="1cb8e-111">Dopo avere impostato un codice, è necessario impostare almeno una riga di numerazione.</span><span class="sxs-lookup"><span data-stu-id="1cb8e-111">After you have set up a code, you set must set up at least one number series line.</span></span> <span data-ttu-id="1cb8e-112">Tale riga contiene informazioni quali il primo e l'ultimo numero nella serie e la data di inizio.</span><span class="sxs-lookup"><span data-stu-id="1cb8e-112">The number series line contains information such as the first and last number in the series and the starting date.</span></span> <span data-ttu-id="1cb8e-113">È possibile impostare più righe di numerazione per codice di numerazione, con una diversa data di inizio per ogni riga.</span><span class="sxs-lookup"><span data-stu-id="1cb8e-113">You can set up more than one number series line per number series code, with a different starting date for each line.</span></span> <span data-ttu-id="1cb8e-114">Le numerazioni verranno utilizzate consecutivamente, avviando ciascuna alla rispettiva data di inizio.</span><span class="sxs-lookup"><span data-stu-id="1cb8e-114">The series will be used consecutively, starting each series on the respective starting date.</span></span>

<span data-ttu-id="1cb8e-115">Se si desidera utilizzare più codici di numerazione per un tipo di anagrafica, ad esempio per utilizzare una numerazione diversa per diverse categorie di articoli, è possibile utilizzare relazioni tra numerazioni.</span><span class="sxs-lookup"><span data-stu-id="1cb8e-115">If you want to use more than one number series code for one type of master data - for example, if you want to use different number series for different categories of items - you can use number series relationships.</span></span>

<span data-ttu-id="1cb8e-116">Oltre ai numeri assegnati manualmente o tramite l'utilizzo del sistema di numerazione, a tutte le transazioni (movimenti contabili) vengono automaticamente assegnati numeri consecutivi.</span><span class="sxs-lookup"><span data-stu-id="1cb8e-116">In addition to the numbers that you assign manually or by use of the numbering system, all transactions (ledger entries) are automatically assigned consecutive numbers.</span></span> <span data-ttu-id="1cb8e-117">Tali numeri possono essere visualizzati nel campo **N. movimento**</span><span class="sxs-lookup"><span data-stu-id="1cb8e-117">These numbers can be seen in the **Entry No.**</span></span> <span data-ttu-id="1cb8e-118">in tutte le finestre dei movimenti contabili.</span><span class="sxs-lookup"><span data-stu-id="1cb8e-118">field in all the ledger entry windows.</span></span> <span data-ttu-id="1cb8e-119">Non è possibile modificare o eliminare tali numeri.</span><span class="sxs-lookup"><span data-stu-id="1cb8e-119">You cannot modify or delete these numbers.</span></span>

## <a name="to-create-relationships-between-number-series"></a><span data-ttu-id="1cb8e-120">Per creare relazioni tra numerazioni</span><span class="sxs-lookup"><span data-stu-id="1cb8e-120">To create relationships between number series</span></span>
<span data-ttu-id="1cb8e-121">È possibile creare relazioni tra codici di numero di serie se ne sono stati impostati più di uno per lo stesso tipo di informazione o transazione di base.</span><span class="sxs-lookup"><span data-stu-id="1cb8e-121">If you have set up more than one number series code for the same kind of basic information or transactions, you can create relationships between the codes.</span></span> <span data-ttu-id="1cb8e-122">Questa funzione può essere utile per selezionare il codice corretto, al momento di utilizzare un numero.</span><span class="sxs-lookup"><span data-stu-id="1cb8e-122">This feature can assist you in deciding among the codes when you use a number.</span></span>

1. <span data-ttu-id="1cb8e-123">Nell'angolo superiore destro, scegliere l'icona **Cerca pagina o report**, immettere **Nr. serie**, quindi scegliere il collegamento correlato.</span><span class="sxs-lookup"><span data-stu-id="1cb8e-123">In the top right corner, choose the **Search for Page or Report** icon, enter **No. Series**, and then choose the related link.</span></span>
2. <span data-ttu-id="1cb8e-124">Selezionare la riga contenente la numerazione per la quale si desidera creare delle relazioni, quindi scegliere **Relazioni**.</span><span class="sxs-lookup"><span data-stu-id="1cb8e-124">Select the line with the number series you want to create relationships for and then choose **Relationships**.</span></span>
3. <span data-ttu-id="1cb8e-125">Nel campo **Codice serie** immettere il codice della numerazione che si desidera associare alla serie selezionata nel passaggio 2.</span><span class="sxs-lookup"><span data-stu-id="1cb8e-125">In the **Series Code** field, enter the code for the number series that you want to relate to the series you selected in step 2.</span></span>
4. <span data-ttu-id="1cb8e-126">Aggiungere una riga per ogni codice che si desidera associare alla numerazione selezionata.</span><span class="sxs-lookup"><span data-stu-id="1cb8e-126">Add a line for each code that you want to relate to the selected number series.</span></span>
5. <span data-ttu-id="1cb8e-127">Chiudere la finestra.</span><span class="sxs-lookup"><span data-stu-id="1cb8e-127">Close the window.</span></span>

<span data-ttu-id="1cb8e-128">Ogni volta che verrà impostato un elemento che richiede un numero, è ora possibile utilizzare le relazioni che sono state create per selezionare la numerazione corretta tra quelle poste in relazione.</span><span class="sxs-lookup"><span data-stu-id="1cb8e-128">Now when you set up something that requires a number, you can use the relationships you created to select among the related number series.</span></span>

## <a name="see-also"></a><span data-ttu-id="1cb8e-129">Vedi anche</span><span class="sxs-lookup"><span data-stu-id="1cb8e-129">See Also</span></span>
[<span data-ttu-id="1cb8e-130">Utilizzare Dynamics NAV</span><span class="sxs-lookup"><span data-stu-id="1cb8e-130">Work with Dynamics NAV</span></span>](ui-work-product.md)

