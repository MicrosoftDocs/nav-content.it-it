---
title: Creare e modificare layout personalizzati per report e documenti
description: "Informazioni su come creare i layout personalizzati che consentono di modificare l'aspetto del report quando è visualizzato, stampato o salvato."
documentationcenter: 
author: jswymer
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: customized report, document layout, logo, personalize
ms.date: 03/29/2017
ms.author: jswymer
ms.translationtype: HT
ms.sourcegitcommit: b9b1f062ee6009f34698ea2cf33bc25bdd5b11e4
ms.openlocfilehash: ee614c44a17873591916bc97bd9b2a3f33fce21b
ms.contentlocale: it-it
ms.lasthandoff: 10/23/2017

---
# <a name="how-to-create-and-modify-a-custom-report-or-document-layout"></a>Procedura: Creare e modificare un layout di documento o report personalizzato
Per impostazione predefinita, un report avrà un layout di report RDLC o Word predefinito o entrambi. Non è possibile modificare i layout predefiniti. Tuttavia, è possibile creare i propri layout personalizzati che consentono di modificare l'aspetto del report quando è visualizzato, stampato o salvato. È possibile creare più layout di report personalizzati per lo stesso report e alternare il layout utilizzato in un report in base alle esigenze.

> [!NOTE]  
>   In [!INCLUDE[d365fin](includes/d365fin_md.md)], il termine "report" riguarda anche i documenti esterni, quali fatture di vendita e conferme di ordini inviate a clienti come file PDF.

Per creare un layout personalizzato, è possibile effettuare una copia di un layout personalizzato esistente o aggiungere un nuovo layout personalizzato, che nella maggior parte dei casi è basato su un layout predefinito. Quando si aggiunge un nuovo layout personalizzato, è possibile scegliere di aggiungere un tipo di layout di report RDLC o Word oppure entrambi. Il nuovo layout personalizzato si baserà automaticamente sul layout predefinito per il report, se ce n'è uno disponibile. Se non è presente un layout predefinito per il tipo, viene creato un nuovo layout vuoto che si dovrà progettare e modificare da zero. Per ulteriori informazioni sui layout di report RDLC e Word, sui layout personalizzati integrati e altro ancora, vedere [Gestire i layout dei report](ui-manage-report-layouts.md).  

## <a name="to-create-a-custom-layout"></a>Per creare un layout personalizzato
1. Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **Selezione layout report**, quindi scegliere il collegamento correlato.  

    Nella finestra **Selezione layout report** sono elencati tutti i report disponibili nella società che è specificata nel campo **Società** nella parte superiore della finestra.
2. Impostare il campo **Società** alla società per la quale si desidera creare il layout di report.
3. Selezionare la riga per il report per il quale si desidera creare il layout, quindi scegliere l'azione **Layout personalizzati**.  
   Viene visualizzata la finestra **Layout report personalizzati** nella quale sono elencati tutti i layout personalizzati che sono disponibili per il report selezionato.
4. Per creare una copia di un layout personalizzato esistente, selezionare il layout personalizzato esistente nell'elenco, quindi scegliere l'azione **Copia**.  
   La copia del layout personalizzato viene visualizzata nella finestra **Layout report personalizzati** e nel campo *Descrizione* è presente la dicitura **Copia di**.
5. Se si desidera aggiungere un nuovo layout personalizzato basato su un layout predefinito, attenersi alla seguente procedura:  
   1. Scegliere l'azione **Nuovo**. Viene visualizzata la finestra **Inserisci layout predefinito per un report**. I campi **ID** e **Nome** vengono automaticamente compilati.
   2. Per aggiungere un tipo di layout di report Word personalizzato, selezionare la casella di controllo **Inserisci layout Word**.
   3. Per aggiungere un tipo di layout di report RDLC personalizzato, selezionare la casella di controllo **Inserisci layout RDLC**.
   4. Scegliere il pulsante **OK**.  
      I nuovi layout personalizzati vengono visualizzati nella finestra **Layout report personalizzati**. Se un nuovo layout è basato su un layout predefinito, contiene le parole **Copia di un layout predefinito** nel campo **Descrizione**. Se non è disponibile alcun layout predefinito per il report, il nuovo layout presenta la dicitura **Nuovo layout** nel campo **Descrizione**. Questa dicitura indica che il layout personalizzato è vuoto.
6. Per impostazione predefinita, il campo **Nome società** è vuoto, il che significa che il layout personalizzato sarà disponibile per il report in tutte le società. Per rendere il layout personalizzato disponibile solo a una società specifica, scegliere **Modifica**, quindi impostare il campo **Nome società** sulla società desiderata.

Il layout personalizzato è stato creato. È ora possibile modificare il layout personalizzato in base alle esigenze.

## <a name="ModifyCustomLayout"></a>Modifica di un layout personalizzato
Per modificare un layout di report, è necessario innanzi tutto esportare il layout come file nel computer o in una rete, quindi aprire il documento esportato e apportare le modifiche. Quando sono state apportate tutte le modifiche, importare il layout di report.

### <a name="to-modify-a-custom-layout"></a>Per modificare un layout personalizzato
1.  Esportare un layout personalizzato dalla finestra **Layout report personalizzati**. Se questa finestra non è già aperta, cercare e aprire la finestra **Selezione layout report**, selezionare il report che ha il layout da modificare, quindi scegliere l'azione **Layout personalizzati**.  
2.  Nella finestra **Layout report personalizzati**, selezionare il layout che si desidera modificare, scegliere l'azione **Esporta layout** e quindi scegliere **Salva** o **Salva con nome** per salvare il documento di layout nel computer o in una rete.  

3.  Aprire il documento di layout di report appena salvato, quindi apportare le modifiche.

      Se si modifica un layout Word, aprire il documento di layout in Word. Per informazioni dettagliate sulle operazioni di modifica, vedere la sezione successiva [Modifica di un layout di report](ui-how-create-custom-report-layout.md#MakeChangesToLayout).

      I layout di report RDLC sono più avanzati dei layout di report Word. Per ulteriori informazioni su come modificare un layout di report RDLC, vedere [Progettazione di layout di report RDLC](https://msdn.microsoft.com/en-us/dynamics-nav/designing-rdlc-report-layouts).

      Ricordarsi di salvare le modifiche effettuate.

4.  Tornare alla finestra **Layout report personalizzati**, selezionare il layout di report esportato e modificato, quindi scegliere l'azione **Importa layout**.  

5. Nella finestra di dialogo **Importa**, selezionare **Scegli** per trovare e selezionare il documento di layout di report e scegliere **Apri**.

##  <a name="MakeChangesToLayout"></a>Modifica di un layout di report Word  
Per apportare modifiche al layout e di formattazione generali, ad esempio modificare il carattere del testo, aggiungere o modificare una tabella o rimuovere un campo dati, utilizzare le funzionalità di modifica di base di Word, come si fa con qualsiasi documento di Word.

Se si sta progettando un layout di report Word da zero o aggiungendo nuovi campi dati, iniziare aggiungendo una tabella che include le righe e le colonne che utilizzeranno i campi dati.

> [!TIP]  
>  Mostra le linee delle griglie della tabella in modo da visualizzare i limiti delle celle della tabella. Ricordarsi di nascondere le linee delle griglie quando si finisce di apportare modifiche. Per visualizzare o nascondere le linee delle griglie della tabella, selezionare la tabella e quindi in **Layout** nella scheda **Tabella** scegliere **Visualizza linee griglia**.  

###  <a name="RemoveField"></a> Rimuovere i campi etichetta e dati dai layout Word  
 I campi etichetta e dati di un report sono contenuti nei controlli contenuto di Word. La figura seguente illustra un controllo contenuto quando è selezionato nel documento Word.  

 ![Controllo contenuto per il campo nel layout di report Word](media/nav_wordreportlayouts_contentcontrol.png "NAV_WordReportLayouts_ContentControl")  

 Il nome del campo etichetta o dati viene visualizzato nel controllo contenuto. Nell'esempio, il nome del campo è CompanyAddr1.  

### <a name="to-remove-a-label-or-data-field"></a>Per rimuovere un campo dati o etichetta  

1.  Fare clic con il tasto destro del mouse sul campo che si desidera eliminare, quindi scegliere **Rimuovi controllo contenuto**.  

     Il controllo campo viene rimosso, ma rimane il nome del campo come testo.  

2.  Eliminare il testo residuo in base alle esigenze.  

### <a name="adding-data-fields"></a>Aggiunta di campi dati
L'aggiunta di campi dati dal set di dati di un report è una funzione più avanzata e richiede la conoscenza del set di dati del report. Per informazioni sull'aggiunta di campi per dati, etichette, dati e immagini, vedere [Procedura: Aggiungere campi a un layout di report Word](ui-how-add-fields-word-report-layout.md).  


## <a name="see-also"></a>Vedi anche
[Gestione dei layout di report](ui-manage-report-layouts.md)  
[Procedura: Modificare il layout attualmente utilizzato in un report](ui-how-change-layout-currently-used-report.md)  
[Procedura: Importare ed esportare un layout di report o documento personalizzato](ui-how-import-and-export-report-layout.md)  
[Utilizzo dei report](ui-work-report.md)  
[Utilizzo di [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)  

