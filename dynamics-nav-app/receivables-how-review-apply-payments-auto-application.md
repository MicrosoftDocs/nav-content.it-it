---
title: 'Procedura: Esaminare o collegare i pagamenti manualmente in seguito al collegamento automatico'
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
ms.openlocfilehash: 556a0f74a7407d247008e2d74420803123056eff
ms.contentlocale: it-it
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-review-or-apply-payments-manually-after-automatic-application"></a>Procedura: Esaminare o collegare i pagamenti manualmente in seguito al collegamento automatico
Per ogni riga di registrazione che rappresenta un pagamento nella finestra **Registrazione riconciliazione pagamenti** è possibile aprire la finestra **Collegamento pagamenti** per vedere tutti i movimenti aperti candidati per il pagamento e visualizzare, per ciascun movimento, informazioni dettagliate sulla corrispondenza dei dati su cui si basa un collegamento di pagamento. Qui è possibile collegare manualmente i pagamenti o applicare nuovamente i pagamenti che sono stati collegati automaticamente a un movimento aperto scorretto. Per ulteriori informazioni sul collegamento automatico, vedere [Procedura: Riconciliare i pagamenti utilizzando il collegamento automatico](receivables-how-reconcile-payments-auto-application.md).

**Importante**: quando il conto corrente bancario per il quale si stanno riconciliando i pagamenti è impostato sulla valuta locale, nella finestra **Collegamento pagamenti** vengono mostrati tutti i movimenti aperti nella valuta locale, inclusi i movimenti aperti per i documenti originariamente fatturati in valute estere. I pagamenti collegati ai movimenti con valute convertite possono quindi essere registrati con importi diversi rispetto al documento originale per via dei tassi di cambio potenzialmente diversi utilizzati rispettivamente dalla banca e da Dynamics NAV.

Di conseguenza, consigliamo di guardare i codici valuta estera nel campo **Codice valuta** della finestra **Collegamento pagamenti** per controllare se i collegamenti sono basati su valute convertite. Per verificare l'importo del documento originale in valuta estera e vedere il tasso di cambio utilizzato, scegliere il campo **Collega-a Nr. mov.**, quindi, nel menu di scelta rapida, fare clic sul pulsante drilldown per aprire la finestra **Movimenti contabili clienti** o la finestra **Movimenti contabili fornitori**.

Ogni rettifica di guadagno-e-perdite resa necessaria dalle conversioni di valuta non viene gestita automaticamente da Dynamics NAV.

**Nota**: non è possibile collegare movimenti con segno diverso dal segno sul pagamento. Ad esempio, per chiudere sia una nota di credito di segno negativo che la relativa fattura relativa di segno positivo, è necessario innanzitutto collegare la nota di credito alla fattura, quindi collegare il pagamento alla fattura con l'importo residuo ridotto.

**Avviso**: se si utilizzano sconti sul pagamento e se la data di pagamento è anteriore alla data di scadenza del pagamento, verrà utilizzato per la corrispondenza il campo **Importo residuo incluso sconto** della finestra **Collegamento pagamenti**. In alternativa, verrà utilizzato il valore del campo **Importo residuo**. Se il pagamento è stato eseguito con un importo scontato dopo la data di scadenza del pagamento, o l'importo completo è stato pagato ma è stato concesso uno sconto, non sarà possibile far corrispondere l'importo.

**Nota**: è possibile collegare un pagamento a un solo conto. Se si desidera suddividere il collegamento su più movimenti aperti, ad esempio per collegare un pagamento forfettario, i movimenti aperti devono essere per lo stesso conto. Per ulteriori informazioni, vedere passaggi 7 e 8 della procedura in questo argomento.

## <a name="to-review-or-apply-payments-after-automatic-application"></a>Per esaminare o collegare i pagamenti in seguito al collegamento automatico
1. Nell'angolo superiore destro, scegliere l'icona **Cerca pagina o report**, immettere **Registrazioni riconciliazione pagamenti**, quindi scegliere il collegamento correlato.
2. Aprire la registrazione della riconciliazione di pagamento di un conto corrente bancario per cui si desidera riconciliare i pagamenti. Per ulteriori informazioni, vedere [Procedura: Riconciliare i pagamenti utilizzando il collegamento automatico](receivables-how-reconcile-payments-auto-application.md).
3. Nella finestra **Registrazione riconciliazione pagamenti**, selezionare un pagamento che si desidera esaminare o collegare manualmente a uno o più movimenti aperti, quindi scegliere l'azione **Collega manualmente**.
4. Selezionare la casella di controllo **Collegato** nella riga del movimento aperto al quale si vuole collegare il pagamento.
5. L'importo del pagamento, che viene mostrato anche nel campo **Importo transazioni** della finestra **Collegamento pagamenti**, viene inserito nel campo **Importo collegato**. Il campo può tuttavia essere modificato, ad esempio se si desidera collegare l'importo a numerosi movimenti aperti.
6. Per collegare una parte dell'importo pagato a un altro movimento aperto per il conto, ad esempio per collegare un pagamento forfettario, selezionare la casella di controllo **Collegato** per la riga. L'importo collegato viene automaticamente dedotto dall'importo della transazione per riflettere la distribuzione dei due movimenti aperti.
7. Per collegare una parte di un pagamento a uno o più movimenti aperti inesistenti nel database, creare una nuova riga sotto la riga per lo stesso conto. Nel campo **Importo collegato** immettere l'importo da collegare nella nuova riga, quindi rettificare il campo **Importo collegato** nella riga esistente.
8. Ripetere i passaggi 5, 6 o 7 per gli altri movimenti aperti a cui si desidera collegare una parte o il totale dell'importo di pagamento.
9. Una volta esaminato un collegamento di pagamento o collegato manualmente a uno o più movimenti aperti, scegliere l'azione **Accetta collegamento**.

Viene chiusa la finestra **Collegamento pagamenti** e nella finestra **Registrazione riconciliazione pagamenti** il valore del campo **Affidabilità corrispondenza** viene modificato in **Accettato** a indicare che il pagamento è stato esaminato o collegato manualmente.

## <a name="see-also"></a>Vedi anche
[Gestire la contabilità clienti](receivables-manage-receivables.md)  
[Gestire le vendite](sales-manage-sales.md)

