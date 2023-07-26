---
title: Deaktivieren oder reaktivieren Sie ein benutzerdefiniertes Formular
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: Sie können ein benutzerdefiniertes Formular reaktivieren oder deaktivieren. Es wird empfohlen, benutzerdefinierte Formulare zu deaktivieren, anstatt Formulare zu löschen, die Sie nicht mehr verwenden, um historische Daten beizubehalten.
author: Courtney
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 6d9a409d-8d16-4c58-ad02-f60aa1ac1714
source-git-commit: 50fa63474cfd40706e74507c3e4c231c1d97d463
workflow-type: tm+mt
source-wordcount: '355'
ht-degree: 0%

---

# Deaktivieren oder reaktivieren Sie ein benutzerdefiniertes Formular

Sie können ein benutzerdefiniertes Formular reaktivieren oder deaktivieren. Es wird empfohlen, benutzerdefinierte Formulare zu deaktivieren, anstatt Formulare zu löschen, die Sie nicht mehr verwenden, um historische Daten beizubehalten.

## Zugriffsanforderungen

Sie müssen über Folgendes verfügen, um die Schritte in diesem Artikel durchzuführen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Adobe Workfront-Plan*</p> </td> 
   <td>Beliebig</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td>Plan</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Administratorzugriff auf benutzerdefinierte Formulare</p> <p>Informationen dazu, wie Workfront-Administratoren diesen Zugriff gewähren, finden Sie unter <a href="/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Benutzern administrativen Zugriff auf bestimmte Bereiche gewähren</a>.</p></td> 
  </tr>  
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welche Konfigurationen für Plan, Lizenztyp oder Zugriffsstufe Sie verwenden.

## Deaktivieren eines benutzerdefinierten Formulars

Sie können nicht mehr verwendete benutzerdefinierte Formulare deaktivieren, ohne die zugehörigen historischen Daten zu verlieren. Benutzer können Objekten zwar kein inaktives benutzerdefiniertes Formular hinzufügen, sie können jedoch trotzdem Daten zu Objekten, an denen es bereits angehängt war, anzeigen und zu ihren Feldern hinzufügen.

Felder in einem inaktiven benutzerdefinierten Formular können auch in einer Ansicht inline bearbeitet werden. Wenn ein Benutzer während einer Inline-Bearbeitung ein Feld aus einem inaktiven benutzerdefinierten Formular hinzufügt, wird das Formular automatisch an das Objekt angehängt, auch wenn das benutzerdefinierte Formular deaktiviert ist.

So deaktivieren Sie ein benutzerdefiniertes Formular:

1. Klicken Sie auf **Hauptmenü** icon ![](assets/main-menu-icon.png) Klicken Sie oben rechts in Adobe Workfront auf **Einrichtung** ![](assets/gear-icon-settings.png).
1. Wählen Sie im linken Bereich die Option **Benutzerdefinierte Forms**.
1. Im **Forms** wählen Sie das benutzerdefinierte Formular aus, das Sie deaktivieren möchten.
1. Wählen Sie in der Spalte Ist aktiv die Option **False** und klicken Sie aus der Spalte. Das Formular ist nicht mehr aktiv.

## Benutzerdefiniertes Formular erneut aktivieren

Wenn Sie ein benutzerdefiniertes Formular reaktivieren, werden die zuvor vorhandenen Einstellungen beibehalten und die Benutzer können mit dem Formular so interagieren, als wäre es nie deaktiviert.

1. Klicken Sie auf **Hauptmenü** icon ![](assets/main-menu-icon.png) Klicken Sie oben rechts in Adobe Workfront auf **Einrichtung** ![](assets/gear-icon-settings.png).
1. Wählen Sie im linken Bereich die Option **Benutzerdefinierte Forms**.
1. Im **Forms** wählen Sie das benutzerdefinierte Formular aus, das Sie reaktivieren möchten.
1. Wählen Sie in der Spalte Ist aktiv die Option **True** und klicken Sie aus der Spalte. Das Formular ist jetzt aktiv.
