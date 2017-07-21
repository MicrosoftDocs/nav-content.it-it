---
title: 'Procedura: Suggerire i pagamenti ai fornitori'
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
ms.openlocfilehash: 11bfba9f279f6bd84c5d169f6f97fd48759bc6df
ms.contentlocale: it-it
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-suggest-vendor-payments"></a>Procedura: Suggerire i pagamenti ai fornitori
Nella finestra **Registrazioni pagamenti** è possibile utilizzare una funzione per suggerire le righe di pagamento in base alle impostazioni, quali ad esempio i pagamenti in scadenza o i pagamenti che prevedono uno sconto.

Per trarre vantaggi dalla funzione Sugg. pagamenti fornitore, occorre innanzitutto attribuire un ordine di priorità ai fornitori. Per ulteriori informazioni, vedere [Procedura: Attribuire un ordine di priorità ai fornitori](purchasing-how-prioritize-vendors.md).

Le voci di fornitori che non sono contrassegnate da **In sospeso** non sono incluse nel processo batch.  

**Importante**: se si desidera avvantaggiarsi degli sconti sui pagamenti e si è immesso un importo disponibile, l'importo sarà usato innanzitutto in ordine di priorità per i movimenti fornitori scaduti ordinati in senso prioritario, quindi per i movimenti scaduti fornitori non ordinati in senso prioritario e, infine, per i movimenti fornitori aperti che hanno diritto a sconti sui pagamenti in base al numero del fornitore.

## <a name="to-use-the-suggest-vendor-payments-function"></a>Per utilizzare la funzione di suggerimento pagamenti fornitori
1. Nell'angolo superiore destro, scegliere l'icona **Cerca pagina o report**, immettere **Registrazioni pagamenti**, quindi scegliere il collegamento correlato.
2. Aprire le registrazioni rilevanti e scegliere l'azione **Sugg. pagamenti fornitore**.
3. Compilare i campi, se necessario. Selezionare il campo per visualizzare una breve descrizione del campo o il collegamento a ulteriori informazioni.
4. Scegliere il pulsante **OK**.

## <a name="to-insert-the-due-date-as-posting-date-on-payment-journal-lines"></a>Per inserire la data di scadenza come data di registrazione nelle righe di registrazione pagamenti
Quando si esegue il processo batch **Sugg. pagamenti fornitore** per creare righe di pagamento per i fornitori, è possibile compilare due campi speciali per assicurarsi che le righe generate utilizzino la data di scadenza per calcolare la data di registrazione. Questi campi sono **Calcola data di registrazione da Collega a - Scadenza doc.** e **Offset Collega a - Scadenza doc.**

**Importante**: non è possibile utilizzare il campo **Calcola data di registrazione da Collega a - Scadenza doc.** insieme al campo **Trova sconti pagamenti** o al campo **Raggruppa per fornitore**. Il motivo è che se la data di registrazione è basata sulla data di scadenza, lo sconto pagamento potrebbe non essere calcolato correttamente, in quanto la data di registrazione potrebbe essere successiva alla data dello sconto di pagamento.
Inoltre, se la data di registrazione calcolata è già trascorsa, la data di registrazione verrà spostata alla data di lavoro e verrà visualizzato un avviso.

In alternativa, è possibile creare manualmente le righe di pagamento utilizzando la data di scadenza per calcolare la data di registrazione. Una volta collegati i movimenti contabili fornitori, è possibile utilizzare l'azione **Calcola data registrazione**. La data di registrazione nella riga di registrazione verrà aggiornata alla data di scadenza della fattura di acquisto correlata. Per ulteriori informazioni, vedere [Procedura: Collegare manualmente le transazioni di acquisto](payables-how-apply-purchase-transactions-manually.md).  

**Nota**: se la fattura di acquisto è scaduta, la data di registrazione verrà impostata sulla data di lavoro e il carattere nella riga diventerà di colore rosso.

## <a name="see-also"></a>Vedi anche
[Gestire la contabilità fornitori](payables-manage-payables.md)  
[Effettuare i pagamenti](payables-make-payments.md)  
[Utilizzo delle registrazioni COGE](ui-work-general-journals.md)

