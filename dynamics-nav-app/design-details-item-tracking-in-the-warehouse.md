---
title: "Dettagli di progettazione - Disponibilità tracciabilità articolo"
description: "Questo argomento descrive come assicurarsi che le persone che elaborano ordini possono basarsi sulla disponibilità dei numeri seriali o di lotto."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: design, item, tracking, serial number, lot number, outbound documents
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 1e632e2d7e0b4afe167721d0b68102b48f820307
ms.contentlocale: it-it
ms.lasthandoff: 10/16/2017

---
# <a name="design-details-item-tracking-availability"></a>Dettagli di progettazione: Disponibilità tracciabilità articolo
Nelle finestre **Righe tracciabilità articolo** e **Riepilogo tracciabilità articolo** sono presenti informazioni dinamiche sulla disponibilità relative ai numeri seriali o di lotto. Lo scopo di questo è di aumentare la trasparenza per gli utenti nei documenti in uscita, come gli ordini di vendita, mostrando loro quali numeri seriali o quante unità di un numero di lotto sono attualmente assegnati in altri documenti aperti. Ciò riduce l'incertezza che è causata dalla doppia allocazione e infonde fiducia nei gestori ordini che i numeri di tracciabilità articolo e le date che promettono negli ordini di vendita non registrati possano essere rispettati. Per ulteriori informazioni, vedere [Dettagli di progettazione: Finestra righe tracciabilità articolo](design-details-item-tracking-lines-window.md).  
  
Quando si apre la finestra **Righe tracciabilità articolo**, i dati sulla disponibilità vengono recuperati dalla tabella **Mov. contabile articoli** e dalla tabella **Movimenti impegni**, senza filtro sulla data. Quando si sceglie il campo **Nr. seriale** o il campo **Nr. lotto**, viene visualizzata la finestra **Riepilogo tracciabilità articolo** e viene mostrato un riepilogo delle informazioni sulla tracciabilità articoli nella tabella **Movimenti impegni**. Il riepilogo contiene le seguenti informazioni relative a ogni numero seriale o di lotto nella riga di tracciabilità articolo:  
  
|Campo|Description|  
|---------------------------------|---------------------------------------|  
|**Quantità totale**|La quantità totale del numero seriale o di lotto al momento nel magazzino.|  
|**Qtà totale richiesta**|La quantità totale del numero seriale o di lotto attualmente richiesta in tutti i documenti.|  
|**Quantità corrente in sospeso**|Quantità che viene immessa nell'istanza corrente della finestra **Righe tracciabilità articolo** ma non ancora caricata nel database.|  
|**Quantità totale disponibile**|La quantità del numero seriale o di lotto disponibile per l'utente da richiedere.<br /><br /> Questa quantità viene calcolata da altri campi nella finestra nel modo seguente:<br /><br /> quantità totale – (quantità richiesta totale + quantità corrente in sospeso).|  
  
> [!NOTE]  
>  È inoltre possibile vedere le informazioni nella tabella precedente utilizzando la funzione **Seleziona movimenti** nella finestra **Righe tracciabilità articolo**.  
  
Per mantenere le prestazioni del database, i dati di disponibilità vengono recuperati solo una volta dal database quando si apre la finestra **Righe tracciabilità articolo** e si utilizza la funzione **Aggiorna disponibilità** nella finestra.  
  
## <a name="calculation-formula"></a>Formula di Calcolo  
Come descritto nella tabella precedente, la disponibilità di un numero seriale o di lotto specificato viene calcolata nel modo seguente:  
  
* quantità totale disponibile = quantità in magazzino – (tutte le domande + quantità non ancora sottoposta a commit nel database)  
  
> [!IMPORTANT]  
>  La formula implica che il calcolo della disponibilità del numero seriale o di lotto prenda in considerazione solo il magazzino e ignori i carichi previsti. Di conseguenza, l'approvvigionamento non ancora registrato in magazzino non influisce sulla disponibilità di tracciabilità articolo, a differenza della disponibilità articolo normale in cui sono inclusi i carichi previsti.  
  
## <a name="see-also"></a>Vedi anche  
[Dettagli di progettazione: Tracciabilità articolo](design-details-item-tracking.md)
