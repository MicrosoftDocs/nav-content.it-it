---
title: 'Procedura: esportare pagamenti in un file della banca'
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
ms.openlocfilehash: 09bdf56b3d5e76b12d868091e89232ce9c08e215
ms.contentlocale: it-it
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-export-payments-to-a-bank-file"></a>Procedura: esportare pagamenti in un file della banca
Quando si è pronti a effettuare i pagamenti ai fornitori mediante la finestra **Registrazioni pagamenti**, è possibile esportare un file con le informazioni di pagamento nelle righe di registrazione. È quindi possibile caricare il file sul sito elettronico della banca per elaborare i trasferimenti di denaro correlati.

Nella versione generica di Dynamics NAV, viene installato e connesso un provider di servizi globale per convertire i dati bancari in qualsiasi formato di file richiesto dalla banca.

**Nota**: prima di eseguire l'esportazione dalle registrazioni pagamenti, è necessario abilitare l'esportazione nel batch registrazione correlato. Inoltre, il proprio conto corrente e il conto corrente bancario del fornitore devono essere impostati per il pagamento elettronico. Per ulteriori informazioni, vedere [Procedura: Impostare il servizio di conversione di dati bancari](bank-how-setup-bank-data-conversion-service.md).

Per visualizzare i file di pagamento che sono stati esportati dalle registrazioni pagamenti, si utilizza la finestra **Registri di bonifici**. Da questa finestra è inoltre possibile riesportare i file di pagamento in caso di errori tecnici o di modifiche al file.

## <a name="to-export-payments-to-a-bank-file"></a>Per esportare pagamenti in un file della banca
1. Nell'angolo superiore destro, scegliere l'icona **Cerca pagina o report**, immettere **Registrazioni pagamenti**, quindi scegliere il collegamento correlato.
2. Compilare le righe di registrazione pagamenti, utilizzando la funzione **Sugg. pagamenti fornitore**. Per ulteriori informazioni, vedere [Procedura: Suggerire i pagamenti ai fornitori](payables-how-suggest-vendor-payments.md).  
3. Una volta completate tutte le righe di registrazione pagamenti, scegliere **Esporta pagamenti su file**.

    Tutti i messaggi di errore verranno visualizzati nel riquadro Dettaglio informazioni di **Errori nel file di pagamento** dove è anche possibile scegliere un messaggio di errore per visualizzare informazioni dettagliate. È necessario risolvere tutti gli errori prima di esportare il file di pagamento.

    **Suggerimento**: quando si utilizza il servizio di conversione dati bancari, un messaggio di errore comune informa che il numero di conto corrente bancario non ha la lunghezza richiesta dalla banca. Per evitare o risolvere questo errore, è necessario cancellare il valore nel campo **IBAN** della finestra **Scheda conto bancario**, quindi immettere nel campo **Nr. conto bancario** un numero di conto corrente bancario nel formato richiesto dalla banca.
4. Nella finestra **Salva con nome** specificare il percorso in cui verrà esportato il file e scegliere **Salva**.

Il file di pagamento bancario viene esportato verso il percorso specificato, quindi è possibile procedere a caricarlo nel conto corrente bancario elettronico ed effettuare i pagamenti effettivi.

Quando si riceve conferma che i pagamenti sono stati elaborati correttamente dalla banca, è possibile registrare le righe di registrazione pagamenti esportate.

## <a name="to-plan-when-to-post-exported-payments"></a>Per pianificare quando registrare i pagamenti esportati
Se non si desidera registrare una riga di registrazione pagamenti per un pagamento esportato, ad esempio perché si sta attendendo la conferma che la transazione sia stata lavorata dalla banca, è possibile eliminare la riga di registrazione. Quando in seguito si crea una riga di registrazione pagamenti per pagare l'importo residuo nella fattura, il campo **Importo totale esportato** visualizza la quantità dell'importo pagamento già esportata. Inoltre, è possibile trovare informazioni dettagliate sul totale esportato scegliendo il pulsante **Movimenti dei registri di bonifici** per visualizzare i dettagli relativi ai file di pagamento esportati.

Se si segue una procedura secondo la quale i pagamenti non vengono registrati fino a quando non si riceve la conferma che sono stati elaborati dalla banca, è possibile controllare la situazione in due modi.

* Nelle registrazioni pagamenti con le righe di pagamento suggerite, è possibile ordinare la colonna **Esportato su file pagamento** o **Importo totale esportato** e poi eliminare i suggerimenti di pagamento per le fatture aperte per le quali i pagamenti sono già stati effettuati e per le quali non si desidera creare pagamenti.
* Nella finestra **Sugg. pagamenti fornitore**, dove si specifica quali pagamenti inserire nelle registrazioni pagamenti, è possibile selezionare la casella di controllo **Ignora pagamenti esportati** se non si desidera inserire le righe di registrazione per i pagamenti che sono già stati esportati.

Per visualizzare le informazioni sui pagamenti esportati, scegliere l'azione **Storico esportazione pagamento**.

## <a name="to-re-export-payments-to-a-bank-file"></a>Per riesportare i pagamenti in un file della banca
È possibile riesportare i file di pagamento dalla finestra **Registri di bonifici**. Prima di eliminare o registrare righe di registrazione pagamenti, è possibile anche riesportare il file di pagamento dalla finestra **Registrazioni pagamenti** semplicemente esportandolo di nuovo.

Se sono state eliminate o registrate delle righe di registrazione pagamenti dopo l'esportazione, è possibile riesportare lo stesso file di pagamento dalla finestra **Registri di bonifici**. Selezionare la riga per il batch di bonifici che si desidera riesportare, quindi utilizzare l'azione **Riesporta pagamenti su file**.

## <a name="see-also"></a>Vedi anche
[Contabilità fornitori](payables-manage-payables.md)  
[Gestire gli acquisti](purchasing-manage-purchasing.md)  
[Impostare gli acquisti](purchasing-setup-purchasing.md)

