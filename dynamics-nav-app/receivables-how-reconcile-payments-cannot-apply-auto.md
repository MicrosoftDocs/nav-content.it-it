---
title: 'Procedura: Riconciliare i pagamenti che non possono essere collegati automaticamente'
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
ms.openlocfilehash: f9fd7c2958aaa359d2f6af5dde2e8be81349e900
ms.contentlocale: it-it
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-reconcile-payments-that-cannot-be-applied-automatically"></a>Procedura: Riconciliare i pagamenti che non possono essere collegati automaticamente
Talvolta può essere necessario gestire i pagamenti al conto corrente bancario che non possono essere collegati a un movimento aperto di contabilità generale, cliente o fornitore correlato. I motivi possono essere che in Dynamics NAV non sono presenti documenti a cui possa essere collegato il pagamento o che il documento correlato in Dynamics NAV ha un importo diverso da quello della transazione, ad esempio, a causa del cambio della valuta. Nella finestra **Registrazione riconciliazione pagamenti** tutti gli importi delle transazioni per i pagamenti che non sono ancora collegati vengono visualizzati nel campo **Differenza**, inclusi gli importi che non possono essere collegati per i motivi citati prima.

I pagamenti che non possono essere collegati possono essere visualizzati nelle righe di registrazione riconciliazione pagamenti nei seguenti modi:

- Il valore nel campo **Differenza** è uguale al valore del campo **Importo transazioni**, pertanto nessuna parte del pagamento può essere collegata a un movimento contabile del conto corrente bancario, fornitore o cliente aperto.

- Il valore nel campo **Differenza** è inferiore al valore del campo **Importo transazioni**, pertanto una parte del pagamento può essere collegata a un movimento contabile del conto corrente bancario, fornitore o cliente aperto. La parte residua del pagamento non può essere collegata e deve essere riconciliata manualmente o registrandola direttamente in un conto.

Per riconciliare questi pagamenti, scegliere il pulsante Trasferisci differenza a conto quindi specificare su quale conto registrare l'importo del campo Differenza quando si effettua la registrazione riconciliazione pagamenti.

**Nota**: tale funzionalità consente di impostare la riconciliazione automatica dei pagamenti ricorrenti che non possono essere collegati ai relativi movimenti contabili del conto corrente bancario, fornitore o cliente aperti. Per ulteriori informazioni, vedere [Procedura: Mappare il testo nei pagamenti ricorrenti a conti per la riconciliazione automatica](receivables-how-map-text-recurring-payments-accounts-auto-reconcilliation.md).

## <a name="to-reconcile-payments-that-cannot-be-applied"></a>Per riconciliare i pagamenti che non possono essere collegati
1. Nell'angolo superiore destro, scegliere l'icona **Cerca pagina o report**, immettere **Registrazioni riconciliazione pagamenti**, quindi scegliere il collegamento correlato.
2. Aprire una registrazione della riconciliazione di pagamento. Per ulteriori informazioni, vedere [Procedura: Riconciliare i pagamenti utilizzando il collegamento automatico](receivables-how-reconcile-payments-auto-application.md).
3. Scegliere **Trasferisci differenza a conto**. Verrà visualizzata la finestra **Trasferisci differenza a conto** 3 .
4. Nel campo **Tipo conto** specificare il tipo di conto in cui sarà registrato l'importo di pagamento.
5. Nel campo **Nr. conto** specificare il conto in cui sarà registrato l'importo di pagamento.
6. Nel campo **Descrizione** specificare il testo che descrive questa registrazione di pagamento diretto. Per impostazione predefinita, viene inserito il testo nel campo **Testo transazione** nella riga di registrazione riconciliazione pagamenti.
7. Scegliere il pulsante **OK**.

Se il valore nel campo **Differenza** è uguale al valore del campo **Importo transazioni** quando si registra la riconciliazione pagamenti, l'intero pagamento nella riga di registrazione sarà registrato direttamente nel conto di contropartita specificato.

Se il valore nel campo **Differenza** è inferiore al valore del campo **Importo transazioni**, verrà creata una nuova riga di registrazione aggiuntiva con lo stesso testo e la stessa data e con la differenza inserita nel campo **Importo transazioni**. Nella riga di registrazione originale, la differenza verrà dedotta dal valore nel campo **Importo transazioni** e il pagamento rimarrà collegato al relativo movimento contabile del conto corrente bancario, fornitore o cliente. Quando si contabilizza la registrazione riconciliazione pagamenti, una parte del pagamento verrà registrata come pagamento collegato. L'altra parte del pagamento verrà registrata direttamente nel conto specificato.

## <a name="see-also"></a>Vedi anche
[Gestire la contabilità clienti](receivables-manage-receivables.md)  
[Gestire le vendite](sales-manage-sales.md)

