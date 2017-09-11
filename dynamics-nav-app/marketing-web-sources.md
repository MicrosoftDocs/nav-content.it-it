---
title: "Impostare le origini Web per le società contatto"
author: edupont04
ms.custom: na
ms.date: 09/16/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 6b60b1344a1e18ad91863046110df880f75f7c04
ms.openlocfilehash: eeb05b22a14917d759dadfe29957568baea6db34
ms.contentlocale: it-it
ms.lasthandoff: 07/19/2017

---
# <a name="set-up-web-sources-for-contact-companies"></a><span data-ttu-id="8a320-102">Impostare le origini Web per le società contatto</span><span class="sxs-lookup"><span data-stu-id="8a320-102">Set Up Web Sources for Contact Companies</span></span>
<span data-ttu-id="8a320-103">È possibile utilizzare le origini Web con le società contatto per identificare, ad esempio, motori di ricerca e siti Web dove effettuare la ricerca di informazioni sui contatti.</span><span class="sxs-lookup"><span data-stu-id="8a320-103">You can use web sources with your contact companies to identify, for example, search engines and web sites, on the Internet that you want to use to search for information about the contacts.</span></span> <span data-ttu-id="8a320-104">Quando si assegna un'origine Web, specificare il motore di ricerca e la parola di ricerca che saranno utilizzati per individuare le informazioni richieste.</span><span class="sxs-lookup"><span data-stu-id="8a320-104">When assigning web sources, you specify which search engine and search word the application will use to find the requested information.</span></span>

<span data-ttu-id="8a320-105">L'utilizzo delle origini Web nei contatti è un processo a due passaggi.</span><span class="sxs-lookup"><span data-stu-id="8a320-105">Using web sources on contacts is a two-step process.</span></span> <span data-ttu-id="8a320-106">Innanzitutto, occorre definire il codice origine Web.</span><span class="sxs-lookup"><span data-stu-id="8a320-106">First, you define the web source code.</span></span> <span data-ttu-id="8a320-107">Questo passaggio deve essere eseguito una sola volta per ogni origine Web.</span><span class="sxs-lookup"><span data-stu-id="8a320-107">You only have to perform this step one time for each web source.</span></span> <span data-ttu-id="8a320-108">Dopo aver creato un codice origine Web, è possibile iniziare ad assegnarlo ai contatti.</span><span class="sxs-lookup"><span data-stu-id="8a320-108">Once you have a web source code, you can start to assign the code to contact persons.</span></span>

## <a name="define-a-web-source-code"></a><span data-ttu-id="8a320-109">Definire un codice origine Web</span><span class="sxs-lookup"><span data-stu-id="8a320-109">Define a Web Source Code</span></span>
1. <span data-ttu-id="8a320-110">Nell'angolo superiore destro, scegliere l'icona **Cerca pagina o report**, immettere **Origini Web**, quindi scegliere il collegamento correlato.</span><span class="sxs-lookup"><span data-stu-id="8a320-110">In the top right corner, choose the **Search for Page or Report** icon, enter **Web Sources**, and then choose the related link.</span></span>
2. <span data-ttu-id="8a320-111">Scegliere l'azione **Nuovo**.</span><span class="sxs-lookup"><span data-stu-id="8a320-111">Choose the **New** actions.</span></span>
3. <span data-ttu-id="8a320-112">Compilare i campi **Codice**, **Descrizione** e **URL**.</span><span class="sxs-lookup"><span data-stu-id="8a320-112">Fill in the **Code**, **Description**, and **URL** fields.</span></span>

  <span data-ttu-id="8a320-113">Nel campo **URL** immettere %1 per inserire un segnaposto per una parola di ricerca nell'URL.</span><span class="sxs-lookup"><span data-stu-id="8a320-113">Type %1 in the **URL** field to insert a placeholder for a search word in the URL.</span></span> <span data-ttu-id="8a320-114">Quando si apre l'origine Web da un contatto, %1 verrà automaticamente sostituito con la parola da ricercare (ad esempio il nome della società) inserita nella finestra **Origini Web contatto**.</span><span class="sxs-lookup"><span data-stu-id="8a320-114">When you launch the web source from a contact, the %1 is replaced with the search word, for example, the name of the company that you have entered in the **Contact Web Sources** window.</span></span>

<span data-ttu-id="8a320-115">Ripetere tali passaggi per impostare altre origini Web.</span><span class="sxs-lookup"><span data-stu-id="8a320-115">Repeat these steps to set up as many web sources as you want.</span></span>

## <a name="assign-web-sources-to-a-contact-company"></a><span data-ttu-id="8a320-116">Assegnare origini Web a una società contatto</span><span class="sxs-lookup"><span data-stu-id="8a320-116">Assign Web Sources to a Contact Company</span></span>
<span data-ttu-id="8a320-117">Quando si assegna un'origine Web, specificare il motore di ricerca e la parola di ricerca che saranno utilizzati per individuare le informazioni richieste.</span><span class="sxs-lookup"><span data-stu-id="8a320-117">When assigning web sources, you specify which search engine and search word that the application will use to find the requested information.</span></span>

1. <span data-ttu-id="8a320-118">Aprire il contatto.</span><span class="sxs-lookup"><span data-stu-id="8a320-118">Open the contact.</span></span>
2. <span data-ttu-id="8a320-119">Scegliere l'azione **Società**, quindi l'azione **Origini Web**.</span><span class="sxs-lookup"><span data-stu-id="8a320-119">Choose the **Company** action, and then choose the **Web Sources** action.</span></span> <span data-ttu-id="8a320-120">Verrà visualizzata la finestra **Origine Web contatto**.</span><span class="sxs-lookup"><span data-stu-id="8a320-120">The **Contact Web Sources** window opens.</span></span>
3. <span data-ttu-id="8a320-121">Nel campo **Codice origine Web** scegliere l'origine Web che si desidera assegnare.</span><span class="sxs-lookup"><span data-stu-id="8a320-121">In the **Web Source Code** field, choose the web source you want to assign.</span></span>
4. <span data-ttu-id="8a320-122">Nel campo **Parola ricerca** inserire la parola ricerca che verrà utilizzata per individuare le informazioni.</span><span class="sxs-lookup"><span data-stu-id="8a320-122">In the **Search Word** field, enter the search word that you want to use to find the information.</span></span>

<span data-ttu-id="8a320-123">Ripetere tali passaggi per assegnare altre origini Web.</span><span class="sxs-lookup"><span data-stu-id="8a320-123">Repeat these steps to assign as many web sources as you want.</span></span>

<span data-ttu-id="8a320-124">È inoltre possibile assegnare l'origine Web dalla finestra **Lista contatti** seguendo la stessa procedura.</span><span class="sxs-lookup"><span data-stu-id="8a320-124">You can also assign web sources from the **Contact List** window by following the same procedure.</span></span>

##<a name="see-also"></a><span data-ttu-id="8a320-125">Vedi anche</span><span class="sxs-lookup"><span data-stu-id="8a320-125">See Also</span></span>
[<span data-ttu-id="8a320-126">Creare società contatto</span><span class="sxs-lookup"><span data-stu-id="8a320-126">Create Contact Companies</span></span>](marketing-create-contact-companies.md)

