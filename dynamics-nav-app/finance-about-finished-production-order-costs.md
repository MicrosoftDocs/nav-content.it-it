---
title: Informazioni sui costi di un ordine di produzione chiuso
description: "La chiusura di un ordine di produzione è un'attività importante nel completamento del ciclo di vita del costing dell'articolo prodotto. I costi finali, inclusi gli scostamenti in un ambiente con costi standard, i valori effettivi in un ambiente con costi FIFO, medi o LIFO, vengono calcolati tramite il processo batch **Rettifica costo - Movimenti articoli**."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 09/06/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 6b6fd4fe1ba4bd279aacbca38bf953bce5a996fc
ms.contentlocale: it-it
ms.lasthandoff: 10/16/2017

---
# <a name="about-finished-production-order-costs"></a>Informazioni sui costi di un ordine di produzione chiuso
La chiusura di un ordine di produzione è un'attività importante nel completamento del ciclo di vita del costing dell'articolo prodotto. I costi finali, inclusi gli scostamenti in un ambiente con costi standard, i valori effettivi in un ambiente con costi FIFO, medi o LIFO, vengono calcolati tramite il processo batch **Rettifica costo - Movimenti articoli** che consente la riconciliazione finanziaria dei costi di produzione degli articoli. Affinché un ordine di produzione venga considerato per la rettifica del costo, lo stato deve essere impostato come **Completato**. È pertanto essenziale che, al completamento, lo stato di un ordine di produzione venga modificato in **Completato**.  

## <a name="example"></a>Esempio  
 In un ambiente di costi standard, quando si consuma materiale per produrre un articolo, detto semplicemente, il costo dell'articolo più i costi generali e di manodopera confluiscono nel WIP. Quando l'articolo viene prodotto, il WIP viene ridotto dell'importo del costo standard dell'articolo. In genere, questi costi netti non sono uguali a zero. Perché l'importo sia uguale a zero, è necessario eseguire il processo batch **Rettifica costo - Movimenti articoli**, notando che solo gli ordini di produzione con stato **Completato** verranno considerati per la rettifica.  

## <a name="see-also"></a>Vedi anche  
[Gestione dei costi di magazzino](finance-manage-inventory-costs.md)  
[Manufacturing](production-manage-manufacturing.md)  
[Utilizzo di [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

