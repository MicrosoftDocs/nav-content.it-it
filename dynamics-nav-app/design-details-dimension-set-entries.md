---
title: Dettagli di progettazione - Movimenti set di dimensioni
description: "Questa documentazione fornisce informazioni tecniche dettagliate sui concetti e sui principi utilizzati per riprogettare la funzionalità di archiviazione e registrazione dei movimenti dimensioni."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: design, dimensions, codeunit
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 1dfba8b14019991c95f40ffd5f7fbaed5df414eb
ms.openlocfilehash: 6b34fde01e35cdd3178a28a787397f52a43eefab
ms.contentlocale: it-it
ms.lasthandoff: 12/01/2017

---
# <a name="design-details-dimension-set-entries"></a><span data-ttu-id="46837-103">Dettagli di progettazione: Movimenti set di dimensioni</span><span class="sxs-lookup"><span data-stu-id="46837-103">Design Details: Dimension Set Entries</span></span>
<span data-ttu-id="46837-104">Questa documentazione fornisce informazioni tecniche dettagliate sui concetti e sui principi utilizzati per riprogettare la funzionalità di archiviazione e registrazione dei movimenti dimensioni in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="46837-104">This documentation provides detailed technical insight into the concepts and principles that are used to redesign the dimension entry storing and posting feature in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span> <span data-ttu-id="46837-105">Viene innanzitutto illustrata una panoramica dei concetti alla base della riprogettazione.</span><span class="sxs-lookup"><span data-stu-id="46837-105">The documentation starts by describing conceptual overviews of the redesign.</span></span> <span data-ttu-id="46837-106">Viene quindi illustrata l'architettura tecnica per mostrare in che modo viene eseguita la riprogettazione.</span><span class="sxs-lookup"><span data-stu-id="46837-106">Then it explains the technical architecture to show how the redesign is made.</span></span> <span data-ttu-id="46837-107">Infine, vengono forniti esempi di codice per preparare l'utente alla migrazione e all'aggiornamento del codice di dimensione.</span><span class="sxs-lookup"><span data-stu-id="46837-107">Finally, it provides code examples to prepare you for dimension code migration and upgrade.</span></span>  

## <a name="in-this-section"></a><span data-ttu-id="46837-108">In questa sezione</span><span class="sxs-lookup"><span data-stu-id="46837-108">In This Section</span></span>  
[<span data-ttu-id="46837-109">Sintesi movimenti set di dimensioni</span><span class="sxs-lookup"><span data-stu-id="46837-109">Dimension Set Entries Overview</span></span>](design-details-dimension-set-entries-overview.md)  
[<span data-ttu-id="46837-110">Dettagli di progettazione: Ricerca delle combinazioni di dimensione</span><span class="sxs-lookup"><span data-stu-id="46837-110">Design Details: Searching for Dimension Combinations</span></span>](design-details-searching-for-dimension-combinations.md)  
[<span data-ttu-id="46837-111">Dettagli di progettazione: Struttura della tabella</span><span class="sxs-lookup"><span data-stu-id="46837-111">Design Details: Table Structure</span></span>](design-details-table-structure.md)  
[<span data-ttu-id="46837-112">Dettagli di progettazione: Gestione dimensioni della codeunit 408</span><span class="sxs-lookup"><span data-stu-id="46837-112">Design Details: Codeunit 408 Dimension Management</span></span>](design-details-codeunit-408-dimension-management.md)  
[<span data-ttu-id="46837-113">Dettagli di progettazione: Esempi di codice dei modelli modificati nelle modifiche</span><span class="sxs-lookup"><span data-stu-id="46837-113">Design Details: Code Examples of Changed Patterns in Modifications</span></span>](design-details-code-examples-of-changed-patterns-in-modifications.md)

