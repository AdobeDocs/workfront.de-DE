---
title: Anzeigenlogik hinzufügen und Logik zu einem benutzerdefinierten Formular überspringen
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: Sie können festlegen, welche Abschnitte eines benutzerdefinierten Formulars angezeigt oder übersprungen werden sollen, je nach den Optionen, die ein Benutzer beim Ausfüllen vornimmt.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: c687c4a8-a99d-4ac0-b785-5bfe503a7e2c
source-git-commit: 59e3b958dd81f2f068bc06c3fe439de0084f9ce4
workflow-type: tm+mt
source-wordcount: '897'
ht-degree: 0%

---

# Anzeigenlogik hinzufügen und Logik zu einem benutzerdefinierten Formular überspringen

Sie können festlegen, welche Abschnitte eines benutzerdefinierten Formulars angezeigt oder übersprungen werden sollen, je nach den Optionen, die ein Benutzer beim Ausfüllen vornimmt.

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

## Überlegungen zur Verwendung der Anzeigelogik und der Logik zum Überspringen

* Um eine Anzeigerlogik zu einem benutzerdefinierten Feld, Widget oder Abschnittsumbruch hinzuzufügen, muss mindestens ein Auswahlfeld (Optionsfelder, Dropdown-Menüs oder Kontrollkästchen) vor dem Feld im Formular positioniert werden.

   Informationen zu benutzerdefinierten Feldern und Widgets in benutzerdefinierten Formularen finden Sie unter [Benutzerdefiniertes Feld zu einem benutzerdefinierten Formular hinzufügen](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md) und [Hinzufügen oder Bearbeiten eines Asset-Widgets in einem benutzerdefinierten Formular](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

* Sie können einem Widget oder einer Abschnittsumbruch keine Logik zum Überspringen hinzufügen. Sie können sie nur zu einem Multiple-Choice-Feld hinzufügen (Optionsfelder, Dropdown-Listen oder Kontrollkästchen).

* Sie können sowohl die Anzeigenlogik als auch die Logik zum benutzerdefinierten Feld hinzufügen. Folgendes gilt für das benutzerdefinierte Feld:

   * Es handelt sich um ein Multiple-Choice-Feld (Optionsfelder, Dropdown-Listen oder Kontrollkästchen).
   * Dem Feld wird ein Multiple-Choice-Feld vorangestellt
   * Danach folgt ein weiteres benutzerdefiniertes Feld

* Beim Kopieren von Formularen mit Anzeigenlogik oder Logik zum Überspringen wird die Logik in das neue benutzerdefinierte Formular kopiert.
* Beachten Sie Folgendes, wenn Sie eine Logikregel für die Anzeige eines benutzerdefinierten Formulars erstellen

   * Benutzerdefinierte Felder, die nicht in einer Logikanweisung zur Anzeige enthalten sind, werden standardmäßig in einem benutzerdefinierten Formular angezeigt.
   * Sie können Logikanweisungen für mehrere Felder erstellen.

* Bei der Massenbearbeitung von Objekten werden alle benutzerdefinierten Felder im Feld &quot;Objekte bearbeiten&quot;angezeigt, einschließlich der Felder, die übersprungen oder ausgeblendet werden.

## Erstellen eines benutzerdefinierten Beispielformulars mit Anzeige- und Übersprunglogik

Am besten erfahren Sie, wie Sie einem benutzerdefinierten Formular eine Anzeige- und Auslassungslogik hinzufügen, indem Sie das praktische Beispiel lesen, das in den beiden folgenden Abschnitten erläutert wird:

* [Anzeigelogik](#display-logic)
* [Logik überspringen](#skip-logic)

### Anzeigelogik {#display-logic}

1. Klicken Sie auf **Hauptmenü** icon ![](assets/main-menu-icon.png) Klicken Sie oben rechts in Adobe Workfront auf **Einrichtung** ![](assets/gear-icon-settings.png).

1. Klicken Sie im linken Bereich auf **Benutzerdefinierte Forms** ![](assets/custom-forms-icon.png).

1. Erstellen Sie das benutzerdefinierte Beispielformular:

   1. Klicken **Neues benutzerdefiniertes Formular** Klicken Sie auf **Projekt** in der Dropdown-Liste.

   1. Im **Formulartitel** Feld, Typ **Beispiel für ein benutzerdefiniertes Formular - Erlernen der Anzeigenlogik und Logik überspringen**.

   1. Klicken **Feld hinzufügen** in der oberen linken Ecke.
   1. Fügen Sie ein Dropdown-Feld mit dem Namen *Problemfeld* durch Klicken auf **Dropdown**, dann eingeben **Problemfeld** im **Titel** ankreuzen.

   1. under **Auswahlmöglichkeiten** Fügen Sie die folgenden Auswahlmöglichkeiten in die Textfelder ein:

      Erforderliche Forschung

      Keine Forschung mehr

   1. Klicken **Speichern und schließen** in der unteren linken Ecke.

1. Wählen Sie das neue **Beispiel für ein benutzerdefiniertes Formular - Erlernen der Anzeigenlogik und Logik überspringen** benutzerdefiniertes Formular und klicken Sie auf **Bearbeiten**.

1. Fügen Sie ein neues einzeiliges Textfeld mit dem Namen *sonstige Forschung* durch Klicken auf **Einzelzeilentext-Feld**, dann eingeben **sonstige Forschung** im **Titel** ankreuzen.

1. Klicken **Logik hinzufügen** in der Nähe der linken unteren Seite des **Benutzerdefiniertes Formular bearbeiten** angezeigt.

1. In dem sich öffnenden Feld wird mit dem **Anzeigelogik** Registerkarte öffnen, richten Sie die Logik ein für den Zeitpunkt, zu dem die **sonstige Forschung** wird im Formular angezeigt, indem Sie auf **Problemfeld** in der ersten Dropdown-Liste, **Erforderliche Forschung** in der zweiten Dropdown-Liste und **Ausgewählt** in der dritten Dropdown-Liste.
1. Klicken **Speichern** zum Schließen der **Feldlogik** und klicken Sie auf **Fertig** im **Feldeinstellungen** Bereich.

   Wenn jetzt jemand **Erforderliche Forschung** im **Problemfeld** in der Dropdown-Liste **sonstige Forschung** wird angezeigt.

1. Klicken **Vorschau** , um sicherzustellen, dass die Logik wie gewünscht im Formular angezeigt wird.
1. Klicken **Endvorschau** wenn Sie feststellen, dass die Logik erwartungsgemäß funktioniert.
1. Klicken **Speichern und schließen** auf **Benutzerdefiniertes Formular bearbeiten** Fenster zum Speichern des Formulars, dann fortfahren mit [Logik überspringen](#skip-logic) unten.

### Logik überspringen {#skip-logic}

Die Logik zum Überspringen funktioniert ähnlich wie die Anzeigelogik, fungiert jedoch als umgekehrt: Anstatt bestimmte benutzerdefinierte Multiple-Choice-Felder basierend auf bestimmten Auswahlen anzuzeigen, legen Sie anhand der Benutzerauswahl fest, welche Felder übersprungen werden sollen.

Um mehr darüber zu erfahren, fahren Sie mit der Arbeit an dem benutzerdefinierten Beispielformular fort, das Sie im Abschnitt erstellt haben [Anzeigelogik](#display-logic) in diesem Artikel:

1. Klicken Sie auf **Hauptmenü** icon ![](assets/main-menu-icon.png) Klicken Sie oben rechts in Adobe Workfront auf **Einrichtung** ![](assets/gear-icon-settings.png).

1. Klicken **Benutzerdefinierte Forms**.
1. Wählen Sie das Formular aus **Beispiel für ein benutzerdefiniertes Formular - Erlernen der Anzeigenlogik und Logik überspringen** die Sie in den obigen Schritten erstellt haben, klicken Sie auf **Bearbeiten**.

1. Wählen Sie das von Ihnen erstellte Dropdown-Feld namens *Problemfeld*.
1. Klicken Sie auf **Logik hinzufügen** im **Feldeinstellungen** Seitenleiste.

1. Im **Feldlogik** und stellen Sie sicher, dass die **Logik überspringen** ausgewählt ist.

1. Setzen Sie das erste Dropdown-Menü auf **Keine Forschung mehr** und die zweite Dropdown-Liste **Ausgewählt**.

1. Im **Überspringen Sie dann zu** Dropdown-Liste auswählen **Ende des Formulars.**

   Wenn jetzt jemand **Keine Forschung mehr** im **Problemfeld** in das Dropdown-Feld springen, wird das Formular direkt am Ende des Formulars übersprungen, ohne dass die **sonstige Forschung** -Feld.

1. Klicken Sie auf **Speichern**.
1. Klicken **Vorschau**  , um sicherzustellen, dass die Logik die gewünschte Anwendung findet.
1. Klicken **Fertig** unten links im Formular angezeigt.
