---
title: Hinzufügen einer Anzeigelogik und Überspringen einer Logik zu einem Formular
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: Sie können festlegen, welche Abschnitte eines benutzerdefinierten Formulars angezeigt oder übersprungen werden sollen, je nachdem, welche Auswahl ein Benutzer beim Ausfüllen trifft.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 5f5dbeb5-b974-489c-8f4d-ebaa00f5e5ba
source-git-commit: 554e08c22f6ee142a9ced8fa991d0126b6360b0c
workflow-type: tm+mt
source-wordcount: '1318'
ht-degree: 0%

---

# Hinzufügen einer Anzeigelogik und Überspringen einer Logik zu einem Formular

Sie können festlegen, welche Abschnitte eines benutzerdefinierten Formulars angezeigt oder übersprungen werden sollen, je nachdem, welche Auswahl ein Benutzer beim Ausfüllen trifft.

>[!NOTE]
>
>Logik gilt nur innerhalb eines Formulars und kann nicht auf Auswahlen aus einem anderen Formular basieren.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Adobe Workfront-Plan </td> 
   <td>Beliebig</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td>
   <p>Neu: Standard</p>
   <p>oder</p>
   <p>Aktuell: Plan</p></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td>Administrativer Zugriff auf benutzerdefinierte Formulare </td> 
  </tr>  
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Logiksymbole anzeigen und überspringen

Benutzerdefinierte Formulare zeigen Symbole an, um anzugeben, welche Logik auf bestimmte Felder angewendet wird. Symbole auf einem Feld im Formular-Designer geben an, dass Logik auf das Feld angewendet wird.

| Symbol | Speicherort auf dem Feld im Formular-Designer | Definition |
|--- |--- |--- |
| ![Anzeigelogik für Zielfeld](assets/display-logic-bottom-left.png) | Unten links | Das Feld ist das Zielfeld für die Anzeigelogik. Wenn eine bestimmte Auswahl im Formular vorgenommen wird, wird dieses Feld angezeigt. |
| ![Symbol für Anzeigelogik definieren](assets/display-logic-bottom-right.png) | Unten rechts | Das Feld definiert die Anzeigelogik. Eine bestimmte Auswahl oder ein bestimmter Wert in diesem Feld zeigt das Zielfeld an. |
| ![Logik für Zielfeld überspringen](assets/skip-logic-bottom-left.png) | Unten links | Das Feld ist das Zielfeld für die Logik zum Überspringen . Wenn eine bestimmte Auswahl im Formular vorgenommen wird, springt das Formular zu diesem Feld weiter und die Felder dazwischen werden ausgeblendet. |
| ![Logiksymbol zum Überspringen definieren](assets/skip-logic-bottom-right.png) | Unten rechts | Das Feld definiert die Logik zum Überspringen. Eine bestimmte Auswahl oder ein bestimmter Wert in diesem Feld überspringt andere Felder und wechselt direkt zum Zielfeld. |

![Logiksymbole](assets/logic-icons-3.png)

Wählen Sie ein Feld mit angewendeter Logik aus, um die vorhandenen Logikregeln in den Feldeinstellungen anzuzeigen.

![Logische Regeln](assets/form-designer-view-only-logic.png)

## Überlegungen zur Verwendung der Anzeigelogik und zum Überspringen der Logik

* Um Anzeigelogik zu einem benutzerdefinierten Feld, Widget oder Abschnittsumbruch hinzuzufügen, muss mindestens ein Multiple-Choice-Feld (Optionsfelder, Dropdown-Listen oder Kontrollkästchen) vor dem Feld im Formular positioniert werden.
Informationen zu benutzerdefinierten Feldern und Widgets in benutzerdefinierten Formularen finden Sie unter [Erstellen eines benutzerdefinierten Formulars](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).
* Sie können keine Logik zum Überspringen zu einem Widget oder Abschnittsumbruch hinzufügen. Sie können sie nur einem Multiple-Choice-Feld hinzufügen (Optionsschaltflächen, Dropdown-Liste oder Kontrollkästchen).
* Es ist nicht möglich, eine Logik zum Anzeigen oder Überspringen anzuwenden, um die Auswahl eines Felds mit mehreren Optionen ein- oder auszublenden. Sie können beispielsweise die Auswahl, die für ein Dropdown-Feld, eine Kontrollkästchen-Gruppe oder ein Optionsfeld angezeigt wird, nicht auf der Grundlage der Anzeige- oder Überspringen-Logik eines anderen Felds einschränken.
* Sie können sowohl Anzeigelogik als auch Überspringen-Logik zu einem benutzerdefinierten Feld hinzufügen, wenn Folgendes für das benutzerdefinierte Feld zutrifft:

   * Es handelt sich um ein Feld mit Mehrfachauswahl (Optionsfelder, Dropdown oder Kontrollkästchen)
   * Ihm geht ein Multiple-Choice-Feld voran
   * Darauf folgt ein weiteres benutzerdefiniertes Feld

* Beim Kopieren von Formularen mit Anzeigelogik oder Überspringen wird die Logik in das neue benutzerdefinierte Formular kopiert.
* Bei der Massenbearbeitung von Objekten werden alle benutzerdefinierten Felder im Feld Objekte bearbeiten angezeigt, einschließlich der übersprungenen oder ausgeblendeten Felder.
* Beachten Sie Folgendes, wenn Sie eine Anzeigelogik-Regel für ein benutzerdefiniertes Formular erstellen:

   * Benutzerdefinierte Felder, die nicht in einer Display-Logikanweisung enthalten sind, werden standardmäßig in einem benutzerdefinierten Formular angezeigt.
   * Sie können Logikanweisungen mit mehreren Feldern erstellen.
   * Wenn auf alle Felder unter einem Abschnittsumbruch eine Anzeigelogik angewendet wurde und sie infolge der Logik alle ausgeblendet sind, wird der gesamte Abschnitt im benutzerdefinierten Formular ausgeblendet.

## Hinzufügen einer Anzeigelogik zu einem benutzerdefinierten Formular

Die Anzeigelogik definiert, welche benutzerdefinierten Felder im Formular angezeigt werden, wenn Benutzende einen bestimmten Wert in einem Multiple-Choice-Feld auswählen. Die Logik wird dem Zielfeld hinzugefügt, das nur angezeigt wird, wenn der Wert ausgewählt ist.

{{step-1-to-setup}}

1. Klicken Sie **Benutzerdefinierte Forms**.
1. Ein neues benutzerdefiniertes Formular erstellen oder ein vorhandenes Formular öffnen. Siehe [Erstellen eines benutzerdefinierten Formulars](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md) für Details.
1. Fügen Sie dem Formular nach Bedarf Felder hinzu. Mindestens ein Multiple-Choice-Feld (Optionsfeld, Dropdown oder Kontrollkästchen) muss vor dem Zielfeld positioniert werden, das angezeigt wird.
1. Wählen Sie das Zielfeld aus und klicken **unten links** Bildschirm auf „Logik hinzufügen“.
1. Wählen Sie die **Anzeigelogik** aus.
1. Klicken Sie **Logik-Builder auf** Anzeigeregel hinzufügen“.

   ![Display Logic Builder](assets/custom-form-logic-builder-display-blank.png)

1. Gehen Sie im Builder wie folgt vor, um die logische Anweisung zu erstellen.

   1. Die erste Option besteht darin, das definierende Feld auszuwählen. Dies ist das Feld mit dem Auswahlwert, der die Zielgruppe anzeigt. Es muss ein Multiple-Choice-Feld sein.
   1. Die zweite Option besteht darin, den Auswahlwert auszuwählen. Nur die für dieses Feld bereits definierten Werte sind verfügbar.
   1. Die dritte Option ist **Ausgewählt** oder **Nicht ausgewählt**. Die Auswahl **Ausgewählt** bedeutet, dass bei Auswahl des Werts das Zielfeld angezeigt wird. Die Auswahl **Nicht ausgewählt** bedeutet, dass das Zielfeld angezeigt wird, wenn ein anderer Wert im definierenden Feld ausgewählt wird.
   1. Um eine Und **Regel** die Logikanweisung hinzuzufügen, klicken Sie **Regel hinzufügen** direkt unter der soeben erstellten Regel. Befolgen Sie die gleichen Anweisungen, um die Regel zu erstellen. Alle - und -Regeln müssen erfüllt sein, damit das Zielfeld angezeigt wird.

      ![Display Logic Builder](assets/custom-form-logic-builder-display1.png)

   1. Um eine **OR**-Regel zur Logikanweisung hinzuzufügen, klicken Sie **Regel hinzufügen** unten im Logik-Builder. Klicken Sie dann im Bereich **auf „Regel hinzufügen** und folgen Sie denselben Anweisungen, um die Regel zu erstellen. Wenn eine OR-Regel erfüllt ist, wird das Zielfeld angezeigt.

1. Klicken Sie **Speichern** wenn Sie mit dem Erstellen der Logikanweisung fertig sind.

   Die Symbole für die Anzeigelogik werden dem Zielfeld und dem definierenden Feld im Formular-Designer hinzugefügt.

## Hinzufügen einer Logik zum Überspringen zu einem benutzerdefinierten Formular

Die Überspringen-Logik definiert benutzerdefinierte Formularfelder, die übersprungen werden, wenn Benutzende einen bestimmten Wert in einem Multiple-Choice-Feld auswählen. Übersprungene Felder werden im Formular ausgeblendet. Die Logik wird auf das definierende Feld angewendet, in dem die Auswahl getroffen wird, nicht auf die übersprungenen Felder.

{{step-1-to-setup}}

1. Klicken Sie **Benutzerdefinierte Forms**.
1. Ein neues benutzerdefiniertes Formular erstellen oder ein vorhandenes Formular öffnen. Siehe [Erstellen eines benutzerdefinierten Formulars](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md) für Details.
1. Fügen Sie dem Formular nach Bedarf Felder hinzu. Das definierende Feld für die Logik zum Überspringen muss ein Multiple-Choice-Feld sein (Optionsfeld, Dropdown oder Kontrollkästchen).
1. Wählen Sie das definierende Feld aus und klicken **unten links** Bildschirm auf „Logik hinzufügen“.
1. Wählen Sie die **Logik überspringen** aus.
1. Klicken Sie **Logikgenerator auf** Regel zum Überspringen hinzufügen“.

   ![Logikgenerator überspringen](assets/custom-form-logic-builder-skip-blank.png)

1. Gehen Sie im Builder wie folgt vor, um die logische Anweisung zu erstellen.

   1. Das definierende Feld wird im Builder angezeigt. Dies ist das Feld, auf das Sie die Logik zum Überspringen angewendet haben.
   1. Die erste Option besteht darin, den Auswahlwert auszuwählen. Nur die bereits für das Feld definierten Werte sind verfügbar.
   1. Die zweite Option ist **Ausgewählt** oder **Nicht ausgewählt**. Die Auswahl **Ausgewählt** bedeutet, dass bei Auswahl des Werts das Zielfeld angezeigt wird und die Felder dazwischen übersprungen werden. Die Auswahl **Nicht ausgewählt** bedeutet, dass, wenn ein anderer Wert im definierenden Feld ausgewählt ist, das Zielfeld angezeigt wird und die Felder dazwischen übersprungen werden.
   1. Die dritte Option ist das Zielfeld oder der Ort, zu dem Sie wechseln möchten. Wählen Sie einen Feldnamen oder &quot;**des Formulars“**. Möglicherweise müssen Sie zuerst auf das Wort „leer“ klicken, bevor Sie eine Option auswählen.

      ![Logikgenerator überspringen](assets/custom-form-logic-builder-skip1.png)

   1. Um eine **OR**-Regel zur Logikanweisung hinzuzufügen, klicken Sie **Regel hinzufügen** unten im Logik-Builder. Wählen Sie dann die Optionen aus, die denselben Aufforderungen folgen, um die Regel zu erstellen. Wenn eine **Oder**-Regel erfüllt ist, wird das Zielfeld angezeigt.

1. Klicken Sie **Speichern** wenn Sie mit dem Erstellen der Logikanweisung fertig sind.

   Die Symbole zum Überspringen werden dem Zielfeld und dem definierenden Feld im Formular-Designer hinzugefügt.


