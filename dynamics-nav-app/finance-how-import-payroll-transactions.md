---
title: 'Procedura: Importare transazioni retributive '
author: SorenGP
ms.custom: na
ms.date: 09/29/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: d5e70a0a1659c7facdeec3f0971eda43ff8a03cc
ms.contentlocale: it-it
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-import-payroll-transactions"></a>Procedura: Importare transazioni retributive 
Per indicare i pagamenti di stipendio e le transazioni correlate, è necessario importare e registrare in contabilità generale le transazioni finanziarie trasformate dal provider di retribuzioni. A tale scopo, è necessario innanzitutto importare un file csv che si riceve dal provider di retribuzioni nella finestra **Contabilità generale**. Successivamente si esegue il mapping tra i conti esterni nel file retribuzioni e i conti C/G pertinenti. Infine, si registrano le transazioni retribuzioni in base alla mappatura dei conti.

## <a name="to-import-a-payroll-file"></a>Per importare un file delle retribuzioni
1. Nell'angolo superiore destro, scegliere l'icona **Cerca pagina o report**, immettere **Registrazioni COGE**, quindi scegliere il collegamento correlato.
2. Nel batch registrazioni COGE appropriato scegliere l'azione **Importa transazioni retribuzioni**.
3. Nella finestra **Importa** selezionare il file retribuzioni interessato, quindi scegliere **OK**. Il file deve essere in formato CSV. 
4. Seguire i passaggi indicati nella finestra **Importa transazioni retribuzioni** per importare le transazioni e mappare i conti, quindi scegliere il pulsante **Fine**.

    Le registrazioni COGE vengono completate con le righe che rappresentano le transazioni contenute nel file retribuzioni e con i relativi conti nella colonna **Conto C/G**.
4. Modificare o registrare le righe delle registrazioni relative a tutte le altre le transazioni della contabilità generale. Per ulteriori informazioni, vedere [Procedura: Elaborazione delle registrazioni COGE](ui-work-general-journals.md).   

## <a name="see-also"></a>Vedi anche
[Contabilità](finance-setup.md)  
[Procedura: Utilizzare le registrazioni di contabilità generale](ui-work-general-journals.md)  

