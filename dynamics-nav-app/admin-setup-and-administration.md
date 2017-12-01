---
title: Task amministrativi in Dynamics NAV
description: Alcuni task in [! INCLUDA] [d365fin (includes/d365fin_md.md)] richiedono un setup e un'amministrazione centrale. In questa sezione, viene fornita una descrizione di tali task e informazioni su come utilizzarli.
author: edupont04
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 09/01/2017
ms.author: edupont
ms.translationtype: HT
ms.sourcegitcommit: 1dfba8b14019991c95f40ffd5f7fbaed5df414eb
ms.openlocfilehash: 3ddb647d28a4065be248a265316b38e8d37d28c2
ms.contentlocale: it-it
ms.lasthandoff: 12/01/2017

---
# <a name="setup-and-administration-in-dynamics-nav"></a><span data-ttu-id="71e49-104">Impostazione e amministrazione in Dynamics NAV</span><span class="sxs-lookup"><span data-stu-id="71e49-104">Setup and Administration in Dynamics NAV</span></span>
<span data-ttu-id="71e49-105">I task di amministrazione centrale vengono generalmente eseguiti da un solo ruolo nella società.</span><span class="sxs-lookup"><span data-stu-id="71e49-105">Central administration tasks are usually performed by one role in the company.</span></span> <span data-ttu-id="71e49-106">L'ambito di tali task può dipendere dalle dimensioni dell'azienda e dalle responsabilità previste dalla mansione dell'amministratore.</span><span class="sxs-lookup"><span data-stu-id="71e49-106">The scope of these tasks can depend on the company's size and the administrator's job responsibilities.</span></span> <span data-ttu-id="71e49-107">Questi task possono includere la gestione della sincronizzazione con il database di code di processi ed e-mail, l'impostazione di utenti, la personalizzazione dell'interfaccia utente e la gestione delle chiavi di crittografia.</span><span class="sxs-lookup"><span data-stu-id="71e49-107">These tasks can include managing database synchronization of job and email queues, setting up users, customizing the user interface, and managing encryption keys.</span></span>  

<span data-ttu-id="71e49-108">Per la riuscita di qualsiasi nuovo software aziendale, è importante immettere i valori di setup appropriati dall'inizio.</span><span class="sxs-lookup"><span data-stu-id="71e49-108">Entering the correct setup values from the start is important to the success of any new business software.</span></span> [!INCLUDE[d365fin](includes/d365fin_md.md)]<span data-ttu-id="71e49-109"> include varie guide di setup per la configurazione dei dati principali.</span><span class="sxs-lookup"><span data-stu-id="71e49-109"> includes a number of setup guides that help you set up core data.</span></span> <span data-ttu-id="71e49-110">Per ulteriori informazioni, vedere [Impostazione di Dynamics NAV](setup.md).</span><span class="sxs-lookup"><span data-stu-id="71e49-110">For more information, see [Setting Up Dynamics NAV](setup.md).</span></span>

<!--Whether you use [!INCLUDE[rim](../../includes/rim_md.md)] to implement setup values or you manually enter them in the new company, you can support your setup decisions with some general recommendations for selected setup fields that are known to potentially cause the solution to be inefficient if defined incorrectly.-->  

<span data-ttu-id="71e49-111">Un utente o amministratore avanzato può impostare il framework di scambio di dati per consentire agli utenti di esportare e importare i dati nei file bancari e di ruolo paga, ad esempio per i diversi processi di gestione bancaria.</span><span class="sxs-lookup"><span data-stu-id="71e49-111">A super user or an administrator can set up the Data Exchange Framework to enable users to export and import data in bank and payroll files, for example for various cash management processes.</span></span>  

<span data-ttu-id="71e49-112">Nella tabella seguente viene descritta una sequenza di task, con collegamenti agli argomenti che li descrivono.</span><span class="sxs-lookup"><span data-stu-id="71e49-112">The following table describes a sequence of tasks, with links to the topics that describe them.</span></span>   

|<span data-ttu-id="71e49-113">**Per**</span><span class="sxs-lookup"><span data-stu-id="71e49-113">**To**</span></span>|<span data-ttu-id="71e49-114">**Vedere**</span><span class="sxs-lookup"><span data-stu-id="71e49-114">**See**</span></span>|  
|------------|-------------|  
|<span data-ttu-id="71e49-115">Aggiungere utenti, gestire i permessi e l'accesso ai dati, assegnare ruoli.</span><span class="sxs-lookup"><span data-stu-id="71e49-115">Add users, manage permissions and access to data, assign roles.</span></span>|[<span data-ttu-id="71e49-116">Utenti, profili e Gestioni ruolo utente in Dynamics NAV</span><span class="sxs-lookup"><span data-stu-id="71e49-116">Users, Profiles, and Role Centers in Dynamics NAV</span></span>](admin-users-profiles-roles.md)|  
|<span data-ttu-id="71e49-117">Tenere traccia di tutte le modifiche dirette apportate dagli utenti ai dati nel database per identificare l'origine di eventuali errori e delle modifiche ai dati.</span><span class="sxs-lookup"><span data-stu-id="71e49-117">Track all direct modifications that users make to data in the database to identify the origin of errors and data changes.</span></span>|[<span data-ttu-id="71e49-118">Registrazione di modifiche in Dynamics NAV</span><span class="sxs-lookup"><span data-stu-id="71e49-118">Logging Changes in Dynamics NAV</span></span>](across-log-changes.md)|  
|<span data-ttu-id="71e49-119">Supportare le decisioni di setup con alcuni consigli per i campi selezionati che potrebbero provocare la mancata efficacia della soluzione se definiti in modo errato</span><span class="sxs-lookup"><span data-stu-id="71e49-119">Support your setup decisions with recommendations for selected fields that are known to potentially cause the solution to be inefficient if set up incorrectly</span></span>|[<span data-ttu-id="71e49-120">Impostare aree di applicazione complesse utilizzando le procedure ottimali</span><span class="sxs-lookup"><span data-stu-id="71e49-120">Set Up Complex Application Areas Using Best Practices</span></span>](set-up-complex-application-areas-using-best-practices.md)|  
|<span data-ttu-id="71e49-121">Esporre le pagine, le codeunit e le query come servizi Web.</span><span class="sxs-lookup"><span data-stu-id="71e49-121">Expose pages, codeunits, and queries as web services.</span></span>|[<span data-ttu-id="71e49-122">Procedura: Pubblicare un servizio Web</span><span class="sxs-lookup"><span data-stu-id="71e49-122">How to: Publish a Web Service</span></span>](across-how-publish-web-service.md)|  
|<span data-ttu-id="71e49-123">Impostare un server SMTP per consentire la comunicazione e-mail in entrata e in uscita da Dynamics NAV.</span><span class="sxs-lookup"><span data-stu-id="71e49-123">Set up an SMTP server to enable e-mail communication in and out of Dynamics NAV</span></span>| [<span data-ttu-id="71e49-124">Procedura: Impostare la posta elettronica manualmente o tramite il setup assistito</span><span class="sxs-lookup"><span data-stu-id="71e49-124">How to: Set Up Email Manually or Using the Assisted Setup</span></span>](madeira-how-setup-email.md)|  
|<span data-ttu-id="71e49-125">Immettere richieste singole o ricorrenti per eseguire report o codeunit.</span><span class="sxs-lookup"><span data-stu-id="71e49-125">Enter single or recurring requests to run reports or codeunits.</span></span>|[<span data-ttu-id="71e49-126">Utilizzare le code processi per pianificare le attività</span><span class="sxs-lookup"><span data-stu-id="71e49-126">Use Job Queues to Schedule Tasks</span></span>](admin-job-queues-schedule-tasks.md)|  
|<span data-ttu-id="71e49-127">Gestire, eliminare o comprimere documenti</span><span class="sxs-lookup"><span data-stu-id="71e49-127">Manage, delete, or compress documents</span></span>|[<span data-ttu-id="71e49-128">Gestire i documenti</span><span class="sxs-lookup"><span data-stu-id="71e49-128">Manage Documents</span></span>](admin-manage-documents.md)|  

## <a name="see-also"></a><span data-ttu-id="71e49-129">Vedi anche</span><span class="sxs-lookup"><span data-stu-id="71e49-129">See Also</span></span>
[<span data-ttu-id="71e49-130">Panoramica sulle funzionalità aziendali</span><span class="sxs-lookup"><span data-stu-id="71e49-130">Overview of Business Functionality</span></span>](madeira-business-functionality.md)  
[<span data-ttu-id="71e49-131">Funzionalità aziendali generali</span><span class="sxs-lookup"><span data-stu-id="71e49-131">General Business Functionality</span></span>](ui-across-business-areas.md)  
<span data-ttu-id="71e49-132">[Utilizzo di [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="71e49-132">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  
<span data-ttu-id="71e49-133">[Benvenuto in [!INCLUDE[d365fin](includes/d365fin_md.md)]](index.md)</span><span class="sxs-lookup"><span data-stu-id="71e49-133">[Welcome to [!INCLUDE[d365fin](includes/d365fin_md.md)]](index.md)</span></span>  

