---
title: Impostare o modificare il piano dei conti
author: edupont04
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 6b60b1344a1e18ad91863046110df880f75f7c04
ms.openlocfilehash: 2a2f1f2ec3ac5bdd935ec19c11d74e16bdee7686
ms.contentlocale: it-it
ms.lasthandoff: 07/19/2017

---

# <a name="set-up-or-change-the-chart-of-accounts"></a><span data-ttu-id="7fba1-102">Impostare o modificare il piano dei conti</span><span class="sxs-lookup"><span data-stu-id="7fba1-102">Set Up or Change the Chart of Accounts</span></span>
<span data-ttu-id="7fba1-103">Il piano dei conti mostra i conti di contabilità che memorizzano i dati finanziari.</span><span class="sxs-lookup"><span data-stu-id="7fba1-103">The chart of accounts shows the ledger accounts that store your financial data.</span></span> <span data-ttu-id="7fba1-104">Dynamics NAV include un piano dei conti standard pronto per supportare l'azienda.</span><span class="sxs-lookup"><span data-stu-id="7fba1-104">Dynamics NAV includes a standard chart of accounts that is ready to support your business.</span></span>
<span data-ttu-id="7fba1-105">Tuttavia, è possibile modificare i conti predefinti ed è possibile aggiungere nuovi conti.</span><span class="sxs-lookup"><span data-stu-id="7fba1-105">However, you can change the default accounts, and you can add new accounts.</span></span>  

## <a name="adding-or-changing-accounts"></a><span data-ttu-id="7fba1-106">Aggiungere o modificare i conti</span><span class="sxs-lookup"><span data-stu-id="7fba1-106">Adding or Changing Accounts</span></span>
<span data-ttu-id="7fba1-107">Nel piano dei conti, è possibile aprire ogni conto C/G e aggiungere o modificare le impostazioni.</span><span class="sxs-lookup"><span data-stu-id="7fba1-107">From the chart of accounts, you can open each G/L account and add or change settings.</span></span>

<span data-ttu-id="7fba1-108">**Nota**: è possibile eliminare un conto di contabilità generale.</span><span class="sxs-lookup"><span data-stu-id="7fba1-108">**Note**: You can delete a general ledger account.</span></span> <span data-ttu-id="7fba1-109">Tuttavia, prima che venga eliminato, è necessario soddisfare le seguenti condizioni:</span><span class="sxs-lookup"><span data-stu-id="7fba1-109">However, before you delete it, the following must be true:</span></span>  
- <span data-ttu-id="7fba1-110">Il saldo nel conto deve essere pari a zero.</span><span class="sxs-lookup"><span data-stu-id="7fba1-110">The balance on the account must be zero.</span></span>  
- <span data-ttu-id="7fba1-111">Nel campo **Consenti Eliminaz. Conti C/G Anteriori a** della finestra **Setup Contabilità Generale** deve essere impostata una data ed è necessario che il conto non includa movimenti contabili in tale data o dopo tale data.</span><span class="sxs-lookup"><span data-stu-id="7fba1-111">The **Allow G/L Acc. Deletion Before** field must be set in the **General Ledger Setup** window, and the account must not have ledger entries on or after that date.</span></span>  
- <span data-ttu-id="7fba1-112">Se il campo **Verifica Uso Conti C/G** della finestra **Setup Contabilità Generale** è selezionato, il conto non deve essere utilizzato in tutte le categorie di registrazione o impostazioni delle registrazioni.</span><span class="sxs-lookup"><span data-stu-id="7fba1-112">If the **Check G/L Account Usage** field in the **General Ledger Setup** window is selected, then the account must not be used in any posting groups or posting setup.</span></span>  

<span data-ttu-id="7fba1-113">Dynamics NAV impedirà di eliminare un conto di contabilità generale che memorizza dati necessari per il piano dei conti.</span><span class="sxs-lookup"><span data-stu-id="7fba1-113">Dynamics NAV will prevent you from deleting a general ledger account that stores data that is needed in the chart of accounts.</span></span>  

##<a name="see-also"></a><span data-ttu-id="7fba1-114">Vedi anche</span><span class="sxs-lookup"><span data-stu-id="7fba1-114">See Also</span></span>  
[<span data-ttu-id="7fba1-115">Contabilità generale e piano dei conti</span><span class="sxs-lookup"><span data-stu-id="7fba1-115">The General Ledger and the Chart of Accounts</span></span>](finance-setup-general-ledger.md)  
[<span data-ttu-id="7fba1-116">Gestire i conti correnti bancari</span><span class="sxs-lookup"><span data-stu-id="7fba1-116">Manage Bank Accounts</span></span>](bank-manage-bank-accounts.md)  
[<span data-ttu-id="7fba1-117">Dimensioni</span><span class="sxs-lookup"><span data-stu-id="7fba1-117">Dimensions</span></span>](finance-setup-dimensions.md)  
[<span data-ttu-id="7fba1-118">Procedura: Utilizzare i codici GIFI in Canada</span><span class="sxs-lookup"><span data-stu-id="7fba1-118">How to: Work With GIFI Codes in Canada</span></span>](ca-finance-setup-work-GiFI-codes.md)

