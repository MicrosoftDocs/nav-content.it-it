---
title: "Procedura: Attribuire un ordine di priorità ai fornitori"
author: SorenGP
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: 3b89bf07e1e9d1839b6c86a01111e936fb62c9f3
ms.contentlocale: it-it
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-prioritize-vendors"></a>Procedura: Attribuire un ordine di priorità ai fornitori
Dynamics NAV può fornire suggerimenti di pagamento ai fornitori, ad esempio pagamenti con scadenza a breve termine oppure pagamenti che prevedono uno sconto. Per ulteriori informazioni, vedere [Procedura: Suggerire pagamenti fornitore](payables-how-suggest-vendor-payments.md).

Innanzitutto, è necessario assegnare una priorità ai fornitori assegnando loro dei numeri.

## <a name="to-prioritize-vendors"></a>Per attribuire un ordine di priorità ai fornitori
1. Nell'angolo superiore destro, scegliere l'icona **Cerca pagina o report**, immettere **Fornitori**, quindi scegliere il collegamento correlato.
2. Selezionare il fornitore appropriato e scegliere **Modifica**.
3. Nel campo **Priorità** immettere un numero.

In Dynamics NAV il numero più basso, escluso lo 0, ha la massima priorità. Così, ad esempio, se si usano 1, 2 e 3, 1 avrà la massima priorità.

Se non si desidera dare la priorità a un fornitore, lasciare vuoto il campo **Priorità**. Quindi, se si usa la funzione di suggerimento di pagamento, il fornitore si troverà dopo tutti i fornitori che hanno un numero di priorità. Si possono immettere tutti i livelli di priorità necessari.

## <a name="see-also"></a>Vedi anche
[Impostare gli acquisti](purchasing-setup-purchasing.md)  
[Gestire la contabilità fornitori](payables-manage-payables.md)

