---
title: Panoramica dei task per la gestione delle vendite
description: "Descrive come si gestiscono le attività di vendita."
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: trade, sell
ms.date: 09/08/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 030739b491ba5c914d10811cfbac994917f9eb9d
ms.contentlocale: it-it
ms.lasthandoff: 10/16/2017

---
# <a name="sales"></a>Vendite
Si crea una fattura di vendita o un ordine di vendita per registrare il contratto con un cliente per vendere alcuni prodotti con determinate condizioni di consegna e pagamento.

È necessario utilizzare gli ordini di vendita se il processo di vendita richiede che si possano spedire parti di una quantità di un ordine, ad esempio, perché la quantità completa non è disponibile in una sola volta. Se si vendono articoli con consegna diretta dal fornitore al cliente, come una spedizione diretta, è necessario utilizzare anche gli ordini di vendita. In tutti gli altri aspetti, gli ordini di vendita funzionano come le fatture di vendita. Con gli ordini di vendita è possibile anche utilizzare la funzionalità Promesse ordine per comunicare determinate date di consegna ai clienti.  

È possibile negoziare con il cliente prima di tutto creando un'offerta di vendita, che è possibile convertire in una fattura di vendita o un ordine di vendita quando ci si accorda sulla vendita. Dopo che il cliente ha confermato il contratto, è possibile inviare una conferma dell'ordine per registrare l'obbligo di consegnare i prodotti come concordato.

È possibile correggere o annullare in modo semplice una fattura di vendita registrata prima che venga pagata. Ciò risulta utile se si desidera correggere un errore di digitazione o se il cliente richiede una modifica in anticipo nell'elaborazione dell'ordine. Se la fattura di vendita registrata è stata pagata, allora sarà necessario creare una nota di credito di vendita o un ordine di reso da vendita per stornare la vendita.

Per garantire la buona riuscita delle iniziative di marketing e la chiusura delle vendite, è fondamentale prendere le decisioni ottimali nel momento appropriato. La funzionalità di marketing in [!INCLUDE[d365fin](includes/d365fin_md.md)] offre un quadro accurato e tempestivo delle informazioni sui contatti consentendo di presentarsi in modo efficace a potenziali clienti, nonché di incrementare il livello di soddisfazione dei clienti. Per ulteriori informazioni, vedere [Relationship Management](marketing-relationship-management.md).

Negli ambienti aziendali in cui il cliente deve pagare prima che vengano consegnati i prodotti, ad esempio nelle vendita al dettaglio, è necessario attendere la ricezione del pagamento prima di consegnare i prodotti. Nella maggior parte dei casi, i pagamenti in entrata vengono elaborati alcune settimane dopo la consegna collegando i pagamenti alle relative fatture di vendita non pagate registrate. Per ulteriori informazioni, vedere [Procedura: Riconciliare i pagamenti utilizzando il collegamento automatico](receivables-how-reconcile-payments-auto-application.md).

I documenti di vendita possono essere inviati come file PDF allegati all'e-mail. Il corpo e-mail conterrà un estratto del documento di vendita, ad esempio i prodotti, l'importo totale e un collegamento al sito di PayPal. Per ulteriori informazioni, vedere [Procedura: Inviare documenti via e-mail](ui-how-send-documents-email.md).

Per tutti i processi di vendita, è possibile incorporare un workflow di approvazione, ad esempio, per richiedere che le vendite di grandi volumi siano approvate dal responsabile della contabilità. Per ulteriori informazioni, vedere [Utilizzo dei workflow](across-use-workflows.md).

Nella tabella seguente viene descritta una sequenza di task, con collegamenti agli argomenti che li descrivono.

| Per | Vedere |
| --- | --- |
| Creare un'offerta di vendita in cui si presentano prodotti a condizioni negoziabili prima della conversione dell'offerta in una fattura di vendita. |[Procedura: Fare offerte](sales-how-make-offers.md) |
| Creare una fattura di vendita per registrare il contratto con un cliente per vendere prodotti con determinate condizioni di consegna e pagamento. |[Procedura: Fatturare le vendite](sales-how-invoice-sales.md) |
| Elaborare un ordine di vendita con la spedizione parziale o la spedizione diretta. |[Procedura: Vendere prodotti](sales-how-sell-products.md) |
|Impostare righe di vendita o acquisto standard da inserire nei documenti, ad esempio, per ordini di approvvigionamento ricorrenti.|[Procedura: Creare righe di vendite e acquisti ricorrenti](sales-how-work-standard-lines.md)|  
| Collegare un ordine di vendita a un ordine di acquisto per vender un articolo con spedizione diretta che verrà consegnato direttamente dal fornitore al cliente. |[Procedura: Effettuare spedizioni dirette](sales-how-drop-shipment.md) |
|Ricevere un articolo non in stock spedito da un fornitore al magazzino in modo da spedire l'articolo al cliente.|[Procedura: Creare ordini speciali](sales-how-to-create-special-orders.md)|
| Eseguire un'azione in una fattura di vendita registrata non pagata per creare automaticamente una nota di credito e per annullare la fattura di vendita o per ricrearla in modo da apportare correzioni. |[Procedura: Correggere o annullare le fatture di vendita non pagate](sales-how-correct-cancel-sales-invoice.md) |
| Creare una nota di credito vendita per stornare una fattura di vendita registrata specifica per riflettere i prodotti resi dal cliente e l'importo di pagamento da restituire. |[Procedura: Elaborare i resi o gli annullamenti vendite](sales-how-process-sales-returns-cancellations.md) |
|Gestire l'impegno del cliente per acquistare grandi quantità consegnate nel tempo in diverse spedizioni.|[Procedura: Utilizzare gli ordini di vendita programmati](sales-how-to-create-blanket-sales-orders.md)|
|Vendere articoli di assemblaggio che al momento non sono disponibili creando un ordine di assemblaggio collegato per fornire la quantità completa o parziale dell'ordine di vendita.|[Procedura: Vendere articoli assemblati su ordine](assembly-how-to-sell-items-assembled-to-order.md)|
|Fatturare al cliente una volta per più spedizioni combinando le spedizioni in una sola fattura.|[Procedura: Combinare le spedizioni in una singola fattura](sales-how-to-combine-shipments-on-a-single-invoice.md)|
|Comunicare ai clienti le date di consegna dell'ordine calcolando la data CTP (Capable-To-Promise) o ATP (Available-To-Promise).|[Procedura: Calcolare le date per la promessa ordine](sales-how-to-calculate-order-promising-dates.md)|

## <a name="see-also"></a>Vedi anche
[Setup Vendite](sales-setup-sales.md)  
[Procedura: Registrare nuovi clienti](sales-how-register-new-customers.md)  
[Gestione della contabilità clienti](receivables-manage-receivables.md)  
[Gestione della contabilità fornitori](payables-manage-payables.md)  
[Gestione progetti](projects-manage-projects.md)    
[Utilizzo di [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)  
[Funzionalità aziendali generali](ui-across-business-areas.md)

## 

