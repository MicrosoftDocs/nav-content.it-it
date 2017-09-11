---
title: Imposte sulla vendita e Goods and Services Tax in Canada
author: edupont04
ms.custom: na
ms.date: 09/21/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: c032a02b545441b927ef5c4facc9f77731f37ab7
ms.contentlocale: it-it
ms.lasthandoff: 06/26/2017

---

# <a name="sales-tax-and-goods-and-services-tax-in-canada"></a><span data-ttu-id="6c94b-102">Imposte sulla vendita e Goods and Services Tax in Canada</span><span class="sxs-lookup"><span data-stu-id="6c94b-102">Sales Tax and Goods and Services Tax in Canada</span></span>
<span data-ttu-id="6c94b-103">In Canada, quando un fornitore non è presente da un punto di vista commerciale nella provincia in cui vengono effettuati gli acquisti, il fornitore addebita solo le imposte Goods and Services Tax (GST) o Harmonized Sales Tax (HST).</span><span class="sxs-lookup"><span data-stu-id="6c94b-103">In Canada, when a vendor does not have a business presence in the province in which purchases are made, the vendor will charge the Goods and Services Tax (GST) or Harmonized Sales Tax (HST) only.</span></span> <span data-ttu-id="6c94b-104">Tuttavia, se nella provincia è prevista un'imposta Provincial Sales Tax (PST), l'acquirente deve calcolare anche l'imposta PST e pagarla direttamente alla provincia.</span><span class="sxs-lookup"><span data-stu-id="6c94b-104">However, if the province has a Provincial Sales Tax (PST), then the purchaser must still calculate the PST and pay it directly to the province.</span></span> <span data-ttu-id="6c94b-105">Se viene selezionato un codice Provincial Tax Area Code, Dynamics NAV lo usa per calcolare l'imposta PST e registrarla in modo da ottenere un debito d'imposta sia nella contabilità generale che nei record dell'imposta.</span><span class="sxs-lookup"><span data-stu-id="6c94b-105">When a Provincial Tax Area Code is selected, Dynamics NAV uses it to calculate the PST and post it so that there is a tax liability in both the general ledger and the tax entry records.</span></span> <span data-ttu-id="6c94b-106">Di conseguenza, il codice area imposte selezionato in questo campo deve essere solo un codice che include l'imposta PST e non GST.</span><span class="sxs-lookup"><span data-stu-id="6c94b-106">Therefore, the tax area code selected here should be one where only the PST is included, not the GST.</span></span>  
<span data-ttu-id="6c94b-107">Per ulteriori informazioni sulle imposte di vendita, vedere [Imposte di vendita e categorie fiscali negli Stati Uniti e in Canada](us-finance-setup-sales-tax.md).</span><span class="sxs-lookup"><span data-stu-id="6c94b-107">For more information about sales tax, see [Sales Tax and Tax Groups in the US and Canada](us-finance-setup-sales-tax.md).</span></span>  

## <a name="submitting-the-gsthst-file"></a><span data-ttu-id="6c94b-108">Inviare il file GST/HST</span><span class="sxs-lookup"><span data-stu-id="6c94b-108">Submitting the GST/HST File</span></span>
<span data-ttu-id="6c94b-109">Le informazioni fiscali nei documenti di acquisto vengono utilizzate per generare il trasferimento Internet di file GST/HST che è necessario inviare alle autorità fiscali.</span><span class="sxs-lookup"><span data-stu-id="6c94b-109">The tax information in purchase documents is used to generate a GST/HST internet file transfer that you must  provided to the tax authorities.</span></span> <span data-ttu-id="6c94b-110">Il file include le imposte Goods and Services Tax (GST) e Harmonized Sales Tax (HST).</span><span class="sxs-lookup"><span data-stu-id="6c94b-110">This file includes goods and services tax (GST) and harmonized sales tax (HST).</span></span> <span data-ttu-id="6c94b-111">Il file viene creato in un formato .tax, che può essere trasferito tramite Internet.</span><span class="sxs-lookup"><span data-stu-id="6c94b-111">The file is created in a .tax file format, which can be transferred via the internet.</span></span>  

## <a name="see-also"></a><span data-ttu-id="6c94b-112">Vedi anche</span><span class="sxs-lookup"><span data-stu-id="6c94b-112">See Also</span></span>
[<span data-ttu-id="6c94b-113">Contabilità</span><span class="sxs-lookup"><span data-stu-id="6c94b-113">Finance</span></span>](finance-setup.md)  
[<span data-ttu-id="6c94b-114">Impostare gli aspetti finanziari</span><span class="sxs-lookup"><span data-stu-id="6c94b-114">Set Up Finance</span></span>](finance-setup-setup-finance-setup.md)  
[<span data-ttu-id="6c94b-115">Imposte di vendita e gruppi di imposte negli Stati Uniti e in Canada</span><span class="sxs-lookup"><span data-stu-id="6c94b-115">Sales Tax and Tax Groups in the US and Canada</span></span>](us-finance-setup-sales-tax.md)

