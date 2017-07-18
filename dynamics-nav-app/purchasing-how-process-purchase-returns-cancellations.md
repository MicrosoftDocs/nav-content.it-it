---
title: 'Procedura: Elaborare i resi o gli annullamenti acquisti'
author: SorenGP
ms.custom: na
ms.date: 11/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: 94067fb3d10975c1db29d2e3f1d5d6373fcbf9f2
ms.contentlocale: it-it
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-process-purchase-returns-or-cancellations"></a>Procedura: Elaborare i resi o gli annullamenti acquisti
Se si desidera restituire gli articoli al fornitore o annullare l'assistenza acquistata, è possibile creare e registrare una nota di credito di acquisto in cui viene specificata la modifica richiesta rispetto alla fattura di acquisto originale. Per includere le informazioni corrette della fattura di acquisto, è possibile creare la nota di credito di acquisto da una fattura d'acquisto registrata o utilizzare la funzione di copia.

In genere, si crea una nota di credito di acquisto in risposta a una nota di credito inviata da un fornitore. La nota di credito di acquisto funziona come la documentazione interna del processo relativo alla nota di credito per scopi contabili.

La modifica può essere correlata a tutti o solo ad alcuni prodotti nella fattura di acquisto originale. Di conseguenza, è possibile restituire parzialmente gli articoli ricevuti o richiedere il risarcimento parziale dei servizi ricevuti. In questo caso, è necessario modificare le informazioni della fattura di acquisto copiata.

Oltre alla fattura di acquisto registrata originale, è possibile collegare la nota di credito di acquisto ad altri documenti di acquisto, ad esempio un'altra fattura di acquisto registrata, in quanto si restituiscono anche gli articoli consegnati con la fattura.

## <a name="to-create-a-purchase-credit-memo-from-a-posted-purchase-invoice"></a>Per creare una nota di credito di acquisto da una fattura di acquisto registrata
1. Nell'angolo superiore destro, scegliere l'icona **Cerca pagina o report**, immettere **Note credito acquisto**, quindi scegliere il collegamento correlato.  
2. Nella finestra **Fatture acquisto registrate** selezionare la fattura di acquisto registrata che si desidera stornare, quindi scegliere l'azione **Crea nota credito di rettifica**.

    La maggior parte dei campi nella testata della nota di credito di acquisto viene compilata con le informazioni della fattura di acquisto registrata. È possibile modificare tutti i campi, ad esempio con nuove informazioni che riflettono il contratto di reso.
3. Modificare le informazioni nelle righe in base al contratto, quali il numero di articoli resi o l'importo da rimborsare.
4. Scegliere l'azione **Collega movimenti**.
5. Nella finestra **Collega movimenti fornitori**, selezionare la riga con il documento di acquisto registrato a cui si desidera collegare la nota di credito di acquisto, quindi scegliere l'azione **Collega-a ID**. Il numero della nota di credito di acquisto viene inserito nel campo **Collega-a ID**.
6. Nel campo **Importo da collegare** immettere l'importo che si desidera collegare se inferiore all'importo originale.

    Nella parte inferiore della finestra **Collega movimenti fornitori** è possibile vedere l'importo totale da collegare per stornare tutti i movimenti coinvolti, ad esempio quando il valore del campo **Saldo** è zero.
7. Scegliere il pulsante **OK**. Quando si registra la nota di credito di acquisto, verrà collegata ai documenti di acquisto registrati specificati.

    Dopo avere creato o modificato le righe della nota di credito di acquisto necessarie e aver specificato uno o più collegamenti, è possibile passare alla registrazione della nota di credito di acquisto.
8. Scegliere l'azione **Registra**.

Le fatture di acquisto registrate a cui si applica la nota di credito vengono ora stornate. Se è già stata pagata la fattura originale, il fornitore dovrà rimborsare il pagamento. Se la nota di credito riguarda solo parte del prodotto nella fattura originale, è possibile pagare solo l'importo restante nella fattura di acquisto originale per chiuderla.

La nota di credito di acquisto viene rimossa e sostituita con un nuovo documento nell'elenco delle note di credito di acquisto registrate.

## <a name="to-create-a-purchase-credit-memo-from-scratch"></a>Per creare una nota di credito di acquisto da zero
1. Nell'angolo superiore destro, scegliere l'icona **Cerca pagina o report**, immettere **Fatture acquisto registrate**, quindi scegliere il collegamento correlato.
2. Scegliere l'azione **Nuovo** per aprire una nuova nota di credito di acquisto vuota.
3. Nel campo **Fornitore** immettere il nome del fornitore esistente.
4. Scegliere l'azione **Copia documento**.
5. Nella finestra **Copia documento acquisto**, nel campo **Tipo di documento**, selezionare **Fattura registrata**.
6. Scegliere il campo **Nr. documento** per aprire la finestra **Fatture acquisto registrate**, quindi selezionare la fattura di acquisto registrata che contiene le righe da stornare.
7. Selezionare la casella di controllo **Ricalcola righe** se si desidera che le righe copiate della fattura di acquisto registrata vengano aggiornate con le modifiche al prezzo dell'articolo e al costo unitario poiché la fattura è stata registrata.
8. Scegliere il pulsante **OK**. Le righe della fattura copiate vengono inserite nella nota di credito di acquisto.
9. Completare la nota di credito acquisto come descritto nella sezione "Per creare una nota di credito di acquisto da una fattura di acquisto registrata" del presente argomento.

## <a name="see-also"></a>Vedi anche
[Gestire gli acquisti](purchasing-manage-purchasing.md)  
[Procedura: Registrare gli acquisti](purchasing-how-record-purchases.md)  

