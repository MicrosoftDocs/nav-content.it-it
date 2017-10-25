---
title: 'Procedura: Creare report elettronici di transazioni IVA'
description: "È necessario creare una lista di transazioni che includono l'IVA con importi oltre la soglia corrente effettuati entro la data specificata. Inviare il report alle autorità fiscali."
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
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 20bce3e89d70ffc1a21fc647ff98aeca50e4f64a
ms.contentlocale: it-it
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-create-electronic-vat-transactions-reports"></a>Procedura: Creare report elettronici di transazioni IVA
È necessario creare una lista di transazioni che includono l'IVA con importi oltre la soglia corrente effettuati entro la data specificata. Inviare il report alle autorità fiscali.  

### <a name="to-create-a-vat-transactions-report"></a>Per creare un report di transazioni IVA  

1.  Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **Report IVA**, quindi scegliere il collegamento correlato.  

2.  Compilare i campi come indicato nella tabella seguente.  

    |Campo|Description|  
    |---
    titolo: Procedura: Creare report elettronici di transazioni IVA descrizione: È necessario creare una lista di transazioni che includono l'IVA con importi oltre la soglia corrente effettuati entro la data specificata. Inviare il report alle autorità fiscali.

    documentationcenter: '' author: SorenGP

    ms.prod: "dynamics-nav-2017" ms.topic: article ms.devlang: na ms.tgt_pltfrm: na ms.workload: na ms.search.keywords: ms.date: 07/01/2017 ms.author: sgroespe

----------------------------------|---------------------------------------|  
    |**Senza contratto**|I movimenti IVA che hanno generato questa riga non sono associati a un contratto.|  
    |**Contratto**|I movimenti IVA che hanno generato questa riga sono associati a un contratto.|  
    |**Altro**| I movimenti IVA che hanno generato questa riga non sono associati a un contratto speciale, ad esempio per manutenzione in corso o altre eccezioni.|  

    > [!TIP]  
    >  In [!INCLUDE[navnow](../../includes/navnow_md.md)], the contract that the tax authorities are looking for can be blanket orders or service contracts. To identify if the VAT report line belongs to a blanket order or service contract, you can drill down to see the underlying VAT entries from the **Amount** field.  

     Credit memos are included in the VAT transaction report if the customer or vendor is from a country/region that is outside the EU and not black-listed. For more information, see [Italian VAT](italian-vat.md).  

 Dopo avere creato il report IVA, è necessario inviarlo alle autorità fiscali. Per ulteriori informazioni, vedere [Procedura: Esportare i report di transazioni IVA](how-to-export-vat-transactions-reports.md).  

## <a name="see-also"></a>Vedi anche  
 [IVA italiana](italian-vat.md)

