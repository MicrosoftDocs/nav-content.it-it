---
title: Utilizzare il processo batch Suggerisci pagamenti fornitore
description: "È possibile specificare le impostazioni di pagamento dei fornitori per ottenere suggerimenti o proposte per pagamenti in scadenza oppure per cui è disponibile uno sconto."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: vendor payment, creditor, debt, balance due, AP
ms.date: 06/06/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 99bec4a5cc06209d4e7cfc0e7d2736bfc6fe9e1e
ms.contentlocale: it-it
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-suggest-vendor-payments"></a>Procedura: Suggerire i pagamenti ai fornitori
Nella finestra **Registraz. pagamenti** è possibile utilizzare il processo batch **Sugg. pagamenti fornitore** per suggerire le righe di pagamento. Le righe per operazioni come i pagamenti che scadono presto oppure i pagamenti dove è disponibile uno sconto sul pagamento vengono suggerite in base alle impostazioni.

Per trarre completamente giovamento dalle righe suggerite, è prima necessario assegnare una priorità ai fornitori. Per ulteriori informazioni, vedere [Procedura: Attribuire un ordine di priorità ai fornitori](purchasing-how-prioritize-vendors.md).  

I movimenti fornitori, che non sono **In Sospeso**, non sono inclusi.  

> [!IMPORTANT]  
>   Per trarre vantaggio dagli sconti sui pagamenti, se si è immesso un importo disponibile, l'importo verrà utilizzato per:  

* Movimenti fornitori scaduti con priorità innanzitutto in ordine di priorità.  
* Movimenti fornitori scaduti senza priorità.  
* Movimenti fornitori che vengono qualificati per gli sconti sui pagamenti, sistemati in base al numero di fornitori.  

## <a name="to-use-the-suggest-vendor-payments-function"></a>Per utilizzare la funzione di suggerimento pagamenti fornitori
1. Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **Registrazioni pagamenti**, quindi scegliere il collegamento correlato.  
2. Aprire le registrazioni rilevanti e scegliere l'azione **Sugg. pagamenti fornitore**.  
3. Compilare i campi, se necessario. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  
4. Scegliere il pulsante **OK**.  

## <a name="to-insert-the-due-date-as-posting-date-on-payment-journal-lines"></a>Per inserire la data di scadenza come data di registrazione nelle righe di registrazione pagamenti
Quando si esegue il processo batch **Sugg. pagamenti fornitore** per creare righe di pagamento per i fornitori, è possibile compilare due campi speciali per assicurarsi che le righe generate utilizzino la data di scadenza per calcolare la data di registrazione. Questi campi sono **Calcola data di registrazione da Collega a - Scadenza doc.** e **Offset Collega a - Scadenza doc.**  

> [!IMPORTANT]  
>   Non è possibile utilizzare il campo **Calcola data di registrazione da Collega a - Scadenza doc** insieme al campo **Trova sconti pagamenti** o al campo **Raggruppa per fornitore**. Se la data di registrazione è basata sulla data di scadenza, gli sconti sui pagamenti potrebbero non essere calcolati correttamente, in quanto la data di registrazione potrebbe essere successiva alla data dello sconto sul pagamento.  

Inoltre, se la data di registrazione calcolata è già trascorsa, la data di registrazione viene spostata alla data di lavoro e viene visualizzato un avviso.  

In alternativa, è possibile creare manualmente le righe di pagamento utilizzando la data di scadenza per calcolare la data di registrazione. Dopo che si collegano movimenti contabili fornitori, è possibile utilizzare l'azione **Calcola data registrazione** per aggiornare la data di registrazione nella riga di registrazione con la data di scadenza della fattura relativa di acquisto. Per ulteriori informazioni, vedere [Procedura: Collegare manualmente le transazioni di acquisto](payables-how-apply-purchase-transactions-manually.md).  

> [!NOTE]  
>   Se la fattura di acquisto è scaduta, la data di registrazione viene impostata sulla data di lavoro e il carattere nella riga diventa di colore rosso.  

## <a name="see-also"></a>Vedi anche
[Gestione della contabilità fornitori](payables-manage-payables.md)  
[Effettuare i pagamenti](payables-make-payments.md)  
[Utilizzo delle registrazioni COGE](ui-work-general-journals.md)  
[Utilizzo di [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)  

