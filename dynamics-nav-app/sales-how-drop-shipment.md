---
title: Creare un ordine di vendita collegato a un ordine di acquisto per una spedizione diretta
description: Viene descritto come creare un ordine di vendita collegato a un ordine di acquisto per consentire la spedizione diretta dal fornitore al cliente.
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: direct shipment
ms.date: 03/29/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 6a8210808532ff8945660c23f0bf91719e2f2963
ms.contentlocale: it-it
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-make-drop-shipments"></a>Procedura: Effettuare spedizioni dirette
Una spedizione diretta è costituita dalla spedizione di articoli direttamente da un fornitore a un cliente.

Quando un ordine di vendita è contrassegnato per la spedizione diretta e si crea un ordine di acquisto specificando il cliente nel campo **Vendere a - Nr. cliente**, è possibile collegare due documenti e istruire il fornitore di spedire direttamente al cliente.

## <a name="to-create-a-sales-order-for-drop-shipment"></a>Per creare un ordine di vendita per una spedizione diretta
Per preparare una spedizione diretta, si crea un ordine di vendita per un articolo come al solito, ad eccezione del fatto che è necessario indicare sulla riga di vendita che la vendita richiede la spedizione diretta.

1. Creare un ordine cliente per un articolo. Per ulteriori informazioni, vedere [Procedura: Vendere prodotti](sales-how-sell-products.md).
2. Nella riga ordine di vendita per la spedizione diretta selezionare la casella di controllo **Spedizione diretta**. Utilizzare la funzione **Scegli colonne** se il campo non è visualizzato. Per ulteriori informazioni, vedere [Personalizzazione utente](ui-user-personalization.md).

## <a name="to-create-the-purchase-order-for-drop-shipment"></a>Per creare l'ordine di acquisto per la spedizione diretta
Per preparare una spedizione diretta per l'articolo da vendere, si crea un ordine di acquisto come al solito, ad eccezione del fatto che è necessario indicare nell'ordine di acquisto che deve essere spedito al cliente e non a se stessi.

1. Creare un ordine di acquisto. Non compilare i campi nelle righe. Per ulteriori informazioni, vedere [Procedura: Registrare gli acquisti](purchasing-how-record-purchases.md).
2. Nel campo **Vendere a - Nr. cliente** selezionare il cliente a cui si sta vendendo.
3. Scegliere l'azione **Spedizioni dirette** e scegliere l'azione **Ottieni ordini vendite**.
4. Nella finestra **Lista vendite**, selezionare l'ordine di vendita che è stato preparato nella sezione "Per creare un ordine di vendita per una spedizione diretta".
5. Scegliere il pulsante **OK**.

Le informazioni di riga dall'ordine di vendita vengono inserite nelle righe dell'ordine di acquisto.

È possibile istruire il fornitore di spedire gli articoli al cliente, ad esempio spedendo l'ordine di acquisto come PDF.     

## <a name="to-view-the-linked-purchase-order-from-the-sales-order"></a>Per visualizzare l'ordine di acquisto collegato dall'ordine di vendita
* Selezionare la riga dell'ordine di vendita con spedizione diretta, scegliere l'azione **Ordine**, scegliere l'azione **Spedizione diretta** e quindi scegliere l'azione **Ordine acquisto**.

## <a name="to-post-a-drop-shipment"></a>Per registrare una spedizione diretta
Dopo che il fornitore ha spedito gli articoli, è possibile registrare l'ordine di vendita come spedito. È possibile registrare anche l'ordine di acquisto, ma solo con l'opzione **Ricevi** finché l'ordine di vendita non viene fatturato.

1. Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **Ordini di vendita**, quindi scegliere il collegamento correlato.
2. Aprire l'ordine di vendita creato nella sezione "Per creare un ordine di vendita per una spedizione diretta".
3. Nel campo **Qtà da spedire**, specificare la quantità dell'ordine da spedire, la quantità dell'ordine completa o parziale.
4. Scegliere l'azione **Registra** o **Registra e invia**.
5. Selezionare l'opzione **Spedizione** per fatturare in seguito oppure l'opzione **Spedisci e fattura** per fatturare immediatamente.

## <a name="see-also"></a>Vedi anche
[Procedura: Creare ordini speciali](sales-how-to-create-special-orders.md)|  
[Procedura: Vendere prodotti](sales-how-sell-products.md)  
[Procedura: Registrare gli acquisti](purchasing-how-record-purchases.md)  
[Vendite](sales-manage-sales.md)  
[Magazzino](inventory-manage-inventory.md)  
[Utilizzo di [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

