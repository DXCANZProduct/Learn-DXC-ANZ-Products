---
# required metadata

title: EDI Core
description: EDI Core - Setup document types - Validation profiles
author: jdutoit2
manager: Kym Parker
ms.date: 2023-03-06
ms.topic: article
ms.prod: 
ms.service: dynamics-ax-applications
ms.technology: 

# optional metadata

ms.search.form: SAB_EDIDocumentTypeTable, SAB_EDITradingPartner 
audience: Application User
# ms.devlang: 
ms.reviewer: jdutoit2

# ms.tgt_pltfrm: 
ms.custom: ["21901", "intro-internal"]
ms.search.region: IconEDI
# ms.search.industry: [leave blank for most, retail, public sector]
ms.author: jdutoit2
ms.search.validFrom:   2016-05-31
ms.dyn365.ops.version:  AX 7.0.1
---

# Document types - Validation profiles

## Setup Validation profiles

Users can access the form by navigating to **EDI > Setup > Document types**.

Validation profiles are groups of business validation rules that can be applied to a trading partner. They provide the ability to set variable tolerances on various different aspects of the documents business process. 
Once a validation profile is created it can be configured by adding validation rules to it and defining the error tolerance of the rule. 

> Note:  The validation profiles FastTab is only displayed from Document types that have valid validation options

Create new validation profile:
- To create a new record, select the **New** button in the validation profiles FastTab.
- Specify the **Name** and **Description** of the profile.
- Select the **Name** hyperlink or the **Setup** button to update profile details.

Copy existing validation profile: 
- To create a new record by copying an existing record, select the applicable document type, select the existing record to copy and select the **Copy** button in the Validation profiles FastTab.
- Specify the **Name** and **Description** of the profile.
- Select **Copy**.
- Select the **Name** hyperlink or the **Setup** button to update profile details.

Add validation rules to profile:
- Select **Add** to add the validation rule.
- Select the **Validation rule**.
- Select the **Error tolerance** to specify the validation level.  If a validation rule fails, this will be used to determine how it reacts. Options:
  - **Info** - An Infolog is displayed with information only. If the validation rule fails a message will be written to the staging records log but the record will continue to process.
  - **Warning** - An Infolog is displayed with a warning. If the validation rule fails a message will be written to the staging records log but the record will continue to process. 
  - **Error** - An Infolog is displayed with an error. If the validation rule fails, the EDI Document will not be processed, and the staging records will be set to error state.

