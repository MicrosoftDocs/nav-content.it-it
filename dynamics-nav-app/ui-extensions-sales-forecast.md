---
title: Previsione vendite e magazzino
author: edupont04
ms.custom: na
ms.date: 09/23/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: 765527ed4f4800acec20f0abbd4374e95c9c36dc
ms.contentlocale: it-it
ms.lasthandoff: 06/26/2017

---

# <a name="sales-and-inventory-forecast-for-dynamics-nav"></a>Previsione vendite e magazzino per Dynamics NAV
La Gestione del magazzino è un trade-off tra l'assistenza clienti e la gestione dei costi. Da un lato, un magazzino basso richiede meno capitale di lavoro, ma dall'altro un magazzino in esaurimento potenzialmente porta a vendite mancate. L'estensione Previsione vendite e magazzino prevede le vendite potenziali utilizzando i dati storici e fornisce una chiara panoramica delle scorte esaurite previste. A seconda della previsione, l'estensione consente di creare le richieste di approvvigionamento per i fornitori e quindi di risparmiare tempo.  

## <a name="setting-up-forecasting"></a>Impostazione delle previsioni
In Dynamics NAV occorre impostare la connessione ad Azure Machine Learning (Azure ML). Per ulteriori informazioni, vedere [Procedura: Registrare Dynamics NAV nel portale di gestione di Azure](ui-how-register-dynamics-nav-azure.md). Una volta stabilita la connessione, è possibile configurare la previsione per utilizzare un tipo diverso di periodo per il report, ad esempio passare dalle previsioni mensili alle previsioni trimestrali. È inoltre possibile scegliere il numero di periodi per calcolare la previsione, a seconda dei dettagli si desidera includere nella previsione. Si suggerisce di effettuare una previsione in base al mese e con un orizzonte di 12 mesi.  

## <a name="using-the-forecasts"></a>Uso delle previsioni
L'estensione utilizza le funzionalità Azure ML per stimare le vendite future in base allo storico delle vendite allo scopo di evitare l'insufficienza di scorte. Ad esempio, quando si sceglie un articolo nella finestra **Articoli**, nel grafico **Previsione articolo** vengono visualizzate le vendite stimate dell'articolo nel periodo futuro. In questo modo è possibile vedere se si stanno per esaurire le scorte dell'articolo.  

È inoltre possibile utilizzare l'estensione per suggerire quando rifornire il magazzino. Ad esempio, se si crea un ordine di acquisto per Fabrikam perché si desidera acquistare la loro nuova sedia da scrittorio, l'estensione Previsione vendite e magazzino suggerisce anche di rifornirsi della poltrona girevole LONDRA che in genere viene acquistata da questo fornitore. Ciò avviene in quanto l'estensione prevede che le scorte della poltrona girevole LONDRA si esauriranno nel prossimo bimestre e pertanto è possibile che si desideri ordinare già da ora altre sedie.  

## <a name="see-also"></a>Vedi anche
[Gestire le vendite](sales-manage-sales.md)  
[Gestire i costi del magazzino](inventory-manage-inventory.md)  
[Personalizzazione di Dynamics NAV utilizzando le estensioni](ui-extensions.md)  
[Procedura: Registrare Dynamics NAV nel portale di gestione di Azure](ui-how-register-dynamics-nav-azure.md)  

