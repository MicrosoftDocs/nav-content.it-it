---
title: Impostare l'arrotondamento delle fatture
description: "È possibile arrotondare gli importi delle fatture quando si creano fatture. È inoltre possibile che la normativa o le autorità locali impongano una modalità di arrotondamento specifica, ad esempio a un importo divisibile per 0,05."
documentationcenter: 
author: bholtorf
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/15/2017
ms.author: bholtorf
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: d52f27fc7733a485a329884d15c58921caf4719f
ms.contentlocale: it-it
ms.lasthandoff: 10/16/2017

---
# <a name="set-up-invoice-rounding"></a>Impostare l'arrotondamento delle fatture
Se è necessario arrotondare gli importi delle fatture quando si creano le fatture, è possibile utilizzare la funzione di arrotondamento automatica. Quando una fattura viene arrotondata, viene aggiunta un'ulteriore riga con l'importo di arrotondamento. Questa riga verrà contabilizzata insieme alle altre righe della fattura.

> [!NOTE]  
>  È possibile che la normativa o le autorità locali impongano una modalità di arrotondamento specifica, ad esempio a un importo divisibile per 0,05.  
  
Per utilizzare l'arrotondamento fattura automatico, è necessario:  
  
* Specificare i conti di contabilità generale in cui verranno registrate le differenze di arrotondamento.  
* Impostare regole per l'arrotondamento delle fatture nella valuta locale e in una valuta estera.  
* Attivare la funzione.  
  
> [!NOTE]  
>  Oltre alle funzionalità di arrotondamento fattura, sono disponibili le funzionalità di arrotondamento importo unitario e arrotondamento importo per eseguire l'arrotondamento degli importi sulle fatture.  
 
## <a name="how-to-set-up-general-ledger-accounts-for-invoice-rounding-differences"></a>Procedura: Impostare i conti contabilità generale per le differenze di arrotondamento fattura
Per utilizzare la funzione di arrotondamento fattura automatico, è necessario impostare il conto o i conti di contabilità generale in cui verranno registrate le differenze di arrotondamento. Prima di ciò è necessario impostare le categorie di registrazione articolo/servizio IVA. Per ulteriori informazioni, vedere [Impostare l'IVA](finance-setup-vat.md).  
  
### <a name="to-set-up-general-ledger-accounts-for-invoice-rounding-differences"></a>Per impostare i conti contabilità generale per le differenze di arrotondamento fattura  
1. Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **Piano dei conti**, quindi scegliere il collegamento correlato.  
2. Nella pagina **Piano dei conti** impostare il conto e assegnargli il nome **Arrotondamento fattura** o simile. In [!INCLUDE[d365fin](includes/d365fin_md.md)] il nome del conto verrà utilizzato come testo per le fatture arrotondate.  
3. A seconda che si utilizzi l'IVA o la tassa sulla vendita, nei campi **Cat. reg. art./serv. imposta** o **Cat. reg. art./serv. IVA**, scegliere una categoria di registrazione per gli importi arrotondati. È possibile impostare un nuovo codice di gruppo da utilizzare per l'arrotondamento delle fatture.
4. Lasciare vuoti i campi **Tipo reg. gen.** e **Cat. reg. business imposta** o **Cat. reg. business IVA**. <!-- Why do we say to leave these blank, when there are a lot of other fields we also leave blank but don't mention? -->  
  
A questo punto è possibile assegnare il conto arrotondamento fatture alle categorie di registrazione nella pagina **Categorie registrazione fornitori**.  <!-- Why only the vendor posting groups? -->

## <a name="how-to-set-up-rounding-for-foreign-and-local-currencies"></a>Procedura: Impostare l'arrotondamento per le valute locali ed estere
Prima di poter utilizzare la funzione di arrotondamento delle fatture, è necessario impostare le regole di arrotondamento per le valute locali ed estere.

### <a name="to-set-up-rounding-for-foreign-currencies"></a>Per impostare l'arrotondamento per le valute estere  
1. Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **Servizi tasso di cambio valuta**, quindi scegliere il collegamento correlato.  
2. Nella pagina **Valute** scegliere la valuta estera per aprire la **Scheda valuta**, quindi compilare i campi **Precisione arrot. importo**, **Precisione arrot. importo unit.**, **Precisione arrot. fatt.** e **Tipo arrot. fatt.**.
  
### <a name="to-set-up-rounding-for-your-local-currency"></a>Per impostare l'arrotondamento per la valuta locale
1. Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "Cerca pagina o report"), immettere **Setup contabilità generale**, quindi selezionare il collegamento correlato.  
2. Nella pagina **Setup contabilità generale**, nella Scheda dettaglio **Generale**, compilare i campi **Precisione arrot. fatt.** e **Tipo arrot. fatt.**.  

## <a name="how-to-activate-the-invoice-rounding-function"></a>Procedura: Attivare la funzione di arrotondamento fatture  
Per assicurarsi che le fatture di acquisto e vendita vengano arrotondate automaticamente è necessario attivare la funzione di arrotondamento fatture. È possibile attivare la funzione di arrotondamento in maniera indipendente per le fatture relative alle vendite e gli acquisti.

1. Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **Setup contabilità clienti e vendite** o **Setup contabilità fornitori e acquisti**, quindi scegliere il collegamento correlato.  
2. Nella Scheda dettaglio **Generale** selezionare la casella di controllo **Arrotondamento fattura**.  
  
## <a name="see-also"></a>Vedi anche  
[Procedura: Fatturare le vendite](sales-how-invoice-sales.md)  
[Procedura: Registrare gli acquisti](purchasing-how-record-purchases.md)
