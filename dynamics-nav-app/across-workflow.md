---
title: Workflow
description: "È possibile impostare e utilizzare i workflow che collegano task di processi aziendali eseguiti da utenti diversi. I task di sistema, ad esempio la registrazione automatica, possono essere inclusi come passaggi nei flussi di lavoro e preceduti o seguiti da task degli utenti. La richiesta e la concessione dell'approvazione per creare nuovi record sono passaggi tipici del workflow."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: e1efc43df4e0676c8c8bd704c58458ab9398cbe1
ms.contentlocale: it-it
ms.lasthandoff: 10/16/2017

---
# <a name="workflow"></a>Workflow
È possibile impostare e utilizzare i workflow che collegano task di processi aziendali eseguiti da utenti diversi. I task di sistema, ad esempio la registrazione automatica, possono essere inclusi come passaggi nei flussi di lavoro e preceduti o seguiti da task degli utenti. La richiesta e la concessione dell'approvazione per creare nuovi record sono passaggi tipici del workflow.  

 Nella finestra **Workflow** creare un workflow elencando le fasi interessate nelle righe. Ogni fase consiste in un evento del flusso di lavoro, moderato dalle condizioni di evento, e in una risposta del flusso di lavoro, moderata dalle opzioni di risposta. È possibile definire le fasi del flusso di lavoro compilando i campi delle righe del flusso di lavoro in base a elenchi fissi di valori di evento e di risposta che rappresentano gli scenari supportati dal codice dell'applicazione.  

 La versione generica di [!INCLUDE[d365fin](includes/d365fin_md.md)] include una serie di workflow preconfigurati, rappresentati da modelli di workflow che si possono copiare per creare workflow. Il codice dei modelli di flusso di lavoro che vengono aggiunti da Microsoft hanno il prefisso "MS-". Per ulteriori informazioni, vedere l'elenco dei modelli di workflow nella finestra Modelli del workflow.  

 Se uno scenario aziendale richiede un evento o una risposta del flusso di lavoro non supportati, il partner Microsoft deve implementarli tramite la personalizzazione del codice dell'applicazione. Per ulteriori informazioni, vedere [Procedura dettagliata: Implementazione di nuovi eventi e risposte workflow](https://msdn.microsoft.com/en-us/library/mt574349.aspx) su MSDN.  

 Nella tabella seguente viene descritta una sequenza di task, con collegamenti agli argomenti che li descrivono.  

|**Task**|**Vedere**|  
|------------|-------------|  
|Impostare gli utenti del flusso di lavoro, specificare la modalità di notifica per gli utenti e creare nuovi flussi di lavoro. Per i nuovi flussi di lavoro per gli scenari non sostenuti, implementare gli elementi necessari del flusso di lavoro personalizzando il codice dell'applicazione.|[Impostazione dei workflow](across-set-up-workflows.md)|  
|Abilitare i flussi di lavoro, intervenire sulle relative notifiche, incluse le approvazioni di richieste, e approvare le richieste per eseguire un passaggio del flusso di lavoro. Archiviare ed eliminare i flussi di lavoro.|[Utilizzo dei workflow](across-use-workflows.md)|  

## <a name="see-also"></a>Vedi anche  
[Vendite](sales-manage-sales.md)  
[Acquisti](purchasing-manage-purchasing.md)  
[Gestione di progetti](projects-manage-projects.md)  
[Utilizzo di [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

