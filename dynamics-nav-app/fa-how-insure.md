---
title: Assicurazione di cespiti
Description: "È possibile assegnare un cespite a una polizza assicurativa che è rappresentata da una scheda assicurazione."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: policy, coverage
ms.date: 06/02/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: b4e6733454a56396daa4bbbc817e1bbcde9dec46
ms.contentlocale: it-it
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-insure-fixed-assets"></a>Procedura: Assicurazione di cespiti
La polizza assicurativa di un cespite è rappresentata da una scheda assicurazione. È possibile assegnare un solo cespite a una sola polizza assicurativa o più cespiti a una sola polizza assicurativa.

Assegnare un cespite a una polizza assicurativa registrando nel registro di copertura assicurativa dalla finestra **Registr. assicuraz.**.

Inoltre, è possibile assegnare un cespite ad una polizza assicurativa e creare i movimenti contabili della copertura quando si registra il costo di acquisto. Questa operazione si esegue registrando un costo di acquisto dalla registrazione cespiti con il campo **Nr. assicurazione** compilato. La casella di controllo **Reg. automatica assicurazione** nella finestra **Setup cespiti** deve essere selezionata. Per ulteriori informazioni, vedere la sezione "Per registrare manualmente un'acquisizione del cespite mediante Registrazioni cespiti in C/G" in [Procedura: Acquisire cespiti](fa-how-acquire.md).

Se la casella di controllo **Reg. automatica assicurazione** della finestra **Setup cespiti** non è selezionata, la registrazione delle acquisizioni dalla registrazione cespiti creerà righe nella finestra **Registr. assicuraz.** che devono essere registrate manualmente.

> [!WARNING]  
>   Se non si seleziona la casella di controllo **Reg. automatica assicurazione** nella finestra **Setup cespiti**, la registrazione assicurazioni deve essere basata su una definizione di registrazioni senza numerazione. Questo si verifica perché i numeri di documento inseriti dalla riga di registrazione cespiti saranno in conflitto con la numerazione della registrazione assicurazioni. Per ulteriori informazioni sui batch e sulle definizioni registrazioni, vedere [Procedura: Impostare i valori generali per i cespiti](fa-how-setup-general.md).

Dopo aver assegnato un cespite ad una polizza assicurativa, la casella di controllo **Assicurato** viene selezionata nella scheda cespite. Quando si vende il cespite, la casella di controllo viene deselezionata automaticamente.

## <a name="to-create-or-modify-an-insurance-card"></a>Per creare o modificare una scheda assicurazione
La polizza assicurativa di un cespite deve essere rappresentata da una scheda assicurazione.

In caso di ricezione di informazioni relative a modifiche dell'importo di copertura, immettere le nuove informazioni nella finestra **Scheda assicurazione** per assicurarsi che la copertura della polizza venga analizzata correttamente.  

1. Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **Assicurazione**, quindi scegliere il collegamento correlato.
2. Scegliere l'azione **Nuovo** per creare una nuova scheda per una polizza assicurativa. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
3. In alternativa, selezionare la polizza assicurativa che si desidera modificare, quindi scegliere l'azione **Modifica**.

## <a name="to-assign-a-fixed-asset-to-an-insurance-policy-by-posting-from-the-insurance-journal"></a>Per assegnare un cespite a una polizza assicurativa mediante la registrazione dalla registrazione assicurazioni
Assegnare un cespite a una polizza assicurativa mediante la registrazione al registro della copertura assicurativa.  

La seguente procedura illustra come creare manualmente una riga di registrazione assicurazioni. Se la casella di controllo **Reg. automatica assicurazione** è selezionata nella finestra **Setup cespiti**, le righe di registrazione assicurazioni vengono create automaticamente durante la registrazione dei costi di acquisto. In tal caso, è sufficiente registrare la registrazione.  

1. Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **Registrazioni assicurazioni**, quindi scegliere il collegamento correlato.  
2. Aprire la registrazione pertinente e compilare le righe di registrazione necessarie.  
3. Per assegnare più cespiti a una sola polizza, creare righe di registrazione con lo stesso valore nel campo **Nr. assicurazione** e valori diversi nel campo **Nr. cespite**.  
4. Scegliere l'azione **Registra**.  

    > [!NOTE]  
>   I movimenti delle registrazioni delle assicurazioni vengono registrati soltanto nelle registrazioni della copertura assicurativa.  

## <a name="to-update-the-insurance-value-of-a-fixed-asset"></a>Per aggiornare il valore dell'assicurazione di un cespite
Il processo batch **Indice Cespiti** consente di aggiornare il valore dei cespiti coperti da assicurazione.  

1. Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **Indice assicurazioni**, quindi scegliere il collegamento correlato.
2. Compilare i campi, se necessario.

    > [!NOTE]  
>   Nel campo **Cifra indicizzazione** immettere una riduzione del 5%, ad esempio 95, nel campo laddove si immette un aumento del 2% come 102.  
3. Scegliere il pulsante **OK**.  

   Tramite il processo batch verrà calcolato il nuovo importo come percentuale del valore totale assicurato, come indicato nella finestra **Statistiche Assicurazioni** e verrà creata una riga nelle registrazioni delle assicurazioni.  
4. Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **Registrazioni assicurazioni**, quindi scegliere il collegamento correlato.  
5. Aprire la registrazione assicurazioni appropriata, esaminare i valori creati e registrarli nel registro di copertura assicurativa.  

## <a name="to-monitor-insurance-coverage"></a>Per controllare la copertura assicurativa
[!INCLUDE[d365fin](includes/d365fin_md.md)] fornisce le finestre dedicate per statistiche e report da utilizzare per analizzare le polizze assicurative e controllare se i cespiti sono sovra o sotto assicurati.  

### <a name="overview-of-insurance-policies"></a>Sintesi delle polizze assicurative
Per una sintesi delle polizze assicurative, visualizzare in anteprima o stampare il report **Assicurazione - Lista**. Nel report vengono visualizzate tutte le polizze e i campi più importanti delle schede assicurative.  

### <a name="insurance-coverage"></a>Copertura assicurativa
Per sapere quale polizza assicurativa copre ogni risorsa e per quale importo, è possibile visualizzare in anteprima o stampare il report **Assicurazione - Totale valori assicurati**.  

### <a name="overunder-coverage"></a>Sopra/sottocopertura
È possibile controllare se i cespiti sono sovra o sotto assicurati nei seguenti modi:  

* La finestra **Statistiche assicurazioni**. Un importo positivo nel campo **Sopra/sotto assicurato** indica che il cespite è soprassicurato. Un importo negativo indica invece che è sottoassicurato.  
* La finestra **Statistiche cespiti**. Scegliere il campo **Valore totale assicurato** per visualizzare la finestra **Mov.cont. copert. assicurativa**.  
* Il report **Sopra/sottocopertura**.  
* Il report **Analisi assicurazioni**.  

### <a name="uninsured-fixed-assets"></a>Cespiti non assicurati
Per controllare di non aver dimenticato di assegnare un cespite ad una polizza assicurativa è possibile stampare o visualizzare in anteprima il report **Assicur. - Cespiti non Assic.** In questo report vengono visualizzati i cespiti i cui importi non sono stati registrati nel registro della copertura assicurativa.  

## <a name="to-view-insurance-coverage-ledger-entries"></a>Per visualizzare i movimenti contabili di copertura assicurativa
È possibile visualizzare i movimenti effettuati nel registro copertura assicurativa.  

1. Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **Assicurazione**, quindi scegliere il collegamento correlato.  
2. Selezionare la polizza assicurativa rilevante e scegliere l'azione **Mov.cont. copert. assicurativa**.  

## <a name="to-view-the-total-insurance-value-of-fixed-assets"></a>Per visualizzare il valore totale assicurato dei cespiti
In una finestra della matrice dedicata vengono visualizzati i valori assicurativi registrati per ognuna delle polizze assicurative di ogni cespite come risultato degli importi contabilizzati a fini assicurativi registrati.  

1. Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **Assicurazione**, quindi scegliere il collegamento correlato.  
2. Selezionare la polizza assicurativa rilevante e scegliere l'azione **Val. tot. assicurato per cespite**.  
3. Compilare i campi, se necessario.  
4. Scegliere l'azione **Mostra matrice**.  
5. Per visualizzare i movimenti contabili sottostanti della copertura assicurativa, selezionare un valore nella matrice.  

## <a name="to-correct-insurance-coverage-entries"></a>Per correggere i movimenti di copertura assicurativa
Se un cespite è stato collegato a una polizza assicurativa errata, è possibile correggere creando due movimenti di riclassificazione dalla registrazione assicurazioni.  

1. Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **Registrazioni assicurazioni**, quindi scegliere il collegamento correlato.  
2. Creare una riga di registrazione per il cespite e la polizza assicurativa corretta in cui il valore del campo **Importo** è positivo.  
3. Creare un'altra riga di registrazione per il cespite e la polizza assicurativa non corretta in cui il valore del campo **Importo** è negativo.  
4. Scegliere l'azione **Registra**.  

Il cespite viene scollegato dalla polizza assicurativa errata, sulla seconda riga, e viene allegato a quella corretta, sulla prima riga.  

## <a name="see-also"></a>Vedi anche
[Cespiti](fa-manage.md)  
[Impostazione di cespiti](fa-setup.md)  
[Finanze](finance.md)  
[Utilizzo di [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)  

