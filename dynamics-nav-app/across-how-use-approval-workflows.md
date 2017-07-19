---
title: 'Procedura: Utilizzare i workflow di approvazione'
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
ms.openlocfilehash: e4135aa801b0b507b5f179d02a240a7554ed45cd
ms.contentlocale: it-it
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-use-approval-workflows"></a>Procedura: Utilizzare i workflow di approvazione
Quando un record, ad esempio un documento di acquisto o una scheda cliente, deve essere approvato da una persona della propria organizzazione, inviare una richiesta di approvazione come parte di un flusso di lavoro. In base all'impostazione del flusso di lavoro, al responsabile dell'approvazione appropriato viene inviata una notifica relativa alla richiesta di approvazione del record.

I workflow di approvazione principali dei documenti di acquisto e vendita, le registrazioni dei pagamenti, le schede cliente e le schede articolo sono un punto di inizio per il setup assistito. Per ulteriori informazioni, vedere [Benvenuto in Dynamics NAV](across-get-started.md).

## <a name="to-request-approval-of-a-record"></a>Per richiedere l'approvazione di un record
La seguente attività viene eseguita da un utente approvazione.

1. Nella finestra del record, selezionare l'azione **Invia richiesta approvazione**.
2. Per visualizzare tutte le richieste di approvazione, nell'angolo superiore destro, scegliere l'icona **Cerca pagina o report**, immettere **Movimenti richieste approvazione**, quindi scegliere il collegamento correlato.

Lo stato del movimento di approvazione viene aggiornato da **Creato** ad **Aperto**. Lo stato del record, ad esempio per una una fattura di acquisto, viene aggiornato da **Aperto** a **Approvazione in sospeso** e rimane bloccato per l'elaborazione finché tutti i responsabili dell'approvazione non hanno approvato il record.

Quando il responsabile dell'approvazione ha approvato il record, lo stato viene impostato su **Rilasciato**. È quindi possibile continuare con i task del record.

## <a name="to-cancel-requests-for-approval"></a>Per annullare le richieste di approvazione
La seguente attività viene eseguita da un utente approvazione con diritti di approvazione.

È possibile che un cliente desideri modificare un ordine dopo che questo è stato inviato per l'approvazione. In questo caso, è possibile annullare il processo di approvazione e apportare le modifiche necessarie all'ordine prima di richiedere nuovamente l'approvazione.

1. Nella finestra in cui viene visualizzato il record, selezionare l'azione **Annulla richiesta approvazione**.

Una volta che la richiesta di approvazione è stata annullata, lo stato della voce di approvazione correlata viene impostato automaticamente su **Annullato**. Lo stato del record viene aggiornato da **Approvazione in sospeso** ad **Aperto**. Il processo di approvazione può quindi essere avviato nuovamente.

## <a name="to-make-minor-changes-to-approved-records"></a>Per apportare modifiche di lieve entità a record approvati
Se si desidera apportare una modifica di lieve entità a un record dopo la relativa approvazione, è possibile riaprire il record, apportare la modifica e, successivamente, rilasciarlo. Per le modifiche di lieve entità, questa operazione può essere eseguita mediante i pulsanti **Riapri** e **Rilascia**.

1. Aprire la finestra in cui è visualizzato il record, ad esempio una fattura di acquisto, e scegliere l'azione **Riapri**.

    Il campo **Stato del documento** viene impostato su Aperto.
3. Apportare le modifiche necessarie al record, ad esempio l'indirizzo del fornitore.
4. Scegliere l'azione **Rilascia**.

Quando si riapre il record originale, lo stato del movimento di approvazione correlato rimane Approvato nella finestra **Movimenti approvazione**.

## <a name="to-approve-or-reject-requests-for-approval"></a>Per approvare o rifiutare le richieste di approvazione
La seguente attività viene eseguita da un utente approvazione con diritti di approvazione.

È possibile elaborare le richieste di approvazione nella finestra **Richieste da approvare**, ad esempio per approvare più richieste per volta. In alternativa, è possibile elaborare ogni richiesta nel record correlati, ad esempio nella finestra **Fattura acquisto** scegliendo il collegamento nella notifica ricevuta.

1. Nell'angolo superiore destro, scegliere l'icona **Cerca pagina o report**, immettere **Richieste da approvare**, quindi scegliere il collegamento correlato.
2. Selezionare una o più righe per il record o i record che si desidera approvare o rifiutare.
3. Selezionare l'azione **Approva**, **Rifiuta** o **Delega**.

Una volta che un record è stato approvato o rifiutato, lo stato di approvazione nel campo **Stato** viene automaticamente impostato su **Approvato** o **Rifiutato**.

Se è impostata una gerarchia di responsabili, lo stato del record sarà impostato su **Approvazione in sospeso** fino a quando tutti i responsabili non avranno approvato il record. A quel punto lo stato del record verrà impostato automaticamente su **Rilasciato**.

Contemporaneamente, lo stato di approvazione cambierà da **Creato** ad **Aperto** non appena verrà creata una richiesta di approvazione per il record. Se la richiesta viene rifiutata, lo stato di approvazione diventa **Rifiutato**. Lo stato rimane **Aperto** o **Rifiutato** fino a quando tutti i responsabili non hanno approvato la richiesta.

## <a name="to-delegate-requests-for-approval"></a>Per delegare le richieste di approvazione
La seguente attività viene eseguita da un utente approvazione con diritti di approvazione.

Per impedire l'accumularsi dei documenti nel sistema o un eventuale altro blocco del flusso di lavoro, il responsabile dell'approvazione e l'amministratore dell'approvazione possono delegare la richiesta di approvazione a un sostituto. Il sostituto può essere un sostituto designato, il responsabile approvazione diretto o l'amministratore approvazioni, in tale ordine di priorità. Questa funzionalità viene in genere utilizzata se il responsabile dell'approvazione si trova fuori sede e non è in grado di approvare le richieste prima della data di scadenza.

1. Nell'angolo superiore destro, scegliere l'icona **Cerca pagina o report**, immettere **Richieste da approvare**, quindi scegliere il collegamento correlato.
2. Selezionare una o più righe per le richieste di approvazione che si desidera delegare a un responsabile sostitutivo e quindi scegliere l'azione **Delega**.

Viene inviata una notifica nella quale viene chiesto al responsabile sostitutivo di approvare la richiesta.

## <a name="to-manage-overdue-approval-requests"></a>Per gestire le richieste di approvazione scadute
La seguente attività viene eseguita da un utente approvazione con diritti di approvazione.

A intervalli regolari, è necessario ricordare, agli utenti del flusso di lavoro di approvazione, le richieste di approvazione scadute su cui devono intervenire. A tal fine è possibile utilizzare la funzione Invia notifiche di approvazione scadute.

La funzione Invia notifiche di approvazione scadute cerca tutte le richieste di approvazione aperte attualmente scadute. Ogni responsabile a cui è associato almeno un movimento di approvazione scaduto riceve una notifica con l'elenco di tutte le relative richieste di approvazione scadute. La notifica viene anche inviata in copia per conoscenza al responsabile dell'approvazione e a tutti i richiedenti delle approvazioni scadute. Questa operazione è utile se il movimento di approvazione scaduto deve essere delegato a un sostituto.

1. Nell'angolo superiore destro, scegliere l'icona **Cerca pagina o report**, immettere **Richieste di approvazione scadute**, quindi scegliere il collegamento correlato.
2. Nella finestra **Richieste di approvazione scadute**, scegliere l'azione **Invia notifiche di approvazioni scadute**.

## <a name="see-also"></a>Vedi anche  
[Gestire le vendite](sales-manage-sales.md)    
[Documenti in entrata](across-income-documents.md)  
[Gestire gli acquisti](purchasing-manage-purchasing.md)  
[Utilizzare Dynamics NAV](ui-work-product.md)

