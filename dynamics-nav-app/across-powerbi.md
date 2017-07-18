---
title: Utilizzo del pacchetto di contenuti Dynamics NAV per Power BI
author: edupont04
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: 6351e4819a2f3665cc561b5b1f868eea5d435f75
ms.contentlocale: it-it
ms.lasthandoff: 06/26/2017

---

# <a name="using-the-dynamics-nav-content-pack-for-power-bi"></a>Utilizzo del pacchetto di contenuti Dynamics NAV per Power BI
Ottenere informazioni approfondite sui dati di Dynamics NAV è semplice con Power BI e con il pacchetto di contenuti Dynamics NAV. Power BI recupera i dati e quindi sviluppa un dashboard e i report pronti per l'uso basati su tali dati.  

Il pacchetto di contenuti è preconfigurato per utilizzare i dati di vendita e i dati finanziari della società demo che si crea quando ci si sottoscrive per l'anteprima di Dynamics NAV.  

- Selezionare qualsiasi visualizzazione sul dashboard per portare in primo piano uno dei sette report sottostanti.  
- Filtrare il report o aggiungere i campi che si desidera monitorare.  
- Aggiungere la visualizzazione personalizzata al dashboard per continuare la tracciabilità.  
Dashboard e report sottostanti vengono aggiornati ogni giorno. È possibile controllare la pianificazione aggiornata e modificare la frequenza del set di dati.  

## <a name="accessing-dynamics-nav-in-power-bi"></a>Accedere a Dynamics NAV in Power BI
Per visualizzare i dati di Dynamics NAV in Power BI, è necessario disporre di quanto segue:  

- Accedere a Dynamics NAV. Per ulteriori informazioni, vedere [Dynamics NAV](http://go.microsoft.com/fwlink/?LinkID=759714).  
- Accesso a Power BI. Per ulteriori informazioni, vedere [Power BI](https://powerbi.microsoft.com).

Nel sito di Power BI è possibile trovare informazioni aggiuntive su come [aggiungere il pacchetto di contenuti Dynamics NAV a Power BI](http://go.microsoft.com/fwlink/?LinkID=760850).  

Per accedere al pacchetto di contenuti Dynamics NAV in Power BI, nella finestra di connessione, è necessario specificare le seguenti informazioni:

| Campo       | Descrizione              |
|-------------|--------------------------|
|**URL Feed OData**|L'URL OData in modo che Power BI possa accedere ai dati della società, come https://mybusiness.com:7048/MS/OData/Company('CRONUS%20US').|
|**Metodo di autenticazione**|Selezionare **Di base**.|
|**Nome utente**|L'account di posta elettronica utilizzato per effettuare l'accesso a Dynamics NAV, ad esempio *me@mybusiness.com*.|
|**Password**|Questa è la chiave di accesso al servizio Web per il proprio account utente in Dynamics NAV.|

Ciò significa che è necessario ottenere due informazioni da Dynamics NAV: l'URL OData e la chiave di accesso al servizio Web per il proprio account utente.  
**Ottenere l'URL**  
Quando si aggiunge Dynamics NAV a Power BI, è necessario specificare un URL in modo che Power BI possa accedere ai dati dalla società. Nella finestra di connessione, l'URL è denominato **URL Feed OData** e deve avere il seguente formato:

         https://mybusiness.projectmadeira.com:7048/MS/OData/Company('CRONUS%20US')  
In questo esempio, *mybusiness* il nome del servizio Dynamics NAV e *CRONUS US* è il nome della società demo in cui *%20* rappresenta lo spazio nel nome.   
Per ottenere l'URL, in Dynamics NAV cercare ed aprire la finestra **Servizi Web**. In questa finestra viene visualizzato un elenco dei servizi Web attualmente disponibili ed è possibile copiare il collegamento dal campo **OData URL** per uno dei servizi Web predefiniti di OData.  
**Ottenere la chiave di accesso al servizio Web**  
Per utilizzare i dati di Dynamics NAV, in Power BI, nella finestra **Collega a Dynamics NAV**, è necessario specificare il nome utente, ovvero il proprio account di posta elettronica e una password. La password è la chiave di accesso al servizio Web impostata per il proprio account utente in Dynamics NAV.  
Per ottenere una chiave di accesso al servizio Web, in Dynamics NAV, cercare la finestra **Utenti** quindi aprire la scheda per il proprio account utente. Nella Scheda dettaglio **Accesso al servizio Web**, copiare il contenuto del campo **Chiave di accesso al servizio Web**. Se il campo è vuoto, nella barra multifunzione, selezionare **Modifica chiave di accesso al servizio Web**, selezionare il campo **La chiave non scade mai** e quindi fare clic sul pulsante OK. È quindi possibile copiare la chiave.  

## <a name="getting-data-from-dynamics-nav"></a>Acquisizione dei dati da Dynamics NAV
Il dashboard di Dynamics NAV mostra i report tipici che più opportuno utilizzare per tenere traccia delle attività. I dati vengono estratti dalla società di Dynamics NAV utilizzando i servizi Web per la lettura dei dati live. Nella finestra **Servizi Web** di Dynamics NAV, vengono elencati i servizi Web che sono stati impostati per l'utente, incluse le seguenti operazioni utilizzate dal pacchetto di contenuto in Power BI:  

- ItemSalesAndProfit  
- ItemSalesByCustomer  
- powerbifinance-setup  
- SalesDashboard  
- SalesOpportunities  
- SalesOrdersBySalesPerson  
- TopCustomerOverview  

**Nota**: se si modifica il nome di uno qualsiasi dei servizi Web, i dati non verranno mostrati in Power BI.  
Se si desidera aggiungere altri dati in Power BI, è necessario trovare le tabelle in Dynamics NAV, esporle come servizi Web e aggiungerle al pacchetto di contenuto. Questo è uno scenario avanzato e è consigliabile iniziare con i dati che sono già disponibili in Power BI.  

## <a name="troubleshooting"></a>Troubleshooting
Il dashboard di Power BI si basa sui servizi Web rilasciati che sono elencati sopra e visualizza i dati della società demo o della società dell'utente se si importano i dati della soluzione finanziaria-di setup corrente. Tuttavia, se si verifica un errore, in questa sezione viene fornita una soluzione alternativa per i problemi più comuni.  

**"La convalida dei parametri non è riuscita. Assicurarsi che tutti i parametri siano validi"**  
Se l'errore viene visualizzato dopo l'accesso all'URL di Dynamics NAV, assicurarsi che i seguenti requisiti vengano soddisfatti:  

- l'URL segue esattamente questo modello:

    https://mybusiness.projectmadeira.com:7048/MS/OData/Company('CRONUS%20US')  
- Eliminare qualsiasi testo dopo il nome della società tra parentesi  
- Assicurarsi che non vi sia una barra finale alla fine dell'URL.  
- Assicurarsi che sia una connessione sicura come indicato dall'URL che inizia con *https*.  


**"Accesso non riuscito"**  
Se viene visualizzato un errore di "accesso non riuscito" quando si accede al dashboard con le credenziali di Dynamics NAV, questo potrebbe essere causato da uno dei seguenti problemi:

* L'account che si sta utilizzando non dispone delle autorizzazioni di lettura per i dati di Dynamics NAV da tale account.

    Verificare il proprio account utente in Dynamics NAV e assicurarsi che sia stata utilizzata la chiave di accesso al servizio Web corretta come password, quindi riprovare.  
* L'istanza di Dynamics NAV a cui ci si sta provando a connettere non dispone di un certificato SSL valido. In questo caso verrà visualizzato un messaggio di errore più dettagliato ("impossibile stabilire una relazione SSL attendibile").

    **Nota**: non sono supportati i certificati autofirmati.  


**"Oops"**  
Se viene visualizzata una finestra di dialogo "Oops" dopo aver superato la finestra di dialogo di autenticazione, nei casi più frequenti questo errore è causato da un problema di connessione ai dati del pacchetto di contenuto.

* Verificare che l'URL corrisponda al modello che è stato specificato in precedenza:

    https://mybusiness.projectmadeira.com:7048/MS/OData/Company('CRONUS%20US')  
* Un errore comune consiste nello specificare l'URL completo per un servizio Web specifico:

    https://mybusiness.projectmadeira.com:7048/MS/OData/Company('CRONUS%20US')/powerbifinance-setup  
* Oppure è possibile che si sia stato dimenticato di specificare il nome della società:

    https://mybusiness.projectmadeira.com:7048/MS/OData/  


## <a name="see-also"></a>Vedi anche
[Benvenuto in Dynamics NAV](across-get-started.md)  

