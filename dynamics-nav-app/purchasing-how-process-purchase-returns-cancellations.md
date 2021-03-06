---
title: Utilizzare note di credito di acquisto per elaborare resi o annullamenti
description: Descrizione di come creare e registrare una nota di credito acquisto quando si desidera effettuare un reso degli articoli a un fornitore o annullare servizi acquistati.
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: cancel, undo, correct
ms.date: 08/03/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 3f0c187e2cd2520854fe69f3896f6d7311cdc2da
ms.contentlocale: it-it
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-process-purchase-returns-or-cancellations"></a>Procedura: Elaborare i resi o gli annullamenti acquisti
Se si desidera restituire gli articoli al fornitore o annullare l'assistenza acquistata, è possibile creare e registrare una nota di credito di acquisto in cui viene specificata la modifica richiesta rispetto alla fattura di acquisto originale. Per includere le informazioni corrette in merito alle fatture di acquisto, è possibile creare la nota di credito di acquisto direttamente dalla fattura di acquisto registrata oppure creare una nuova nota di credito di acquisto con le informazioni copiate dalla fattura.

Se è necessario più controllo del processo di reso da acquisto, ad esempio i documenti di warehouse per la gestione degli articoli o una sintesi migliorata per il recapito degli articoli restituiti da più documenti di acquisto con un unico reso, è possibile creare gli ordini di reso da acquisto. Un ordine di reso da acquisto automaticamente crea la nota di credito di acquisto correlata. Per ulteriori informazioni, vedere la sezione "Per creare un ordine di reso da acquisto sulla base di uno o più documenti di acquisto registrati".

> [!NOTE]  
>   Se una fattura di acquisto registrata non è stata ancora pagata, allora è possibile utilizzare le funzioni **Annulla** o **Rettifica** nella fattura di acquisto registrata per stornare automaticamente le transazioni implicate. Queste funzionano solo per le fatture non pagate e non supportano i resi o le cancellazioni parziali. Per ulteriori informazioni, vedere [Procedura: Correggere o annullare le fatture di acquisto non pagate](purchasing-how-correct-cancel-unpaid-purchase-invoices.md).

In genere, si crea una nota di credito di acquisto o un ordine di reso da acquisto in risposta a una nota di credito inviata da un fornitore. La nota di credito di acquisto o l'ordine di reso da acquisto funziona come documentazione interna del processo di nota di credito per scopi contabili o per controllare la spedizione degli articoli interessati.

La modifica può essere correlata a tutti o solo ad alcuni prodotti nella fattura di acquisto originale. Di conseguenza, è possibile restituire parzialmente gli articoli ricevuti o richiedere il risarcimento parziale dei servizi ricevuti. In questo caso, è necessario modificare le informazioni nella nota di credito di acquisto o nell'ordine di reso da acquisto.

Oltre alla fattura di acquisto registrata originale, è possibile collegare la nota di credito di acquisto o l'ordine di reso da acquisto ad altri documenti di acquisto, ad esempio un'altra fattura di acquisto registrata, in quanto si restituiscono anche gli articoli consegnati con la fattura.

La registrazione della nota di credito annullerà anche tutti gli addebiti articolo assegnati al documento registrato, in modo che i movimenti valorizzazione articolo siano identici a prima dell'assegnazione dell'addebito articolo.

## <a name="inventory-costing"></a>Costing di magazzino
Per mantenere la corretta valutazione del magazzino, in genere si desidera selezionare gli articoli di reso dal magazzino al costo unitario con cui sono stati acquistati e non al costo unitario corrente. Questa operazione è detta storno esatto costo.

Sono disponibili due funzioni per assegnare lo storno esatto costo automaticamente.  

|Funzione|Description|  
|------------------|---------------------------------------|  
|La funzione**Ottieni righe documento registrato da stornare** nella finestra **Ordine di reso acquisto**|Copia le righe di uno o più documenti registrati da stornare nell'ordine di reso da acquisto. Per ulteriori informazioni, vedere la sezione "Per creare un ordine di reso da acquisto e la relativa nota di credito di acquisto per una o più fatture di acquisto registrate".|  
|La funzione**Copia documento** nelle finestre **Nota credito acquisto** e **Ordine di reso acquisto**|Copia la testata e le righe di un documento registrato da stornare.<br /><br /> È necessario che la casella di controllo **Storno esatto costo obblig.** sia selezionata nella finestra **Setup contabilità fornitori e acquisti**.|

Per assegnare manualmente lo storno esatto costo, è necessario utilizzare il campo **Collega-da mov. art.** per ogni tipo di riga di documento di reso e selezionare il numero del movimento di acquisto originale. In questo modo, la nota di credito di acquisto o l'ordine di reso da acquisto viene collegato al movimento di acquisto originale e l'articolo verrà valutato al costo unitario originale.

Per ulteriori informazioni, vedere [Dettagli di progettazione: Costing di magazzino](design-details-inventory-costing.md).

## <a name="to-create-a-purchase-credit-memo-from-a-posted-purchase-invoice"></a>Per creare una nota di credito di acquisto da una fattura di acquisto registrata
1. Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **Fatture di acquisto registrate**, quindi scegliere il collegamento correlato.  
2. Nella finestra **Fatture acquisto registrate** selezionare la fattura di acquisto registrata che si desidera stornare, quindi scegliere l'azione **Crea nota credito di rettifica**.

    La maggior parte dei campi nella testata della nota di credito di acquisto viene compilata con le informazioni della fattura di acquisto registrata. È possibile modificare tutti i campi, ad esempio con nuove informazioni che riflettono il contratto di reso.
3. Modificare le informazioni nelle righe in base al contratto, quali il numero di articoli resi o l'importo da rimborsare.
4. Scegliere l'azione **Collega movimenti**.
5. Nella finestra **Collega movimenti fornitori**, selezionare la riga con il documento di acquisto registrato a cui si desidera collegare la nota di credito di acquisto, quindi scegliere l'azione **Collega-a ID**. Il numero della nota di credito di acquisto viene inserito nel campo **Collega-a ID**.
6. Nel campo **Importo da collegare** immettere l'importo che si desidera collegare se inferiore all'importo originale.

    Nella parte inferiore della finestra **Collega movimenti fornitori** è possibile vedere l'importo totale da collegare per stornare tutti i movimenti coinvolti, ad esempio quando il valore del campo **Saldo** è zero.
7. Scegliere il pulsante **OK**. Quando si registra la nota di credito di acquisto, verrà collegata ai documenti di acquisto registrati specificati.

    Dopo avere creato o modificato le righe della nota di credito di acquisto necessarie e aver specificato uno o più collegamenti, è possibile passare alla registrazione della nota di credito di acquisto.
8. Scegliere l'azione **Registra**.

Le fatture di acquisto registrate a cui si applica la nota di credito vengono ora stornate. Se è già stata pagata la fattura originale, il fornitore dovrà rimborsare il pagamento. Se la nota di credito riguarda solo parte del prodotto nella fattura originale, è possibile pagare solo l'importo restante nella fattura di acquisto originale per chiuderla.

La nota di credito di acquisto viene rimossa e sostituita con un nuovo documento nell'elenco delle note di credito di acquisto registrate.

## <a name="to-create-a-purchase-credit-memo-by-copying-a-posted-purchase-invoice"></a>Per creare una nota di credito di acquisto copiando una fattura di acquisto registrata
1. Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **Note credito acquisto**, quindi scegliere il collegamento correlato.
2. Scegliere l'azione **Nuovo** per aprire una nuova nota di credito di acquisto vuota.
3. Nel campo **Fornitore** immettere il nome del fornitore esistente.
4. Scegliere l'azione **Copia documento**.
5. Nella finestra **Copia documento acquisto**, nel campo **Tipo di documento**, selezionare **Fattura registrata**.
6. Selezionare il campo **Nr. documento** per aprire la finestra **Fatture acquisto registrate** e selezionare la fattura di acquisto registrata contenente le righe da stornare.
7. Selezionare la casella di controllo **Ricalcola righe** se si desidera che le righe copiate della fattura di acquisto registrata vengano aggiornate con le modifiche al prezzo dell'articolo e al costo unitario poiché la fattura è stata registrata.
8. Scegliere il pulsante **OK**. Le righe della fattura copiate vengono inserite nella nota di credito di acquisto.
9. Completare la nota di credito acquisto come descritto nella sezione "Per creare una nota di credito di acquisto da una fattura di acquisto registrata" del presente argomento.

## <a name="to-create-a-purchase-return-order-based-on-one-or-more-a-posted-purchase-documents"></a>Per creare un ordine di reso da acquisto sulla base di uno o più documenti di acquisto registrati
1. Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **Ordini di reso acquisto**, quindi scegliere il collegamento correlato.  
2. Scegliere l'azione **Nuovo**.  
3. Compilare i campi appropriati nella Scheda dettaglio **Generale**.
4. Nella Scheda dettaglio **Righe**, compilare le righe manualmente oppure copiare le informazioni da altri documenti per compilare le righe automaticamente:

    - Utilizzare la funzione **Ottieni righe documento registrato da stornare** per copiare una o più righe da uno o più documenti registrati. Questa funzione consente di stornare sempre esattamente i costi dalle righe del documento registrato. Questa funzionalità è descritta nei passaggi seguenti.    
    - Utilizzare la funzione **Copia documento** per copiare un documento esistente nell'ordine di reso. Utilizzare questa funzione per copiare l'intero documento. Può essere un documento registrato o un documento non ancora registrato. Questa funzione consente lo storno esatto costo solo quando la casella di controllo **Storno esatto costo obblig.** è selezionata nella finestra **Setup contabilità clienti**.  

4. Scegliere l'azione **Ottieni righe documento registrato da stornare**.
5. Nella parte superiore della finestra **Righe documento acquisto reg.** selezionare la casella di controllo **Mostra solo righe reversibili** se si desidera visualizzare solo le righe associate a quantità non ancora rese. Se, ad esempio, è già stata resa una quantità della fattura di acquisto registrata, potrebbe essere preferibile non includere tale quantità in un nuovo documento di reso da a acquisto.

    > [!NOTE]  
    >  Questo campo è valido solo per righe di carichi registrati e di fatture registrate, ma non per righe di resi registrati o di note di credito registrate.  

    Nella parte sinistra della finestra sono elencati i diversi tipi di documento, mentre il numero tra parentesi indica il numero di documenti disponibili per ogni tipo di documento.

6. Nel campo **Filtro tipo documento** selezionare il tipo di righe documento registrate che si intende utilizzare.  
7. Selezionare le righe che si desidera copiare nel nuovo documento.  

    > [!NOTE]  
    >  Se si utilizza CTRL+A per selezionare tutte le righe, vengono copiate tutte le righe incluse nel filtro impostato, ma viene ignorato il filtro **Mostra solo righe reversibili**. Si supponga, ad esempio, di avere filtrato le righe in base a un particolare numero di documento con due righe, una delle quali è già stata completamente resa. Anche se si seleziona il campo **Mostra solo righe reversibili**, se si preme CTRL+A per copiare tutte le righe, vengono copiate entrambe le righe anziché solo quella non ancora stornata.  

8. Scegliere **OK** per copiare le righe nel nuovo documento.  

    Si verificheranno i processi seguenti:  

    -   Per le righe del documento registrato di tipo **Articolo**, viene creata una nuova riga che rappresenta una copia della riga del documento registrato, con la quantità che non è ancora stata stornata. Il campo **Collega-a mov. art.** viene automaticamente compilato con il numero del movimento contabile articolo presente nella riga del documento registrata.  

    -   Per le righe del documento registrato non di tipo **Articolo**, ad esempio addebiti articoli, viene creata una nuova riga che rappresenta una copia della riga del documento registrato originale.  

    -   Viene calcolato il valore del campo **Costo unitario (VL)** nella nuova riga in base ai costi nei movimenti contabili articoli corrispondenti.  

    -   Se il documento copiato è una spedizione registrata, un carico registrato, un carico da reso registrato o una spedizione di reso registrata, il prezzo unitario viene calcolato automaticamente in base alla scheda articolo.  

    -   Se il documento copiato è una nota di credito o una fattura registrata, il prezzo unitario, gli sconti fattura e gli sconti riga vengono copiati dalla riga del documento registrato.  

    -   Se la riga del documento registrata include righe di tracciabilità articolo, il campo **Collega-a mov. art.** nelle righe di tracciabilità articolo viene compilato con i numeri dei movimenti contabili articoli appropriati indicati nelle righe di tracciabilità articolo registrate.  

     Quando si copia da una fattura o una nota di credito registrata, gli sconti fattura e gli sconti riga pertinenti vengono copiati come validi al momento della registrazione del documento dalla riga del documento registrato nella riga del nuovo documento. Si noti, tuttavia, che se l'opzione **Calcola sconto fatt.** è attivata nella finestra **Setup contabilità fornitori e acquisti** , lo sconto fattura verrà calcolato quando si registra la riga del nuovo documento. È possibile, pertanto, che l'importo riga per la nuova riga sia diverso da quello della riga del documento registrato, a seconda del nuovo calcolo dello sconto fattura.  

    > [!NOTE]  
    >  Se parte della quantità della riga del documento registrato è già stata stornata, venduta o consumata, viene creata una riga solo per la quantità rimanente in magazzino o non ancora resa. Se l'intera quantità della riga del documento registrato è già stata stornata, non viene creata una nuova riga.  
    >   
    >  Se il flusso delle merci nel documento registrato corrisponde a quello nel nuovo documento, viene creata una copia della riga del documento registrato originale nel nuovo documento. Il campo **Collega-da mov. art.** non viene compilato perché in questo caso, lo storno esatto costo non è possibile. Se, ad esempio, si utilizza la funzione **Ottieni righe documento registrato da stornare** per ottenere una riga di nota di credito acquisto registrata per una nuova nota di credito acquisto, nella nuova nota di credito viene copiata esclusivamente la riga di nota di credito registrata originale.  

8. Nella finestra **Ordine di reso acquisto**, nel campo **Cod. causa di reso** di ciascuna riga, selezionare il motivo del reso.
9. Scegliere l'azione **Registra**.

## <a name="to-create-a-replacement-purchase-order-from-a-purchase-return-order"></a>Per creare un ordine di acquisto di sostituzione da un ordine di reso da acquisto
È possibile raggiungere un accordo con un fornitore per la sostituzione di un articolo quale compensazione per un articolo acquistato. L'articolo sostitutivo può essere uguale oppure diverso. Questa situazione potrebbe presentarsi, ad esempio, se il fornitore ha spedito l'articolo sbagliato.  
1.  Nella finestra **Ordine di reso acquisto** per un processo di reso attivo, su una riga vuota, creare un movimento negativo per l'articolo in sostituzione immettendo un importo negativo nel campo **Quantità**.  
2. Scegliere l'azione **Sposta righe negative**.  
3. Nella finestra **Muovi righe acquisto negative** compilare i campi secondo le necessità.
4. Scegliere il pulsante **OK**. La riga negativa viene eliminata dall'ordine di reso acquisto e un nuovo ordine di acquisto viene creato. Per ulteriori informazioni, vedere [Procedura: Registrare gli acquisti](purchasing-how-record-purchases.md).  

## <a name="to-create-a-purchase-allowance"></a>Per creare un abbuono di acquisto  
Se si ricevono degli articoli dal fornitore che non corrispondono a quelli richiesti, ad esempio, se sono leggermente danneggiati, se il colore o la misura non sono quelli giusti, il fornitore può proporre un abbuono sull'acquisto.  

È possibile registrare tale costo di acquisto ridotto come addebito articolo in una nota di credito o in un ordine di reso e collegarlo al carico registrato. Di seguito sono descritte le procedure per un ordine di reso da acquisto, ma gli stessi passaggi si applicano a una nota di credito di acquisto.

1. Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **Note credito acquisto**, quindi scegliere il collegamento correlato.
2. Scegliere l'azione **Nuovo** per aprire una nuova nota di credito di acquisto vuota.  
3.  Compilare la testata della nota di credito con le informazioni relative al fornitore che ha inviato l'abbuono.  
4. Nel campo **Tipo** della Scheda dettaglio **Righe** selezionare **Addebito (Articolo)**.  
5.  Nel campo **Nr.** selezionare il valore di addebito articolo appropriato.  

    È possibile creare un numero di addebito articolo particolare per coprire gli abbuoni sugli acquisti.  
6.  Nel campo **Quantità** immettere **1**.  
7.  Nel campo **Costo Diretto Unitario** immettere l'importo dell'abbuono.  
8.  Assegnare l'abbuono come addebito sugli articoli nel carico registrato. Per ulteriori informazioni, vedere [Procedura: Utilizzare gli addebiti articolo al conto per i costi aggiuntivi commerciali](payables-how-assign-item-charges.md). Dopo avere assegnato l'abbuono, tornare alla finestra **Nota credito acquisto**.

Durante la registrazione dell'ordine di reso da acquisto, l'abbuono viene aggiunto all'importo del movimento di acquisto corrispondente. In questo modo è possibile mantenere una valutazione precisa del magazzino.  

## <a name="to-combine-return-shipments"></a>Per cumulare le spedizioni di reso  
Per rendere articoli coperti da diversi ordini di reso acquisto allo stesso fornitore, è possibile utilizzare la funzione **Spedizioni reso cumulative**.  

Al momento della spedizione degli articoli, i relativi ordini di reso acquisto vengono registrati come spediti e vengono quindi create spedizioni di reso acquisto registrate.  

Al momento della fatturazione di questi articoli, anziché fatturare ciascun ordine di reso separatamente, è possibile creare una nota di credito acquisto e copiare automaticamente in questo documento le righe di spedizione di reso acquisto registrate. Sarà quindi possibile registrare la nota di credito acquisto e fatturare tutti gli ordini di reso acquisto aperti contemporaneamente.  

Quando le spedizioni di reso vengono cumulate in una nota di credito e registrate, per le righe fatturate viene creata una nota di credito acquisto registrata. Il campo **Quantità fatturata** dell'ordine di reso acquisto di origine viene aggiornato in base alla quantità fatturata. Tuttavia, l'ordine di reso di acquisto originale non viene eliminato, anche se è stato completamente ricevuto e fatturato; è necessario quindi eliminare l'ordine di reso acquisto manualmente.

> [!NOTE]  
> Si supponga, ad esempio, che esistano più ordini di reso acquisto per il fornitore e che siano stati registrati come spediti.     

1.  Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **Note credito acquisto**, quindi scegliere il collegamento correlato.  
2.  Scegliere l'azione **Nuovo**.  
3. Compilare i campi appropriati nella Scheda dettaglio **Generale**.  
4. Scegliere l'azione **Prendi righe di spedizione reso**.  
5.  Selezionare più righe di spedizione di reso da includere nella fattura.  

    Se è stata selezionata una riga di spedizione di reso non corretta o si desidera effettuare una nuova selezione, è possibile eliminare le righe dalla nota di credito di acquisto ed eseguire nuovamente la funzione **Prendi righe di spedizione reso**.  
6.  Scegliere l'azione **Registra**.  

### <a name="to-remove-open-purchase-return-orders-after-combined-return-shipment-posting"></a>Per rimuovere ordini di reso acquisto aperti dopo la registrazione della spedizione reso cumulativa  

1.  Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **Elimina ordini di reso acq. fatturati**, quindi scegliere il collegamento correlato.  
2.  Compilare i campi in base alle esigenze, quindi scegliere **OK**.  
3.  In alternativa, eliminare i singoli ordini di reso acquisto manualmente.

## <a name="see-also"></a>Vedi anche
[Acquisti](purchasing-manage-purchasing.md)  
[Procedura: Registrare gli acquisti](purchasing-how-record-purchases.md)  
[Procedura: Correggere o annullare le fatture di acquisto non pagate](purchasing-how-correct-cancel-unpaid-purchase-invoices.md)  
[Utilizzo di [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

