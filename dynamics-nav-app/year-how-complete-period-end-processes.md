---
title: Chiudere i periodi
author: jswymer
ms.custom: na
ms.date: 09/16/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: ac1ed2d1dcf8bf780bda91fbf0a04e5c5e8d106a
ms.contentlocale: it-it
ms.lasthandoff: 06/26/2017

---
# <a name="close-periods"></a>Chiudere i periodi
Non è obbligatorio chiudere i periodi, tuttavia, se lo si desidera, vi sono numerose attività di chiusura del periodo (chiusura del mese) che è possibile svolgere. In questo argomento viene fornita una panoramica dei processi e delle attività che possono o non possono essere necessari per la società.

## <a name="general-ledger"></a>Contabilità generale
* Specificare intervalli di date di registrazione a livello di sistema e specifici dell'utente.

    Ciò specifica le date tra cui le registrazioni sono ammesse. In base alle esigenze aziendali, è possibile limitare gli intervalli di date di registrazione all'inizio del processo di chiusura del periodo o in un secondo momento verso la fine del periodo. Per ulteriori informazioni, vedere [Procedura: Specificare i periodi di registrazione](finance-setup-how-specify-posting-periods.md).
* Apportare tutte le rettifiche C/G necessarie.
* Aggiornare e contabilizzare le registrazioni periodiche.
<!--* Process Consolidations-->
* Eseguire le situazioni contabili come segue:
  1. Aprire la finestra **Situazione contabile** e scegliere l'azione **Stampa**.
  2. Compilare la finestra **Situazione contabile** e scegliere l'azione **Stampa**.

## <a name="sales--receivables"></a>Contabilità clienti
* Registrare tutti gli ordini di vendita, le fatture, le note di credito e gli ordini di reso.
* Contabilizzare tutte le registrazioni incassi.
* Aggiornare e contabilizzare le registrazioni periodiche correlate alla contabilità clienti.
* Riconciliare i crediti v/clienti nella contabilità generale.
* Eseguire il processo batch **Elimina ord. vendita fatturati**.

## <a name="purchases--payables"></a>Contabilità fornitori
* Contabilizzare tutti gli ordini di acquisto, le fatture, le note di credito e gli ordini di reso.
* Contabilizzare tutte le registrazioni pagamenti.
* Aggiornare e contabilizzare le registrazioni periodiche correlate alla contabilità fornitori.
* Eseguire il report **Scadenziario fornitori** e riconciliare i debiti v/fornitori nella contabilità generale.
* Eseguire il processo batch **Elimina ordini acquisto fatturati**.

<!-- ### Fixed Assets
* Post all maintenance costs have been posted through the fixed asset journals or invoices.
* Post adjustments.
* Post appreciation.
* Post depreciation.
* Update and post the recurring fixed asset journal.-->

<!--### Intercompany
* Process Intercompany Postings.-->

## <a name="calculate-and-process-sales-tax"></a>Calcolare ed elaborare l'imposta di vendita.
*  Completare le dichiarazioni fiscali.

## <a name="see-also"></a>Vedi anche
[Chiusura di anni e periodi](year-close-years-periods.md)  
[Chiusura dei libri](year-close-books.md)

