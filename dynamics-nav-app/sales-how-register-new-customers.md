---
title: 'Procedura: Registrare nuovi clienti'
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
ms.openlocfilehash: 191a9d0b38425c2e36400050afa4fa89ccd2556a
ms.contentlocale: it-it
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-register-new-customers"></a>Procedura: Registrare nuovi clienti
I clienti sono l'origine del reddito. Ogni cliente a cui è stata effettuata una vendita deve essere registrato come una scheda cliente.

Prima di registrare nuovi clienti, è necessario impostare vari codici di vendita che sarà possibile selezionare durante la compilazione delle schede cliente. Per ulteriori informazioni, vedere [Impostare le vendite](sales-setup-sales.md).

Le schede cliente contengono le informazioni richieste per la vendita dei prodotti al cliente. Per ulteriori informazioni, vedere [Procedura: Fatturare le vendite](sales-how-invoice-sales.md) e [Procedura: Registrare nuovi prodotti](inventory-how-register-new-products.md).

**Nota**: se esistono i modelli cliente per diversi tipi di cliente, quando si crea una nuova scheda cliente, verrà visualizzata una finestra automaticamente da cui sarà possibile selezionare un modello appropriato. Se esiste solo un modello cliente, allora le nuove schede cliente utilizzeranno sempre tale modello.

## <a name="to-create-a-new-customer-card"></a>Per creare una nuova scheda cliente
1. Nella home page scegliere l'azione **Clienti** per aprire l'elenco dei clienti esistenti.  
2. Nella finestra **Clienti** scegliere l'azione **Nuovo**.

    Se esiste solo un modello cliente, allora verrà visualizzata una nuova scheda cliente con alcuni campi compilati con le informazioni derivanti dal modello.

    Se esistono più modelli cliente, verrà aperta una finestra nella quale sarà possibile selezionare un modello cliente. In questo caso, seguire i due passaggi successivi.
3. Nella finestra **Selezionare un modello per un nuovo cliente** scegliere il modello da utilizzare per la nuova scheda cliente.
4. Scegliere il pulsante **OK**. Una nuova scheda cliente verrà visualizzata con alcuni campi compilati con le informazioni del modello.  
5. Continuare a compilare o a modificare i campi della scheda cliente in base alle necessità. Selezionare il campo per visualizzare una breve descrizione del campo o il collegamento a ulteriori informazioni.

Nella Scheda dettaglio **Prezzi vendita** è possibile visualizzare gli sconti o i prezzi speciali che si concedono al cliente se vengono soddisfatti determinati criteri come un articolo, la quantità minima di ordine o la data di scadenza. Ogni riga rappresenta un prezzo speciale o uno sconto riga. Ogni colonna rappresenta un criterio da applicare per garantire il prezzo speciale immesso nel campo **Prezzo unitario** o lo sconto riga immesso nel campo **Sconto riga**. Per ulteriori informazioni, vedere [Registrazione di prezzi, sconti e contratti di pagamento per le vendite](sales-how-record-sales-price-discount-payment-agreements.md).

Il cliente è ora registrato e la scheda cliente è pronta per essere utilizzata nei documenti di vendita.

Se si desidera utilizzare questa scheda cliente come modello quando si creano nuove schede cliente, è possibile salvarla come modello. Per ulteriori informazioni, vedere la seguente sezione:

## <a name="to-save-the-customer-card-as-a-template"></a>Per salvare la scheda cliente come modello
1. Nella finestra **Scheda cliente** scegliere l'azione **Salva come modello**. Nella finestra **Modello cliente** verrà visualizzata la scheda cliente come modello.
2. Compilare i campi, se necessario. Selezionare il campo per visualizzare una breve descrizione del campo o il collegamento a ulteriori informazioni.
3. Per riutilizzare le dimensioni nei modelli, selezionare l'azione **Dimensioni**. Verrà visualizzata la finestra **Modelli dimensioni** nella quale saranno indicati tutti i codici per le dimensioni che sono impostati per il cliente.
4. Modificare o immettere i codici di dimensione da collegare alle nuove schede cliente create utilizzando la definizione.  
5. Una volta completato il nuovo modello cliente, fare clic su **OK**.

Il modello cliente viene aggiunto all'elenco dei modelli cliente, in modo che sia possibile utilizzarlo per creare nuove schede cliente.

## <a name="see-also"></a>Vedi anche  
[Gestire le vendite](sales-manage-sales.md)    
[Impostare le vendite](sales-setup-sales.md)    
[Utilizzare Dynamics NAV](ui-work-product.md)

