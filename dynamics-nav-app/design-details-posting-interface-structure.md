---
title: Dettagli di progettazione - Struttura dell'interfaccia di registrazione
description: Questo argomento fornisce una sintesi delle procedure globali nella struttura dell'interfaccia di registrazione.
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: posting, interface, design
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: cc5efca8087bc24ab988ae592a9ba60e4caf46bb
ms.contentlocale: it-it
ms.lasthandoff: 10/16/2017

---
# <a name="design-details-posting-interface-structure"></a><span data-ttu-id="2eb61-103">Dettagli di progettazione: struttura dell'interfaccia di registrazione</span><span class="sxs-lookup"><span data-stu-id="2eb61-103">Design Details: Posting Interface Structure</span></span>
<span data-ttu-id="2eb61-104">Nella struttura dell'interfaccia di registrazione di [!INCLUDE[d365fin](includes/d365fin_md.md)] esistono diverse procedure globali che utilizzano la stessa struttura:</span><span class="sxs-lookup"><span data-stu-id="2eb61-104">In the [!INCLUDE[d365fin](includes/d365fin_md.md)] posting interface structure, there are several global procedures that use the same structure:</span></span>  
  
* <span data-ttu-id="2eb61-105">Codice della procedura di chiamata di RunWithoutCheck e di RunWithCheck – interfaccia generica di registrazione per riga registrazioni COGE.</span><span class="sxs-lookup"><span data-stu-id="2eb61-105">RunWithCheck and RunWithoutCheck call procedure Code – generic posting interface for Gen. Jnl Line.</span></span>  
* <span data-ttu-id="2eb61-106">CustPostApplyCustLedgEntry – registrare il collegamento del cliente, chiamato da codeunit 226 CustEntry- Collegare i movimenti registrati.</span><span class="sxs-lookup"><span data-stu-id="2eb61-106">CustPostApplyCustLedgEntry – post customer application, called from codeunit 226 CustEntry-Apply Posted Entries.</span></span>  
* <span data-ttu-id="2eb61-107">VendPostApplyVendLedgEntry – registrare il collegamento del fornitore, chiamato da codeunit 227 VendEntry- Collegare i movimenti registrati.</span><span class="sxs-lookup"><span data-stu-id="2eb61-107">VendPostApplyVendLedgEntry – post vendor application, called from codeunit 227 VendEntry-Apply Posted Entries.</span></span>  
* <span data-ttu-id="2eb61-108">UnapplyCustLedgEntry – registrare l'annullamento del collegamento del cliente, chiamato da codeunit 226 CustEntry- Collegare i movimenti registrati</span><span class="sxs-lookup"><span data-stu-id="2eb61-108">UnapplyCustLedgEntry – post unapply of customer application, called from codeunit 226 CustEntry-Apply Posted Entries</span></span>  
* <span data-ttu-id="2eb61-109">UnapplyVendLedgEntry – registrare l'annullamento del collegamento del fornitore, chiamato da codeunit 227 VendEntry- Collegare i movimenti registrati</span><span class="sxs-lookup"><span data-stu-id="2eb61-109">UnapplyVendLedgEntry – post unapply of vendor application, called from codeunit 227 VendEntry-Apply Posted Entries</span></span>  
  
## <a name="see-also"></a><span data-ttu-id="2eb61-110">Vedi anche</span><span class="sxs-lookup"><span data-stu-id="2eb61-110">See Also</span></span>  
[<span data-ttu-id="2eb61-111">Dettagli di progettazione: struttura del motore di registrazione</span><span class="sxs-lookup"><span data-stu-id="2eb61-111">Design Details: Posting Engine Structure</span></span>](design-details-posting-engine-structure.md)