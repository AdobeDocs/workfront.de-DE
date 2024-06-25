---
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
title: Positionieren Sie benutzerdefinierte Felder und Widgets in einem benutzerdefinierten Formular mit dem Legacy-Formular
description: Sie können benutzerdefinierte Felder und Widgets in einem benutzerdefinierten Formular neu positionieren.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: f96425e3-8e20-43ac-8340-915538ae5886
source-git-commit: d32f274390f6ffc5fdd01c2c9b4b2abd99d7cb10
workflow-type: tm+mt
source-wordcount: '449'
ht-degree: 0%

---

# Positionieren Sie benutzerdefinierte Felder und Widgets in einem benutzerdefinierten Formular mit dem Legacy-Formular

{{form-designer-default}}

Sie können benutzerdefinierte Felder und Widgets in einem benutzerdefinierten Formular neu positionieren.

Informationen zu benutzerdefinierten Feldern und Widgets in benutzerdefinierten Formularen finden Sie unter [Benutzerdefiniertes Feld zu einem benutzerdefinierten Formular hinzufügen](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md) und [Hinzufügen oder Bearbeiten eines Asset-Widgets in einem benutzerdefinierten Formular](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

## Zugriffsanforderungen

Sie müssen über Folgendes verfügen, um die Schritte in diesem Artikel durchzuführen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Adobe Workfront-Plan*</p> </td> 
   <td>Alle</td> 
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

## Positionieren von benutzerdefinierten Feldern und Widgets in einem benutzerdefinierten Formular

1. Beginnen Sie mit der Erstellung oder Bearbeitung eines benutzerdefinierten Formulars, wie unter [Benutzerdefiniertes Formular mit dem alten Formular-Builder erstellen oder bearbeiten](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).
1. Fügen Sie benutzerdefinierte Felder und Widgets zum Formular hinzu, wie unter [Benutzerdefiniertes Feld zu einem benutzerdefinierten Formular mit dem Legacy-Formular hinzufügen](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md) und [Hinzufügen oder Bearbeiten eines Asset-Widgets in einem benutzerdefinierten Formular mit dem alten Formular-Builder](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

1. (Optional) Um benutzerdefinierte Felder und Widgets in derselben Zeile zu positionieren, ziehen Sie eine neben die andere, bis eine Linie dazwischen angezeigt wird.

<!--
Courtney, this is a story that got postponed after I did the work. Slated for some time in 22.4 (https://hub.workfront.adobe.com/task/6220d425000140d7f7d3ea68cc9529c8/documents)
   You can drag multiple items. Press the following keys while you select the items, then drag the items together to the new row:
   * Mac: Command+Shift [Courtney, double-check these commands]
   * Windows: Ctrl+Shift

   When you drop the custom field or widget, a gray box displays around the two items to indicate that they share a row.
-->

>[!NOTE]
>
>* Sie können die **Vorschau** rechts unten, um eine Vorstellung davon zu erhalten, wie die benutzerdefinierten Felder und Widgets im Formular angezeigt werden.
>* Beschreibende Textfelder können keine Zeile freigeben.
>* Benutzerdefinierte Felder und Widgets werden im Formular möglicherweise nicht immer auf die gleiche Weise angezeigt, je nachdem, wie viel Platz auf dem Bildschirm verfügbar ist, wenn ein Benutzer das Formular anzeigt. Beispielsweise kann das dritte Feld in einer Zeile von Feldern zur nächsten Zeile von Feldern umbrechen, wenn der horizontale Bereich begrenzt ist.

1. (Optional) Um ein benutzerdefiniertes Feld oder Widget über oder unter einem anderen zu positionieren, ziehen Sie es über oder unter, bis eine horizontale blaue Linie zwischen den Elementen angezeigt wird.
1. Klicks **Anwenden**.
1. Wenn Sie Ihr benutzerdefiniertes Formular auf andere Weise weiter erstellen möchten, führen Sie einen der folgenden Artikel aus:

   * [Benutzerdefiniertes Feld zu einem benutzerdefinierten Formular mit dem Legacy-Formular hinzufügen](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md#add2)
   * [Hinzufügen oder Bearbeiten eines Asset-Widgets in einem benutzerdefinierten Formular mit dem alten Formular-Builder](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md)
   * [Hinzufügen berechneter Daten zu einem benutzerdefinierten Formular mit dem Legacy-Formular](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md)
   * [Hinzufügen eines Abschnittsumbruchs zu einem benutzerdefinierten Formular mit dem Legacy-Formular](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-section-break-to-a-custom-form.md)
   * [Fügen Sie mit dem alten Formular-Builder Logik hinzu und überspringen Sie Logik zu einem benutzerdefinierten Formular](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md)
   * [Erstellen Sie eine Vorschau und füllen Sie ein benutzerdefiniertes Formular mit dem alten Formular-Builder aus.](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/preview-and-complete-a-custom-form.md)
