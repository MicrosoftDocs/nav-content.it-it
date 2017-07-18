---
title: Imposte di vendita e gruppi di imposte negli Stati Uniti e in Canada
author: edupont04
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: f70a191fc8392bf1685c08c7e905ac96ba7ed069
ms.contentlocale: it-it
ms.lasthandoff: 06/26/2017

---

# <a name="sales-tax-and-tax-groups-in-the-us-and-canada"></a>Imposte di vendita e gruppi di imposte negli Stati Uniti e in Canada
La prima volta che si avvia Dynamics NAV è possibile eseguire una guida al setup assistito per impostare in modo semplice e rapido le informazioni fiscali della società ed eventualmente dei clienti e dei fornitori. In pochi minuti si è pronti a creare documenti di vendita e di acquisto con le imposte calcolate correttamente.
Se si passa a una società vuota, consigliamo di iniziare utilizzando ciascuna guida al setup assistito, inclusa quella per le imposte di vendita. Se si preferisce impostare le imposte manualmente, questo articolo spiega i fattori da tenere in considerazione.  

## <a name="tax-groups-tax-areas-and-tax-jurisdictions"></a>Categorie fiscali, aree imposte e giurisdizioni fiscali
In Dynamics NAV una categoria fiscale rappresenta un gruppo di risorse o di articoli di magazzino che sono soggetti a tassazione identica. Ad esempio, è possibile impostare una categoria fiscale per gli articoli tassabili e un'altra per gli articoli non soggetti a tassazione. È necessario assegnare i codici di categoria fiscale agli articoli di magazzino e ai conti C/G. Analogamente, è necessario assegnare i codici area imposte ai clienti, alle ubicazioni e alle impostazioni della società. Queste assegnazioni possono essere effettuate tramite la guida al setup assistito.  

Ogni area imposte è un raggruppamento delle giurisdizioni fiscali basate su una determinata ubicazione geografica. Ad esempio, l'area imposte di Miami, Florida, include tre giurisdizioni fiscali: città (Miami), provincia (Dade) e stato (Florida). Dynamics NAV include un set di aree imposte limitato con una configurazione predefinita, ma è possibile modificare queste aree e aggiungerne di nuove.  

Se si creano nuove aree e giurisdizioni fiscali è necessario verificare di completare correttamente i campi. Negli Stati Uniti gli stati, le province, le città e le località possono applicare l'imposta di vendita. In Canada, il governo federale e le province possono imporre le imposte di vendita. Le società incassano e rimettono queste imposte alle autorità governative per i prodotti venduti agli utenti finali. Le imposte di vendita possono inoltre essere sommate a un'imposta di vendita esistente. Ad esempio, un'imposta può essere calcolata su un importo di fattura di vendita che già include le imposte di altre giurisdizioni.  

In Canada, gli importi fiscali devono essere dettagliati nei documenti per ogni giurisdizione fiscale. In un documento possono comparire fino a un massimo di quattro giurisdizioni e le giurisdizioni che hanno lo stesso ordine di stampa vengono combinate quando vengono stampate.

## <a name="tax-details"></a>Dettagli imposta
Nella finestra **Dettagli imposta** vengono mostrate le differenti combinazioni delle giurisdizioni fiscali e delle categorie di imposte per determinare le aliquote. Per ogni giurisdizione fiscale, è consigliabile impostare una categoria di imposte per la tassazione normale, un'altra categoria per gli articoli o i servizi che non sono soggetti a tassazione e una categoria aggiuntiva per ogni tipo di articolo o servizio gestito con un'aliquota differente in quella giurisdizione.  

Negli Stati Uniti, quando si vende a un cliente presso un'ubicazione in cui non si ha una *sede* legale, non si incassano le imposte. Per le ubicazioni in cui non è presente una sede legale, assicurarsi che entrambi i campi **Imposta sotto minimo** e **Imposta sopra massimo** siano impostati su 0,00.  

## <a name="see-also"></a>Vedi anche
[Contabilità](finance-setup.md)  
[Impostare gli aspetti finanziari](finance-setup-setup-finance-setup.md)  
[Imposte sulla vendita e Goods and Services Tax in Canada](ca-finance-setup-tax.md)  
[Setup semplificato delle imposte](https://madeira.microsoft.com/en-us/blog/sales-tax-setup-made-easy)  

