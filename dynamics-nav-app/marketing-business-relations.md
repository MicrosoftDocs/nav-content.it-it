---
title: "Impostare relazioni d'affari nelle società contatto"
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
ms.openlocfilehash: 20abe2f08fc726a008719f94389579d02ecbd275
ms.contentlocale: it-it
ms.lasthandoff: 06/26/2017

---
# <a name="set-up-business-relations-on-contact-companies"></a>Impostare relazioni d'affari nelle società contatto
È possibile utilizzare le relazioni d'affari vengono utilizzate per indicare il tipo di relazione commerciale che intercorre con i contatti, ad esempio potenziale cliente, banca, consulente e fornitore di servizi e così via.

L'utilizzo delle relazioni d'affari nei contatti è un processo a due passaggi. Innanzitutto, occorre definire il codice relazioni d'affari. Questo passaggio deve essere eseguito una sola volta per ogni relazione d'affari. Dopo aver creato un codice di relazione d'affari, è possibile iniziare ad assegnarlo alle società.

**Nota**: se si prede di sincronizzare i contatti con fornitori, clienti o conti correnti bancari in altre sezioni dell'applicazione, è consigliabile impostare una relazione d'affari.

## <a name="define-a-business-relation-code"></a>Definire un codice relaz. d'affari
Il codice relazione d'affari definisce una categoria o un tipo della relazione d'affari, ad esempio BANCA o LEGGE. È possibile impostare più codici di relazione d'affari. Per definire la relazione d'affari, utilizzare la finestra **Relazioni d'affari**.

1. Nell'angolo superiore destro, scegliere l'icona **Cerca pagina o report**, immettere **Relazioni d'affari**, quindi scegliere il collegamento correlato.
2. Selezionare l'azione **Nuovo** e immettere un codice e una descrizione. Il codice può avere un massimo di 11 caratteri e può essere qualsiasi combinazione di numeri o lettere.

## <a name="assign-business-relations-to-a-contact"></a>Assegnare relazioni d'affari ai contatti
Non è possibile assegnare relazioni d'affari a un contatto, ma solo alle società.

1. Aprire il contatto.
2. Scegliere l'azione **Società**, quindi l'azione **Relazioni d'affari**.

    Verrà aperta la finestra **Relazioni d'affari contatto**.
3. Nel campo **Codice relazione d'affari** selezionare la relazione d'affari da assegnare.

Ripetere questi passaggi per assegnare altre relazioni d'affari. È inoltre possibile assegnare altre relazioni d'affari dalla lista Contatti seguendo la stessa procedura.

Il numero di relazioni d'affari assegnate al contatto viene visualizzato nel campo **Nr. relazione d'affari** nella sezione **Segmentazione** nella finestra **Contatto**.

Una volta assegnate le relazioni d'affari ai contatti, è possibile utilizzare queste informazioni per selezionare i contatti per i segmenti. Per ulteriori informazioni, vedere [Procedura: aggiungere contatti ai segmenti](marketing-add-contact-segment.md).

##<a name="see-also"></a>Vedi anche
[Creare società contatto](marketing-create-contact-companies.md)

