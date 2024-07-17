---
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
title: Löschen von Objekttypen in einem benutzerdefinierten Formular
description: In einem vorhandenen benutzerdefinierten Formular können Sie Objekttypen löschen, die mit dem Formular verknüpft sind. Danach können Benutzer das Formular nicht mehr an Objekte dieses Typs anhängen.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: ca6565c4-3d9e-4a11-a7b6-fce701923bf2
source-git-commit: d32f274390f6ffc5fdd01c2c9b4b2abd99d7cb10
workflow-type: tm+mt
source-wordcount: '304'
ht-degree: 0%

---

# Löschen von Objekttypen in einem benutzerdefinierten Formular

{{form-designer-default}}

In einem vorhandenen benutzerdefinierten Formular können Sie Objekttypen löschen, die mit dem Formular verknüpft sind. Danach können Benutzer das Formular nicht mehr an Objekte dieses Typs anhängen.

## Zugriffsanforderungen

Sie müssen über Folgendes verfügen, um die Schritte in diesem Artikel durchzuführen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Adobe Workfront-Abo</p> </td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td>
   <p>Neu: Standard</p>
   <p>oder</p>
   <p>Aktuell: Plan</p></td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Administratorzugriff auf benutzerdefinierte Formulare</p> </td> 
  </tr>  
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Löschen von Objekttypen in einem benutzerdefinierten Formular

Sie können Objekttypen aus einem vorhandenen benutzerdefinierten Formular löschen.

Ein benutzerdefiniertes Formular muss mindestens einen Objekttyp aufweisen.

>[!CAUTION]
>
>Wenn Personen das benutzerdefinierte Formular bereits an Objekte des Typs angehängt haben, den Sie löschen möchten, und dem das Formular Daten hinzugefügt haben, werden diese Daten beim Löschen dieses Objekttyps im Formular dauerhaft gelöscht. Sie kann historische Informationen enthalten, die Benutzer später benötigen.
>
>Im Allgemeinen empfehlen wir, die Anzahl der Bearbeitungen eines bereits verwendeten benutzerdefinierten Formulars zu minimieren. Es gibt kein Benachrichtigungssystem, um Benutzer, die das benutzerdefinierte Formular verwenden, über Ihre Änderungen zu informieren.

{{step-1-to-setup}}

1. Klicken Sie im linken Bereich auf **Benutzerdefinierter Forms** .
1. Wählen Sie das benutzerdefinierte Formular aus, das Sie bearbeiten möchten, und klicken Sie dann auf das Symbol ![Bearbeiten](assets/edit-icon.png).
1. Klicken Sie auf das X für einen der **Objekttypen**, die Sie aus dem Formular löschen möchten, und klicken Sie dann in der angezeigten Warnmeldung auf **Löschen** .

   ![](assets/click-x-object-types.jpg)

1. (Optional) Wiederholen Sie den vorherigen Schritt für jeden anderen Objekttyp, den Sie aus dem Formular entfernen möchten.
1. Klicken Sie auf **Fertig** und dann auf **Speichern und schließen**.
