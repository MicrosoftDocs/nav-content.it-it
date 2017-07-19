---
title: 'Procedura: Abilitare i pagamenti clienti attraverso PayPal'
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
ms.openlocfilehash: a2268d8454af761c40b11d89b01778a3f92090fb
ms.contentlocale: it-it
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-enable-customer-payments-through-paypal"></a>Procedura: Abilitare i pagamenti clienti attraverso PayPal#
Come alternativa alla riscossione dei pagamenti tramite bonifico o carte di credito, è possibile offrire ai clienti di pagare tramite il conto PayPal.

Quando un cliente sceglie il collegamento a PayPal in una fattura di vendita o in un documento ordine di vendita, viene visualizzata la pagina di assistenza per il conto PayPal nella quale sono disponibili i dettagli di pagamento per la vendita. Il cliente può quindi pagare la fattura con la stessa modalità di un qualsiasi altro pagamento PayPal.

Per abilitare i pagamenti dei clienti attraverso PayPal, è necessario attenersi alla seguente procedura:

1. Impostare PayPal Payments Standard come servizio di pagamento nella finestra **Servizi di pagamento**.
2. Selezionare PayPal Payments Standard nel campo **Servizio di pagamento** nel documento di vendita in questione.

Il servizio PayPal Payments Standard verrà installato come estensione di Dynamics NAV e sarà pronto per essere abilitato. Per ulteriori informazioni, vedere [Personalizzazione di Dynamics NAV utilizzando le estensioni](ui-extensions.md).

## <a name="to-enable-the-paypal-payments-standard-service"></a>Per abilitare il servizio PayPal Payments Standard
1. Nell'angolo superiore destro, scegliere l'icona **Cerca pagina o report**, immettere **Servizi di pagamento**, quindi scegliere il collegamento correlato.  
2. Nella finestra **Servizi di pagamento** scegliere l'azione **Nuovo**.
3. Selezionare **PayPal Standard**, quindi chiudere la finestra.
4. Nella finestra **Servizi di pagamento** scegliere l'azione **Setup**.
5. Compilare i campi, se necessario. Selezionare il campo per visualizzare una breve descrizione del campo o il collegamento a ulteriori informazioni.

    **Nota**: selezionare la casella di controllo **Includi sempre in documenti** se il collegamento ipertestuale per il servizio di pagamento PayPal deve essere sempre visibile nei documenti di vendita laddove il pagamento tramite PayPal è abilitato.

6. Chiudere la finestra.

## <a name="to-select-paypal-payments-standard-on-a-sales-invoice"></a>Per selezionare PayPal Payments Standard in una fattura di vendita
1. Nella home page scegliere **Fatture vendite**.
2. Aprire la fattura di vendita per cui si desidera abilitare i pagamenti tramite PayPal.
3. Nel campo **Servizio di pagamento** scegliere PayPal Payments Standard.

**Nota**: il campo **Servizio di pagamento** è visibile solo se il servizio PayPal Payments Standard è abilitato.   

## <a name="see-also"></a>Vedi anche  
[Impostare le vendite](sales-setup-sales.md)  
[Gestire le vendite](sales-manage-sales.md)  
[Personalizzazione di Dynamics NAV utilizzando le estensioni](ui-extensions.md)

