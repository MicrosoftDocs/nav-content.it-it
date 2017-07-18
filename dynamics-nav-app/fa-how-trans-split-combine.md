---
title: 'Procedura: Trasferimento, divisione o raggruppamento dei cespiti'
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
ms.openlocfilehash: 96bea0054d2ea3cdabfa179d8f4c78cf90d7777c
ms.contentlocale: it-it
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-transfer-split-or-combine-fixed-assets"></a>Procedura: Trasferimento, divisione o raggruppamento dei cespiti
Utilizzare le registrazioni di riclassificazione cespiti per trasferire, suddividere e raggruppare i cespiti. Visualizzare o stampare i risultati della riclassificazione cespiti con il report **Cespiti - Valore contabile 02**.

## <a name="to-transfer-a-fixed-asset-to-a-different-department"></a>Per trasferire un cespite in un reparto diverso  
Il trasferimento dei cespiti in ubicazioni diverse può essere utilizzato, ad esempio, quando si assegna un cespite al reparto produzione mentre è in costruzione e al termine della costruzione viene spostato nel reparto amministrativo.  

1. Impostare un nuovo cespite. Immettere il nuovo reparto nel campo **Cod. Reparto**.
2. Assegnare un registro beni ammortizzabili al nuovo cespite. Per ulteriori informazioni, vedere [Procedura: Acquisire i cespiti](fa-how-acquire.md).
3. Nell'angolo superiore destro, scegliere l'icona **Cerca pagina o report**, immettere **Registrazioni riclass. cespiti**, quindi scegliere il collegamento correlato.
4. Creare una registrazione di riclassificazione in cui il campo **Nr. cespite** contiene il cespite originale e il campo **Nuovo nr. cespite** contiene il nuovo cespite da spostare.  
5. Scegliere l'azione **Riclassifica**.

    Vengono create due righe in Registrazioni C/G cespiti utilizzando la definizione ed il batch specificati nella finestra **Setup Reg. Cespiti** per il registro beni ammortizzabili indicato. Per ulteriori informazioni, vedere [Procedura: Impostare l'ammortamento cespiti](fa-how-setup-depreciation.md).
6. Nell'angolo superiore destro, scegliere l'icona **Cerca pagina o report**, immettere **Registrazioni cespiti in C/G**, quindi scegliere il collegamento correlato.    
7. Nella finestra **Registrazioni cespiti in C/G**, scegliere l'azione **Registra** per registrare la riclassificazione eseguita ai passaggi 4 e 5.

Se per un cespite è stato registrato un costo d'acquisto, è possibile utilizzare le registrazioni di riclassificazione cespiti per suddividere i costi di acquisto in diversi cespiti.  

## <a name="to-split-a-fixed-asset-into-three-fixed-assets"></a>Per dividere un cespite in tre cespiti
È possibile dividere un unico cespite in più cespiti, ad esempio quando è necessario distribuire un cespite in tre diversi reparti. In tal caso, è possibile spostare ad esempio il 25 percento del costo di acquisto e dell'ammortamento del cespite originale al secondo cespite ed il 45 percento al terzo cespite. Il rimanente 30 percento resterà al cespite originale.

1. Impostare due nuovi cespiti. Immettere il nuovo reparto nel campo **Cod. Reparto**.
2. Assegnare i registri beni ammortizzabili ai nuovi cespiti. Per ulteriori informazioni, vedere [Procedura: Acquisire i cespiti](fa-how-acquire.md).
3. Nell'angolo superiore destro, scegliere l'icona **Cerca pagina o report**, immettere **Registrazioni riclass. cespiti**, quindi scegliere il collegamento correlato.
4. Creare due righe di registrazione riclassificazione, una per ogni nuovo cespite.
5. Nella prima riga, immettere il secondo cespite nel campo **Nuovo nr. cespite** e 25 nel campo **Riclassifica costi di acq. %**.
6. Nella seconda riga, immettere il terzo cespite nel campo **Nuovo nr. cespite** e 40 nel campo **Riclassifica costi di acq. %**.
7. In entrambe le righe, selezionare le caselle di controllo **Riclassifica costi di acq.** e **Riclassifica ammortamento**.   
8. Scegliere l'azione **Riclassifica**.

    Vengono create due righe in Registrazioni C/G cespiti utilizzando la definizione ed il batch specificati nella finestra **Setup Reg. Cespiti** per il registro beni ammortizzabili indicato. Per ulteriori informazioni, vedere [Procedura: Impostare l'ammortamento cespiti](fa-how-setup-depreciation.md).    
9. Nell'angolo superiore destro, scegliere l'icona **Cerca pagina o report**, immettere **Registrazioni cespiti in C/G**, quindi scegliere il collegamento correlato.
10. Nella finestra **Registrazioni cespiti in C/G**, scegliere l'azione **Registra** per registrare la riclassificazione eseguita ai passaggi da 4 a 8.

## <a name="to-combine-two-fixed-assets-into-one"></a>Per raggruppare due cespiti in uno
È possibile raggruppare più cespiti in un unico cespite, ad esempio quando si spostano i cespiti distribuiti in un unico reparto. Se sono stati registrati i costi di acquisto e l'ammortamento del cespite da spostare, i valori verranno raggruppati singolo cespite.

1. Nell'angolo superiore destro, scegliere l'icona **Cerca pagina o report**, immettere **Registrazioni riclass. cespiti**, quindi scegliere il collegamento correlato.
2. Creare una registrazione di riclassificazione in cui il campo **Nr. cespite** contiene il cespite originale da spostare/raggruppare e il campo **Nuovo nr. cespite** contiene il cespite in cui verrà raggruppato.
3. Lasciare vuoti il campo **Riclassifica costi di acq. %** per sposare/raggruppare l'intero costo di acquisto.    
4. Selezionare le caselle di controllo **Riclassifica costi di acq.** e **Riclassifica ammortamento**.
5. Nella scheda **Azioni** selezionare **Riclassifica**.

    Vengono create due righe in Registrazioni C/G cespiti utilizzando la definizione ed il batch specificati nella finestra **Setup Reg. Cespiti** per il registro beni ammortizzabili indicato. Per ulteriori informazioni, vedere [Procedura: Impostare l'ammortamento cespiti](fa-how-setup-depreciation.md).   
6. Nell'angolo superiore destro, scegliere l'icona **Cerca pagina o report**, immettere **Registrazioni cespiti in C/G**, quindi scegliere il collegamento correlato.
7. Nella finestra **Registrazioni cespiti in C/G**, scegliere l'azione **Registra** per registrare la riclassificazione eseguita ai passaggi da 2 a 5.

## <a name="to-view-changed-depreciation-book-values-due-to-fixed-asset-reclassification"></a>Per visualizzare i valori del registro beni ammortizzabili modificati a causa dalla riclassificazione dei cespiti  
1. Nell'angolo superiore destro, scegliere l'icona **Cerca pagina o report**, immettere **Valore contabile cespiti 02**, quindi scegliere il collegamento correlato.
2. Compilare i campi, se necessario.
3. Selezionare il pulsante **Stampa** o **Anteprima**.  

## <a name="see-also"></a>Vedi anche
[Gestione di cespiti](fa-manage.md)  
[Impostazione cespiti](fa-setup.md)  
[Contabilità](finance-setup.md)  
[Benvenuto in Dynamics NAV](across-get-started.md)

