---
title: Benutzerdefiniertes Formular mit dem alten Formular-Builder erstellen oder bearbeiten
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: Sie können ein neues benutzerdefiniertes Formular erstellen oder bearbeiten.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 5712e82d-bd1d-4d8a-9a2a-1e19b562b9d1
source-git-commit: ccb2b6bb9fa63d29523ff396490f9580ad130bdd
workflow-type: tm+mt
source-wordcount: '956'
ht-degree: 0%

---

# Benutzerdefiniertes Formular mit dem alten Formular-Builder erstellen oder bearbeiten

<!--Audited: 01/2024-->

<span class="preview">Die hervorgehobenen Informationen auf dieser Seite beziehen sich auf Funktionen, die noch nicht allgemein verfügbar sind. Sie ist nur in der Vorschau-Umgebung für alle Kunden oder in der Produktionsumgebung für Kunden verfügbar, die schnelle Versionen aktiviert haben.</span>

<span class="preview">Informationen zu schnellen Versionen finden Sie unter [Schnelle Versionen für Ihre Organisation aktivieren oder deaktivieren](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>

<span class="preview">Weitere Informationen zur aktuellen Version finden Sie unter [Übersicht über die Version 2024 im zweiten Quartal](/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-release-overview.md).</span>

Sie können ein neues benutzerdefiniertes Formular erstellen oder bearbeiten. Beide Aufgaben werden in diesem Artikel erläutert.

Informationen zum Erstellen eines neuen benutzerdefinierten Formulars aus einem vorhandenen finden Sie unter [Kopieren Sie ein benutzerdefiniertes Formular, um ein neues mit dem alten Formular-Builder zu erstellen](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/copy-custom-form-to-create-a-new-one.md).

In diesem Artikel wird beschrieben, wie Sie ein benutzerdefiniertes Formular mit dem alten Formular-Builder erstellen können. Informationen zum Erstellen eines benutzerdefinierten Formulars mit dem Formularentwickler finden Sie unter [Formular mit dem Formularentwickler erstellen](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

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
   <td><p>Neu: Standard</p>
   <p>oder</p>
   <p>Aktuell: Plan</p></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Administratorzugriff auf benutzerdefinierte Formulare</p> </td> 
  </tr>  
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Erstellen eines benutzerdefinierten Formulars

{{step-1-to-setup}}

1. Klicks **Benutzerdefinierte Forms** im linken Bereich.

   Benutzerdefinierte Formulare werden in einer Liste angezeigt. Sie können alle benutzerdefinierten Formulare und benutzerdefinierten Felder überprüfen, die für Ihr Unternehmen erstellt wurden. Sie können auch sehen, wer die einzelnen Formulare erstellt hat, welche Objekte damit verknüpft sind und ob sie aktiv sind.

1. Klicks **Neues benutzerdefiniertes Formular.**
1. Wählen Sie mindestens einen Objekttyp aus, den Sie mit dem benutzerdefinierten Formular verknüpfen möchten, und klicken Sie dann auf **Weiter**.

   ![](assets/choose-object-type.jpg)

1. Im **Formulareinstellungen** sich öffnende Registerkarte, geben Sie eine **Formulartitel** und optional **Beschreibung** für das benutzerdefinierte Formular.

1. (Optional) Wenn Sie dem Formular weitere Objekttypen hinzufügen möchten, damit es an weitere Objekte angehängt werden kann, klicken Sie auf die Schaltfläche **plus** signieren nach **Objekttypen** und wählen Sie dann den gewünschten Objekttyp im angezeigten Menü aus.

   Sie können dies wiederholen, um beliebig viele Objekttypen hinzuzufügen.

1. (Optional) Klicken Sie auf die **X** auf einen Objekttyp klicken, um ihn aus dem Formular zu löschen.

   Informationen zum Löschen von Objekttypen aus einem bereits gespeicherten benutzerdefinierten Formular finden Sie unter [Löschen von Objekttypen in einem benutzerdefinierten Formular](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/delete-object-type-on-a-custom-form.md).

1. Klicks **Fertig** in der linken unteren Ecke des Bildschirms.

   >[!TIP]
   >
   >Sie können auf **Anwenden** Sie können jederzeit ein benutzerdefiniertes Formular erstellen, um Ihre Änderungen zu speichern und das Formular zu öffnen.

1. Wenn Sie dem Formular ein neues benutzerdefiniertes Feld hinzufügen möchten, fahren Sie mit dem [Benutzerdefiniertes Feld zu einem benutzerdefinierten Formular hinzufügen](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md) oder [Wiederverwenden eines benutzerdefinierten Felds oder Widgets in einem benutzerdefinierten Formular](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/reuse-an-existing-field.md).

   Oder

   Wenn Sie Ihr benutzerdefiniertes Formular auf andere Weise weiter erstellen möchten, führen Sie einen der folgenden Artikel aus:

   * [Hinzufügen oder Bearbeiten eines Asset-Widgets in einem benutzerdefinierten Formular](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md)
   * [Positionieren von benutzerdefinierten Feldern und Widgets in einem benutzerdefinierten Formular](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/position-fields-in-a-custom-form.md)
   * [Hinzufügen eines Abschnittsumbruchs zu einem benutzerdefinierten Formular](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-section-break-to-a-custom-form.md)
   * [Hinzufügen errechneter Daten zu einem benutzerdefinierten Formular](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md)
   * [Vorhandenes berechnetes benutzerdefiniertes Feld in einem benutzerdefinierten Formular wiederverwenden](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/use-existing-calc-field-new-custom-form.md)
   * [Anzeigenlogik hinzufügen und Logik zu einem benutzerdefinierten Formular überspringen](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md)

## Bearbeiten eines benutzerdefinierten Formulars

Sie können ein benutzerdefiniertes Formular jederzeit bearbeiten, nachdem es erstellt wurde.

>[!CAUTION]
>
>Informationen zum Entfernen von Feldern aus einem benutzerdefinierten Formular ohne die von Benutzern eingegebenen Daten finden Sie im Abschnitt . [Benutzerdefiniertes Feld entfernen, ohne die von Benutzern eingegebenen Daten zu verlieren](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/delete-a-custom-field.md#remove) im Artikel [Löschen eines benutzerdefinierten Felds oder Widgets aus dem System](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/delete-a-custom-field.md).
>
>Im Allgemeinen empfehlen wir, die Anzahl der Bearbeitungen eines bereits verwendeten benutzerdefinierten Formulars zu minimieren. Es gibt kein Benachrichtigungssystem, um Benutzer, die das benutzerdefinierte Formular verwenden, über Ihre Änderungen zu informieren.

{{step-1-to-setup}}

1. Klicks **Benutzerdefinierte Forms** im linken Bereich.

   Benutzerdefinierte Formulare werden in einer Liste angezeigt. Sie können alle benutzerdefinierten Formulare und benutzerdefinierten Felder überprüfen, die für Ihr Unternehmen erstellt wurden. Sie können auch sehen, wer die einzelnen Formulare erstellt hat, welche Objekte damit verknüpft sind und ob sie aktiv sind.

1. Wählen Sie das benutzerdefinierte Formular aus, das Sie bearbeiten möchten, und klicken Sie dann auf **Bearbeiten** <span class="preview">oder ![Symbol Bearbeiten](assets/edit-icon.png).</span>
1. (Optional) Um den Titel und die Beschreibung des benutzerdefinierten Formulars zu ändern, klicken Sie auf die **Formulareinstellungen** tab, und geben Sie dann eine **Formulartitel** und **Beschreibung**.

1. (Optional) Wenn Sie dem Formular weitere Objekttypen hinzufügen möchten, damit es an weitere Objekte angehängt werden kann, klicken Sie auf das Pluszeichen + nach **Objekttypen** und wählen Sie dann den gewünschten Typ im angezeigten Menü aus.

   ![](assets/add-object-type-existing-form.png)

   Sie können dies wiederholen, um beliebig viele Objekttypen hinzuzufügen.

   Sie können auch auf das X für einen Objekttyp klicken, um ihn aus dem Formular zu löschen. Dies sollte mit Vorsicht geschehen, wenn Sie einen Objekttyp aus einem benutzerdefinierten Formular löschen möchten, das Sie bereits gespeichert haben. Weitere Informationen finden Sie unter [Löschen von Objekttypen in einem benutzerdefinierten Formular](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/delete-object-type-on-a-custom-form.md).

1. Klicks **Fertig**.

   >[!TIP]
   >
   >Sie können auf **Anwenden** Sie können jederzeit ein benutzerdefiniertes Formular erstellen, um Ihre Änderungen zu speichern und das Formular zu öffnen.

1. Wenn Sie dem Formular ein neues benutzerdefiniertes Feld hinzufügen möchten, fahren Sie mit dem [Benutzerdefiniertes Feld zu einem benutzerdefinierten Formular hinzufügen](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md) oder [Wiederverwenden eines benutzerdefinierten Felds oder Widgets in einem benutzerdefinierten Formular](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/reuse-an-existing-field.md).

   Oder

   Wenn Sie Ihr benutzerdefiniertes Formular auf andere Weise weiter erstellen möchten, führen Sie einen der folgenden Artikel aus:

   * [Hinzufügen oder Bearbeiten eines Asset-Widgets in einem benutzerdefinierten Formular](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md)
   * [Positionieren von benutzerdefinierten Feldern und Widgets in einem benutzerdefinierten Formular](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/position-fields-in-a-custom-form.md)
   * [Hinzufügen eines Abschnittsumbruchs zu einem benutzerdefinierten Formular](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-section-break-to-a-custom-form.md)
   * [Hinzufügen errechneter Daten zu einem benutzerdefinierten Formular](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md)
   * [Vorhandenes berechnetes benutzerdefiniertes Feld in einem benutzerdefinierten Formular wiederverwenden](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/use-existing-calc-field-new-custom-form.md)
   * [Anzeigenlogik hinzufügen und Logik zu einem benutzerdefinierten Formular überspringen](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md)
