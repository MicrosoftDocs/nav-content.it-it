---
title: 'Procedura: Effettuare spedizioni dirette'
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
ms.openlocfilehash: f636de789dc6b006a449ec59c390fab85e62b443
ms.contentlocale: it-it
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-make-drop-shipments"></a>Procedura: Effettuare spedizioni dirette
Una spedizione diretta è costituita dalla spedizione di articoli direttamente da un fornitore a un cliente.

Quando un ordine di vendita è contrassegnato per la spedizione diretta e si crea un ordine di acquisto specificando il cliente nel campo **Vendere a - Nr. cliente**, è possibile collegare due documenti e istruire il fornitore di spedire direttamente al cliente.

## <a name="to-create-a-sales-order-for-drop-shipment"></a>Per creare un ordine di vendita per una spedizione diretta
Per preparare una spedizione diretta, si crea un ordine di vendita per un articolo come al solito, ad eccezione del fatto che è necessario indicare sulla riga di vendita che la vendita richiede la spedizione diretta.

1. Creare un ordine cliente per un articolo. Per ulteriori informazioni, vedere [Procedura: Vendere prodotti](sales-how-sell-products.md).
2. Nella riga ordine di vendita dell'articolo con spedizione diretta, selezionare la casella di controllo **Spedizione diretta**.

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
1. Selezionare la riga dell'ordine di vendita con spedizione diretta, scegliere l'azione **Ordine**, scegliere l'azione **Spedizione diretta** e quindi scegliere l'azione **Ordine acquisto**.

L'ordine di acquisto collegato viene aperto.

## <a name="to-post-a-drop-shipment"></a>Per registrare una spedizione diretta
Quando il fornitore ha spedito gli articoli, è possibile registrare l'ordine di vendita come spedito. È possibile registrare anche l'ordine di acquisto, ma solo con l'opzione **Ricevi** finché l'ordine di vendita non viene fatturato.
1. Nell'angolo superiore destro, scegliere l'icona **Cerca pagina o report**, immettere **Ordini di vendita**, quindi scegliere il collegamento correlato.
2. Aprire l'ordine di vendita creato nella sezione "Per creare un ordine di vendita per una spedizione diretta".
3. Nel campo **Qtà da spedire**, specificare la quantità dell'ordine da spedire, la quantità dell'ordine completa o parziale.
3. Scegliere l'azione **Registra** o **Registra e invia**.
4. Selezionare l'opzione **Spedizione** per fatturare in seguito oppure l'opzione **Spedisci e fattura** per fatturare immediatamente.

## <a name="see-also"></a>Vedi anche
[Procedura: vendere prodotti](sales-how-sell-products.md)    
[Procedura: Registrare gli acquisti](purchasing-how-record-purchases.md)  
[Gestire le vendite](sales-manage-sales.md)  
[Gestire i costi del magazzino](inventory-manage-inventory.md)      
[Utilizzare Dynamics NAV](ui-work-product.md)

