---
title: Assegnare addebiti articoli a vendite e acquisti
description: "Se si desidera aggiungere ai movimenti di magazzino ulteriori costi, quali spedizione, gestione fisica, assicurazione e trasporto sostenuti per l'acquisto o la vendita degli articoli, è possibile utilizzare la funzionalità Addebiti articoli."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: transportation, added cost
ms.date: 06/06/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: f5eebe7d1837657771d4f3004627be716d4d51bc
ms.contentlocale: it-it
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-use-item-charges-to-account-for-additional-trade-costs"></a>Procedura: Utilizzare gli addebiti articolo al conto per i costi aggiuntivi commerciali
Per una valutazione corretta, è necessario includere nei movimenti di magazzino tutti i costi aggiuntivi, quali spedizione, gestione fisica, assicurazione e trasporto sostenuti per l'acquisto o la vendita degli articoli. Per gli acquisti, il costo franco di tutte le spese allo sbarco di un articolo acquistato è dato dal prezzo di acquisto del fornitore più tutti gli addebiti articolo diretti aggiuntivi che è possibile assegnare ai singoli carichi o alle singole spedizioni di reso. Per le vendite, per un'azienda conoscere il costo della spedizione di articoli venduti è altrettanto importante che conoscere il costo franco di tutte le spese di sbarco degli articoli acquistati.

Oltre a registrare il costo aggiuntivo nel valore di magazzino, è possibile utilizzare la funzionalità Addebiti per le seguenti operazioni:

- Determinare il costo franco di tutte le spese allo sbarco di un articolo allo scopo di stabilire strategie più accurate di ottimizzazione della rete di distribuzione.
- Scomporre il costo unitario o il prezzo unitario di un articolo a scopo di analisi.
- Includere gli abbuoni sugli acquisti nel costo unitario e gli abbuoni sulle vendite nel prezzo unitario.

Prima di poter assegnare gli addebiti articoli, è necessario impostare i numeri di addebito articoli per i diversi tipi di addebito, inclusi in quali conti C/G andranno registrati i costi relativi a vendite, acquisti e rettifiche di magazzino. Un numero di addebito articolo contiene una combinazione di gruppi di registrazioni di prodotti generali, codici di gruppi imposta, gruppo di registrazione di prodotti IVA e addebiti articoli. Inserendo il numero di addebito articoli in un documento d'acquisto o di vendita, il conto C/G pertinente viene recuperato in base al setup del numero di addebito articolo e alle informazioni nel documento.

Sia per i documenti di vendita che di acquisto, è possibile assegnare un addebito articolo in due modi:
- Nel documento in cui sono elencati gli articoli ai quali l'addebito si riferisce. In genere questo metodo si utilizza per i documenti che non sono stati ancora completamente registrati.
- In una fattura separata collegando l'addebito articolo a un carico o una spedizione registrata dove vengono elencati gli articoli a cui l'addebito si riferisce.

> [!NOTE]  
>   È possibile assegnare addebiti articoli a ordini, fatture e note di credito, per i documenti di vendita e per quelli di acquisto. Di seguito viene descritto come utilizzare gli addebiti articolo per una fattura di acquisto. I passaggi sono simili per tutti gli altri documenti di acquisto o vendita.

## <a name="to-set-up-item-charge-numbers"></a>Per impostare i numeri di addebito articolo
I numeri di addebito articolo vengono utilizzati per distinguere fra i vari tipi di addebito utilizzati nella propria società.

1. Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **Addebiti articoli**, quindi scegliere il collegamento correlato.
2. Scegliere l'azione **Nuovo** nella finestra **Addebiti articoli** per creare una nuova riga.
3. Compilare i campi, se necessario. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

## <a name="to-assign-an-item-charge-directly-to-the-purchase-invoice-for-the-item"></a>Per assegnare un addebito articolo direttamente alla fattura di acquisto per l'articolo
Se si conosce l'addebito articolo nel momento in cui si registra una fattura di acquisto per l'articolo, attenersi alla procedura seguente.

1. Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **Fatture di acquisto**, quindi scegliere il collegamento correlato.
2. Creare una nuova fattura di acquisto. Per ulteriori informazioni, vedere [Procedura: Registrare gli acquisti](purchasing-how-record-purchases.md).
3. Assicurarsi che la fattura di acquisto abbia una o più righe di tipo Articolo.
4. In una nuova riga selezionare **Addebito (Articolo)** nel campo **Tipo**.
5. Nel campo **Quantità** immettere il numero di unità dell'addebito articolo che sono state fatturate.
6. Nel campo **Costo Diretto Unitario** immettere l'importo dell'addebito articolo.
7. Compilare i rimanenti campi, se necessario. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

    Nei seguenti passaggi, verrà effettuata l'assegnazione effettiva. Finché l'addebito articolo non è assegnato completamente, il valore nel campo **Qtà da assegnare** verrà visualizzato con carattere rosso.
8. Nella Scheda dettaglio **Righe** fare clic sull'azione **Assegnazione addebito articolo**.

    Verrà visualizzata la finestra **Assegnazione addebito articolo** che mostra una riga per ogni riga di tipo Articolo nella fattura di acquisto. Per assegnare l'addebito articolo a una o più righe della fattura, è possibile utilizzare una funzione che assegna e distribuisce l'addebito automaticamente oppure è possibile compilare manualmente il campo **Qtà da assegnare**. Nei seguenti passaggi viene descritto come utilizzare la funzione Suggerisci assegnazione addebiti articoli.

9. Nella finestra **Assegnazione addebito articolo**, selezionare l'azione **Suggerisci assegnazione addebiti articoli**.
10. Se vi sono più di una riga fattura di tipo Articolo, selezionare una delle quattro opzioni di distribuzione.  

Finché l'addebito articolo è assegnato completamente, il valore nel campo **Qtà da assegnare** nella fattura di acquisto verrà visualizzato come zero.

L'addebito è ora assegnato alla fattura di acquisto. Quando si registra il carico della fattura di acquisto, i valori di magazzino degli articoli vengono aggiornati con il costo dell'addebito articolo.  

## <a name="to-assign-an-item-charge-from-a-separate-invoice-to-the-purchase-invoice-for-the-item"></a>Per assegnare un addebito articolo da una fattura distinta alla fattura di acquisto per l'articolo
Se si riceve una fattura per l'addebito articolo dopo aver effettuato la registrazione del carico dell'acquisto originale, attenersi alla procedura seguente.
1. Ripetere i passaggi da 1 a 8 della sezione Per assegnare un addebito articolo direttamente alla fattura di acquisto per l'articolo.
2. Nella finestra **Assegnaz. addebito art.** scegliere l'azione **Prendi righe di carico**.
3. Nella finestra **Righe carico acq.** selezionare il carico di acquisto registrato per l'articolo a cui si desidera assegnare l'addebito quindi scegliere **OK**.
4. Scegliere l'azione **Suggerisci ass. addebiti art.**.

Gli addebiti articoli nella fattura di acquisto distinta vengono ora assegnati all'articolo nel carico di acquisto registrato, viene quindi aggiornato il valore di magazzino dell'articolo con il costo dell'addebito articolo.

## <a name="see-also"></a>Vedi anche
[Gestione della contabilità fornitori](payables-manage-payables.md)  
[Procedura: Registrare gli acquisti](purchasing-how-record-purchases.md)  
[Procedura: Fatturare le vendite](sales-how-invoice-sales.md)  
[Utilizzo di [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)  

