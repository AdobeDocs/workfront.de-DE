---
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
title: Löschen von Objekttypen in einem benutzerdefinierten Formular
description: In einem vorhandenen benutzerdefinierten Formular können Sie Objekttypen löschen, die mit dem Formular verknüpft sind. Danach können Benutzer das Formular nicht mehr an Objekte dieses Typs anhängen.
author: Caroline
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: ca6565c4-3d9e-4a11-a7b6-fce701923bf2
source-git-commit: 50fa63474cfd40706e74507c3e4c231c1d97d463
workflow-type: tm+mt
source-wordcount: '333'
ht-degree: 0%

---

# Löschen von Objekttypen in einem benutzerdefinierten Formular

In einem vorhandenen benutzerdefinierten Formular können Sie Objekttypen löschen, die mit dem Formular verknüpft sind. Danach können Benutzer das Formular nicht mehr an Objekte dieses Typs anhängen.

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
   <td> <p>Administratorzugriff auf benutzerdefinierte Formulare</p> <p>Informationen dazu, wie Workfront-Administratoren diesen Zugriff gewähren, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Benutzern administrativen Zugriff auf bestimmte Bereiche gewähren</a>.</p> </td> 
  </tr>  
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welche Konfigurationen für Plan, Lizenztyp oder Zugriffsstufe Sie verwenden.

## Löschen von Objekttypen in einem benutzerdefinierten Formular

Sie können Objekttypen aus einem vorhandenen benutzerdefinierten Formular löschen.

Ein benutzerdefiniertes Formular muss mindestens einen Objekttyp aufweisen.

>[!CAUTION]
>
>Wenn Personen das benutzerdefinierte Formular bereits an Objekte des Typs angehängt haben, den Sie löschen möchten, und dem das Formular Daten hinzugefügt haben, werden diese Daten beim Löschen dieses Objekttyps im Formular dauerhaft gelöscht. Sie kann historische Informationen enthalten, die Benutzer später benötigen.
>
>Im Allgemeinen empfehlen wir, die Anzahl der Bearbeitungen eines bereits verwendeten benutzerdefinierten Formulars zu minimieren. Es gibt kein Benachrichtigungssystem, um Benutzer, die das benutzerdefinierte Formular verwenden, über Ihre Änderungen zu informieren.

1. Klicken Sie auf **Hauptmenü** icon ![](assets/main-menu-icon.png) Klicken Sie oben rechts in Adobe Workfront auf **Einrichtung** ![](assets/gear-icon-settings.png).

1. Klicks **Benutzerdefinierte Forms** im linken Bereich.
1. Wählen Sie das benutzerdefinierte Formular aus, das Sie bearbeiten möchten, und klicken Sie dann auf **Bearbeiten**.
1. Klicken Sie auf das X auf einem der **Objekttypen** die Sie aus dem Formular löschen möchten, klicken Sie auf **Löschen** in der angezeigten Warnmeldung angezeigt.

   ![](assets/click-x-object-types.jpg)

1. (Optional) Wiederholen Sie den vorherigen Schritt für jeden anderen Objekttyp, den Sie aus dem Formular entfernen möchten.
1. Klicks **Fertig** Klicken Sie auf **Schließen und speichern**.
