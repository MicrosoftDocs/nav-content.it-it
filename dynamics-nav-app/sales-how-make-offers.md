---
title: 'Procedura: Fare offerte'
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
ms.openlocfilehash: e126c755a9121c3a91f3af72f3f1ae14702a4701
ms.contentlocale: it-it
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-make-offers"></a>Procedura: Fare offerte
Creare un'offerta di vendita per registrare la propria offerta al cliente per vendere alcuni prodotti a determinate condizioni di consegna e di pagamento. È possibile inviare l'offerta di vendita al cliente per comunicare l'offerta. È possibile inviare il documento via e-mail come allegato PDF. È inoltre possibile fare in modo che il corpo e-mail venga precompilato con un riepilogo dell'offerta. Per ulteriori informazioni, vedere [Procedura: Inviare documenti via e-mail](ui-how-send-documents-email.md).

Quando si negozia con il cliente, è possibile modificare e inviare nuovamente l'offerta di vendita in base alle esigenze. Se il cliente accetta l'offerta, si converte l'offerta di vendita in un ordine o una fattura di vendita in cui viene elaborata la vendita. Per ulteriori informazioni vedere [Procedura: Fatturare le vendite](sales-how-invoice-sales.md) o [Procedura: Vendere prodotti](sales-how-sell-products.md).

I prodotti possono essere sia articoli di magazzino che servizi. Per ulteriori informazioni, vedere [Procedura: Registrare nuovi prodotti](inventory-how-register-new-products.md). Il processo dell'offerta di vendita è lo stesso per entrambi i tipi di prodotto.

**Nota**: in Dynamics NAV un prodotto viene indicato con il termine “articolo”.

È possibile compilare i campi cliente nell'offerta di vendita in due modi a seconda che il cliente sia già registrato o meno.

## <a name="to-create-a-sales-quote"></a>Per creare un'offerta di vendita
1. Nella home page scegliere l'azione **Offerta vendita**.  
2. Nel campo **Cliente** immettere il nome di un cliente esistente.

    Altri campi nella finestra **Offerta di vendita** vengono compilati con le informazioni standard del cliente selezionato. Se il cliente non è registrato, è necessario attenersi alla seguente procedura:

3. Nel campo **Cliente** immettere il nome del nuovo cliente.
4. Nella finestra di dialogo relativa alla registrazione del nuovo cliente fare clic su **Sì**.
5. Nella finestra **Selezionare un modello per un nuovo cliente** scegliere un modello su cui basare la scheda del nuovo cliente, quindi scegliere **OK**.
6. Una nuova scheda cliente verrà visualizzata, precompilata con le informazioni sul modello cliente selezionato. Il campo **Nome** viene precompilato con il nome del nuovo cliente immesso nella fattura di vendita.
7. Procedere compilando i restanti campi della scheda cliente. Per ulteriori informazioni, vedere [Procedura: Registrare nuovi clienti](sales-how-register-new-customers.md).  
8. Una volta completata la scheda cliente, scegliere **OK** per tornare alla finestra **Offerta di vendita**.

    Diversi campi nell'offerta di vendita sono ora compilati con le informazioni specificate nella nuova scheda cliente.
9. Compilare i restanti campi della finestra **Offerta di vendita** in base alle proprie esigenze. Selezionare il campo per visualizzare una breve descrizione del campo o il collegamento a ulteriori informazioni.

    A questo punto compilare le righe dell'offerta di vendita con gli articoli di magazzino o i servizi che si desidera offrire al cliente.

    **Nota**: se sono state impostate righe di vendita periodiche per il cliente, ad esempio un ordine di rifornimento mensile, è possibile inserire queste righe nell'offerta scegliendo l'azione **Ottieni righe di vendita ricorrenti**.
10. Nella Scheda dettaglio **Righe**, nel campo **Nr. articolo**, immettere il numero di un'assistenza o di un articolo di magazzino.
11. Nel campo **Quantità** immettere il numero di articoli offerti.

    **Nota**: per gli articoli di tipo Assistenza, la quantità è un'unità temporale, ad esempio le ore, come indicato nel campo **Cod. unità di misura** nella riga.

    Il campo **Importo riga** viene aggiornato al valore del campo **Prezzo unitario** moltiplicato per il valore del campo **Quantità**.

    Il prezzo e gli importi riga vengono visualizzati con o senza le tasse di vendita a seconda della selezione nel campo **Prezzi IVA inclusa** della scheda cliente.
12. Nel campo **% sconto riga** immettere una percentuale se si intende concedere al cliente uno sconto sul prodotto. Il valore nel campo **Importo riga** viene aggiornato di conseguenza.

    **Nota**: se sono stati impostati prezzi articolo speciali nella Scheda dettaglio **Prezzi di vendita e sconti riga di vendita** per il cliente o la scheda articolo, la percentuale di sconto riga, il prezzo e l'importo nella riga dell'offerta vengono automaticamente aggiornati se vengono soddisfatti i criteri di prezzo concordati. Per ulteriori informazioni, vedere [Registrazione di prezzi, sconti e contratti di pagamento per le vendite](sales-how-record-sales-price-discount-payment-agreements.md).
13. Per aggiungere un commento sulla riga dell'offerta che il cliente può vedere sull'offerta di vendita stampata, scrivere un testo nel campo **Descrizione** nella riga vuota.  
14. Ripetere i passaggi da 10 a 13 per ogni articolo che si desidera offrire al cliente.

    I totali sotto le righe vengono automaticamente calcolati quando si creano o si modificano le righe.
15. Nel campo **Importo sconto fattura** immettere un importo che deve essere dedotto dal valore indicato nel campo **Totale IVA incl.**.

    **Nota**: se sono stati impostati degli sconti su fattura per il cliente, il valore percentuale specificato viene automaticamente inserito nel campo **% sconto fattura** se vengono soddisfatti i criteri e l'importo correlato viene inserito nel campo **Importo sconto fatt. IVA esclusa**. Per ulteriori informazioni, vedere [Registrazione di prezzi, sconti e contratti di pagamento per le vendite](sales-how-record-sales-price-discount-payment-agreements.md).
16. Una volta completate le righe dell'offerta di vendita, scegliere l'azione **E-mail** o **Stampa**.

    Se si seleziona l'azione **E-mail**, viene automaticamente allegato un file PDF a un'e-mail per il cliente. È possibile impostare l'e-mail in modo che includa un riepilogo dell'offerta. Per ulteriori informazioni, vedere [Procedura: Inviare documenti via e-mail](ui-how-send-documents-email.md).
17. Se il cliente accetta l'offerta, scegliere l'azione **Crea fattura** o **Crea ordine**.

L'offerta di vendita viene rimossa dal database. Viene creata una fattura, o un ordine, di vendita basata sulle informazioni contenute nell'offerta di vendita nella quale è possibile elaborare la vendita. Nel campo **Nr. offerta** della fattura di vendita, o dell'ordine di vendita, è possibile vedere il numero dell'offerta di vendita da cui è stata creata la fattura. Per ulteriori informazioni vedere [Procedura: Fatturare le vendite](sales-how-invoice-sales.md) o [Procedura: Vendere prodotti](sales-how-sell-products.md).

## <a name="see-also"></a>Vedi anche  
[Gestire le vendite](sales-manage-sales.md)  
[Impostare le vendite](sales-setup-sales.md)  
[Procedura: Inviare documenti via e-mail](ui-how-send-documents-email.md)  
[Utilizzare Dynamics NAV](ui-work-product.md)

