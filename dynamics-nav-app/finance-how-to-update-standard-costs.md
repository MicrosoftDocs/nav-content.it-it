---
title: Come aggiornare i costi standard
description: "Periodicamente è necessario aggiornare i costi standard dei componenti ed eseguire il rollup dei nuovi costi nell'articolo padre."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/09/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: b9b1f062ee6009f34698ea2cf33bc25bdd5b11e4
ms.openlocfilehash: dd2bb16af611be7f7720fdf07eb65fd268aba039
ms.contentlocale: it-it
ms.lasthandoff: 10/23/2017

---
# <a name="how-to-update-standard-costs"></a>Procedura: Aggiornare i costi standard
Periodicamente è necessario aggiornare i costi standard dei componenti ed eseguire il rollup dei nuovi costi nell'articolo padre. Il processo in genere è costituito dai quattro passaggi seguenti:  

1.  Aggiornare i costi ai livelli di capacità e componente. Per ulteriori informazioni, vedere il processo batch **Suggerisci costo std. articolo**.  
2.  Consolidamento e roll up dei costi dei componenti e della capacità per calcolare il costo totale di produzione o di assemblaggio degli articoli.  
3.  Implementare i costi standard che vengono registrati quando si eseguono i processi batch precedenti. I costi standard non saranno effettivi finché non verranno implementati. Per ulteriori informazioni, vedere Implementare modifiche costo std..  
4.  Implementare le modifiche per aggiornare il campo **Costo unitario** nella scheda articolo ed eseguire la rivalutazione di magazzino. Per ulteriori informazioni, vedere [Procedura: Rivalutare il magazzino](inventory-how-revalue-inventory.md).  

Per ulteriori informazioni, vedere [Informazioni sul calcolo del costo standard](finance-about-calculating-standard-cost.md).  
## <a name="to-update-standard-costs"></a>Per aggiornare i costi standard  
1.  Eseguire il processo batch **Rettifica costo - Movimenti articoli**.  
2.  Eseguire il processo batch **Registra costo magazzino in C/G**.  
3.  Aprire il **Prospetto costo standard** e utilizzare una o più delle funzioni seguenti:  

    1.  Eseguire il processo batch **Suggerisci costo std. articolo**.  
    2.  Analizzare i risultati e apportare le modifiche necessarie.  
    3.  Eseguire il processo batch **Suggerisci costo standard capacità**.  
    4.  Analizzare i risultati e apportare le modifiche necessarie.
    5. Eseguire il processo batch **Roll up del costo standard**.
    6.  Analizzare i risultati e apportare le modifiche necessarie.
    7.  Eseguire il processo batch **Implementa modifiche costo std.**  
4.  Esaminare e registrare la finestra **Registrazioni rivalutazioni**, che è stata popolata con le voci dei passaggi precedenti del processo.  

## <a name="see-also"></a>Vedi anche  
 [Informazioni sul calcolo del costo standard](finance-about-calculating-standard-cost.md)   
 [Gestione dei costi di magazzino](finance-manage-inventory-costs.md)   
 [Dettagli di progettazione: Metodi di costing](design-details-costing-methods.md) [[Contabilità](finance.md)]  
 [Utilizzo di [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)  

