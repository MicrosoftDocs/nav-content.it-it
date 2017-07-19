---
title: 'Procedura: Rettificare i costi degli articoli'
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
ms.openlocfilehash: 59db38c159dd2810656edc668ee431c6414b9d90
ms.contentlocale: it-it
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-adjust-item-costs"></a>Procedura: Rettificare i costi degli articoli   
Il costo di un articolo (valore di magazzino) che si acquista e in seguito si vende può variare nel tempo, ad esempio perché un costo di spedizione viene aggiunto al costo di acquisto dopo che è stato venduto l'articolo. Per conoscere sempre il valore di magazzino corretto, i costi degli articoli devono quindi essere regolarmente rettificati.
In questo modo si garantisce che le statistiche relative ai margini siano aggiornate e che gli indicatore KPI finanziari siano corretti.

**Nota**: i costi degli articoli vengono rettificati solo tramite il metodo di costing FIFO. Questo significa che il costo unitario di un articolo è il valore effettivo di tutto il carico dell'articolo e che il magazzino viene calcolato in base al presupposto secondo cui i primi articoli inseriti in magazzino sono i primi a essere venduti.

Tramite i processi della funzione di rettifica dei costi vengono elaborati solo i movimenti di valorizzazione che non sono ancora stati rettificati. Se si verifica una situazione in cui è necessario trasferire costi in entrata modificati ai movimenti in uscita associati, vengono creati nuovi movimenti di valorizzazione di rettifica, basati sulle informazioni dei movimenti di valorizzazione originali, ma che contengono l'importo di rettifica. La funzione di rettifica dei costi viene utilizzata la data di registrazione del movimento di valorizzazione originale, a meno che tale data non sia inclusa in un periodo di magazzino chiuso. In tal caso, viene utilizzata la data di inizio del successivo periodo di magazzino aperto. Se non si utilizzano i periodi di magazzino, la data nel campo **Consenti registraz. da** nella finestra **Setup contabilità generale** verrà definita quando la rettifica viene registrata.

**Nota**: dopo avere immesso i costi degli articoli sono stati rettificati, il costo di magazzino deve essere registrato nella contabilità generale, automaticamente o manualmente. Per ulteriori informazioni, vedere [Procedura: Registrare costi di magazzino nella contabilità generale](inventory-how-post-inventory-cost-gl.md).

È possibile rettificare i costi articolo in due modi:
 - Impostare il sistema affinché venga effettuata la rettifica automatica delle eventuali modifiche dei costi ogni volta che si verificano transazioni di magazzino.
 - Manualmente, eseguendo il processo batch **Rettifica costo - Movimenti articoli** per uno o più articoli quando si è a conoscenza che i relativi costi hanno modificato.  

## <a name="to-adjust-item-costs-automatically"></a>Per rettificare i costi degli articoli automaticamente
1. Nell'angolo superiore destro, scegliere l'icona **Cerca pagina o report**, immettere **Setup magazzino**, quindi scegliere il collegamento correlato.
2. Nella finestra **Setup magazzino**, nel campo **Rettifica costo automatica**, selezionare uno dei seguenti valori.

|Opzione |Comportamento |
|-------|---------|
|Mai|I costi non vengono rettificati al momento della registrazione.|
|Giorno|I costi vengono rettificati se la registrazione avviene entro un giorno dalla work date.|
|Settimana|I costi vengono rettificati se la registrazione avviene entro una settimana dalla work date.|
|Mese|I costi vengono rettificati se la registrazione avviene entro un mese dalla work date.|
|Trimestre|I costi vengono rettificati se la registrazione avviene entro un trimestre dalla work date.|
|Anno|I costi vengono rettificati se la registrazione avviene entro un anno dalla work date.|
|Sempre|I costi vengono sempre rettificati durante la registrazione, indipendentemente dalla data di esecuzione dell'operazione.|

## <a name="to-adjust-item-costs-manually"></a>Per rettificare i costi degli articoli manualmente
1. Nell'angolo superiore destro, scegliere l'icona **Cerca pagina o report**, immettere **Rettifica costo movimenti articoli**, quindi scegliere il collegamento correlato.
2. Nella finestra **Rettifica costo movimenti articoli**, specificare gli articoli per cui rettificare i costi e se i costi rettificati verranno registrati nella contabilità generale contemporaneamente.

## <a name="see-also"></a>Vedi anche
[Gestire i costi del magazzino](inventory-manage-inventory.md)  
[Procedura: Registrare costi di magazzino nella contabilità generale](inventory-how-post-inventory-cost-gl.md)  
[Gestire le vendite](sales-manage-sales.md)  
[Gestire gli acquisti](purchasing-manage-purchasing.md)

