---
title: Come stampare l'avviso di rimessa
description: "È possibile aiutare i fornitori a eseguire le riconciliazioni stampando l'avviso di rimessa prima di effettuare una registrazione pagamenti e dopo la registrazione di un pagamento."
documentationcenter: 
author: bholtorf
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 10/26/2017
ms.author: bholtorf
ms.translationtype: HT
ms.sourcegitcommit: a16640e014e157d4dbcaabc53d0df2d3e063f8f9
ms.openlocfilehash: 71c84b4a7bad83e6008c0fa34f908e133b014a59
ms.contentlocale: it-it
ms.lasthandoff: 10/26/2017

---

#<a name="how-to-print-remittance-advice"></a>Procedura: Stampare l'avviso di rimessa
È possibile stampare l'avviso di rimessa prima di eseguire una registrazione pagamenti e dopo la registrazione di un pagamento. Questo avviso visualizza i numeri delle fatture fornitore e consente ai fornitori di eseguire le riconciliazioni.

##<a name="to-print-remittance-advice"></a>Per stampare l'avviso di rimessa
1. Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **Registrazioni pagamenti**, quindi scegliere il collegamento correlato.  
2. Nella finestra **Registrazioni pagamenti**, selezionare il pagamento per il quale l'avviso di rimessa deve essere stampato.  
3. Scegliere l'azione **Stampa avviso di rimessa**.  
4. Nel processo batch **Avviso di rimessa - Giornale di registrazione**, nella Scheda dettaglio **Righe registrazioni COGE**, scegliere i filtri appropriati.  
  
    >[!Note]
    > È possibile filtrare utilizzando il numero di documento esterno del fornitore per la corrispondenza tra pagamenti e fatture.

5. Nella Scheda dettaglio **Fornitore**, scegliere i filtri appropriati.  
6. Scegliere **Stampa** per stampare il report o **Anteprima** per visualizzarlo.  

## <a name="using-remittance-advice-reports"></a>Utilizzo dii report relativi agli avvisi di rimessa
Nella tabella seguente sono descritti i report utilizzabili con l'avviso di rimessa:

|Report|Description|
|----|----|
|Report Avviso di rimessa - Giornale di registrazione|In questo report sono indicati i documenti inclusi nel pagamento. Per le righe delle registrazioni COGE, è possibile specificare il modello di registrazioni e il batch registrazioni da cui gli avvisi di rimessa verranno stampati, la data della prima attività da stampare e il filtro per un numero di documento. Per i fornitori, è possibile immettere il numero dei fornitori da includere nel report. |
|Report Avviso di rimessa - Movimenti| In questo report sono indicati i documenti inclusi nel pagamento. È possibile definire il contenuto del report impostando dei filtri. È possibile impostare ulteriori campi nella scheda scegliendo il campo **Campo**. Per i movimenti contabili fornitori, è possibile specificare i fornitori da includere nel report, la data della prima attività da stampare, la valuta e il numero di movimento da includere. |

> [!Note]
> Il report Avviso di rimessa - Giornale di registrazione non supporta gli scenari di applicazione per valute o le tolleranze di pagamento. Per ulteriori informazioni, vedere [Procedura: Abilitare il collegamento dei movimenti contabili fornitore in valute diverse](finance-how-enable-application-ledger-entries-different-currencies.md).

> [!Tip]
> Per ulteriori informazioni su come utilizzare i report, vedere, [Visualizzazione di report test prima della registrazione](ui-how-view-test-reports-posting.md), [Utilizzare i report](ui-work-report.md) e [Ricerca, filtro e ordinamento di dati](ui-enter-criteria-filters.md).

##<a name="see-also"></a>Vedi anche  
[Benvenuto in Dynamics NAV](across-get-started.md)
