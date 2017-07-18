---
title: 'Procedura: Utilizzare le chiavi di allocazione nelle registrazioni COGE'
author: edupont04
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: d239ab62c4be88ccc4a2ce2669dcc2c20a3c0126
ms.contentlocale: it-it
ms.lasthandoff: 06/26/2017

---

#  <a name="how-to-use-allocation-keys-in-general-journals"></a>Procedura: Utilizzare le chiavi di allocazione nelle registrazioni COGE
È possibile assegnare un movimento in una registrazione generale a più conti diversi, quando tale registrazione viene contabilizzata. L'allocazione può essere effettuata per quantità, percentuale o importo.

## <a name="to-set-up-allocation-keys"></a>Per impostare le chiavi di allocazione 
1. Nell'angolo superiore destro, scegliere l'icona **Cerca pagina o report**, immettere **Reg. periodiche generali**, quindi scegliere il collegamento correlato.
2. Scegliere il campo **Nome batch** per aprire la finestra **Batch registrazioni COGE**.
3. È possibile modificare le allocazioni in un batch esistente nell'elenco o creare un nuovo batch con le allocazioni.
  * Per creare un nuovo batch, scegliere l'azione **Nuovo** e andare al passaggio successivo.
  * Per modificare le allocazioni di registrazioni esistenti, selezionare le registrazioni e andare al passaggio 7.    
4. Nel campo **Nome** immettere un nome per il batch, ad esempio PULIZIE. Nel campo **Descrizione** immettere una descrizione, ad esempio Registrazioni spese pulizie.
5. Al termine, chiudere la finestra. Verrà visualizzata una nuova registrazione periodica vuota. 
6. Compilare i campi nella riga.
7. Scegliere l'azione **Allocazioni**. 
8. Aggiungere una riga per ciascuna allocazione. È necessario compilare il campo **Allocazione %**, **Quantità allocazione** o **Importo**. È inoltre necessario compilare il campo **Nr. conto** e, se si sta allocando la transazione tra dimensioni globali, anche i campi delle dimensioni globali.
9. Se in una riga è stata immessa una percentuale, il valore del campo **Importo** viene calcolato automaticamente. Questi importi hanno il segno opposto rispetto all'importo totale nel campo **Importo** delle registrazioni periodiche.
10. Dopo aver immesso le righe di allocazione, scegliere **OK** per tornare alla finestra **Reg. periodiche generali**. Il campo **Importo allocato (VL)** viene compilato e corrisponde al campo **Importo**.
11. Effettuare la registrazione.

## <a name="to-change-an-allocation-key-that-has-already-been-set-up"></a>Per modificare una chiave di allocazione già impostata
1. Nell'angolo superiore destro, scegliere l'icona **Cerca pagina o report**, immettere **Reg. periodiche generali**, quindi scegliere il collegamento correlato.
2. Nella finestra **Registrazioni periodiche generali** selezionare le registrazioni con l'allocazione.
3. Selezionare la riga con l'allocazione e scegliere l'azione **Allocazioni**.
4. Modificare i campi pertinenti e chiudere la finestra.

## <a name="see-also"></a>Vedi anche
[Utilizzo delle registrazioni COGE](ui-work-general-journals.md)  
[Contabilizzare documenti e registrazioni](ui-post-documents-journals.md)




