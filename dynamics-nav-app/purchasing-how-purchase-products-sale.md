---
title: Creare una fattura di acquisto da una fattura di vendita per acquistare gli articoli per una vendita
description: "Da una fattura di vendita, per acquistare prodotti, è possibile creare una fattura di acquisto per un fornitore."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: supply planning, sales demand, replenish
ms.date: 05/16/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: a6380570c9fb2bc5880bf531b4311fbf6e9cf4ec
ms.contentlocale: it-it
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-purchase-items-for-a-sale"></a>Procedura: Acquistare articoli per una vendita
Dagli ordini di vendita e dalle fatture di vendita, è possibile utilizzare funzioni per creare rapidamente i documenti di acquisto relativi alle quantità mancanti di articoli che sono necessari per la vendita. È possibile utilizzare due funzioni diverse che variano a seconda del tipo documento.

|Funzione|Description|
|--------|-----------|
|**Crea ordini di acquisto**|Da un ordine di vendita, questa funzione crea un ordine di acquisto per ciascun fornitore di articoli nell'ordine di vendita. È possibile modificare la quantità di acquisto prima di creare gli ordini di acquisto. Vengono suggerite solo le quantità di vendita non disponibili.
|**Crea fattura di acquisto**|Da un ordine di vendita e da una fattura di vendita, questa funzione crea una fattura di acquisto per un fornitore selezionato per tutte le righe o per le righe selezionate nel documento di vendita. Viene suggerita la quantità di vendita completa.|

## <a name="to-create-one-or-more-purchase-orders-from-a-sales-order"></a>Per creare uno o più ordini di acquisto da un ordine di vendita
Per creare un ordine di acquisto per ogni quantità articolo non disponibile nell'ordine di vendita, è possibile utilizzare la funzione **Crea ordini di acquisto**.

1. Nella home page, selezionare la sezione **Ordini di vendita in corso**.
2. Aprire un ordine di vendita per cui si desidera acquistare degli articoli.
3. Scegliere l'azione **Crea ordini di acquisto**.

    Viene visualizzata la finestra **Crea ordini di acquisto** in cui viene mostrata una riga per ogni articolo differente nell'ordine di vendita. Vengono visualizzate per impostazione predefinita le righe per entrambe le quantità di vendita disponibili e non disponibili (in grigio). È possibile scegliere l'azione **Mostra non disponibili** per visualizzare solo le righe relative alle quantità di vendita non disponibili.

    Il campo **Quantità da acquistare** contiene la quantità di vendita non disponibile per impostazione predefinita.
4. Per effettuare un acquisto di una quantità diversa dalla quantità di vendita non disponibile, modificare il valore nel campo **Quantità da acquistare**.

    > [!NOTE]  
   >   È possibile modificare anche il campo **Quantità da acquistare** nelle righe inattive anche se rappresentano le quantità di vendita completamente disponibili.
5. Scegliere il pulsante **OK**.

    Un ordine di acquisto viene creato per ciascun fornitore di articoli nell'ordine di vendita, inclusa qualsiasi modifica delle quantità effettuata nella finestra **Crea ordini di acquisto**.
6. Continuare a elaborare l'ordine o gli ordini di acquisto, ad esempio, modificando o aggiungendo altre righe all'ordine di acquisto. Per ulteriori informazioni, vedere [Procedura: Registrare gli acquisti](purchasing-how-record-purchases.md).


## <a name="to-create-a-purchase-invoice-from-a-sales-order-or-sales-invoice"></a>Per creare una fattura di acquisto da un ordine o una fattura di vendita
Per creare un'unica fattura di acquisto per una o più righe di un documento di vendita selezionando prima il fornitore da cui effettuare l'acquisto, utilizzare la funzione **Crea fattura di acquisto**.

> [!NOTE]  
>   Questa funzione crea una fattura di acquisto per la quantità articolo esatta nel documento di vendita selezionato. Per modificare la quantità di acquisto, è necessario modificare la fattura di acquisto dopo che è stata creata.  

1. Nella home page, selezionare la sezione **Fatture vendita in corso**.
2. Aprire una fattura di vendita per cui si desidera acquistare degli articoli.
3. Selezionare una o più righe della fattura di vendita da utilizzare nella fattura di acquisto. Per utilizzare tutte le righe della fattura di vendita, selezionarle tutte o non selezionarne alcuna.
4. Scegliere l'azione **Crea fattura di acquisto**.
5. Selezionare **Tutte le righe** o **Righe selezionate**, quindi scegliere **OK**.  
6. Nell'elenco di fornitori che viene visualizzato, selezionare il fornitore da cui si desidera acquistare tutti gli articoli e scegliere **OK**.

    Viene creata una fattura d'acquisto che contiene una, più o tutte le righe nella fattura di vendita.
7. Continuare a elaborare la fattura di acquisto, ad esempio, modificando o aggiungendo altre righe alla fattura di acquisto. Per ulteriori informazioni, vedere [Procedura: Registrare gli acquisti](purchasing-how-record-purchases.md).

## <a name="see-also"></a>Vedi anche
[Acquisti](purchasing-manage-purchasing.md)  
[Procedura: Registrare gli acquisti](purchasing-how-record-purchases.md)  
[Procedura: Fatturare le vendite](sales-how-invoice-sales.md)  
[Procedura: Registrare nuovi fornitori](purchasing-how-register-new-vendors.md)  
[Utilizzo di [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

