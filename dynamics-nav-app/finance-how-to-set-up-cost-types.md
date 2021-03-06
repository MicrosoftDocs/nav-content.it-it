---
title: Come impostare un piano dei tipi di costo
description: "Il piano dei tipi di costo è simile al piano dei conti nella contabilità generale."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: cost types, general ledger, accounts
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 104b057639090bd9797f06ebcc6b573899b9f87c
ms.contentlocale: it-it
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-set-up-cost-types"></a>Procedura: Impostare i tipi di costo
Il piano dei tipi di costo è simile al piano dei conti nella contabilità generale. È possibile impostare il piano dei tipi di costo nelle modalità seguenti:  

-   Strutturare il piano dei tipi di costo in modo analogo ai conti economici del piano dei conti della contabilità generale. Successivamente, il piano dei conti della contabilità generale può essere trasferito al piano dei tipi di costo. È possibile apportare tutte le rettifiche necessarie dopo il trasferimento.  
-   Creare un nuovo piano dei tipi di costo o aggiungere nuovi tipi di costo al piano dei tipi di costo esistente. È necessario creare ogni nuovo tipo di costo singolarmente.  

## <a name="to-transfer-the-general-ledger-chart-of-accounts-to-the-chart-of-cost-types"></a>Per trasferire il piano dei conti della contabilità generale al piano dei tipi di costo  
1.  Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **Piano dei tipi di costo**, quindi scegliere il collegamento correlato.  
2.  Scegliere l'azione **Ottieni tipi costo da piano dei conti**. Nella finestra di dialogo fare clic sul pulsante **Sì** per confermare il trasferimento. La funzione utilizza il piano dei conti per creare un piano dei tipi di costo.  

    Il piano dei tipi di costo contiene ora tutti i conti economici nella contabilità generale e include le testate e i subtotali. È possibile modificare il piano dei tipi di costo, in base alle esigenze. Ad esempio, è possibile eliminare i tipi di costo esistenti duplicati.  

    > [!IMPORTANT]  
    >  Con la funzione **Registra tipi costo in piano dei conti** è possibile aggiornare la relazione tra il piano dei conti e il piano dei tipi di costo. Il campo **Nr.** viene compilato e verificato per garantire che ciascun conto di contabilità generale sia correlato a un solo tipo di costo. La funzione viene eseguita automaticamente prima del trasferimento dei movimenti C/G nella contabilità industriale.  

## <a name="to-set-up-new-cost-types-in-the-chart-of-cost-types-window"></a>Per impostare nuovi tipi di costo nella finestra Piano dei tipi di costo  
1.  Aprire la finestra **Piano dei tipi di costo** in modalità di modifica.  
2.  Compilare i campi in base alle esigenze. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

    > [!NOTE]  
    >  È possibile impostare e gestire tipi di costo nella scheda **Scheda tipo di costo** o nella finestra **Piano dei tipi di costo**. In questa procedura è possibile impostare i tipi di costo nella finestra  **Piano dei tipi di costo**.

3.  Dopo avere creato tutti i tipi di costo, scegliere l'azione **Indentazione tipi costo**. Nella finestra di dialogo scegliere il pulsante **Sì**.  
4.  Collegare il nuovo tipo di costo al corrispondente conto di contabilità generale.  

    > [!IMPORTANT]  
    >  Se le definizioni per i conti sono state immesse nei campi **Totale** del tipo riga **Fine-Totale** prima di eseguire la funzione **Indentazione tipi costo**, sarà necessario inserirle nuovamente in seguito poiché questa funzione sovrascrive i valori in tutti i campi **Fine-Totale**.  

## <a name="to-update-cost-types"></a>Per aggiornare i tipi di costo  
1.  Nella finestra **Setup contabilità industriale** selezionare se si desidera che il piano dei tipi di costo venga aggiornato automaticamente quando il piano dei conti viene modificato.  
2.  Nel campo **Allinea conto C/G** è possibile selezionare una delle seguenti opzioni.  

- **Nessun allineamento**: non esiste alcuna modifica corrispondente nel grafico dei tipi di costo quando si modifica il piano dei conti.  
- **Automatico**: viene apportata una modifica corrispondente nel grafico dei tipi di costo quando si modifica il piano dei conti.  
- **Richiesta**: viene visualizzato un messaggio in cui viene chiesto se apportare una modifica corrispondente nel grafico dei tipi di costo quando si modifica il piano dei conti.  

## <a name="see-also"></a>Vedi anche  
[Contabilizzazione dei costi](finance-manage-cost-accounting.md)  
[Definizione della relazione tra i tipi di costo e i conti di contabilità generale](finance-defining-the-relationship-between-cost-types-and-general-ledger-accounts.md)   
[Definizione dei centri di costo e degli oggetti di costo per il piano dei conti](finance-defining-cost-centers-and-cost-objects-for-chart-of-accounts.md)   
[Saldi tra tipo di costo, centro di costo e oggetto di costo](finance-balances-between-cost-type-cost-center-and-cost-object.md)   
[Impostazione della contabilità industriale](finance-set-up-cost-accounting.md)   
[Terminologia della contabilità industriale](finance-terminology-in-cost-accounting.md)   
[Informazioni sulla contabilità industriale](finance-about-cost-accounting.md)  
[Utilizzo di [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

