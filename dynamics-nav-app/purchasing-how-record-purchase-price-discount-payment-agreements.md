---
title: 'Procedura: Registrare i prezzi di acquisto e gli sconti'
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
ms.openlocfilehash: f99bb0aeef2c25048b0da3e0476ae2d612bff562
ms.contentlocale: it-it
ms.lasthandoff: 06/26/2017

---

#<a name="how-to-record-purchase-prices-and-discounts"></a>Procedura: Registrare i prezzi di acquisto e gli sconti
I differenti accordi relativi a prezzi e sconti applicati quando si effettuano acquisti da fornitori diversi devono essere definiti in modo che le regole e i valori concordati vengano applicati ai documenti di acquisto creati per il fornitore.

Per quanto riguarda i prezzi, è possibile fare in modo che venga inserito un prezzo di acquisto speciale nelle righe di acquisto quando si verifica una determinata combinazione di fornitore, articolo, quantità minima, unità di misura o data di inizio o di fine.

Nel caso degli sconti, è possibile impostare e utilizzare due tipi di sconti:

|Tipo di sconto: |Descrizione |
|--------------|------------|
|**Sconto riga acquisto**|È possibile fare in modo che venga inserito uno sconto sull'importo nelle righe di acquisto quando si verifica una determinata combinazione di fornitore, articolo, quantità minima, unità di misura o data di inizio o di fine. Il principio è lo stesso dei prezzi di acquisto.|
|**Sconto fattura**|Uno sconto in percentuale che viene sottratto dal totale del documento se l'importo del valore di tutte le righe di un documento di acquisto supera un determinato valore minimo.|

Poiché gli sconti riga acquisto e i prezzi di acquisto sono basati su una combinazione di articolo e fornitore, è anche possibile immettere questa configurazione dalla scheda articolo, in cui sono definiti le regole e i valori. Per ulteriori informazioni, vedere [Procedura: Registrare nuovi prodotti](inventory-how-register-new-products.md).

## <a name="to-set-up-a-special-purchase-price-for-a-vendor"></a>Per impostare un prezzo di acquisto speciale per un fornitore
1. Nell'angolo superiore destro, scegliere l'icona **Cerca pagina o report**, immettere **Fornitori**, quindi scegliere il collegamento correlato.
2. Aprire la scheda fornitore interessata e scegliere l'azione **Prezzi**.

    Il campo **Tipo di acquisto** è già impostato su **Fornitore** e il campo **Codice acquisto** è impostato sul numero del fornitore.
3. Compilare i campi della riga in base alle esigenze. Selezionare il campo per visualizzare una breve descrizione del campo o il collegamento a ulteriori informazioni.
4. Compilare una riga per ogni combinazione per la quale il fornitore concede uno sconto riga acquisto.

## <a name="to-set-up-a-line-discount-for-a-vendor"></a>Per impostare uno sconto riga per un fornitore
1. Nell'angolo superiore destro, scegliere l'icona **Cerca pagina o report**, immettere **Fornitori**, quindi scegliere il collegamento correlato.
2. Aprire la scheda fornitore interessata e scegliere l'azione **Sconti riga**.

    Il campo **Tipo di acquisto** è già impostato su **Fornitore** e il campo **Codice acquisto** è impostato sul numero del fornitore.
3. Compilare i campi della riga in base alle esigenze. Selezionare il campo per visualizzare una breve descrizione del campo o il collegamento a ulteriori informazioni.
4. Compilare una riga per ogni combinazione per la quale il fornitore concede uno sconto riga acquisto.

## <a name="to-set-up-an-invoice-discount-for-a-vendor"></a>Per impostare uno sconto su fattura per un fornitore
Una volta informati degli sconti su fattura concessi dai fornitori, immettere il codice sconto fattura nelle schede fornitore e impostare le condizioni per ciascun codice.

1. Nell'angolo superiore destro, scegliere l'icona **Cerca pagina o report**, immettere **Fornitori**, quindi scegliere il collegamento correlato.
2. Aprire la scheda fornitore relativa al fornitore al quale saranno applicati gli sconti fattura.
3. Nel campo **Cod. sconto fatt.** selezionare un codice per le condizioni di sconto fattura in questione che verrà utilizzato per calcolare gli sconti fattura per il fornitore.

    **Nota**: i codici sconto fattura sono rappresentati da schede fornitore esistenti. Questo consente di assegnare rapidamente le condizioni dello sconto fattura ai fornitori perché basterà selezionare il nome di un altro fornitore che avrà le stesse condizioni.

    Continuare a impostare le nuove condizioni dello sconto fattura di acquisto.
4. Nella finestra **Scheda fornitore** scegliere l'azione **Sconti fattura**. Verrà visualizzata la finestra **Sconti fattura fornitori**.
5. Nel campo **Codice valuta** immettere il codice per una valuta alla quale sono collegate le condizioni dello sconto fattura nella riga. Lasciare il campo vuoto se si desidera impostare le condizioni di sconto fattura in valuta locale.
6. Nel campo **Importo minimo** immettere l'importo minimo che una fattura deve avere affinché le possa essere applicato lo sconto.
7. Nel campo **% sconto** immettere lo sconto fattura sotto forma di percentuale dell'importo fattura.
8. Ripetere i passaggi da 5 a 7 per ogni valuta per la quale il fornitore riceverà uno sconto fattura diverso.

Lo sconto fattura è ora impostato e assegnato al fornitore in questione. Quando si seleziona il codice fornitore nel campo **Cod. sconto fatt.** nelle altre schede fornitore, lo stesso sconto fattura viene assegnato a quei fornitori.

## <a name="see-also"></a>Vedi anche  
[Impostare gli acquisti](purchasing-setup-purchasing.md)  
[Gestire gli acquisti](purchasing-manage-purchasing.md)

