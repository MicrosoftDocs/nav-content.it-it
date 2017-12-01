---
title: Utilizzo dell'estensione per la migrazione QuickBooks
description: Descrive come utilizzare l'estensione per importare clienti, fornitori, articoli e conti da QuickBooks Desktop a Dynamics NAV.
author: edupont04
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms. search.keywords: app, add-in, manifest, customize, import, implement
ms.date: 03/29/2017
ms.author: edupont
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 7b8cf77369a2073f746aebdca5d4cbeba80283ec
ms.contentlocale: it-it
ms.lasthandoff: 10/16/2017

---
# <a name="the-quickbooks-data-migration-extension-for-dynamics-nav"></a>Estensione di migrazione dei dati QuickBooks per Dynamics NAV
Questa estensione consente di eseguire la migrazione di clienti, fornitori, articoli e conti da QuickBooks Desktop a [!INCLUDE[d365fin](includes/d365fin_md.md)]. Se l'azienda al momento utilizza QuickBooks, è possibile esportare le informazioni rilevanti e aprire una guida al setup assistito per caricare i dati in [!INCLUDE[d365fin](includes/d365fin_md.md)].  
Per ulteriori informazioni, vedere [Importazione dei dati aziendali da altri sistemi contabili](upload-data.md).

## <a name="exporting-data-from-quickbooks-desktop"></a>Esportazione di dati da QuickBooks Desktop
È necessario aver esportato alcuni o tutti i clienti, i fornitori, gli articoli di magazzino e i conti esistenti in un file IIF (Intuit Interchange Format). L'estensione per la migrazione dei dati QuickBooks include una mappatura predefinita dei dati QuickBooks affinché i dati esistenti possano essere utilizzati per testare la nuova azienda con [!INCLUDE[d365fin](includes/d365fin_md.md)]. La mappatura predefinita sarà sufficiente nella maggior parte dei casi, ma è possibile modificare la mappatura nella guida al setup assistito.  
Nel menu File di QuickBooks è presente un'utilità per l'esportazione di elenchi. Ai fini di [!INCLUDE[d365fin](includes/d365fin_md.md)], è possibile esportare i seguenti elenchi:

* Lista clienti  
* Lista fornitori  
* Elenco articoli  
* Lista conti  

I dati esportati vengono salvati come file IIF, che può essere successivamente caricato in [!INCLUDE[d365fin](includes/d365fin_md.md)].

## <a name="finding-the-quickbooks-data-migration-extension"></a>Utilizzo dell'estensione per la migrazione dei dati QuickBooks
L'estensione per la migrazione dei dati QuickBooks si trova nella Guida setup assistito Migrazione dati ed è pronta all'uso. Per utilizzare l'estensione dopo aver esportato i dati da QuickBooks, scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **Setup assistito**, quindi scegliere il collegamento correlato. Scegliere **Migra dati aziendali**, quindi seguire i passaggi nella guida.  

## <a name="see-also"></a>Vedi anche
[Importazione dei dati aziendali da altri sistemi contabili](upload-data.md)  
[Personalizzazione di [!INCLUDE[d365fin](includes/d365fin_md.md)] utilizzando le estensioni ](ui-extensions.md)  

