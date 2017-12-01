---
title: Come fare un'offerta per una vendita assemblaggio su ordine
description: "È possibile utilizzare gestione assemblaggio per personalizzare un articolo di assemblaggio nella richiesta di un cliente durante il processo di vendita."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/15/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 7ee62ddff43778bd81d4ed65c2dcdd466b79e422
ms.contentlocale: it-it
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-quote-an-assemble-to-order-sale"></a>Procedura: Fare un'offerta per una vendita assemblaggio su ordine
È possibile utilizzare gestione assemblaggio per personalizzare un articolo di assemblaggio nella richiesta di un cliente durante il processo di vendita. Per ulteriori informazioni, vedere [Procedura: Vendere articoli assemblati su ordine](assembly-how-to-sell-items-assembled-to-order.md).  

Come per la vendita di qualsiasi altro tipo di articolo, è inoltre possibile creare un'offerta di vendita di un articolo di assemblaggio personalizzato prima della conversione in ordine di vendita. Questo processo prevede diversi passaggi aggiuntivi se viene confrontato alla creazione di un'offerta di vendita normale e utilizza una variazione di un ordine di assemblaggio collegato, ossia un'offerta di assemblaggio.

> [!NOTE]  
>  Come in tutti i tipi di offerte, le quantità nelle offerte di assemblaggio non vengono utilizzate per la disponibilità, la pianificazione o gli impegni.  

## <a name="to-create-a-sales-quote-for-an-assemble-to-order-item"></a>Per creare un'offerta di vendita per un articolo assemblato su ordine  
1.  Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **Offerte di vendita**, quindi scegliere il collegamento correlato.  
2.  Creare una riga dell'offerta di vendita con una riga per un articolo di assemblaggio. Per ulteriori informazioni, vedere [Procedura: Fare offerte](sales-how-make-offers.md).  
3.  Nel campo **Qtà per assemblaggio su ordine** immettere la quantità completa.

    > [!NOTE]  
    >  Non si crea un'offerta per una quantità parziale. Di conseguenza, è necessario immettere la stessa quantità immessa nel campo **Quantità** della riga dell'offerta di vendita.  

4.  Nella Scheda dettaglio **Righe** scegliere **Riga**, **Assemblaggio su ordine**, quindi **Righe di assemblaggio su ordine**. In alternativa, scegliere il campo **Qtà per assemblaggio su ordine** della riga.  
5.  Nella finestra **Righe di assemblaggio su ordine** esaminare o modificare le righe dell'ordine di assemblaggio in base all'offerta richiesta dal cliente. Se si desidera visualizzare altre informazioni, scegliere l'azione **Mostra documento** per aprire l'ordine dell'offerta programmata completo. Non è possibile modificare il contenuto della maggior parte dei campi né effettuare la registrazione.  
6.  Dopo avere rettificato le righe dell'ordine di assemblaggio in base all'offerta, chiudere la finestra **Righe di assemblaggio su ordine** per tornare alla finestra **Offerta vendita**.  
7.  Se il cliente accetta l'offerta, creare un ordine di vendita per l'articolo di assemblaggio offerto. Per ulteriori informazioni, vedere [Procedura: Fare offerte](sales-how-make-offers.md). L'offerta di assemblaggio collegata ed eventuali personalizzazioni sono collegate al nuovo ordine di vendita per preparare l'assemblaggio dell'articolo o degli articoli da vendere.  

## <a name="see-also"></a>Vedi anche  
[Gestione assemblaggio](assembly-assemble-items.md)  
[Procedura: Utilizzare le distinte base](inventory-how-work-BOMs.md)  
[Magazzino](inventory-manage-inventory.md)  
[Dettagli di progettazione: Gestione warehouse](design-details-warehouse-management.md)  
[Utilizzo di [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

