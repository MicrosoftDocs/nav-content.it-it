---
title: "Impostare settori industriali per le società contatto"
author: jswymer
ms.custom: na
ms.date: 09/16/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: 466f8513b3abc8c10dc579bff5fde9ea11c21d27
ms.contentlocale: it-it
ms.lasthandoff: 06/26/2017

---
# <a name="set-up-industry-groups-for-contact-companies"></a>Impostare settori industriali per le società contatto
I gruppi industriali vengono utilizzati per indicare il tipo di settore industriale a cui appartengono i contatti, ad esempio il settore del commercio al dettaglio o l'industria automobilistica.

L'utilizzo dei settori industriali nei contatti è un processo a due passaggi. Innanzitutto, occorre definire il codice dei settori industriali. Questo passaggio deve essere eseguito una sola volta per ogni settore industriale. Dopo aver creato un codice di settore industriale, è possibile iniziare ad assegnarlo alle società.

**Nota**: se si prede di sincronizzare i contatti con fornitori, clienti o conti correnti bancari in altre sezioni dell'applicazione, è consigliabile impostare una relazione d'affari.

## <a name="define-an-industry-group-code"></a>Definire un filtro codice settore industriale
Il codice settore industriale definisce il tipo o la categoria del gruppo, ad esempio ANNUNCIO per la pubblicità o STAMPA per la TV e la radio. È possibile impostare più codici di settori industriali. Per definire i settori industriali, utilizzare la finestra **Settori industriali**.

1. Nell'angolo superiore destro, scegliere l'icona **Cerca pagina o report**, immettere **Settori industriali**, quindi scegliere il collegamento correlato.
2. Selezionare l'azione **Nuovo** e immettere un codice e una descrizione. Il codice può avere un massimo di 11 caratteri e può essere qualsiasi combinazione di numeri o lettere.

## <a name="assign-industry-groups-to-a-contact"></a>Assegnare settori industriali a un contatto
Non è possibile assegnare i settori industriali a un contatto, ma solo alle società.

1. Aprire il contatto.
2. Scegliere l'azione **Società**, quindi l'azione **Settori industriali**. Verrà visualizzata la finestra **Settori industriali contatto**.
3. Nel campo **Codice settore industriale** selezionare il settore industriale da assegnare.

Ripetere tali passaggi per assegnare altri settori industriali. È inoltre possibile assegnare settori industriali nella finestra Lista Contatti seguendo la stessa procedura.

Il numero di settori industriali assegnati al contatto nel campo **Nr. settori industriali** verrà automaticamente immesso nella sezione **Segmentazione** della finestra **Contatto**.

Una volta assegnati i settori industriali ai contatti, è possibile utilizzare queste informazioni per selezionare i contatti per i segmenti. Per ulteriori informazioni, vedere [Procedura: aggiungere contatti ai segmenti](marketing-add-contact-segment.md).

##<a name="see-also"></a>Vedi anche
[Creare società contatto](marketing-create-contact-companies.md)

