---
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
title: Löschen oder Deaktivieren eines benutzerdefinierten Formulars
description: Sie können ein benutzerdefiniertes Formular aus dem System löschen oder deaktivieren.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 4d97badf-b6d0-4e7c-bff8-9ff63e83586b
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '356'
ht-degree: 0%

---

# Löschen oder Deaktivieren eines benutzerdefinierten Formulars

Sie können ein benutzerdefiniertes Formular aus dem System löschen oder deaktivieren.

>[!CAUTION]
>
>Beim Löschen eines benutzerdefinierten Formulars werden auch alle benutzerdefinierten Daten zu den mit dem Formular verknüpften Objekten gelöscht. Die gelöschten Daten können nicht wiederhergestellt werden. Ziehen Sie stattdessen die Deaktivierung eines benutzerdefinierten Formulars in Betracht. Wenn Sie ein benutzerdefiniertes Formular deaktivieren, das Sie nicht mehr verwenden, behalten Sie alle zugehörigen historischen Daten bei.

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

## Löschen eines benutzerdefinierten Formulars

1. Klicken Sie auf **Hauptmenü** icon ![](assets/main-menu-icon.png) Klicken Sie oben rechts in Adobe Workfront auf **Einrichtung** ![](assets/gear-icon-settings.png).

1. Klicken **Benutzerdefinierter Forms.**
1. Wählen Sie das benutzerdefinierte Formular aus und klicken Sie auf **Löschen**.
1. Wenn Sie sicher sind, dass Sie das benutzerdefinierte Formular und alle zugehörigen Daten zu Objekten, an die es angehängt wurde, dauerhaft löschen möchten, klicken Sie auf **Ja, löschen**.

## Deaktivieren eines benutzerdefinierten Formulars

Sie können nicht mehr verwendete benutzerdefinierte Formulare deaktivieren, ohne die zugehörigen historischen Daten zu verlieren. Benutzer können Objekten zwar kein inaktives benutzerdefiniertes Formular hinzufügen, sie können jedoch trotzdem Daten zu Objekten, an denen es bereits angehängt war, anzeigen und zu ihren Feldern hinzufügen.

Felder in einem inaktiven benutzerdefinierten Formular können auch in einer Ansicht inline bearbeitet werden. Wenn ein Benutzer während einer Inline-Bearbeitung ein Feld aus einem inaktiven benutzerdefinierten Formular hinzufügt, wird das Formular automatisch an das Objekt angehängt, auch wenn das benutzerdefinierte Formular deaktiviert ist.

Wenn Sie ein benutzerdefiniertes Formular erneut aktivieren, werden die zuvor vorhandenen Einstellungen beibehalten und die Benutzer können damit so interagieren, als wäre es nie deaktiviert.

So deaktivieren Sie ein benutzerdefiniertes Formular:

1. Klicken Sie auf **Hauptmenü** icon ![](assets/main-menu-icon.png) Klicken Sie oben rechts in Adobe Workfront auf **Einrichtung** ![](assets/gear-icon-settings.png).

1. Klicken Sie auf den Namen des benutzerdefinierten Formulars, das Sie deaktivieren möchten.
1. Klicken Sie auf **Formulareinstellungen** Registerkarte.
1. Deaktivieren Sie die **Ist aktiv** -Option.
1. Klicken **Speichern und schließen**.
