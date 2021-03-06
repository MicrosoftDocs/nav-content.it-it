---
title: Esportare file Positive Pay
description: Assicurarsi che la banca compensi solo gli assegni e gli importi convalidati tramite l'esportazione di file Positive Pay che contengano informazioni sul fornitore e pagamento.
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: check, clearing
ms.date: 06/16/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: bf09817e318b5338da0358f829ea2ed1edde9d67
ms.contentlocale: it-it
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-export-a-positive-pay-file"></a>Procedura: Esportare un file Positive Pay
Per assicurarsi che la banca compensi solo gli assegni e gli importi convalidati, è possibile esportare un file Positive Pay con informazioni su fornitore, numero di assegno e importo del pagamento da inviare alla banca per riferimento quando si elaborano i pagamenti.

[!INCLUDE[d365fin](includes/d365fin_md.md)] è preconfigurato per supportare i file Positive Pay per Bank of America e City Bank.

## <a name="to-set-up-a-bank-account-for-positive-pay"></a>Per impostare un conto bancario per i file Positive Pay
1. Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **C/C bancari**, quindi scegliere il collegamento correlato.
2. Aprire la scheda della banca per cui si desidera utilizzare il Positive Pay.
3. Nel campo **Codice esportazione Positive Pay** immettere POSPAYBANK.
4. Chiudere la finestra.

## <a name="to-export-a-positive-pay-file"></a>Per esportare un file Positive Pay
1. Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **C/C bancari**, quindi scegliere il collegamento correlato.
2. Selezionare il conto bancario per cui si desidera esportare un file Positive Pay.
3. Scegliere l'opzione **Esportazione Positive Pay**.

    Verrà visualizzata la finestra **Esportazione Positive Pay** che mostra i pagamenti che sono stati effettuati per il conto bancario dalla data dell'ultimo caricamento, come mostrato nei campi **Data ultimo caricamento** e **Data ultimo caricamento**.
4. Nel campo **Data limite caricamento** specificare una data prima della quale i pagamenti non sono inclusi nel file esportato.
5. Scegliere l'azione **Esporta**.
6. Nella finestra **Esporta file** scegliere il pulsante **Salva**, quindi salvare il file in un percorso appropriato.
7. Caricare il file nel sito elettronico della banca.
8. Annotare o copiare il numero di conferma visualizzato quando il file viene caricato.

Per visualizzare i record Positive Pay esportati

1. Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **C/C bancari**, quindi scegliere il collegamento correlato.
2. Selezionare il conto bancario per cui si desidera visualizzare i record di esportazione Positive Pay.
3. Scegliere l'azione **Movimenti Positive Pay**.

    Nella finestra **Movimenti Positive Pay** è possibile visualizzare tutti i record di esportazione Positive Pay per il conto corrente bancario.
4. Nel campo **Numero di conferma** immettere per ogni record esportare il numero di conferma che si riceve quando il caricamento del file alla banca è riuscito.
5. Per visualizzare le righe di pagamento, scegliere l'azione **Dettagli movimenti Positive Pay**.

Per riesportare file Positive Pay

1. Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **C/C bancari**, quindi scegliere il collegamento correlato.
2. Selezionare il conto bancario per cui si desidera riesportare i file Positive Pay.
3. Scegliere l'azione **Movimenti Positive Pay**.
4. Selezionare la riga per il file di esportazione Positive Pay da riesportare.
5. Nella finestra **Movimenti Positive Pay** selezionare l'azione **Riesporta Positive Pay su file**.

## <a name="see-also"></a>Vedi anche
[Finanze](finance.md)  
[Impostazione di dati finanziari](finance-setup-finance.md)  
[Utilizzo delle registrazioni COGE](ui-work-general-journals.md)  
[Utilizzo di [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

