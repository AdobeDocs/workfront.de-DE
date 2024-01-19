---
product-area: projects
navigation-topic: manage-tasks
title: Aufgaben kopieren und duplizieren
description: Sie können eine Aufgabe aus einem Projekt in ein anderes Projekt kopieren oder eine Aufgabe innerhalb desselben Projekts duplizieren.
author: Alina
feature: Work Management
exl-id: daf89062-cf58-4c39-83ff-727d969a9630
source-git-commit: 980e6c2cea2ceb98abda6b98811e734d895ad274
workflow-type: tm+mt
source-wordcount: '1736'
ht-degree: 1%

---

# Aufgaben kopieren und duplizieren

Sie können eine Aufgabe aus einem Projekt in ein anderes Projekt kopieren oder eine Aufgabe innerhalb desselben Projekts duplizieren.

Sie können eine oder mehrere Aufgaben oder übergeordnete Aufgaben gleichzeitig kopieren oder duplizieren.

## Zugriffsanforderungen

<!-- drafted for P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Standard</p> 
   Or
   <p>Legacy license: Work or higher </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Tasks and Projects</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to a task</p> <p>Contribute or higher permissions to the project</p> 
   <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Arbeit oder höher </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf Aufgaben und Projekte bearbeiten</p> <p><b>NOTIZ</b>

Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Berechtigungen für eine Aufgabe verwalten </p> <p>Beitragen oder höhere Berechtigungen zum Projekt</p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Überlegungen zum Kopieren von Aufgaben

Beachten Sie beim Kopieren einer Aufgabe Folgendes:

* Wenn Sie eine Aufgabe von einem Projekt in ein anderes kopieren, können die Aufgabendaten neu berechnet werden. Bei der Neuberechnung werden der Zeitplan, den das neue Projekt verwendet, und die Informationen zum Zeitplan des Projekts berücksichtigt.
* Benutzerdefinierte Formulare werden mit der Aufgabe kopiert. Die Informationen in den benutzerdefinierten Feldern werden nur dann an die kopierten Aufgaben übertragen, wenn Sie beim Kopieren der Aufgabe &quot;Benutzerdefinierte Daten kopieren&quot;auswählen.
* Sie haben die Möglichkeit, beim Kopieren einige der Aufgabe zugeordnete Elemente in die kopierte Aufgabe zu kopieren. Die folgenden Objekte werden jedoch standardmäßig nicht an die kopierte Aufgabe übertragen:
   * Probleme
   * Protokollierte Stunden
   * Benutzerkommentare <!--not sure about this, enable only if requested by users and verified by Product: System activity comments transfer to the new task if they relate to information that you specifically select to be copied. For example, if you select to copy Expenses to the new task, system comments that identify adding expenses to the task will transfer to the copied task. -->
* Die folgenden Elemente werden standardmäßig zur kopierten Aufgabe verschoben:

   * Meilensteine werden in die kopierte Aufgabe übertragen und aus der ursprünglichen Aufgabe entfernt.
   * Unteraufgaben werden an die neue Aufgabe übertragen.

* Sie können eine Aufgabe gleichzeitig kopieren oder mehrere Aufgaben gleichzeitig kopieren, wenn Sie Aufgaben in einer Liste bearbeiten.

## Aufgaben in eine Liste kopieren {#copy-tasks-in-a-list}

1. Wechseln Sie zu dem Projekt, das die Aufgabe oder die Aufgaben enthält, die Sie kopieren möchten.

   Oder

   Wechseln Sie zu einem Aufgabenbericht.

1. (Bedingt) Klicken Sie auf **Aufgaben** im linken Bereich, wenn Sie das Projekt geöffnet haben, das die Aufgaben enthält.
1. Klicken Sie auf **Planmodus** icon ![](assets/qs-list-mode-or-save-mode-icon-small.png)und stellen sicher, dass **Automatische Speicherung** aktiviert ist.

   ![](assets/autosave-icon-on-highlighted-350x202.png)

   >[!IMPORTANT]
   >
   >Sie können Aufgaben nur beim automatischen Speichern Ihrer Änderungen in eine Liste kopieren. Informationen zum Speichern von Optionen beim Bearbeiten von Aufgaben finden Sie unter [Aufgaben in einer Liste bearbeiten](../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md).

1. Wählen Sie die zu kopierenden Aufgaben aus und führen Sie einen der folgenden Schritte aus:

   * Klicken Sie auf **Mehr Menü** Klicken Sie oben in der Aufgabenliste auf **Kopieren nach**.
   * Klicken Sie mit der rechten Maustaste auf die ausgewählten Aufgaben und klicken Sie dann auf **Kopieren nach**.
   * Klicken Sie bei der Auswahl einer Aufgabe auf die **Mehr** Menü ![](assets/more-icon-task-list.png) neben dem Aufgabennamen in der Liste und klicken Sie dann auf **Kopieren nach**.

   ![](assets/copy-task-in-list-nwe-350x131.png)

1. Fahren Sie mit dem Kopieren der Aufgabe fort, wie im Abschnitt beschrieben [Kopieren einer Aufgabe auf Aufgabenebene](#copy-a-task-at-the-task-level) beginnt mit Schritt 4.

   <!--
      (NOTE: is this still accurate?!)
   -->

## Kopieren einer Aufgabe auf Aufgabenebene {#copy-a-task-at-the-task-level}

Neben dem Kopieren von Aufgaben in eine Aufgabenliste können Sie auch eine Aufgabe kopieren, nachdem Sie sie geöffnet haben.

1. Suchen Sie eine Aufgabe in Ihrem Workfront-System, indem Sie danach suchen.
1. Klicken Sie auf den Namen der Aufgabe, um sie zu öffnen.
1. Klicken Sie auf **Mehr** Dropdown-Menü ![](assets/qs-more-menu.png) neben dem Namen der Aufgabe klicken Sie auf **Kopieren nach**.

   ![](assets/taskcopy-to-at-the-task-level-nwe-350x200.png)

   Das Feld Aufgabe kopieren wird angezeigt.

1. (Optional) Aktualisieren Sie die **Aufgabenname**.

   >[!TIP]
   >
   >Dieses Feld ist abgeblendet und kann nicht bearbeitet werden, wenn Sie mehrere Aufgaben in einer Liste kopieren möchten. Sie können den Mauszeiger über das Feld &quot;Aufgabenname&quot;bewegen und eine Liste aller ausgewählten Aufgaben wird angezeigt.
   >
   >![](assets/copy-task-multiple-tasks-box-with-list-of-task-names-nwe-350x130.png)

1. Geben Sie den Namen der **Zielprojekt** wo Sie die Aufgabe in die **Zielprojekt auswählen** -Feld.

   >[!TIP]
   >
   >* Beim Namen des Projekts wird zwischen Groß- und Kleinschreibung unterschieden.
   >* Sie können auch mit der Eingabe der Referenznummer beginnen oder die Kennung des Projekts eingeben. Auf diese Weise können Sie zwischen Projekten mit identischen Namen unterscheiden.
   >* In der Liste werden nur 100 Projekte angezeigt.

   Der aktuelle Projektname wird standardmäßig angezeigt. Wenn Sie die Aufgabe im selben Projekt kopieren möchten, lassen Sie dieses Feld unverändert.

1. (Bedingt) Klicken Sie auf **Zugriff anfordern** , um Zugriff auf das Projekt anzufordern, wenn Sie keinen Zugriff auf das ausgewählte Projekt haben.
1. (Bedingt) Kopieren Sie die Aufgabe weiterhin in das ausgewählte Zielprojekt, ohne Zugriff anzufordern, wenn Sie Zugriff haben, um Aufgaben zu einer der Aufgaben im Zielprojekt hinzuzufügen.

   ![](assets/copy-task-request-access-from-project-nwe-350x125.png)

   >[!TIP]
   >
   >Ähnliche Meldungen werden angezeigt, wenn das ausgewählte Projekt noch nicht genehmigt, abgeschlossen oder deaktiviert ist, wenn der Workfront-Administrator verhindert, dass diesen Projekten Aufgaben hinzugefügt werden. Weitere Informationen finden Sie unter [Systemweite Projektvoreinstellungen konfigurieren](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

1. Klicks **Optionen** Deaktivieren Sie dann im linken Bereich die Aufgabenattribute, die Sie nicht mit der Aufgabe kopieren möchten. Alle Optionen sind standardmäßig ausgewählt.

   >[!TIP]
   >
   >Auswählen und Deselektieren **Alle auswählen** Deaktiviert alle Optionen.

   Deaktivieren Sie die folgenden Optionen, um sie nicht an die kopierte Aufgabe zu übertragen. In der folgenden Tabelle wird beschrieben, was passiert, wenn die Optionen deaktiviert werden:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Einschränkung</td> 
      <td> <p>Die Aufgabenbegrenzung wird auf "Sofort wie möglich"oder "So spät wie möglich"festgelegt, basierend auf der Einstellung "Projektplanmodus".</p> <p> Wenn diese Option aktiviert ist, wird die aktuelle Einschränkung der Aufgabe an die kopierte Aufgabe übertragen. </p> <p>Hinweis: Wenn beim Verschieben oder Kopieren einer Aufgabe mit datumsspezifischen Begrenzungen in ein anderes Projekt die Beschränkungsdaten der Aufgabe außerhalb der Daten des neuen Projekts liegen, wird entweder die Aufgabenbegrenzung so bald wie möglich oder so spät wie möglich geändert oder die geplanten Start- oder Abschlussdaten der Projekte angepasst. Beispiele für datumsspezifische Begrenzungen sind "Must On", "Must Finish On", "Start No Before", "Start No Later Than" usw. Informationen zu Aufgabenbegrenzungen und dazu, wie Aufgabenbegrenzungen oder Projektdaten betroffen sein können, finden Sie unter <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">Übersicht über Aufgabenbegrenzungen</a> und suchen Sie nach einer bestimmten Einschränkung.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Arbeitsaufträge</td> 
      <td> <p>Alle Zuweisungen werden aus der Aufgabe entfernt. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Genehmigungsprozess</td> 
      <td>Alle Genehmigungsprozesse werden aus der Aufgabe entfernt.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Fortschritt</td> 
      <td>Der Aufgabenstatus ist "Neu". Andernfalls behält die kopierte Aufgabe den Status der vorhandenen Aufgabe bei.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Finanzinformationen</td> 
      <td>Die finanziellen Informationen der Aufgabe werden entfernt.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Alle Vorgänger</td> 
      <td> <p>Dies bedeutet, dass die Abhängigkeiten nicht auf die kopierten Aufgaben übertragen werden. </p> <p>Wenn diese Option aktiviert ist, bleiben die Vorgänger in der Gruppe der kopierten Aufgaben erhalten, andere werden gelöscht.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Dokumente</td> 
      <td> <p>Die der Aufgabe angehängten Dokumente werden nicht an die kopierte Aufgabe übertragen. Dazu gehören Versionen, Testsendungen und verknüpfte Dokumente.</p> <p>Dokumentgenehmigungen sind nicht enthalten. Dokumentgenehmigungen können beim Kopieren einer Aufgabe nie kopiert werden.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Erinnerungsnachrichten</td> 
      <td>Die Aufgabenerinnerungen werden nicht an die kopierte Aufgabe übertragen. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ausgaben</td> 
      <td>Die bei der Aufgabe protokollierten Ausgaben werden nicht an die kopierte Aufgabe übertragen. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Berechtigungen</td> 
      <td>Workfront entfernt die Namen aller Entitäten, die in der Liste "Freigeben"der Aufgabe angezeigt werden. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Benutzerdefinierte Daten</td> 
      <td> <p>Die Werte für die benutzerdefinierten Felder werden gelöscht und die benutzerdefinierten Formulare werden in die kopierte Aufgabe übertragen. </p> <p>Wenn diese Option aktiviert ist, werden sowohl die Formulare als auch die Werte für die benutzerdefinierten Felder an die kopierte Aufgabe übertragen. </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Optional) Klicken Sie auf **Übergeordnetes Element auswählen** Wählen Sie im linken Bereich die Aufgabe im Zielprojekt aus, die Sie der kopierten Aufgabe übergeordnet werden möchten.

   >[!TIP]
   >
   >Bei der Auswahl, mehrere Aufgaben in einer Liste zu kopieren, werden alle ausgewählten Aufgaben zu den untergeordneten Elementen des ausgewählten übergeordneten Elements.

   Wählen Sie ein übergeordnetes Element aus, indem Sie einen der folgenden Schritte ausführen:

   * Wählen Sie in der Aufgabenliste einen der übergeordneten Elemente des Projektplans aus.
   * Klicken Sie auf das Suchsymbol ![Suchsymbol](assets/search-icon.png) und suchen Sie anhand des Namens nach einer übergeordneten Aufgabe.

   Die Aufgabe wird in der Liste angezeigt.

   ![Auswählen einer übergeordneten Aufgabe beim Verschieben einer Aufgabe mit Suchfunktion ](assets/select-parent-when-moving-tasks-with-search-functionality-nwe-350x110.png)

1. Wählen Sie das Optionsfeld für das übergeordnete Element aus, nachdem Sie es gefunden haben.

   Wenn Sie keine übergeordnete Aufgabe auswählen, werden die Aufgaben als Hauptaufgaben und nicht als Unteraufgaben kopiert und am Ende der Aufgabenliste im Zielprojekt platziert.

1. Klicks **Aufgabe kopieren**

   Oder

   Klicks **Aufgaben kopieren** wenn Sie mehrere Aufgaben in einer Liste auswählen.
Die kopierten Aufgaben befinden sich jetzt im angegebenen Projekt und sind entweder Unteraufgaben der ausgewählten übergeordneten Aufgabe oder die letzten Aufgaben des Projekts.

## Aufgaben duplizieren

Sie können eine Aufgabe in einer Aufgabenliste schnell duplizieren, wenn Sie für dasselbe Projekt eine identische Aufgabe benötigen.

* [Überlegungen zum Duplizieren von Aufgaben](#considerations-for-duplicating-tasks)
* [Aufgaben duplizieren](#duplicate-tasks)

### Überlegungen zum Duplizieren von Aufgaben {#considerations-for-duplicating-tasks}

* Sie können eine Aufgabe nur dann in einer Aufgabenliste duplizieren, wenn die Liste nach Aufgabennummer sortiert ist.
* Die neue Aufgabe hat denselben Namen wie die ursprüngliche Aufgabe.
* Sie können nicht auswählen, welche Informationen für die neue Aufgabe dupliziert werden. Fast alle Informationen aus der ursprünglichen Aufgabe werden standardmäßig an die duplizierte Aufgabe übermittelt, einschließlich der übergeordneten Beziehung.
* Die folgenden Elemente werden nicht in die neue Aufgabe übertragen:

   * Protokollierte Stunden
   * Notizen
   * Probleme
   * Nur die Vorgänger, die sich in derselben Gruppe kopierter Aufgaben befinden, werden ebenfalls mit ihren Nachfolgeaufgaben kopiert.

     **BEISPIEL**

     Wenn Sie z. B. Aufgabe 2 und den Vorgänger, Aufgabe 1, gleichzeitig kopieren, haben Sie eine Kopie von Aufgabe 2 und eine Kopie von Aufgabe 1. Die Kopie von Aufgabe 1 ist der Vorgänger der Kopie von Aufgabe 2. Wenn Sie jedoch nur Aufgabe 2 kopieren, ohne den Vorgänger zu kopieren, hat die Kopie keinen Vorgänger.

* Beim Duplizieren einer übergeordneten Aufgabe werden auch alle untergeordneten Aufgaben dupliziert, auch wenn die untergeordneten Aufgaben nicht ausgewählt sind.
* Sie können eine oder mehrere Aufgaben gleichzeitig duplizieren.

  Sie können jedoch nicht mehrere Aufgaben duplizieren, die nicht sequenziell sind.

* Meilensteine werden in die neue Aufgabe verschoben und aus der ursprünglichen Aufgabe entfernt.

### Aufgaben duplizieren

1. Wechseln Sie zu dem Projekt, das die zu duplizierenden Aufgaben enthält.
1. Klicks **Aufgaben** im linken Bereich.
1. Führen Sie einen der folgenden Schritte aus:

   * (Bedingt) Klicken Sie auf die **Planmodus** icon ![](assets/qs-list-mode-or-save-mode-icon-small.png) und die **Automatische Speicherung** aktiviert ist, wählen Sie die Aufgaben aus, die Sie duplizieren möchten, und klicken Sie dann auf **Mehr Menü** ![](assets/qs-more-menu-29x11.png) > **Duplizieren**.

     ![](assets/duplicate-tasks-in-list-nwe-350x196.png)

   * (Bedingt) Klicken Sie auf die **Planmodus** icon ![](assets/qs-list-mode-or-save-mode-icon-small.png) > **Manuelles Speichern** > **Standard** oder **Timeline-Planung** und führen Sie dann die folgenden Schritte aus:

      1. Wählen Sie die zu duplizierenden Aufgaben aus und klicken Sie auf **Duplizieren**.
      1. (Optional) Klicken Sie auf **Rückgängig** , um Ihre Änderungen rückgängig zu machen und die Aufgaben nicht zu duplizieren.
      1. (Optional und bedingt) Klicken Sie auf **Wiederholen** wenn Sie zuvor auf **Rückgängig**, um die Änderungen beizubehalten und die Aufgaben zu duplizieren.

      1. Klicks **Speichern** , um Ihre Änderungen zu speichern.

         Die Aufgaben werden dupliziert und demselben Projekt wie die ursprünglichen Aufgaben hinzugefügt.
