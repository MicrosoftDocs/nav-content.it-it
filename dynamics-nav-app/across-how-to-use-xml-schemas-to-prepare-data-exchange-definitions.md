---
title: Creare oggetti XMLport basati su schemi XML
description: Utilizzare gli schemi XML per impostare il framework del servizio di scambio documenti.
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/21/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: b9b1f062ee6009f34698ea2cf33bc25bdd5b11e4
ms.openlocfilehash: 607d51d929e019662fdc4e17f7bbb064f806f32a
ms.contentlocale: it-it
ms.lasthandoff: 10/23/2017

---
# <a name="how-to-use-xml-schemas-to-prepare-data-exchange-definitions"></a>Procedura: Utilizzare gli schemi XML per preparare le definizioni di scambio di dati
Per abilitare l'importazione/esportazione di dati in file XML attraverso il framework di scambio dati in [!INCLUDE[d365fin](includes/d365fin_md.md)], è possibile usare gli schemi XML per definire quali elementi di dati si desidera scambiare con [!INCLUDE[d365fin](includes/d365fin_md.md)]. È possibile effettuare questa attività nella finestra **Visualizzatore schema XML** caricando il file di schema XML, selezionando gli elementi dati pertinenti e quindi inizializzando una definizione di scambio dati o un oggetto XMLport.  

 Dopo avere definito gli elementi dati da includere in base allo schema XML, è possibile utilizzare l'azione **Genera XMLport** per creare l'oggetto XMLport.  

 In alternativa, è possibile utilizzare l'azione **Genera definizione scambio dati** per inizializzare una definizione di scambio di dati in base agli elementi dati selezionati, che poi può essere completata nella struttura di scambio di dati. Viene creato un record nella finestra **Registrazione definizioni di scambio** dove si continua il processo definendo il mapping tra gli elementi del file e i campi in [!INCLUDE[d365fin](includes/d365fin_md.md)]. Per ulteriori informazioni, vedere [Procedura: Impostare le definizioni di scambio di dati](across-how-to-set-up-data-exchange-definitions.md).  

 In questo argomento sono contenute le seguenti procedure:  

-   Per caricare un file di schema XML  

-   Per selezionare o rimuovere i nodi in uno schema XML  

-   Per generare una definizione di scambio di dati basata su uno schema XML  

-   Per generare un oggetto XMLport per il file basato su uno schema XML  

-   Per importare un oggetto XMLport in Object Designer  

### <a name="to-load-an-xml-schema-file"></a>Per caricare un file di schema XML  

1.  Assicurarsi che il file schema XML pertinente sia disponibile. L'estensione del file è .xsd.  

2.  Nella casella **Cerca** immettere **Schemi XML**, quindi selezionare il collegamento correlato.  

3.  Nel gruppo **Nuovo** della scheda **Pagina iniziale** scegliere **Nuovo**.  

4.  Compilare i campi come indicato nella tabella seguente.  

    |Campo|Description|  
    |---------------------------------|---------------------------------------|  
    |**Codice**|Specificare un codice per identificare lo Schema XML.|  
    |**Description**|Specificare una descrizione dello Schema XML.|  

     Il campo **Spazio dei nomi di destinazione** specifica lo spazio dei nomi nel file schema XML che è stato caricato dalla riga.  

5.  Nel gruppo **Processo** della scheda **Pagina iniziale** scegliere **Carica schema**, quindi selezionare il file di schema XML.  

     Quando il file viene caricato, i campi rimanenti nella riga vengono compilati con informazioni provenienti dal file e viene selezionata la casella di controllo **Schema caricato**.  

    > [!NOTE]  
    >  La struttura ad albero dello schema XML caricato è compressa per impostazione predefinita. Ogni nodo può essere espanso scegliendo il pulsante **+** accanto al nodo desiderato. Per espandere tutti i nodi, selezionare **Espandi tutto** nella barra multifunzione.  

### <a name="to-select-or-clear-nodes-in-an-xml-schema"></a>Per selezionare o rimuovere i nodi in uno schema XML  

1.  Nella casella **Cerca** immettere **Visualizzatore schema XML**, quindi selezionare il collegamento correlato.  

2.  Compilare i campi nell'intestazione come descritto nella tabella riportata di seguito.  

    |Campo|Description|  
    |---------------------------------|---------------------------------------|  
    |**Codice schema XML**|Specificare il file schema XML che è stato caricato nel passaggio 5 nella sezione "Per caricare un file schema XML".|  
    |**Nuovo nr. XMLport**|Specificare il numero dell'oggetto XMLport che viene creato da questo schema XML quando si sceglie l'azione **Genera XMLPort**.|  

     Le righe sono ora compilate con nodi che rappresentano tutti gli elementi nello Schema XML. I nodi per gli elementi obbligatori secondo lo Schema XML vengono selezionati per impostazione predefinita.  

3.  Nella prima riga, nella colonna **Nome nodo**, espandere il nodo **Documento**, quindi espandere gradualmente i nodi sottostanti che si desidera esaminare.  

     In alternativa, fare clic con il pulsante destro del mouse su un nodo, quindi selezionare **Espandi tutto**.  

4.  Nella scheda **Pagina iniziale**, nel gruppo **Visualizzazione**, scegliere una delle seguenti azioni per modificare i nodi che sono visualizzati.  

    |**Azione**|Description|  
    |----------------|---------------------------------------|  
    |**Mostra tutto**|Tutti i nodi vengono visualizzati.|  
    |**Nascondi voci non obbligatorie**|Solo i nodi che rappresentano gli articoli richiesti in base allo schema XML vengono visualizzati. Questi nodi sono in genere indicati da un **1** nel campo **MinOccurs**.<br /><br /> Selezionare **Mostra tutto** per stornare la visualizzazione.|  
    |**Nascondi voci non selezionate**|Solo i nodi in cui la casella di controllo **Selezionato** è selezionata vengono visualizzati.<br /><br /> Selezionare **Mostra tutto** per stornare la visualizzazione.|  

5.  Nel gruppo **Gestisci** della scheda **Pagina iniziale** scegliere **Modifica**.  

6.  Con la casella di controllo **Selezionato** specificare per ciascun nodo se si desidera che l'elemento sia supportato nella definizione di scambio dati per il file della banca SEPA correlato.  

    > [!NOTE]  
    >  Quando si seleziona un nodo figlio obbligatorio, vengono selezionati anche tutti i relativi nodi padre.  

7.  Selezionare l'azione **Seleziona tutti gli elementi obbligatori** per selezionare nuovamente tutti i nodi che rappresentano gli elementi che sono richiesti in base allo Schema XML.  

8.  Selezionare l'azione **Deseleziona tutto** per annullare eventuali selezionare.  

     Il campo **Scelta** specifica che il nodo dispone di due o più nodi di pari livello che fungono da opzioni.  

### <a name="to-generate-a-data-exchange-definition-that-is-based-on-an-xml-schema"></a>Per generare una definizione di scambio di dati basata su uno schema XML  

1. Nella casella **Cerca** immettere **Schemi XML**, quindi selezionare il collegamento correlato.  

2. Selezionare lo schema XML pertinente, quindi, nella scheda **Pagina iniziale**, nel gruppo **Processo**, scegliere **Apri visualizzatore schema XML**.  

3. Assicurarsi che i nodi pertinenti siano selezionati. Per ulteriori informazioni, vedere la sezione "Per selezionare o rimuovere i nodi in uno schema XML".  

4. Nella finestra **Visualizzatore schema XML**, nella scheda **Pagina iniziale**, nel gruppo **Processo** scegliere **Genera definizione scambio dati**.  

   Verrà creata una definizione di scambio dati nella finestra **Registrazione definizioni di scambio** che si potrà completare specificando gli elementi del file da mappare con i campi in [!INCLUDE[d365fin](includes/d365fin_md.md)]. Per ulteriori informazioni, vedere [Procedura: Impostare le definizioni di scambio di dati](across-how-to-set-up-data-exchange-definitions.md).  

> [!NOTE]  
>  È inoltre possibile utilizzare la funzione **Ottieni struttura file** della finestra **Registrazione definizioni di scambio** che utilizza la funzionalità della finestra **Visualizzatore schema XML** per precompilare la Scheda dettaglio **Definizioni colonne**.  

### <a name="to-generate-an-xmlport-that-is-based-on-an-xml-schema"></a>Per generare un oggetto XMLport basato su uno schema XML  

1.  Nella casella **Cerca** immettere **Schemi XML**, quindi selezionare il collegamento correlato.  

2.  Selezionare lo schema XML pertinente, quindi, nella scheda **Pagina iniziale**, nel gruppo **Processo**, scegliere **Apri visualizzatore schema XML**.  

3.  Nel campo **Nuovo nr. XMLport** specificare il numero che il nuovo oggetto XMLport riceverà quando sarà generato.  

4.  Assicurarsi che i nodi pertinenti siano selezionati. Per ulteriori informazioni, vedere la sezione "Per selezionare o rimuovere i nodi in uno schema XML".  

5.  Nella scheda **Pagina iniziale**, nel gruppo **Processo**, scegliere **Genera XMLPort**, quindi salvare l'oggetto come file con estensione TXT nel percorso appropriato.  

6. Importare il nuovo oggetto XMLport nell'ambiente di sviluppo di [!INCLUDE[d365fin](includes/d365fin_md.md)] e compilarlo.

## <a name="see-also"></a>Vedi anche  
[Procedura: Impostare le definizioni di scambio di dati](across-how-to-set-up-data-exchange-definitions.md)   
[Procedura: esportare pagamenti in un file della banca](payables-how-export-payments-bank-file.md)   
[Riscuotere pagamenti con addebito diretto SEPA](finance-collect-payments-with-sepa-direct-debit.md)   
[Informazioni sul framework di scambio dati](across-about-the-data-exchange-framework.md)

