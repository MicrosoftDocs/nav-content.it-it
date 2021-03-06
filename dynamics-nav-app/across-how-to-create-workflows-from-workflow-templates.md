---
title: Come creare flussi di lavoro da modelli di flusso di lavoro
description: "Per risparmiare tempo durante la creazione di nuovi workflow, è possibile creare i workflow da modelli di workflow."
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
ms.openlocfilehash: b0c2143b85a7301711498ecd40d6f6685be17eda
ms.contentlocale: it-it
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-create-workflows-from-workflow-templates"></a>Procedura: Creare flussi di lavoro da modelli di flusso di lavoro
Per risparmiare tempo durante la creazione di nuovi workflow, è possibile creare i workflow da modelli di workflow.  

 I modelli di workflow sono flussi di lavoro non modificabili presenti nella versione generica di [!INCLUDE[d365fin](includes/d365fin_md.md)]. Il codice dei modelli di flusso di lavoro che vengono aggiunti da Microsoft hanno il prefisso "MS-".  

 Un altro modo per creare rapidamente un workflow consiste nell'importare un workflow esistente disponibile in un file all'esterno di [!INCLUDE[d365fin](includes/d365fin_md.md)]. Per ulteriori informazioni, vedere [Procedura: Esportare e importare workflow](across-how-to-export-and-import-workflows.md).  

Nella finestra **Workflow** creare un workflow elencando le fasi interessate nelle righe. Ogni fase consiste in un evento del flusso di lavoro, moderato dalle condizioni di evento, e in una risposta del flusso di lavoro, moderata dalle opzioni di risposta. È possibile definire le fasi workflow compilando i campi delle righe del workflow in base a elenchi fissi di valori di evento e di risposta che rappresentano gli scenari supportati dal codice dell'applicazione. Per ulteriori informazioni, vedere [Procedura: Creare workflow](across-how-to-create-workflows.md).  

## <a name="to-create-a-workflow-from-workflow-template"></a>Per creare un flusso di lavoro da un modello di flusso di lavoro  
1.  Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **Workflow** e quindi scegliere il collegamento correlato.  
2.  Scegliere l'azione **Crea flusso di lavoro da modello**. Verrà aperta la finestra **Modelli del workflow**.  
3.  Selezionare un modello di flusso di lavoro e scegliere il pulsante **OK**.  

     Verrà visualizzata la finestra **Workflow** per un nuovo workflow contenente tutte le informazioni del modello selezionato. Il valore nel campo **Codice** ad esempio con "-01" per indicare che questo è il primo workflow che viene creato dal modello di workflow.  
4.  Continuare la creazione del flusso di lavoro modificando i passaggi del flusso di lavoro o aggiungendone di nuovi. Per ulteriori informazioni, vedere [Procedura: Creare workflow](across-how-to-create-workflows.md).  

## <a name="see-also"></a>Vedi anche  
 [Procedura: Creare workflow](across-how-to-create-workflows.md)   
 [Procedura: Esportare e importare workflow](across-how-to-export-and-import-workflows.md)   
 [Procedura: Visualizzare le istanze di fasi workflow archiviate](across-how-to-view-archived-workflow-step-instances.md)   
 [Procedura: Eliminare i workflow](across-how-to-delete-workflows.md)   
 [Procedura dettagliata: Impostazione e utilizzo di un workflow di approvazione di acquisto](walkthrough-setting-up-and-using-a-purchase-approval-workflow.md)   
 [Impostazione dei workflow](across-set-up-workflows.md)   
 [Utilizzo dei workflow](across-use-workflows.md)   
 [Workflow](across-workflow.md)   

