---
title: Creare e gestire gli articoli non in stock
description: Descrive come vendere gli articoli non inventariabili o non gestiti in magazzino.
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: non-inventoriable
ms.date: 06/02/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: dd1497d0727935d4954f826eceb303761850dada
ms.contentlocale: it-it
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-work-with-nonstock-items"></a>Procedura: Utilizzare gli articoli non in stock
È possibile offrire per loro comodità determinati articoli ai clienti che non si desidera mantenere in magazzino fino a quando non si inizia a venderli. Se si desidera iniziare a mantenere tali articoli in magazzino, è possibile convertirli in schede articolo normali in due modi.

* Dalla scheda articolo non in stock, creare una nuova scheda articolo in base a un modello.
* Da una riga di ordine di vendita di tipo **Articolo** con un campo vuoto **No**, selezionare un articolo non in stock. Una scheda articolo viene creata automaticamente per l'articolo non in stock.

> [!NOTE]  
>   Non è possibile selezionare un articolo non in stock dalla finestra **Fattura di vendita**. È possibile selezionare un articolo non in stock dalla finestra **Offerta di vendita**, ma l'articolo non in stock non verrà convertito in articolo normale quando si utilizza la funzione **Crea ordine**.

Un articolo non in stock ha in genere il numero di articolo del fornitore che lo fornisce. Per abilitare la conversione di una scheda articolo non in stock in una scheda articolo normale, è necessario impostare come la numerazione articolo fornitore viene convertita nella numerazione articolo dell'utente.   

## <a name="to-create-a-nonstock-item"></a>Per creare un articolo non in stock
Nelle schede articolo non in stock sono presenti molte informazioni in meno rispetto alle schede articolo normale perché vengono utilizzate solo per offrirle in offerte e in altri modi. Per tale motivo, devono essere convertite in schede articolo normale prima di registrare le transazioni di vendita relative.

1. Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **Articoli non in stock**, quindi scegliere il collegamento correlato.
2. Scegliere l'azione **Nuovo**.
3. Compilare i campi, se necessario. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

## <a name="to-set-up-how-nonstock-item-numbers-are-converted-to-your-own-numbering"></a>Per impostare come i numeri articolo non in stock vengono convertiti nella numerazione dell'utente
Per abilitare la conversione di una scheda articolo non in stock in una scheda articolo normale, è necessario impostare la modalità con cui la numerazione articolo fornitore viene convertita nel formato di numerazione articolo dell'utente.

1. Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **Setup articolo non in stock**, quindi scegliere il collegamento correlato.
2. Compilare i campi, se necessario.

## <a name="to-convert-a-nonstock-item-to-a-normal-item"></a>Per convertire un articolo non in stock in articolo normale
1. Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **Articoli non in stock**, quindi scegliere il collegamento correlato.
2. Aprire la scheda dell'articolo non in stock da convertire in articolo normale.
3. Nella finestra **Scheda articolo non in stock** scegliere l'azione **Crea articolo**.

Verrà visualizzata una nuova scheda articolo precompilata con le informazioni dell'articolo non in stock e viene creato un modello articolo relativo. È possibile immettere o modificare i campi della nuova scheda articolo secondo le necessità. Per ulteriori informazioni, vedere [Procedura: Registrare nuovi articoli](inventory-how-register-new-items.md).

## <a name="to-sell-a-nonstock-item-and-convert-it-to-a-normal-item"></a>Per vendere un articolo non in stock e convertirlo in articolo normale
1. Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **Ordini di vendita**, quindi scegliere il collegamento correlato.
2. Scegliere l'azione **Nuovo**. Compilare i campi nella Scheda dettaglio **Generale** come per qualsiasi ordine di vendita. Per ulteriori informazioni, vedere [Procedura: Vendere prodotti](sales-how-sell-products.md).
3. In una nuova riga vendite, nel campo **Tipo**, selezionare **Articolo**, ma lasciare **Nr.** essere lasciato vuoto.
4. Scegliere l'azione **Riga**, quindi l'azione **Selezionare articoli non in stock**.

    L'articolo non in stock viene convertito in articolo normale. Verrà visualizzata una nuova scheda articolo precompilata con le informazioni dell'articolo non in stock e viene creato un modello articolo relativo.
5. Nella finestra **Articoli non in stock** selezionare l'articoli non in stock che si desidera vendere, quindi scegliere **OK**.
6. Una volta completato l'ordine di vendita, scegliere l'azione **Registra**.

È possibile immettere o modificare i campi della nuova scheda articolo secondo le necessità. Per ulteriori informazioni, vedere [Procedura: Registrare nuovi articoli](inventory-how-register-new-items.md).

> [!NOTE]  
>   Un record di cross reference articolo viene creato automaticamente per il fornitore dell'articolo tra il numero dell'articolo fornitore e il nuovo numero dell'articolo.

## <a name="see-also"></a>Vedi anche
[Procedura: Registrare nuovi articoli](inventory-how-register-new-items.md)  
[Procedura: Creare ordini speciali](sales-how-to-create-special-orders.md)|  
[Magazzino](inventory-manage-inventory.md)  
[Utilizzo di [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

