---
title: Impostare le dimensioni
author: edupont04
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2017
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 1b7a293982dfc7ff73c163ad1711e2bce098e98e
ms.contentlocale: it-it
ms.lasthandoff: 10/16/2017

---

# <a name="set-up-dimensions"></a>Impostare le dimensioni
Innanzitutto è necessario definire le dimensioni e i valori dimensioni da utilizzare per la società. Definire inoltre la scelta delle dimensioni da utilizzare come dimensioni globali e collegamenti dimensioni. Valutare con attenzione quali dimensioni può risultare utile definire come dimensioni globali e collegamenti dimensioni in base alle esigenze della società.  
Per impostare tutte le diverse dimensioni di cui si desidera tenere traccia, utilizzare la finestra **Dimensioni**. che contiene una riga per ogni dimensione, ad esempio *Progetto*, *Reparto*, *Area* e *Agente*.  

Per ogni dimensione è necessario anche impostarne i valori, ad esempio tutti i reparti della società. I valori di dimensione possono essere impostati in una struttura gerarchica simile al piano dei conti, in modo che i dati possano essere suddivisi in vari livelli di granularità e i sottoinsiemi dei valori di dimensione sommati.  

È possibile specificare due dimensioni globali che saranno automaticamente disponibili ovunque, ad esempio nei report e nei processi batch. Possono inoltre essere specificate sei dimensioni a collegamento rapido aggiuntive che saranno disponibili sotto forma di campo nelle righe di registrazioni e del documento. Le dimensioni rimanenti possono essere utilizzate accedendo a una finestra distinta in cui vengono visualizzate le dimensioni relative alla riga.  

In base alle necessità della società, è possibile impostare un numero illimitato di dimensioni e di valori dimensioni per ognuna di esse. Tutte le dimensioni impostate possono essere utilizzate nei movimenti di registrazione e nei documenti, oltre che nei report e nei processi batch collegate alle dimensioni.  

## <a name="set-up-default-dimensions-for-customers-vendors-and-other-accounts"></a>Impostare le dimensioni di default per clienti, fornitori e altri conti
È possibile impostare una dimensione di default per un singolo conto specifico. Il codice verrà copiato automaticamente nella registrazione o nel documento quando nella riga verrà compilato il campo con il numero di conto. È comunque possibile eliminare o modificare il codice qualora lo si ritenga necessario. È inoltre possibile rendere obbligatoria una dimensione in modo che non sia possibile registrare un movimento con un tipo di conto specifico senza avere assegnato a quest'ultimo una dimensione.  

Inoltre, è possibile impostare una dimensione predefinita per ogni tipo di conto. Il programma copierà quindi il codice nelle registrazioni o nel documento quando il tipo di conto viene compilato nella riga. Tuttavia, è sempre possibile modificare il codice del documento se necessario.  

Infine, è inoltre possibile rendere obbligatoria una dimensione in modo che non sia possibile registrare un movimento con un tipo di conto specifico senza avere assegnato a quest'ultimo una dimensione.

## <a name="see-also"></a>Vedi anche
[Utilizzo delle dimensioni](finance-dimensions.md)  
[Impostare i processi finanziari di base](finance-setup-finance.md)

