---
title: 'Procedura: Inviare documenti via e-mail'
author: SorenGP
ms.custom: na
ms.date: 11/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: e4476c2ab903001017dcd6c8bdaa84892ba79c9e
ms.contentlocale: it-it
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-send-documents-by-email"></a>Procedura: Inviare documenti via e-mail
Per comunicare rapidamente i contenuti dei documenti aziendali ai partner commerciali, quali le informazioni sui pagamenti nei documenti di vendita ai clienti, è possibile utilizzare la funzionalità di layout del report per definire il contenuto specifico del documento che deve essere inserito nel corpo e-mail automaticamente.

Per abilitare i messaggi e-mail all'interno di Dynamics NAV, avviare il setup assistito **Imposta indirizzo e-mail** nella home page.

È possibile inviare tramite e-mail praticamente tutti i tipi di documento come allegati ai messaggi e-mail direttamente dalla finestra che mostra il documento. Oltre all'allegato, è possibile impostare corpi e-mail specifici per il documento con le informazioni di base estratte dal documento, precedute da un testo standard di saluto e di introduzione al documento in questione. Per offrire ai clienti di pagare elettronicamente gli articoli acquistati utilizzando un servizio di pagamento come PayPal, è possibile inserire nel corpo e-mail anche le informazioni su Paypal e il collegamento ipertestuale di PayPal.

Da tutti i documenti supportati, avviare l'invio tramite e-mail scegliendo l'azione **Invia**, nei documenti registrati, o l'azione **Registra e invia** nei documenti non registrati.

Se il campo **E-mail** della finestra **Invia documento a** è impostato su **Sì (Chiedi impostazioni)**, la finestra **Invia messaggio e-mail** viene aperta con il contatto impostato nel campo **A:** e il documento allegato come file PDF. Nel campo **Corpo** è possibile immettere il testo manualmente oppure è possibile impostare il sistema in modo che il campo sia compilato con un corpo e-mail preparato specificatamente per il documento.

Nella procedura riportata di seguito viene descritto come impostare il report **Vendite - Fattura** in modo che venga utilizzato per il corpo e-mail specifico del documento quando si inviano tramite e-mail le fatture di vendita.

## <a name="to-set-up-a-document-specific-email-body-for-sales-invoices"></a>Per impostare un corpo e-mail specifico del documento per le fatture di vendita
1. Nell'angolo superiore destro scegliere l'icona **Cerca pagina o report**, immettere **Selezioni report Vendite**, quindi scegliere il collegamento correlato.
2. Nella finestra **Selezione report - Vendite**, nel campo **Utilizzo**, selezionare **Fattura**.
3. In una nuova riga nel campo **ID report** selezionare ad esempio il report standard 1306.
4. Selezionare la casella di controllo **Utilizza per corpo e-mail**.
5. Scegliere il campo **ID layout corpo e-mail**, quindi selezionare uno dei layout disponibili dalla finestra **Layout report personalizzati**.
6. I layout dei report definiscono lo stile e il contenuto del corpo e-mail, incluso il testo standard che precede le informazioni principali del documento nel corpo e-mail.
7. Per visualizzare o modificare il layout su cui si basa il corpo e-mail, nella scheda **Layout report personalizzati** scegliere l'azione **Modifica layout**.
8. Se si desidera offrire ai clienti la possibilità di pagare elettronicamente gli articoli acquistati, è possibile configurare il servizio di pagamento correlato, come PayPal, inserire nel corpo e-mail anche le informazioni su Paypal e il collegamento ipertestuale a PayPal. Per ulteriori informazioni, vedere [Procedura: Abilitare i pagamenti clienti attraverso PayPal](sales-how-enable-customer-payments-paypal.md).
9. Scegliere il pulsante **OK**.

A questo punto, quando si sceglie ad esempio l'azione Invia nella finestra **Fattura vendita registrata**, il corpo e-mail conterrà le informazioni del report 1306 precedute dal testo standard creato in base al layout di report selezionato nel passaggio 5.

Nella procedura riportata di seguito viene descritto come inviare una fattura di vendita registrata come messaggio e-mail con il documento allegato come file PDF e con il corpo e-mail specifico del documento.
## <a name="to-send-documents-by-email"></a>Per inviare i documenti tramite e-mail
1. Nell'angolo superiore destro, scegliere l'icona **Cerca pagina o report**, immettere **Fatture vendite registrate**, quindi scegliere il collegamento correlato.
2. Selezionare la fattura di vendita appropriata e scegliere l'azione **Invia**. Verrà visualizzata la finestra **Invia documento a**.
3. Nel campo **E-mail** selezionare **Sì (Chiedi impostazioni)**. Per ulteriori informazioni, vedere [Procedura: Impostare profili di invio documenti](sales-how-setup-document-send-profiles.md).
4. Scegliere il pulsante **OK**. Verrà visualizzata la finestra **Invia messaggio e-mail**.
5. Nel campo **A:** immettere un indirizzo e-mail valido. Il valore predefinito è l'indirizzo e-mail del cliente.
6. Nel campo **Cc:**, specificare un indirizzo e-mail per inviare una copia del messaggio anche a un altro destinatario.
7. Nel campo **Ccn:**, specificare un indirizzo e-mail per inviare una copia del messaggio e-mail a un altro destinatario senza che l'indirizzo e-mail e il nome specificati vengano visualizzati dagli altri destinatari.
8. Nel campo **Oggetto**, immettere un testo descrittivo dell'oggetto. Il valore predefinito è il nome e il numero di fattura del cliente.
9. Nel campo **Allegato** la fattura generata viene allegata per impostazione predefinita come file PDF. Scegliere il pulsante di ricerca per aprire il file o per allegarne un altro.
10. Nel campo **Corpo**, immettere un breve messaggio per il destinatario.

    Se il corpo e-mail specifico del documento è impostato nella finestra **Selezione report - Vendite**, il campo **Corpo** viene compilato automaticamente. Per ulteriori informazioni, vedere la sezione “Per impostare un corpo e-mail specifico del documento per le fatture di vendita” in questo argomento.
11. Selezionare la casella di controllo **Modifica in Outlook Web App** per aprire il messaggio e-mail nell'app di posta elettronica di Office 365.
12. Scegliere **OK** per inviare il messaggio e-mail.

**Nota**: se non è necessario specificare le impostazioni dell'e-mail ogni volta che si invia un documento, è possibile selezionare l'opzione **Sì (Usa impostazioni di default)** nel campo E-mail della finestra **Invia documento a**. In questo caso, non verrà visualizzata la finestra **Invia messaggio e-mail**. Vedere il passaggio 4. Per ulteriori informazioni, vedere [Procedura: Impostare profili di invio documenti](sales-how-setup-document-send-profiles.md).

## <a name="see-also"></a>Vedi anche  
[Utilizzare Dynamics NAV](ui-work-product.md)  
[Procedura: Fatturare le vendite](sales-how-invoice-sales.md)

