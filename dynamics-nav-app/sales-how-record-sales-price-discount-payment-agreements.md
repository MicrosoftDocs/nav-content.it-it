---
title: 'Procedura: Registrare i prezzi di vendita e gli sconti'
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
ms.openlocfilehash: 2d6438108fb2c36bb6f0d44efddc053bd628d068
ms.contentlocale: it-it
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-record-sales-prices-and-discounts"></a>Procedura: Registrare i prezzi di vendita e gli sconti
È necessario definire i diversi criteri di prezzo e di sconto applicati alle transazioni di vendita ai diversi clienti affinché vengano applicati le regole e i valori concordati ai documenti di vendita creati per i clienti.

Per quanto riguarda i prezzi, è possibile fare in modo che venga inserito un prezzo di vendita speciale nelle righe di vendita quando si verifica una determinata combinazione di cliente, articolo, quantità minima, unità di misura o data di inizio o di fine.

Nel caso degli sconti, è possibile impostare e utilizzare due tipi di sconti su vendita:

|Tipo di sconto: |Descrizione |
|--------------|------------|
|**Sconto Riga Vendita**|È possibile fare in modo che venga inserito uno sconto sull'importo nelle righe di vendita quando si verifica una determinata combinazione di cliente, articolo, quantità minima, unità di misura o data di inizio o di fine. Il principio è lo stesso dei prezzi di vendita.|
|**Sconto fattura**|Uno sconto in percentuale che viene sottratto dal totale del documento se l'importo del valore di tutte le righe di un documento di vendita supera un determinato valore minimo.|

Poiché i prezzi di vendita e gli sconti riga di vendita si basano su una combinazione di articolo e cliente, è altresì possibile eseguire questa configurazione dalla scheda articolo dello specifico articolo, dove si applicano regole e valori.

## <a name="to-set-up-a-sales-price-for-a-customer"></a>Per impostare un prezzo di vendita per un cliente
1. Nell'angolo superiore destro, scegliere l'icona **Cerca pagina o report**, immettere **Clienti**, quindi scegliere il collegamento correlato.
2. Aprire la scheda cliente interessata e scegliere l'azione **Prezzi**.

    Il campo **Tipo vendita** viene precompilato con **Cliente** e il campo **Codice vendita** viene precompilato con il numero del cliente.
3. Compilare i campi della riga in base alle esigenze. Selezionare il campo per visualizzare una breve descrizione del campo o il collegamento a ulteriori informazioni.
4. Compilare una riga per ogni combinazione che concederà un prezzo di vendita speciale al cliente.

## <a name="to-set-up-a-sales-line-discount-for-a-customer"></a>Per impostare uno sconto riga vendita per un cliente
1. Nell'angolo superiore destro, scegliere l'icona **Cerca pagina o report**, immettere **Clienti**, quindi scegliere il collegamento correlato.
2. Aprire la scheda cliente interessata e scegliere l'azione **Sconti riga**.

    Il campo **Tipo vendita** viene precompilato con **Cliente** e il campo **Codice vendita** viene precompilato con il numero del cliente.
3.  Compilare i campi della riga in base alle esigenze. Selezionare il campo per visualizzare una breve descrizione del campo o il collegamento a ulteriori informazioni.
4. Compilare una riga per ogni combinazione che concederà uno sconto riga vendita al cliente.

## <a name="to-set-up-an-invoice-discount-for-a-customer"></a>Per impostare uno sconto su fattura per un cliente
Dopo avere stabilito a quali clienti si debbano applicare gli sconti fattura, è necessario immettere i codici di sconto fattura nelle schede clienti e impostare le condizioni relative ai singoli codici.

1. Nell'angolo superiore destro, scegliere l'icona **Cerca pagina o report**, immettere **Clienti**, quindi scegliere il collegamento correlato.
2. Aprire la scheda cliente relativa al cliente al quale saranno applicati gli sconti fattura.
3. Nel campo **Cod. sconto fatt.** selezionare un codice per le condizioni di sconto fattura in questione che verrà utilizzato per calcolare gli sconti fattura per il cliente.

    **Nota**: i codici sconto fattura sono rappresentati da schede clienti esistenti. Questo consente di assegnare rapidamente le condizioni dello sconto fattura ai clienti perché basterà selezionare il nome di un altro cliente che avrà le stesse condizioni.

    Continuare a impostare le nuove condizioni dello sconto fattura di vendita.
4. Nella finestra **Scheda cliente** scegliere l'azione **Sconti fattura**. Viene aperta la finestra **Sconti fattura clienti**.
5. Nel campo **Codice valuta** immettere il codice per una valuta alla quale sono collegate le condizioni dello sconto fattura nella riga. Lasciare il campo vuoto se si desidera impostare le condizioni di sconto fattura in valuta locale.
6. Nel campo **Importo minimo** immettere l'importo minimo che una fattura deve avere affinché le possa essere applicato lo sconto.
7. Nel campo **% sconto** immettere lo sconto fattura sotto forma di percentuale dell'importo fattura.
8. Ripetere i passaggi da 5 a 7 per ogni valuta per la quale il cliente riceverà uno sconto fattura diverso.

Lo sconto fattura è ora impostato e assegnato al cliente in questione. Quando si seleziona il codice cliente nel campo **Cod. sconto fatt.** nelle altre schede cliente, lo stesso sconto fattura viene assegnato a quei clienti.

## <a name="see-also"></a>Vedi anche  
[Impostare le vendite](sales-setup-sales.md)  
[Gestire le vendite](sales-manage-sales.md)

