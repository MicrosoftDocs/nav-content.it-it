---
title: 'Procedura: Cessione o ritiro dei cespiti'
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
ms.openlocfilehash: 795bb23e7c0b46be095b2bbdfe7705b3d7b1e4ee
ms.contentlocale: it-it
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-dispose-of-or-retire-fixed-assets"></a>Procedura: Cessione o ritiro dei cespiti
In caso di vendita o cessione di un cespite, occorre registrare il valore di cessione per calcolare e registrare il guadagno o la perdita. L'ultimo movimento registrato per un cespite deve essere un movimento di cessione. In caso di cessione parziale di un cespite è possibile registrare più di un movimento di cessione. Il totale di tutti gli importi di cessione registrati deve essere un importo in Avere.

 **NOTA**: in caso di cessione di un cespite in cambio di un altro cespite, occorre registrare sia la vendita del cespite precedente (cessione) sia l'acquisto del nuovo (acquisizione). Per ulteriori informazioni, vedere [Procedura: Acquisire i cespiti](fa-how-acquire.md).

## <a name="to-post-a-disposal-from-the-fixed-asset-gl-journal"></a>Per registrare una cessione tramite Registrazioni Cespiti in C/G  
1. Nell'angolo superiore destro, scegliere l'icona **Cerca pagina o report**, immettere **Registrazioni cespiti in C/G**, quindi scegliere il collegamento correlato.  
2. Creare una riga di registrazione iniziale e compilare i campi in base alle esigenze. Selezionare il campo per visualizzare una breve descrizione del campo o il collegamento a ulteriori informazioni.
3. Nel campo **Tipo reg. cespite** scegliere **Cessione**.
4. Scegliere l'azione **Inserisci conto cespiti**. Una seconda riga di registrazione viene creata per la contropartita impostata per la registrazione della cessione.

    **Nota**: il passaggio 4 funziona solo se è stato impostato quanto segue: nella finestra **Scheda Cat. Reg. Cespite** della categoria di registrazione del cespite, il campo **Conto cessione** contiene il conto di addebito contabilità generale e il campo **Conto saldo cessione** contiene il conto C/G in cui si desidera registrare i movimenti di contropartita per la rivalutazione. Per ulteriori informazioni, vedere Impostare la sezione "Per impostare categorie di registrazione cespiti" in [Procedura: Impostare i valori generali per i cespiti](fa-how-setup-general.md).
5. Scegliere l'azione **Registra**.

In caso di vendita o di cessione parziale di un cespite occorre suddividere il cespite prima di registrare la transazione di cessione. Per ulteriori informazioni, vedere [Procedura: Trasferimento, divisione o raggruppamento dei cespiti](fa-how-trans-split-combine.md).

## <a name="to-view-disposal-ledger-entries"></a>Per visualizzare i movimenti contabili di cessione  
In caso di vendita o di cessione di un cespite, il valore di cessione viene registrato nella contabilità generale dove è possibile visualizzare il risultato.   

1. Nell'angolo superiore destro, scegliere l'icona **Cerca pagina o report**, immettere **Cespiti**, quindi scegliere il collegamento correlato.  
2. Selezionare il cespite di cui visualizzare i movimenti, quindi scegliere l'azione **Registri beni ammortizzabili**.
3. Selezionare il registro beni ammortizzabili di cui visualizzare i movimenti, quindi scegliere l'azione **Movimenti contabili**.
4. Selezionare una riga con **Cessione** nel campo **Categoria reg. cespite** e scegliere l'azione **Naviga**.  
5. Nella finestra **Naviga** scegliere la riga del movimento contabile e fare clic sull'azione **Mostra**.
Viene visualizzata la finestra **Movimenti C/G** in cui è possibile visualizzare i movimenti che hanno comportato la registrazione di cessione.

## <a name="see-also"></a>Vedi anche
[Gestione di cespiti](fa-manage.md)  
[Impostazione cespiti](fa-setup.md)  
[Contabilità](finance-setup.md)  
[Benvenuto in Dynamics NAV](across-get-started.md)

