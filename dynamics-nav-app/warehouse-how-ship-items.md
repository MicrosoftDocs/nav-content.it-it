---
title: Come spedire articoli
description: "A seconda della configurazione della warehouse, è possibile registrare la spedizione del documento aziendale in uscita correlato, ad esempio un ordine di vendita, direttamente, oppure è possibile utilizzare i documenti di spedizione warehouse che rispettano un flusso di lavoro e si integrano alle diverse attività di warehouse."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/21/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 121f1e32d1fa265d4e059dc0ee43fad22f732472
ms.contentlocale: it-it
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-ship-items"></a>Procedura: Spedire articoli
Quando gli articoli partono da una warehouse che non è impostata per l'elaborazione delle spedizioni warehouse, occorre registrare semplicemente la spedizione nel documento aziendale correlato, ad esempio un ordine di vendita, un ordine di assistenza, un ordine di reso acquisto o un ordine di trasferimento in uscita.

Quando gli articoli vengono spediti da una warehouse impostata in modo da richiedere l'elaborazione delle spedizioni warehouse, è possibile spedire articoli solo in base ai documenti di origine rilasciati alla warehouse da altri reparti della società affinché vengano elaborati.

> [!NOTE]
> Se la warehouse prevede cross-docking e collocazioni, per ogni riga, è possibile visualizzare la quantità di articoli inseriti nelle collocazioni di cross-dock. Il programma calcola le quantità automaticamente ogni volta che i campi della spedizione vengono aggiornati. Se si tratta di articoli facenti parte della spedizione che si sta preparando, è possibile creare un prelievo per tutte le righe e completare la spedizione. Per ulteriori informazioni, vedere [Procedura: Articoli di cross-dock](warehouse-how-to-cross-dock-items.md).

## <a name="to-ship-items-with-a-sales-order"></a>Per spedire gli articoli con un ordine di vendita
Di seguito viene descritto come ricevere gli articoli con un ordine di acquisto. I passaggi riguardanti gli ordini di reso acquisto, gli ordini di assistenza e gli ordini di trasferimento in uscita sono simili.  
1. Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "Cerca pagina o report"), immettere **Ordini vendita**, quindi scegliere il collegamento correlato.
2. Aprire un ordine di vendita esistente o crearne uno. Per ulteriori informazioni, vedere [Procedura: Vendere prodotti](sales-how-sell-products.md).
3. Nel campo **Qtà da Spedire** immettere la quantità ricevuta.

    Il valore nel campo **Qtà spedita** viene aggiornato. Se si tratta di una spedizione parziale, il valore è inferiore al valore nel campo **Quantità**.
4. Scegliere l'azione **Registra**.

## <a name="to-ship-items-with-a-warehouse-shipment"></a>Per spedire gli articoli con una spedizione warehouse
Innanzitutto, creare un documento di spedizione da un documento di origine aziendale. Selezionare gli articoli specificati per la spedizione.

### <a name="to-create-a-warehouse-shipment"></a>Per creare una spedizione warehouse
In genere, l'impiegato responsabile della spedizione crea una spedizione warehouse.
1.  Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "Cerca pagina o report"), immettere **Spedizioni warehouse**, quindi scegliere il collegamento correlato.  
2.  Scegliere l'azione **Nuovo**.  

    Compilare i campi della Scheda dettaglio **Generale**. Quando si recuperano le righe dei documenti di origine, alcune informazioni vengono copiate in ciascuna riga.  

    Per la configurazione warehouse con stoccaggi e prelievi guidati, se l'ubicazione dispone di una zona e di una collocazione di default per le spedizioni, i campi **Cod. zona** e **Cod. Collocazione** vengono compilati automaticamente ma è possibile modificarli in base alle esigenze.  

    > [!NOTE]  
    >  Se si desidera spedire gli articoli con codici classe warehouse diversi dal codice classe della collocazione specificato nel campo **Cod. collocazione** della testata del documento, è necessario eliminare il contenuto del campo **Cod. collocazione** della testata prima di recuperare le righe del documento di origine per gli articoli.  
3.  Scegliere l'azione **Prendi documenti origine**. Verrà visualizzata la finestra **Documenti origine**.

    Da una spedizione warehouse nuova o aperta, è possibile utilizzare la finestra **Filtri per ottenere documenti origine** per recuperare le righe del documento di origine rilasciato che definiscono quali articoli spedire.

    1. Scegliere l'azione **Usa filtri per richiamare doc. orig.**.  
    2. Per impostare un nuovo filtro, immettere un codice descrittivo nel campo **Codice**, quindi scegliere l'azione **Modifica**.  
    3. Definire il tipo di righe del documento origine che si desidera recuperare compilando i campi Filtro appropriati.  
    4. Scegliere l'azione **Esegui**.  

    Tutte le righe del documento origine rilasciato che soddisfano i criteri di filtro vengono inserite nella finestra **Spedizione warehouse** da cui è stata attivata la funzione di filtro.  

    Le combinazioni di filtri definite vengono salvate nella finestra **Filtri per ottenere documenti origine** finché non saranno necessarie in momento successivo. È possibile creare un numero indefinito di combinazioni di filtri. È possibile modificare i criteri in qualsiasi momento scegliendo l'azione **Modifica**.

4.  Selezionare i documenti di origine per i quali si desidera spedire gli articoli, quindi scegliere **OK**.  

Le righe dei documenti di origine verranno visualizzate nella finestra **Spedizione warehouse**. Il campo **Qtà da spedire** viene compilato con la quantità inevasa per ciascuna riga, ma è possibile modificare tale quantità in base alle esigenze. Se è stato eliminato il contenuto del campo **Cod. collocazione** della Scheda dettaglio **Generale** prima di recuperare le righe, è necessario immettere un codice collocazione appropriato in ogni riga di spedizione.  

> [!NOTE]  
>  Non è possibile spedire un numero di articoli maggiore di quello indicato nel campo **Qtà inevasa** della riga del documento di origine. Per spedire più articoli, recuperare un altro documento di origine contenente una riga per l'articolo utilizzando la funzione di filtro appropriata.  

Dopo avere recuperato le righe per la spedizione, è possibile avviare il processo che consente di inviare le righe agli impiegati warehouse affinché procedano al prelievo.

### <a name="to-pick-and-ship"></a>Per prelevare gli articoli e procedere alla spedizione
In genere, un lavoratore warehouse responsabile del prelievo crea un documento di prelievo o apre un documento di prelievo già creato.
1. Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "Cerca pagina o report"), immettere **Spedizioni warehouse**, quindi scegliere il collegamento correlato.
2. Selezionare la spedizione warehouse da cui si desidera prelevare, quindi scegliere l'azione **Crea prelievo**.
3. Compilare i campi della finestra di richiesta, quindi fare clic sul pulsante **OK**. Verrà creato il documento di prelievo della warehouse specificato.

    In alternativa, aprire un prelievo warehouse esistente.
4. Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "Cerca pagina o report"), immettere **Prelievi**, quindi scegliere il collegamento correlato. Selezionare il prelievo warehouse che si desidera utilizzare.

    Se la warehouse è impostata per l'utilizzo delle collocazioni, le righe di prelievo vengono convertite in righe di azione Prendere e Mettere.

    È possibile ordinare le righe, assegnare un addetto al prelievo, impostare un filtro breakbulk, se si utilizzano stoccaggi e prelievi guidati, e stampare le istruzioni di prelievo.

5. Eseguire il prelievo effettivo degli articoli e posizionarli nella collocazione di spedizione specificata, o nell'area di spedizione, se non si utilizzano le collocazioni.
6. Scegliere l'azione **Registra prelievo**.

    I campi **Qtà da spedire** e **Stato del documento** nella testata del documento di spedizione verranno aggiornati. Gli articoli prelevati non saranno più disponibili per il prelievo per altre spedizioni o per operazioni interne.
7. Stampare i documenti di spedizione, preparare i colli per la spedizione e registrare la spedizione.

Per ulteriori informazioni sul prelievo per spedizioni warehouse, vedere [Procedura: Prelevare articoli per la spedizione warehouse](warehouse-how-to-pick-items-for-warehouse-shipment.md).

È anche possibile utilizzare il prospetto prelievi per combinare diverse istruzioni di prelievo in un'unica istruzione (per più spedizioni) e ottimizzare in tal modo le operazioni di prelievo nella warehouse. Per ulteriori informazioni, vedere [Procedura: Pianificare i prelievi nei prospetti](warehouse-how-to-plan-picks-in-worksheets.md).

> [!NOTE]
> Se si sta attendendo l'arrivo di determinati articoli nella warehouse e si utilizza la funzionalità di cross-dock, per ciascuna riga di spedizione o del prospetto prelievi in [!INCLUDE[d365fin](includes/d365fin_md.md)] verrà calcolata la quantità dell'articolo disponibile nella collocazione di cross-dock. Tale valore viene aggiornato ogni volta che si apre e si chiude il prospetto o il documento di spedizione. Per ulteriori informazioni, vedere [Procedura: Articoli di cross-dock](warehouse-how-to-cross-dock-items.md).

## <a name="see-also"></a>Vedi anche  
[Gestione warehouse](warehouse-manage-warehouse.md)  
[Magazzino](inventory-manage-inventory.md)  
[Impostazione gestione warehouse](warehouse-setup-warehouse.md)     
[Gestione assemblaggio](assembly-assemble-items.md)    
[Dettagli di progettazione: Gestione warehouse](design-details-warehouse-management.md)  
[Utilizzo di [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

