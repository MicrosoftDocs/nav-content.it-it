---
title: Installare le estensioni per personalizzare Dynamics NAV
description: "Informazioni sull'aggiunta di funzionalit� e la personalizzazione di Dynamics NAV tramite l'installazione delle estensioni."
documentationcenter: 
author: edupont04
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: app, add-in, manifest, customize
ms.date: 07/07/2017
ms.author: edupont
ms.translationtype: HT
ms.sourcegitcommit: a16640e014e157d4dbcaabc53d0df2d3e063f8f9
ms.openlocfilehash: 109eb8d0e2a38566739878ef513ffa3bec8dcd30
ms.contentlocale: it-it
ms.lasthandoff: 10/26/2017

---
# <a name="customizing-dynamics-nav-using-extensions"></a>Personalizzazione di Dynamics NAV utilizzando le estensioni
� possibile modificare [!INCLUDE[d365fin](includes/d365fin_md.md)] installando estensioni che, ad esempio, aggiungano funzionalit�, modifichino il comportamento o permettano di accedere a nuovi servizi online.
La prima volta che si avvia [!INCLUDE[d365fin](includes/d365fin_md.md)], alcune estensioni risultano gi� installate. Con il tempo verranno rese disponibili altre estensioni e sar� possibile scegliere se installarle o meno.

Ad esempio, Microsoft fornisce un'estensione che consente l'integrazione con PayPal Payments Standard. Questa estensione � installata per impostazione di default.
Se tuttavia diventa disponibile un'altra estensione che offre l'integrazione con un altro servizio di pagamento, � possibile installare la nuova estensione e scegliere quale dei due servizi utilizzare.  

Le estensioni vengono gestite nella finestra **Gestione estensioni**. � possibile accedere a questa finestra dalla home page. In alternativa, scegliere l'icona **Cerca pagina o report** ![Cerca pagina o report](media/ui-search/search_small.png "Cerca pagina o report") nell'angolo superiore destro, inserire **Estensione**, quindi scegliere il collegamento correlato.  

> [!NOTE]  
>   Se si prevede di dover accedere a un'estensione, ma non � possibile individuare la relativa funzionalit�, controllare la finestra **Gestione estensioni**, se l'estensione non � elencata, � possibile installarla come descritto nella sezione seguente.  

## <a name="installing-an-extension"></a>Installazione di un'estensione
� possibile ottenere le nuove estensioni dal marketplace all'indirizzo [AppSource.microsoft.com](https://appsource.microsoft.com/en-us/marketplace/apps?product=dynamics-365%3Bdynamics-365-for-financials&page=1) dove sono disponibili tutte le estensioni per [!INCLUDE[d365fin](includes/d365fin_md.md)] e le app, le estensioni e i pacchetti di contenuti per altri prodotti Microsoft. Impostare i filtri desiderati, leggere le informazioni relative a ciascuna estensione e ottenere un'estensione per [!INCLUDE[d365fin](includes/d365fin_md.md)].  
> [!NOTE]  
>   Accedere ad [AppSource.microsoft.com](https://appsource.microsoft.com/) utilizzando l'account e-mail che si usa per [!INCLUDE[d365fin](includes/d365fin_md.md)]. Utilizzare lo stesso account e-mail per altri prodotti e servizi per un'esperienza fluida.  

� inoltre possibile accedere al marketplace da [!INCLUDE[d365fin](includes/d365fin_md.md)]. Nella finestra **Gestione estensioni** � possibile vedere le estensioni attualmente installate e aprire la pagina **Marketplace delle estensioni** che mostra le estensioni per [!INCLUDE[d365fin](includes/d365fin_md.md)] al momento disponibili in AppSource. Se si sceglie il collegamento *Altre app*, si passa a [AppSource.microsoft.com](https://appsource.microsoft.com/en-us/marketplace/apps?product=dynamics-365%3Bdynamics-365-for-financials&page=1).  

Se si sceglie un'estensione, � possibile leggerne una descrizione e accedere alla Guida dell'estensione per ottenere ulteriori informazioni. Quando si sceglie di ottenere una interno, � necessario accettare le condizioni per l'utilizzo. Se si ottiene l'estensione dal sito Web AppSource, verr� eseguito l'accesso in [!INCLUDE[d365fin](includes/d365fin_md.md)] per completare l'installazione.  

Quando si installa un'estensione, potrebbe essere necessario configurarla. Se ad esempio si intende utilizzare l'estensione **PayPal Payments Standard per [!INCLUDE[d365fin](includes/d365fin_md.md)]** sar� necessario specificare un conto.
Altre estensioni aggiungono semplicemente dei campi a una pagina esistente oppure aggiungono una nuova pagina.   

Se si disinstalla un'estensione e successivamente si cambia idea, � possibile installarla di nuovo. Quando si disinstalla un'estensione che si sta utilizzando, i dati vengono mantenuti in modo da essere disponibili qualora la si reinstallasse.  

Alcune estensioni sono fornite da Microsoft, altre sono fornite da [altre societ�](ui-extensions-other.md). Tutte le estensioni sono state sottoposte a testing prima di essere rese disponibili. Tuttavia si consiglia di accedere ai collegamenti forniti con ciascuna estensione per ottenere maggiori informazioni sull'estensione prima di scegliere di installarla.  

Microsoft fornisce le seguenti estensioni:  

* [Migrazione dei dati Dynamics GP](ui-extensions-dynamicsgp-data-migration.md)  
* [PayPal Payments Standard](ui-extensions-paypal-payments-standard.md)  
* [Migrazione dei dati QuickBooks](ui-extensions-quickbooks-data-migration.md)  
* [Previsione vendite e magazzino](ui-extensions-sales-forecast.md)  
* [Registro paga di Ceridian](ui-extensions-ceridian-payroll.md)  
* [Importazione del file retribuzioni di Quickbooks](ui-extensions-quickbooks-payroll.md)  
* [WorldPay Payments Standard](ui-extensions-worldpay-payments-standard.md)
* [Utilizzare codici postali di GetAddress.io per il Regno Unito](ui-extensions-getaddressio.md)
* [Migrazione dei dati online QuickBooks](ui-extensions-quickbooks-online-data-migration.md)
* [Portale contabile](ui-extensions-accountant-portal.md)  
* [Analisi di immagini](ui-extensions-image-analyzer.md)

> [!NOTE]  
>  Le nuove estensioni non saranno subito disponibili in AppSource dopo l'annuncio di un aggiornamento. Seguire gli aggiornamenti sulla disponibilit� delle estensioni tramite il sito Web  [AppSource.microsoft.com](https://appsource.microsoft.com/en-us/marketplace/apps?product=dynamics-365%3Bdynamics-365-for-financials&page=1).

## <a name="see-also"></a>Vedi anche
[Procedura: Abilitare i pagamenti clienti attraverso PayPal](sales-how-enable-payment-service-extensions.md)  
[Migrare i dati aziendali da altri sistemi contabili](upload-data.md)    
[Estensioni per [!INCLUDE[d365fin](includes/d365fin_md.md)] fornite da altri provider](ui-extensions-other.md)  
[Benvenuto in [!INCLUDE[d365fin_long](includes/d365fin_long_md.md)]](index.md)  

##


