---
title: Impostare i conti correnti bancari
description: "È possibile riconciliare i conti correnti bancari in Dynamics NAV con gli estratti conto della banca."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: feed, stream
ms.date: 09/26/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 3581615fe94006aa9245f5e66fe6cf475b22acfb
ms.contentlocale: it-it
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-set-up-bank-accounts"></a>Procedura: impostare i conti correnti bancari
I conti correnti bancari vengono utilizzati in [!INCLUDE[d365fin](includes/d365fin_md.md)] per tenere traccia delle transazioni bancarie. I conti possono essere denominati in valuta locale o estera. Dopo aver impostato i conti correnti bancari è possibile utilizzare l'opzione per la stampa di assegni.

## <a name="to-set-up-bank-accounts"></a>Per impostare i conti correnti bancari
1. Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **C/C bancari**, quindi scegliere il collegamento correlato.
2. Nella finestra **C/C bancari** scegliere l'azione **Nuovo**.
3. Compilare i campi come necessario. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

> [!NOTE]
> Per compilare il campo **Saldo** con un saldo iniziale, è necessario registrare un movimento contabile del conto corrente bancario con la quantità in questione. È possibile effettuare questa operazione eseguendo un una riconciliazione bancaria. Per ulteriori informazioni, vedere [Procedura: Riconciliare i conti bancari separatamente](bank-how-reconcile-bank-accounts-separately.md). In alternativa, è possibile implementare il saldo iniziale come parte della creazione di dati generali in nuove aziende utilizzando il setup assistito **Migra dati aziendali**. Per ulteriori informazioni, vedere [Benvenuto in [!INCLUDE[d365fin](includes/d365fin_md.md)](index.md).

## <a name="to-set-up-your-bank-account-for-import-or-export-of-bank-files"></a>Per impostare il conto corrente bancario per l'importazione o l'esportazione di file dei conti correnti bancari
I campi nella nella Scheda dettaglio **Trasferimento** della finestra **Scheda conto corrente bancario** sono correlati all'importazione e all'esportazione dei feed e dei file della banca. Per ulteriori informazioni, vedere [Procedura: Impostare il servizio di conversione di dati bancari](bank-how-setup-bank-data-conversion-service.md).

1. Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **C/C bancari**, quindi scegliere il collegamento correlato.
2. Aprire la scheda di un conto corrente bancario per il quale verranno esportati o importati i file dei conti correnti bancari.
3. Compilare i campi appropriati nella Scheda dettaglio **Trasferimento**. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

> [!NOTE]  
>   I diversi servizi di esportazione file e i rispettivi formati richiedono valori di configurazione differenti nella finestra **Scheda conto corrente bancario**. Si verrà informati sui valori di setup mancanti o non corretti mentre si tenta di esportare il file. Leggere quindi con attenzione le brevi descrizioni dei campi o fare riferimento agli argomenti di procedura correlati. Ad esempio, esportare un file di pagamento per il trasferimento elettronico dei fondi (EFT) in Nord America richiede che sia il campo **Nr. ultimo avviso di rimessa** che il campo **Nr. transito** siano compilati. Per ulteriori informazioni, vedere [Procedura: Esportare pagamenti in un file della banca](payables-how-export-payments-bank-file.md).

## <a name="to-set-up-vendor-bank-accounts-for-export-of-bank-files"></a>Per impostare i conti correnti fornitore per l'esportazione di file dei conti correnti bancari
I campi nella nella Scheda dettaglio **Trasferimento** della finestra **Scheda C/C bancari fornitori** sono correlati all'esportazione dei feed e dei file dei conti correnti bancari. Per ulteriori informazioni, vedere [Procedura: Impostare il servizio di conversione di dati bancari](bank-how-setup-bank-data-conversion-service.md) e [Procedura: Esportare pagamenti in un file della banca](payables-how-export-payments-bank-file.md).

1. Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **Fornitori**, quindi scegliere il collegamento correlato.
2. Aprire la scheda di un conto corrente bancario fornitore nel quale verranno esportati i file di pagamento della banca.
3. Scegliere l'azione **C/C bancari**.
3. Nella Scheda dettaglio **Trasferimenti** della finestra **Scheda C/C bancari fornitori** compilare i campi come richiesto. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

## <a name="to-set-the-opening-balance-on-new-bank-accounts"></a>Per impostare il saldo iniziale su nuovi conti correnti bancari


## <a name="see-also"></a>Vedi anche
[Impostazione delle attività bancarie](bank-setup-banking.md)  
[Gestione di conti correnti bancari](bank-manage-bank-accounts.md)  
[Utilizzo di [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

