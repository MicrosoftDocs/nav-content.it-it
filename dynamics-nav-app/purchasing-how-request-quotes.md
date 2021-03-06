---
title: Creare un'offerta di acquisto per richiedere un'offerta dal fornitore
description: Descrive come creare un documento di un'offerta di vendita o una richiesta di offerta (RdO) per registrare la propria offerta a un cliente per la vendita di prodotti in base a termini determinati.
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: rfq
ms.date: 08/08/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 615f40834b26826edafbfc70eb82db969c6d3d4c
ms.contentlocale: it-it
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-request-quotes"></a>Procedura: Richiedere le offerte
Un'offerta di acquisto può essere utilizzata come bozza preliminare di un ordine di acquisto e l'ordine può essere in seguito convertito in ordine o fattura di acquisto.


## <a name="to-create-a-purchase-quote"></a>Per creare un'offerta di acquisto
1. Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **Offerte di acquisto**, quindi scegliere il collegamento correlato.
2. Creare un nuovo documento nello stesso modo in cui si crea un ordine di acquisto. Per ulteriori informazioni, vedere [Procedura: Registrare gli acquisti](purchasing-how-record-purchases.md).

## <a name="to-convert-a-purchase-quote-to-a-purchase-order"></a>Per convertire un'offerta di acquisto in un ordine di acquisto
Una volta che l'offerta fornitore viene accettata, può essere convertita in fattura o ordine di acquisto per elaborare l'acquisto.

1. Aprire un'offerta di acquisto pronta per essere convertita e scegliere l'azione **Crea ordine**.

L'offerta di acquisto viene rimossa dal database. Viene creata una fattura, o un ordine, di acquisto basata sulle informazioni contenute nell'offerta di acquisto nella quale è possibile elaborare l'acquisto. Nel campo **Nr. offerta** dell'ordine o della fattura di acquisto è presente il numero dell'offerta di acquisto da cui è stato convertito.

## <a name="see-also"></a>Vedi anche
[Acquisti](purchasing-manage-purchasing.md)  
[Impostazioni acquisti](purchasing-setup-purchasing.md)  
[Procedura: Inviare documenti via e-mail](ui-how-send-documents-email.md)  
[Utilizzo di [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

