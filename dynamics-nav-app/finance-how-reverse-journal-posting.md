---
title: Annullare una registrazione con un movimento di pareggio
description: "Se è stata eseguita una registrazione errata nelle registrazioni generali, è possibile utilizzare la funzione Storno per annullare la registrazione con un audit trail corretto."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: reimbursement
ms.date: 08/03/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: b9b1f062ee6009f34698ea2cf33bc25bdd5b11e4
ms.openlocfilehash: 2970914c36f892a5610509e9dc4015d0fb159642
ms.contentlocale: it-it
ms.lasthandoff: 10/23/2017

---
# <a name="how-to-reverse-postings"></a>Procedura: Stornare le registrazioni
Per stornare una registrazione errata, selezionare un movimento e creare movimenti di storno, ovvero movimenti identici a quelli originali ma con segno opposto nel campo relativo all'importo, con numero di documento e data di registrazione identici a quelli del movimento originale. Dopo lo storno di un movimento, è necessario creare il movimento corretto.

È possibile stornare solo movimenti immessi da una riga di registrazioni generali. Un movimento può essere stornato solo una volta.

Per ulteriori informazioni sulla registrazione dalle registrazioni generali, vedere [Procedura: Registrare le transazioni direttamente nella contabilità generale](finance-how-post-transactions-directly.md).

Se è stata eseguita una registrazione di quantità negativa, ad esempio se è stato creato un ordine di acquisto con un numero errato di articoli e lo si è registrato come ricevuto (ma non fatturato), è possibile annullare la registrazione.

Se è stata eseguita una registrazione di quantità positiva, ad esempio se è stato creato un ordine di reso con un numero errato di articoli e lo si è registrato come spedito (ma non fatturato), è possibile annullare la registrazione.   

## <a name="to-reverse-the-journal-posting-of-a-general-ledger-entry"></a>Per stornare la registrazione di un movimento di contabilità generale
È possibile stornare i movimenti da tutte le finestre **Movimenti contabili**. La seguente procedura è basata sulla finestra **Movimenti C/G**.
1. Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **Movimenti C/G**, quindi scegliere il collegamento correlato.
2. Selezionare il movimento che si desidera stornare quindi scegliere l'azione **Storno**. Si noti che è necessario che il movimento derivi da una registrazione.
3. Nella finestra **Storna movimenti transazioni**, selezionare il movimento appropriato quindi scegliere l'azione **Storna**.
4. Scegliere il pulsante **Sì** nel messaggio di conferma.

## <a name="to-undo-a-quantity-posting-on-a-posted-purchase-receipt"></a>Per annullare la registrazione di una quantità in una ricezione acquisti registrata  

1.  Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **Ricezioni acquisti registrate**, quindi scegliere il collegamento correlato.  
2.  Aprire il carico registrato che si desidera annullare.  
3.  Selezionare la riga o le righe che si desidera annullare.  
4.  Scegliere l'azione **Annulla carico**.

    Una riga di rettifica viene registrata sotto la riga di carico selezionata.  

    Se la quantità è stata ricevuta in un carico warehouse, una riga di rettifica viene inserita nel carico warehouse registrato.  

    I campi **Quantità ricevuta** e **Qtà carichi non fatt.** nell'ordine di acquisto collegato verranno impostati su un valore pari a zero.

## <a name="to-undo-and-then-redo-a-quantity-posting-on-a-posted-return-shipment"></a>Per annullare e successivamente ripetere la registrazione di una quantità in una spedizione di reso registrata

1.  Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **Spedizioni reso registrate**, quindi scegliere il collegamento correlato.  
2.  Aprire la spedizione reso registrata che si desidera annullare.
3. Selezionare la riga o le righe che si desidera annullare.  

4.  Scegliere l'azione **Eliminare spedizione reso**.  

    Nel documento registrato viene inserita una riga correttiva e i campi **Qtà reso spedita** e **Reso spedito non fatt.** nell'ordine di reso vengono impostati su un valore pari a zero.  

    Ora tornare all'ordine di reso di acquisto per ripetere la registrazione.  

5.  Nella finestra **Spedizione reso registrata** prendere nota del numero nel campo **Nr. ordine di reso**.    
6.  Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **Ordini di reso acquisto**, quindi scegliere il collegamento correlato.  
7.  Aprire l'ordine di reso in questione quindi scegliere l'azione **Riapri**.  
8.  Correggere la voce nel campo **Quantità** e registrare nuovamente l'ordine di reso acquisto.  

## <a name="see-also"></a>Vedi anche
[Procedura: Registrare le transazioni direttamente nella contabilità generale](finance-how-post-transactions-directly.md)  
[Utilizzo delle registrazioni COGE](ui-work-general-journals.md)  
[Finanze](finance.md)  
[Utilizzo di [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)  

