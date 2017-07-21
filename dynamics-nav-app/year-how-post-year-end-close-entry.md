---
title: 'Procedura: Registrare il movimento di chiusura di fine anno'
author: jswymer
ms.custom: na
ms.date: 09/16/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: a8fdb459a2b98066bb93bb47cc0bd9721b992d94
ms.contentlocale: it-it
ms.lasthandoff: 06/26/2017

---
# <a name="how-to-post-year-end-closing-entry"></a>Procedura: Registrare il movimento di chiusura di fine anno
Nell'ambito della chiusura dei registri contabili relativi a un anno fiscale verrà eseguito il processo batch Chiudi conto economico per trasferire i risultati dell'anno su un conto dello stato patrimoniale e chiudere i conti economici. Dopo avere eseguito il processo batch Chiudi conto economico, è necessario aprire le registrazioni specificate nel processo batch, quindi analizzare e registrare i movimenti.

## <a name="to-post-the-year-end-closing-entry"></a>Per registrare il movimento di chiusura di fine anno
1. Nell'angolo superiore destro, scegliere l'icona **Cerca pagina o report**, immettere **Registrazioni COGE**, quindi scegliere il collegamento correlato.
2. Nella finestra **Registrazione COGE**, nel campo **Nome batch**, selezionare il batch contenente i movimenti di chiusura.
3. Analizzare i movimenti.
4. Per contabilizzare le registrazioni, scegliere l'azione **Registra**.

**Nota**: se viene rilevato un errore, viene visualizzato un messaggio di errore. Se la registrazione avviene correttamente, i movimenti registrati vengono rimossi dalle registrazioni. Dopo il completamento della registrazione, in ogni conto economico viene registrato un movimento in modo che il relativo saldo sia uguale a zero, e il risultato dell'anno viene trasferito al conto patrimoniale.

## <a name="see-also"></a>Vedi anche
[Chiusura dei libri](year-close-books.md)  
[Chiusura del conto economico](year-close-income-statement.md)  
[Procedura: Chiudere i periodi contabili](year-close-account-periods.md)  
