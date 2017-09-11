---
title: "Impostare relazioni d'affari nelle società contatto"
author: jswymer
ms.custom: na
ms.date: 09/16/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 6b60b1344a1e18ad91863046110df880f75f7c04
ms.openlocfilehash: 6616473a00e85e52648713d7e067f4b3b72caecf
ms.contentlocale: it-it
ms.lasthandoff: 07/19/2017

---
# <a name="set-up-business-relations-on-contact-companies"></a><span data-ttu-id="5ee12-102">Impostare relazioni d'affari nelle società contatto</span><span class="sxs-lookup"><span data-stu-id="5ee12-102">Set Up Business Relations on Contact Companies</span></span>
<span data-ttu-id="5ee12-103">È possibile utilizzare le relazioni d'affari vengono utilizzate per indicare il tipo di relazione commerciale che intercorre con i contatti, ad esempio potenziale cliente, banca, consulente e fornitore di servizi e così via.</span><span class="sxs-lookup"><span data-stu-id="5ee12-103">You can use business relations to indicate the business relationship you have with your contacts, for example, a prospect, bank, consultant, service supplier, and so on.</span></span>

<span data-ttu-id="5ee12-104">L'utilizzo delle relazioni d'affari nei contatti è un processo a due passaggi.</span><span class="sxs-lookup"><span data-stu-id="5ee12-104">Using business relations on contacts is a two-step process.</span></span> <span data-ttu-id="5ee12-105">Innanzitutto, occorre definire il codice relazioni d'affari.</span><span class="sxs-lookup"><span data-stu-id="5ee12-105">First, you define the business relation code.</span></span> <span data-ttu-id="5ee12-106">Questo passaggio deve essere eseguito una sola volta per ogni relazione d'affari.</span><span class="sxs-lookup"><span data-stu-id="5ee12-106">You only have to perform this step one time for each business relation.</span></span> <span data-ttu-id="5ee12-107">Dopo aver creato un codice di relazione d'affari, è possibile iniziare ad assegnarlo alle società.</span><span class="sxs-lookup"><span data-stu-id="5ee12-107">Once you have a business relation code, you can start to assign the code to contact companies.</span></span>

<span data-ttu-id="5ee12-108">**Nota**: se si prede di sincronizzare i contatti con fornitori, clienti o conti correnti bancari in altre sezioni dell'applicazione, è consigliabile impostare una relazione d'affari.</span><span class="sxs-lookup"><span data-stu-id="5ee12-108">**Note**: If you plan to synchronize your contacts with vendors, customers, or bank accounts in other parts of the application, you may want to set up a business relation for them.</span></span>

## <a name="define-a-business-relation-code"></a><span data-ttu-id="5ee12-109">Definire un codice relaz. d'affari</span><span class="sxs-lookup"><span data-stu-id="5ee12-109">Define a Business Relation Code</span></span>
<span data-ttu-id="5ee12-110">Il codice relazione d'affari definisce una categoria o un tipo della relazione d'affari, ad esempio BANCA o LEGGE.</span><span class="sxs-lookup"><span data-stu-id="5ee12-110">The business relation code defines a category or type of the business relationship, such as BANK or LAW.</span></span> <span data-ttu-id="5ee12-111">È possibile impostare più codici di relazione d'affari.</span><span class="sxs-lookup"><span data-stu-id="5ee12-111">You can have several business relation codes.</span></span> <span data-ttu-id="5ee12-112">Per definire la relazione d'affari, utilizzare la finestra **Relazioni d'affari**.</span><span class="sxs-lookup"><span data-stu-id="5ee12-112">To define the business relation, you use the **Business Relations** window.</span></span>

1. <span data-ttu-id="5ee12-113">Nell'angolo superiore destro, scegliere l'icona **Cerca pagina o report**, immettere **Relazioni d'affari**, quindi scegliere il collegamento correlato.</span><span class="sxs-lookup"><span data-stu-id="5ee12-113">In the top right corner, choose the **Search for Page or Report** icon, enter **Business Relations**, and then choose the related link.</span></span>
2. <span data-ttu-id="5ee12-114">Selezionare l'azione **Nuovo** e immettere un codice e una descrizione.</span><span class="sxs-lookup"><span data-stu-id="5ee12-114">Choose the **New** action, and fill in a code and description.</span></span> <span data-ttu-id="5ee12-115">Il codice può avere un massimo di 11 caratteri e può essere qualsiasi combinazione di numeri o lettere.</span><span class="sxs-lookup"><span data-stu-id="5ee12-115">The code can be a maximum of 11 characters, and can be any combination of numbers and letters.</span></span>

## <a name="assign-business-relations-to-a-contact"></a><span data-ttu-id="5ee12-116">Assegnare relazioni d'affari ai contatti</span><span class="sxs-lookup"><span data-stu-id="5ee12-116">Assign Business Relations to a Contact</span></span>
<span data-ttu-id="5ee12-117">Non è possibile assegnare relazioni d'affari a un contatto, ma solo alle società.</span><span class="sxs-lookup"><span data-stu-id="5ee12-117">You cannot assign business relations to a contact person - only companies.</span></span>

1. <span data-ttu-id="5ee12-118">Aprire il contatto.</span><span class="sxs-lookup"><span data-stu-id="5ee12-118">Open the contact.</span></span>
2. <span data-ttu-id="5ee12-119">Scegliere l'azione **Società**, quindi l'azione **Relazioni d'affari**.</span><span class="sxs-lookup"><span data-stu-id="5ee12-119">Choose the **Company** action, and then the **Business Relations** action.</span></span>

    <span data-ttu-id="5ee12-120">Verrà aperta la finestra **Relazioni d'affari contatto**.</span><span class="sxs-lookup"><span data-stu-id="5ee12-120">The **Contact Business Relations** window opens.</span></span>
3. <span data-ttu-id="5ee12-121">Nel campo **Codice relazione d'affari** selezionare la relazione d'affari da assegnare.</span><span class="sxs-lookup"><span data-stu-id="5ee12-121">In the **Business Relation Code** field, select the business relation you want to assign.</span></span>

<span data-ttu-id="5ee12-122">Ripetere questi passaggi per assegnare altre relazioni d'affari.</span><span class="sxs-lookup"><span data-stu-id="5ee12-122">Repeat these steps to assign as many business relations as you want.</span></span> <span data-ttu-id="5ee12-123">È inoltre possibile assegnare altre relazioni d'affari dalla lista Contatti seguendo la stessa procedura.</span><span class="sxs-lookup"><span data-stu-id="5ee12-123">You can also assign business relations from the contact list by following the same procedure.</span></span>

<span data-ttu-id="5ee12-124">Il numero di relazioni d'affari assegnate al contatto viene visualizzato nel campo **Nr. relazione d'affari** nella sezione **Segmentazione** nella finestra **Contatto**.</span><span class="sxs-lookup"><span data-stu-id="5ee12-124">The number of business relations you have assigned to the contact is displayed in the **No. of Business Relations** field in the **Segmentation** section in the **Contact** window.</span></span>

<span data-ttu-id="5ee12-125">Una volta assegnate le relazioni d'affari ai contatti, è possibile utilizzare queste informazioni per selezionare i contatti per i segmenti.</span><span class="sxs-lookup"><span data-stu-id="5ee12-125">After you have assigned business relations to your contacts, you can use this information to select contacts for your segments.</span></span> <span data-ttu-id="5ee12-126">Per ulteriori informazioni, vedere [Procedura: aggiungere contatti ai segmenti](marketing-add-contact-segment.md).</span><span class="sxs-lookup"><span data-stu-id="5ee12-126">For more information, see [How to: Add Contacts to Segments](marketing-add-contact-segment.md).</span></span>

##<a name="see-also"></a><span data-ttu-id="5ee12-127">Vedi anche</span><span class="sxs-lookup"><span data-stu-id="5ee12-127">See Also</span></span>
[<span data-ttu-id="5ee12-128">Creare società contatto</span><span class="sxs-lookup"><span data-stu-id="5ee12-128">Create Contact Companies</span></span>](marketing-create-contact-companies.md)

