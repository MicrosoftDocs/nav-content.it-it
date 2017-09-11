---
title: Personalizzazione di Dynamics NAV utilizzando le estensioni
author: edupont04
ms.custom: na
ms.date: 09/23/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 6b60b1344a1e18ad91863046110df880f75f7c04
ms.openlocfilehash: cc832772a255c7c801a7b956c74da827caca3765
ms.contentlocale: it-it
ms.lasthandoff: 07/19/2017

---

# <a name="customizing-dynamics-nav-using-extensions"></a><span data-ttu-id="4b604-102">Personalizzazione di Dynamics NAV utilizzando le estensioni</span><span class="sxs-lookup"><span data-stu-id="4b604-102">Customizing Dynamics NAV Using Extensions</span></span>
<span data-ttu-id="4b604-103">È possibile modificare Dynamics NAV installando estensioni che aggiungono funzionalità, modificano il comportamento o permettono di accedere a nuovi servizi online.</span><span class="sxs-lookup"><span data-stu-id="4b604-103">You can change Dynamics NAV by installing extensions that add functionality, change behavior, or give you access to new online services, for example.</span></span>
<span data-ttu-id="4b604-104">La prima volta che si avvia Dynamics NAV, alcune estensioni risultano già installate.</span><span class="sxs-lookup"><span data-stu-id="4b604-104">When you first launch Dynamics NAV, some extensions are already installed for you.</span></span> <span data-ttu-id="4b604-105">Con il tempo verranno rese disponibili altre estensioni e sarà possibile scegliere se installarle o meno.</span><span class="sxs-lookup"><span data-stu-id="4b604-105">Over time, more extensions can be made available to you, and you can then choose if you want to use the extension or not.</span></span>

<span data-ttu-id="4b604-106">Ad esempio, Microsoft fornisce un'estensione che consente l'integrazione con PayPal Payments Standard.</span><span class="sxs-lookup"><span data-stu-id="4b604-106">For example, Microsoft provides an extension that provides integration with PayPal Payments Standard.</span></span> <span data-ttu-id="4b604-107">Questa estensione è installata per impostazione predefinita.</span><span class="sxs-lookup"><span data-stu-id="4b604-107">This extension is installed by default.</span></span>
<span data-ttu-id="4b604-108">Se tuttavia diventa disponibile un'altra estensione che offre l'integrazione con un altro servizio di pagamento, è possibile installare la nuova estensione e scegliere quale dei due servizi utilizzare.</span><span class="sxs-lookup"><span data-stu-id="4b604-108">But if another extension is made available that offers integration with another payment service, you can install the new extension and then choose which of the two services to use.</span></span>  

<span data-ttu-id="4b604-109">Le estensioni vengono gestite nella finestra **Gestione estensioni**.</span><span class="sxs-lookup"><span data-stu-id="4b604-109">You manage the extensions in the **Extension Management** window.</span></span> <span data-ttu-id="4b604-110">È possibile accedere a questa finestra dalla home page.</span><span class="sxs-lookup"><span data-stu-id="4b604-110">You can access this window from Home.</span></span> <span data-ttu-id="4b604-111">In alternativa, scegliere l'icona **Cerca pagina o report** nell'angolo superiore destro, immettere **Estensione**, quindi scegliere il collegamento correlato.</span><span class="sxs-lookup"><span data-stu-id="4b604-111">Alternatively, choose the **Search for Page or Report** icon in the top right corner, enter **Extension**, and then choose the related link.</span></span>   

## <a name="installing-an-extension"></a><span data-ttu-id="4b604-112">Installazione di un'estensione</span><span class="sxs-lookup"><span data-stu-id="4b604-112">Installing an Extension</span></span>
<span data-ttu-id="4b604-113">Se le nuove estensioni vengono rese disponibili perché sono state installate nel server, verranno visualizzate nella finestra **Gestione estensioni**.</span><span class="sxs-lookup"><span data-stu-id="4b604-113">If new extensions are made available to you because they have been published to your server, they will be shown in the **Extension Management** window.</span></span> <span data-ttu-id="4b604-114">Da qui, è possibile scegliere di installare o di disinstallare le estensioni.</span><span class="sxs-lookup"><span data-stu-id="4b604-114">From here, you can choose to install and uninstall extensions.</span></span>  

<span data-ttu-id="4b604-115">Se si sceglie un'estensione, è possibile leggerne una descrizione e accedere alla Guida dell'estensione per ottenere ulteriori informazioni.</span><span class="sxs-lookup"><span data-stu-id="4b604-115">If you choose an extension, you can read about what the extension does, and you can access Help for the extension to learn more.</span></span> <span data-ttu-id="4b604-116">Quando si sceglie di ottenere una interno, è necessario accettare le condizioni per l'utilizzo.</span><span class="sxs-lookup"><span data-stu-id="4b604-116">When you choose to get an extension, you must agree to the terms of use.</span></span>  

<span data-ttu-id="4b604-117">Quando si installa un'estensione, potrebbe essere necessario configurarla. Se ad esempio si intende utilizzare l'estensione **PayPal Payments Standard per Dynamics NAV** sarà necessario specificare un conto.</span><span class="sxs-lookup"><span data-stu-id="4b604-117">When you install an extension, you might have to set it up, such as specifying an account for use with the **PayPal Payments Standard for Dynamics NAV** extension.</span></span>
<span data-ttu-id="4b604-118">Altre estensioni aggiungono semplicemente dei campi a una pagina esistente oppure aggiungono una nuova pagina.</span><span class="sxs-lookup"><span data-stu-id="4b604-118">Other extensions simply add fields to an existing page, or they add a new page, for example.</span></span>   

<span data-ttu-id="4b604-119">Se si disinstalla un'estensione e successivamente si cambia idea, è possibile installarla di nuovo.</span><span class="sxs-lookup"><span data-stu-id="4b604-119">If you uninstall an extension, and you then change your mind, you can install it again.</span></span> <span data-ttu-id="4b604-120">Quando si disinstalla un'estensione che si sta utilizzando, i dati vengono mantenuti in modo da essere disponibili qualora la si reinstallasse.</span><span class="sxs-lookup"><span data-stu-id="4b604-120">When you uninstall an extension that you have been using, the data is preserved so that if you install the extension again, your data is still available.</span></span>  

<span data-ttu-id="4b604-121">Microsoft fornisce le seguenti estensioni:</span><span class="sxs-lookup"><span data-stu-id="4b604-121">Microsoft provides the following extensions:</span></span>  
- [<span data-ttu-id="4b604-122">PayPal Payments Standard</span><span class="sxs-lookup"><span data-stu-id="4b604-122">PayPal Payments Standard</span></span>](ui-extensions-paypal-payments-standard.md)  
- [<span data-ttu-id="4b604-123">Previsione vendite e magazzino</span><span class="sxs-lookup"><span data-stu-id="4b604-123">Sales and Inventory Forecast</span></span>](ui-extensions-sales-forecast.md)  

<span data-ttu-id="4b604-124">Altre estensioni sono inoltre disponibili per impostazione predefinita, in base al proprio paese.</span><span class="sxs-lookup"><span data-stu-id="4b604-124">Other extensions are also available by default, depending on your country/region.</span></span>

## <a name="see-also"></a><span data-ttu-id="4b604-125">Vedi anche</span><span class="sxs-lookup"><span data-stu-id="4b604-125">See Also</span></span>  
[<span data-ttu-id="4b604-126">Procedura: Abilitare i pagamenti clienti attraverso PayPal</span><span class="sxs-lookup"><span data-stu-id="4b604-126">How to: Enable Customer Payment Through PayPal</span></span>](sales-how-enable-customer-payments-paypal.md)  
[<span data-ttu-id="4b604-127">Benvenuto in Dynamics NAV</span><span class="sxs-lookup"><span data-stu-id="4b604-127">Welcome to Dynamics NAV</span></span>](across-get-started.md)  

