---
title: Registrazione di assistenza
description: "La funzionalità di registrazione dei servizi di assistenza consente di elaborare i documenti in modo efficiente e di gestire in modo efficace il servizio di assistenza offerto ai clienti. È possibile creare e aggiornare documenti registrati, nonché creare movimenti contabili sia nell'area di assistenza che in altri moduli per garantire modifiche correttamente aggiornate."
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 09/18/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 7ab0d57c960b0568c1da1896914f1a1ce939d0ea
ms.contentlocale: it-it
ms.lasthandoff: 10/16/2017

---
# <a name="service-posting"></a>Registrazione di assistenza
La funzionalità di registrazione dei servizi di assistenza consente di elaborare i documenti in modo efficiente e di gestire in modo efficace il servizio di assistenza offerto ai clienti. È possibile creare e aggiornare documenti registrati, nonché creare movimenti contabili sia nell'area di assistenza che in altri moduli per garantire modifiche correttamente aggiornate.  

> [!NOTE]  
>  Di seguito viene descritta la registrazione di assistenza indipendentemente dalla modalità di gestione fisica degli articoli nella warehouse.  
>   
>  In un'ubicazione non impostata per richiedere la gestione warehouse, le azioni di registrazione vengono effettuate direttamente nella finestra **Righe assistenza**. Nelle ubicazioni che prevedono la gestione in warehouse, le azioni di registrazione descritte, tranne Spedizione e consumo, vengono eseguite indirettamente tramite diverse funzioni di spedizione warehouse, a seconda del setup. Per ulteriori informazioni, vedere [Procedura: Prelevare articoli con prelievi magazzino](warehouse-how-to-pick-items-with-inventory-picks.md).  

## <a name="ship"></a>Spedizione  
L'opzione relativa alla spedizione consente di registrare gli articoli e il tempo appropriati immessi nelle righe di un ordine di assistenza dopo il completamento dell'assistenza stessa. Viene creata una spedizione registrata e si verificano aggiornamenti nel modulo Magazzino e in altri moduli di [!INCLUDE[d365fin](includes/d365fin_md.md)] con l'indicazione che gli articoli sono stati prelevati dal magazzino e inviati al cliente. In particolare, vengono generati movimenti contabili relativi agli articoli e al valore, movimenti assistenza e movimenti garanzia.  

Se l'ubicazione è impostata in modo da richiedere la gestione warehouse, la spedizione e movimentazione degli articoli nelle righe di assistenza funzionano allo stesso modo di altri documenti di origine. La sola differenza sta nel fatto che gli articoli nelle righe di assistenza possono essere consumati esternamente o internamente e richiedono due diverse funzioni di rilascio.

## <a name="invoice"></a>Fattura  
Questa opzione consente di emettere una fattura verso il cliente a cui si desidera addebitare l'assistenza. L'importo da fatturare è in genere costituito dalla differenza tra la quantità spedita registrata mediante la funzione **Registrare spedizione** e la quantità consumata registrata mediante la funzione **Registra consumo**. Non è possibile fatturare quantità che non sono state spedite. Quando si esegue la funzione **Registra fatture**, viene creata una fattura di assistenza registrata e vengono aggiornati i documenti registrati prima di modificarli in base alle quantità contenute nella fattura emessa. Analogamente ad altre procedure di registrazione, vengono generati i movimenti contabili corrispondenti, inclusi i movimenti di contabilità generale.  

## <a name="ship-and-invoice"></a>Spedizione e Fattura  
L'opzione di spedizione e fattura consente di emettere sia una spedizione di assistenza che una fattura contemporaneamente.  

## <a name="ship-and-consume"></a>Spedizione e consumo  
L'opzione di spedizione e consumo consente di registrare e contabilizzare articoli, costi oppure ore utilizzati per prestare assistenza, ma che non possono essere inclusi nella fattura da inviare al cliente. In base a questa opzione non viene emessa alcuna fattura, ma è possibile generare contemporaneamente una spedizione e un consumo di assistenza per indicare che al cliente sono stati concessi alcuni articoli oppure ore gratuiti. Per registrare il consumo, vengono inoltre creati i movimenti contabili corrispondenti.  

> [!NOTE]  
>  La procedura di registrazione di assistenza consente di eseguire la registrazione parziale. Prima di effettuare la registrazione, è inoltre possibile creare una spedizione parziale o una fattura parziale compilando i campi **Qtà da spedire** e **Qtà da fatturare** nelle singole righe di assistenza degli ordini di assistenza. Si tenga presente che non è possibile creare una fattura per un articolo che non è stato spedito. Ciò significa che è necessario registrare una spedizione prima di emettere una fattura oppure la spedizione e la fattura devono essere contemporanee.  

Dopo il completamento della registrazione, sarà possibile visualizzare i documenti di assistenza registrati nelle finestre corrispondenti, ovvero **Spedizione assistenza registrata** e **Fattura assistenza registrata**. I movimenti creati possono essere visualizzati in apposite finestre contenenti movimenti registrati, ad esempio **Movimenti C/G**, **Mov. contabili articoli**, **Movimenti warehouse**, **Movimenti assistenza**, **Movimenti cont. commesse** e **Movimenti garanzia**.  

## <a name="to-view-information-about-a-posted-service-document"></a>Per visualizzare informazioni su un documento di assistenza registrato  
Quando si registra una fattura, una spedizione o una nota di credito di assistenza, le informazioni presenti nel documento vengono trasferite nella finestra **Fattura assistenza registrata**, **Spedizione assistenza registrata** o **Nota credito assistenza registrata** rispettivamente. In queste finestre non è possibile immettere, modificare né eliminare alcuna informazione. Nelle finestre è possibile stampare una spedizione, una fattura o una nota di credito.  

Nella procedura seguente viene utilizzata una fattura di assistenza registrata come esempio, ma la stessa procedura può essere applicata alle spedizioni di assistenza registrate e alle note di credito registrate.  

1. Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **Fattura assistenza registrata**, quindi scegliere il collegamento correlato.  
2. Aprire la fattura di assistenza registrata che si desidera visualizzare.  
3. Per ottenere una panoramica della fattura registrata, scegliere l'azione **Statistiche**.  

    Viene visualizzata la finestra **Statistiche ordine assistenza**. Nella finestra vengono visualizzate informazioni quali quantità, importo, IVA, costo, margine e limite di credito del cliente per il documento registrato.

## <a name="see-also"></a>Vedi anche  
[Procedura: Registrare gli ordini di assistenza](service-how-to-post-service-orders.md)   
[Procedura: Creare ordini di assistenza](service-how-to-create-service-orders.md)

