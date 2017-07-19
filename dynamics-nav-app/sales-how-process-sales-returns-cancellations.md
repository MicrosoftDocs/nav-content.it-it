---
title: 'Procedura: Elaborare i resi o gli annullamenti vendite'
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
ms.openlocfilehash: 92b65379f2ec633712a2b2c0f06615c6de61cc6e
ms.contentlocale: it-it
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-process-sales-returns-or-cancellations"></a>Procedura: Elaborare i resi o gli annullamenti vendite
Se il cliente desidera restituire gli articoli o ottenere il rimborso per degli articoli o dei servizi vendutigli, è necessario creare e registrare una nota di credito di vendita in cui viene specificata la modifica richiesta. Per includere le informazioni corrette della fattura di vendita, è possibile creare la nota di credito di vendita da una fattura di vendita registrata o utilizzare la funzione di copia.

Oltre alla fattura di vendita registrata originale, è possibile collegare la nota di credito di vendita ad altri documenti di vendita, ad esempio un'altra fattura di vendita registrata, in quanto il cliente restituisce anche gli articoli consegnati con la fattura.

Un reso o un risarcimento può essere correlato solo ad alcuni degli articoli o dei servizi nella fattura di vendita originale. In questo caso, è necessario modificare le informazioni nelle righe della nota di credito di vendita. Quando si registra la nota di credito di vendita, i documenti di vendita influenzati dalla variazione vengono stornati ed è possibile creare un pagamento di rimborso per il cliente.

È possibile inviare la nota di credito vendita registrata al cliente per confermare il reso o l'annullamento e comunicare che il valore correlato verrà rimborsato, ad esempio quando gli articoli vengono resi.

## <a name="to-create-a-sales-credit-memo-from-a-posted-sales-invoice"></a>Per creare una nuova nota di credito di vendita da una fattura di vendita registrata
1. Nell'angolo superiore destro, scegliere l'icona **Cerca pagina o report**, immettere **Fatture vendite registrate**, quindi scegliere il collegamento correlato.  
2. Nella finestra **Fatture vendita registrate** selezionare la fattura di vendita registrata che si desidera stornare, quindi scegliere l'azione **Crea nota credito di rettifica**.

    La maggior parte dei campi nella testata della nota di credito di vendita viene compilata con le informazioni della fattura di vendita registrata. È possibile modificare tutti i campi, ad esempio con nuove informazioni che riflettono il contratto di reso.
3. Modificare le informazioni nelle righe in base al contratto, quali il numero di articoli resi o l'importo da rimborsare.
4. Scegliere l'azione **Collega movimenti**.
5. Nella finestra **Collega movimenti clienti**, selezionare la riga con il documento di vendita registrato a cui si desidera collegare la nota di credito di vendita, quindi scegliere l'azione **Collega-a ID**.

    Il numero della nota di credito di vendita viene inserito nel campo **Collega-a ID**.  
6. Nel campo **Importo da collegare** immettere l'importo che si desidera collegare se inferiore all'importo originale.

    Nella parte inferiore della finestra **Collega movimenti clienti** è possibile vedere l'importo totale da collegare per stornare tutti i movimenti coinvolti, ad esempio quando il valore del campo **Saldo** è zero.  
7. Scegliere il pulsante **OK**. Quando si registra la nota di credito di vendita, verrà applicata ai documenti di vendita registrati specificati.

    Dopo avere creato o modificato le righe della nota di credito di vendita necessarie e aver specificato uno o più collegamenti, è possibile passare alla registrazione della nota di credito di vendita.
8. Scegliere l'azione **Registra e invia**.

Viene visualizzata la finestra di dialogo **Registra e invia conferma** contenente il metodo di invio preferito del cliente. È possibile modificare il metodo di invio scegliendo il pulsante di ricerca per il campo **Invia documento a**. Per ulteriori informazioni, vedere [Procedura: Impostare profili di invio documenti](sales-how-setup-document-send-profiles.md).

I documenti di vendita registrati che sono stati collegati alla nota di credito sono ora stornati ed è possibile creare un pagamento del rimborso per il cliente. La nota di credito di vendita viene rimossa e sostituita con un nuovo documento nell'elenco delle note di credito di vendita registrate.

## <a name="to-create-a-sales-credit-memo-from-scratch"></a>Per creare una nota di credito di vendita da zero
1. Nell'angolo superiore destro, scegliere l'icona **Cerca pagina o report**, immettere **Fatture vendite registrate**, quindi scegliere il collegamento correlato.
2. Scegliere l'azione **Nuovo** per aprire una nuova nota di credito di vendita vuota.
3. Nel campo **Cliente** immettere il nome di un cliente esistente.
4. Scegliere l'azione **Copia documento**.
5. Nella finestra **Copia documento vendita**, nel campo **Tipo di documento**, selezionare **Fattura registrata**.
6. Scegliere il campo **Nr. documento** per aprire la finestra **Fatture vendita registrate**, quindi selezionare la fattura di vendita registrata che contiene le righe da stornare.
7. Selezionare la casella di controllo **Ricalcola righe** se si desidera che le righe copiate della fattura di vendita registrata vengano aggiornate con le modifiche al prezzo dell'articolo e al costo unitario poiché la fattura è stata registrata.
8. Scegliere il pulsante **OK**. Le righe della fattura copiate vengono inserite nella nota di credito vendite.
9. Completare la nota di credito di vendita come descritto nella sezione "Per creare una nota di credito di vendita da una fattura di vendita registrata" del presente argomento.

## <a name="see-also"></a>Vedi anche  
[Gestire le vendite](sales-manage-sales.md)  
[Impostare le vendite](sales-setup-sales.md)  
[Procedura: Inviare documenti via e-mail](ui-how-send-documents-email.md)  
[Utilizzare Dynamics NAV](ui-work-product.md)

