---
title: Esporre oggetti come servizi Web
description: Pubblicare oggetti di [! INCLUDA] [d365fin (includes/d365fin_md.md)] come servizi Web per renderli immediatamente disponibili nella rete.
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
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 7c2bb65caeed819088382f811eb179eaeda35a7c
ms.contentlocale: it-it
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-publish-a-web-service"></a>Procedura: Pubblicare un servizio Web
I servizi Web sono un modo semplice ed efficace per rendere le funzionalità di applicazioni disponibili a vari sistemi e utenti esterni. [!INCLUDE[d365fin](includes/d365fin_md.md)] include vari oggetti che, per impostazione predefinita, vengono esposti come servizi Web in seguito all'integrazione in altri servizi Microsoft, ma è anche possibile aggiungere altri servizi Web.  

È possibile impostare un servizio Web nel client Windows o nel client Web. È necessario pubblicare il servizio Web per renderlo disponibile alle richieste di assistenza nella rete. Gli utenti possono individuare i servizi Web puntando un browser al percorso del server e richiedendo un elenco dei servizi disponibili. Quando si pubblica un servizio Web, diviene immediatamente disponibile in rete per gli utenti autenticati. Tutti gli utenti autorizzati possono accedere ai metadati per i servizi Web, ma solo gli utenti che dispongono di permessi sufficienti possono accedere ai dati effettivi.

## <a name="creating-and-publishing-a-web-service"></a>Creazione e pubblicazione di un servizio Web  
 I seguenti passaggi illustrano come creare e pubblicare un servizio Web.  

#### <a name="to-create-and-publish-a-web-service"></a>Per creare e pubblicare un servizio Web  

1.  Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **Servizi Web**, quindi scegliere il collegamento correlato.  

2.  Nella pagina **Servizi Web** selezionare **Nuovo**. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  

    > [!NOTE]  
    >  **Codeunit** e **Pagina** sono tipi validi per servizi Web SOAP. **Pagina** e **Query** sono tipi validi per i servizi Web OData.  
    Inoltre, se il database contiene più società, è possibile scegliere un ID oggetto specifico di una delle società.  
    Il nome del servizio è visibile agli utenti del servizio Web e poiché è la base per l'identificazione e la distinzione dei servizi Web, è importante che sia un nome significativo.

3.  Selezionare la casella di controllo nella colonna **Pubblicato**.  

     Quando si pubblica il servizio Web, nei campi **URL OData** e **URL SOAP** è possibile vedere gli URL che sono generati per il servizio Web. È possibile verificare il servizio web immediatamente selezionando i collegamenti nei campi **URL SOAP** e **URL OData**. In alternativa, è possibile copiare il valore del campo e salvarlo per un successivo utilizzo.  

Dopo la pubblicazione di un servizio Web, questo è immediatamente disponibile per le parti esterne. È possibile verificare la disponibilità del servizio Web utilizzando un browser, oppure è possibile scegliere il collegamento nei campi **URL SOAP** e **URL OData** nella finestra **Servizi Web**. La procedura seguente illustra come verificare la disponibilità del servizio Web per un uso successivo.  

#### <a name="to-verify-the-availability-of-a-web-service"></a>Per verificare la disponibilità di un servizio Web  

1.  Nel browser immettere l'URL pertinente. Nella seguente tabella sono illustrati i tipi di URL che è possibile immettere. Per i servizi Web SOAP, utilizzare il seguente formato per l'URI.  

    <table>
    <tr>
    <th>Tipo di servizio Web</th>
    <th>Sintassi</th>
    <th>Esempio</th>
    </tr>
    <tr>
    <td>SOAP</td>
    <td>https://*Server*:*SOAPWebServicePort*/*ServerInstance*/WS/*CompanyName*/salesDocuments/</td>
    <td>https://mycompany.financials.dynamics.com:7047/MS/WS/MyCompany/Page/salesDocuments?tenant=mycompany.financials.dynamics.com</td>
    </tr>
    <tr>
    <td>OData</td>
    <td>https://*Server*:*ODataWebServicePort*/*ServerInstance*/OData/Company('*CompanyName*')</td>
    <td>https://MyCompany.financials.dynamics.com:7048/MS/OData/Company('MyCompany')/salesDocuments?tenant=MyCompany.financials.dynamics.com

         The company name is case-sensitive.</td>
    </tr>
    </table>

2.  Esaminare le informazioni visualizzate nel browser. Verificare che sia possibile visualizzare il nome del servizio Web creato.  

 Quando si accede a un servizio Web e si desidera scrivere i dati di nuovo in [!INCLUDE[d365fin](includes/d365fin_md.md)], è necessario specificare il nome della società. È possibile specificare la società come parte di URI come illustrato negli esempi, oppure è possibile specificare la società come parte dei parametri di query. Ad esempio, gli URI successivi scelgono lo stesso servizio Web OData e sono entrambi URI validi.  

```  
https://localhost:7048/server/OData/Company('CRONUS International Ltd.')/Customer  
```  

```  
https://localhost:7048/server/OData/Customer?company='CRONUS International Ltd.'  
```  

## <a name="see-also"></a>Vedi anche  
[Impostazione e amministrazione in Dynamics NAV](admin-setup-and-administration.md)  

