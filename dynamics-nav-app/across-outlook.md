---
title: Utilizzo di Dynamics NAV come Posta in arrivo aziendale in Outlook
author: edupont04
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2017
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: cf4202c3b7186eb1dd4633f74d2d48664458455e
ms.contentlocale: it-it
ms.lasthandoff: 10/16/2017

---

# <a name="using-dynamics-nav-as-your-business-inbox-in-outlook"></a>Utilizzo di Dynamics NAV come Posta in arrivo aziendale in Outlook
Dynamics NAV offre la possibilità di gestire le interazioni d'affari con i clienti e fornitori, direttamente in Microsoft Outlook. Con il componente aggiuntivo Outlook di Dynamics NAV, è possibile visualizzare i dati finanziari relativi a clienti e fornitori e creare e inviare documenti finanziari, quali offerte o fatture.  

Alcune società che utilizzano Office 365 limitano i permessi degli utenti alla distribuzione dei componenti aggiuntivi. Pertanto è necessario assicurarsi di disporre di una sottoscrizione di Office 365 che include la posta elettronica e consente di distribuire i componenti aggiuntivi. È possibile effettuare l'iscrizione per una prova gratuita di 1 mese di di Office 365 [qui](https://products.office.com/try).  

## <a name="get-the-add-in"></a>Ottenere il componente aggiuntivo
In Dynamics NAV, una delle guide al setup assistito è **Impostare i componenti aggiuntivi per Office**. La guida consente inoltre di impostare una connessione tra l'account di Office 365 e Dynamics NAV. Il componente aggiuntivo di Dynamics NAV verrà automaticamente aggiunto a Outlook.  

Il nuovo componente aggiuntivo viene aggiunto alla barra multifunzione di Outlook e in Outlook Web Access nella barra multifunzione del componente aggiuntivo, immediatamente sopra il corpo del messaggio e-mail.  

## <a name="using-the-add-in"></a>Utilizzo del componente aggiuntivo
Quando si riceve un messaggio da un cliente, direttamente in Outlook è possibile aprire il componente aggiuntivo di Dynamics NAV che riconosce il cliente e apre la scheda cliente relativa alla sua società. Dal dashboard, è possibile visualizzare le informazioni generali per il cliente ed eseguire il drill-down per ulteriori dettagli sui documenti specifici. È inoltre possibile approfondire le informazioni cronologiche di vendita per il cliente.
Nel componente aggiuntivo, è possibile creare un'offerta di vendita e inviarla di nuovo al cliente senza uscire da Outlook. Tutte le informazioni necessarie per inviare l'offerta di vendita sono disponibili nella Posta in arrivo aziendale in Outlook.  
Una volta che si inseriscono i dati, è possibile registrare l'offerta. È possibile inviarla tramite posta elettronica. Dynamics NAV genera un file PDF all'offerta di vendita e lo allega al messaggio e-mail definito nel componente aggiuntivo.  

Un'esperienza simile si applica ai messaggi dei fornitori e ai documenti di acquisto.  

Talvolta si desidera visualizzare più campi rispetto a quelli che è possibile visualizzare nel componente aggiuntivo, ad esempio se si desidera compilare le righe di una fattura. Per ottenere maggiore spazio, è possibile visualizzare il componente aggiuntivo in una finestra separata. Fa parte ancora di Outlook, ma offre più spazio per il lavoro. Se si digitano i dati per il documento nella nuova finestra, le modifiche vengono salvate automaticamente. Al termine dell'immissione dei dati per il documento, è possibile chiudere la pagina. Scegliendo il frame del componente aggiuntivo in Outlook, il documento viene aggiornato automaticamente con le modifiche apportate nella visualizzazione apposita.  

## <a name="quick-document-lookup"></a>Ricerca rapida del documento
Il Componente aggiuntivo dei Collegamenti del documento di Dynamics NAV offre accesso rapido ai documenti citati nei messaggi di posta elettronica. Il componente aggiuntivo è disponibile per un messaggio e-mail se un numero di documento viene riconosciuto nel corpo del messaggio. Aprire il componente aggiuntivo consente l'accesso rapido al documento.  

Ad esempio, se si riceve un messaggio e-mail che cita il testo *S-QUO100*, Dynamics NAV lo identifica come un'offerta di vendita e consente di aprire il documento in Outlook. In Outlook, selezionare il pulsante **Collegamenti documento** immediatamente sopra il corpo del messaggio e-mail. In the Outlook Web App, selezionare il testo *V-OFFER1001* nel corpo del messaggio e-mail.  

Nel componente aggiuntivo Collegamenti documento, è possibile modificare ed effettuare azioni relative il documento, come in Dynamics NAV.

## <a name="see-also"></a>Vedi anche
[Benvenuto in Dynamics NAV](across-get-started.md)  
[Finanze](finance.md)  
[Gestire le vendite](sales-manage-sales.md)  
[Gestire gli acquisti](purchasing-manage-purchasing.md)  

