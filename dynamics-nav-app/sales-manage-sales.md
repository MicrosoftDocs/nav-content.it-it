---
title: Gestire le vendite
author: SorenGP
ms.custom: na
ms.date: 11/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: 20e380abb2f8f598391a66e50a7ec7a1c8b15fa1
ms.contentlocale: it-it
ms.lasthandoff: 06/26/2017

---

# <a name="manage-sales"></a>Gestire le vendite
Si crea una fattura di vendita o un ordine di vendita per registrare il contratto con un cliente per vendere alcuni prodotti con determinate condizioni di consegna e pagamento.

È necessario utilizzare gli ordini di vendita se il processo di vendita richiede che si possano spedire parti di una quantità di un ordine, ad esempio, perché la quantità completa non è disponibile in una sola volta. Se si vendono articoli con consegna diretta dal fornitore al cliente, come una spedizione diretta, è necessario utilizzare anche gli ordini di vendita. In tutti gli altri aspetti, gli ordini di vendita funzionano come le fatture di vendita.  

Per garantire la buona riuscita delle iniziative di marketing e la chiusura delle vendite, è fondamentale prendere le decisioni ottimali nel momento appropriato. La funzionalità di marketing in Dynamics NAV offre un quadro accurato e tempestivo delle informazioni sui contatti consentendo di presentarsi in modo efficace a potenziali clienti, nonché di incrementare il livello di soddisfazione dei clienti. Per ulteriori informazioni, vedere [Relationship Management](marketing-relationship-management.md).

È possibile negoziare con il cliente prima di tutto creando un'offerta di vendita, che è possibile convertire in una fattura di vendita quando ci si accorda sulla vendita. Dopo che il cliente ha confermato il contratto, ad esempio dopo un processo di offerta, è possibile inviare una conferma dell'ordine per registrare l'obbligo di consegnare i prodotti come concordato.

Quando si consegnano i prodotti, nella quantità totale o parziale, si registra l'ordine di vendita, o la fattura di vendita, come spedito o come spedito e fatturato per creare i relativi movimenti contabili articolo e cliente nel sistema.

Negli ambienti aziendali in cui il cliente deve pagare prima che vengano consegnati i prodotti, ad esempio nelle vendita al dettaglio, è necessario attendere la ricezione del pagamento prima di consegnare i prodotti. Nella maggior parte dei casi, i pagamenti in entrata vengono elaborati alcune settimane dopo la consegna collegando i pagamenti alle relative fatture di vendita non pagate registrate. Per ulteriori informazioni, vedere [Procedura: Riconciliare i pagamenti utilizzando il collegamento automatico](receivables-how-reconcile-payments-auto-application.md).

I documenti di vendita possono essere inviati come file PDF allegati all'e-mail. Il corpo e-mail conterrà un estratto del documento di vendita, ad esempio i prodotti, l'importo totale e un collegamento al sito di PayPal. Per ulteriori informazioni, vedere [Procedura: Inviare documenti via e-mail](ui-how-send-documents-email.md).

Per tutti i processi di vendita, è possibile incorporare un workflow di approvazione, ad esempio, per richiedere che le vendite di grandi volumi siano approvate dal responsabile della contabilità. Per ulteriori informazioni, vedere [Utilizzo dei workflow di approvazione](across-how-use-approval-workflows.md).

Nella tabella seguente viene descritta una sequenza di task, con collegamenti agli argomenti che li descrivono.

|Per |Vedere |
|---|----|
|Creare un'offerta di vendita in cui si presentano prodotti a condizioni negoziabili prima della conversione dell'offerta in una fattura di vendita.|[Procedura: Fare offerte](sales-how-make-offers.md)|
|Creare una fattura di vendita per registrare il contratto con un cliente per vendere prodotti con determinate condizioni di consegna e pagamento.|[Procedura: Fatturare le vendite](sales-how-invoice-sales.md)|
|Elaborare un ordine di vendita con la spedizione parziale o la spedizione diretta.|[Procedura: Vendere prodotti](sales-how-sell-products.md)|
|Collegare un ordine di vendita a un ordine di acquisto per vender un articolo con spedizione diretta che verrà consegnato direttamente dal fornitore al cliente.|[Procedura: Effettuare spedizioni dirette](sales-how-drop-shipment.md)|
|Creare una nota di credito vendita per stornare una fattura di vendita registrata specifica per riflettere i prodotti resi dal cliente e l'importo di pagamento da restituire.|[Procedura: Elaborare i resi o gli annullamenti vendite](sales-how-process-sales-returns-cancellations.md)|
|Creare una scheda cliente per ogni cliente a cui si effettua una vendita.|[Procedura: Registrare nuovi clienti](sales-how-register-new-customers.md)|

## <a name="see-also"></a>Vedi anche  
[Impostare le vendite](sales-setup-sales.md)  
[Gestire la contabilità clienti](receivables-manage-receivables.md)  
[Gestire la contabilità fornitori](payables-manage-payables.MD)      
[Utilizzare Dynamics NAV](ui-work-product.md)  
[Tra le aree aziendali](ui-across-business-areas.md)

