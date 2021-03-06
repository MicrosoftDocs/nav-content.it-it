---
title: Impostare la valutazione magazzino e i costi
description: Nella tabella seguente viene descritta una sequenza di task, con collegamenti agli argomenti che li descrivono.
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/06/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 3ff4138a200f7bfa4e24aa4e5e421cfa73d24fa2
ms.contentlocale: it-it
ms.lasthandoff: 10/16/2017

---
# <a name="setting-up-inventory-valuation-and-costing"></a>Impostazione della valutazione magazzino e i costi
Per assicurarsi che i costi di magazzino vengano registrati correttamente, è necessario impostare vari campi e finestre prima di iniziare a effettuare transazioni di articoli.

Nella tabella seguente viene descritta una sequenza di task, con collegamenti agli argomenti che li descrivono.

|**Per**|**Vedere**|  
|------------|-------------|  
|Impostare un metodo di costing per ogni articolo in modo da definire come verrà utilizzato il relativo costo in entrata per valutare il valore di magazzino e il delle merci vendute.|[Procedura: Registrare nuovi articoli](inventory-how-register-new-items.md)|  
|Assicurarsi che il costo venga registrato automaticamente nella contabilità generale ogni volta che viene contabilizzata una transazione di magazzino.|Campo **Reg. automatica costi** nella pagina **Setup magazzino**|  
|Assicurarsi che i costi previsti siano registrati nella contabilità generale per visualizzare, dai conti C/G provvisori, una stima degli importi residui e il costo degli articoli trattati, prima dell'effettiva fatturazione.|Campo **Reg. costi previsti in C/G** nella pagina **Setup magazzino**|  
|Impostare il sistema affinché venga effettuata la rettifica automatica delle eventuali modifiche dei costi ogni volta che si registrano transazioni di magazzino.|[Procedura: Rettificare i costi degli articoli](inventory-how-adjust-item-costs.md)|  
|Definire se il costo medio deve essere calcolato solo per articolo o per articolo per ogni unità di stockkeeping e per ogni variante dell'articolo.|Campo **Tipo calcolo costo medio** nella pagina **Setup magazzino**|  
|Selezionare il periodo di tempo che si desidera venga utilizzato dal programma per calcolare il costo medio ponderato degli articoli per i quali è utilizzato il metodo di costing Medio.|Campo **Costo medio periodo** nella pagina **Setup magazzino**|  
|Definire i periodi di magazzino per controllare il valore di magazzino nel tempo, disabilitando la registrazione delle transazioni nei periodi di magazzino chiusi.|[Procedura: Utilizzare periodi di magazzino](finance-how-to-work-with-inventory-periods.md)|  
|Assicurarsi che i resi di vendita vengano applicati alla transazione in uscita originale per mantenere il valore di magazzino.|Campo **Storno esatto costo obblig.** nella pagina **Contabilità clienti**|  
|Assicurarsi che i resi di acquisto vengano applicati alla transazione in entrata originale per mantenere il valore di magazzino.|Campo **Storno esatto costo obblig.** nella pagina **Contabilità fornitori**|
|Impostare le regole di arrotondamento da applicare quando i prezzi degli articoli e i costi standard vengono rettificati o suggeriti.|Pagina **Metodo di arrotondamento**|  

## <a name="see-also"></a>Vedi anche  
[Gestione dei costi di magazzino](finance-manage-inventory-costs.md)  
[Utilizzo di Dynamics NAV](ui-work-product.md)  
[Finanze](finance.md)  

