---
title: Konfigurieren der Freigabe für benutzerdefinierte Felder und Widgets mit dem Formularentwickler
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: Wenn Sie ein neues benutzerdefiniertes Feld oder Widget zu einem benutzerdefinierten Formular hinzufügen, kann standardmäßig jeder Benutzer im System mit Zugriff auf benutzerdefinierte Formulare die Eigenschaften für dieses Element bearbeiten (z. B. Titel und Name). Sie können dies ändern, indem Sie steuern, für wen es freigegeben werden kann.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
source-git-commit: 6c43d836c24f893d1b7d7d01c1dd0b1cc3fba357
workflow-type: tm+mt
source-wordcount: '1095'
ht-degree: 1%

---

# Konfigurieren der Freigabe für benutzerdefinierte Felder und Widgets mit dem Formularentwickler

Wenn Sie ein neues benutzerdefiniertes Feld oder Widget zu einem benutzerdefinierten Formular hinzufügen, kann standardmäßig jeder Benutzer im System mit Zugriff auf benutzerdefinierte Formulare die Eigenschaften für dieses Element bearbeiten (z. B. Titel und Name). Sie können dies ändern, indem Sie steuern, für wen es freigegeben werden kann.

Informationen zu benutzerdefinierten Feldern und Widgets in benutzerdefinierten Formularen finden Sie unter [Formular mit dem Formularentwickler erstellen](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

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

## Konfigurieren der Freigabe eines benutzerdefinierten Felds oder Widgets aus der Formularliste

{{step-1-to-setup}}

1. Klicken Sie im linken Bereich auf **Benutzerdefinierte Forms**.
1. Klicks **Felder** um den Bereich Felder zu öffnen.
1. Wählen Sie das Element aus, für das Sie die Freigabe konfigurieren möchten, und klicken Sie dann auf ![Freigabesymbol](assets/share-icon.png).
1. Geben Sie im angezeigten Feld Benutzerdefinierter Feldzugriff an, für wen Sie das Element freigeben möchten und wie Sie es freigeben möchten:

   1. In der unteren linken Ecke des **Benutzerdefinierter Feldzugriff** Feld, unter **Zugriff auf benutzerdefinierte Felder gewähren an** eingeben, beginnen Sie mit der Eingabe des Namens eines Benutzers, Teams, einer Rolle, einer Gruppe oder eines Unternehmens, für den bzw. das Sie das Element freigeben möchten, und klicken Sie dann auf den Namen, wenn er angezeigt wird.

      ![Feld für benutzerdefinierten Feldzugriff](assets/share-field-give-access-to.jpg)

   1. Wenn Sie genauer wissen möchten, wie Sie das Element freigeben möchten, klicken Sie auf die Dropdownliste rechts neben dem Namen und verwenden Sie dann eine der folgenden Optionen:

      ![Freigabeoptionen](assets/share-field-view-mng-options.jpg)

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
1. (Optional) Klicken Sie auf das Zahnradsymbol ![Symbol Einstellungen](assets/gear-icon-settings.png) in der oberen rechten Ecke, wenn Sie eine systemweite Freigabeoption für das Feld wählen möchten.

   Nicht alle der folgenden Optionen werden in diesem Dropdown-Menü gleichzeitig angezeigt. Beispielsweise wird die zweite nur angezeigt, wenn eine der beiden anderen ausgewählt ist.

   * **Machen Sie diesen bearbeitbaren Code systemweit so, dass er von jedem in Workfront bearbeitet werden kann** (Standardoption)

     Wenn Sie ein benutzerdefiniertes Feld oder Widget hinzufügen und die Freigabe nicht einschränken, können alle Benutzer im System, die Zugriff auf benutzerdefinierte Formulare haben, es anzeigen und seine Eigenschaften bearbeiten.

   * **Systemweiten Bearbeitungszugriff entfernen**

     Beschränkt den Zugriff auf nur die, die Sie der Liste hinzugefügt haben.

   * **Machen Sie dies systemweit sichtbar, damit jeder in Workfront es sehen kann.**

1. Klicken Sie auf **Speichern**.

## Konfigurieren der Freigabe eines benutzerdefinierten Felds oder Widgets aus dem Formularentwickler

{{step-1-to-setup}}

1. Klicken Sie im linken Bereich auf **Benutzerdefinierte Forms**.
1. Öffnen Sie ein benutzerdefiniertes Formular oder erstellen Sie ein neues benutzerdefiniertes Formular.
1. Wählen Sie im Formularentwickler das Element aus, für das Sie die Freigabe konfigurieren möchten, und klicken Sie dann auf **Freigeben** im Feld rechts.
1. In dem Feld, das angezeigt wird, unter **Gewähren Sie benutzerdefinierten Formularzugriff auf**, beginnen Sie mit der Eingabe des Namens des Benutzers, Teams, der Rolle, Gruppe oder Firma, für den/die Sie das Element freigeben möchten, und drücken Sie dann die Eingabetaste **Eingabe** wenn der Name angezeigt wird.
1. Wenn Sie genauer wissen möchten, wie Sie das Element freigeben, klicken Sie auf das Dropdown-Menü rechts neben dem Namen und verwenden Sie dann eine der folgenden Optionen:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
      <tbody> 
       <tr> 
        <td role="rowheader">Anzeigen</td> 
        <td> <p>Klicks <strong>Erweiterte Einstellungen</strong> um anzugeben, ob die Benutzer das Element zu einem benutzerdefinierten Formular hinzufügen oder es für andere Benutzer freigeben können sollen.</p> </td> 
       </tr> 
       <tr> 
        <td role="rowheader">Verwalten</td> 
        <td> <p>Ermöglicht Zugriff auf das Bearbeiten des benutzerdefinierten Felds und dessen Anzeige sowohl in der Feldbibliothek als auch im Formularentwickler.</p> <p>Klicks <strong>Erweiterte Einstellungen</strong> um anzugeben, ob die Benutzer das Element aus dem System löschen oder für andere Benutzer freigeben können sollen.</p> </td> 
       </tr> 
     </tbody> 
    </table>

1. (Optional) Wiederholen Sie die Schritte 5 bis 6, um weitere Namen zur Liste hinzuzufügen und deren Optionen zu konfigurieren.
1. (Optional) Wählen Sie eine systemweite Freigabeoption für das Feld aus:

   * **Jeder im System kann** (Standardoption)

     Wenn Sie ein benutzerdefiniertes Feld oder Widget hinzufügen und die Freigabe nicht einschränken, können alle Benutzer im System, die Zugriff auf benutzerdefinierte Formulare haben, es anzeigen und seine Eigenschaften bearbeiten.

   * **Jeder im System kann**
   * **Nur eingeladene Personen können auf**

     Beschränkt den Zugriff auf nur die Elemente, die Sie der Liste hinzugefügt haben.

   ![Freigabeoptionen](assets/share-field-in-designer.png)

1. Klicken Sie auf **Speichern**.

## Vererbter Zugriff auf benutzerdefinierte Felder und Widgets bei der Freigabe eines benutzerdefinierten Formulars

Wenn ein Benutzer ein benutzerdefiniertes Formular für eine Gruppe, eine Rolle, ein Team oder ein Unternehmen freigegeben hat, erben die Empfänger den Zugriff auf die Ansicht auf alle benutzerdefinierten Felder und Widgets, die sich im Formular befinden. Diese Zugriffsebene auf diese Elemente im Formular wird immer beibehalten, damit das Formular für die Empfänger wie von der Person, die es erstellt hat, gewünscht funktionieren kann. Dies gilt auch für Empfänger, die Zugriff auf das Formular haben.

Sie können ermitteln, wer Zugriff auf ein benutzerdefiniertes Feld oder Widget erhalten hat, und den Zugriff darauf entfernen.

>[!NOTE]
>
>Wenn ein Empfänger Zugriff auf ein benutzerdefiniertes Feld oder Widget im freigegebenen benutzerdefinierten Formular verwalten hat, wird dieser Zugriff für den Empfänger beibehalten.

### Erfahren Sie, wer Zugriff auf ein benutzerdefiniertes Feld oder Widget erhalten hat. {#find-out-who-has-inherited-access-to-a-custom-field-or-widget}

{{step-1-to-setup}}

1. Klicken Sie im linken Bereich auf **Benutzerdefinierte Forms**.
1. Klicks **Felder** und wählen Sie dann das Feld, Bild oder Zugriffs-Widget aus.
1. Klicken Sie in dem angezeigten Feld auf **Vererbte Berechtigungen** und die angezeigten Namen anzeigen.
1. Klicks **Abbrechen**.

### Entfernen des Zugriffs auf ein benutzerdefiniertes Feld oder Widget in einem benutzerdefinierten Formular, das freigegeben wurde {#remove-access-to-a-custom-field-or-widget-in-a-custom-form-that-was-shared}

Wenn Sie den Zugriff auf ein benutzerdefiniertes Feld oder Widget in einem benutzerdefinierten Formular entfernen müssen, das freigegeben wurde, müssen Sie die Freigabe des Formulars aufheben. Anweisungen finden Sie im Abschnitt . [Zugriff auf ein benutzerdefiniertes Formular entfernen](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md#remove-access-to-a-custom-form-from-the-list-of-forms) im Artikel [Freigeben eines benutzerdefinierten Formulars](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md).
