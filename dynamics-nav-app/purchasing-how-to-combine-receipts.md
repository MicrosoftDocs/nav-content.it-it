---
title: Come cumulare i carichi
description: "Se si desidera fatturare più di un carico di acquisto per volta, utilizzare la funzione Cumula carichi."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/14/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 10749dc8d8d692d94c5405fbb0a4a965d482f013
ms.contentlocale: it-it
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-combine-receipts-on-a-single-invoice"></a>Procedura: Combinare i carichi in una singola fattura
Se si desidera fatturare più di un carico di acquisto per volta, utilizzare la funzione **Cumula carichi**.  

Prima di creare un carico di acquisto cumulato, è necessario che venga registrato più di un carico per lo stesso fornitore nella stessa valuta. In altri termini, è necessario compilare due o più ordini di acquisto e registrarli come ricevuti, ma non fatturati.  

Quando i carichi di acquisto vengono cumulati in una fattura e registrati, viene creata una fattura di acquisto registrata per le righe fatturate. Il campo **Quantità fatturata** dell'ordine di acquisto o dell'ordine di acquisto programmato di origine viene aggiornato in base alla quantità fatturata. Tuttavia, il documento di acquisto originale non viene eliminato, anche se è stato completamente ricevuto e fatturato; è necessario quindi eliminare il documento di acquisto manualmente.  

## <a name="to-combine-receipts"></a>Per cumulare i carichi  
1. Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **Fatture di acquisto**, quindi scegliere il collegamento correlato.  
2. Scegliere l'azione **Nuovo**. Per ulteriori informazioni, vedere [Procedura: Registrare gli acquisti](purchasing-how-record-purchases.md).  
3. Nella Scheda dettaglio **Righe** scegliere l'azione **Prendi righe di carico**.  
4. Selezionare più righe di carico che si desidera includere nella fattura.  

    Se è stata selezionata una riga di carico non corretta o si desidera effettuare di nuovo la selezione, eliminare semplicemente le righe nella fattura di acquisto ed eseguire nuovamente la funzione **Prendi righe di carico**.  
5. Per registrare la fattura scegliere l'azione **Registra**.  

## <a name="to-remove-open-purchase-orders-after-combined-receipt-posting"></a>Per rimuovere ordini di acquisto aperti dopo la registrazione del carico cumulativa  
1. Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **Elimina ordini acquisto fatturati**, quindi scegliere il collegamento correlato.  
2. Compilare i campi, se necessario. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)].
3. Scegliere il pulsante **OK**.  

In alternativa, eliminare i singoli ordini manualmente.

Ripetere i passaggi da 1 a 3 per tutti gli altri documenti interessati, ad esempio gli ordini di acquisto programmati.

## <a name="see-also"></a>Vedi anche  
[Acquisti](purchasing-manage-purchasing.md)  
[Utilizzo di [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

