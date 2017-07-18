---
title: 'Procedura: Impostare il servizio di conversione di dati bancari'
author: SorenGP
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: 801e2abee52ec9804028a797e4f330b5e080549a
ms.contentlocale: it-it
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-set-up-the-bank-data-conversion-service"></a>Procedura: Impostare il servizio di conversione di dati bancari
Tramite la finestra **Registraz. pagamenti** è possibile esportare le righe pagamento in un flusso di dati che è possibile quindi caricare alla banca per l'elaborazione automatica in modo che non sia necessario eseguire singolarmente i pagamenti elettronici. Per ulteriori informazioni, vedere [Procedura: Esportare pagamenti in un file della banca](payables-how-export-payments-bank-file.md).

Un provider di servizi globale per convertire le informazioni pagamento in qualsiasi formato di dati richiesto dalla banca viene connesso e preparato per essere abilitato in Dynamics NAV.

Come alternativa al servizio Feed bancario di Envestnet è inoltre possibile utilizzare il servizio di conversione di dati bancari per disporre di un file dell'estratto conto ricevuto dalla banca convertito nel flusso di dati che è possibile importare in Dynamics NAV. Per ulteriori informazioni, vedere [Procedura: Collegare i pagamenti automaticamente e Riconciliazione dei conti correnti bancari](receivables-apply-payments-auto-reconcile-bank-accounts.md).

**Nota**: il servizio di conversione di dati bancari può imporre un limite al numero di righe che possono essere esportate in un file. Se il limite viene superato, viene visualizzato un messaggio di errore. È consigliabile che i file del rendiconto bancario non superino 1000 righe, dato che, in caso contrario, il tempo di elaborazione nel servizio di conversione dati bancari può aumentare significativamente.

## <a name="to-sign-your-company-up-for-the-bank-data-conversion-service"></a>Per iscrivere la società al servizio di conversione di dati bancari
1. Nell'angolo superiore destro, scegliere l'icona **Cerca pagina o report**, immettere **Setup servizio conv. dati banca**, quindi scegliere il collegamento correlato.  
2. Viene aperta la finestra **Setup servizio conv. dati banca** con tre campi precompilati con gli URL del provider del servizio di conversione di dati bancari.

    **Nota**: nel database dimostrativo CRONUS International Ltd. i campi Nome utente e Password sono precompilati con informazioni di connessione dimostrative, che dovranno essere sostituite con le informazioni effettive della società nel momento in cui si procederà all'iscrizione al servizio di conversione di dati bancari.
3. Nel campo **URL iscrizione** scegliere il pulsante Sfoglia per aprire la pagina di iscrizione del provider del servizio.  
4. Nella pagina di iscrizione del provider del servizio dati bancari, immettere il nome utente e la password per l'iscrizione della società al servizio, quindi eseguire il processo di registrazione come indicato dal provider del servizio.

    La società è ora iscritta al servizio di conversione di dati bancari. Continuare immettendo il nome utente e la password specificati per il servizio nei campi di setup correlati in Dynamics NAV.
5. Nella finestra **Setup servizio conv. dati banca**, nel campo **Nome utente**, immettere lo stesso valore che è stato immesso come nome di connessione nella pagina del provider del servizio nel passaggio 4.
6. Nel campo **Password** immettere lo stesso valore che è stato immesso nel campo **Password** nella pagina del provider del servizio nel passaggio 4.

## <a name="to-encrypt-your-login-information"></a>Per crittografare le informazioni di accesso
Si consiglia di proteggere le informazioni di accesso immesse nella finestra **Setup servizio conv. dati banca**. È possibile crittografare dati nel server Dynamics NAV generando nuove chiavi di crittografia o importando quelle esistenti che vengono abilitate nell'istanza del server Dynamics NAV che collega al database.

1. Nella finestra **Setup servizio conv. dati banca** scegliere l'azione **Gestione crittografia**.
2. Nella finestra **Gestione crittografia dati** abilitare la crittografia dei dati.

##<a name="to-view-or-update-the-list-of-currently-supported-bank-data-formats"></a>Per visualizzare o aggiornare la lista dei formati di dati bancari attualmente supportato
1. Nell'angolo superiore destro, scegliere l'icona **Cerca pagina o report**, immettere **Setup servizio conv. dati banca**, quindi scegliere il collegamento correlato.
2. Nella finestra **Setup servizio conv. dati banca**, scegliere l'azione **Nome banca - Lista conversione dati** per aprire l'elenco dei nomi di banca che rappresentano i formati di dati bancari che sono supportati dal servizio di conversione.
3. Nella pagina **Nome banca - Lista conversione dati** scegliere l'azione **Aggiorna lista nomi banche**.

La lista dei formati di dati bancari che sono supportati dal servizio di conversione di dati bancari ora è aggiornata. Si tratta dell'elenco di nomi di banca, filtrato per paese, che è possibile selezionare dal campo **Nome banca - Conversione dati** presente nella finestra **Scheda conto bancario**.

**Nota**: l'aggiornamento dei formati di dati bancari supportati si verifica anche quando si seleziona o si immette un valore nel campo **Nome banca - Conversione dati** del conto corrente bancario.

A questo punto è stata eseguita l'iscrizione al servizio di conversione di dati bancari. Continuare a riflettere le informazioni di iscrizione in ogni conto bancario che utilizzerà il servizio.

## <a name="to-set-up-bank-accounts-to-use-the-bank-data-conversion-service"></a>Per impostare i conti correnti bancari da utilizzare per il servizio di conversione di dati bancari
1. Nell'angolo superiore destro, scegliere l'icona **Cerca pagina o report**, immettere **C/C bancari**, quindi scegliere il collegamento correlato.
2. Aprire la scheda del conto corrente bancario per il quale si esporteranno o importeranno i file della banca utilizzando il servizio di conversione di dati bancari.
3. Nella Scheda dettaglio **Trasferimento**, nel campo **Formato esportazione pagamento** scegliere **Servizio di conversione di dati bancari - Bonifico** per impostare l'esportazione del pagamento.
4. Nel campo **Nome banca - Conversione dati** immettere o selezionare il nome del formato di dati della banca per la quale ci si è iscritti nel passaggio 4 della sezione “Per iscriversi al servizio di conversione di dati bancari”.
5. Ripetere i passaggi da 1 a 4 per altri conti correnti bancari che utilizzeranno la funzionalità di servizio di conversione di dati bancari.

## <a name="see-also"></a>Vedi anche  
[Impostare le attività bancarie](bank-setup-banking.md)  
[Gestire i conti correnti bancari](bank-manage-bank-accounts.md)

