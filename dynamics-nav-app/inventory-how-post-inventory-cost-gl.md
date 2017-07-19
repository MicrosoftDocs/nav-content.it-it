---
title: "Procedura: Registrare costi di magazzino nella contabilità generale"
author: SorenGP
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: 59815db9c7b435ff585e1174b570029a360dea6e
ms.contentlocale: it-it
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-post-inventory-costs-to-the-general-ledger"></a>Procedura: Registrare costi di magazzino nella contabilità generale   
Quando si registrano transazioni di magazzino, ad esempio spedizioni, fatture di vendite o rettifiche di magazzino, le modifiche alle quantità e ai costo vengono registrate automaticamente rispettivamente nei movimenti contabili articoli e nei movimenti di valorizzazione. Per riflettere la modifica del valore di magazzino nei registri finanziari, è necessario registrare i costi di magazzino nei conti giacenza magazzino correlati in contabilità generale.

I costi possono venire registrati nella contabilità generale in due modi.

- Automaticamente, impostando il programma in modo che i costi di magazzino vengano registrati nella contabilità generale ogni volta che si registra una transazione di magazzino.
- Manualmente, in modo che i costi di magazzino vengano registrati solo nella contabilità generale quando si esegue un processo batch.


## <a name="to-post-inventory-costs-automatically"></a>Per registrare automaticamente i costi di magazzino
1. Nell'angolo superiore destro, scegliere l'icona **Cerca pagina o report**, immettere **Setup magazzino**, quindi scegliere il collegamento correlato.
2. Nella finestra **Setup magazzino**, selezionare la casella di controllo **Reg. automatica costi**.

Per ogni transazione di magazzino registrata, verranno registrati i valori appropriati nel conto giacenza magazzino, nel conto di rettifica e nel conto COGS nella contabilità generale.

Anche se si utilizza la registrazione automatica dei costi, è comunque necessario eseguire periodicamente il processo batch Rettifica costo - Mov. art. per assicurarsi che i costi delle merci vengano trasferiti alle transazioni in uscita appropriate, ad esempio vendite o trasferimenti. Si tratta di un'operazione particolarmente importante nel caso in cui si vendano merci prima di fatturare il relativo acquisto.

Se durante la registrazione del costo di magazzino nella contabilità generale viene rilevato un errore nel setup delle dimensioni, la registrazione viene interrotta.

## <a name="to-post-inventory-costs-manually"></a>Per registrare manualmente i costi di magazzino
1. Nell'angolo superiore destro, scegliere l'icona **Cerca pagina o report**, immettere **Registra costo magazzino in C/G**, quindi scegliere il collegamento correlato.
2. Per registrare manualmente i costi di magazzino nella contabilità generale, eseguire il processo batch. Quando si esegue questo processo batch, vengono creati i movimenti C/G sulla base dei movimenti di valorizzazione. È possibile registrare i movimenti in modo che vengano riepilogati per categoria di registrazione.

**Nota**: quando si esegue questo processo batch, si possono verificarsi errori dovuti a setup mancante o setup delle dimensioni incompatibile. Se vengono rilevati errori nel setup delle dimensioni, questi vengono ignorati e vengono utilizzate le dimensioni del movimento di valorizzazione. In caso di errori di altro tipo, la registrazione dei movimenti di valorizzazione viene saltata e i movimenti vengono elencati alla fine del report in una sezione relativa ai “movimenti saltati”. Per registrare questi movimenti, è prima necessario correggere gli errori.

Per visualizzare un elenco di errori prima di eseguire il processo batch di registrazione, eseguire il report **Registra costo mag. in C/G - Test**. Nel report di test vengono elencati tutti gli errori rilevati durante una registrazione di test. È quindi possibile correggere gli errori e poi eseguire il processo batch di registrazione del costo di magazzino senza saltare alcun movimento.

Se si desidera semplicemente ottenere informazioni sui valori che possono essere registrati nella contabilità generale senza eseguire la registrazione, è possibile eseguire il processo batch Registra costo magazzino in C/G senza effettuare la registrazione dei valori nella contabilità generale. A tale scopo, è necessario deselezionare il campo Registra dalla pagina di richiesta. In questo modo, quando si esegue il processo batch, viene esclusivamente prodotto il report in cui sono indicati i valori pronti per essere registrati nella contabilità generale, ma che non sono stati ancora registrati.

## <a name="see-also"></a>Vedi anche
[Gestire i costi del magazzino](inventory-manage-inventory.md)    
[Procedura: Rettificare i costi degli articoli](inventory-how-adjust-item-costs.md)  
[Gestire le vendite](sales-manage-sales.md)  
[Gestire gli acquisti](purchasing-manage-purchasing.md)

