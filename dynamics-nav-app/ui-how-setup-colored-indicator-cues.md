---
title: 'Procedura: Impostare un indicatore colorato nelle pile'
author: SusanneWindfeldPedersen
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: 04272431b01c0ab398618d9878b90d73e6324abe
ms.contentlocale: it-it
ms.lasthandoff: 06/26/2017

---
    
# <a name="how-to-set-up-a-colored-indicator-on-cues"></a>Procedura: Impostare un indicatore colorato nelle pile
È possibile impostare delle pile che vengono visualizzate nella pagina **Home** in modo che includano un indicatore che cambia colore in base ai valori dei dati presenti nelle pile. 

L'indicatore viene visualizzato come una barra colorata lungo il bordo superiore della pila. Fornisce un segnale visivo dello stato dell'attività della pila, che può indicare le condizioni favorevoli o sfavorevoli per spingere l'utente a intraprendere un'azione. Ad esempio, se una pila visualizza le fatture di vendita in corso, è possibile impostare l'indicatore in modo che appaia verde (favorevole) quando il totale delle fatture di vendita in corso è minore di 10 e rosso (sfavorevole) quando il totale è maggiore di 20.

Nella finestra **Setup pila**, si impostano gli indicatori di tutte le pile disponibili nel database della società.

Per impostare l'indicatore, specificare fino a due valori di soglia che definiscono tre intervalli dei valori dei dati (basso, medio e alto) e a cui è possibile applicare un colore diverso (o stile).

## <a name="to-set-up-colored-indicators-on-cues"></a>Per impostare indicatori colorati nelle pile
1. In **Attività**, nella pagina **Home**, scegliere **Imposta pile**.  
Verrà visualizzata la finestra **Setup pila**. Nella finestra sono elencati gli indicatori attualmente impostati nelle pile.
2. Per modificare un indicatore, modificare i campi e modificare, ad esempio, i valori per le diverse soglie.  

Nella tabella seguente sono elencati i colori corrispondenti alle opzioni dei campi **Stile intervallo inferiore**, **Stile intervallo medio** e **Stile intervallo superiore**.

|Opzione|Colore|
|------|-----|
|**Nessuno**|Nessun colore (lo stesso colore della sezione Pila|
|**Favorevole**|Verde|
|**Sfavorevole**|Rosso|
|**Ambiguo**|Giallo|
|**Subordinato**|Grigio|

## <a name="see-also"></a>Vedi anche
[Utilizzare Dynamics NAV](ui-work-product.md)

