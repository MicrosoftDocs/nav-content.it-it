---
title: 'Procedura: Impostare gli interessi di mora'
description: "Per ciascuna condizione di addebito degli interessi, è possibile specificare come gli interessi di mora devono essere calcolati. È possibile impostare i calcoli di addebito degli interessi con diversi tassi di interesse per diversi periodi."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: b9b1f062ee6009f34698ea2cf33bc25bdd5b11e4
ms.openlocfilehash: 1cd4451c384e5d7dbdb74156b51c276dfd17508b
ms.contentlocale: it-it
ms.lasthandoff: 10/23/2017

---
# <a name="how-to-set-up-interest-on-arrears"></a>Procedura: Impostare gli interessi di mora
Per ciascuna condizione di addebito degli interessi, è possibile specificare come gli interessi di mora devono essere calcolati. È possibile impostare i calcoli di addebito degli interessi con diversi tassi di interesse per diversi periodi.  

Quando si collega una condizione di addebito degli interessi con gli interessi di mora a un cliente o a un fornitore, gli interessi di mora vengono calcolati. Quindi, è possibile eseguire il report Calcolo interessi di mora per visualizzare i dettagli degli interessi di mora per clienti o fornitori.  

Una volta eseguito il report, se un cliente deve gli interessi di mora, le informazioni sulla quantità degli interessi di mora da pagare vengono aggiunte al rendiconto cliente.  

## <a name="to-set-up-interest-on-arrears"></a>Per impostare gli interessi di mora  

1.  Scegliere l'icona ![Cerca pagina o report](../../media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **Condiz. interessi finanziari**, quindi scegliere il collegamento correlato.  
2.  Nella finestra **Condiz. interessi finanziari**, selezionare il movimento richiesto della condizione di addebito degli interessi, quindi scegliere l'azione **Int. di mora**.  
3.  Nella finestra **Interessi di mora**, scegliere l'azione **Nuovo**.  
4.  Compilare i campi come indicato nella tabella seguente.  

    |Campo|Description|  
    |---------------------------------|---------------------------------------|  
    |**Data Inizio**|Specificare la data a partire dalla quale si desidera calcolare gli interessi di mora. **Importante:** La data di inizio per la prima transazione degli interessi non può essere successiva alla data di registrazione più recente delle transazioni finanziarie.|  
    |**Tasso di interesse**|Specificare il tasso di interesse che deve essere calcolato per la mora.|  
    |**Description**|Specificare la descrizione per gli interessi di mora.|  

5.  Scegliere il pulsante **OK**.  

Di seguito viene descritto come collegare gli interessi mora a un cliente, ma gli stessi passaggi si applicano anche per gli interessi di mora di un fornitore.  

## <a name="to-apply-interest-on-arrears-to-a-customer"></a>Per collegare gli interessi di mora a un cliente  

1.  Scegliere l'icona ![Cerca pagina o report](../../media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **Clienti**, quindi scegliere il collegamento correlato.  
2.  Selezionare il cliente a cui devono essere applicati gli interessi di mora e scegliere l'azione **Modifica**.  
3.  Nella Scheda dettaglio **Pagamenti**, nel campo **Codice int. di mora**, selezionare la condizione di addebito degli interessi appropriata che include gli interessi di mora.  
4.  Scegliere il pulsante **OK**.  

## <a name="see-also"></a>Vedi anche  
 [Panoramica degli interessi di mora](interest-on-arrears-overview.md)   

