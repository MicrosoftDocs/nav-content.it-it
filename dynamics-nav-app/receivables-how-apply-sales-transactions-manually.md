---
title: 'Procedura: Riconciliare manualmente i pagamenti dei clienti'
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
ms.openlocfilehash: de0c94386ad5a0bbfba5cc0516fa7faa5cdcc0b4
ms.contentlocale: it-it
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-reconcile-customer-payments-manually"></a>Procedura: Riconciliare manualmente i pagamenti dei clienti
Quando si riceve un incasso da un cliente o si effettua un rimborso in contanti a un cliente, è necessario stabilire se collegare il pagamento o il rimborso a uno o più movimenti contabili aperti. È possibile specificare l'importo esatto che si desidera applicare. È ad esempio possibile applicare solo parte del pagamento e quindi applicare solo parzialmente i movimenti contabili clienti. È importante in una determinata fase chiudere (collegare) tutti i movimenti contabili clienti per ottenere statistiche e stampati clienti corretti degli estratti conto e degli interessi finanziari.

È possibile collegare i movimenti contabili clienti in tre modi diversi:

- Immettendo informazioni nelle finestre dedicate, ad esempio nella finestra **Registrazioni incassi** e nella finestra **Registrazione riconciliazione pagamenti**.
- Dai documenti nota di credito di vendita.
- Dai movimenti contabili clienti dopo che i documenti di vendita sono stati registrati ma non collegati.

**Nota**: se il campo **Metodo collegamento** nella scheda cliente è impostato su **Collega al più Vecchio**, i pagamenti saranno automaticamente collegati al movimento di credito meno recente, a meno che non si specifichi manualmente a quale movimento collegarli. Se il metodo di collegamento per un cliente è impostato su **Manuale**, i movimenti dovranno essere collegati manualmente.

È possibile collegare i pagamenti dei clienti manualmente nella finestra **Registrazioni incassi**. Una registrazione incassi è un tipo di registrazione generale che può essere utilizzata per registrare transazioni in conti di contabilità generale, bancari, cliente, fornitori e cespiti. È possibile collegare il pagamento a uno o più movimenti Dare quando si registra il pagamento oppure collegare dai movimenti registrati in un momento successivo.

È inoltre possibile collegare i pagamenti dei clienti e dei fornitori nella finestra **Registrazione riconciliazione pagamenti** utilizzando le funzioni per l'importazione del rendiconto bancario, il collegamento automatico e la riconciliazione del conto corrente bancario. Per ulteriori informazioni, vedere [Riconciliare i pagamenti utilizzando il collegamento automatico](receivables-how-reconcile-payments-auto-application.md). In alternativa, è possibile riconciliare i pagamenti dei clienti in base a un elenco di documenti di vendita non pagati nella finestra **Registrazione pagamenti**. Per ulteriori informazioni, vedere [Procedura: Riconciliare i pagamenti dei clienti da un elenco di documenti di vendita non pagati](receivables-how-reconcile-customer-payments-list-unpaid-sales-documents.md).

## <a name="to-fill-and-post-a-cash-receipt-journal"></a>Per compilare e contabilizzare una registrazione incasso
1. Nell'angolo superiore destro, scegliere l'icona **Cerca pagina o report**, immettere **Registrazioni incassi**, quindi scegliere il collegamento correlato.
2. Selezionare il batch appropriato nel campo **Nome batch**.
3. Compilare il campo **Data di Registrazione**.  
4. Nel campo **Tipo di documento** selezionare **Pagamento**.

    Il campo **Nr. documento** viene compilato dalla numerazione assegnata al batch.
5. Utilizzare il campo **Nr. documento esterno** per archiviare un identificatore, quale il numero di assegno del cliente.
6. Nel campo **Tipo conto** selezionare **Cliente**.
7. Nel campo **Nr. conto** selezionare il conto C/G desiderato.
8. Se si desidera registrare il collegamento contemporaneamente alle registrazioni, effettuare una delle operazioni seguenti.
9. Nel campo **Tipo contropartita** selezionare **Conto C/G** per i pagamenti in contanti e **Conto C/C bancario** per gli altri pagamenti.
10. Nel campo **Nr. conto profitti/perdite** selezionare il conto cassa per i pagamenti in contanti o il conto bancario appropriato per gli altri pagamenti.
11. Effettuare la registrazione.

## <a name="to-apply-a-payment-to-a-single-customer-ledger-entry"></a>Per collegare un pagamento a un singolo movimento contabile cliente
1. Nell'angolo superiore destro, scegliere l'icona **Cerca pagina o report**, immettere **Registrazioni incassi**, quindi scegliere il collegamento correlato.
2. Nella prima riga delle registrazioni immettere le informazioni relative al movimento da collegare.
3. Nel campo **Tipo di documento** immettere **Pagamento**.
4. Nel campo **Tipo conto** immettere **Cliente**.
5. Nel campo **Tipo contropartita** immettere **Conto bancario**.
6. Nel campo **Collega-a nr. doc.** scegliere il campo da aprire nella finestra **Collega movimenti clienti**.
7. Nella finestra **Collega movimenti clienti** selezionare il movimento a cui collegare il pagamento.
8. Nel campo **Importo da collegare** immettere l'importo che si desidera collegare al movimento. Se non si immette alcun importo, verrà collegato l'importo massimo.

    Nella parte inferiore della finestra **Collega movimenti clienti** è possibile vedere l'importo specifico nel campo **Importo collegato** e anche se il saldo del collegamento è corretto.
9. Scegliere il pulsante **OK**. Nella finestra **Registrazioni incassi** viene a questo punto visualizzato nel campo **Collega-a tipo doc.** e nel campo **Collega-a nr. doc.** il movimento selezionato. .
10. Effettuare la registrazione dell'incasso.

## <a name="to-apply-a-payment-to-multiple-customer-ledger-entries"></a>Per collegare un pagamento a più movimenti contabili clienti
1. Nell'angolo superiore destro, scegliere l'icona **Cerca pagina o report**, immettere **Registrazioni incassi**, quindi scegliere il collegamento correlato.
2. Nella prima riga delle registrazioni immettere le informazioni relative al movimento da collegare.
3. Nel campo **Tipo di documento** immettere **Pagamento**.
4. Nel campo **Tipo conto** immettere **Cliente**.
5. Nel campo **Tipo contropartita** immettere **Conto bancario**.
6. Nel campo **Importo** immettere il pagamento completo come importo negativo.
7. Per collegare il pagamento a più movimenti contabili clienti durante la registrazione, scegliere l'azione **Collega movimenti**.
8. Selezionare le righe con i movimenti a cui si desidera collegare il movimento, quindi scegliere l'azione **Collega a ID**.
9. In ciascuna riga del campo **Importo da collegare** immettere l'importo da collegare al singolo movimento. Se non si immette alcun importo, verrà collegato l'importo massimo.

    Nella parte inferiore della finestra **Collega movimenti clienti** è possibile vedere l'importo specifico nel campo **Importo collegato** e anche se il saldo del collegamento è corretto.
10. Scegliere il pulsante **OK**.
11. Effettuare la registrazione dell'incasso.

## <a name="to-apply-a-credit-memo-to-a-single-customer-ledger-entry"></a>Per collegare una nota di credito a un singolo movimento contabile cliente
1. Nell'angolo superiore destro, scegliere l'icona **Cerca pagina o report**, immettere **Note credito vendita**, quindi scegliere il collegamento correlato.
2. Aprire la nota di credito di vendita desiderata.
3. Per collegare la nota di credito a un singolo movimento contabile cliente durante la registrazione, nel campo **Collega-a nr. doc.**, selezionare il movimento al quale si desidera collegare il pagamento.
4. Nella riga del campo **Importo da collegare** immettere l'importo da collegare al movimento.

    Se non si immette alcun importo, verrà applicato automaticamente l'importo massimo. Nella parte inferiore della finestra **Collega movimenti clienti** è possibile vedere l'importo specifico nel campo **Importo collegato** e anche se il saldo del collegamento è corretto.
5. Scegliere il pulsante **OK**. Nella finestra **Note credito vendita** viene a questo punto visualizzato nel campo **Collega-a tipo doc.** e nel campo **Collega-a nr. doc.** il movimento selezionato. . e l'importo della nota di credito da registrare, rettificato per eventuali sconti di pagamenti.
6. Registrare la nota di credito.

## <a name="to-apply-a-credit-memo-to-multiple-customer-ledger-entries"></a>Per collegare una nota di credito a più movimenti contabili clienti
1. Nell'angolo superiore destro, scegliere l'icona **Cerca pagina o report**, immettere **Note credito vendita**, quindi scegliere il collegamento correlato.
2. Aprire la nota di credito di vendita desiderata.
3. Per collegare la nota di credito a più movimenti contabili clienti durante la registrazione, scegliere l'azione **Collega movimenti**.
4. Selezionare le righe con i movimenti a cui si desidera collegare il movimento, quindi scegliere l'azione **Collega a ID**.
5. In ciascuna riga del campo **Importo da collegare** immettere l'importo da collegare al singolo movimento. Se non si immette alcun importo, verrà collegato l'importo massimo.

  Nella parte inferiore della finestra **Collega movimenti clienti** è possibile vedere l'importo specifico nel campo **Importo collegato** e anche se il saldo del collegamento è corretto.
6. Scegliere il pulsante **OK**. Nella finestra **Nota credito vendita** viene a questo punto visualizzato l'importo della nota di credito da registrare, rettificato di ogni possibile sconto.
7. Registrare la nota di credito.

## <a name="to-apply-posted-customer-ledger-entries"></a>Per collegare i movimenti contabili clienti registrati
1. Nell'angolo superiore destro, scegliere l'icona **Cerca pagina o report**, immettere **Clienti**, quindi scegliere il collegamento correlato.
2. Aprire la scheda cliente relativa al cliente per il quale sono disponibili i movimenti da collegare.
3. Scegliere l'azione **Mov. contabili** e selezionare la riga con il movimento che sarà il movimento di collegamento.
4. Scegliere l'azione **Collega movimenti**. Verrà visualizzata la finestra **Collega movimenti clienti** nella quale saranno indicati i movimenti aperti per il cliente.
5. Selezionare le righe con i movimenti a cui si desidera collegare il movimento, quindi scegliere l'azione **Collega a ID** .
6. In ciascuna riga del campo **Importo da collegare** immettere l'importo da collegare al singolo movimento. Se non si immette alcun importo, verrà collegato l'importo massimo.

    Nella parte inferiore della finestra **Collega movimenti clienti** è possibile vedere l'importo specifico nel campo **Importo collegato**.
7. Scegliere l'azione **Registra collegamento**. Viene visualizzata la finestra **Registra collegamento** con il numero di documento del movimento di collegamento e la data di registrazione del movimento con la data di registrazione più recente.  
8. Scegliere **OK** per registrare il collegamento.

    Se il collegamento registrato ha comportato la creazione di movimenti contabili clienti chiusi, per tali movimenti contabili verrà deselezionato il campo **Aperto**.
9. Per vedere i movimenti contabili, nell'angolo superiore destro, scegliere l'icona **Cerca pagina o report**, immettere **Clienti**, quindi scegliere il collegamento correlato. Spostarsi sulla scheda del cliente per visualizzare i movimenti contabili.

Nella lista dei movimenti contabili, nella riga che contiene il movimento contabile che era stato interamente collegato, è possibile vedere che la casella di controllo **Aperto** non è selezionata.  

**Nota**: dopo aver selezionato un movimento dalla finestra **Collega movimenti clienti** o numerosi movimenti impostando **Collega-a ID**, il campo **Importo collegato** nella riga di registrazione conterrà la somma dei restanti importi per i movimenti registrati selezionati, a meno che il campo non contenga un'impostazione differente. Se si seleziona **Collega al più Vecchio** nel campo **Metodo collegamento** della scheda cliente, il collegamento viene stabilito automaticamente.

## <a name="to-apply-customer-ledger-entries-in-different-currencies-to-one-another"></a>Per collegare movimenti contabili clienti nelle varie valute
Se si effettua una vendita a un cliente in una valuta e si riceve il pagamento in un'altra, è possibile ancora collegare la fattura al pagamento.

Se si collega un movimento (Movimento 1) espresso in una determinata valuta a un movimento (Movimento 2) con valuta diversa, verrà utilizzata la data di registrazione del Movimento 1 per trovare il tasso di cambio appropriato per la conversione degli importi nel Movimento 2. Il tasso di cambio rilevante è disponibile nella finestra **Tassi di cambio valuta**.

È necessario abilitare il collegamento dei movimenti contabili clienti in differenti valute. Per ulteriori informazioni, vedere [Procedura: Abilitare il collegamento dei movimenti contabili fornitore in valute diverse](finance-setup-how-enable-application-ledger-entries-different-currencies.md).

1. Nell'angolo superiore destro, scegliere l'icona **Cerca pagina o report**, immettere **Registrazioni incassi**, quindi scegliere il collegamento correlato.
2. Aprire la registrazione desiderata e compilare la prima riga delle registrazioni vuota con un codice valuta.
3. Scegliere l'azione **Collega movimenti**.
4. Selezionare la riga con il movimento a cui si intende collegare il movimento nelle registrazioni incassi. Scegliere l'azione **Collega a ID**, quindi selezionare il movimento che si desidera collegare.
5. Scegliere **OK** per tornare alle registrazioni incassi.
6. Registrare la registrazione vendite.

**Importante**: quando si collegano movimenti in valute diverse, i movimenti vengono convertiti nella valuta locale. Sebbene i tassi di cambio per le due valute siano fissi, ad esempio tra USD ed EUR, è possibile che durante la conversione di tali valute estere nella valuta locale vengano prodotti importi residui di piccola entità. Gli importi residui vengono registrati come utili e perdite sul conto specificato nel campo **Conto utili realizzati** o **Conto perdite realizzate** della finestra **Valute**. Viene rettificato anche il campo **Importo (USD)** nei movimenti contabili fornitori rilevanti.

## <a name="to-unapply-an-application-of-customer-entries"></a>Per scollegare un collegamento di movimenti clienti
Quando si scollega un collegamento errato, vengono creati e registrati movimenti di rettifica identici a quelli originali ma con segno opposto nel campo relativo all'importo, per tutti i movimenti, incluse le registrazioni di contabilità generale derivanti dal collegamento, quali ad esempio sconto pagamento e profitti e perdite legati alla valuta. Vengono inoltre riaperti i movimenti chiusi dal collegamento.

1. Nell'angolo superiore destro, scegliere l'icona **Cerca pagina o report**, immettere **Clienti**, quindi scegliere il collegamento correlato.
2. Aprire la scheda cliente desiderata.
3. Scegliere l'azione **Movimenti contabili**.
4. Selezionare il movimento contabile rilevante e scegliere l'azione **Scollega movimenti**.
5. In alternativa, scegliere l'azione **Movimenti contabili dettagliati**.
6. Selezionare il movimento di collegamento e scegliere l'azione **Scollega movimenti**.
7. Compilare i campi della testata, quindi scegliere l'azione **Scollega**.

**Importante**: se un movimento è stato collegato da più di un movimento di collegamento, è necessario prima scollegare il movimento di collegamento più recente.

## <a name="see-also"></a>Vedi anche
[Gestire la contabilità clienti](receivables-manage-receivables.md)  
[Gestire le vendite](sales-manage-sales.md)

