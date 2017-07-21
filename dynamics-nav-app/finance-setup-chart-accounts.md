---
title: Impostare o modificare il piano dei conti
author: edupont04
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: 48cd91958545b40b2ab0c5e48442fc874845af5b
ms.contentlocale: it-it
ms.lasthandoff: 06/26/2017

---

# <a name="set-up-or-change-the-chart-of-accounts"></a>Impostare o modificare il piano dei conti
Il piano dei conti mostra i conti di contabilità che memorizzano i dati finanziari. Dynamics NAV include un piano dei conti standard pronto per supportare l'azienda.
Tuttavia, è possibile modificare i conti predefinti ed è possibile aggiungere nuovi conti.  

## <a name="adding-or-changing-accounts"></a>Aggiungere o modificare i conti
Nel piano dei conti, è possibile aprire ogni conto C/G e aggiungere o modificare le impostazioni.

**Nota**: è possibile eliminare un conto di contabilità generale. Tuttavia, prima che venga eliminato, è necessario soddisfare le seguenti condizioni:  
- Il saldo nel conto deve essere pari a zero.  
- Nel campo **Consenti Eliminaz. Conti C/G Anteriori a** della finestra **Setup Contabilità Generale** deve essere impostata una data ed è necessario che il conto non includa movimenti contabili in tale data o dopo tale data.  
- Se il campo **Verifica Uso Conti C/G** della finestra **Setup Contabilità Generale** è selezionato, il conto non deve essere utilizzato in tutte le categorie di registrazione o impostazioni delle registrazioni.  

Dynamics NAV impedirà di eliminare un conto di contabilità generale che memorizza dati necessari per il piano dei conti.  

##<a name="see-also"></a>Vedi anche  
[Contabilità generale e piano dei conti](finance-setup-general-ledger.md)  
[Gestire i conti correnti bancari](bank-manage-bank-accounts.md)  
[Dimensioni](finance-setup-dimensions.md)  
[Procedura: Utilizzare i codici GIFI in Canada](ca-finance-setup-work-GiFI-codes.md)

