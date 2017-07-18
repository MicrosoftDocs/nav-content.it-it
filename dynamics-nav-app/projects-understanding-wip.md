---
title: Metodi WIP
author: SorenGP
ms.custom: na
ms.date: 11/01/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: f21357897dd730d96db7abab469d5958c6fe117c
ms.contentlocale: it-it
ms.lasthandoff: 06/26/2017

---

# <a name="understanding-wip-methods"></a>Metodi WIP

Dynamics NAV supporta i seguenti metodi di calcolo e di registrazione del valore WIP.

|Metodo WIP |Formula di calcolo |Descrizione calcolo|
|-----------|--------------------|-----------------------|
|Valore coso|Ricavo riconosciuto = Prezzo fatturato fatturabile<br /><br /> Costi totali stimati = Prezzo totale fatturabile x Rapporto costi budget<br /><br /> Costi WIP = \(Percentuale di completamento - % fatturata\) x Costi totali stimati<br /><br /> Percentuale di completamento = Costi totali utilizzo/Costi totali budget<br /> % fatturata = Prezzo fatturato fatturabile<br /><br /> Costi riconosciuti prezzo totale fatturabile = Costi totali utilizzo - WIP|Per calcolare il valore costo iniziare calcolando il valore di quanto è stato fornito facendo una proporzione dei costi totali stimati in base alla percentuale di completamento. I costi fatturati vengono sottratti facendo una proporzione dei costi totali stimati in base alla percentuale fatturata.<br /><br /> Questo calcolo richiede che il prezzo totale fatturabile, il prezzo totale budget e i costi totali budget siano inseriti correttamente per l'intera commessa.|
|Costo del venduto|Ricavo riconosciuto = Prezzo fatturato fatturabile<br /><br /> Costi riconosciuti = Costo totale budget x Percentuale fatturata<br /><br /> % fatturata = Prezzo fatturato fatturabile / Prezzo totale fatturabile<br /><br /> \(La percentuale fatturata esiste come colonna nelle righe dei task commessa\)<br /><br /> Costi WIP= Costi totali utilizzo - Costi riconosciuti|Per calcolare il costo del venduto iniziare calcolando i costi riconosciuti. I costi vengono riconosciuti in modo proporzionale in base ai costi totali budget.<br /><br /> Questo calcolo richiede che il prezzo totale fatturabile e i costi totali budget siano inseriti correttamente per l'intera commessa.|
|Valore vendite|Costi riconosciuti = Costi totali utilizzo<br /><br /> Ricavo riconosciuto = Prezzo totale utilizzo x Rapporto fatturazione previsto<br /><br /> % recupero costi = Prezzo totale fatturabile / Prezzo totale budget<br /><br /> Vendite WIP = Vendite riconosciute - Prezzo fatturato fatturabile|I calcoli del valore vendite riconoscono il ricavo in modo proporzionale in base ai costi totali utilizzo e al rapporto di recupero costi previsto.<br /><br /> Questo calcolo richiede che il prezzo totale fatturabile e il prezzo totale budget siano inseriti correttamente per l'intera commessa.|
|Percentuale di completamento|Costi riconosciuti = Costi totali utilizzo<br /><br /> Ricavo riconosciuto = Prezzo totale fatturabile x Percentuale di completamento<br /><br /> Percentuale di completamento = Costi totali utilizzo/Costi totali budget<br /><br /> \(Indicato come "% completamento costi" nelle righe dei task commessa\)<br /> Vendite WIP = Vendite riconosciute - Prezzo fatturato fatturabile|I calcoli della percentuale di completamento riconoscono il ricavo in modo proporzionale in base alla percentuale di completamento, ovvero il rapporto tra i costi totali utilizzo e i costi di budget.<br /><br /> Questo calcolo richiede che il prezzo totale fatturabile e i costi totali budget siano inseriti correttamente per l'intera commessa.|
|Contratto completato|Importo WIP = Importo costo WIP = Utilizzo \(costo totale\)<br /><br /> Importo vendita WIP = Fatturabile \(Prezzo fatturato\)|Il ricavo e i costi vengono riconosciuti dal contratto completato solo in seguito al completamento della commessa. Ciò risulta utile qualora le previsioni dei costi e del ricavo della commessa siano particolarmente incerte.<br /><br /> Qualsiasi utilizzo viene registrato in Conto costi WIP \(cespiti\) e tutte le vendite fatturate vengono registrate in Conto vendite fatturate WIP \(passività\), fino al completamento della commessa.|

## <a name="see-also"></a>Vedi anche
[Gestione di progetti](projects-manage-projects.md)  
[Contabilità](finance-setup.md)  
[Gestire gli acquisti](purchasing-manage-purchasing.md)         
[Gestire le vendite](sales-manage-sales.md)      
[Utilizzare Dynamics NAV](ui-work-product.md)  

