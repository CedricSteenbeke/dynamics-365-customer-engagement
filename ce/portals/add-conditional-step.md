---
title: "Configure a conditional step type for a portal | MicrosoftDocs"
description: "Instructions to add and configure a conditional step type for a portal."
ms.custom: 
  - dyn365-portal
ms.date: 12/03/2018
ms.service: dynamics-365-customerservice
ms.suite: ""
ms.tgt_pltfrm: ""
ms.topic: article
ms.assetid: 3ae12878-2e9b-49fd-93a8-2465e6ade17d
ms.reviewer: ""
author: sbmjais
ms.author: shjais
manager: shubhadaj
search.audienceType: 
  - admin
  - customizer
  - enduser
search.app: 
  - D365CE
  - D365Portals
---
# Add a conditional step type

A Web Form Step can be a 'Condition' type that indicates the step should evaluate an expression. If the expression evaluates to true then the next step is displayed. If the expression evaluates to false and if the 'Next Step If Condition Fails' has been specified, that step will be displayed. The current entity is the target used to evaluate the expression against. Record Source defaults to the Record Source of the previous step.

## Attributes

| Name                         | Description                                                                                                                                                                                                                          |
|------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Condition                    | The Conditional expression to be evaluated                                                                                                                                                                                           |
| Next Step if Condition Fails | The Conditional Step Type, unlike all others, has two Next Step lookups. The default Next Step lookup will be respected if the condition evaluates to true. This property sets the next step should the condition evaluate to false. |

The available operands are as follows:

| Operand(s)    | Type                   |
|---------------|------------------------|
| =, ==         | Equals                 |
| !=            | Not Equals             |
| &gt;          | Greater Than           |
| &lt;          | Less Than              |
| &gt;=         | Greater Than or Equals |
| &lt;=         | Less Than or Equals    |
| &             | And                    |
| \|             | Or                     |
| !             | Not                    |
| =\*, ==\*, -= | Like                   |
| !=\*          | Not Like               |

## Format

The format of the expression is as follows:

\[entity attribute logical name\] \[operand\] \[value\]

Example:

new\_categorycode = 750101

A condition can have multiple expressions. You can use parentheses to group nested expressions, for example:

new\_categorycode = 750101 & gendercode = 2

-   new\_categorycode = 750101 & (gendercode = 2 | gendercode = 3)

-   new\_name = Jane Doe

-   new\_twooptionfield = true

-   new\_twooptionfield = false

### See also

[Configure a Dynamics 365 Portals](configure-portal.md)  
[Define entity forms and custom logic within the Dynamics 365 Portals](entity-forms-custom-logic.md)  
[Web Form steps for portals](web-form-steps.md)  
[Load Form/Load Tab step type](load-form-step.md)  
[Redirect step type](add-redirect-step.md)  
[Add custom JavaScript](add-custom-javascript.md)  

