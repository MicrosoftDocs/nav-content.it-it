---
title: 'Procedura: Vendere prodotti'
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
ms.openlocfilehash: e45d67005364f7d45817d917ccaeab219b6f8446
ms.contentlocale: it-it
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-sell-products"></a>Procedura: Vendere prodotti
Si crea una fattura di vendita o un ordine di vendita per registrare il contratto con un cliente per vendere alcuni prodotti con determinate condizioni di consegna e pagamento.

**Nota**: utilizzare gli ordini di vendita se il processo di vendita richiede che si possano spedire parti di una quantità di un ordine, ad esempio, perché la quantità completa non è disponibile in una sola volta. Se si vendono articoli con consegna diretta dal fornitore al cliente, come una spedizione diretta, è necessario utilizzare anche gli ordini di vendita. Per ulteriori informazioni, vedere [Procedura: Effettuare spedizioni dirette](sales-how-drop-shipment.md). In tutti gli altri aspetti, gli ordini di vendita funzionano come le fatture di vendita. Per ulteriori informazioni, vedere [Procedura: Fatturare le vendite](sales-how-invoice-sales.md).

È possibile negoziare con il cliente prima di tutto creando un'offerta di vendita, che è possibile convertire in un ordine di vendita quando ci si accorda sulla vendita. Per ulteriori informazioni, vedere [Procedura: Fare offerte](sales-how-make-offers.md).

Dopo che il cliente ha confermato il contratto, ad esempio dopo un processo di offerta, è possibile inviare una conferma dell'ordine per registrare l'obbligo di consegnare i prodotti come concordato.

Quando si consegnano i prodotti, nella quantità totale o parziale, si registra l'ordine di vendita come spedito o come spedito e fatturato per creare i relativi movimenti contabili articolo e cliente nel sistema. Quando si registra l'ordine di vendita, è possibile inviare via email il documento come allegato PDF. È possibile impostare il messaggio con un testo precompilato che riepiloga le informazioni dell'ordine e per il pagamento, ad esempio con un collegamento a PayPal. Per ulteriori informazioni, vedere [Procedura: Inviare documenti via e-mail](ui-how-send-documents-email.md).

Negli ambienti aziendali in cui il cliente deve pagare prima che vengano consegnati i prodotti, ad esempio nelle vendita al dettaglio, è necessario attendere la ricezione del pagamento prima di consegnare i prodotti. Nella maggior parte dei casi, i pagamenti in entrata vengono elaborati alcune settimane dopo la consegna collegando i pagamenti alle relative fatture di vendita non pagate registrate. Per ulteriori informazioni, vedere [Procedura: Riconciliare i pagamenti utilizzando il collegamento automatico](receivables-how-reconcile-payments-auto-application.md).

Se la fattura di vendita registrata è stata pagata, allora sarà necessario creare una nota di credito di vendita per stornare la vendita. Per ulteriori informazioni vedere [Procedura: Elaborare i resi o gli annullamenti vendite](sales-how-process-sales-returns-cancellations.md).

I prodotti possono essere sia articoli di magazzino che servizi. Per ulteriori informazioni, vedere [Procedura: Registrare nuovi prodotti](inventory-how-register-new-products.md). Il processo dell'ordine di vendita è lo stesso per entrambi i tipi di prodotto.

**Nota**: in Dynamics NAV un prodotto viene indicato con il termine “articolo”.

È possibile compilare i campi cliente nell'ordine di vendita in due modi a seconda che il cliente sia già registrato o meno.

## <a name="to-create-a-sales-order"></a>Per creare un ordine di vendita
1. Nella home page scegliere l'azione **Ordine vendita**.  
2. Nel campo **Cliente** immettere il nome di un cliente esistente.

    Altri campi nella finestra **Ordine di vendita** vengono compilati con le informazioni standard del cliente selezionato. Se il cliente non è registrato, è necessario attenersi alla seguente procedura:

3. Nel campo **Cliente** immettere il nome del nuovo cliente.
4. Nella finestra di dialogo relativa alla registrazione del nuovo cliente fare clic su **Sì**.  
5. Nella finestra **Selezionare un modello per un nuovo cliente** scegliere un modello su cui basare la scheda del nuovo cliente, quindi scegliere **OK**.

    Una nuova scheda cliente verrà visualizzata, precompilata con le informazioni sul modello cliente selezionato. Il campo **Nome** viene precompilato con il nome del nuovo cliente immesso nell'ordine di vendita.
6. Procedere compilando i restanti campi della scheda cliente. Per ulteriori informazioni, vedere [Procedura: Registrare nuovi clienti](sales-how-register-new-customers.md).  
7. Una volta completata la scheda cliente, scegliere **OK** per tornare alla finestra **Ordine di vendita**.

    Diversi campi nell'ordine di vendita sono ora compilati con le informazioni specificate nella nuova scheda cliente.
8. Compilare i restanti campi della finestra **Ordine di vendita** in base alle proprie esigenze. Selezionare il campo per visualizzare una breve descrizione del campo o il collegamento a ulteriori informazioni.

    A questo punto compilare le righe dell'ordine di vendita con gli articoli di magazzino o i servizi che si desidera vendere al cliente.

    Se sono state impostate le righe di vendita periodiche per il cliente, ad esempio un ordine di rifornimento mensile, è possibile inserire queste righe nell'ordine scegliendo l'azione **Ottieni righe di vendita ricorrenti**.
9. Nella Scheda dettaglio **Righe** del campo **Articolo** immettere il numero di un articolo di magazzino o di un servizio.  
10. Nel campo **Quantità** immettere il numero di articoli da vendere.

    **Nota**: per gli articoli di tipo Assistenza, la quantità è un'unità temporale, ad esempio le ore, come indicato nel campo **Cod. unità di misura** nella riga.

    Il campo **Importo riga** viene aggiornato al valore del campo **Prezzo unitario** moltiplicato per il valore del campo **Quantità**.

    Il prezzo e gli importi riga vengono visualizzati con o senza le tasse di vendita a seconda della selezione nel campo **Prezzi IVA inclusa** della scheda cliente.
11. Nel campo **% sconto riga** immettere una percentuale se si intende concedere al cliente uno sconto sul prodotto. Il valore nel campo **Importo riga** viene aggiornato di conseguenza.

    Se sono stati impostati prezzi articolo speciali nella Scheda dettaglio **Prezzi di vendita e sconti riga di vendita** per il cliente o la scheda articolo, la percentuale di sconto riga, il prezzo e l'importo nella riga dell'offerta vengono automaticamente aggiornati se vengono soddisfatti i criteri di prezzo concordati. Per ulteriori informazioni, vedere [Registrazione di prezzi, sconti e contratti di pagamento per le vendite](sales-how-record-sales-price-discount-payment-agreements.md).
12. Per aggiungere un commento sulla riga dell'offerta che il cliente può vedere sull'offerta di vendita stampata, scrivere un testo nel campo **Descrizione** nella riga vuota.  
13. Ripetere i passaggi da 10 a 13 per ogni articolo che si desidera offrire al cliente.

    I totali sotto le righe vengono automaticamente calcolati quando si creano o si modificano le righe.
14. Nel campo **Importo sconto fattura** immettere un importo che deve essere dedotto dal valore indicato nel campo **Totale IVA incl.**.

    Se sono stati impostati degli sconti su fattura per il cliente, il valore percentuale specificato viene automaticamente inserito nel campo **% sconto fattura** se vengono soddisfatti i criteri e l'importo correlato viene inserito nel campo **Importo sconto fatt. IVA esclusa**. Per ulteriori informazioni, vedere [Registrazione di prezzi, sconti e contratti di pagamento per le vendite](sales-how-record-sales-price-discount-payment-agreements.md).
15. Per spedire solo una parte della quantità ordinata, immettere la quantità desiderata nel campo **Qtà da spedire**. Il valore viene copiato nel campo **Qtà da fatturare**.
16. Per fatturare solo una parte della quantità spedita, immettere la quantità desiderata nel campo **Qtà da fatturare**. La quantità deve essere inferiore al valore presente nel campo **Qtà da spedire**.   
17. Una volta completate le righe dell'ordine di vendita, scegliere l'azione **Registra e invia**.
Viene visualizzata la finestra di dialogo **Registra e invia conferma** contenente il metodo di invio preferito del cliente.

È possibile modificare il metodo di invio scegliendo il pulsante di ricerca per il campo **Invia documento a**. Per ulteriori informazioni, vedere [Procedura: Impostare profili di invio documenti](sales-how-setup-document-send-profiles.md).

I movimenti contabili cliente e articolo sono ora creati nel sistema e l'ordine di vendita è emesso come documento PDF. Una volta che l'ordine di vendita è completamente registrato, viene rimosso dalla lista degli ordini di vendita e viene sostituito con nuovi documenti nella lista delle fatture di vendita registrate e nella lista delle spedizioni registrate.

## <a name="see-also"></a>Vedi anche  
[Gestire le vendite](sales-manage-sales.md)  
[Impostare le vendite](sales-setup-sales.md)  
[Magazzino](inventory-manage-inventory.md)  
[Procedura: Inviare documenti via e-mail](ui-how-send-documents-email.md)  
[Utilizzare Dynamics NAV](ui-work-product.md)
