---
title: Panoramica delle impostazioni per gli articoli in assistenza e i componenti degli articoli in assistenza
description: Informazioni sulle impostazioni da eseguire prima di poter utilizzare gli articoli di assistenza, inclusi i valori di default, ad esempio il tempo di risposta, la percentuale di sconto contrattuale e il gruppo dei prezzi di assistenza.
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
ms.openlocfilehash: 0632bdc3b12e60c9b49893df748e8ca165c5b9d4
ms.contentlocale: it-it
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-set-up-service-items-and-service-item-components"></a>Procedura: Impostare gli articoli in assistenza e i componenti degli articoli in assistenza
Per utilizzare gli articoli in assistenza, è necessario impostare quanto segue

* Gruppi di articoli in assistenza 
* Facoltativo

## <a name="to-set-up-service-item-groups"></a>Per impostare gruppi di articoli in assistenza
È possibile impostare gruppi di articoli correlati tra loro in termini di riparazione e manutenzione. Per gli articoli in assistenza appartenenti a un gruppo di articoli in assistenza è possibile definire valori di default, ad esempio il tempo di risposta, la percentuale di sconto contrattuale e il gruppo dei prezzi di assistenza. Per gli articoli in un gruppo di articoli in assistenza è possibile specificare se al momento della vendita debbano essere automaticamente registrati come articoli in assistenza.  
  
I gruppi di articoli in assistenza vengono assegnati ad articoli nella scheda **Articolo** e ad articoli in assistenza nella scheda **Articolo in assistenza**.  
  
1. Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **Gruppi articoli in assistenza**, quindi scegliere il collegamento correlato.  
2. Creare un nuovo gruppo di articoli in assistenza.  
3. Compilare i campi **Codice** e **Descrizione**.  
4. Nel campo **% Sconto Contratto di Default** immettere la percentuale di sconto contrattuale predefinito che si intende assegnare agli articoli in assistenza appartenenti al gruppo.  
5. Nel campo **Cod. gruppo prezzi assist. di default** immettere il codice del gruppo di prezzi di assistenza di default che si intende assegnare agli articoli in assistenza appartenenti al gruppo.  
6. Nel campo **Tempo risp. di def.(ore)** immettere il tempo di risposta di default, espresso in ore, che si intende assegnare agli articoli in assistenza appartenenti al gruppo.  
7. Se si desidera che al momento della vendita gli articoli del gruppo vengano registrati come articoli in assistenza, selezionare il campo **Crea articolo in assistenza**.  

## <a name="to-set-up-service-item-components"></a>Per impostare i componenti degli articoli in assistenza
Un articolo in assistenza può essere composto da diversi componenti che possono essere sostituiti da pezzi di ricambio quando si presta assistenza al prodotto. Questi componenti vengono impostati nella pagina **Lista comp. artic. assist.** Inoltre, se si intende impostare dei componenti per gli articoli in assistenza rappresentati da distinte base, è possibile copiare gli articoli della distinta base e crearli come componenti dell'articolo in assistenza. 
  
1. Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **Articoli in assistenza**, quindi scegliere il collegamento correlato. 
2. Aprire l'articolo in assistenza per cui si desidera impostare i componenti.  
3. Scegliere l'azione **Componenti**. Verrà visualizzata la finestra **Lista comp. artic. assist.**.  
4. Aggiungere un nuovo componente  
5. Nel campo **Tipo** scegliere **Articolo in assistenza** se il componente stesso è un articolo in assistenza registrato. In caso contrario, selezionare **Articolo**.  
6. Nel campo **Nr.** scegliere l'articolo o l'articolo in assistenza che rappresenta un componente dell'articolo in assistenza.  

## <a name="to-set-up-service-item-components-from-a-bom"></a>Per impostare i componenti degli articoli in assistenza da una distinta base
1.  Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **Articoli in assistenza**, quindi scegliere il collegamento correlato.  
2. Aprire l'articolo in assistenza per cui si desidera impostare dei componenti da una distinta base.  
3. Scegliere l'azione **Componenti**. Verrà visualizzata la finestra **Lista comp. artic. assist.**.  
4. Scegliere l'azione **Copia da DBV**.  
  
    Se l'articolo a cui è collegato l'articolo in assistenza è una distinta base, verranno automaticamente creati componenti per tutti gli articoli nella distinta base.  

## <a name="to-set-up-a-service-shelf"></a>Per impostare uno scaffale di assistenza
È possibile impostare scaffali di assistenza che indicano dove memorizzare gli articoli di assistenza. Gli scaffali di assistenza vengono assegnati agli articoli in assistenza nelle pagine **Ordine assistenza** e **Prospetto art. in assist.**  
  
1. Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **Scaffali assistenza**, quindi scegliere il collegamento correlato.
2. Compilare i campi in base alle esigenze.

## <a name="see-also"></a>Vedi anche
[Procedura: Impostare codici per servizi standard](service-how-setup-service-coding.md)   
[Procedura: Impostare il troubleshooting:](service-how-setup-troubleshooting.md)
