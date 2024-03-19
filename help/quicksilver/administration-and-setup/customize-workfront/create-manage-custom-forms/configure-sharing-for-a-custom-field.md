---
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
title: Konfigurieren der Freigabe für benutzerdefinierte Felder und Widgets mit dem alten Formular-Builder
description: Wenn Sie ein neues benutzerdefiniertes Feld oder Widget zu einem benutzerdefinierten Formular hinzufügen, kann standardmäßig jeder Benutzer im System mit Zugriff auf benutzerdefinierte Formulare die Eigenschaften für dieses Element bearbeiten (z. B. Titel und Name). Sie können dies ändern, indem Sie steuern, für wen es freigegeben werden kann.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: ae774e73-9798-40d1-a96d-a4511f729e7f
source-git-commit: ccb2b6bb9fa63d29523ff396490f9580ad130bdd
workflow-type: tm+mt
source-wordcount: '1003'
ht-degree: 0%

---

# Konfigurieren der Freigabe für benutzerdefinierte Felder und Widgets mit dem alten Formular-Builder

<span class="preview">Die hervorgehobenen Informationen auf dieser Seite beziehen sich auf Funktionen, die noch nicht allgemein verfügbar sind. Sie ist nur in der Vorschau-Umgebung für alle Kunden oder in der Produktionsumgebung für Kunden verfügbar, die schnelle Versionen aktiviert haben.</span>

<span class="preview">Informationen zu schnellen Versionen finden Sie unter [Schnelle Versionen für Ihre Organisation aktivieren oder deaktivieren](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>

<span class="preview">Weitere Informationen zur aktuellen Version finden Sie unter [Übersicht über die Version 2024 im zweiten Quartal](/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-release-overview.md).</span>

Wenn Sie ein neues benutzerdefiniertes Feld oder Widget zu einem benutzerdefinierten Formular hinzufügen, kann standardmäßig jeder Benutzer im System mit Zugriff auf benutzerdefinierte Formulare die Eigenschaften für dieses Element bearbeiten (z. B. Titel und Name). Sie können dies ändern, indem Sie steuern, für wen es freigegeben werden kann.

Informationen zu benutzerdefinierten Feldern und Widgets in benutzerdefinierten Formularen finden Sie unter [Benutzerdefiniertes Feld zu einem benutzerdefinierten Formular mit dem Legacy-Formular hinzufügen](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md) und [Hinzufügen oder Bearbeiten eines Asset-Widgets in einem benutzerdefinierten Formular mit dem alten Formular-Builder](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

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

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Konfigurieren der Freigabe für ein benutzerdefiniertes Feld oder Widget

{{step-1-to-setup}}

1. Klicken Sie im linken Bereich auf **Benutzerdefinierte Forms**.
1. Wenn Sie die Freigabe für ein benutzerdefiniertes Feld oder Widget in der Workfront-Instanz Ihres Unternehmens konfigurieren, gehen Sie wie folgt vor:

   1. Klicks **Felder** um den Bereich Felder zu öffnen.
   1. Wählen Sie das Element aus, für das Sie die Freigabe konfigurieren möchten, und klicken Sie dann auf **Freigeben** <span class="preview">oder ![Freigabesymbol](assets/share-icon.png).</span>

   Wenn Sie die Freigabe für ein benutzerdefiniertes Feld oder Widget in einem vorhandenen benutzerdefinierten Formular konfigurieren, führen Sie die folgenden Schritte aus:

   1. Wählen Sie das benutzerdefinierte Formular aus und klicken Sie auf **Bearbeiten** <span class="preview">oder ![Symbol Bearbeiten](assets/edit-icon.png).</span>
   1. Wählen Sie im Formularbearbeitungsbereich auf der rechten Seite das Element aus, für das Sie die Freigabe konfigurieren möchten.
   1. Klicken Sie im linken Bereich auf **Feld freigeben**.

1. Im **Benutzerdefinierter Feldzugriff** das angezeigt wird, geben Sie an, für wen Sie das Element freigeben möchten und wie Sie es freigeben möchten:

   1. In der unteren linken Ecke des **Benutzerdefinierter Feldzugriff** Feld, unter **Zugriff auf benutzerdefinierte Felder gewähren an** eingeben, beginnen Sie mit der Eingabe des Namens eines Benutzers, Teams, einer Rolle, einer Gruppe oder eines Unternehmens, für den bzw. das Sie das Element freigeben möchten, und klicken Sie dann auf den Namen, wenn er angezeigt wird.

      ![](assets/share-field-give-access-to.jpg)

   1. Wenn Sie genauer wissen möchten, wie Sie das Element freigeben möchten, klicken Sie auf die Dropdownliste rechts neben dem Namen und verwenden Sie dann eine der folgenden Optionen:

      ![](assets/share-field-view-mng-options.jpg)

      <table style="table-layout:auto"> 
       <col> 
       <col> 
       <tbody> 
        <tr> 
         <td role="rowheader">Anzeigen</td> 
         <td> <p>Sie können auf <strong>Erweiterte Einstellungen</strong> um anzugeben, ob der Benutzer oder die Benutzer über seinen Zugriff das Element zu einem benutzerdefinierten Formular hinzufügen oder es für andere Benutzer freigeben können sollen.</p> </td> 
        </tr> 
        <tr> 
         <td role="rowheader">Verwalten</td> 
         <td> <p>Ermöglicht Zugriff auf das Bearbeiten des benutzerdefinierten Felds und dessen Anzeige in der Feldbibliothek und auf der Seite, auf der Sie benutzerdefinierte Formulare erstellen.</p> <p>Sie können auf <strong>Erweiterte Einstellungen</strong> , um anzugeben, ob der Benutzer oder die Benutzer über seinen Zugriff das Element aus dem System löschen oder für andere Benutzer freigeben können sollen.</p> </td> 
        </tr> 
       </tbody> 
      </table>

1. (Optional) Wiederholen Sie den vorherigen Schritt, um der Liste weitere Namen hinzuzufügen und ihre Optionen zu konfigurieren.
1. (Optional) Klicken Sie auf das Zahnradsymbol ![](assets/gear-icon-settings.png) in der oberen rechten Ecke, wenn Sie eine systemweite Freigabeoption für das Feld wählen möchten.

   Nicht alle der folgenden Optionen werden in diesem Dropdown-Menü gleichzeitig angezeigt. Beispielsweise wird die zweite nur angezeigt, wenn eine der beiden anderen ausgewählt ist.

   * **Machen Sie diesen bearbeitbaren Code systemweit so, dass er von jedem in Workfront bearbeitet werden kann** (Standardoption)

     Wenn Sie ein benutzerdefiniertes Feld oder Widget hinzufügen und die Freigabe nicht einschränken, können alle Benutzer im System, die Zugriff auf benutzerdefinierte Formulare haben, es anzeigen und seine Eigenschaften bearbeiten.

   * **Systemweiten Bearbeitungszugriff entfernen**

     Beschränkt den Zugriff auf nur die, die Sie der Liste hinzugefügt haben.

   * **Machen Sie dies systemweit sichtbar, damit jeder in Workfront es sehen kann.**

1. Klicks **Speichern** oder **Speichern und schließen**.

## Vererbter Zugriff auf benutzerdefinierte Felder und Widgets bei der Freigabe eines benutzerdefinierten Formulars

Wenn ein Benutzer ein benutzerdefiniertes Formular für eine Gruppe, eine Rolle, ein Team oder ein Unternehmen freigegeben hat, erben die Empfänger den Zugriff auf die Ansicht auf alle benutzerdefinierten Felder und Widgets, die sich im Formular befinden. Diese Zugriffsebene auf diese Elemente im Formular wird immer beibehalten, damit das Formular für die Empfänger wie von der Person, die es erstellt hat, gewünscht funktionieren kann. Dies gilt auch für Empfänger, die Zugriff auf das Formular haben.

Sie können ermitteln, wer Zugriff auf ein benutzerdefiniertes Feld oder Widget erhalten hat, und den Zugriff darauf entfernen.

>[!NOTE]
>
>Wenn ein Empfänger Zugriff auf ein benutzerdefiniertes Feld oder Widget im freigegebenen benutzerdefinierten Formular verwalten hat, wird dieser Zugriff für den Empfänger beibehalten.

* [Erfahren Sie, wer Zugriff auf ein benutzerdefiniertes Feld oder Widget erhalten hat.](#find-out-who-has-inherited-access-to-a-custom-field-or-widget)
* [Entfernen des Zugriffs auf ein benutzerdefiniertes Feld oder Widget in einem benutzerdefinierten Formular, das freigegeben wurde](#remove-access-to-a-custom-field-or-widget-in-a-custom-form-that-was-shared)

### Erfahren Sie, wer Zugriff auf ein benutzerdefiniertes Feld oder Widget erhalten hat. {#find-out-who-has-inherited-access-to-a-custom-field-or-widget}

1. Klicken Sie auf **Hauptmenü** icon ![](assets/main-menu-icon.png) Klicken Sie oben rechts in Adobe Workfront auf **Einrichtung** ![](assets/gear-icon-settings.png).

1. Klicken Sie im linken Bereich auf **Benutzerdefinierte Forms**.
1. Klicken Sie auf **Felder** und wählen Sie das Feld, Bild oder Zugriffs-Widget aus.
1. Klicken Sie in dem angezeigten Feld auf **Vererbte Berechtigungen** und die angezeigten Namen anzeigen.
1. Klicks **Abbrechen**.

### Entfernen des Zugriffs auf ein benutzerdefiniertes Feld oder Widget in einem benutzerdefinierten Formular, das freigegeben wurde {#remove-access-to-a-custom-field-or-widget-in-a-custom-form-that-was-shared}

Wenn Sie den Zugriff auf ein benutzerdefiniertes Feld oder Widget in einem benutzerdefinierten Formular entfernen müssen, das freigegeben wurde, müssen Sie die Freigabe des Formulars aufheben. Anweisungen finden Sie im Abschnitt . [Zugriff auf ein benutzerdefiniertes Formular entfernen](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md#unshare) im Artikel [Freigeben eines benutzerdefinierten Formulars](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md).
