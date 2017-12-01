---
title: 'Procedura: Registrare Dynamics NAV nel portale di gestione di Azure'
author: edupont04
manager: edupont
ms.author: edupont
ms.custom: na
ms.date: 11/15/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2018
ms.translationtype: HT
ms.sourcegitcommit: 6b60b1344a1e18ad91863046110df880f75f7c04
ms.openlocfilehash: d41b96ab5807402a342991d5c5bc2d672db09e2f
ms.contentlocale: it-it
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-register-dynamics-nav-in-the-azure-management-portal"></a>Procedura: Registrare Dynamics NAV nel portale di gestione di Azure
Se si desidera utilizzare i servizi che si basano su Microsoft Azure, è necessario registrare Dynamics NAV nel portale di gestione di Azure. Ad esempio, l'estensione [Previsione vendite e magazzino](ui-extensions-sales-forecast.md) richiede di specificare una chiave API e l'URI API e altri servizi richiedono informazioni simili. Dove si trovano dunque tali informazioni?

È possibile utilizzare la guida **Impostare il portale di gestione di Azure** per registrare Dynamics NAV nel portale di gestione di Azure ed estrarre le informazioni che servono per usare i servizi, ad esempio l'estensione di previsione vendite e previsione magazzino, Power BI, Office 365 e altro. È necessario registrarsi una sola volta nel portale di gestione di Azure e occorre essere un amministratore o un utente principale di Dynamics NAV.

Lo scopo della registrazione è fornire a Dynamics NAV e al servizio da collegare i rispettivi dettagli di Azure Active Directory (Azure AD).

## <a name="to-register-dynamics-nav-in-the-azure-management-portal"></a>Per registrare Dynamics NAV nel portale di gestione di Azure
1. Effettuare l'accesso al portale di gestione di Azure all'indirizzo [https://portal.azure.com](https://portal.azure.com). Se non si ha familiarità con il portale di gestione di Azure, è possibile trovare indicazioni nella [raccolta di documenti di Azure](https://azure.microsoft.com/en-us/documentation/articles).
2. Nel riquadro di spostamento sinistro scegliere **Più servizi**, quindi **Registrazioni app**.
3. Nel menu superiore scegliere **Aggiungi**, quindi nel **riquadro Crea** compilare i campi con le seguenti informazioni:
    - **Nome**: specificare un nome per la propria soluzione Dynamics NAV, ad esempio *Dynamics NAV*.
    - **Tipo di applicazione**: scegliere **Web App* / API**.
    - **URL accesso**: immettere l'URL del client del browser Dynamics NAV, ad esempio *https://MyServer:8080/DynamicsNAV/WebClient/OAuthLanding.htm*.
        Il file OAuthLanding.htm è un file che consente di gestire lo scambio di dati tra Dynamics NAV e altri servizi tramite Azure AD.
4. Fare clic sul pulsante **Crea**.
    Dynamics NAV viene inserito nel **riquadro delle registrazioni delle app**, in modo da potervi ora aggiungere le impostazioni.
5. Nell'**Elenco delle registrazioni delle app** scegliere una nuova app. Se questa non apre il riquadro **Impostazioni**, è necessario visualizzare un'azione per aprire **Impostazioni**.
6. Nel riquadro **Impostazioni**, nella sezione **Accesso API**, scegliere **Chiavi**.
7. Nel riquadro **Chiavi** specificare una descrizione e quando si desidera lasciare scadere la chiave, quindi scegliere **Salva**.
8. Copiare la chiave generata in una posizione temporanea, servirà nella procedura seguente.
9. Nella sezione **Accesso API** scegliere **Autorizzazioni necessarie**.
    - Aggiungere le autorizzazioni delegate per visualizzare tutti i report nel servizio Power BI
    - Aggiungere le autorizzazioni delegate per accedere e leggere il profilo utente in Microsoft Azure Active Directory
    - Ripetere la procedura per altri servizi a cui si desidera concedere l'accesso a Dynamics NAV
10. Chiudere il riquadro **Impostazioni**, quindi il riquadro **Elementi fondamentali**, copiare il valore dell'**ID applicazione** in una posizione temporanea.

Dynamics NAV è stato registrato nel portale di gestione di Azure, è stato concesso l'accesso ai servizi pertinenti e sono state estratte le informazioni necessarie in Dynamics NAV.  

## <a name="to-add-the-information-to-dynamics-nav"></a>Per aggiungere informazioni a Dynamics NAV
1. Nell'angolo superiore destro scegliere l'icona **Cerca pagina o report**, immettere **Setup guidato applicazione Azure AD**, quindi scegliere il collegamento correlato.
2. Nella procedura guidata scegliere **Avanti**.
3. Nel campo **ID client** specificare il contenuto copiato in precedenza dal campo **ID applicazione**.
4. Nel campo **Chiave privata** specificare il contenuto copiato in precedenza dal riquadro **Chiavi**.
5. Selezionare **Avanti**. Se non viene visualizzato un messaggio di errore, la procedura è terminata.

Dynamics NAV è registrato e pronto per connettersi a servizi, quali Cortana Intelligence e Power BI.

## <a name="see-also"></a>Vedi anche
[Previsione vendite e magazzino](ui-extensions-sales-forecast.md)  
[Impostare Dynamics NAV](setup.md)  

