---
title: Utilizzare Excel per importare i dati in Dynamics NAV
description: Utilizzare il pacchetto di configurazione di default per aggiungere i dati del cliente in Excel e importare nuovamente i dati in Dynamics NAV.
author: edupont04
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: migration, Excel
ms.date: 07/05/2017
ms.author: edupont
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: eb9b7137ee31824ba845ff336c00c6f0e59f6f5c
ms.contentlocale: it-it
ms.lasthandoff: 10/16/2017

---
# <a name="importing-data-from-legacy-accounting-software-using-a-configuration-package"></a><span data-ttu-id="b7ed0-103">Importazione di dati del software di contabilizzazione legacy utilizzando un pacchetto di configurazione</span><span class="sxs-lookup"><span data-stu-id="b7ed0-103">Importing Data from Legacy Accounting Software using a Configuration Package</span></span>
<span data-ttu-id="b7ed0-104">È possibile importare dati master e alcuni dati transazionali da altri sistemi finanziari in base al pacchetto di configurazione standard disponibile in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="b7ed0-104">You can import master data and some transactional data from other finance systems based on the default configuration package in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span> <span data-ttu-id="b7ed0-105">Nella finestra **Pacchetti di configurazione** è possibile utilizzare il pacchetto per importare e convalidare i dati prima di applicare il pacchetto.</span><span class="sxs-lookup"><span data-stu-id="b7ed0-105">In the **Configuration Packages** window, you can work with the package to import and validate the data before you apply the package.</span></span>  

<span data-ttu-id="b7ed0-106">Se si ha familiarità con i Servizi di RapidStart per Microsoft Dynamics, si conoscono anche i pacchetti di configurazione.</span><span class="sxs-lookup"><span data-stu-id="b7ed0-106">If you are familiar with RapidStart Services for Microsoft Dynamics, you are also familiar with configuration packages.</span></span> <span data-ttu-id="b7ed0-107">Il pacchetto di configurazione di default supporta i più comuni tipi di dati che si desidera importare da un sistema legacy.</span><span class="sxs-lookup"><span data-stu-id="b7ed0-107">The default configuration package supports the most common types of data that you want to import from a legacy system.</span></span> <span data-ttu-id="b7ed0-108">In Excel è possibile aggiungere i dati del sistema legacy e configurarli in base alla logica di business di [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="b7ed0-108">In Excel, you can then add the data from the legacy system and set it up according to the business logic of the [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span>  

> [!TIP]  
>   <span data-ttu-id="b7ed0-109">In alternativa, usare le procedure guidate di migrazione dati per importare i dati da QuickBooks o Dynamics GP.</span><span class="sxs-lookup"><span data-stu-id="b7ed0-109">Alternatively, use data migration wizards to import data from QuickBooks or Dynamics GP.</span></span> <span data-ttu-id="b7ed0-110">Per ulteriori informazioni, vedere [Migrazione dei dati di QuickBooks](ui-extensions-quickbooks-data-migration.md) o [Migrazione dei dati di Dynamics GP](ui-extensions-dynamicsgp-data-migration.md).</span><span class="sxs-lookup"><span data-stu-id="b7ed0-110">For more information, see [QuickBooks Data Migration](ui-extensions-quickbooks-data-migration.md) or [Dynamics GP Data Migration](ui-extensions-dynamicsgp-data-migration.md).</span></span>  

## <a name="working-with-data-in-excel"></a><span data-ttu-id="b7ed0-111">Utilizzo di dati in Excel</span><span class="sxs-lookup"><span data-stu-id="b7ed0-111">Working with Data in Excel</span></span>
<span data-ttu-id="b7ed0-112">Quando si esporta il pacchetto di configurazione di default in Excel, la cartella di lavoro generata contiene un prospetto per ogni tabella del pacchetto.</span><span class="sxs-lookup"><span data-stu-id="b7ed0-112">When you export the default configuration package to Excel, the generated workbook contains a worksheet for each table in the package.</span></span> <span data-ttu-id="b7ed0-113">Per semplificare i task, è possibile avvantaggiarsi degli strumenti di modifica XML incorporati in Excel.</span><span class="sxs-lookup"><span data-stu-id="b7ed0-113">To simplify your tasks, you can take advantage of the XML manipulation tools that are built into Excel.</span></span> <span data-ttu-id="b7ed0-114">È inoltre possibile utilizzare le funzioni incorporate di Excel per agevolare la formattazione dei dati e inserire i dati nella cella appropriata.</span><span class="sxs-lookup"><span data-stu-id="b7ed0-114">You can also use Excel built-in functions to help with data formatting and to put data in the correct cell.</span></span> <span data-ttu-id="b7ed0-115">Ad esempio, aggiungere un prospetto vuoto e copiarvi i dati legacy.</span><span class="sxs-lookup"><span data-stu-id="b7ed0-115">For example, add a blank worksheet and copy the legacy data to it.</span></span> <span data-ttu-id="b7ed0-116">Creare quindi una formula Excel per mappare i dati nel prospetto di trasformazione tra i campi del prospetto esportato e i dati legacy del cliente.</span><span class="sxs-lookup"><span data-stu-id="b7ed0-116">Then make an Excel formula to map data in the transformation worksheet between the fields in the exported worksheet and customer legacy data.</span></span> <span data-ttu-id="b7ed0-117">Dopo aver eseguito la mappatura di tutti i dati, copiare l'intervallo dei dati nel prospetto della tabella.</span><span class="sxs-lookup"><span data-stu-id="b7ed0-117">After you have mapped all of the data, copy the range of data onto the table worksheet.</span></span>  

> [!IMPORTANT]  
>  <span data-ttu-id="b7ed0-118">Non modificare le colonne nei prospetti.</span><span class="sxs-lookup"><span data-stu-id="b7ed0-118">Do not change the columns in the worksheets.</span></span> <span data-ttu-id="b7ed0-119">Se vengono spostate, modificate o eliminate, il prospetto non può essere importato in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="b7ed0-119">If they are moved, changed, or deleted, the worksheet cannot be imported into [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span>

## <a name="tables-in-the-default-configuration-package"></a><span data-ttu-id="b7ed0-120">Tabelle nel pacchetto di configurazione di default</span><span class="sxs-lookup"><span data-stu-id="b7ed0-120">Tables in the Default Configuration Package</span></span>
<span data-ttu-id="b7ed0-121">Il pacchetto di configurazione di default supporta le seguenti tabelle:</span><span class="sxs-lookup"><span data-stu-id="b7ed0-121">The default configuration package supports the following tables:</span></span>

-   <span data-ttu-id="b7ed0-122">Condizioni pagamento</span><span class="sxs-lookup"><span data-stu-id="b7ed0-122">Payment Terms</span></span>
-   <span data-ttu-id="b7ed0-123">Gruppo prezzi cliente</span><span class="sxs-lookup"><span data-stu-id="b7ed0-123">Customer Price Group</span></span>
-   <span data-ttu-id="b7ed0-124">Metodo di spedizione</span><span class="sxs-lookup"><span data-stu-id="b7ed0-124">Shipment Method</span></span>
-   <span data-ttu-id="b7ed0-125">Agenti/Addetti acq.</span><span class="sxs-lookup"><span data-stu-id="b7ed0-125">Salesperson/Purchaser</span></span>
-   <span data-ttu-id="b7ed0-126">Località</span><span class="sxs-lookup"><span data-stu-id="b7ed0-126">Location</span></span>
-   <span data-ttu-id="b7ed0-127">Conto C/G</span><span class="sxs-lookup"><span data-stu-id="b7ed0-127">GL Account</span></span>
-   <span data-ttu-id="b7ed0-128">Cliente</span><span class="sxs-lookup"><span data-stu-id="b7ed0-128">Customer</span></span>
-   <span data-ttu-id="b7ed0-129">Fornitore</span><span class="sxs-lookup"><span data-stu-id="b7ed0-129">Vendor</span></span>
-   <span data-ttu-id="b7ed0-130">Articolo</span><span class="sxs-lookup"><span data-stu-id="b7ed0-130">Item</span></span>
-   <span data-ttu-id="b7ed0-131">Testate vendita</span><span class="sxs-lookup"><span data-stu-id="b7ed0-131">Sales Header</span></span>
-   <span data-ttu-id="b7ed0-132">Righe vendite</span><span class="sxs-lookup"><span data-stu-id="b7ed0-132">Sales Line</span></span>
-   <span data-ttu-id="b7ed0-133">Testate acquisti</span><span class="sxs-lookup"><span data-stu-id="b7ed0-133">Purchase Header</span></span>
-   <span data-ttu-id="b7ed0-134">Righe Acquisto</span><span class="sxs-lookup"><span data-stu-id="b7ed0-134">Purchase Line</span></span>
-   <span data-ttu-id="b7ed0-135">Righe registrazioni COGE</span><span class="sxs-lookup"><span data-stu-id="b7ed0-135">Gen. Journal Line</span></span>
-   <span data-ttu-id="b7ed0-136">Righe reg. magazzino</span><span class="sxs-lookup"><span data-stu-id="b7ed0-136">Item Journal Line</span></span>
-   <span data-ttu-id="b7ed0-137">Cat. reg. cliente</span><span class="sxs-lookup"><span data-stu-id="b7ed0-137">Customer Posting Group</span></span>
-   <span data-ttu-id="b7ed0-138">Cat. reg. fornitore</span><span class="sxs-lookup"><span data-stu-id="b7ed0-138">Vendor Posting Group</span></span>
-   <span data-ttu-id="b7ed0-139">Cat. reg. magazzino</span><span class="sxs-lookup"><span data-stu-id="b7ed0-139">Inventory Posting Group</span></span>
-   <span data-ttu-id="b7ed0-140">Unità di misura</span><span class="sxs-lookup"><span data-stu-id="b7ed0-140">Unit of Measure</span></span>
-   <span data-ttu-id="b7ed0-141">Cat. reg. business</span><span class="sxs-lookup"><span data-stu-id="b7ed0-141">Gen. Business Posting Group</span></span>
-   <span data-ttu-id="b7ed0-142">Cat. reg. articoli/servizi</span><span class="sxs-lookup"><span data-stu-id="b7ed0-142">Gen. Product Posting Group</span></span>
-   <span data-ttu-id="b7ed0-143">Setup registrazioni COGE</span><span class="sxs-lookup"><span data-stu-id="b7ed0-143">General Posting Setup</span></span>
-   <span data-ttu-id="b7ed0-144">Regioni</span><span class="sxs-lookup"><span data-stu-id="b7ed0-144">Territory</span></span>
-   <span data-ttu-id="b7ed0-145">Categorie articolo</span><span class="sxs-lookup"><span data-stu-id="b7ed0-145">Item Category</span></span>
-   <span data-ttu-id="b7ed0-146">Prezzo vendita</span><span class="sxs-lookup"><span data-stu-id="b7ed0-146">Sales Price</span></span>
-   <span data-ttu-id="b7ed0-147">Prezzo acquisto</span><span class="sxs-lookup"><span data-stu-id="b7ed0-147">Purchase Price</span></span>

## <a name="importing-customer-data"></a><span data-ttu-id="b7ed0-148">Importazione di dati dei clienti</span><span class="sxs-lookup"><span data-stu-id="b7ed0-148">Importing Customer Data</span></span>
<span data-ttu-id="b7ed0-149">Dopo che i dati dei clienti sono stati importati in Excel, vengono importati in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="b7ed0-149">After the customer data has been entered in Excel, you import the data into [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span> <span data-ttu-id="b7ed0-150">Nella finestra **Pacchetti di configurazione** importare i dati del file Excel. È possibile verificare che i dati siano coerenti con [!INCLUDE[d365fin](includes/d365fin_md.md)] prima di applicare il pacchetto.</span><span class="sxs-lookup"><span data-stu-id="b7ed0-150">In the **Configuration Packages** window, you import the data from the Excel file, and you can validate that the data is consistent with [!INCLUDE[d365fin](includes/d365fin_md.md)] before you apply the package.</span></span>

## <a name="see-also"></a><span data-ttu-id="b7ed0-151">Vedi anche</span><span class="sxs-lookup"><span data-stu-id="b7ed0-151">See Also</span></span>
[<span data-ttu-id="b7ed0-152">Importazione dei dati aziendali da altri sistemi contabili</span><span class="sxs-lookup"><span data-stu-id="b7ed0-152">Importing Business Data from Other Finance Systems</span></span>](upload-data.md)  
[<span data-ttu-id="b7ed0-153">Migrazione dei dati QuickBooks</span><span class="sxs-lookup"><span data-stu-id="b7ed0-153">QuickBooks Data Migration</span></span>](ui-extensions-quickbooks-data-migration.md)  
[<span data-ttu-id="b7ed0-154">Migrazione dei dati Dynamics GP</span><span class="sxs-lookup"><span data-stu-id="b7ed0-154">Dynamics GP Data Migration</span></span>](ui-extensions-dynamicsgp-data-migration.md)
