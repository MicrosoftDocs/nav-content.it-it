---
title: Migrare i dati da Dynamics GP tramite l'estensione per la migrazione dei dati
description: Utilizzare l'estensione per la migrazione dei dati di Dynamics GP per migrare i dati relativi a clienti, fornitori, articoli di magazzino e conti da Dynamics GP a Dynamics NAV.
documentationcenter: 
author: edupont04
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms. search.keywords: app, add-in, manifest, customize, import, implement
ms.date: 03/29/2017
ms.author: edupont
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 0156ec040b96f007674161361e4368b81f7c42d9
ms.contentlocale: it-it
ms.lasthandoff: 10/16/2017

---
# <a name="the-dynamics-gp-data-migration-extension-for-dynamics-nav"></a><span data-ttu-id="6d373-103">Estensione di migrazione dei dati Dynamics GP per Dynamics NAV</span><span class="sxs-lookup"><span data-stu-id="6d373-103">The Dynamics GP Data Migration Extension for Dynamics NAV</span></span>
<span data-ttu-id="6d373-104">Questa estensione consente di eseguire la migrazione di clienti, fornitori, articoli di magazzino e conti da Dynamics GP a [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="6d373-104">This extension makes it easy to migrate customers, vendors, inventory items, and accounts from Dynamics GP to [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span> <span data-ttu-id="6d373-105">Se l'azienda al momento utilizza Dynamics GP, è possibile esportare i record principali rilevanti e aprire una guida al setup assistito per aggiungere i dati in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="6d373-105">If your business uses Dynamics GP today, you can export the relevant master records and then open an assisted setup guide to add the data to [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span> <span data-ttu-id="6d373-106">Per ulteriori informazioni, vedere [Migrare i dati aziendali da altri sistemi contabili](upload-data.md).</span><span class="sxs-lookup"><span data-stu-id="6d373-106">For more information, see [Migrate Business Data from Other Finance Systems](upload-data.md).</span></span>

## <a name="exporting-data-from-dynamics-gp"></a><span data-ttu-id="6d373-107">Esportazione dei dati da Dynamics GP</span><span class="sxs-lookup"><span data-stu-id="6d373-107">Exporting Data from Dynamics GP</span></span>
<span data-ttu-id="6d373-108">È necessario avere esportato alcuni o tutti i clienti, i fornitori, gli articoli di magazzino e i conti esistenti su un file, utilizzando la funzionalità Dynamics GP per l'esportazione dei dati.</span><span class="sxs-lookup"><span data-stu-id="6d373-108">You must have exported some or all of your existing customers, vendors, inventory items, and accounts to a file, using the Dynamics GP functionality for data export.</span></span> <span data-ttu-id="6d373-109">Ai fini di [!INCLUDE[d365fin](includes/d365fin_md.md)], è possibile esportare i seguenti tipi di dati:</span><span class="sxs-lookup"><span data-stu-id="6d373-109">For the purposes of [!INCLUDE[d365fin](includes/d365fin_md.md)], you can export the following types of data:</span></span>

* <span data-ttu-id="6d373-110">Conto</span><span class="sxs-lookup"><span data-stu-id="6d373-110">Account</span></span>  
* <span data-ttu-id="6d373-111">Cliente</span><span class="sxs-lookup"><span data-stu-id="6d373-111">Customer</span></span>  
* <span data-ttu-id="6d373-112">Articolo</span><span class="sxs-lookup"><span data-stu-id="6d373-112">Item</span></span>  
* <span data-ttu-id="6d373-113">Fornitore</span><span class="sxs-lookup"><span data-stu-id="6d373-113">Vendor</span></span>  

<span data-ttu-id="6d373-114">L'estensione per la migrazione dei dati di Dynamics GP mappa automaticamente i dati esportati in modo che i dati dell'utente siano disponibili rapidamente nella nuova società [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="6d373-114">The Dynamics GP Data Migration extension automatically maps the exported data so that your data is quickly available to you in your new [!INCLUDE[d365fin](includes/d365fin_md.md)] company.</span></span> <span data-ttu-id="6d373-115">Durante il processo le informazioni di supporto di setup vengono create, come le categorie di registrazione.</span><span class="sxs-lookup"><span data-stu-id="6d373-115">During the process, supporting setup information is created, such as posting groups.</span></span> <span data-ttu-id="6d373-116">Gli articoli di magazzino verranno introdotti nel sistema con il FIFO come il metodo di valutazione del costo.</span><span class="sxs-lookup"><span data-stu-id="6d373-116">Inventory items will be brought into the system with FIFO as the cost valuation method.</span></span> <span data-ttu-id="6d373-117">I conti verranno impostati come il segmento di conto principale di Dynamics GP con dimensioni, poiché [!INCLUDE[d365fin](includes/d365fin_long_md.md)] non ha segmenti di conto.</span><span class="sxs-lookup"><span data-stu-id="6d373-117">Accounts will be set up as the main account segment from Dynamics GP with dimensions, because [!INCLUDE[d365fin](includes/d365fin_long_md.md)] does not have account segments.</span></span>

## <a name="see-also"></a><span data-ttu-id="6d373-118">Vedi anche</span><span class="sxs-lookup"><span data-stu-id="6d373-118">See Also</span></span>
[<span data-ttu-id="6d373-119">Importazione dei dati aziendali da altri sistemi contabili</span><span class="sxs-lookup"><span data-stu-id="6d373-119">Importing Business Data from Other Finance Systems</span></span>](upload-data.md)  
<span data-ttu-id="6d373-120">[Personalizzazione di [!INCLUDE[d365fin](includes/d365fin_md.md)] utilizzando le estensioni ](ui-extensions.md)</span><span class="sxs-lookup"><span data-stu-id="6d373-120">[Customizing [!INCLUDE[d365fin](includes/d365fin_md.md)] Using Extensions ](ui-extensions.md)</span></span>  
