---
title: 'Procedura: Formulare previsioni del flusso di cassa'
author: bholtorf
ms.custom: na
ms.date: 09/16/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2017
ms.translationtype: HT
ms.sourcegitcommit: 6b60b1344a1e18ad91863046110df880f75f7c04
ms.openlocfilehash: 154fcaef89af0f6a131f4bcf0e9cf9a3f85f5903
ms.contentlocale: it-it
ms.lasthandoff: 10/16/2017

---

# <a name="how-to-make-predictive-cash-flow-forecasts"></a>Procedura: Formulare previsioni del flusso di cassa
Le previsioni del flusso di cassa consentono di garantire che la società abbia abbastanza contanti disponibili per onorare i suoi obblighi finanziari e sono utili per identificare eventuali rettifiche. Ad esempio, se si dispone di un surplus di cassa, potrebbe servire per ripagare qualche debito e un allarme anticipato sarà apprezzabile se i tempi sembrano stretti. 

Cortana Intelligence utilizza il servizio Azure Machine Learning per effettuare previsioni affidabili. Ad esempio, le previsioni di Cortana Intelligence consentono di predire ed evitare disavanzi di cassa. Il servizio associa informazioni storiche con registrazioni attuali relative alla contabilità fornitori e agli incassi, comprese le registrazioni contenenti date di scadenza future. Queste registrazioni comprendono:
* Ordini d'acquisto
* Ordini vendita
* Fatture di vendita e di acquisto registrate
* Note di credito

## <a name="before-you-start"></a>Operazioni preliminari  
Vi sono alcune operazioni da fare prima di poter utilizzare Cortana Intelligence per le previsioni del flusso di cassa: 
* Se non si stanno già utilizzando le previsioni del flusso di cassa, sarà necessario impostare:
    * Una o più impostazioni in **Setup flusso di cassa**. 
    * Conti relativi a crediti, debiti, ordini di vendita e di acquisto. Cortana Intelligence utilizza le registrazioni in questi conti.
    * Una o più previsioni del flusso di cassa in **Previsione flusso di cassa**. Assicurarsi di includere gli ordini di acquisto, gli ordini di vendita, i crediti e i debiti come origini.  
    Per ulteriori informazioni, cercare _previsioni flusso di cassa_ nel sistema della Guida. 
* Conoscere l'URL API e la chiave API del servizio Web predittivo da utilizzare.  
    È possibile utilizzare Azure Machine Learning o un altro servizio, se esistente. In alternativa, un modello pubblico denominato _Forecasting model for Microsoft Dynamics NAV_ è disponibile online nella galleria Cortana Intelligence. Attenersi alla seguente procedura per utilizzare il modello:

    1. In un browser andare alla [Galleria Cortana Intelligence](https://go.microsoft.com/fwlink/?linkid=828352)
    2. Cercare il modello _Forecasting Model for Microsoft Dynamics NAV_, quindi aprirlo in Azure Machine Learning Studio.
    3. Utilizzare l'account Microsoft per impostare un'area di lavoro, quindi copiare il modello.
    4. Eseguire il modello e pubblicarlo come servizio Web.
    5. Prendere nota dell'URL API e della chiave API. Le credenziali verranno utilizzate quando Cortana Intelligence verrà impostato in Microsoft Dynamics NAV.  

* Considerare la frequenza con cui calcolare la previsione. Il servizio Azure Machine Learning ha limitazioni relative all'utilizzo. Ad esempio, se si dispone di molti articoli, potrebbe essere meglio calcolare meno di frequente. 
* Farsi assegnare alla Gestione ruolo utente Contabile. 

## <a name="set-up-cortana-intelligence"></a>Impostare Cortana Intelligence
È possibile utilizzare una guida al setup assistito per impostare le previsioni del flusso di cassa. La guida aiuta a specificare aspetti, quali la frequenza di aggiornamento della previsione, i conti sui cui basarla, le informazioni su quando effettuare i pagamenti delle imposte e se utilizzare Cortana Intelligence.  

Se si sta già utilizzando le previsioni del flusso di cassa e si desidera solo attivare Cortana Intelligence, è possibile anche utilizzare una procedura manuale. Quando si accede, viene visualizzata una notifica su una barra blu nella parte superiore dell'area di lavoro. Per impostare subito Cortana Intelligence, scegliere **Sì**. Il messaggio viene visualizzato solo una volta. Se lo si chiude, utilizzare la procedura manuale per impostare Cortana Intelligence.  

**Suggerimento:** considerare la durata del periodo che il servizio utilizzerà nei suoi calcoli. Più dati immessi, più accurate saranno le previsioni. Inoltre, prestare attenzione a scostamenti ampi nei periodi. Influiranno anche sulle previsioni. Se Cortana Intelligence non trova una quantità sufficiente di dati o i dati variano molto, il servizio non farà una previsione. 

Per utilizzare guida al setup assistito:
1. Nella Gestione ruolo utente Contabile, nel grafico **Previsione flusso di cassa**, scegliere l'azione **Apri setup assistito**.
2. Compilare i campi come richiesto in ogni step della guida.

Per utilizzare una procedura manuale:
1. Cercare **Setup flusso di cassa**, quindi selezionare il collegamento correlato.
2. Espandere la Scheda dettaglio **Cortana Intelligence** e compilare i campi come richiesto.

## <a name="turn-on-cortana-intelligence-for-cash-flow-forecasts"></a>Attivare Cortana Intelligence per le previsioni del flusso di cassa
1. Cercare **Previsioni flusso di cassa**, quindi selezionare il collegamento correlato.
2. Scegliere l'azione **Prospetto flusso di cassa**.
3. Nella pagina **Prospetto flusso di cassa** scegliere l'azione **Suggerisci righe prospetto**.  
4. In **Tipi origine da includere** scegliere la casella di controllo **Previsione di Cortana Intelligence**.

## <a name="investigate-a-cash-flow-forecast"></a>Analizzare una previsione del flusso di cassa
Per dare un'occhiata ai dati dietro la previsione, inclusi gli scostamenti scegliere la colonna **Cortana Intelligence**. Nella prima riga della tabella viene visualizzato lo scostamento. Le altre righe sono disposte in base al documento di origine.  

Ad esempio, è possibile vedere come la previsione:    
* Gestisce le vendite e gli acquisti confermati 
* Sottrae i debiti e aggiunge i crediti
* Salta gli ordini di vendita e di acquisto doppi

## <a name="see-also"></a>Vedi anche  
[Utilizzare Dynamics NAV](ui-work-product.md)

