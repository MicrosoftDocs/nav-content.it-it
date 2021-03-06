---
title: Utilizzare OCR per convertire il PDF in fatture elettroniche| Documenti Microsoft
description: "Descrive come è possibile utilizzare un servizio OCR per convertire i file di immagine o i PDF in entrata in documenti elettronici in Financials."
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: electronic document, e-invoice, incoming document, OCR, ecommerce, document exchange, import invoice
ms.date: 11/09/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 1dfba8b14019991c95f40ffd5f7fbaed5df414eb
ms.openlocfilehash: f002a3975ecb6efe851cc9ac9774626f63bf760b
ms.contentlocale: it-it
ms.lasthandoff: 12/01/2017

---
# <a name="how-to-use-ocr-to-turn-pdf-and-image-files-into-electronic-documents"></a>Procedura: Utilizzare OCR per convertire PDF e file di immagine in documenti elettronici
Dai PDF o dai file di immagine che si ricevono dai partner commerciali, è possibile impostare che un servizio OCR (Optical Character Recognition, riconoscimento ottico dei caratteri) generi documenti elettronici che si possono convertire in record di documento in [!INCLUDE[d365fin](includes/d365fin_md.md)]. Ad esempio, quando si riceve una fattura nel formato PDF dal fornitore, è possibile inviarla al servizio OCR dalla finestra **Documenti in entrata**. Questa funzionalità è descritta nella prima procedura.

In alternativa all'invio del file dalla finestra **Documenti in entrata**, è possibile inviare il file al servizio OCR tramite e-mail. Successivamente, quando si riceve il documento elettronico, un record di documento entrata correlato viene creato automaticamente. Questa funzionalità è descritta nella seconda procedura.

Dopo alcuni secondi, viene ricevuto il file dal servizio OCR come fattura elettronica che può essere convertita in una fattura di acquisto per il fornitore. Questa funzionalità è descritta nella terza procedura.

Poiché OCR si basa sul riconoscimento ottico, è probabile che il servizio OCR interpreti scorrettamente i caratteri nei file PDF o di immagine quando, ad esempio, elabora per la prima volta i documenti di un determinato fornitore. Potrebbe non interpretare il logo della società come nome del fornitore o potrebbe comprendere erroneamente l'importo totale in una ricevuta a causa del layout. Per evitare che questi errori aumentino, è possibile correggerli in una versione separata della finestra **Documenti in entrata**. Quindi si inviano le correzioni al servizio di OCR per permettergli di interpretare correttamente i caratteri specifici la volta successiva che elabora un PDF o un documento di immagine dello stesso fornitore. Per ulteriori informazioni, vedere la sezione "Istruire il servizio OCR a evitare errori".

Il traffico dei file al e dal servizio OCR viene elaborato da un movimento coda processi dedicato, creato automaticamente quando si abilita la relativa connessione del servizio. Per ulteriori informazioni, vedere [Procedura: Impostare Documenti in entrata](across-how-setup-income-documents.md).

## <a name="to-send-a-pdf-or-image-file-to-the-ocr-service-from-the-incoming-documents-window"></a>Per inviare un file di immagine o PDF al servizio OCR dalla finestra **Documenti in entrata**
1. Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **Documenti in entrata**, quindi scegliere il collegamento correlato.
2. Creare un nuovo record di documento in entrata e allegare il file. Per ulteriori informazioni, vedere [Procedura: Creare i record di documenti in entrata](across-how-create-income-document-records.md).  
3. Nella finestra **Documenti in entrata** selezionare una o più righe e quindi scegliere **Invia a coda processi**.

    Il valore nel campo **Stato OCR** diventa **Pronto**. Il file di immagine o PDF allegato viene inviato al servizio OCR dalla coda processi in base alla pianificazione, a condizione che non siano presenti errori.
4. In alternativa, nella finestra **Documenti in entrata** selezionare una o più righe e quindi scegliere l'azione **Invia al servizio OCR**.

Il valore nel campo **Stato OCR** diventa **Inviato**, a condizione che non siano presenti errori.

## <a name="to-send-a-pdf-or-image-file-to-the-ocr-service-by-email"></a>Per inviare un file di immagine o PDF del servizio OCR tramite e-mail
Dall'applicazione e-mail, è possibile inviare un messaggio e-mail al provider di servizi OCR con il file di immagine o PDF allegato. Per informazioni sull'indirizzo e-mail di destinazione, vedere il sito Web del provider di servizi OCR.

Dal momento che non esiste alcun record di documento in entrata per il file, un nuovo record verrà creato automaticamente nella finestra **Documenti in entrata** quando si riceve il documento elettronico risultante dal servizio OCR. Per ulteriori informazioni, vedere [Procedura: Creare i record di documenti in entrata](across-how-create-income-document-records.md).

> [!NOTE]  
>   Se si utilizza un tablet o un telefono, è possibile inviare il file al servizio OCR non appena viene scattata la foto del documento oppure è possibile creare direttamente un documento in entrata. Per ulteriori informazioni, vedere la sezione "Creare record di documenti in entrata facendo una foto" in [Procedura: Creare i record di documenti in entrata](across-how-create-income-document-records.md).

## <a name="to-receive-the-resulting-electronic-document-from-the-ocr-service"></a>Per ricevere il documento elettronico risultante dal servizio OCR.
Il documento elettronico creato dal servizio OCR dal PDF o dal file di immagine viene ricevuto automaticamente nella finestra **Documenti in entrata** dal movimento coda processi impostato quando si abilita il servizio OCR.

Se non viene utilizzata una coda processi o si desidera ricevere un documento OCR finito prima di quanto previsto dal programma coda processi, è possibile scegliere il pulsante **Ricevi dal servizio OCR**. In tal modo verrà ricevuto qualsiasi documento completato dal servizio OCR.

> [!NOTE]  
>   Se il servizio OCR è impostato per richiedere la verifica manuale dei documenti elaborati, nel campo **Stato OCR** è presente **In attesa di verifica**. In tal caso, eseguire le seguenti operazioni per accedere al sito Web del servizio OCR per verificare manualmente un documento OCR.

1. Nel campo **Stato OCR** scegliere il collegamento ipertestuale **In attesa di verifica**. In alternativa, scegliere il riquadro **In attesa di verifica** nella home page.
2. Nel sito Web del servizio OCR, accedere utilizzando le credenziali dell'account del servizio OCR. Sono le credenziali utilizzate anche per l'impostazione del servizio. Per ulteriori informazioni, vedere la sezione "Per impostare un servizio OCR" in [Procedura: Impostare documenti in entrata](across-how-setup-income-documents.md).

    Se si accede al sito Web dal campo **Stato OCR** il documento in questione viene visualizzato subito dopo l'accesso. Se si accede al sito Web selezionando il riquadro nella home page, scegliere nella prima pagina del servizio OCR che viene visualizzata il pulsante **Avvia** nella scheda **Verifica** o fare doppio clic sul documento da verificare.

    Vengono visualizzate le informazioni per il documento OCR, inclusi il contenuto di origine del PDF o del file di immagine e i valori dei campi OCR risultanti.
3. Analizzare i diversi valori dei campi e modificare o immettere manualmente i valori nei campi che il servizio OCR ha etichettato come incerti.
4. Scegliere il pulsante **OK**. Il processo OCR è completato e il documento elettronico risultante viene inviato alla finestra **Documenti in entrata** in [!INCLUDE[d365fin](includes/d365fin_md.md)], in base al programma coda processi.

    Se si accede al sito Web selezionando il riquadro nella home page, qualsiasi altro documento OCR da verificare viene visualizzato automaticamente nel sito Web.
5. Ripetere il passaggio 4 per qualsiasi altro documento OCR da verificare.

A questo punto è possibile passare alla creazione dei record per i documenti elettronici ricevuti in [!INCLUDE[d365fin](includes/d365fin_md.md)], manualmente o automaticamente. Per ulteriori informazioni, vedere la procedura che segue. È inoltre possibile connettere il nuovo record del documento in entrata al documento esistente registrato o non registrato in modo che il file di origine sia facilmente accessibile da [!INCLUDE[d365fin](includes/d365fin_md.md)]. Per ulteriori informazioni, vedere [Elaborare i documenti in entrata](across-process-income-documents.md).

## <a name="to-create-a-purchase-invoice-from-an-electronic-document-received-from-the-ocr-service"></a>Per creare una fattura di acquisto da un documento elettronico ricevuto dal servizio OCR
Di seguito viene descritto come creare un record di fattura di acquisto da una fattura fornitore ricevuta come documento elettronico dal servizio OCR. La procedura è identica a quella per creare, ad esempio, una riga di registrazione COGE da una ricevuta di spesa o un ordine di reso vendita da un cliente.

> [!NOTE]  
>   I campi **Descrizione** e **Nr.** nelle righe di documento create verranno compilati solo se è stato precedentemente mappato il testo individuato nel documento OCR ai due campi in [!INCLUDE[d365fin](includes/d365fin_md.md)]. Puoi effettuare questa operazione di mappatura come cross-references articoli, per le righe del documento di tipo Articolo. È anche possibile utilizzare la funzione di mappatura testo a conto. Per ulteriori informazioni, vedi la sezione "Per mappare il testo di un documento in entrata a un determinato fornitore, C/G o conto corrente bancario".

Per mappare i numeri di articolo del documento alle descrizioni degli articoli del fornitore, aprire la scheda di ciascun articolo e scegliere l'azione **Cross reference** per impostare i riferimenti incrociati tra le descrizioni degli articoli dell'utente e quelle del fornitore. Per ulteriori informazioni, vedi le descrizioni comandi per l'azione **Cross reference** nelle schede articolo.

1. Selezionare la riga relativa al documento in entrata quindi scegliere l'azione **Crea documento**.

Una fattura di acquisto verrà creata in [!INCLUDE[d365fin](includes/d365fin_md.md)] sulla base delle informazioni contenute nel documento elettronico del fornitore che è stato ricevuto dal servizio OCR. Le informazioni verranno inserite nella nuova fattura di acquisto in base alla mappatura definita come cross-reference o come testo di mappatura testo a conto.

Tutti gli errori di convalida, in genere correlati a dati mancanti o errati in [!INCLUDE[d365fin](includes/d365fin_md.md)], verranno visualizzati nella Scheda dettaglio **Errori e avvisi**. Per ulteriori informazioni, vedere la sezione "Per gestire gli errori durante la ricezione di documenti elettronici".

### <a name="to-map-text-on-an-incoming-document-to-a-specific-vendor-account"></a>Per mappare il testo di un documento in entrata a un determinato conto del fornitore
Per i documenti in entrata, in genere l'azione **Mappa testo a conto** si utilizza per definire che un determinato testo in una fattura fornitore ricevuta dal servizio OCR viene mappato a un determinato conto fornitore. Andando in avanti, qualsiasi parte della descrizione del documento in entrata esistente come testo di mappatura indica che il campo **Nr.** nelle righe di registrazione o del documento risultanti di tipo Conto G/C viene compilato con il fornitore in questione.

Oltre alla mappatura a un conto fornitore o ad altri conti C/G, è possibile mappare anche a un conto bancario. Ciò risulta utile, ad esempio, per i documenti elettronici relativi alle spese che sono già state pagate in cui si desidera creare una riga registrazione COGE pronta per essere registrata in un conto corrente bancario.

1. Seleziona la riga del documento in entrata pertinente quindi scegli l'azione **Mappa testo a conto**. Verrà aperta la finestra **Mappatura testo a conto**.
3. Nel campo **Mapping testo**, immetti qualsiasi testo presente nelle fatture del fornitore per cui desideri creare documenti di acquisto o righe delle registrazioni. È possibile immettere fino a 50 caratteri.
4. Nel campo **Nr. fornitore** immetti il fornitore per cui verrà creata la riga del documento o di registrazione acquisto.
5. Nel campo **Nr. conto dare**, immetti il conto C/G di tipo dare che verrà inserito nel documento di acquisto o nella riga di registrazione creata di tipo Conto C/G.
6. Nel campo **Nr. conto avere**, immetti il conto C/G di tipo avere che verrà inserito nel documento di acquisto o nella riga di registrazione creata di tipo Conto C/G.

    > [!NOTE]
    > Non usare i campi **Tipo di origine saldo** e **Nr. origine saldo** in relazione ai documenti in entrata. Vengono utilizzati solo per la riconciliazione automatica di pagamento. Per ulteriori informazioni, vedere [Procedura: Mappare il testo nei pagamenti ricorrenti a conti per la riconciliazione automatica](receivables-how-map-text-recurring-payments-accounts-auto-reconcilliation.md).

7. Ripeti i passaggi da 2 a 5 per qualsiasi testo su documenti in entrata per cui vuoi creare automaticamente i documenti.

## <a name="to-handle-errors-when-receiving-electronic-documents"></a>Per gestire gli errori durante la ricezione di documenti elettronici
1. Nella finestra **Documenti in entrata**, selezionare la riga per un documento elettronico ricevuto dal servizio OCR con errori. Ciò è indicato dal valore Errore nel campo **Stato OCR**.
2. Scegliere l'azione **Modifica** per aprire la finestra **Documento in entrata**.
3. Nella Scheda dettaglio **Errori e avvisi**, selezionare il messaggio quindi scegliere l'azione **Apri record correlato**.
4. Viene visualizzata la finestra contenente i dati errati o mancanti, ad esempio una scheda fornitore con un valore di campo mancante.
5. Correggere l'errore o gli errori come descritto in ogni messaggio di errore.
6. Continuare a elaborare il documento elettronico in entrata scegliendo di nuovo l'azione **Crea manualmente**.
7. Ripetere i passaggi 5 e 6 per tutti gli errori rimanenti finché il documento elettronico non può essere ricevuto correttamente.

## <a name="to-train-the-ocr-service-to-avoid-errors"></a>Per istruire il servizio OCR a evitare errori
Poiché OCR si basa sul riconoscimento ottico, è probabile che il servizio OCR interpreti scorrettamente i caratteri nei file PDF o di immagine quando, ad esempio, elabora per la prima volta i documenti da un determinato fornitore. Potrebbe non interpretare il logo della società come nome del fornitore o potrebbe comprendere erroneamente l'importo totale in una ricezione di spese a causa del layout. Per evitare che tali errori vanno avanti, è possibile correggere i dati ricevuti dal servizio OCR e quindi inviare il feedback all'assistenza.

La finestra **Correzione dati OCR** che si apre dalla finestra **Documento in entrata** mostra i campi della Scheda dettaglio **Informazioni finanziarie** in due colonne, una con i dati OCR modificabili e una con i dati OCR di sola lettura. Scegliendo il pulsante **Invia commenti e suggerimenti OCR** il contenuto della finestra **Correzione dati OCR** viene inviato al servizio OCR. La volta successiva che il servizio elabora file PDF o di immagine contenenti i dati in questione, le correzioni verranno incluse per evitare gli stessi errori.

1. Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **Documenti in entrata**, quindi scegliere il collegamento correlato.
2. Aprire un record del documento in entrata contenente i dati ricevuti dal servizio OCR da correggere.
3. In alternativa, nella finestra **Documento in entrata** scegliere l'azione **Correggi dati OCR**.
4. Nella finestra **Correggi dati OCR** sovrascrivere i dati nella colonna modificabile per ogni campo contenente un valore non corretto.
5. Per annullare le correzioni apportate dall'apertura della finestra **Correzione dati OCR**, scegliere l'azione **Reimposta dati OCR**.
6. Per inviare le correzioni al servizio OCR, scegliere l'azione **Invia commenti e suggerimenti OCR**.
7. Per salvare le correzioni, chiudere la finestra **Correzione dati OCR**.

I campi della Scheda dettaglio **Informazioni finanziarie** nella finestra **Documento in entrata** vengono aggiornati con i nuovi valori immessi nel passaggio 4.

## <a name="see-also"></a>Vedi anche
[Elaborare i documenti in entrata](across-process-income-documents.md)  
[Documenti in entrata](across-income-documents.md)  
[Acquisti](purchasing-manage-purchasing.md)  
[Utilizzo di [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

