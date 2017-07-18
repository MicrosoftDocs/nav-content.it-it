---
title: Creazione di numerazioni
author: SusanneWindfeldPedersen
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: 22b3bcf71c99e106527d6bfa35478045d29b9629
ms.contentlocale: it-it
ms.lasthandoff: 06/26/2017

---

# <a name="create-number-series"></a>Creazione di numerazioni

Per ogni società impostata, è necessario assegnare codici di identificazione univoci a elementi quali i conti di contabilità generale, i conti clienti e i conti fornitori, le fatture e i documenti. La numerazione è importante non solo ai fini dell'identificazione. Un sistema di numerazione progettato correttamente semplifica la gestione e l'analisi della società e può ridurre il numero di errori correlati all'immissione dei dati.

È possibile impostare un sistema con una quantità illimitata di numerazioni. È possibile utilizzare le numerazioni per tutti i tipi di documenti e di registrazioni, nonché per l'anagrafica, ad esempio per clienti, articoli e commesse.

È possibile combinare l'utilizzo delle numerazioni con la numerazione manuale.

Per creare un sistema di numerazione, è necessario impostare uno o più codici per ogni tipo di anagrafica o documento. È possibile, ad esempio, impostare un codice per la numerazione dei clienti, un altro per la numerazione delle fatture di vendita e un altro ancora per la numerazione di documenti in registrazioni COGE.

Dopo avere impostato un codice, è necessario impostare almeno una riga di numerazione. Tale riga contiene informazioni quali il primo e l'ultimo numero nella serie e la data di inizio. È possibile impostare più righe di numerazione per codice di numerazione, con una diversa data di inizio per ogni riga. Le numerazioni verranno utilizzate consecutivamente, avviando ciascuna alla rispettiva data di inizio.

Se si desidera utilizzare più codici di numerazione per un tipo di anagrafica, ad esempio per utilizzare una numerazione diversa per diverse categorie di articoli, è possibile utilizzare relazioni tra numerazioni.

Oltre ai numeri assegnati manualmente o tramite l'utilizzo del sistema di numerazione, a tutte le transazioni (movimenti contabili) vengono automaticamente assegnati numeri consecutivi. Tali numeri possono essere visualizzati nel campo **N. movimento** in tutte le finestre dei movimenti contabili. Non è possibile modificare o eliminare tali numeri.

## <a name="to-create-relationships-between-number-series"></a>Per creare relazioni tra numerazioni
È possibile creare relazioni tra codici di numero di serie se ne sono stati impostati più di uno per lo stesso tipo di informazione o transazione di base. Questa funzione può essere utile per selezionare il codice corretto, al momento di utilizzare un numero.

1. Nell'angolo superiore destro, scegliere l'icona **Cerca pagina o report**, immettere **Nr. serie**, quindi scegliere il collegamento correlato.
2. Selezionare la riga contenente la numerazione per la quale si desidera creare delle relazioni, quindi scegliere **Relazioni**.
3. Nel campo **Codice serie** immettere il codice della numerazione che si desidera associare alla serie selezionata nel passaggio 2.
4. Aggiungere una riga per ogni codice che si desidera associare alla numerazione selezionata.
5. Chiudere la finestra.

Ogni volta che verrà impostato un elemento che richiede un numero, è ora possibile utilizzare le relazioni che sono state create per selezionare la numerazione corretta tra quelle poste in relazione.

## <a name="see-also"></a>Vedi anche
[Utilizzare Dynamics NAV](ui-work-product.md)

