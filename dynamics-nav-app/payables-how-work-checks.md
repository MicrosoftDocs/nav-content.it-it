---
title: 'Procedura: Utilizzo degli assegni'
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
ms.openlocfilehash: 421516a7580a90d6eabc8ecfcc841215839994c9
ms.contentlocale: it-it
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-work-with-checks"></a>Procedura: Utilizzo degli assegni
Dynamics NAV supporta l'emissione elettronica e manuale di assegni. In entrambi i metodi vengono utilizzate le registrazioni pagamenti per emettere assegni ai fornitori. È inoltre possibile annullare assegni e visualizzare movimenti contabili assegni.

Il processo di emissione degli assegni comporta il suggerimento di pagamenti, la creazione di movimenti contabili e la stampa di assegni automatici.

La stampante deve essere configurata per i moduli di assegni e deve essere definito il layout dell'assegno da utilizzare. Per ulteriori informazioni, vedere [Procedura: Definire i layout degli assegni](finance-setup-how-define-check-layouts.md)

## <a name="to-issue-checks"></a>Per emettere assegni
1. Nell'angolo superiore destro, scegliere l'icona **Cerca pagina o report**, immettere **Registrazioni pagamenti**, quindi scegliere il collegamento correlato.
2. Compilare le registrazioni con pagamenti rilevanti, ad esempio utilizzando la funzione Sugg. pagamenti fornitore. Per ulteriori informazioni, vedere [Procedura: Suggerire i pagamenti ai fornitori](payables-how-suggest-vendor-payments.md).
3. Nel campo **Tipo pagamento banca** nelle righe di registrazione per il pagamento che si desidera effettuare con assegni, selezionare una delle seguenti opzioni:

 - **Assegno automatico**: selezionare questa opzione per stampare un assegno relativo all'importo specificato nella riga di registrazione pagamenti. È necessario stampare gli assegni prima di poter registrare le righe di registrazione. È possibile selezionare **Assegno automatico** solo se il campo **Tipo contropartita** o il campo **Tipo conto** è impostato su **Conto bancario**.

 - **Assegno manuale**: selezionare questa opzione se è stato creato un assegno manualmente e si desidera creare un corrispondente movimento contabile per questo importo. Non è possibile stampare assegni tramite questa opzione da Dynamics NAV. È possibile selezionare **Assegno manuale** solo se il campo **Tipo contropartita** o il campo **Tipo conto** è impostato su **Conto bancario**.

    **Nota**: è necessario stampare gli assegni automatici prima di poter registrare le righe di registrazione correlate.
4. In caso di assegni automatici, scegliere **Stampa assegno**.
5. Nella finestra **Assegno** compilare i campi secondo le proprie necessità. Selezionare il campo per visualizzare una breve descrizione del campo o il collegamento a ulteriori informazioni.
6. Selezionare il pulsante **Stampa**.

**Nota**: se è necessario stampare automaticamente gli assegni provenienti da vari conti correnti bancari utilizzando più di una valuta, eseguire un singolo processo batch **Stampa assegno** per ogni valuta, specificando il conto corrente bancario appropriato.

## <a name="to-cancel-printed-checks-that-are-not-posted"></a>Per annullare assegni stampati che non sono registrati
È possibile annullare gli assegni non registrati dopo che sono stati stampati utilizzando l'azione **Annullo assegno** della finestra **Registrazioni pagamenti**.
1. Nella finestra **Registrazioni pagamenti** scegliere **Annullo assegno**, quindi scegliere gli assegni da annullare.

## <a name="to-void-checks"></a>Per annullare gli assegni
Una volta che i pagamenti tramite assegno sono stati registrati, è possibile annullare gli assegni dai movimenti contabili bancari risultanti.

1. Nell'angolo superiore destro, scegliere l'icona **Cerca pagina o report**, immettere **C/C bancari**, quindi scegliere il collegamento correlato.
2. Selezionare il conto corrente bancario appropriato, scegliere l'azione **Modifica**, quindi scegliere l'azione **Mov. contabili assegni**.
3. Nella finestra **Mov. contabili assegni** scegliere l'azione **Annullo assegno**.
4. Selezionare la casella di controllo **Annullo solo assegno**.
5. Scegliere **OK**.

## <a name="see-also"></a>Vedi anche
[Gestire la contabilità fornitori](payables-manage-payables.md)  
[Impostare le attività bancarie](bank-setup-banking.md)  
