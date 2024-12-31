---
product-area: projects
navigation-topic: manage-tasks
title: Aufgaben in einer Liste bearbeiten
description: Sie können Aufgabeninformationen in einer Aufgabenliste bearbeiten, indem Sie die in der Liste angezeigten Felder bearbeiten. Weitere Informationen zu anderen Möglichkeiten zum Bearbeiten von Aufgaben finden Sie unter Aufgaben bearbeiten .
author: Alina
feature: Work Management
exl-id: 2af81907-3657-459e-b780-65983e224ca8
source-git-commit: 1da2e6448f7ac6f4bd5bd76846fbfc1a23c3da77
workflow-type: tm+mt
source-wordcount: '2848'
ht-degree: 2%

---

# Aufgaben in einer Liste bearbeiten {#edit-tasks-in-a-list}

Sie können Aufgabeninformationen in einer Aufgabenliste bearbeiten, indem Sie die in der Liste angezeigten Felder bearbeiten. Weitere Informationen zu anderen Bearbeitungsmöglichkeiten für Aufgaben finden Sie unter [Aufgaben bearbeiten](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Arbeit oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene*</td> 
   <td> <p>Zugriff auf Aufgaben und Projekte bearbeiten</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Einschränkungen in Ihrer Zugriffsebene festgelegt hat. Informationen dazu, wie Workfront-Admins Ihre Zugriffsebene ändern können, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Erstellen oder Ändern benutzerdefinierter Zugriffsebenen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Contribute oder höhere Berechtigungen für die Aufgabe und das Projekt</p> <p>Informationen zum Anfordern zusätzlicher Zugriffsberechtigungen finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Anfordern von Zugriffsberechtigungen für Objekte </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um herauszufinden, über welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie verfügen.

## Überlegungen zum Bearbeiten von Aufgaben in einer Liste {#considerations-about-editing-tasks-in-a-list}

Das Bearbeiten von Aufgaben in einer Liste ist eine schnelle Möglichkeit, Änderungen an mehreren Aufgaben gleichzeitig vorzunehmen, wobei klar erkennbar ist, wie sich Ihre Änderungen auf die Projektzeitleiste auswirken können.

Beachten Sie beim Bearbeiten von Aufgaben in einer Liste Folgendes:

* Anders als bei der Bearbeitung im Bearbeitungsfeld Berechtigungen verwalten für die Aufgabe benötigen, können Sie eine Aufgabe in einer Liste nur mit Contribute-Berechtigungen für die Aufgabe bearbeiten. Auf diese Weise können Sie die folgenden eingeschränkten Informationen für die Aufgabe bearbeiten:

   * Beschreibung
   * Status
   * Prozent abgeschlossen
   * Informationen zu benutzerdefinierten Formularen

     >[!NOTE]
     >
     >Sie können ein benutzerdefiniertes Aufgabenfeld in einer Liste nur bearbeiten, wenn Sie über die Berechtigung zum Aktualisieren des Felds verfügen.

   * Stunden protokollieren
   * Zuweisungen ändern
   * Finanzinformationen anzeigen
   * Kosten, Aufgaben oder Probleme hinzufügen

* Sie können eine Aufgabe in den folgenden Listen bearbeiten:

   * Der Abschnitt Aufgaben des Projekts
   * Der Abschnitt Teilaufgaben des Projekts
   * Aufgabenbericht

     >[!NOTE]
     >
     >Standardmäßig speichert Workfront Ihre Änderungen an Aufgaben automatisch im Abschnitt Teilaufgaben oder in einem Aufgabenbericht.

* Sie können steuern, wann Workfront die Änderungen an den Aufgaben in einer Liste speichert. Ihre Änderungen können automatisch oder manuell gespeichert werden.

  Informationen zum Konfigurieren der Änderungen, die Sie an Aufgaben in einer Liste vornehmen, wenn Workfront die Änderungen speichert, finden Sie im Abschnitt [Auswählen einer Speicheroption beim Bearbeiten von Aufgaben in einer ](#select-a-save-option-when-editing-tasks-in-a-list)) dieses Artikels.

* Andere Benutzer müssen ihre Seiten aktualisieren, bevor sie die Aktualisierungen sehen können, die Sie an einer Aufgabe vornehmen.

## Wählen Sie beim Bearbeiten von Aufgaben in einer Liste eine Speicheroption aus. {#select-a-save-option-when-editing-tasks-in-a-list}

Sie können festlegen, wo die Änderungen, die Sie an Aufgaben in einer Liste vornehmen, automatisch gespeichert werden, sobald sie auftreten, oder ob Sie jede Änderung manuell speichern möchten.

>[!IMPORTANT]
>
>Je nachdem, ob Sie die Aufgaben automatisch oder manuell speichern, können Sie die Informationen einer anderen Person überschreiben, während Sie Aufgaben in einer Liste bearbeiten. Informationen dazu, wie Workfront Änderungen an Aufgaben speichert, die Sie gleichzeitig mit anderen Benutzern ausführen, finden Sie unter [Übersicht über das Speichern gleichzeitiger Änderungen in einer Aufgabenliste](../../../manage-work/tasks/manage-tasks/save-concurrent-changes-in-a-task-list.md).

Wenn Sie Ihre Änderungen in einer Liste für ein Projekt speichern, für das entweder „Automatisch“ oder „Automatisch“ und „Bei Änderung“ als Aktualisierungstyp ausgewählt ist, aktualisiert Workfront die Projekt-Zeitleiste zusammen mit allen projektinternen und projektübergreifenden Abhängigkeiten. Zeitleistenberechnungen können lange dauern, wenn das Projekt groß ist oder viele Abhängigkeiten vorhanden sind. Einige Methoden zum Bearbeiten einer Aufgabenliste können schneller sein als andere, je nachdem, welche Methode Sie zum Speichern Ihrer Änderungen ausgewählt haben.

Sie können steuern, wann Workfront die Änderungen an den Aufgaben in einer Liste speichert. Die folgenden Szenarien sind vorhanden: 

* Sie können Workfront nach jeder Aktualisierung die Änderungen automatisch speichern lassen.

  Weitere Informationen finden Sie im Abschnitt [Bearbeiten von Aufgaben in einer Liste und automatisches Speichern ](#edit-tasks-in-a-list-and-automatically-save-changes) Änderungen“ in diesem Artikel.

* Sie können steuern, wann Sie mehrere Änderungen gleichzeitig anwenden, indem Sie eine Schaltfläche Speichern manuell verwenden.

  Weitere Informationen finden Sie im Abschnitt [Bearbeiten von Aufgaben in einer Liste und manuelles Speichern ](#edit-tasks-in-a-list-and-manually-save-changes) Änderungen“ in diesem Artikel.

### Aufgaben in einer Liste bearbeiten und Änderungen automatisch speichern {#edit-tasks-in-a-list-and-automatically-save-changes}

>[!TIP]
>
>Das Speichern Ihrer Änderungen und aller Projektabhängigkeiten kann langsamer sein, wenn Ihr Projekt mehr als 2.000 Aufgaben hat oder wenn es viele Abhängigkeiten hat.

Beachten Sie beim automatischen Speichern der Aufgabenlisten-Änderungen Folgendes:

* Sie können eine benutzerdefinierte Ansicht auf die Aufgabenliste anwenden und alle aufgabenbezogenen Felder bearbeiten, auf die Sie Zugriff haben, um sie zu aktualisieren.
* Automatische Änderungen können nicht rückgängig gemacht werden. Dies ist die Standardeinstellung.
* Workfront berechnet die Zeitleiste des Projekts und alle projektinternen und projektübergreifenden Abhängigkeiten nach jeder Änderung automatisch neu, wenn der Projektaktualisierungstyp „Automatisch“ oder „Automatisch“ und „Bei Änderung“ ist. Informationen zum Projektaktualisierungstyp finden Sie unter [Auswahl des Projektaktualisierungstyps](../../../manage-work/projects/manage-projects/select-project-update-type.md).

So bearbeiten Sie Aufgaben in einer Liste und speichern die Änderungen automatisch:

1. Gehen Sie zum Projekt und klicken Sie dann auf den Abschnitt **Aufgaben**.
1. Klicken Sie oben in der Liste auf **Menü** Planmodus![](assets/qs-list-mode-or-save-mode-icon-small.png) und stellen Sie sicher, dass die Option **Automatisches Speichern** ausgewählt ist.

   ![](assets/autosave-setting-enabled-quicksilver-task-list-350x308.png)

1. Bearbeiten Sie alle Felder, für die Sie über die Berechtigung zum manuellen Aktualisieren verfügen.

   ![](assets/inline-editing-a-task-350x26.png)

1. (Optional) Drücken Sie **Esc**, um Ihre Änderungen zu verwerfen.
1. Drücken Sie die Eingabetaste , um Ihre Änderungen an den Aufgaben und in der Projekt-Zeitleiste zu speichern.
1. (Optional) Klicken Sie mit der rechten Maustaste auf eine Aufgabe, die Sie ändern möchten.

   Oder

   Klicken Sie auf das **Mehr**-Menü ![](assets/more-icon-task-list.png) rechts neben dem Aufgabennamen.

1. (Optional) Wählen Sie aus den folgenden Optionen aus:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>In neuer Registerkarte öffnen</strong></td> 
      <td>Öffnet die Aufgabe in einer neuen Browser-Registerkarte. </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Bearbeiten</strong></td> 
      <td><p>Öffnet das Feld <strong>Aufgabe bearbeiten</strong> in dem Sie die Aufgabe bearbeiten können.</p><p>Informationen zum Bearbeiten einer Aufgabe finden Sie unter <a href="#edit-tasks-in-a-list" class="MCXref xref">Aufgaben in einer Liste bearbeiten</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Löschen</td> 
      <td><p>Löscht die Aufgabe.</p><p>Informationen zum Löschen von Aufgaben finden Sie unter <a href="../../../manage-work/tasks/manage-tasks/delete-tasks.md" class="MCXref xref">Aufgaben löschen</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Einrücken</td> 
      <td><p>Zieht die Aufgabe um eine Ebene ein. </p><p>Diese Option wird nur bei eigenständigen Aufgaben angezeigt.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ausrücken</td> 
      <td><p>Richtet die Aufgabe um eine Ebene aus </p><p>Diese Option wird nur für untergeordnete Aufgaben angezeigt. </p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Aufgabe oben einfügen</td> 
      <td>Fügt eine Aufgabe oberhalb der ausgewählten Aufgabe ein.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Aufgabe unten einfügen</td> 
      <td>Fügt eine Aufgabe unter der ausgewählten Aufgabe ein</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Duplizieren</td> 
      <td><p>Erstellt eine doppelte Version der Aufgabe innerhalb desselben Projekts. </p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Kopieren in</td> 
      <td><p>Kopiert die Aufgabe in ein anderes Projekt.</p><p>Informationen zum Kopieren und Duplizieren von Aufgaben finden Sie unter <a href="../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md" class="MCXref xref">Aufgaben kopieren und duplizieren</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Verschieben nach</td> 
      <td><p>Verschiebt die Aufgabe in ein anderes Projekt.</p><p>Informationen zum Verschieben von Aufgaben finden Sie unter <a href="../../../manage-work/tasks/manage-tasks/move-tasks.md" class="MCXref xref">Aufgaben verschieben</a>.</p></td> 
     </tr> 
    </tbody> 
   </table>

   Änderungen werden automatisch gespeichert und können nicht rückgängig gemacht werden.

### Aufgaben in einer Liste bearbeiten und Änderungen manuell speichern {#edit-tasks-in-a-list-and-manually-save-changes}

Sie können Änderungen an Aufgaben in einer Liste manuell speichern. Wenn Sie Änderungen auf diese Weise speichern, können Sie diese vor dem Speichern umkehren.

>[!TIP]
>
>* Sie können Änderungen an Aufgaben in einer Liste nicht rückgängig machen, wenn Sie sie im Abschnitt Teilaufgaben oder in einem Aufgabenbericht bearbeiten.
>* Es gibt keine Einschränkungen bezüglich der Anzahl der Änderungen, die rückgängig gemacht werden können. Sie können sie alle einzeln umkehren, bis Sie den ursprünglichen Status der Aufgaben erreicht haben.
>

Beachten Sie beim manuellen Speichern von Änderungen in einer Aufgabenliste Folgendes:

* Um Aufgabenlistenänderungen manuell zu speichern, benötigen Sie Berechtigungen zum Verwalten der Aufgaben und des Projekts.
* Sie können das Projekt nicht bearbeiten. Die Option zum Bearbeiten des Projekts ist deaktiviert.
* Sie können die Informationen in der Kopfzeile des Projekts nicht aktualisieren. Sie können Folgendes nur tun, wenn Sie die Änderungen in der Aufgabenliste manuell speichern:

   * Projekt abonnieren.
   * Fügen Sie das Projekt Ihrer Favoritenliste hinzu.
   * Öffnen Sie eine Aufgabe, indem Sie in der Liste auf ihren Namen klicken.

* Aufgaben stapelweise bearbeiten. Das Bearbeitungssymbol ist deaktiviert, wenn mehrere Aufgaben ausgewählt werden.
* Workfront Trigger-Benachrichtigungen über Änderungen, die Sie an den Aufgaben vornehmen, erst nach dem Speichern der Änderungen.

Es gibt zwei Möglichkeiten, Änderungen an Aufgaben in einer Liste manuell zu speichern. Diese beiden Möglichkeiten werden nachfolgend beschrieben.

* [Änderungen in einer Aufgabenliste manuell speichern, wenn Sie die Option „Standard manuell speichern“ auswählen](#save-changes-in-a-task-list-manually-when-you-select-the-manual-save-standard-option)
* [Änderungen in einer Aufgabenliste manuell speichern, wenn Sie die Option „Manuelles Speichern der Zeitleistenplanung“ auswählen](#save-changes-in-a-task-list-manually-when-you-select-the-manual-save-timeline-planning-option)

#### Änderungen in einer Aufgabenliste manuell speichern, wenn Sie die Option „Standard manuell speichern“ auswählen {#save-changes-in-a-task-list-manually-when-you-select-the-manual-save-standard-option}

>[!TIP]
>
>Wenn Ihr Projekt über mehr als 2.000 Aufgaben verfügt oder viele Abhängigkeiten aufweist, kann es eine Weile dauern, bis Sie die Änderungen an Ihren Aufgaben und deren Auswirkungen auf alle Projektabhängigkeiten visuell erkennen können. In diesem Fall kann das Speichern der Änderungen länger dauern, wenn das Projekt mehr als 2.000 Aufgaben hat oder viele Abhängigkeiten aufweist.

Beachten Sie beim Aktualisieren von Aufgaben in einer Liste nach Auswahl der Option „Standard manuell speichern“ Folgendes:

* Sie können eine benutzerdefinierte Ansicht auf die Aufgabenliste anwenden und alle aufgabenbezogenen Felder bearbeiten, zu deren Verwaltung Sie in dieser Ansicht berechtigt sind.
* Workfront berechnet die Zeitleiste des Projekts und alle projektinternen und projektübergreifenden Abhängigkeiten, nachdem Sie auf „Speichern“ geklickt haben und der Projektaktualisierungstyp „Automatisch“ oder „Automatisch“ und „Bei Änderung“ ist. Informationen zum Projektaktualisierungstyp finden Sie unter [Auswahl des Projektaktualisierungstyps](../../../manage-work/projects/manage-projects/select-project-update-type.md).

So bearbeiten Sie Aufgaben in einer Liste bei Auswahl der Option „Manuelles Speichern - Standard“:

1. Wechseln Sie zu einem Projekt und klicken Sie dann auf den **Aufgaben** Abschnitt .
1. Klicken Sie auf **Planmodus**-![](assets/qs-list-mode-or-save-mode-icon-small.png) oben in der Liste und wählen Sie **Manuelles Speichern** aus. Klicken Sie dann auf **Standard** > **Apply**.

   ![](assets/manual-standard-setting-enabled-quicksilver-task-list-350x493.png)

   Es wird eine Symbolleisteneinstellung mit Optionen zum Rückgängigmachen, Wiederholen und Speichern von Änderungen angezeigt.

   ![](assets/undo,-redo,-save,-and-cancel-widget-for-task-list-350x65.png)

1. Klicken Sie in ein Feld, für das Sie über die Berechtigung zum manuellen Aktualisieren verfügen. Das Feld kann nun bearbeitet werden, und Sie können Ihre Änderungen vornehmen.

   ![](assets/inline-editing-a-task-350x26.png)

1. Drücken Sie die Eingabetaste , um die vorgenommenen Änderungen vorübergehend zu speichern.
1. (Optional) Klicken Sie auf das Symbol **Rückgängig** ![](assets/undo-icon-on-task-list.png), um eine Änderung rückgängig zu machen und ein Feld in den Originalzustand zurückzuversetzen.
1. (Optional und bedingt) Klicken Sie auf das Symbol **Wiederholen** ![](assets/redo-icon-on-task-list.png), um die rückgängig gemachte Änderung wiederherzustellen.

1. (Optional) Klicken Sie mit der rechten Maustaste auf eine Aufgabe, die Sie ändern möchten.

   Oder

   Klicken Sie auf die ![](assets/more-icon-task-list.png) **Mehr**.

1. (Optional) Wählen Sie aus den folgenden Optionen aus:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>In neuer Registerkarte öffnen</strong> </td> 
      <td>Öffnet die Aufgabe in einer neuen Browser-Registerkarte. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Löschen</td> 
      <td>Informationen zum Löschen von Aufgaben finden Sie unter <a href="../../../manage-work/tasks/manage-tasks/delete-tasks.md" class="MCXref xref">Aufgaben löschen</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Einrücken</td> 
      <td> <p>Zieht die Aufgabe um eine Ebene ein. </p> <p>Diese Option wird nur bei eigenständigen Aufgaben angezeigt.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ausrücken</td> 
      <td> <p>Richtet die Aufgabe um eine Ebene aus </p> <p>Diese Option wird nur für untergeordnete Aufgaben angezeigt. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Aufgabe oben einfügen</td> 
      <td>Fügt eine Aufgabe oberhalb der ausgewählten Aufgabe ein.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Aufgabe unten einfügen</td> 
      <td>Fügt eine Aufgabe unter der ausgewählten Aufgabe ein</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Duplizieren</td> 
      <td> <p>Erstellt eine doppelte Version der Aufgabe innerhalb desselben Projekts. </p> <p>Informationen zum Kopieren und Duplizieren von Aufgaben finden Sie unter <a href="../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md" class="MCXref xref">Aufgaben kopieren und duplizieren</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Workfront aktualisiert alle projektinternen und projektübergreifenden Abhängigkeiten, wenn Sie Änderungen an der Zeitleiste von Aufgaben vornehmen.
1. Klicken Sie **Speichern**, wenn Sie Ihre Aufgabenänderungen dauerhaft beibehalten und die Zeitleiste des Projekts speichern möchten.

#### Änderungen in einer Aufgabenliste manuell speichern, wenn Sie die Option „Manuelles Speichern der Zeitleistenplanung“ auswählen {#save-changes-in-a-task-list-manually-when-you-select-the-manual-save-timeline-planning-option}

Das Speichern Ihrer Änderungen und aller Projektabhängigkeiten ist schneller. Dies ist nicht für Projekte mit mehr als 2000 Aufgaben verfügbar.

>[!IMPORTANT]
>
>Es wird empfohlen, diese Option beim Bearbeiten einer großen Liste von Aufgaben mit mehr als einigen Hundert Aufgaben mit vielen Abhängigkeiten zu verwenden. Mit dieser Option können Sie Ihre Änderungen viel schneller visuell identifizieren als mit der Option „Manuelles Speichern“.

Beachten Sie bei Verwendung der Option „Manuelles Speichern der Zeitleistenplanung“ in einer Aufgabenliste Folgendes:

* Sie können die Option „Manuelles Speichern der Zeitleistenplanung“ nicht auf Projekte mit mehr als 2.000 Aufgaben anwenden.
* Benutzerdefinierte Ansichten, Filter oder Gruppierungen können nicht auf die Aufgabenliste angewendet werden. Die Dropdown-Menüs Ansicht, Filter und Gruppierung sowie das Symbol Agile-Ansicht sind deaktiviert. Die standardmäßig angewendete Ansicht enthält eine begrenzte Anzahl von Feldern.
* Die Zeitleiste des Projekts und alle projektinternen Abhängigkeiten werden nach jeder Änderung automatisch berechnet, wenn der Projektaktualisierungstyp „Automatisch“ oder „Automatisch“ und „Bei Änderung“ ist.
* Die projektübergreifenden Abhängigkeiten werden berechnet, nachdem Sie auf „Speichern“ geklickt haben, wenn der Projektaktualisierungstyp „Automatisch“ oder „Automatisch“ und „Bei Änderung“ ist. Informationen zum Projektaktualisierungstyp finden Sie unter [Auswahl des Projektaktualisierungstyps](../../../manage-work/projects/manage-projects/select-project-update-type.md).

So bearbeiten Sie Aufgaben in einer Liste mithilfe der Option „Manuelles Speichern der Zeitleistenplanung“:

1. Wechseln Sie zu einem Projekt und klicken Sie dann auf den Abschnitt **Aufgaben**.
1. Klicken Sie oben in der Liste auf **Planmodus**-![](assets/qs-list-mode-or-save-mode-icon-small.png) und wählen Sie **Manuelles Speichern** aus. Klicken Sie dann auf **Timeline Planning**> **Apply**.

   Diese Option ist bei Projekten mit mehr als 2000 Aufgaben abgeblendet.

   ![](assets/manual-timeline-planning-setting-enabled-quicksilver-task-list-350x490.png)

   >[!TIP]
   >
   >Wenn Sie diese Seite verlassen, aktiviert Workfront die Option „Automatisches Speichern“ erneut.

   Beachten Sie die folgenden Änderungen in der Liste:

   * Die Dropdown-Menüs Ansicht, Gruppierung und Filter werden entfernt und die Ansicht wird durch die folgenden Felder ersetzt:

      * Aufgabennummer
      * Aufgabenname
      * Einschränkungstyp
      * Dauer
      * Geplantes Startdatum
      * Geplantes Abschlussdatum
      * Vorgänger
      * Arbeitsaufträge
      * Status
      * Prozent abgeschlossen

   * Das Symbol für die Agile-Ansicht wurde entfernt.
   * Es wird eine Symbolleisteneinstellung mit Optionen zum Rückgängigmachen, Wiederholen und Speichern von Änderungen angezeigt.

     ![](assets/undo,-redo,-save,-and-cancel-widget-for-task-list-350x65.png)

1. Bearbeiten Sie alle Felder, für die Sie über die Berechtigung zum manuellen Aktualisieren verfügen.

   ![](assets/inline-editing-a-task-350x26.png)

1. Drücken Sie die Eingabetaste , um die vorgenommenen Änderungen vorübergehend zu speichern.
1. (Optional) Klicken Sie auf das Symbol **Rückgängig** ![](assets/undo-icon-on-task-list.png), um eine Änderung rückgängig zu machen und ein Feld in den Originalzustand zurückzuversetzen.
1. (Optional und bedingt) Klicken Sie auf das Symbol **Wiederholen** ![](assets/redo-icon-on-task-list.png), um die rückgängig gemachte Änderung wieder aufzunehmen.

1. (Optional) Klicken Sie mit der rechten Maustaste auf eine Aufgabe, die Sie ändern möchten

   Oder

   Klicken Sie auf die ![](assets/more-icon-task-list.png) **Mehr**.

1. Wählen Sie aus den folgenden Optionen aus:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>In neuer Registerkarte öffnen</strong> </td> 
      <td>Öffnet die Aufgabe in einer neuen Browser-Registerkarte. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Löschen</td> 
      <td>Informationen zum Löschen von Aufgaben finden Sie unter <a href="../../../manage-work/tasks/manage-tasks/delete-tasks.md" class="MCXref xref">Aufgaben löschen</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Einrücken</td> 
      <td> <p>Zieht die Aufgabe um eine Ebene ein. </p> <p>Diese Option wird nur bei eigenständigen Aufgaben angezeigt.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ausrücken</td> 
      <td> <p>Richtet die Aufgabe um eine Ebene aus </p> <p>Diese Option wird nur für untergeordnete Aufgaben angezeigt. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Aufgabe oben einfügen</td> 
      <td>Fügt eine Aufgabe oberhalb der ausgewählten Aufgabe ein.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Aufgabe unten einfügen</td> 
      <td>Fügt eine Aufgabe unter der ausgewählten Aufgabe ein</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Duplizieren</td> 
      <td> <p>Erstellt eine doppelte Version der Aufgabe innerhalb desselben Projekts. </p> <p>Informationen zum Kopieren und Duplizieren von Aufgaben finden Sie unter <a href="../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md" class="MCXref xref">Aufgaben kopieren und duplizieren</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Workfront aktualisiert alle projektinternen und projektübergreifenden Abhängigkeiten, wenn Sie die Zeitleiste einer Aufgabe ändern.
1. Klicken Sie **Speichern**, wenn Sie Ihre Aufgabenänderungen dauerhaft beibehalten und die Zeitleiste des Projekts speichern möchten.

## Aufgabe in einer Liste mithilfe der Zusammenfassung bearbeiten

1. Navigieren Sie zu dem Projekt, das die Aufgaben enthält, die Sie bearbeiten möchten.
1. Klicken Sie **linken** auf Aufgaben .

   Die Liste der Aufgaben für das Projekt wird angezeigt.

1. Klicken Sie auf das Menü Mehr ![](assets/more-icon-task-list.png) nach dem Aufgabennamen und dann auf **Zusammenfassung öffnen**. Wählen Sie die Aufgabe aus, die Sie bearbeiten möchten, und klicken Sie dann auf **Zusammenfassung öffnen** ![](assets/qs-open-summary-icon-in-new-toolbar-small.png) in der oberen rechten Ecke der Liste.

   Die **Zusammenfassung** wird geöffnet.

   ![](assets/qs-task-right-panel-in-a-task-list-350x328.png)

1. (Optional) Klicken Sie auf das **X**-Symbol oben rechts in der Zusammenfassung, um das Bedienfeld zu schließen und die Aufgaben inline zu bearbeiten.

   Führen Sie die Schritte zum Bearbeiten einer Aufgabe in einer Liste aus, um die Aufgabe inline zu bearbeiten.

   Informationen zum Bearbeiten der Aufgabe in einer Liste finden Sie unter [Überlegungen zum Bearbeiten von Aufgaben in einer Liste](#considerations-about-editing-tasks-in-a-list) in diesem Artikel.

1. (Optional) Geben Sie eine Aktualisierung für die Aufgabe im Bereich **Updates** ein.
1. Klicken Sie auf eines der folgenden Symbole oder Bereiche, um zur Aufgabe zu wechseln und Informationen auf Aufgabenebene zu bearbeiten:

   | Dokumente | Klicken Sie **Zum Hinzufügen hier klicken**, um der Aufgabe Dokumente hinzuzufügen. |
   |---|---|
   | Details | Klicken, um Informationen über die Aufgabe zu aktualisieren. |
   | Benutzerdefinierte Formulare | Klicken Sie, um benutzerdefinierte Forms hinzuzufügen oder zu entfernen oder die Informationen in den Formularen zu aktualisieren. |
   | Stunden | Klicken, um Stunden einzutragen. |
   | Genehmigungen | Klicken, um Aufgabengenehmigungen hinzuzufügen. |

   {style="table-layout:auto"}

1. Klicken Sie im Browser auf die Schaltfläche „Zurück“, um zur Aufgabenliste zurückzukehren, wenn Sie die Aktualisierung der Aufgabe abgeschlossen haben.

## Aufgaben stapelweise bearbeiten

Sie können mehrere Aufgaben gleichzeitig bearbeiten. Stellen Sie sicher, dass Sie über Verwaltungsberechtigungen für die Aufgaben verfügen, um sie bearbeiten zu können.

1. Navigieren Sie zu einem Projekt, das Aufgaben enthält, die Sie stapelweise bearbeiten möchten.
1. Klicken Sie **linken** auf „Aufgaben“.
1. Stellen Sie sicher **dass die Option &quot;**&quot; ausgewählt ist.

   >[!IMPORTANT]
   >
   >Beim manuellen Speichern von Aufgaben können Sie Aufgaben nicht stapelweise bearbeiten.

   Weitere Informationen zum Speichern von Änderungen an Aufgaben in einer Liste finden Sie im Abschnitt [Überlegungen zum Bearbeiten von Aufgaben in einer Liste](#considerations-about-editing-tasks-in-a-list) in diesem Artikel.

1. Mehrere Aufgaben in der Aufgabenliste auswählen.
1. Klicken Sie auf **Bearbeiten-Symbol** ![](assets/qs-edit-icon.png).

   Das **Aufgaben bearbeiten** wird geöffnet.

1. Geben Sie die Informationen an, die Sie für alle ausgewählten Aufgaben ändern möchten.

   Die Bearbeitung der Informationen für alle Aufgaben ist identisch mit der Bearbeitung der Informationen für eine Aufgabe. Wenn Sie die Aufgabendauer bearbeiten möchten, müssen die ausgewählten Aufgaben dieselbe Vorgangseinschränkung aufweisen. Andernfalls wird das Feld **Dauer** nicht ausgefüllt.

   Weitere Informationen zum Bearbeiten einer Aufgabe finden Sie unter [Aufgaben bearbeiten](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

   >[!NOTE]
   >
   >Die Informationen, die Sie zu allen ausgewählten Aufgaben ändern, überschreiben die vorhandenen Informationen zu einzelnen Aufgaben, mit Ausnahme des Felds **Arbeitsaufträge**. Wenn Sie einen neuen Verantwortlichen in der Massenbearbeitung hinzufügen, wird dieser Verantwortliche allen ausgewählten Aufgaben hinzugefügt. Wenn den ausgewählten Aufgaben andere Verantwortliche zugewiesen werden, bleiben diese zusätzlich zu der durch Massenbearbeitung hinzugefügten zugewiesen.

1. Klicken Sie **Benutzerdefinierte Forms**, um die benutzerdefinierten Formulare zu bearbeiten, die an alle ausgewählten Aufgaben angehängt sind. In der Liste werden nur aktive benutzerdefinierte Formulare angezeigt.

   Wenn die ausgewählten Aufgaben keine benutzerdefinierten Formulare gemeinsam haben, werden in diesem Abschnitt keine Formulare aufgelistet.

   Sie können nur die Felder in den Formularen bearbeiten, die an alle ausgewählten Aufgaben angehängt sind und für die Sie über die Berechtigung zum Bearbeiten verfügen.

1. (Optional) Wählen Sie im Abschnitt Benutzerdefinierte Forms die Option **Benutzerdefinierte Ausdrücke neu berechnen** aus, um sicherzustellen, dass alle berechneten benutzerdefinierten Felder in den benutzerdefinierten Formularen, die an die ausgewählten Aufgaben angehängt sind, auf dem neuesten Stand sind.
1. Klicken Sie auf **Änderungen speichern**.

   Alle von Ihnen vorgenommenen Änderungen sind nun für alle ausgewählten Aufgaben sichtbar.

Informationen zur Massenbearbeitung benutzerdefinierter Formulare finden Sie im Abschnitt „Bearbeiten mehrerer benutzerdefinierter Forms bei der Massenbearbeitung von Objekten“ in [Verwalten benutzerdefinierter Formulare, die an Objekte angehängt ](../../../workfront-basics/work-with-custom-forms/manage-custom-forms-attached-to-objects.md).
