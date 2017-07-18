---
title: Gestire i documenti in entrata
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
ms.openlocfilehash: 49acc3549180b73dada6415f3ea40f17c1dd9e4c
ms.contentlocale: it-it
ms.lasthandoff: 06/26/2017

---

# <a name="manage-incoming-documents"></a>Gestire i documenti in entrata
Alcune transazioni commerciali non vengono registrate in Dynamics NAV dall'inizio. Invece, un documento commerciale esterno arriva nella propria società come allegato a un messaggio e-mail o copia cartacea che è possibile scansionare e trasformare in file. Ciò è tipico degli acquisti, dove questi file di documenti in entrata rappresentano le ricevute di pagamento per le spese o i piccoli acquisti.

Dai PDF o dai file di immagine dei documenti in entrata è possibile impostare un servizio esterno OCR (Optical Character Recognition, riconoscimento ottico dei caratteri) in modo che generi documenti elettronici che possono essere convertiti in record di documenti in Dynamics NAV.

Nella finestra **Documenti in entrata** è possibile utilizzare diverse funzioni per esaminare le ricevute relative alle spese, gestire le attività OCR e convertire i file dei documenti in entrata, manualmente o automaticamente, nei relativi documenti o in righe di registrazione. I file esterni possono essere allegati in qualsiasi fase dell'elaborazione, ad esempio ai documenti registrati, nonché ai fornitori, clienti e movimenti di contabilità generale risultanti.

L'elaborazione di documenti in entrata è costituita dalle seguenti operazioni principali:

* Registrare i documenti esterni in Dynamics NAV creando le righe nella finestra **Documenti in entrata** attenendosi a uno dei modi seguenti:
    * Manualmente, utilizzando le funzioni semplici da un PC o un dispositivo mobile, in uno dei seguenti modi:
        * Utilizzare il pulsante **Crea da file** e compilare i campi pertinenti nella finestra **Documento in entrata**. Il file viene automaticamente allegato.  
        * Utilizzare il pulsante **Nuovo** e compilare i campi pertinenti nella finestra **Documento in entrata** e allegare manualmente il relativo file.
        * Da un tablet o un telefono, utilizzare il pulsante **Crea da fotocamera** per creare un nuovo record di documento in entrata e quindi inviare l'immagine, ad esempio al servizio OCR.
    * Automaticamente, ricevendo il documento dal servizio OCR come documento elettronico dopo aver inviato tramite e-mail il PDF o il file di immagine correlato al servizio OCR. La Scheda dettaglio **Informazioni finanziarie** viene automaticamente compilata nella finestra **Documento in entrata**.
* Utilizzare il servizio OCR per convertire PDF o file di immagine in documenti elettronici che possono essere convertiti in record di documento in Dynamics NAV.
* Creare nuovi documenti o righe registrazione COGE dai record di un documento in entrata immettendo le informazioni mentre vengono lette nei file del documento in entrata.
* Allegare i file di documenti in entrata ai documenti di acquisto e vendita con qualsiasi stato, ad esempio fornitore, cliente e movimenti di contabilità generale derivanti dalla registrazione.
* Visualizzare i record di documenti in entrata e i relativi allegati in qualsiasi documento o movimento di acquisto e vendita oppure individuare tutti i movimenti di contabilità generale senza i record di documenti in entrata nella finestra **Piano dei conti**.


|Per |Vedere |
|---|----|
|Impostare la funzionalità Documenti in entrata e impostare il servizio OCR.|[Procedura: Impostare documenti in entrata](across-how-setup-income-documents.md)|
|Creare i record dei documenti in entrata, allegare i file, utilizzare OCR per convertire i file PDF in documenti elettronici, convertire documenti elettronici in record di documento, controllare i documenti di vendita e di acquisto registrati dei record di documenti in entrata.|[Elaborare i documenti in entrata](across-process-income-documents.md)|

## <a name="see-also"></a>Vedi anche  
[Gestire gli acquisti](purchasing-manage-purchasing.md)  
[Utilizzare Dynamics NAV](ui-work-product.md)

