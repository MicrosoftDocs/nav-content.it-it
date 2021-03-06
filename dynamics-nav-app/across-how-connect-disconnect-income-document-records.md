---
title: Creare i documenti in entrata da documenti
description: "È possibile creare i record dei documenti in entrata, ad esempio le fatture elettroniche, e gestire le attività OCR, il commercio elettronico e il servizio di scambio documenti."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: electronic document, e-invoice, incoming document, OCR, ecommerce, document exchange, import invoice
ms.date: 06/02/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: fd8eba03f98d4d667a25639c1c958edf6936b0cb
ms.contentlocale: it-it
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-create-incoming-document-records-directly-from-documents-and-entries"></a>Procedura: Creare i record di documenti in entrata direttamente da documenti e movimenti
È possibile archiviare i documenti aziendali esterni in [!INCLUDE[d365fin](includes/d365fin_md.md)] allegando i file del documento ai record di documento in entrata correlati. Se il documento, ad esempio una fattura di acquisto, non è stato creato come record di documento in arrivo, è comunque possibile creare e connettere ad esso un record di documento in arrivo in un secondo momento. È inoltre possibile allegare file di documento in entrata a documenti di vendita e di acquisto registrati e a movimenti di contabilità cliente o fornitore utilizzando il Dettaglio informazioni di **File di documento in entrata** ad esempio nelle finestre **Fatture acquisto registrate** e **Movimenti contabili fornitori**.

Nelle finestre **Piano dei conti** e **Movimenti C/G** è possibile utilizzare una funzione di ricerca per trovare movimenti di contabilità generale per documenti di vendita e di acquisto registrati che non hanno record di documenti in entrata e successivamente collegarli centralmente a record esistenti o crearne di nuovi con file di documento allegati. Per ulteriori informazioni, vedere [Procedura: Trovare documenti registrati senza record di documenti in entrata](across-how-find-posted-documents-without-income-document-records.md).

Le procedure riportate di seguito mostrano come allegare un file a una fattura di acquisto esistente che non è stata creata da un record di documento in entrata e come allegare un file a un movimento contabile fornitore. L'operazione di allegare un file a documenti di vendita o di acquisto registrati funziona in modo analogo.

## <a name="to-create-and-connect-an-incoming-document-record-from-a-purchase-invoice"></a>Per creare e connettere un record di documento in entrata da una fattura di acquisto
1. Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **Fatture di acquisto**, quindi scegliere il collegamento correlato.
2. Selezionare la riga relativa a una fattura di acquisto a cui si desidera allegare un file e quindi scegliere l'azione **Crea documento in entrata da file**.
3. In alternativa, selezionare la riga relativa a una fattura di acquisto a cui si desidera allegare un file e, successivamente, scegliere l'azione **Allega file**.
4. Nella finestra **Inserisci file** selezionare il file che rappresenta il documento in entrata in questione, quindi scegliere il pulsante **Apri**.

## <a name="to-create-and-connect-an-incoming-document-record-from-a-vendor-ledger-entry"></a>Per creare e connettere un record di documento in entrata da un movimento di contabilità fornitori
1. Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **Movimenti contabili fornitori**, quindi scegliere il collegamento correlato.
2. Selezionare una riga relativa a un movimento contabile fornitore a cui si desidera allegare un file e quindi scegliere l'azione **Crea documento in entrata da file**.
3. In alternativa, selezionare la riga relativa a un movimento contabile fornitore a cui si desidera allegare un file e, successivamente, scegliere l'azione **Allega file**.
4. Nella finestra **Inserisci file** selezionare il file che rappresenta il documento in entrata in questione, quindi scegliere il pulsante **Apri**.

## <a name="to-remove-a-connection-from-an-incoming-document-record-to-a-posted-document"></a>Per rimuovere una connessione dal record di un documento in entrata a un documento registrato
È possibile rimuovere i file allegati da documenti non registrati in qualsiasi momento eliminando il record del documento in entrata correlato. Se il documento è registrato, è innanzitutto necessario rimuovere la connessione dal record del documento in entrata.

1. Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **Documenti in entrata**, quindi scegliere il collegamento correlato.
2. Selezionare la riga per un record in entrata del documento connesso a un documento registrato che si desidera rimuovere quindi selezionare l'azione **Rimuovi riferimento a record**.

La connessione al documento registrato viene rimossa. È ora possibile connettere un altro record di documento in entrata al documento registrato come descritto in questo argomento.

## <a name="see-also"></a>Vedi anche
[Elaborare i documenti in entrata](across-process-income-documents.md)  
[Documenti in entrata](across-income-documents.md)  
[Acquisti](purchasing-manage-purchasing.md)  
[Utilizzo di [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

