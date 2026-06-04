---
title: Deaktivieren oder Reaktivieren eines benutzerdefinierten Formulars
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: Sie können ein benutzerdefiniertes Formular erneut aktivieren oder deaktivieren. Es wird empfohlen, benutzerdefinierte Formulare zu deaktivieren, anstatt Formulare zu löschen, die Sie nicht mehr zur Aufbewahrung historischer Daten verwenden.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 6d9a409d-8d16-4c58-ad02-f60aa1ac1714
TQID: https://experienceleague.adobe.com/w4GbXu2z8f8kymWMp7mGn5qRm5gf5X0u9WAI2b5Lcdk
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2:
  - id: d87de1f9-8e24-4c4d-aa4c-a403075091a1
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 346
ht-degree: 12%

---

# Deaktivieren oder Reaktivieren eines benutzerdefinierten Formulars

Sie können ein benutzerdefiniertes Formular erneut aktivieren oder deaktivieren. Es wird empfohlen, benutzerdefinierte Formulare zu deaktivieren, anstatt Formulare zu löschen, die Sie nicht mehr zur Aufbewahrung historischer Daten verwenden.

>[!NOTE]
>
>Wenn ein benutzerdefiniertes Formular deaktiviert ist, aber weiterhin Teil eines Warteschlangenthemas oder einer Anfrage-Warteschlangendefinition ist, wird es an neue Anfragen angehängt. Wenn Sie nicht möchten, dass das Formular in den Anfragen enthalten ist, müssen Sie es manuell aus der Anfragewarteschlange entfernen.

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront-Paket</td> 
   <td><p>Beliebig</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront-Lizenz</td> 
   <td><p>Standard</p>
       <p>Abo</p></td>
  </tr> 
  <tr> 
   <td>Konfigurationen der Zugriffsebene</td> 
   <td> <p>Administrativer Zugriff auf benutzerdefinierte Formulare</p> </td> 
  </tr>  
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Deaktivieren eines benutzerdefinierten Formulars

Sie können benutzerdefinierte Formulare, die Sie nicht mehr verwenden, deaktivieren, ohne die zugehörigen historischen Daten zu verlieren. Benutzende können kein inaktives benutzerdefiniertes Formular zu Objekten hinzufügen, sie können jedoch weiterhin Daten zu den Feldern von Objekten anzeigen und hinzufügen, an die es bereits angehängt war.

Felder in einem inaktiven benutzerdefinierten Formular können in einer Ansicht weiterhin inline bearbeitet werden. Wenn ein(e) Benutzende(r) während einer Inline-Bearbeitung ein Feld aus einem inaktiven benutzerdefinierten Formular hinzufügt, wird das Formular automatisch an das Objekt angehängt, auch wenn das benutzerdefinierte Formular deaktiviert ist.

Deaktivieren eines benutzerdefinierten Formulars:

{{step-1-to-setup}}

1. Wählen Sie im linken Bedienfeld **Benutzerdefinierte Forms**.
1. Wählen Sie im Bereich **Forms** das benutzerdefinierte Formular aus, das Sie deaktivieren möchten.
1. Wählen Sie in der Spalte „Ist aktiv **die Option &quot;**&quot; und klicken Sie aus der Spalte heraus. Das Formular ist nicht mehr aktiv.

## Reaktivieren eines benutzerdefinierten Formulars

Wenn Sie ein benutzerdefiniertes Formular erneut aktivieren, werden die Einstellungen beibehalten, die es zuvor hatte, und Benutzende können mit ihm so interagieren, als ob es nie deaktiviert worden wäre.

{{step-1-to-setup}}

1. Wählen Sie im linken Bedienfeld **Benutzerdefinierte Forms**.
1. Wählen Sie im Bereich **Forms** das benutzerdefinierte Formular aus, das Sie erneut aktivieren möchten.
1. Wählen Sie in der Spalte Ist aktiv **True** und klicken Sie aus der Spalte heraus. Das Formular ist jetzt aktiv.
