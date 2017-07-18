---
title: 'Procedura: Utilizzare i codici GIFI in Canada'
author: SorenGP
ms.custom: na
ms.date: 09/21/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: 695bca0a6836c47610210b759ae48af27484761f
ms.contentlocale: it-it
ms.lasthandoff: 06/26/2017

---

#<a name="how-to-work-with-gifi-codes-in-canada"></a>Procedura: Utilizzare i codici GIFI in Canada
Le informazioni fiscali possono includere conti di contabilità generale, report, conti economici, conti patrimoniali e conti profitti/perdite. Le informazioni fiscali vengono classificate tramite codici. L'utilizzo dei codici consente al governo di elaborare le informazioni, preparare l'archiviazione elettronica e convalidare le informazioni fiscali elettronicamente. L'utilizzo dei codici consente anche alle organizzazioni statistiche di lavorare in modo più efficiente, in quanto le informazioni finanziarie sono accessibili più facilmente. Per ulteriori informazioni, vedere il [il sito Web della Canada Revenue Agency](http://www.cra-arc.gc.ca/).

L'agenzia Canada Revenue Agency utilizza i codici General Index of Financial Information (GIFI) per raccogliere, convalidare ed elaborare elettronicamente le informazioni finanziarie e fiscali. È consigliabile assegnare i codici GIFI solo ai conti di registrazione, in modo che tutti i totali vengano calcolati dal software fiscale.

Quando un conto è associato a un codice GIFI, viene riportato all'agenzia delle entrate in base a questo campo codice. Più conti possono avere tutti lo stesso codice GIFI, ma ogni conto può avere un solo codice GIFI.

È possibile esportare le informazioni sui saldi in base al codice GIFI e salvare il file esportato in Excel, questa procedura è utile per il trasferimento delle informazioni al software fiscale.

## <a name="to-set-up-gifi-codes"></a>Per impostare i codici GIFI
In Dynamics NAV, è necessario impostare i codici GIFI per conti di contabilità generale, report, conti economici, conti patrimoniali e conti profitti/perdite.

1. Nell'angolo superiore destro, scegliere l'icona **Cerca pagina o report**, immettere **Codici GIFI**, quindi scegliere il collegamento correlato.
2. Nella finestra **Codici GIFI** scegliere l'azione **Nuovo**.
3. Impostare codici GIFI compilando i campi. Selezionare il campo per visualizzare una breve descrizione del campo o il collegamento a ulteriori informazioni.

## <a name="to-associate-gifi-codes-with-gl-accounts"></a>Per associare i codici GIFI con i conti C/G
Per creare un report con informazioni finanziarie in base al codice GIFI, ogni codice GIFI deve essere associato ai conti appropriati nel piano dei conti.

1. Nell'angolo superiore destro, scegliere l'icona **Cerca pagina o report**, immettere **Piano dei conti**, quindi scegliere il collegamento correlato.
2. Selezionare un conto di contabilità generale e scegliere l'azione **Modifica**.
3. Nella Scheda dettaglio **Contabilità industriale** nel campo **Codice GIFI** selezionare un codice GIFI appropriato.

## <a name="to-view-account-balances-using-the-gifi-code-report"></a>Per visualizzare i saldi dei conti utilizzando il report con codice GIFI
È possibile analizzare i saldi del conto in base al codice GIFI utilizzando il report **Saldi dei conti per codice GIFI**.

1. Nell'angolo superiore destro, scegliere l'icona **Cerca pagina o report**, immettere **Saldi dei conti per codice GIFI**, quindi scegliere il collegamento correlato.
2. Specificare cosa includere nel report compilando i campi. Selezionare il campo per visualizzare una breve descrizione del campo o il collegamento a ulteriori informazioni.
3. Selezionare il pulsante **Stampa** o **Anteprima**.

## <a name="to-export-balance-information-using-gifi-codes"></a>Per esportare le informazioni sui saldi in base ai codici GIFI
È possibile esportare le informazioni sui saldi in base ai codici GIFI e salvare il file esportato in Excel. È possibile modificare, salvare, o eliminare il file. È possibile utilizzare il file per trasferire le informazioni al software fiscale.

1. Nell'angolo superiore destro, scegliere l'icona **Cerca pagina o report**, immettere **Esporta info GIFI in Excel**, quindi scegliere il collegamento correlato.
2. Specificare gli elementi da esportare in Excel compilando i campi. Selezionare il campo per visualizzare una breve descrizione del campo o il collegamento a ulteriori informazioni.
3. Scegliere il pulsante **OK**.

**Nota**: il file di Excel ha le seguenti caratteristiche:

* Il saldo è arrotondato alla percentuale più vicina, ma il valore della cella mantiene la stessa percentuale come in contabilità generale.

* I numeri negativi sono rappresentati come numero positivo tra parentesi. Di conseguenza, -123 è rappresentato come (123).

## <a name="see-also"></a>Vedi anche
[Contabilità](finance-setup.md)   
[Impostare i processi finanziari di base](finance-setup-setup-finance-setup.md)

