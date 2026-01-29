---
product-area: projects
navigation-topic: manage-tasks
title: Aufgaben in einer Liste bearbeiten
description: Sie können Aufgabeninformationen in einer Aufgabenliste bearbeiten, indem Sie die in der Liste angezeigten Felder bearbeiten. Sie müssen den Planungsmodus in einer Aufgabenliste definieren, um anzugeben, wie Ihre Änderungen in Workfront gespeichert werden sollen. Sie können Ihre Änderungen manuell oder automatisch speichern.
author: Alina
feature: Work Management
exl-id: 2af81907-3657-459e-b780-65983e224ca8
source-git-commit: 665e753880be59cf07062d75c66a7be5f2056aa1
workflow-type: tm+mt
source-wordcount: '3233'
ht-degree: 3%

---

# Aufgaben in einer Liste bearbeiten {#edit-tasks-in-a-list}

<!-- Audited: 10/2025 -->

<div class="preview">

Die hervorgehobenen Informationen auf dieser Seite beziehen sich auf Funktionen, die noch nicht allgemein verfügbar sind. Sie ist nur in der Vorschau -Umgebung für alle Kunden verfügbar. Dieselben Funktionen sind ab einer Woche ab der Vorschau-Version auch in der Produktionsumgebung für alle Kunden verfügbar.

Weitere Informationen finden Sie unter [Schnittstellenmodernisierung](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md).

</div>

Sie können Aufgabeninformationen in einer Aufgabenliste bearbeiten, indem Sie die in der Liste angezeigten Felder bearbeiten. Weitere Informationen zu anderen Bearbeitungsmöglichkeiten für Aufgaben finden Sie unter [Aufgaben bearbeiten](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Paket</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td> <p>Standard<p>
   <p>Work oder höher</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriff auf Aufgaben und Projekte bearbeiten</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Mitwirken an oder höhere Berechtigungen für die Aufgabe und das Projekt</p></td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++ 

<!--Old:
<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td> <p>New: Standard<p>
   <p>Current: Work or higher</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to Tasks and Projects</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Contribute or higher permissions to the task and the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Überlegungen zum Bearbeiten von Aufgaben in einer Liste {#considerations-about-editing-tasks-in-a-list}

Das Bearbeiten von Aufgaben in einer Liste ist eine schnelle Möglichkeit, Änderungen an mehreren Aufgaben gleichzeitig vorzunehmen, mit einem klaren Überblick darüber, wie sich Ihre Änderungen auf die Projektzeitleiste auswirken können.

Beachten Sie beim Bearbeiten von Aufgaben in einer Liste Folgendes:

* Anders als bei der Bearbeitung im Bearbeitungsfeld Berechtigungen für die Aufgabe verwalten müssen, können Sie eine Aufgabe in einer Liste nur mit den Berechtigungen Beitragen zur Aufgabe bearbeiten. Auf diese Weise können Sie die folgenden eingeschränkten Informationen für die Aufgabe bearbeiten:

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

* Sie können steuern, wann Workfront die an den Aufgaben vorgenommenen Änderungen in einer Liste speichert, indem Sie den Planungsmodus definieren, bevor Sie mit der Bearbeitung der Aufgaben beginnen.

  Sie können sich entscheiden, ob Workfront die von Ihnen vorgenommenen Änderungen wie folgt speichert:

   * Automatisch, nach jeder Änderung
   * Manuell, erst nachdem Sie auf Speichern geklickt haben.

  Informationen zum Konfigurieren, wann Workfront Änderungen an Aufgaben in einer Liste speichert, finden Sie im Abschnitt [Ändern des Planungsmodus vor dem Bearbeiten von Aufgaben in einer Liste](#modify-plan-mode-before-editing-tasks-in-a-list) in diesem Artikel.

* Andere Benutzer müssen ihre Seiten aktualisieren, bevor sie die Aktualisierungen sehen können, die Sie an einer Aufgabe vornehmen.

## Ändern des Planungsmodus vor der Bearbeitung von Aufgaben in einer Liste

Sie können entscheiden, ob die Änderungen, die Sie an Aufgaben in einer Liste vornehmen, automatisch gespeichert werden, sobald sie auftreten, oder ob Sie jede Änderung manuell speichern möchten. Dazu müssen Sie den Planungsmodus in einer Aufgabenliste ändern, bevor Sie die Aufgaben bearbeiten.

>[!IMPORTANT]
>
>Je nachdem, ob Sie die Aufgaben automatisch oder manuell speichern, können Sie die Informationen einer anderen Person überschreiben, während Sie Aufgaben in einer Liste bearbeiten. Weitere Informationen finden Sie unter [Übersicht über das Speichern gleichzeitiger Änderungen in einer Aufgabenliste](../../../manage-work/tasks/manage-tasks/save-concurrent-changes-in-a-task-list.md).

Wenn Sie Ihre Änderungen in einer Liste für ein Projekt speichern, für das entweder „Automatisch“ oder „Automatisch“ und „Bei Änderung“ als Aktualisierungstyp ausgewählt ist, aktualisiert Workfront die Projekt-Zeitleiste zusammen mit allen projektinternen und projektübergreifenden Abhängigkeiten. Zeitleistenberechnungen können lange dauern, wenn das Projekt groß ist oder viele Abhängigkeiten vorhanden sind. Einige Methoden zum Bearbeiten einer Aufgabenliste können schneller sein als andere, je nachdem, welche Methode Sie zum Speichern Ihrer Änderungen ausgewählt haben.

Sie können steuern, wann Workfront die Änderungen an den Aufgaben in einer Liste speichert. Die folgenden Szenarien sind vorhanden:

* Sie können Workfront nach jeder Aktualisierung die Änderungen automatisch speichern lassen.

  Weitere Informationen finden Sie im Abschnitt [Festlegen des Planungsmodus zum automatischen Speichern von Änderungen](#set-the-plan-mode-to-automatically-save-changes) in diesem Artikel.

* Sie können steuern, wann Sie mehrere Änderungen gleichzeitig anwenden, indem Sie eine Schaltfläche Speichern manuell verwenden.

  Weitere Informationen finden Sie im Abschnitt [Festlegen des Planungsmodus zum manuellen Speichern von Änderungen](#set-the-plan-mode-to-manually-save-changes) in diesem Artikel.

### Planmodus zum automatischen Speichern von Änderungen festlegen

>[!TIP]
>
>Das Speichern Ihrer Änderungen und aller Projektabhängigkeiten kann langsamer sein, wenn Ihr Projekt mehr als 2.000 Aufgaben hat oder wenn es viele Abhängigkeiten hat.

Beachten Sie beim automatischen Speichern der Aufgabenlisten-Änderungen Folgendes:

* Sie können eine benutzerdefinierte Ansicht auf die Aufgabenliste anwenden und alle aufgabenbezogenen Felder bearbeiten, auf die Sie Zugriff haben, um sie zu aktualisieren.
* Automatische Änderungen können nicht rückgängig gemacht werden. Dies ist die Standardeinstellung.
* Wenn als Projektaktualisierungstyp „Automatisch“ oder „Automatisch“ und „Bei Änderung“ festgelegt ist, berechnet Workfront die Zeitleiste des Projekts und alle projektinternen und projektübergreifenden Abhängigkeiten nach jeder Änderung automatisch neu. Informationen zum Projektaktualisierungstyp finden Sie unter [Auswahl des Projektaktualisierungstyps](../../../manage-work/projects/manage-projects/select-project-update-type.md).

So bearbeiten Sie Aufgaben in einer Liste und speichern die Änderungen automatisch:

{{step1-to-projects}}

1. Wählen Sie auf **Seite** ein Projekt aus.
1. Klicken Sie im linken Bedienfeld auf den Abschnitt **Aufgaben**.

1. Klicken Sie auf **Planmodus**-Symbol ![Planmodus-Symbol](assets/plan-mode-icon.png) oben in der Liste und stellen Sie sicher, dass die Option **Automatisches Speichern** ausgewählt ist.

   ![Aktivieren Sie die Einstellung für automatisches Speichern](assets/autosave-setting-enabled-quicksilver-task-list-350x308.png)

1. Bearbeiten Sie alle Felder, für die Sie über die Berechtigung zum manuellen Aktualisieren verfügen.

1. (Optional) Drücken Sie **Esc**, um Ihre Änderungen zu verwerfen.
1. Drücken Sie **Eingabetaste** (Windows) oder **Zurück** (Mac) auf der Tastatur, um Ihre Änderungen an den Aufgaben und der Projekt-Zeitleiste zu speichern.
1. (Optional) Klicken Sie mit der rechten Maustaste auf eine Aufgabe, die Sie ändern möchten.

   ODER

   Klicken Sie auf das **Mehr**-Menü ![](assets/more-icon-task-list.png) rechts neben dem Aufgabennamen.

1. (Optional) Wählen Sie aus den folgenden Optionen aus:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">In neuer Registerkarte öffnen</td> 
      <td>Öffnet die Aufgabe in einer neuen Browser-Registerkarte. </td> 
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
      <td role="rowheader">Bearbeiten</td> 
      <td><p>Öffnet das Feld Aufgabe bearbeiten, in dem Sie die Aufgabe bearbeiten können.</p><p>Informationen zum Bearbeiten einer Aufgabe finden Sie unter <a href="#edit-tasks-in-a-list" class="MCXref xref">Aufgaben in einer Liste bearbeiten</a>.</p></td> 
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
      <td role="rowheader">Duplizieren</td> 
      <td><p>Erstellt eine doppelte Version der Aufgabe innerhalb desselben Projekts. </p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Kopieren nach…</td> 
      <td><p>Kopiert die Aufgabe in ein anderes Projekt.</p><p>Informationen zum Kopieren und Duplizieren von Aufgaben finden Sie unter <a href="../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md" class="MCXref xref">Aufgaben kopieren und duplizieren</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Verschieben nach...</td> 
      <td><p>Verschiebt die Aufgabe in ein anderes Projekt.</p><p>Informationen zum Verschieben von Aufgaben finden Sie unter <a href="../../../manage-work/tasks/manage-tasks/move-tasks.md" class="MCXref xref">Aufgaben verschieben</a>.</p></td> 
     </tr> 
    </tbody> 
   </table>

### Planmodus zum manuellen Speichern von Änderungen festlegen {#edit-tasks-in-a-list-and-manually-save-changes}

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

Es gibt zwei Möglichkeiten, Änderungen an Aufgaben in einer Liste manuell zu speichern:

* [Änderungen in einer Aufgabenliste manuell speichern, wenn Sie die Option „Standard manuell speichern“ auswählen](#save-changes-in-a-task-list-manually-when-you-select-the-manual-save-standard-option)
* [Änderungen in einer Aufgabenliste manuell speichern, wenn Sie die Option „Manuelles Speichern der Zeitleistenplanung“ auswählen](#save-changes-in-a-task-list-manually-when-you-select-the-manual-save-timeline-planning-option)

#### Änderungen in einer Aufgabenliste manuell speichern, wenn Sie die Option „Standard manuell speichern“ auswählen {#save-changes-in-a-task-list-manually-when-you-select-the-manual-save-standard-option}

>[!TIP]
>
>Wenn Ihr Projekt über mehr als 2.000 Aufgaben verfügt oder viele Abhängigkeiten aufweist, kann es eine Weile dauern, bis Sie die Änderungen an Ihren Aufgaben und deren Auswirkungen auf alle Projektabhängigkeiten visuell erkennen können. In diesem Fall kann das Speichern der Änderungen länger als erwartet dauern.

Beachten Sie beim Aktualisieren von Aufgaben in einer Liste nach Auswahl der Option „Standard manuell speichern“ Folgendes:

* Sie können eine benutzerdefinierte Ansicht auf die Aufgabenliste anwenden und alle aufgabenbezogenen Felder bearbeiten, zu deren Verwaltung Sie in dieser Ansicht berechtigt sind.
* Wenn als Projektaktualisierungstyp „Automatisch“ oder „Automatisch“ und „Bei Änderung“ ausgewählt ist, berechnet Workfront die Zeitleiste des Projekts und alle projektinternen und projektübergreifenden Abhängigkeiten, nachdem Sie auf „Speichern“ geklickt haben. Informationen zum Projektaktualisierungstyp finden Sie unter [Auswahl des Projektaktualisierungstyps](../../../manage-work/projects/manage-projects/select-project-update-type.md).

So bearbeiten Sie Aufgaben in einer Liste bei Auswahl der Option „Manuelles Speichern - Standard“:

{{step1-to-projects}}

1. Wählen Sie auf **Seite** ein Projekt aus.

1. Klicken Sie im linken Bedienfeld auf den Abschnitt **Aufgaben**.

1. Klicken Sie oben in **Liste auf** Plan![Modus](assets/plan-mode-icon.png)Symbol „Plan-Modus“.

1. Wählen **Dialogfeld &quot;**&quot; die Option **Manuelles Speichern** und klicken Sie dann auf **Standard**.

   ![Aktivieren Sie die Einstellung „Manuelles Speichern“](assets/manual-standard-setting-enabled-quicksilver-task-list-350x493.png)

1. Klicken Sie **Apply**. Es wird eine Symbolleisteneinstellung mit Optionen zum Rückgängigmachen, Wiederholen und Speichern von Änderungen angezeigt.

   ![Symbolleiste zum manuellen Speichern](assets/undo,-redo,-save,-and-cancel-widget-for-task-list-350x65.png)

1. Klicken Sie in ein Feld, für das Sie über die Berechtigung zum manuellen Aktualisieren verfügen. Das Feld kann nun bearbeitet werden, und Sie können Ihre Änderungen vornehmen.

1. Drücken Sie **Eingabetaste** (Windows) oder **Zurück** (Mac) auf der Tastatur, um die von Ihnen vorgenommenen Änderungen vorübergehend zu speichern.

1. (Optional) Klicken Sie auf das **Rückgängig**-Symbol ![Rückgängig-Symbol](assets/undo-icon-on-task-list.png), um eine Änderung rückgängig zu machen und ein Feld in den Originalzustand zurückzuversetzen.

1. (Optional und bedingt) Klicken Sie auf das **Wiederholen**-Symbol ![Wiederholen-Symbol](assets/redo-icon-on-task-list.png), um die rückgängig gemachte Änderung wiederherzustellen.

1. (Optional) Klicken Sie mit der rechten Maustaste auf eine Aufgabe, die Sie ändern möchten.

   ODER

   Klicken Sie auf die **** Mehr![](assets/more-icon-task-list.png).

1. (Optional) Wählen Sie aus den folgenden Optionen aus:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">In neuer Registerkarte öffnen</td> 
      <td>Öffnet die Aufgabe in einer neuen Browser-Registerkarte. </td> 
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
* Wenn der Projektaktualisierungstyp Automatisch oder Automatisch und Bei Änderung ist, werden die projektübergreifenden Abhängigkeiten nach dem Klicken auf Speichern berechnet. Informationen zum Projektaktualisierungstyp finden Sie unter [Auswahl des Projektaktualisierungstyps](../../../manage-work/projects/manage-projects/select-project-update-type.md).

So bearbeiten Sie Aufgaben in einer Liste mithilfe der Option „Manuelles Speichern der Zeitleistenplanung“:


{{step1-to-projects}}

1. Wählen Sie auf **Seite** ein Projekt aus.

1. Klicken Sie im linken Bedienfeld auf den Abschnitt **Aufgaben**.

1. Klicken Sie oben in **Liste auf** Plan![Modus](assets/plan-mode-icon.png)Symbol „Plan-Modus“.

1. Wählen Sie im **Planmodus** die Option **Manuelles Speichern** und klicken Sie dann auf **Timeline-Planung**.

   ![Zeitleistenplanungs-Einstellung anwenden](assets/manual-timeline-planning-setting-enabled-quicksilver-task-list-350x490.png)

   >[!TIP]
   >
   >Die **Zeitplanung**-Option ist für Projekte mit mehr als 2000 Aufgaben abgeblendet.

1. Klicken Sie auf **Übernehmen**.

   Die Liste enthält folgende Änderungen:

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

     ![Symbolleiste zum manuellen Speichern](assets/undo,-redo,-save,-and-cancel-widget-for-task-list-350x65.png)

1. Bearbeiten Sie alle Felder, für die Sie über die Berechtigung zum manuellen Aktualisieren verfügen.

1. Drücken Sie **Eingabetaste** (Windows) oder **Zurück** (Mac) auf der Tastatur, um die von Ihnen vorgenommenen Änderungen vorübergehend zu speichern.
1. (Optional) Klicken Sie auf das **Rückgängig**-Symbol ![Rückgängig-Symbol](assets/undo-icon-on-task-list.png), um eine Änderung rückgängig zu machen und ein Feld in den Originalzustand zurückzuversetzen.
1. (Optional und bedingt) Klicken Sie auf das **Wiederholen**-Symbol ![Wiederholen-Symbol](assets/redo-icon-on-task-list.png), um die rückgängig gemachte Änderung wieder herzustellen.

1. (Optional) Klicken Sie mit der rechten Maustaste auf eine Aufgabe, die Sie ändern möchten.

   ODER

   Klicken Sie auf die **** Mehr![](assets/more-icon-task-list.png).

1. Wählen Sie aus den folgenden Optionen aus:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">In neuer Registerkarte öffnen</td> 
      <td>Öffnet die Aufgabe in einer neuen Browser-Registerkarte. </td> 
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
      <td role="rowheader">Duplizieren</td> 
      <td> <p>Erstellt eine doppelte Version der Aufgabe innerhalb desselben Projekts. </p> <p>Informationen zum Kopieren und Duplizieren von Aufgaben finden Sie unter <a href="../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md" class="MCXref xref">Aufgaben kopieren und duplizieren</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Workfront aktualisiert alle projektinternen und projektübergreifenden Abhängigkeiten, wenn Sie die Zeitleiste einer Aufgabe ändern.
1. Klicken Sie **Speichern**, wenn Sie Ihre Aufgabenänderungen dauerhaft beibehalten und die Zeitleiste des Projekts speichern möchten.

## Aufgabe in einer Liste mithilfe der Zusammenfassung bearbeiten

{{step1-to-projects}}

1. Wählen Sie auf **Seite** ein Projekt aus.

1. Klicken Sie im linken Bedienfeld auf den Abschnitt **Aufgaben**. Die Liste der Aufgaben für das Projekt wird angezeigt.

1. Wählen Sie die Aufgabe aus, die Sie bearbeiten möchten, und klicken Sie dann auf **Zusammenfassung öffnen** Symbol ![Zusammenfassung öffnen](assets/task-summary-icon.png) in der oberen rechten Ecke der Liste. Das Bedienfeld **Aufgabenzusammenfassung** wird geöffnet.

1. (Optional) Geben Sie eine Aktualisierung für die Aufgabe im Bereich **Updates** ein.
1. Klicken Sie auf eines der folgenden Symbole oder Bereiche, um zur Aufgabe zu wechseln und Informationen auf Aufgabenebene zu bearbeiten:

<table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Dokumente</td> 
      <td>Dokumente zur Aufgabe hinzufügen. </td> 
     </tr> 
          <tr> 
      <td role="rowheader">Benutzerdefinierte Formulare</td> 
      <td>Hinzufügen oder Entfernen benutzerdefinierter Formulare oder Aktualisieren von Informationen auf den Formularen.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Stunden</td> 
      <td>Stunden protokollieren.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Genehmigungen</td> 
      <td>Aufgabengenehmigungen hinzufügen.</td> 
     </tr> 
     <tr> 
    </tbody> 
   </table>

1. Klicken Sie auf **X** in der oberen rechten Ecke des Bedienfelds, um es zu schließen.

## Aufgaben stapelweise bearbeiten

Sie können mehrere Aufgaben gleichzeitig bearbeiten. Stellen Sie sicher, dass Sie Verwaltungsberechtigungen für die von Ihnen ausgewählten Aufgaben haben, um sie stapelweise bearbeiten zu können.

Die gleichzeitige Bearbeitung mehrerer Aufgaben unterscheidet sich je nach ausgewählter Umgebung.

### Massenbearbeitung von Aufgaben in der Produktionsumgebung

{{step1-to-projects}}

1. Wählen Sie auf **Seite** ein Projekt aus.
1. Klicken Sie im linken Bedienfeld auf den Abschnitt **Aufgaben**.

1. Klicken Sie auf **Planmodus**-Symbol ![Planmodus-Symbol](assets/plan-mode-icon.png) oben in der Liste und stellen Sie sicher, dass die Option **Automatisches Speichern** ausgewählt ist.

   ![Aktivieren Sie die Einstellung für automatisches Speichern](assets/autosave-setting-enabled-quicksilver-task-list-350x308.png)

   >[!IMPORTANT]
   >
   >Beim manuellen Speichern von Aufgaben können Sie Aufgaben nicht stapelweise bearbeiten.

1. Wählen Sie mehrere Aufgaben in der Aufgabenliste aus.
1. (Optional) Klicken Sie auf das **Mehr** Menü ![Mehr](assets/more-icon.png) oben in der Aufgabenliste und dann auf **Ausdrücke neu berechnen**, um alle Informationen in berechneten benutzerdefinierten Feldern zu aktualisieren.
1. Klicken Sie auf das **Bearbeiten**-Symbol ![Bearbeiten](assets/qs-edit-icon.png). Das **Aufgaben bearbeiten** wird in der neuen -Version geöffnet.

   Die Bearbeitung der Informationen für alle Aufgaben ist identisch mit der Bearbeitung der Informationen für eine Aufgabe.

   Weitere Informationen zum Bearbeiten einer Aufgabe finden Sie unter [Aufgaben bearbeiten](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

1. (Bedingt) Gehen Sie in der neuen -Version wie folgt vor:

   1. Geben Sie die Informationen an, die Sie für alle ausgewählten Aufgaben in einem der folgenden Bereiche ändern möchten:

      * Übersicht
      * Arbeitsaufträge
      * Benutzerdefinierte Formulare
      * Finanzielle Details
      * Einstellungen
      * Einstellungen
      * Kommentar

      >[!NOTE]
      >
      >* Die Informationen, die Sie zu allen ausgewählten Aufgaben ändern, überschreiben die vorhandenen Informationen zu einzelnen Aufgaben, mit Ausnahme des Felds **Arbeitsaufträge**. Wenn Sie einen neuen Verantwortlichen in der Massenbearbeitung hinzufügen, wird dieser Verantwortliche allen ausgewählten Aufgaben hinzugefügt. Wenn den ausgewählten Aufgaben andere Verantwortliche zugewiesen werden, bleiben diese zusätzlich zu der durch Massenbearbeitung hinzugefügten zugewiesen.
      >* Wenn Sie die Aufgabendauer bearbeiten möchten, müssen die ausgewählten Aufgaben dieselbe Aufgabenbeschränkung aufweisen. Andernfalls wird **Feld** Dauer“ nicht ausgefüllt.
      >
      >* In der Liste werden nur aktive benutzerdefinierte Formulare angezeigt. Wenn die ausgewählten Aufgaben keine benutzerdefinierten Formulare gemeinsam haben, werden in diesem Abschnitt keine Formulare aufgelistet.
      >* Sie können nur die Felder in den Formularen bearbeiten, die an alle ausgewählten Aufgaben angehängt sind und für die Sie über die Berechtigung zum Bearbeiten verfügen.  Informationen zur Massenbearbeitung benutzerdefinierter Formulare finden Sie unter [Verwalten benutzerdefinierter Formulare, die an Objekte angehängt sind](../../../workfront-basics/work-with-custom-forms/manage-custom-forms-attached-to-objects.md).

   1. Klicken Sie auf **Speichern**.
   1. (Optional) Klicken Sie **Zurück zum alten Erlebnis wechseln** unten im Feld **Aufgaben bearbeiten**.

1. (Bedingt) Gehen Sie in der alten -Version wie folgt vor:

   1. Geben Sie die Informationen an, die Sie für alle ausgewählten Aufgaben in einem der folgenden Bereiche ändern möchten:

      * Übersicht
      * Einstellungen
      * Arbeitsaufträge
      * Benutzerdefinierte Formulare
      * Kommentar

   1. (Optional) Wählen Sie im Abschnitt **Benutzerdefinierte Forms** die Option **Benutzerdefinierte Ausdrücke neu berechnen** aus, um sicherzustellen, dass alle berechneten benutzerdefinierten Felder in den benutzerdefinierten Formularen, die an die ausgewählten Aufgaben angehängt sind, auf dem neuesten Stand sind.
   1. Klicken Sie **Änderungen speichern**. Alle von Ihnen vorgenommenen Änderungen sind nun für alle ausgewählten Aufgaben sichtbar.

<div class="preview">

### Massenbearbeitung von Aufgaben in der Vorschau-Umgebung

{{step1-to-projects}}

1. Wählen Sie auf **Seite** ein Projekt aus.
1. Klicken Sie im linken Bedienfeld auf den Abschnitt **Aufgaben**.

1. Klicken Sie auf **Planmodus**-Symbol ![Planmodus-Symbol](assets/plan-mode-icon.png) oben in der Liste und stellen Sie sicher, dass die Option **Automatisches Speichern** ausgewählt ist.

   ![Aktivieren Sie die Einstellung für automatisches Speichern](assets/autosave-setting-enabled-quicksilver-task-list-350x308.png)

   >[!IMPORTANT]
   >
   >Beim manuellen Speichern von Aufgaben können Sie Aufgaben nicht stapelweise bearbeiten.

1. Wählen Sie mehrere Aufgaben in der Aufgabenliste aus.
1. (Optional) Klicken Sie auf das **Mehr** Menü ![Mehr](assets/more-icon.png) oben in der Aufgabenliste und dann auf **Ausdrücke neu berechnen**, um alle Informationen in berechneten benutzerdefinierten Feldern zu aktualisieren.
1. Klicken Sie auf das **Bearbeiten**-Symbol ![Bearbeiten](assets/qs-edit-icon.png). Das **Aufgaben bearbeiten** wird geöffnet.

   Die Bearbeitung der Informationen für alle Aufgaben ist identisch mit der Bearbeitung der Informationen für eine Aufgabe.

   Weitere Informationen zum Bearbeiten einer Aufgabe finden Sie unter [Aufgaben bearbeiten](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

1. Geben Sie die Informationen an, die Sie für alle ausgewählten Aufgaben in einem der folgenden Bereiche ändern möchten:

   * Übersicht
   * Arbeitsaufträge
   * Benutzerdefinierte Formulare
   * Finanzielle Details
   * Einstellungen
   * Einstellungen
   * Kommentar

   >[!NOTE]
   >
   >* Die Informationen, die Sie zu allen ausgewählten Aufgaben ändern, überschreiben die vorhandenen Informationen zu einzelnen Aufgaben, mit Ausnahme des Felds **Arbeitsaufträge**. Wenn Sie einen neuen Verantwortlichen in der Massenbearbeitung hinzufügen, wird dieser Verantwortliche allen ausgewählten Aufgaben hinzugefügt. Wenn den ausgewählten Aufgaben andere Verantwortliche zugewiesen werden, bleiben diese zusätzlich zu der durch Massenbearbeitung hinzugefügten zugewiesen.
   >* Wenn Sie die Aufgabendauer bearbeiten möchten, müssen die ausgewählten Aufgaben dieselbe Aufgabenbeschränkung aufweisen. Andernfalls wird **Feld** Dauer“ nicht ausgefüllt.
   >
   >* In der Liste werden nur aktive benutzerdefinierte Formulare angezeigt. Wenn die ausgewählten Aufgaben keine benutzerdefinierten Formulare gemeinsam haben, werden in diesem Abschnitt keine Formulare aufgelistet.
   >* Sie können nur die Felder in den Formularen bearbeiten, die an alle ausgewählten Aufgaben angehängt sind und für die Sie über die Berechtigung zum Bearbeiten verfügen.  Informationen zur Massenbearbeitung benutzerdefinierter Formulare finden Sie unter [Verwalten benutzerdefinierter Formulare, die an Objekte angehängt sind](../../../workfront-basics/work-with-custom-forms/manage-custom-forms-attached-to-objects.md).

1. Klicken Sie auf **Speichern**.

</div>

