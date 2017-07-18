---
title: Gestire gli acquisti
author: SorenGP
ms.custom: na
ms.date: 11/23/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: df94e447d7d4542f75f3c34105099016b0abbf32
ms.contentlocale: it-it
ms.lasthandoff: 06/26/2017

---

# <a name="manage-purchasing"></a>Gestire gli acquisti
È possibile creare una fattura o un ordine di acquisto per registrare il costo di acquisto e per tenere traccia del conto fornitori. Se è necessario verificare un magazzino, anche le fatture di acquisto vengono utilizzate per aggiornare in modo dinamico i livelli di magazzino in modo da ridurre i costi di magazzino al minimo e migliorare l'assistenza clienti. I costi di acquisto, incluse le spese di assistenza, e i valori di magazzino derivanti dalla registrazione delle fatture di acquisto contribuiscono alle cifre di profitto e altri indicatori KPI finanziari presenti nella home page.

Utilizzare gli ordini di acquisto se il processo di acquisto richiede la registrazione delle le ricevute parziali di una quantità di un ordine, ad esempio, perché la quantità completa non è disponibile presso il fornitore. Se si vendono articoli con consegna diretta dal fornitore al cliente, come una spedizione diretta, è necessario utilizzare anche gli ordini di acquisto. Per ulteriori informazioni, vedere [Procedura: Effettuare spedizioni dirette](sales-how-drop-shipment.md). In tutti gli altri aspetti, gli ordini di acquisto funzionano come le fatture di acquisto.

È possibile creare le fatture di acquisto automaticamente utilizzando il servizio OCR (riconoscimento ottico dei caratteri) per convertire le fatture PDF ricevute dai fornitori in documenti elettronici, che verranno successivamente convertiti in fatture di acquisto da un workflow. Per utilizzare questa funzionalità, è necessario innanzitutto iscriversi al servizio OCR e impostarlo. Per ulteriori informazioni, vedere [Procedura: Elaborare i documenti in entrata](across-process-income-documents.md).      

**Nota**: in Dynamics NAV un prodotto viene indicato con il termine “articolo”.

I prodotti possono essere sia articoli di magazzino che servizi. Per ulteriori informazioni, vedere [Procedura: Registrare nuovi prodotti](inventory-how-register-new-products.md).

Per tutti i processi di acquisto, è possibile incorporare un workflow di approvazione, ad esempio, per richiedere che gli acquisti di grande volume siano approvati dal responsabile della contabilità. Per ulteriori informazioni, vedere [Utilizzo dei workflow di approvazione](across-how-use-approval-workflows.md).

Nella tabella seguente viene descritta una sequenza di task, con collegamenti agli argomenti che li descrivono. Questi task sono elencati nell'ordine in cui vengono in genere eseguiti.


|Per |Vedere |
|---|----|
|Creare una fattura di acquisto per registrare il contratto con un fornitore per acquistare prodotti con determinate condizioni di consegna e pagamento. |[Procedura: Registrare gli acquisti](purchasing-how-record-purchases.md)|
|Creare una fattura di acquisto per tutte le righe o quelle selezionate in una fattura di vendita.|[Procedura: Acquistare i prodotti per una vendita](purchasing-how-purchase-products-sale.md)|
|Creare una nota di credito di acquisto per stornare una fattura di acquisto registrata specifica per riflettere i prodotti resi al fornitore e l'importo di pagamento ricevuto.|[Procedura: Elaborare i resi o gli annullamenti acquisti](purchasing-how-process-purchase-returns-cancellations.md)|
|Creare una scheda fornitore per ogni fornitore da cui si acquista.|[Procedura: Registrare nuovi fornitori](purchasing-how-register-new-vendors.md)|

## <a name="see-also"></a>Vedi anche
[Impostare gli acquisti](purchasing-setup-purchasing.md)  
[Gestire la contabilità fornitori](payables-manage-payables.md)    
[Utilizzare Dynamics NAV](ui-work-product.md)  
[Tra le aree aziendali](ui-across-business-areas.md)

