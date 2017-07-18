---
title: Immissione di criteri di filtro
author: SusanneWindfeldPedersen
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: 8eab393a0a77f9f1595ca1247c7549e68b491cb2
ms.contentlocale: it-it
ms.lasthandoff: 06/26/2017

---

# <a name="entering-criteria-in-filters"></a>Immissione di criteri di filtro
Quando si desidera cercare dei dati, ad esempio nomi e indirizzi dei clienti o gruppi di prodotti, si immettono dei criteri. Nei criteri di ricerca è possibile utilizzare nel campo specificato tutti i numeri e le lettere che normalmente si utilizzano. È inoltre possibile utilizzare alcuni simboli speciali per filtrare ulteriormente i risultati.

## <a name="searching-using-the-quick-filter"></a>Ricerca con l'utilizzo di Filtro rapido
È possibile aggiungere filtri a tutte le pagine, utilizzando la funzione Filtro rapido. Questa funzione viene abilitata scegliendo l'icona della lente di ingrandimento che si trova nell'angolo superiore destro di una pagina. Questo tipo di filtro viene utilizzato per una rapida immissione dei criteri.

**Importante**: la funzione Filtro rapido consente di filtrare i dati facilmente immettendo testo normale, ma non offre molte opzioni di criteri di ricerca. A seconda se si immette il testo normale o il testo con i simboli, il filtro rapido funziona in modo diverso.  
- Se si immette testo normale nei criteri di ricerca, i criteri di ricerca vengono interpretati come una ricerca senza distinzione tra maiuscole e minuscole contenente un determinato testo.  
- Se si immette del testo includendo dei simboli nei criteri di ricerca, i criteri di ricerca vengono interpretati esattamente così come sono stati immessi e la ricerca rileva la differenza tra maiuscole e minuscole.

### <a name="quick-filter-criteria"></a>Criteri di Filtro rapido
<!-- html syntax because symbols conflict with MarkDown syntax -->
<TABLE>
  <TR>
    <TH>Criteri di ricerca</TH>
    <TH>Interpretato come...</TH>
    <TH>Reso come...</TH>
  </TR>
  <TR>
    <TD>>man</TD>
    <TD>@*man*</TD>
    <TD>Tutti i record che contengono il testo man e senza distinzione tra maiuscole e minuscole.</TD>
  </TR>
  <TR>
    <TD>>se</TD>
    <TD>@*se*</TD>
    <TD>Tutti i record che contengono il testo e e senza distinzione tra maiuscole e minuscole.</TD>
  </TR>
  <TR>
    <TD>>Man*</TD>
    <TD>Inizia con Man e con distinzione tra maiuscole e minuscole.</TD>
    <TD>Tutti i record che iniziano con il testo Man.</TD>
  </TR>
  <TR>
    <TD>'man'</TD>
    <TD>Un testo esatto e con distinzione tra maiuscole e minuscole.</TD>
    <TD>Tutti i record che corrispondono esattamente a man.</TD>
  </TR>
  <TR>
    <TD>@*man</TD>
    <TD>Termina con e senza distinzione tra maiuscole e minuscole.</TD>
    <TD>Tutti i record che terminano con man.</TD>
  </TR>
  <TR>
    <TD>@man*</TD>
    <TD>Inizia con e senza distinzione tra maiuscole e minuscole.</TD>
    <TD>Tutti i record che iniziano con man.</TD>
  </TR>
</TABLE>

**Nota**: non è possibile utilizzare i carattere jolly quando si filtrano i campi di enumerazione, come il campo **Stato** negli ordini di vendita. Per immettere un filtro per il tipo di campo, è possibile immettere il valore numerico come parametro di filtro. Ad esempio, nel campo **Stato** in un ordine di vendita con i valori **Aperto**, **Rilasciato**, **In attesa di approvazione**e **Pagamento anticipato in sospeso**, utilizzare i valori **0**, **1**, **2**e **3** per filtrare in base a queste opzioni.  

## <a name="see-also"></a>Vedi anche
[Utilizzare Dynamics NAV](ui-work-product.md)

