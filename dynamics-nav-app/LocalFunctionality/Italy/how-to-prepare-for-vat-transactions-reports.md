---
title: 'Procedura: Preparare i report di transazioni IVA'
description: "È necessario inviare i report periodici alle autorità fiscali per visualizzare l'elenco tutte le transazioni che includono l'IVA."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: a16640e014e157d4dbcaabc53d0df2d3e063f8f9
ms.openlocfilehash: d2919308eb8270cbaa668111fa40a2442677044d
ms.contentlocale: it-it
ms.lasthandoff: 10/26/2017

---
# <a name="how-to-prepare-for-vat-transactions-reports"></a>Procedura: Preparare i report di transazioni IVA
È necessario inviare i report periodici alle autorità fiscali per visualizzare l'elenco tutte le transazioni che includono l'IVA. L'autorità fiscale stabilisce le soglie richieste per la dichiarazione. Attualmente, la soglia è impostata su zero, a indicare che tutte le transazioni vengono dichiarate. Per prepararsi per le dichiarazioni, è necessario impostare la registrazione IVA in modo da includere gli importi di dichiarazione della transazione IVA.  

## <a name="to-set-up-vat-transaction-amounts"></a>Per impostare gli importi delle transazioni IVA  

1.  Scegliere l'icona ![Cerca pagina o report](../../media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **Cat. reg. business IVA** e scegliere il collegamento correlato.  
2.  Scegliere l'azione **Importo report transazioni IVA**.  
3.  Compilare i campi come indicato nella tabella seguente.  

    |Campo|Description|  
    |------------------------------------|---------------------------------------|  
    |**Persona fisica**|Selezionare se questo cliente è una persona fisica.|  
    |**Soggetto residente**|Specificare se il cliente è residente in Italia.<br /><br /> Se un cliente non è un residente, è necessario specificare anche un rappresentante fiscale nella Scheda dettaglio **Commercio estero**.|  
    |**Primo nome**|Specifica il nome della persona.|  
    |**Cognome**|Specifica il cognome della persona.|  
    |**Data di nascita**|Specifica la data di nascita della persona.|  
    |**Luogo di nascita**|Specifica il luogo di nascita della persona.|  

3.  Se il cliente non è in residente in Italia e non è una persona fisica, è necessario specificare un rappresentante fiscale per il cliente.  

    > [!NOTE]  
    >  Prima di poter specificare un rappresentante fiscale, è necessario creare il rappresentante fiscale come contatto.  

### <a name="to-specify-a-tax-representative-for-a-non-resident-customer"></a>Per specificare un rappresentante fiscale per un cliente non residente  

1.  Scegliere l'icona ![Cerca pagina o report](../../media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **Clienti**, quindi scegliere il collegamento correlato.  
2. Selezionare un cliente.
2.  Compilare i campi nella Scheda dettaglio **Commercio estero** come descritto nella tabella riportata di seguito.  

    |Campo|Description|  
    |---------------------------------|---------------------------------------|  
    |**Tipo di rappresentante fiscale**|Specifica se il rappresentante fiscale è un cliente o un contatto. È necessario impostare il campo su **Contatto**.|  
    |**Nr. rappresentante fiscale**|Specificare il contatto che è il rappresentante fiscale per il cliente.|  

    È necessario impostare le informazioni di modo che [!INCLUDE[navnow](../../includes/navnow_md.md)] terrà traccia delle nuove transazioni che corrispondono alle soglie specificate dalle autorità fiscali. Prima di creare il primo report transazioni IVA, è necessario preparare i dati esistenti. Per ulteriori informazioni, vedere [Procedura: Aggiornare i dati delle transazioni IVA](how-to-update-vat-transactions-data.md). È quindi possibile creare i report transazioni IVA. Per ulteriori informazioni, vedere [Procedura: Creare report elettronici di transazioni IVA](how-to-create-electronic-vat-transactions-reports.md).

## <a name="see-also"></a>Vedi anche  
 [Procedura: Aggiornare i dati delle transazioni IVA](how-to-update-vat-transactions-data.md)   
 [Procedura: Creare report elettronici di transazioni IVA](how-to-create-electronic-vat-transactions-reports.md)   
 [IVA italiana](italian-vat.md)

