---
title: 'Procedura: Aggiornare i dati delle transazioni IVA'
description: "Prima di creare il primo report transazioni IVA, è necessario preparare i dati esistenti eseguendo il report **Aggiorna data transazione IVA**."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: b9b1f062ee6009f34698ea2cf33bc25bdd5b11e4
ms.openlocfilehash: c33a2e91a1780e5941faf104f04e9b70cf8a330f
ms.contentlocale: it-it
ms.lasthandoff: 10/23/2017

---
# <a name="how-to-update-vat-transactions-data"></a>Procedura: Aggiornare i dati delle transazioni IVA
Prima di creare il primo report transazioni IVA, è necessario preparare i dati esistenti eseguendo il report **Aggiorna data transazione IVA**. È inoltre necessario eseguire questo report se sono state apportate modifiche al setup in base ai nuovi requisiti delle autorità fiscali.  

È possibile eseguire il report **Aggiorna data transazione IVA** come test prima di modificare i dati. Dopo avere verificato che i filtri soddisfano le previsioni e le richieste delle autorità fiscali, eseguire nuovamente il report per apportare le modifiche appropriate ai dati.  

> [!CAUTION]  
>  Prima di eseguire il report **Aggiorna data transazione IVA**, è necessario attivare il log delle modifiche nella finestra **Setup log modifiche**. Inoltre, è necessario attivare la registrazione delle modifiche nel campo **Includi in report transazioni IVA** nella tabella **Movimenti IVA**.  

## <a name="to-update-vat-transaction-data"></a>Per aggiornare i dati delle transazioni IVA  

1.  Scegliere l'icona ![Cerca pagina o report](../../media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **Aggiorna data transazione IVA**, quindi scegliere il collegamento correlato.  
2.  Facoltativamente, nella Scheda dettaglio **Movimenti IVA** impostare i filtri appropriati.  
3.  Nella Scheda dettaglio **Opzioni** compilare i campi come descritto nella tabella riportata di seguito.  

    |Campo|Description|  
    |---------------------------------|---------------------------------------|  
    |**Confronta con soglia**|Selezionare per confrontare i movimenti IVA rispetto agli importi di soglia specificati nel setup registrazioni IVA.|  
    |**Mostra solo elenco**|Selezionare se non si desidera aggiornare i dati.<br /><br /> Se si seleziona questo campo, [!INCLUDE[navnow](../../includes/navnow_md.md)] stampa un report in modo da poter verificare le modifiche prima che i dati vengano modificati. Il report contiene una riga per ogni documento in cui l'imponibile IVA sia uguale o maggiore degli importi di soglia. **Avviso:** Non selezionare questo campo e il campo **Imposta Includi in report transazioni IVA**.|  
    |**Imposta Includi in report transazioni IVA**|Selezionare per impostare **Imposta Includi in report transazioni IVA** su **Sì** in tutti i movimenti IVA in cui gli importi soddisfano gli importi di soglia specificati nel setup registrazioni IVA. **Avviso:** Se si seleziona questo campo, i dati vengono aggiornati. È consigliabile eseguire il report come test prima di eseguirlo per modificare i dati.|  

4.  Scegliere il pulsante **Stampa** per aggiornare i dati delle transazioni IVA oppure scegliere il pulsante **Anteprima** per visualizzare le modifiche.  

Quando si esegue il report, [!INCLUDE[navnow](../../includes/navnow_md.md)] elabora i movimenti IVA in base ai filtri impostati. Le seguenti regole sono applicabili:  

- Il campo **In blacklist** per il movimento IVA deve essere vuoto.  
- Il campo **Tipo** del movimento IVA non deve essere **Liquidazione**.  

## <a name="see-also"></a>Vedi anche  
[Impostare l'IVA](../../finance-setup-vat.md)  
 [Procedura: Preparare i report di transazioni IVA](how-to-prepare-for-vat-transactions-reports.md)   
 [IVA italiana](italian-vat.md)   

