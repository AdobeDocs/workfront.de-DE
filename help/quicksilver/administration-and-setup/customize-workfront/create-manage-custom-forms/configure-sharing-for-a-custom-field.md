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
source-git-commit: d32f274390f6ffc5fdd01c2c9b4b2abd99d7cb10
workflow-type: tm+mt
source-wordcount: '936'
ht-degree: 0%

---

# Konfigurieren der Freigabe für benutzerdefinierte Felder und Widgets mit dem alten Formular-Builder

{{form-designer-default}}

Wenn Sie ein neues benutzerdefiniertes Feld oder Widget zu einem benutzerdefinierten Formular hinzufügen, kann standardmäßig jeder Benutzer im System mit Zugriff auf benutzerdefinierte Formulare die Eigenschaften für dieses Element bearbeiten (z. B. Titel und Name). Sie können dies ändern, indem Sie steuern, für wen es freigegeben werden kann.

Weitere Informationen zu benutzerdefinierten Feldern und Widgets in benutzerdefinierten Formularen finden Sie unter [Hinzufügen eines benutzerdefinierten Felds zu einem benutzerdefinierten Formular mit dem alten Formular-Builder](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md) und [Hinzufügen oder Bearbeiten eines Asset-Widgets in einem benutzerdefinierten Formular mit dem alten Formular-Builder](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

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

## Konfigurieren der Freigabe für ein benutzerdefiniertes Feld oder Widget

{{step-1-to-setup}}

1. Klicken Sie im linken Bereich auf **Benutzerdefinierter Forms**.
1. Wenn Sie die Freigabe für ein benutzerdefiniertes Feld oder Widget in der Workfront-Instanz Ihres Unternehmens konfigurieren, gehen Sie wie folgt vor:

   1. Klicken Sie auf **Felder** , um den Bereich Felder zu öffnen.
   1. Wählen Sie das Element aus, für das Sie die Freigabe konfigurieren möchten, und klicken Sie dann auf das Symbol ![Freigeben](assets/share-icon.png).

   Wenn Sie die Freigabe für ein benutzerdefiniertes Feld oder Widget in einem vorhandenen benutzerdefinierten Formular konfigurieren, führen Sie die folgenden Schritte aus:

   1. Wählen Sie das benutzerdefinierte Formular aus und klicken Sie dann auf das Symbol ![Bearbeiten](assets/edit-icon.png).
   1. Wählen Sie im Formularbearbeitungsbereich auf der rechten Seite das Element aus, für das Sie die Freigabe konfigurieren möchten.
   1. Klicken Sie im linken Bereich auf **Feld freigeben**.

1. Geben Sie im angezeigten Feld **Benutzerdefinierter Feldzugriff** an, für wen Sie das Element freigeben möchten und wie Sie es freigeben möchten:

   1. Geben Sie in der linken unteren Ecke des Felds **Benutzerdefinierter Feldzugriff** unter **Geben Sie benutzerdefinierten Feldzugriff auf** ein, beginnen Sie mit der Eingabe des Namens eines Benutzers, Teams, Auftrags, einer Gruppe oder eines Unternehmens, für das bzw. das Sie das Element freigeben möchten, und klicken Sie dann auf den Namen, wenn es angezeigt wird.

      ![](assets/share-field-give-access-to.jpg)

   1. Wenn Sie genauer wissen möchten, wie Sie das Element freigeben möchten, klicken Sie auf die Dropdownliste rechts neben dem Namen und verwenden Sie dann eine der folgenden Optionen:

      ![](assets/share-field-view-mng-options.jpg)

      <table style="table-layout:auto"> 
       <col> 
       <col> 
       <tbody> 
        <tr> 
         <td role="rowheader">Anzeigen</td> 
         <td> <p>Sie können auf <strong>Erweiterte Einstellungen</strong> klicken, um festzulegen, ob der Benutzer oder die Benutzer über seinen Zugriff in der Lage sein sollen, das Element zu einem benutzerdefinierten Formular hinzuzufügen oder es für andere Benutzer freizugeben.</p> </td> 
        </tr> 
        <tr> 
         <td role="rowheader">Verwalten</td> 
         <td> <p>Ermöglicht Zugriff auf das Bearbeiten des benutzerdefinierten Felds und dessen Anzeige in der Feldbibliothek und auf der Seite, auf der Sie benutzerdefinierte Formulare erstellen.</p> <p>Sie können auf <strong>Erweiterte Einstellungen</strong> klicken, um festzulegen, ob der Benutzer oder die Benutzer über seinen Zugriff das Element aus dem System löschen oder für andere Benutzer freigeben kann.</p> </td> 
        </tr> 
       </tbody> 
      </table>

1. (Optional) Wiederholen Sie den vorherigen Schritt, um der Liste weitere Namen hinzuzufügen und ihre Optionen zu konfigurieren.
1. (Optional) Klicken Sie oben rechts auf das Zahnradsymbol ![](assets/gear-icon-settings.png) , wenn Sie eine systemweite Freigabeoption für das Feld wählen möchten.

   Nicht alle der folgenden Optionen werden in diesem Dropdown-Menü gleichzeitig angezeigt. Beispielsweise wird die zweite nur angezeigt, wenn eine der beiden anderen ausgewählt ist.

   * **Sorgen Sie dafür, dass dieser Inhalt systemweit bearbeitet werden kann, damit er von allen Benutzern in Workfront bearbeitet werden kann** (Standardoption)

     Wenn Sie ein benutzerdefiniertes Feld oder Widget hinzufügen und die Freigabe nicht einschränken, können alle Benutzer im System, die Zugriff auf benutzerdefinierte Formulare haben, es anzeigen und seine Eigenschaften bearbeiten.

   * **Entfernen des systemweiten Bearbeitungszugriffs**

     Beschränkt den Zugriff auf nur die, die Sie der Liste hinzugefügt haben.

   * **Machen Sie dies systemweit sichtbar, damit jeder in Workfront es sehen kann**

1. Klicken Sie auf **Speichern** oder **Speichern + Schließen**.

## Vererbter Zugriff auf benutzerdefinierte Felder und Widgets bei der Freigabe eines benutzerdefinierten Formulars

Wenn ein Benutzer ein benutzerdefiniertes Formular für eine Gruppe, eine Rolle, ein Team oder ein Unternehmen freigegeben hat, erben die Empfänger den Zugriff auf die Ansicht auf alle benutzerdefinierten Felder und Widgets, die sich im Formular befinden. Diese Zugriffsebene auf diese Elemente im Formular wird immer beibehalten, damit das Formular für die Empfänger wie von der Person, die es erstellt hat, gewünscht funktionieren kann. Dies gilt auch für Empfänger, die Zugriff auf das Formular haben.

Sie können ermitteln, wer Zugriff auf ein benutzerdefiniertes Feld oder Widget erhalten hat, und den Zugriff darauf entfernen.

>[!NOTE]
>
>Wenn ein Empfänger Zugriff auf ein benutzerdefiniertes Feld oder Widget im freigegebenen benutzerdefinierten Formular verwalten hat, wird dieser Zugriff für den Empfänger beibehalten.

* [Ermitteln Sie, wer Zugriff auf ein benutzerdefiniertes Feld oder Widget geerbt hat](#find-out-who-has-inherited-access-to-a-custom-field-or-widget)
* [Entfernen des Zugriffs auf ein benutzerdefiniertes Feld oder Widget in einem benutzerdefinierten Formular, das freigegeben wurde](#remove-access-to-a-custom-field-or-widget-in-a-custom-form-that-was-shared)

### Erfahren Sie, wer Zugriff auf ein benutzerdefiniertes Feld oder Widget erhalten hat. {#find-out-who-has-inherited-access-to-a-custom-field-or-widget}

1. Klicken Sie auf das Symbol **Hauptmenü** oben rechts in Adobe Workfront und klicken Sie dann auf **Setup** ![](assets/gear-icon-settings.png).![](assets/main-menu-icon.png)

1. Klicken Sie im linken Bereich auf **Benutzerdefinierter Forms**.
1. Klicken Sie auf **Felder** und wählen Sie dann das Feld, Bild oder Zugriffs-Widget aus.
1. Klicken Sie im angezeigten Feld auf **Vererbte Berechtigungen** und zeigen Sie die angezeigten Namen an.
1. Klicken Sie auf **Abbrechen**.

### Entfernen des Zugriffs auf ein benutzerdefiniertes Feld oder Widget in einem benutzerdefinierten Formular, das freigegeben wurde {#remove-access-to-a-custom-field-or-widget-in-a-custom-form-that-was-shared}

Wenn Sie den Zugriff auf ein benutzerdefiniertes Feld oder Widget in einem benutzerdefinierten Formular entfernen müssen, das freigegeben wurde, müssen Sie die Freigabe des Formulars aufheben. Anweisungen finden Sie im Abschnitt [Zugriff auf ein benutzerdefiniertes Formular entfernen](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md#unshare) im Artikel [Freigeben eines benutzerdefinierten Formulars](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md).
