---
title: 'Procedura: Registrare nuovi prodotti'
author: SorenGP
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: df84a4d3e15035cd956c7612a12069844f5601d2
ms.contentlocale: it-it
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-register-new-products"></a>Procedura: Registrare nuovi prodotti

I prodotti sono alla base dell'azienda, delle merci o dei servizi di commercio. Ogni prodotto deve essere registrata come scheda articolo.

**Nota**: in Dynamics NAV un prodotto viene indicato con il termine “articolo”.

Le schede articolo contengono le informazioni richieste per l'acquisto, l'archiviazione, la consegna e la contabilità dei prodotti.

La scheda articolo può essere di tipo Magazzino o Assistenza per specificare se il prodotto corrisponde a un'unità fisica o a un'unità di tempo di lavoro. Oltre ad alcuni campi correlati agli aspetti fisici di un articolo, tutti i campi della scheda articolo funzionano in modo analogo per gli articoli e i servizi di magazzino. Per ulteriori informazioni sulla vendita di un articolo, vedere [Procedura: Vendere prodotti](sales-how-sell-products.md) o [Procedura: Fatturare le vendite](sales-how-invoice-sales.md).

**Nota**: se esistono i modelli articolo per diversi tipi di articolo, allora verrà visualizzata una finestra quando si crea una nuova scheda articolo da cui è possibile selezionare un modello appropriato. Se esiste solo un modello articolo, allora le nuove schede articolo utilizzeranno sempre tale modello.

## <a name="to-create-a-new-item-card"></a>Per creare una nuova scheda articolo
1. Nella home page scegliere l'azione **Articoli** per aprire l'elenco degli articoli esistenti.  
2. Nella finestra **Articoli** scegliere l'azione **Nuovo**.

    Se esiste solo un modello articolo, allora verrà visualizzata una nuova scheda articolo con alcuni campi compilati con le informazioni derivanti dal modello.
3. Nella finestra **Selezionare un modello per un nuovo articolo** scegliere il modello da utilizzare per la nuova scheda articolo.
4. Scegliere il pulsante **OK**. Una nuova scheda articolo verrà visualizzata con alcuni campi compilati con le informazioni del modello.
5. Continuare a compilare o a modificare i campi della scheda articolo in base alle necessità. Selezionare il campo per visualizzare una breve descrizione del campo o il collegamento a ulteriori informazioni.

Nella Scheda dettaglio **Prezzi vendita** è possibile visualizzare gli sconti o i prezzi speciali che si concedono per l'articolo se vengono soddisfatti determinati criteri come un cliente, la quantità minima di ordine o la data di scadenza. Ogni riga rappresenta un prezzo speciale o uno sconto riga. Ogni colonna rappresenta un criterio da applicare per garantire il prezzo speciale immesso nel campo **Prezzo unitario** o lo sconto riga immesso nel campo **Sconto riga**. Per ulteriori informazioni, vedere [Registrazione di prezzi, sconti e contratti di pagamento per le vendite](sales-how-record-sales-price-discount-payment-agreements.md).

L'articolo è ora registrato e la scheda articolo è pronta per essere utilizzata nei documenti di acquisto e vendita.

Se si desidera utilizzare questa scheda articolo come modello quando si creano nuove schede articolo, è possibile salvarla come modello. Per ulteriori informazioni, vedere la seguente sezione:

## <a name="to-save-the-item-card-as-a-template"></a>Per salvare la scheda articolo come modello
1. Nella finestra **Scheda articolo** scegliere l'azione **Salva come modello**. Nella finestra **Modello articolo** verrà visualizzata la scheda articolo come modello.
2. Compilare i campi, se necessario. Selezionare il campo per visualizzare una breve descrizione del campo o il collegamento a ulteriori informazioni.
3. Per riutilizzare le dimensioni nei modelli, selezionare l'azione **Dimensioni**. Nella finestra **Modelli dimensioni** verranno visualizzati tutti i codici di dimensione impostati per l'articolo.
4. Modificare o immettere i codici di dimensione da collegare alle nuove schede articolo create utilizzando la definizione.
5. Una volta completato il nuovo modello articolo, scegliere **OK**.

Il modello articolo viene aggiunto all'elenco dei modelli articolo, in modo che sia possibile utilizzarlo per creare nuove schede articolo.

## <a name="see-also"></a>Vedi anche
  [Gestire i costi del magazzino](inventory-manage-inventory.md)  
  [Gestire gli acquisti](purchasing-manage-purchasing.md)  
  [Gestire le vendite](sales-manage-sales.md)

