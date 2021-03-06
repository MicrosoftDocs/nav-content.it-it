---
title: Acquisire i cespiti
description: "È possibile impostare un cespite, assegnare un registro beni ammortizzabili e registrare il costo di acquisizione del cespite."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: purchase fixed asset
ms.date: 06/02/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 17a61be2cd0977a55b098c8ec0b1d1cc164d7898
ms.contentlocale: it-it
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-acquire-fixed-assets"></a>Procedura: Acquisire i cespiti
Per ogni cespite occorre impostare una scheda che ne riporti le relative informazioni. È possibile impostare edifici o attrezzature di produzione come bene principale con un elenco di componenti ed è possibile raggrupparli in vari modi, ad esempio per classe, reparto o ubicazione. Un registro beni ammortizzabili deve essere impostato e assegnato a ogni cespite prima di poterlo acquisire.

Quando un cespite è impostato e un registro beni ammortizzabili è assegnato, è necessario acquisire il cespite. Per acquisire un cespite, occorre registrare il costo di acquisizione nel relativo conto C/G, conto bancario o fornitore registrando una transazione di acquisizione dalla finestra **Registrazioni cespiti in C/G**. È possibile utilizzare la finestra **Acquisizione assistita cespiti** per creare e registrare le righe registrazioni COGE richieste automaticamente.

Il valore residuo di un cespite quando non può più essere utilizzato. È possibile registrare il valore di realizzo contemporaneamente alla registrazione del costo di acquisto. Per ulteriori informazioni, vedere [Procedura: Ammortamento dei cespiti](fa-how-depreciate-amortize.md).

L'indicizzazione consente di correggere i valori per le modifiche generali a livello di prezzo. Il processo batch **Indice cespiti** consente di calcolare i costi di acquisto ai costi di sostituzione.

## <a name="to-create-a-fixed-asset-and-acquire-it-automatically"></a>Per creare un cespite e acquisirlo automaticamente
Di seguito viene descritto come creare e acquisire un cespite utilizzando la finestra **Acquisizione assistita cespiti** per creare e registrare le righe registrazioni cespiti in C/G richieste. È inoltre possibile creare e registrare manualmente le righe di registrazione. Per ulteriori informazioni, vedere la sezione "Per registrare un'acquisizione di cespite manualmente con Registrazioni cespiti in C/G".

1. Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **Cespiti**, quindi scegliere il collegamento correlato.  
2. Scegliere l'azione **Nuovo** e compilare i campi necessari della Scheda dettaglio **Generale**. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
3. Nella Scheda dettaglio **Registro beni ammortizzabili** compilare i campi secondo le necessità. In questo passaggio viene assegnato un registro beni ammortizzabili al cespite.  
4. Se è necessario assegnare più di un registro beni ammortizzabili al cespite, scegliere l'azione **Aggiungi più registri beni ammortizzabili**. Per ulteriori informazioni, vedere la sezione "Per assegnare un registro beni ammortizzabili a un cespite" in [Procedura: Impostare i registri beni ammortizzabili cespiti](fa-how-setup-depreciation.md).

    Quando tutti i campi necessari per acquisire un cespite vengono compilati, la notifica indicante che **si è pronti ad acquisire il cespite** viene visualizzata nella parte superiore della pagina.
5. Scegliere l'azione **Acquisisci** nella notifica.
6. Seguire i passaggi indicati nella finestra **Acquisizione assistita cespiti** per completare l'acquisizione automatica del cespite.

> [!NOTE]  
>   È inoltre possibile registrare i costi di acquisizione in Avere. In tal caso, ricordare che il valore nel campo **Costo di acquisizione IVA inclusa** deve avere il segno meno per indicare un credito.

Quando si sceglie **Fine**, il campo **Valore contabile** nella finestra **Scheda cespite** viene compilato per indicare che il cespite è stato acquisito al costo di acquisizione specificato.  

## <a name="to-set-up-a-component-list-for-a-main-asset"></a>Per impostare una lista di componenti per un bene principale
I cespiti possono essere raggruppati in beni principali e componenti. Un esempio è costituito da un macchinario di produzione composto da molte parti che si intendono raggruppare come segue.  

il bene principale e tutti i suoi componenti devono essere impostati come schede cespiti individuali. In seguito all'impostazione di una lista componenti, i campi **Bene Principale/Componente** e **Componenti di bene principale** nelle schede cespiti vengono compilati automaticamente da [!INCLUDE[d365fin](includes/d365fin_md.md)].

1. Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **Cespiti**, quindi scegliere il collegamento correlato.
2. Selezionare il cespite che costituisce il bene principale, quindi scegliere l'azione **Componenti bene principale**.
3. Nella finestra **Componenti bene principale** scegliere il campo **Nr. cespite**, quindi selezionare il cespite che si desidera aggiungere come componente del bene principale.
4. Chiudere la finestra.
5. Ripetere i passaggi 3 e 4 per ogni bene componente che si intende aggiungere.
6. Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **Setup cespiti**, quindi scegliere il collegamento correlato.
7. Selezionare la casella di controllo **Autorizza reg. in cespiti principali**.

## <a name="to-post-a-fixed-asset-acquisition-manually-with-the-fixed-asset-gl-journal"></a>Per registrare manualmente un'acquisizione del cespite mediante Registrazioni cespiti in C/G
Di seguito viene descritto come acquistare manualmente un cespite creando e registrando le righe nella finestra **Reg. cespiti in G/L**. È inoltre possibile acquisire automaticamente un cespite utilizzando la finestra **Acquisizione assistita cespiti**. Per ulteriori informazioni, vedere il passaggio 5 nella sezione "Per creare un cespite e acquisirlo automaticamente".

> [!NOTE]  
>   È inoltre possibile registrare i costi di acquisizione in Avere. In tal caso, ricordare che il valore nel campo **Importo** deve avere il segno meno per indicare un credito.

1. Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **Registrazioni cespiti in C/G**, quindi scegliere il collegamento correlato.
2. Nella finestra **Registrazioni cespiti in C/G**, nel campo **Tipo reg. cespite** selezionare **Costo di acquisto**.
3. Compilare i rimanenti campi, se necessario.
4. Scegliere l'azione **Registra**.  

> [!TIP]  
>   Se durante la registrazione di un costo di acquisto viene compilato il campo **Nr. Assicurazione**, il costo di acquisizione del cespite verrà registrato automaticamente da [!INCLUDE[d365fin](includes/d365fin_md.md)] nel registro di copertura assicurativa. Per ulteriori informazioni, vedere [Procedura: Assicurazione di cespiti](fa-how-insure.md).

## <a name="to-cancel-an-acquisition-cost-posting-for-one-fixed-asset"></a>Per annullare una registrazione di costo di acquisto per un cespite
In caso di errore nella registrazione di un costo di acquisto, è possibile rimuovere il movimento con il processo batch **Rimuovi mov. cespiti** e registrare il movimento di acquisto corretto. I movimenti errati vengono trasferiti alla finestra **Mov. cont. cespiti errati**.

Ad esempio, se si registra un acquisto con la data errata, è necessario correggerla prontamente perché la data di registrazione del cespite viene utilizzata in diversi calcoli critici.

> [!IMPORTANT]  
>   Non è possibile utilizzare la funzione **Storno** per i movimenti di cespiti.

1. Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **Rimuovi mov. cespiti**, quindi scegliere il collegamento correlato.
2. Compilare i campi, se necessario. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
3. Scegliere **OK** per eseguire il processo batch.
4. Quando il movimento o i movimenti errati vengono annullati, continuare con la registrazione del costo di acquisto corretto.

Per annullare i movimenti contabili per più cespiti alla volta, utilizzare il processo batch **Annulla mov. contabili cespiti**.

## <a name="to-post-the-salvage-value-together-with-the-acquisition-cost"></a>Per registrare il valore di realizzo con il costo di acquisto
È possibile registrare il valore di realizzo insieme al costo di acquisto da Registrazioni Cespiti in C/G.    

1. Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **Rimuovi mov. cespiti**, quindi scegliere il collegamento correlato.
2. Creare la riga di registrazione acquisizione. Per ulteriori informazioni, vedere la sezione "Per registrare un'acquisizione di cespite manualmente con Registrazioni cespiti in C/G".
3. Immettere l'importo del valore di realizzo come avere (con il segno meno) nel campo **Valore di realizzo** nella riga di registrazione.
4. Scegliere l'azione **Registra**.

> [!NOTE]  
>   Il tipo di registrazione **Valore di realizzo** è un'opzione solo della finestra **Registrazioni cespiti**. Non è disponibile nella finestra **Registrazioni cespiti in C/G** perché il valore di realizzo non è mai registrato nella contabilità generale.

## <a name="see-also"></a>Vedi anche
[Cespiti](fa-manage.md)  
[Impostazione di cespiti](fa-setup.md)  
[Finanze](finance.md)  
[Benvenuto in [!INCLUDE[d365fin_long](includes/d365fin_long_md.md)]](index.md)  
[Utilizzo di [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

