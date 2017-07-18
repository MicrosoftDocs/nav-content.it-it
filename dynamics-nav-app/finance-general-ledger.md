---
title: "Contabilità generale e piano dei conti"
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
ms.openlocfilehash: 9965ddcad214e97c5e4858824395d6f651b3c003
ms.contentlocale: it-it
ms.lasthandoff: 06/26/2017

---

# <a name="the-general-ledger-and-the-chart-of-accounts"></a>Contabilità generale e piano dei conti
La contabilità generale memorizza i dati finanziari e il piano dei conti indica in conti in cui sono registrati tutti i movimenti C/G. Dynamics NAV include un piano dei conti standard pronto per supportare l'azienda.

## <a name="general-ledger-setup-and-general-posting-setup"></a>Setup contabilità generale e setup registrazioni COGE
La contabilità generale e la configurazione di come i dati vengono registrati nella contabilità generale sono al centro dei processi aziendali.
Utilizzare la finestra **Setup Contabilità Generale** per specificare le modalità di gestione di determinate questioni contabili relative alla società. Ad esempio i dettagli relativi all'arrotondamento delle fatture, i formati degli indirizzi e se si desidera utilizzare una valuta contabile aggiuntiva.
Analogamente, nella finestra **Setup registrazioni COGE** è possibile specificare come si desidera impostare le combinazioni di categorie di registrazione business generale e le categorie di registrazione di articoli e servizi. Compilare una riga per ogni combinazione di categorie di registrazione business e di categorie di registrazione articoli/servizi.  

## <a name="the-chart-of-accounts"></a>Piano dei Conti
Nel piano dei conti sono visualizzati tutti i conti. Consente di aprire diversi report in cui sono visualizzati i movimenti C/G e i saldi e di chiudere il conto economico. Per ogni conto, è possibile aprire la scheda conto C/G e aggiungere o modificare le impostazioni. È inoltre possibile visualizzare una lista delle categorie di registrazione che registrano nel conto.  

Dynamics NAV impedirà di eliminare un conto di contabilità generale che memorizza dati necessari per il piano dei conti.  

## <a name="account-categories"></a>Categorie di conti
Le categorie di conti consentono di mappare i conti di contabilità generale alle categorie come personalizzazione della struttura dei rendiconti finanziari.  

La finestra **Categorie conto C/G** visualizza le categorie e sottocategorie principali esistenti e i conti C/G assegnati a ogni categoria. È possibile creare nuove sottocategorie e assegnarle categorie ai conti esistenti.  

È possibile raggruppare le categorie di conti impostando un indentazione per le singole sottocategorie. Ciò consente di ottenere una panoramica, in quanto ogni raggruppamento mostra un saldo totale. Ad esempio, è possibile creare sottocategorie per i diversi tipi di cespiti e quindi creare le categorie di registrazione per cespiti rispetto e cespiti correnti. È possibile creare un gruppo di categoria definendo un'indentazione di altre categorie in una riga nella finestra **Categorie conto C/G**.  

Per ogni sottocategoria, è possibile specificare se i conti di questa categoria devono essere inclusi in determinati tipi di report finanziari. Le categorie di conto consentono di definire il layout dei rendiconti finanziari. Ad esempio, l'estratto conto di default presenta un unico movimento relativo ai contanti nelle risorse. Se si desidera che nell'estratto conto siano presenti voci secondarie per la piccola cassa e il conto assegni, è possibile aggiungere due nuove sottocategorie, specificare la Definizione report addizionale Conti di cassa per ognuno di essi e impostate un'indentazione della sottocategoria Cassa. Dopo avere generato le situazioni contabili basate sulle modifiche, l'estratto conto successivo successivo verrà mostrerà il saldo totale per la cassa contanti e due righe con saldi per la piccola cassa e il conto assegni.     

##<a name="see-also"></a>Vedi anche
[Contabilità](finance-setup.md)  
[Impostare o modificare il piano dei conti](finance-setup-setup-chart-accounts.md)  
[Situazioni contabili](finance-setup-account-schedule.md)  

