---
title: 'Procedura: Impostare il servizio di Feed bancario di Envestnet Yodlee'
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
ms.openlocfilehash: 270568214afd2ca8af15f0fa7640337c77ec2f1e
ms.contentlocale: it-it
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-set-up-the-envestnet-yodlee-bank-feeds-service"></a>Procedura: Impostare il servizio di Feed bancario di Envestnet Yodlee
È possibile importare gli estratti conto bancari elettronici dalla banca per compilare rapidamente la finestra **Registrazione riconciliazione pagamenti** in modo da poter collegare i pagamenti e riconciliare il conto bancario. Per ulteriori informazioni, vedere [Collegare i pagamenti automaticamente e Riconciliazione dei conti correnti bancari](receivables-apply-payments-auto-reconcile-bank-accounts.md).

**Nota**: il servizio Feed bancari di Envestnet Yodlee o un altro servizio di feed bancari del fornitore potrebbe non essere disponibile nel sistema. Contattare il partner di Microsoft se si desidera utilizzare un servizio di feed bancari per importare gli estratti conto.

Dopo avere abilitato il servizio del feed bancario, è necessario collegare il conto corrente bancario interessato al conto corrente bancario online da cui deriva il feed. I conti correnti bancari vengono collegati a conti bancari online nelle seguenti situazioni:

- Un conto corrente bancario non esiste in Dynamics NAV per il conto corrente online. Di conseguenza, si crea il conto corrente bancario collegando il conto corrente bancario online.
- Un conto corrente bancario esiste in Dynamics NAV e si desidera collegarlo a un conto corrente bancario online.
- Il collegamento di conto corrente bancario deve essere annullato perché non si desidera più usare il servizio di feed bancario per il conto.
- I conti correnti bancari online sono stati modificati e si desidera aggiornare le informazioni sui conti correnti bancari in Dynamics NAV.

Quando il servizio del feed della banca è abilitato, è possibile impostare un conto corrente bancario per importare automaticamente nuovi estratti conto bancari nella finestra **Registrazione riconciliazione pagamenti** ogni di due ore. Le transazioni per i pagamenti già registrate come applicate e/o riconciliate nella finestra **Registrazione riconciliazione pagamenti** non verranno incluse. Per ulteriori informazioni, vedere la sezione "Per abilitare l'importazione automatica degli estratti conto bancari".

**Nota**: se si utilizza il setup assistito Imposta società, alcuni passaggi delle procedure riportate di seguito verranno eseguiti automaticamente quando si raggiunge il setup del conto corrente bancario della società. Per ulteriori informazioni, vedere [Benvenuto in Dynamics NAV](across-get-started.md).

## <a name="to-enable-the-bank-feed-service"></a>Per abilitare il servizio di feed bancario
1. Nell'angolo superiore destro, scegliere l'icona **Cerca pagina o report**, immettere **C/C bancari**, quindi scegliere il collegamento correlato.
2. Aprire il conto corrente bancario da utilizzare per il servizio di feed bancari.
3. Nella finestra **Conto bancariot** nel campo **Formato importazione rendiconto bancario** selezionare YODLEEBANKFEED.  

Il servizio di feed bancari verrà abilitato quando si collega un conto corrente bancario al conto corrente bancario online correlato. Vedere la procedura seguente.  

## <a name="to-create-a-new-linked-bank-account"></a>Per creare un nuovo conto bancario collegato
1. Nell'angolo superiore destro, scegliere l'icona **Cerca pagina o report**, immettere **C/C bancari**, quindi scegliere il collegamento correlato.
2. Selezionare il conto corrente bancario appropriato e fare clic su **Crea nuovo conto bancario collegato**. Dopo alcuni istanti, si apre la finestra **Collegamento conto bancario**.

    **Nota**: questa finestra mostra l'effettiva pagina Web del servizio Feed bancari di Envestnet Yodlee. La terminologia e la funzionalità della finestra potrebbero non corrispondere alle indicazioni fornite in questo argomento.  
3. Nella finestra **Collegamento conto bancario online** nel riquadro **Collegamento conto**, utilizzare la funzione di ricerca per trovare la banca presso cui si trovano uno o più conti correnti bancari online.
4. Scegliere il nome della banca. Viene visualizzato il riquadro di **accesso**.
5. Immettere il nome utente e la password utilizzati per accedere alla banca online, quindi selezionare il pulsante **Avanti**.  
6. Il servizio di feed bancario prepara il collegamento del primo conto corrente bancario online della banca specificata a un nuovo conto corrente bancario in Dynamics NAV.

    **Nota**: se si dispone di più di un conto corrente bancario online presso la banca, è necessario creare conti correnti bancari aggiuntivi in Dynamics NAV per i conti online aggiuntivi. Vedere i passaggi da 8 a 10.

    Al termine del processo senza errori, il nome della banca apparirà nel riquadro **Conti personali** collegato nella scheda **Collegato**. Il numero tra parentesi indica il numero di conti bancari online che sono stati collegati.
7. Scegliere il pulsante **OK**.

    Se un solo conto bancario online è collegato, si apre la finestra **Scheda conto bancario** per un nuovo conto precompilata con il nome del conto bancario online. Questo indica che l'attività di collegamento del conto corrente bancario è stata completata. L'unica cosa che rimane da fare è impostare il conto bancario. Per ulteriori informazioni, vedere [Procedura: Impostare i conti correnti bancari](bank-how-setup-bank-accounts.md).

    Se più dei conti bancari online sono stati collegati, si apre la finestra **Collegamento conto bancario** con une elenco dei conti bancari online aggiuntivi che non sono ancora collegati ai conti bancari in Dynamics NAV. In questo caso, seguire il passaggio successivo.  
8. Nella finestra **Collegamento conto bancario**, selezionare la riga per un conto corrente bancario online quindi selezionare l'azione **Collega a nuovo conto bancario**.

    Si apre la finestra **Scheda conto bancario** per un nuovo conto precompilata con il nome del conto bancario online.

    Se un conto corrente bancario è già esistente in Dynamics NAV e si desidera collegare il conto bancario online aggiuntivo, seguire il passaggio successivo.  
9. Nella finestra **Collegamento conto bancario**, selezionare la riga per un conto corrente bancario online quindi selezionare l'azione **Collega a conto bancario esistente**.
10. Nella finestra **Lista C/C bancari** selezionare il conto bancario per il quale si desidera effettuare il collegamento e quindi fare clic su **OK**.

## <a name="to-link-a-bank-account-to-an-online-bank-account"></a>Per collegare un conto bancario a un conto bancario online
1. Nell'angolo superiore destro, scegliere l'icona **Cerca pagina o report**, immettere **C/C bancari**, quindi scegliere il collegamento correlato.
2. Selezionare la riga per un conto bancario non collegato a un conto bancario online quindi selezionare l'azione **Collega a conto bancario online**. Si apre la finestra **Collegamento conto bancario online** con il nome della banca precompilato nel riquadro **Collegamento conto**.
3. Scegliere il nome della banca. Viene visualizzato il riquadro di **accesso**.
4. Immettere il nome utente e la password utilizzati per accedere alla banca online, quindi selezionare il pulsante **Avanti**.

    Il servizio di feed bancario prepara il collegamento del conto corrente bancario al conto bancario online corrispondente in Dynamics NAV.

    Al termine del processo senza errori, il nome della banca apparirà nel riquadro **Conti personali** collegato nella scheda **Collegato**. Se la banca ha più di un conto corrente bancario, solo il conto corrente bancario selezionato nel passaggio 2 verrà collegato.
5. Scegliere il pulsante **OK**.

Nella finestra **Lista C/C bancari** è selezionata la casella di controllo **Collegato**.

## <a name="to-unlink-a-bank-account"></a>Per scollegare un conto bancario
1. Nell'angolo superiore destro, scegliere l'icona **Cerca pagina o report**, immettere **C/C bancari**, quindi scegliere il collegamento correlato.  
2. Selezionare la riga per un conto bancario collegato che si desidera scollegare dal relativo conto bancario online e quindi selezionare l'azione **Scollega conto bancario online**.

**Nota**: se si sceglie **Sì** nella finestra di dialogo di conferma, il collegamento al conto bancario online viene rimosso e i dettagli di accesso vengono cancellati. Per collegare il nuovo conto bancario al conto bancario online, è necessario collegarsi ancora alla banca. Per ulteriori informazioni, vedere la sezione "Per collegare un conto bancario a un conto bancario online".

## <a name="to-update-bank-account-linking"></a>Per aggiornare il collegamento del conto bancario
1. Nell'angolo superiore destro, scegliere l'icona **Cerca pagina o report**, immettere **C/C bancari**, quindi scegliere il collegamento correlato.
2. Selezionare il conto corrente bancario appropriato e selezionare l'azione **Aggiorna collegamento conto bancario**.

Se esistono dei problemi per uno dei conti bancari collegati nella finestra **Lista C/C bancari** si apre la finestra **Collegamento conto bancario** in cui sono specificati i conti correnti bancari con problemi. Il modo migliore per risolvere i problemi consiste nello scollegare il conto bancario online e quindi ricreare il collegamento. Per ulteriori informazioni, vedere la sezione "Per collegare un conto bancario a un conto bancario online".

## <a name="to-enable-automatic-import-of-bank-statements"></a>Per abilitare l'importazione automatica degli estratti conto bancari
1. Nell'angolo superiore destro, scegliere l'icona **Cerca pagina o report**, immettere **C/C bancari**, quindi scegliere il collegamento correlato.
2. Selezionare la riga per un conto corrente bancario collegato quindi selezionare l'azione **Setup importazione automatica rendiconti bancari**.
3. Nella finestra **Setup importazione automatica rendiconti bancari** nel campo **Numero di giorni inclusi** specificare il periodo per recuperare le nuove transazioni bancarie.

    **Nota**: si consiglia di impostare il valore di 7 o più giorni.
4. Selezionare la casella **Abilitato**.  
Ogni ora, la finestra **Registrazione riconciliazione pagamenti** verrà verrà compilata con tutti i nuovi pagamenti che vengono effettuati sul conto bancario online.

**Nota**: le transazioni per i pagamenti già registrate come applicate e/o riconciliate nella finestra **Registrazione riconciliazione pagamenti** non verranno incluse.

## <a name="see-also"></a>Vedi anche  
[Impostare le attività bancarie](bank-setup-banking.md)  
[Gestire i conti correnti bancari](bank-manage-bank-accounts.md)  
[Collegare i pagamenti automaticamente e riconciliare i conti correnti bancari](receivables-apply-payments-auto-reconcile-bank-accounts.md)  
[Personalizzazione di Dynamics NAV utilizzando le estensioni ](ui-extensions.md)

