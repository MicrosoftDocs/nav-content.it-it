---
title: "Impostare le origini Web per le società contatto"
author: edupont04
ms.custom: na
ms.date: 09/16/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: 98e70d4dd5022a69e8ba5e53ad32c00d12578e31
ms.contentlocale: it-it
ms.lasthandoff: 06/26/2017

---
# <a name="set-up-web-sources-for-contact-companies"></a>Impostare le origini Web per le società contatto
È possibile utilizzare le origini Web con le società contatto per identificare, ad esempio, motori di ricerca e siti Web dove effettuare la ricerca di informazioni sui contatti. Quando si assegna un'origine Web, specificare il motore di ricerca e la parola di ricerca che saranno utilizzati per individuare le informazioni richieste.

L'utilizzo delle origini Web nei contatti è un processo a due passaggi. Innanzitutto, occorre definire il codice origine Web. Questo passaggio deve essere eseguito una sola volta per ogni origine Web. Dopo aver creato un codice origine Web, è possibile iniziare ad assegnarlo ai contatti.

## <a name="define-a-web-source-code"></a>Definire un codice origine Web
1. Nell'angolo superiore destro, scegliere l'icona **Cerca pagina o report**, immettere **Origini Web**, quindi scegliere il collegamento correlato.
2. Scegliere l'azione **Nuovo**.
3. Compilare i campi **Codice**, **Descrizione** e **URL**.

  Nel campo **URL** immettere %1 per inserire un segnaposto per una parola di ricerca nell'URL. Quando si apre l'origine Web da un contatto, %1 verrà automaticamente sostituito con la parola da ricercare (ad esempio il nome della società) inserita nella finestra **Origini Web contatto**.

Ripetere tali passaggi per impostare altre origini Web.

## <a name="assign-web-sources-to-a-contact-company"></a>Assegnare origini Web a una società contatto
Quando si assegna un'origine Web, specificare il motore di ricerca e la parola di ricerca che saranno utilizzati per individuare le informazioni richieste.

1. Aprire il contatto.
2. Scegliere l'azione **Società**, quindi l'azione **Origini Web**. Verrà visualizzata la finestra **Origine Web contatto**.
3. Nel campo **Codice origine Web** scegliere l'origine Web che si desidera assegnare.
4. Nel campo **Parola ricerca** inserire la parola ricerca che verrà utilizzata per individuare le informazioni.

Ripetere tali passaggi per assegnare altre origini Web.

È inoltre possibile assegnare l'origine Web dalla finestra **Lista contatti** seguendo la stessa procedura.

##<a name="see-also"></a>Vedi anche
[Creare società contatto](marketing-create-contact-companies.md)

