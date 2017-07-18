---
title: Dimensioni
author: edupont04
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: a1b38e74717e87bea6efb46f8f4e5236b6ec4e64
ms.contentlocale: it-it
ms.lasthandoff: 06/26/2017

---

#<a name="dimensions"></a>Dimensioni
Le dimensioni sono dati che si aggiungono ai movimenti per suddividerli in categorie di analisi. Ad esempio, è possibile impostare dimensioni che indicano da quale progetto o reparto ha origine un movimento.
quindi utilizzare tali dimensioni anziché impostare conti di contabilità generale distinti per ogni reparto e progetto. In questo modo si disporrà di informazioni dettagliate sull'analisi all'interno dei dati, senza dover utilizzare un piano dei conti complesso.
È possibile definire un numero illimitato di dimensioni con un numero illimitato di valori dimensioni.  

Ad esempio, si imposta una dimensione denominata *Reparto* e si utilizza la dimensione e un valore di dimensione al momento della registrazione dei documenti di vendita. Quindi, è possibile successivamente ottenere i dati di Business Intelligence su quali articoli sono stati venduti per reparto.
Più dimensioni si impostano e utilizzano, più dettagliati sono i report su cui è possibile basare le decisioni aziendali. Un singolo movimento di vendita può includere informazioni relative a dimensioni multiple, ad esempio, il conto nel quale è stato registrato l'articolo, il luogo di vendita, il nome del venditore e la tipologia del cliente che ha effettuato l'acquisto.  

## <a name="using-dimensions"></a>Utilizzo delle dimensioni
In un documento come un ordine di vendita, è possibile aggiungere le informazioni sulle dimensioni sia per una singola riga del documento che l'intero documento. Ad esempio, nella finestra **Ordine di vendita**, i valori dimensioni per le prime due dimensioni a collegamento rapido possono essere immessi direttamente nel documento, mentre le ulteriori informazioni sulle dimensioni relative alla testata possono essere aggiunte selezionando il pulsante **Dimensioni**.  
Se si lavora nelle registrazioni invece, è possibile aggiungere informazioni sulle dimensioni a un movimento nello stesso modo, se le dimensioni a collegamento rapido sono state impostate come campi direttamente sulle righe di registrazione.  
È possibile impostare le dimensioni di default per i conti o i tipi di conto, in modo che le dimensioni e i valori dimensioni vengano compilati automaticamente.  

## <a name="dimension-sets"></a>Set di dimensioni
Un set di dimensioni è una combinazione univoca di valori dimensioni. Viene archiviato come movimenti set di dimensioni nel database. Ogni movimento set di dimensioni rappresenta un valore dimensioni singolo. Il set di dimensioni è identificato da un ID set di dimensioni comune assegnato a ogni movimento set di dimensioni che appartiene al set di dimensioni.  

Quando si crea una nuova riga di registrazione, testata del documento o riga documento, è possibile specificare una combinazione di valori dimensioni. Anziché archiviare esplicitamente ogni valore dimensioni nel database, viene assegnato un ID set di dimensioni alla riga di registrazione, alla testata del documento o alla riga del documento per specificare il set di dimensioni.  

## <a name="see-also"></a>Vedi anche
[Contabilità](finance-setup.md)  
[Impostare le dimensioni](finance-setup-setup-dimensions.md)  

