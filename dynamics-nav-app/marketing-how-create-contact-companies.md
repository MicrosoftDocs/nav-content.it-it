---
title: "Creare società contatto"
author: jswymer
ms.custom: na
ms.date: 09/16/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: a16e1748472805137d6b9a6d792e93470333f6ff
ms.contentlocale: it-it
ms.lasthandoff: 06/26/2017

---
# <a name="create-contact-companies"></a>Creare società contatto
È possibile creare un contatto per ogni nuova società con cui si interagisce, ad esempio cliente, fornitore, potenziale cliente, banca, studio legale, consulente e così via.

Esistono due modi per creare un contatto: da zero o da un cliente, un fornitore o da un conto corrente bancario esistente.

Prima di creare un contatto, si consiglia di verificare le impostazioni nella finestra **Setup marketing**. Per ulteriori informazioni, vedere [Setup della gestione dei contatti e del marketing](marketing-setup-marketing.md).

## <a name="create-a-company-contact-from-scratch"></a>Creare una società contatto da zero
1. Nell'angolo superiore destro, scegliere l'icona **Cerca pagina o report**, immettere **Contatti**, quindi scegliere il collegamento correlato.
2. Scegliere l'azione **Nuovo**.
3. Nel campo **Nr. campo** inserire un numero per il contatto.

  In alternativa, se è stata impostata una numerazione per i contatti nella finestra **Setup marketing**, è possibile premere INVIO per selezionare il successivo numero di contatto disponibile.
4. Impostare il **Tipo** su **Società**.
5. Compilare gli altri campi come necessario.

## <a name="create-a-company-contact-from-a-customer-vendor-or-bank-account"></a>Creare un contatto per una società da un cliente, fornitore o conto corrente bancario
Se è già stato impostato un numero di clienti, fornitori e conti correnti bancari, è possibile creare contatti sulla base dei dati esistenti. Quando si crea un contatto in questo modo, le informazioni di contatto verranno sincronizzate con clienti, fornitori, o le informazioni del conto corrente bancario.

**Nota**: prima di creare la società contatto in questo modo, è necessario specificare un codice relazione d'affari per clienti, fornitori e conti correnti bancari nella finestra **Setup marketing**. Se verranno creati i contatti da conti bancari, sarà necessario specificare anche la serie di numeri di conti correnti bancari nella finestra **Setup contabilità generale**.

1. Nell'angolo superiore destro, scegliere l'icona **Cerca pagina o report** immettere una delle seguenti opzioni, in base a dove si desidera creare contatti, quindi selezionare il collegamento correlato.
  * **Crea contatti da clienti**
  * **Crea contatti da fornitori**
  * **Crea contatti da conti correnti bancari**
2. Nella finestra del processo batch che si apre, nella sezione **Cliente**, **Fornitore** o **Conti correnti bancari**, impostare i filtri se si desidera creare contatti rispettivamente da clienti, fornitori o conti correnti bancari specifici.
3. Scegliere **OK** per avviare la creazione di contatti.

  Ai nuovi contatti verranno assegnati numeri contatto successivi all'interno della numerazione. Ai nuovi contatti creati verrà assegnata la relazione d'affari per i fornitori specificata nella finestra **Setup marketing**.

**Suggerimento**: è anche possibile creare un cliente, fornitore o conto corrente bancario da un contatto. Per ulteriori informazioni, vedere [Creare un un cliente, un fornitore o un conto corrente bancario da un contatto](marketing-how-create-contacts-new-customers-vendors-bank-accounts.md).
##<a name="see-also"></a>Vedi anche
[Sincronizzazione di contatti con clienti, fornitori e conti correnti bancari](marketing-synchronize-contacts-customers-vendors-bank-accounts.md)  
[Assegnare relazioni d'affari ai contatti](marketing-business-relations.md#assign-business-relations-to-a-contact)  
[Assegnare settori industriali a un contatto](marketing-industry-groups.md#assign-industry-groups-to-a-contact)  
[Assegnare gruppi di mailing a un contatto](marketing-mailing-groups.md#assign-mailing-groups-to-a-contact)  
[Procedura: creare contatti](marketing-create-contact-persons.md)  
