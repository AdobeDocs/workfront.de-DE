---
title: Fügen Sie die Anzeigenlogik hinzu und überspringen Sie die Logik mit dem Formularentwickler
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: Sie können festlegen, welche Abschnitte eines benutzerdefinierten Formulars angezeigt oder übersprungen werden sollen, je nach den Optionen, die ein Benutzer beim Ausfüllen vornimmt.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
source-git-commit: 930a04e02d73b75a6dac957e4dfbc76a5f73246f
workflow-type: tm+mt
source-wordcount: '1358'
ht-degree: 0%

---

# Fügen Sie die Anzeigenlogik hinzu und überspringen Sie die Logik mit dem Formularentwickler

<span class="preview">Die Informationen auf dieser Seite beziehen sich auf Funktionen, die noch nicht allgemein verfügbar sind. Sie ist nur in der Vorschau-Umgebung für alle Kunden oder in der Produktionsumgebung für Kunden verfügbar, die schnelle Versionen aktiviert haben.</span>

<span class="preview">Informationen zu schnellen Versionen finden Sie unter [Schnelle Versionen für Ihre Organisation aktivieren oder deaktivieren](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>

<span class="preview">Weitere Informationen zur aktuellen Version finden Sie unter [Übersicht über die Version 2024 im zweiten Quartal](/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-release-overview.md).</span>

Sie können festlegen, welche Abschnitte eines benutzerdefinierten Formulars angezeigt oder übersprungen werden sollen, je nach den Optionen, die ein Benutzer beim Ausfüllen vornimmt.

>[!NOTE]
>
>Die Logik gilt nur innerhalb eines Formulars und kann nicht auf einer Auswahl aus einem anderen Formular basieren.

## Zugriffsanforderungen

Sie müssen über Folgendes verfügen, um die Schritte in diesem Artikel durchzuführen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Adobe Workfront-Abo </td> 
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
   <td>Administratorzugriff auf benutzerdefinierte Formulare </td> 
  </tr>  
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Logiksymbole anzeigen und überspringen

Benutzerdefinierte Formulare zeigen Symbole an, die angeben, welche Logik auf bestimmte Felder angewendet wird. Die Symbole in einem Feld im Formularentwickler weisen darauf hin, dass auf das Feld Logik angewendet wird.

| Symbol | Position im Feld im Formularentwickler | Definition |
|--- |--- |--- |
| ![Logik für Zielfeld anzeigen](assets/display-logic-bottom-left.png) | Unten links | Das Feld ist das Zielfeld für die Anzeigerogik. Wenn eine bestimmte Auswahl im Formular vorgenommen wird, wird dieses Feld angezeigt. |
| ![Symbol für Anzeigenlogik definieren](assets/display-logic-bottom-right.png) | Unten rechts | Das Feld definiert die Anzeigerogik. Eine bestimmte Auswahl oder ein Wert für dieses Feld zeigt das Zielfeld an. |
| ![Logik für Zielfeld überspringen](assets/skip-logic-bottom-left.png) | Unten links | Das Feld ist das Zielfeld für die Logik zum Überspringen. Wenn eine bestimmte Auswahl im Formular vorgenommen wird, wird das Formular zu diesem Feld übersprungen und die dazwischen liegenden Felder werden ausgeblendet. |
| ![Symbol &quot;Logik überspringen&quot;definieren](assets/skip-logic-bottom-right.png) | Unten rechts | Das Feld definiert die Logik zum Überspringen. Eine bestimmte Auswahl oder ein Wert für dieses Feld überspringt andere Felder und geht direkt zum Zielfeld. |

![Logische Symbole](assets/logic-icons-3.png)

Wählen Sie ein Feld mit angewendeter Logik aus, um die vorhandenen Logikregeln in den Feldeinstellungen anzuzeigen.

![Logische Regeln](assets/form-designer-view-only-logic.png)

## Überlegungen zur Verwendung der Anzeigelogik und der Logik zum Überspringen

* Um eine Anzeigerlogik zu einem benutzerdefinierten Feld, Widget oder Abschnittsumbruch hinzuzufügen, muss mindestens ein Auswahlfeld (Optionsfelder, Dropdown-Menüs oder Kontrollkästchen) vor dem Feld im Formular positioniert werden.
Informationen zu benutzerdefinierten Feldern und Widgets in benutzerdefinierten Formularen finden Sie unter [Formular mit dem Formularentwickler erstellen](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).
* Sie können einem Widget oder einer Abschnittsumbruch keine Logik zum Überspringen hinzufügen. Sie können sie nur zu einem Multiple-Choice-Feld hinzufügen (Optionsfelder, Dropdown-Listen oder Kontrollkästchen).
* Sie können einem benutzerdefinierten Feld sowohl die Anzeigenlogik als auch die Logik überspringen, wenn Folgendes für das benutzerdefinierte Feld zutrifft:

   * Es handelt sich um ein Multiple-Choice-Feld (Optionsfelder, Dropdown-Listen oder Kontrollkästchen).
   * Dem Feld wird ein Multiple-Choice-Feld vorangestellt
   * Danach folgt ein weiteres benutzerdefiniertes Feld

* Beim Kopieren von Formularen mit Anzeigenlogik oder Logik zum Überspringen wird die Logik in das neue benutzerdefinierte Formular kopiert.
* Bei der Massenbearbeitung von Objekten werden alle benutzerdefinierten Felder im Feld &quot;Objekte bearbeiten&quot;angezeigt, einschließlich der Felder, die übersprungen oder ausgeblendet werden.
* Beachten Sie Folgendes, wenn Sie eine Logikregel für die Anzeige eines benutzerdefinierten Formulars erstellen:

   * Benutzerdefinierte Felder, die nicht in einer Logikanweisung zur Anzeige enthalten sind, werden standardmäßig in einem benutzerdefinierten Formular angezeigt.
   * Sie können Logikanweisungen für mehrere Felder erstellen.
   * Wenn auf alle Felder unter einem Abschnittsumbruch eine Anzeigereihenfolge angewendet wird und sie alle aufgrund der Logik ausgeblendet sind, wird der gesamte Abschnitt im benutzerdefinierten Formular ausgeblendet.

## Anzeigenlogik zu einem benutzerdefinierten Formular hinzufügen

Die Anzeigereihenfolge definiert, welche benutzerdefinierten Felder im Formular angezeigt werden, wenn der Benutzer einen bestimmten Wert in einem Multiple-Choice-Feld auswählt. Die Logik wird dem Zielfeld hinzugefügt, das nur bei Auswahl des Werts angezeigt wird.

{{step-1-to-setup}}

1. Klicks **Benutzerdefinierte Forms**.
1. Erstellen Sie ein neues benutzerdefiniertes Formular oder öffnen Sie ein vorhandenes Formular. Siehe [Formular mit dem Formularentwickler erstellen](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md) für Details.
1. Fügen Sie dem Formular nach Bedarf Felder hinzu. Vor dem anzuzeigenden Zielfeld muss mindestens ein Multiple-Choice-Feld (Optionsfeld, Dropdown-Menü oder Kontrollkästchen) positioniert werden.
1. Wählen Sie das Zielfeld aus und klicken Sie auf **Logik hinzufügen** unten links im Bildschirm.
1. Wählen Sie die **Anzeigelogik** Registerkarte.
1. Klicks **Anzeigenregel hinzufügen** auf dem Logikaufbau.

   ![Logikaufbau anzeigen](assets/custom-form-logic-builder-display-blank.png)

1. Führen Sie die folgenden Schritte im Builder aus, um die Logikanweisung zu erstellen.

   1. Die erste Option besteht darin, das definierende Feld auszuwählen. Dies ist das Feld mit dem Auswahlwert, das die Zielgruppe anzeigt. Es muss sich um ein Multiple-Choice-Feld handeln.
   1. Die zweite Option besteht darin, den Auswahlwert auszuwählen. Es sind nur die für dieses Feld bereits definierten Werte verfügbar.
   1. Die dritte Option ist **Ausgewählt** oder **Nicht ausgewählt**. Auswahl **Ausgewählt** bedeutet, dass bei Auswahl des Werts das Zielfeld angezeigt wird. Auswahl **Nicht ausgewählt** bedeutet, dass das Zielfeld angezeigt wird, wenn ein anderer Wert im Definitionsfeld ausgewählt ist.
   1. So fügen Sie eine **und** -Regel zur Logikanweisung hinzu, klicken Sie auf **Regel hinzufügen** direkt unterhalb der soeben erstellten Regel. Befolgen Sie dieselben Anweisungen zum Erstellen der Regel. Alle Und-Regeln müssen erfüllt sein, damit das Zielfeld angezeigt wird.

      ![Logikaufbau anzeigen](assets/custom-form-logic-builder-display1.png)

   1. So fügen Sie eine **Oder** -Regel zur Logikanweisung hinzu, klicken Sie auf **Regel hinzufügen** im unteren Bereich des Logikgenerators. Klicken Sie anschließend auf **Regel hinzufügen** innerhalb des Bereichs Oder und befolgen Sie dieselben Anweisungen zum Erstellen der Regel. Wenn eine Oder-Regel erfüllt ist, wird das Zielfeld angezeigt.

1. Klicks **Speichern** wenn Sie mit dem Erstellen der Logikanweisung fertig sind.

   Die Symbole für die Anzeigenlogik werden dem Zielfeld und dem Definitionsfeld im Formularentwickler hinzugefügt.

>[!NOTE]
>
>Die Anzeigelogik ist bei der Vorschau des Formulars im Formularentwickler vorübergehend nicht verfügbar.

## Logik zum Überspringen zu einem benutzerdefinierten Formular hinzufügen

Logik überspringen definiert benutzerdefinierte Formularfelder, die übersprungen werden, wenn der Benutzer einen bestimmten Wert in einem Multiple-Choice-Feld auswählt. Übersprungene Felder werden im Formular ausgeblendet. Die Logik wird auf das definierende Feld angewendet, in dem die Auswahl vorgenommen wird, nicht auf die Felder, die übersprungen werden.

{{step-1-to-setup}}

1. Klicks **Benutzerdefinierte Forms**.
1. Erstellen Sie ein neues benutzerdefiniertes Formular oder öffnen Sie ein vorhandenes Formular. Siehe [Formular mit dem Formularentwickler erstellen](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md) für Details.
1. Fügen Sie dem Formular nach Bedarf Felder hinzu. Das definierende Feld für die Logik zum Überspringen muss ein Multiple-Choice-Feld sein (Optionsfeld, Dropdown-Menü oder Kontrollkästchen).
1. Wählen Sie das definierende Feld aus und klicken Sie auf **Logik hinzufügen** unten links im Bildschirm.
1. Wählen Sie die **Logik überspringen** Registerkarte.
1. Klicks **Regel zum Überspringen hinzufügen** auf dem Logikaufbau.

   ![Logikaufbau überspringen](assets/custom-form-logic-builder-skip-blank.png)

1. Führen Sie die folgenden Schritte im Builder aus, um die Logikanweisung zu erstellen.

   1. Das definierende Feld wird im Builder angezeigt. Dies ist das Feld, auf das Sie die Logik zum Überspringen angewendet haben.
   1. Die erste Option besteht darin, den Auswahlwert auszuwählen. Es sind nur die für das Feld bereits definierten Werte verfügbar.
   1. Die zweite Option lautet **Ausgewählt** oder **Nicht ausgewählt**. Auswahl **Ausgewählt** bedeutet, dass bei Auswahl des Werts das Zielfeld angezeigt und die dazwischen liegenden Felder übersprungen werden. Auswahl **Nicht ausgewählt** bedeutet, dass bei Auswahl eines anderen Werts im definierenden Feld das Zielfeld angezeigt und die dazwischen liegenden Felder übersprungen werden.
   1. Die dritte Option ist das Zielfeld oder der Ort, zu dem übersprungen werden soll. Wählen Sie einen Feldnamen oder **Formularende**. Möglicherweise müssen Sie zuerst auf das Wort &quot;leer&quot;klicken, bevor Sie eine Option auswählen.

      ![Logikaufbau überspringen](assets/custom-form-logic-builder-skip1.png)

   1. So fügen Sie eine **Oder** -Regel zur Logikanweisung hinzu, klicken Sie auf **Regel hinzufügen** im unteren Bereich des Logikgenerators. Wählen Sie dann die Optionen aus, die denselben Aufforderungen zum Erstellen der Regel folgen. Wenn eine **Oder** -Regel erfüllt ist, wird das Zielfeld angezeigt.

1. Klicks **Speichern** wenn Sie mit dem Erstellen der Logikanweisung fertig sind.

   Die Symbole für die Logik überspringen werden dem Zielfeld und dem Definitionsfeld im Formularentwickler hinzugefügt.

>[!NOTE]
>
>Die Logik zum Überspringen ist bei der Vorschau eines Formulars im Formularentwickler vorübergehend nicht verfügbar.
