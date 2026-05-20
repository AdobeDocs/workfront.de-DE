---
product-area: projects
navigation-topic: manage-projects
title: Übersicht über das Dokumentenmanagement für Projekte und zugehörige Objekte
description: Je nachdem, ob Ihr Workfront-Administrator für Ihre standardmäßige Speichereinstellung auswählt, können Sie Dokumente entweder im alten Workfront-Speicher oder im Adobe-Cloud-Speicher speichern. Dieser Artikel beschreibt, wie Sie Dokumente für Projekte, Portfolios, Programme, Vorlagen, Aufgaben und Probleme verwalten können.
author: Alina
feature: Work Management
exl-id: 5623157e-946e-4475-9df3-b1888a2a0934
source-git-commit: 9a35246858141a3b69ec85be3372c7a8d9497d6e
workflow-type: tm+mt
source-wordcount: '1920'
ht-degree: 0%

---

# Übersicht über das Dokumentenmanagement für Projekte und zugehörige Objekte

Ihr Adobe Workfront-Administrator kann den Standard für die Speichervoreinstellungen Ihres Unternehmens definieren, um anzugeben, wo Dokumente in Workfront gespeichert werden sollen.

Der Workfront-Administrator kann eine der folgenden Optionen auswählen:

* Workfront-Speicher
* Adobe Cloud-Speicher

Mit dieser Einstellung können Sie an Workfront-Objekte angehängte Dokumente automatisch an einem der verfügbaren Speicherorte speichern.

>[!IMPORTANT]
>
>Ihre Workfront-Instanz hat möglicherweise keinen Zugriff auf Workfront- und Adobe-Speicher. Einige Workfront-Instanzen haben nur Zugriff auf Workfront, während andere standardmäßig nur Zugriff auf den Adobe-Cloud-Speicher haben. Für Kunden mit Zugriff auf nur einen Speichertyp ist keine Konfiguration erforderlich.

Der Workfront-Administrator kann einen der folgenden Schritte ausführen:

* Wählen Sie eine der beiden Speicheroptionen als Standard für Ihr Unternehmen
* Sie können beim Erstellen eines der folgenden Objekte auswählen, welchen Speicher Sie bevorzugen:

   * Projekte
   * Portfolios
   * Vorlagen

Informationen zum Festlegen von Speichervoreinstellungen für Workfront finden Sie unter [Aktivieren von Adobe-Cloud-Speicher für Ihr Unternehmen](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-esm.md).

Dieser Artikel beschreibt, wie Sie Dokumente für Projekte, Portfolios, Programme, Aufgaben, Probleme, Vorlagen und Vorlagenaufgaben verwalten können.

<!--

Not sure we need these since this became an overview article: 

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td> <p>Light or higher</p>
   <p>Review or higher</p>
   
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>View or higher access to the objects you want to add documents to:</p>
   <ul><li>Projects</li>
   <li>Portfolios</li>
<li>Programs</li>
<li>Templates</li> 
<li>Tasks</li> 
<li>Issues</li> </ul>  
   
</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p> View or higher permissions to the objects you want to add documents to:</p>

<ul><li>A project</li>
   <li>A portfolio</li>
<li>A program</li>
<li>A template</li> 
<li>A task</li> 
<li>An issue</li> </ul>    
   
</td> 
  </tr> 
 </tbody> 
</table>

*For more detail about the information in this table, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

-->

## Dokumentenspeicher - Übersicht

Kunden haben möglicherweise Zugriff auf eine der folgenden Dokumentenspeicherfunktionen:

* Nur Workfront-Speicher. Der Bereich Speichereinstellungen in den Systemeinstellungen existiert nicht.
* Nur Adobe-Cloud-Speicher. Der Bereich Speichereinstellungen in den Systemeinstellungen existiert nicht.
* Sowohl Workfront Storage als auch Adobe Cloud Storage. Der Workfront-Administrator kann zwischen folgenden Optionen wählen:

   * Wählt eine standardmäßige Speicherumgebung für den zukünftigen Umgang mit Dokumenten aus.
   * Ermöglicht Benutzern die Auswahl des von ihnen gewählten Speichers, wenn sie die folgenden Objekte erstellen:

      * Projekte
      * Portfolios
      * Vorlagen

  >[!NOTE]
  >
  >* Aufgaben und Probleme übernehmen den Speichertyp aus dem Projekt.
  >* Vorlagenaufgaben übernehmen den Speichertyp aus der Vorlage
  >* Programme übernehmen den Speichertyp aus dem Portfolio.


Dokumente, die in Objekten im Workfront-Speicher gespeichert sind, werden anders verwaltet als die im Adobe-Cloud-Speicher gespeicherten Dokumente.

Weitere Informationen finden Sie unter [Übersicht über den Adobe-Cloud-Speicher](/help/quicksilver/review-and-approve-work/esm-overview.md).

In den folgenden Abschnitten wird beschrieben, wie der Dokumentspeicher für Workfront-Objekte funktioniert, wenn sowohl Workfront- als auch Adobe-Cloud-Speicheroptionen in derselben Umgebung vorhanden sind.

### Dokumentenverwaltung für Projekte

Beachten Sie beim Arbeiten mit Projekten Folgendes:

* Wenn Sie ein Adobe-Cloud-Speicher-Projekt erstellen, erstellt Workfront einen Ordner im Abschnitt Dokumente des Projekts, in dem Dokumente gespeichert werden. Der Ordnername entspricht dem Namen des Projekts. Sie können den Ordner nicht löschen oder manuell umbenennen. Der Ordner wird umbenannt, wenn Sie den Projektnamen so ändern, dass er zum neuen Projektnamen passt.
* Wenn Sie ein Adobe-Cloud-Speicherprojekt erstellen oder in ein veraltetes Workfront-Speicherportfolio oder -programm verschieben, wird das Portfolio oder Programm automatisch in ein Adobe-Cloud-Speicherobjekt konvertiert, wenn dem Portfolio oder Programm keine Dokumente beigefügt sind, bevor das Projekt hinzugefügt wird.
* Sie können kein Legacy-Workfront-Speicherprojekt für ein Adobe-Cloud-Speicherportfolio oder -Programm erstellen.
* Wenn Sie ein Projekt aus MS Project importieren, erstellt Workfront ein veraltetes Workfront-Speicherprojekt, auch wenn Ihr Workfront-Administrator den Adobe-Cloud-Speicher als Standard für Ihr System festgelegt hat.
* Wenn Sie Projekte mit einer Workfront-Planungsautomatisierung erstellen, verwendet Workfront die standardmäßige Speichervoreinstellung Ihres Systems für das Projekt. Sie müssen das Planning-Paket erwerben, um Zugriff auf Workfront Planning zu erhalten.

### Dokumentenmanagement für Portfolios

Beachten Sie beim Arbeiten mit Portfolios Folgendes:

* Wenn Sie ein Adobe Cloud-Speicherportfolio erstellen, erstellt Workfront im Abschnitt Dokumente des Portfolios, in dem Dokumente gespeichert werden. Der Ordnername ist derselbe Name wie das Portfolio. Sie können den Ordner nicht löschen oder manuell umbenennen. Der Ordner wird umbenannt, wenn Sie den Namen des Portfolios so ändern, dass er mit dem neuen Namen des Portfolios übereinstimmt.

* Wenn Sie ein Adobe-Cloud-Speicherprojekt zu einem alten Workfront-Speicherportfolio hinzufügen und dem Portfolio keine Dokumente angehängt sind, wird das Portfolio in ein Adobe-Cloud-Speicherportfolio konvertiert.
* Wenn Sie ein Adobe-Cloud-Speicherprojekt zu einem alten Workfront-Speicherportfolio hinzufügen und dem Portfolio Dokumente beigefügt sind, bleibt der Speicher für Portfoliodokumente im Workfront-Speicher. Das Speichersymbol Legacy Workfront für das Portfolio ![Speichersymbol Legacy Portfolio](assets/legacy-storage-project-icon.png) wird jedoch aus dem Portfolio entfernt.
* Sie können kein Legacy-Workfront-Speicherprojekt zu einem Adobe Cloud-Speicherportfolio hinzufügen.

* Wenn Sie Portfolios mit einer Workfront-Planungsautomatisierung erstellen, verwendet Workfront die standardmäßige Speichervoreinstellung Ihres Systems für das Portfolio. Sie müssen das Planning-Paket erwerben, um Zugriff auf Workfront Planning zu erhalten.

### Dokumentenverwaltung für Programme

Beachten Sie beim Arbeiten mit Programmen Folgendes:

* Wenn Sie ein Cloud-Speicherprogramm für Adobe erstellen, erstellt Workfront im Abschnitt Dokumente des Programms einen Ordner, in dem Dokumente gespeichert werden. Der Ordnername entspricht dem Namen des Programms. Sie können den Ordner nicht löschen oder manuell umbenennen. Wenn Sie den Programmnamen ändern, wird der Ordner umbenannt, damit er zum neuen Programmnamen passt.

* Wenn Sie ein Adobe-Cloud-Speicherprojekt zu einem veralteten Workfront-Speicherprogramm hinzufügen und dem Programm keine Dokumente beigefügt sind, wird das Programm in ein Adobe-Cloud-Speicherprogramm konvertiert. Das Portfolio des Programms wird ebenfalls konvertiert.
* Wenn Sie ein Adobe-Cloud-Speicherprojekt zu einem veralteten Workfront-Speicherprogramm hinzufügen und dem Programm Dokumente beigefügt sind, bleibt der Speicher für die Programmdokumente im Workfront-Speicher. Wenn das Portfolio auch Dokumente enthält, bleibt der Dokumentenspeicher ebenfalls im Workfront-Speicher. Andernfalls wird das Portfolio in den Adobe-Cloud-Speicher konvertiert.

  Das Speichersymbol für veraltete Workfront für das Programm ![Speichersymbol für veraltete Portfolios](assets/legacy-storage-project-icon.png) wird aus dem Programm entfernt.
* Sie können kein Legacy-Workfront-Speicherprojekt zu einem Adobe-Cloud-Speicherprogramm hinzufügen.

* Wenn Sie Programme mithilfe einer Workfront-Planungsautomatisierung erstellen, verwendet Workfront die standardmäßige Speichervoreinstellung Ihres Systems für das Programm. Sie müssen das Planning-Paket erwerben, um Zugriff auf Workfront Planning zu erhalten.

### Dokumentverwaltung für Aufgaben

Beachten Sie beim Arbeiten mit Aufgaben Folgendes:

* Aufgaben übernehmen den Speichertyp aus Projekten.
* Wenn Sie ein Dokument zu einer Aufgabe in einem Adobe-Cloud-Speicher-Projekt hochladen, erstellt Workfront automatisch einen Ordner im Abschnitt Dokumente der Aufgabe. Der Ordnername entspricht dem Namen der Aufgabe.
* Sie können den Dokumentordner umbenennen und aus der Adobe-Cloud-Speicheraufgabe löschen, wodurch auch die Dokumente im Ordner gelöscht werden. Nachdem Sie der Aufgabe neue Dokumente hinzugefügt haben, wird der Ordner automatisch neu erstellt. Gelöschte Dokumente werden nicht wieder im Ordner abgelegt.
* Bei Adobe Cloud-Speicherprojekten wird der Dokumentordner auf einer Aufgabe als Unterordner im automatisch für das Projekt erstellten Dokumentenordner angezeigt.
* Es ist nicht möglich, eine Aufgabe aus einem alten Workfront-Speicherprojekt in ein Adobe-Cloud-Speicherprojekt zu kopieren oder zu verschieben. Auch das Gegenteil ist nicht möglich.
* Beim Konvertieren einer Aufgabe in ein Projekt treten die folgenden Szenarien auf: <!--this info also duplicated in Convert tasks to projects-->
   * Eine alte Workfront-Speicheraufgabe erstellt ein veraltetes Workfront-Speicherprojekt.
   * Eine Adobe-Cloud-Speicheraufgabe erstellt ein Adobe-Cloud-Speicherprojekt.
   * Wenn Sie eine ältere Workfront-Speichervorlage zum Konvertieren einer Adobe-Cloud-Speicheraufgabe verwenden, wird ein Adobe-Cloud-Speicherprojekt erstellt.
   * Wenn Sie eine Adobe-Cloud-Speichervorlage zum Konvertieren einer veralteten Workfront-Speicheraufgabe verwenden, wird ein veraltetes Workfront-Speicherprojekt erstellt.
* Sie können im Zusammenfassungsbereich keine Dokumente zu Adobe Cloud-Speicheraufgaben hinzufügen.

### Dokumentenverwaltung für Probleme

Beachten Sie beim Arbeiten mit Problemen Folgendes:

* Probleme übernehmen den Speichertyp aus Projekten.
* Wenn Sie ein Dokument zu einem Problem in einem Adobe-Cloud-Speicher-Projekt hochladen, erstellt Workfront automatisch einen Ordner im Dokumentbereich des Problems. Der Ordnername entspricht dem Problem.
* Sie können den Dokumentordner umbenennen und aus dem Adobe-Cloud-Speicher löschen, wodurch auch die Dokumente im Ordner gelöscht werden. Nachdem Sie dem Problem neue Dokumente hinzugefügt haben, wird der Ordner automatisch neu erstellt. Gelöschte Dokumente werden nicht wieder im Ordner abgelegt.
* Bei Adobe-Cloud-Speicherprojekten wird der Dokumentordner in einem Problem als Unterordner in dem automatisch für das Projekt erstellten Dokumentenordner angezeigt.
* Sie können ein Problem nicht aus einem alten Workfront-Speicherprojekt kopieren oder in ein Adobe-Cloud-Speicherprojekt verschieben. Auch das Gegenteil ist nicht möglich.
* Wenn Sie eine Anfrage mit einem an ein älteres Workfront-Speicherprojekt angehängten Dokument senden, wird das Dokument im Bereich Dokumente der Anfrage unter Verwendung des Speichertyps des Projekts angezeigt, auch wenn die Standardeinstellung für den Systemspeicher Adobe Cloud-Speicher ist.
* Beim Konvertieren eines Problems in ein Projekt treten die folgenden Szenarien auf: <!--this info also duplicated in Convert an issue to a project-->
   * Ein Problem mit einem alten Workfront-Speicher erstellt ein veraltetes Workfront-Speicherprojekt.
   * Ein Adobe-Cloud-Speicherproblem erstellt ein Adobe-Cloud-Speicherprojekt.
   * Wenn Sie eine ältere Workfront-Speichervorlage verwenden, um ein Adobe-Cloud-Speicherproblem zu konvertieren, wird ein Adobe-Cloud-Speicherprojekt erstellt.
   * Wenn Sie eine Adobe-Cloud-Speichervorlage verwenden, um ein veraltetes Workfront-Speicherproblem zu konvertieren, wird ein veraltetes Workfront-Speicherprojekt erstellt.
* Sie können im Bedienfeld „Zusammenfassung“ keine Dokumente zu Problemen mit der Adobe-Cloud-Datenspeicherung hinzufügen.

### Dokumentenverwaltung für Projektvorlagen

Beachten Sie beim Arbeiten mit Vorlagen Folgendes:

* Wenn Sie eine Adobe-Cloud-Speichervorlage erstellen, erstellt Workfront im Dokumentbereich der Vorlage einen Ordner, in dem Dokumente gespeichert werden. Der Ordnername ist mit dem Programmnamen identisch. Sie können den Ordner nicht löschen oder manuell umbenennen. Der Ordner wird umbenannt, wenn Sie den Namen der Vorlage ändern, sodass er zum neuen Namen der Vorlage passt.
* Sie können eine ältere Workfront-Speichervorlage verwenden, um ältere Workfront-Speicherprojekte zu erstellen. Sie können eine Adobe-Cloud-Speichervorlage verwenden, um ein Adobe-Cloud-Speicherprojekt zu erstellen.
* Sie können eine ältere Workfront-Speichervorlage an ein Adobe-Cloud-Speicherprojekt anhängen. Dadurch wird der Speicherort der Dokumente im Projekt nicht geändert.
* Sie können eine Adobe-Cloud-Speichervorlage an ein veraltetes Workfront-Speicherprojekt anhängen. Dadurch wird der Speicherort der Dokumente im Projekt nicht geändert. Dokumente im Cloud-Speicherordner von Adobe für die Vorlage werden dem Projekt direkt und ohne den Ordner hinzugefügt, während die Dokumente in den Vorlagenaufgabenordnern den Ordnern hinzugefügt werden, die an die Projektaufgaben im Abschnitt Dokumente der Aufgaben angehängt sind.

### Dokumentverwaltung für Vorlagenaufgaben

Beachten Sie beim Arbeiten mit Vorlagenaufgaben Folgendes:

* Vorlagenaufgaben übernehmen den Speichertyp aus Vorlagen.
* Wenn Sie ein Dokument zu einer Vorlagenaufgabe auf einer Adobe Cloud-Speichervorlage hochladen, erstellt Workfront automatisch einen Ordner im Abschnitt Dokumente der Vorlagenaufgabe. Der Ordnername entspricht dem der Vorlagenaufgabe.
* Sie können den Dokumentordner umbenennen und aus der Vorlagenaufgabe für die Adobe-Cloud-Datenspeicherung löschen, wodurch auch die Dokumente im Ordner gelöscht werden. Nachdem Sie der Vorlagenaufgabe neue Dokumente hinzugefügt haben, wird der Ordner automatisch neu erstellt. Gelöschte Dokumente werden nicht wieder im Ordner abgelegt.
* Bei Adobe Cloud-Speichervorlagen wird der Dokumentordner auf einer Vorlagenaufgabe als Unterordner im Ordner Dokumente angezeigt, der automatisch für die Vorlage erstellt wird.
* Sie können eine Vorlagenaufgabe nicht von einer alten Workfront-Speichervorlage kopieren oder in eine Adobe-Cloud-Speichervorlage verschieben. Auch das Gegenteil ist nicht möglich.
* Wenn Sie ein Dokument an ein Problem anhängen, das Sie an eine mit dem Adobe-Speicher verknüpfte Anfrage-Warteschlange senden, wird für jedes gesendete Problem ein Ordner erstellt, in dem die Dokumente gespeichert werden. Der Ordner wird auch als Unterordner zum automatisch erstellten Projektordner in der Anfrage-Warteschlange hinzugefügt.
