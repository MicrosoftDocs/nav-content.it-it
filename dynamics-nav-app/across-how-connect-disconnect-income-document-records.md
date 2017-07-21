---
title: 'Procedura: Connettere e disconnettere i record di documenti in entrata da documenti e movimenti'
author: SorenGP
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: fece4e6e38075db6d394c71418fda82a7aa082e1
ms.contentlocale: it-it
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-connect-and-disconnect-incoming-document-records-from-documents-and-entries"></a>Procedura: Connettere e disconnettere i record di documenti in entrata da documenti e movimenti
È possibile archiviare i documenti aziendali esterni in Dynamics NAV allegando i file del documento ai record di documento in entrata correlati. Se il documento, ad esempio una fattura di acquisto, non è stato creato come record di documento in arrivo, è comunque possibile creare e connettere ad esso un record di documento in arrivo in un secondo momento. È inoltre possibile allegare file di documento in entrata a documenti di vendita e di acquisto registrati e a movimenti di contabilità cliente o fornitore utilizzando il Dettaglio informazioni di **File di documento in entrata** ad esempio nelle finestre **Fatture acquisto registrate** e **Movimenti contabili fornitori**.

Nelle finestre **Piano dei conti** e **Movimenti C/G** è possibile utilizzare una funzione di ricerca per trovare movimenti di contabilità generale per documenti di vendita e di acquisto registrati che non hanno record di documenti in entrata e successivamente collegarli centralmente a record esistenti o crearne di nuovi con file di documento allegati. Per ulteriori informazioni, vedere [Procedura: Trovare documenti registrati senza record di documenti in entrata](across-how-find-posted-documents-without-income-document-records.md).

Le procedure riportate di seguito mostrano come allegare un file a una fattura di acquisto esistente che non è stata creata da un record di documento in entrata e come allegare un file a un movimento contabile fornitore. L'operazione di allegare un file a documenti di vendita o di acquisto registrati funziona in modo analogo.

## <a name="to-create-and-connect-an-incoming-document-record-from-a-purchase-invoice"></a>Per creare e connettere un record di documento in entrata da una fattura di acquisto
1. Nell'angolo superiore destro, scegliere l'icona **Cerca pagina o report**, immettere **Fatture acquisto**, quindi scegliere il collegamento correlato.
2. Selezionare la riga relativa a una fattura di acquisto a cui si desidera allegare un file e quindi scegliere l'azione **Crea documento in entrata da file**.
3. In alternativa, selezionare la riga relativa a una fattura di acquisto a cui si desidera allegare un file e, successivamente, scegliere l'azione **Allega file**.
4. Nella finestra **Inserisci file** selezionare il file che rappresenta il documento in entrata in questione, quindi scegliere il pulsante **Apri**.

## <a name="to-create-and-connect-an-incoming-document-record-from-a-vendor-ledger-entry"></a>Per creare e connettere un record di documento in entrata da un movimento di contabilità fornitori
1. Nell'angolo superiore destro, scegliere l'icona **Cerca pagina o report**, immettere **Movimenti contabili fornitori**, quindi scegliere il collegamento correlato.
2. Selezionare una riga relativa a un movimento contabile fornitore a cui si desidera allegare un file e quindi scegliere l'azione **Crea documento in entrata da file**.
3. In alternativa, selezionare la riga relativa a un movimento contabile fornitore a cui si desidera allegare un file e, successivamente, scegliere l'azione **Allega file**.
4. Nella finestra **Inserisci file** selezionare il file che rappresenta il documento in entrata in questione, quindi scegliere il pulsante **Apri**.

## <a name="to-remove-a-connection-from-an-incoming-document-record-to-a-posted-document"></a>Per rimuovere una connessione dal record di un documento in entrata a un documento registrato
È possibile rimuovere i file allegati da documenti non registrati in qualsiasi momento eliminando il record del documento in entrata correlato. Se il documento è registrato, è innanzitutto necessario rimuovere la connessione dal record del documento in entrata.

1. Nell'angolo superiore destro, scegliere l'icona **Cerca pagina o report**, immettere **Documenti in entrata**, quindi scegliere il collegamento correlato.
2. Selezionare la riga per un record in entrata del documento connesso a un documento registrato che si desidera rimuovere quindi selezionare l'azione **Rimuovi riferimento a record**.

La connessione al documento registrato viene rimossa. È ora possibile connettere un altro record di documento in entrata al documento registrato come descritto in questo argomento.

## <a name="see-also"></a>Vedi anche  
[Elaborare i documenti in entrata](across-process-income-documents.md)  
[Documenti in entrata](across-income-documents.md)  
[Gestire gli acquisti](purchasing-manage-purchasing.md)  
[Utilizzare Dynamics NAV](ui-work-product.md)

