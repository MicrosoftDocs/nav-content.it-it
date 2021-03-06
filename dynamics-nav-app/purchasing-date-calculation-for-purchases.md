---
title: Calcolo della data per gli acquisti
description: "Il programma calcola automaticamente la data in cui sarà necessario ordinare un articolo da avere in magazzino in una determinata data. Questa è la data in cui si può prevedere che gli articoli ordinati in una data particolare possano essere disponibili per il prelievo."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/10/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 3f3f87311f0971b2901852a9aa0c766c6c806190
ms.contentlocale: it-it
ms.lasthandoff: 10/16/2017

---
# <a name="date-calculation-for-purchases"></a>Calcolo della data per gli acquisti
[!INCLUDE[d365fin](includes/d365fin_md.md)] calcola automaticamente la data in cui sarà necessario ordinare un articolo da avere in magazzino in una determinata data. Questa è la data in cui si può prevedere che gli articoli ordinati in una data particolare possano essere disponibili per il prelievo.  

Se si specifica una data di carico richiesta nella testata di un ordine di acquisto, la data dell'ordine calcolata è la data in cui si deve effettuare l'ordine per ricevere gli articoli alla data richiesta. Quindi, la data in cui gli articoli saranno disponibili per il prelievo viene calcolata e immessa nel campo **Data carico prevista**.  

Se non si specifica una data di carico richiesta, la data d'ordine presente sulla riga verrà usata come data di partenza per il calcolo della data prevedibile per la ricezione degli articoli e della data in cui gli articoli saranno disponibili per il prelievo.  

## <a name="calculating-with-a-requested-receipt-date"></a>Calcolo con una data di carico richiesta  
Se è presente una data di carico richiesta sulla riga dell'ordine di acquisto, questa data verrà utilizzata come data di partenza per i calcoli successivi.  

- data di carico richiesta - calcolo lead time = data ordine  
- data di carico richiesta + tempo gest. entrata in whse. + lead time di sicurezza = data carico prevista  

Se è stata immessa una data di carico richiesta sulla testata dell'ordine di acquisto, questa data viene copiata nel campo corrispondente in tutte le righe. È possibile modificare questa data in qualsiasi riga oppure rimuoverla.  

## <a name="calculating-without-a-requested-delivery-date"></a>Calcolo senza una data di consegna richiesta  
Se si immette una riga di ordine di acquisto senza una data di consegna richiesta, il campo **Data ordine** nella riga viene compilato con la data nel campo **Data ordine** dell'intestazione dell'ordine di acquisto. Si tratta della data immessa o della work date. Le date seguenti vengono quindi calcolate per la riga dell'ordine di acquisto, con la data dell'ordine come punto di partenza.  

- data ordine + calcolo lead time = data carico pianificato  
- data carico pianificato + tempo gest. entrata in whse. + lead time di sicurezza = data carico prevista  

Se si modifica la data dell'ordine sulla riga, ad esempio quando gli articoli non sono disponibili presso il fornitore fino a una data successiva, le date corrispondenti nella riga saranno ricalcolate automaticamente.  

Se si modifica la data dell'ordine nell'intestazione, questa viene copiata nel campo **Data ordine** in tutte le righe e tutti i campi data correlati vengono ricalcolati.  

## <a name="see-also"></a>Vedi anche  
 [Calcolo della data per le vendite](sales-date-calculation-for-sales.md)   
 [Procedura: Calcolare le date per la promessa ordine](sales-how-to-calculate-order-promising-dates.md)  
 [Utilizzo di [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

