---
product-area: projects
navigation-topic: manage-projects
title: Übersicht über das Dokumentenmanagement für Projekte und zugehörige Objekte
description: Je nachdem, ob Ihr Workfront-Administrator für Ihre standardmäßige Speichereinstellung auswählt, können Sie Dokumente entweder im alten Workfront-Speicher oder im Adobe Enterprise-Speicher speichern. Dieser Artikel beschreibt, wie Sie Dokumente für Projekte, Portfolios, Programme, Vorlagen, Aufgaben und Probleme verwalten können.
author: Alina
feature: Work Management
exl-id: 5623157e-946e-4475-9df3-b1888a2a0934
source-git-commit: 2b0fdb3c74882b566a397872e1cc8007728b770c
workflow-type: tm+mt
source-wordcount: '1755'
ht-degree: 0%

---

# Übersicht über das Dokumentenmanagement für Projekte und zugehörige Objekte

Ihr Adobe Workfront-Administrator kann den Standard für die Speichervoreinstellungen Ihres Unternehmens definieren, um anzugeben, wo Dokumente in Workfront gespeichert werden sollen.

Der Workfront-Administrator kann eine der folgenden Optionen auswählen:

* Workfront-Speicher
* Adobe Enterprise-Speicher

Mit dieser Einstellung können Sie an Workfront-Objekte angehängte Dokumente automatisch an einem der verfügbaren Speicherorte speichern.

>[!IMPORTANT]
>
>Ihre Workfront-Instanz hat möglicherweise keinen Zugriff auf Workfront- und Adobe-Speicher. Einige Workfront-Instanzen haben nur Zugriff auf Workfront, während andere standardmäßig nur Zugriff auf den Adobe Enterprise-Speicher haben. Für Kunden mit Zugriff auf nur einen Speichertyp ist keine Konfiguration erforderlich.

Der Workfront-Administrator kann einen der folgenden Schritte ausführen:

* Wählen Sie eine der beiden Speicheroptionen als Standard für Ihr Unternehmen
* Sie können beim Erstellen eines der folgenden Objekte auswählen, welchen Speicher Sie bevorzugen:

   * Projekte
   * Portfolios
   * Vorlagen

Informationen zum Festlegen von Speichervoreinstellungen für Workfront finden Sie unter [Aktivieren von Adobe Enterprise-Speicher für Ihr Unternehmen](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-esm.md).

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
* Nur Adobe Enterprise-Speicher. Der Bereich Speichereinstellungen in den Systemeinstellungen existiert nicht.
* Sowohl Workfront Storage als auch Adobe Enterprise Storage. Der Workfront-Administrator kann zwischen folgenden Optionen wählen:

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


Dokumente, die in Objekten im Workfront-Speicher gespeichert sind, werden anders verwaltet als die im Adobe Enterprise-Speicher gespeicherten Dokumente.

Weitere Informationen finden Sie unter [Übersicht über Adobe Enterprise Storage](/help/quicksilver/review-and-approve-work/esm-overview.md).

In den folgenden Abschnitten wird beschrieben, wie die Dokumentenspeicherung für Workfront-Objekte funktioniert, wenn sowohl Workfront- als auch Adobe Enterprise-Speicheroptionen in derselben Umgebung vorhanden sind.

### Dokumentenverwaltung für Projekte

Beachten Sie beim Arbeiten mit Projekten Folgendes:

* Wenn Sie ein Enterprise-Storage-Projekt in Adobe erstellen, erstellt Workfront einen Ordner im Abschnitt Dokumente des Projekts, in dem Dokumente gespeichert werden. Der Ordnername entspricht dem Namen des Projekts. Sie können den Ordner nicht löschen oder manuell umbenennen. Der Ordner wird umbenannt, wenn Sie den Projektnamen so ändern, dass er zum neuen Projektnamen passt.
* Wenn Sie ein Adobe-Enterprise-Speicherprojekt erstellen oder in ein veraltetes Workfront-Speicherportfolio oder -programm verschieben, wird das Portfolio oder Programm automatisch in ein Adobe-Enterprise-Speicherobjekt konvertiert.
* Sie können kein Workfront-Speicherprojekt für ein Adobe Enterprise-Speicherportfolio oder -Programm erstellen.
* Wenn Sie ein Projekt aus MS Project importieren, erstellt Workfront ein Workfront-Speicherprojekt, auch wenn der Workfront-Administrator den Adobe Enterprise-Speicher als Standard für Ihr System festgelegt hat.
* Wenn Sie Projekte mit einer Workfront-Planungsautomatisierung erstellen, verwendet Workfront die standardmäßige Speichervoreinstellung Ihres Systems für das Projekt. Sie müssen das Planning-Paket erwerben, um Zugriff auf Workfront Planning zu erhalten.

### Dokumentenmanagement für Portfolios

Beachten Sie beim Arbeiten mit Portfolios Folgendes:

* Wenn Sie ein Adobe-Enterprise-Storage-Portfolio erstellen, erstellt Workfront im Abschnitt Dokumente des Portfolios einen Ordner, in dem Dokumente gespeichert werden. Der Ordnername ist derselbe Name wie das Portfolio. Sie können den Ordner nicht löschen oder manuell umbenennen. Der Ordner wird umbenannt, wenn Sie den Namen des Portfolios so ändern, dass er mit dem neuen Namen des Portfolios übereinstimmt.
* Wenn Sie ein Adobe-Enterprise-Speicherprojekt erstellen oder in ein veraltetes Workfront-Speicherportfolio verschieben, wird das Portfolio automatisch in ein Adobe-Enterprise-Speicherobjekt konvertiert.
* Wenn dem konvertierten Portfolio zuvor Dokumente beigefügt waren, bleiben sie weiterhin im Workfront-Speicher gespeichert. Neue Dokumente werden auch im Workfront-Speicher gespeichert.
* Wenn an das konvertierte Portfolio keine Dokumente im Workfront-Speicher angehängt waren, werden neue Dokumente im Adobe Enterprise-Speicher gespeichert.
* Wenn Sie Portfolios mit einer Workfront-Planungsautomatisierung erstellen, verwendet Workfront die standardmäßige Speichervoreinstellung Ihres Systems für das Portfolio. Sie müssen das Planning-Paket erwerben, um Zugriff auf Workfront Planning zu erhalten.

### Dokumentenverwaltung für Programme

Beachten Sie beim Arbeiten mit Programmen Folgendes:

* Wenn Sie ein Adobe-Enterprise-Storage-Programm erstellen, erstellt Workfront im Programmabschnitt Dokumente einen Ordner, in dem Dokumente gespeichert werden. Der Ordnername entspricht dem Namen des Programms. Sie können den Ordner nicht löschen oder manuell umbenennen. Wenn Sie den Programmnamen ändern, wird der Ordner umbenannt, damit er zum neuen Programmnamen passt.
* Wenn Sie ein Adobe-Enterprise-Speicherprojekt erstellen oder in ein veraltetes Workfront-Speicherportfolio verschieben, wird das Portfolio automatisch in ein Adobe-Enterprise-Speicherobjekt konvertiert.
* Wenn dem konvertierten Programm zuvor Dokumente beigefügt waren, bleiben diese weiterhin im Workfront-Speicher gespeichert. Neue Dokumente werden auch im Workfront-Speicher gespeichert.
* Wenn dem konvertierten Programm keine Dokumente im Workfront-Speicher angehängt waren, werden neue Dokumente im Adobe Enterprise-Speicher gespeichert.
* Wenn Sie Programme mithilfe einer Workfront-Planungsautomatisierung erstellen, verwendet Workfront die standardmäßige Speichervoreinstellung Ihres Systems für das Programm. Sie müssen das Planning-Paket erwerben, um Zugriff auf Workfront Planning zu erhalten.

### Dokumentverwaltung für Aufgaben

Beachten Sie beim Arbeiten mit Aufgaben Folgendes:

* Aufgaben übernehmen den Speichertyp aus Projekten.
* Wenn Sie ein Dokument zu einer Aufgabe in einem Adobe-Speicherprojekt hochladen, erstellt Workfront automatisch einen Ordner im Abschnitt Dokumente der Aufgabe. Der Ordnername entspricht dem Namen der Aufgabe.
* Sie können den Dokumentordner umbenennen und aus der Aufgabe &quot;Adobe Enterprise-Storage“ löschen, wodurch auch die Dokumente im Ordner gelöscht werden. Nachdem Sie der Aufgabe neue Dokumente hinzugefügt haben, wird der Ordner automatisch neu erstellt. Gelöschte Dokumente werden nicht wieder im Ordner abgelegt.
* Bei Enterprise-Storage-Projekten in Adobe wird der Dokumentenordner auf einer Aufgabe als Unterordner im automatisch für das Projekt erstellten Dokumentenordner angezeigt.
* Es ist nicht möglich, eine Aufgabe aus einem Workfront-Speicherprojekt in ein Adobe-Speicherprojekt zu kopieren oder zu verschieben. Auch das Gegenteil ist nicht möglich.
* Beim Konvertieren einer Aufgabe in ein Projekt treten die folgenden Szenarien auf: <!--this info also duplicated in Convert tasks to projects-->
   * Eine Workfront-Speicheraufgabe erstellt ein Workfront-Speicherprojekt.
   * Bei einer Adobe-Aufgabe für den Unternehmensspeicher wird ein Adobe-Speicherprojekt erstellt.
   * Durch die Verwendung einer Workfront-Speichervorlage zum Konvertieren einer Adobe-Speicheraufgabe wird ein Adobe-Speicherprojekt erstellt.
   * Durch die Verwendung einer Adobe-Speichervorlage zum Konvertieren einer Workfront-Speicheraufgabe wird ein Workfront-Speicherprojekt erstellt.

### Dokumentenverwaltung für Probleme

Beachten Sie beim Arbeiten mit Problemen Folgendes:

* Probleme übernehmen den Speichertyp aus Projekten.
* Wenn Sie ein Dokument zu einem Problem in einem Adobe-Speicherprojekt hochladen, erstellt Workfront automatisch einen Ordner im Abschnitt Dokumente des Problems. Der Ordnername entspricht dem Problem.
* Sie können den Dokumentordner umbenennen und aus dem Adobe-Unternehmensspeicherproblem löschen, wodurch auch die Dokumente im Ordner gelöscht werden. Nachdem Sie dem Problem neue Dokumente hinzugefügt haben, wird der Ordner automatisch neu erstellt. Gelöschte Dokumente werden nicht wieder im Ordner abgelegt.
* Bei Enterprise-Storage-Projekten in Adobe wird der Dokumentordner in einem Problem als Unterordner im automatisch für das Projekt erstellten Dokumentenordner angezeigt.
* Ein Problem kann nicht aus einem Workfront-Speicherprojekt in ein Adobe-Speicherprojekt kopiert oder verschoben werden. Auch das Gegenteil ist nicht möglich.
* Wenn Sie eine Anfrage mit einem an ein Workfront-Storage-Projekt angehängten Dokument senden, wird das Dokument im Bereich Dokumente der Anfrage unter Verwendung des Speichertyps des Projekts angezeigt, auch wenn die Standardeinstellung für den Systemspeicher Adobe Enterprise ist.
* Beim Konvertieren eines Problems in ein Projekt treten die folgenden Szenarien auf: <!--this info also duplicated in Convert an issue to a project-->
   * Bei einem Workfront-Speicherproblem wird ein Workfront-Speicherprojekt erstellt.
   * Bei einem Adobe-Problem mit Enterprise-Storage wird ein Adobe-Storage-Projekt erstellt.
   * Wenn Sie eine Workfront-Speichervorlage zum Konvertieren eines Adobe-Speicherproblems verwenden, wird ein Adobe-Speicherprojekt erstellt.
   * Wenn Sie eine Adobe-Speichervorlage zum Konvertieren eines Workfront-Speicherproblems verwenden, wird ein Workfront-Speicherprojekt erstellt.

### Dokumentenverwaltung für Projektvorlagen

Beachten Sie beim Arbeiten mit Vorlagen Folgendes:

* Wenn Sie eine Adobe-Unternehmensspeichervorlage erstellen, erstellt Workfront einen Ordner im Abschnitt Dokumente der Vorlage, in dem Dokumente gespeichert werden. Der Ordnername ist mit dem Programmnamen identisch. Sie können den Ordner nicht löschen oder manuell umbenennen. Der Ordner wird umbenannt, wenn Sie den Namen der Vorlage ändern, sodass er zum neuen Namen der Vorlage passt.
* Sie können eine Workfront-Speichervorlage verwenden, um Workfront-Speicherprojekte zu erstellen. Sie können eine Adobe-Speichervorlage verwenden, um ein Adobe-Speicherprojekt zu erstellen.
* Sie können eine Workfront-Speichervorlage an ein Adobe-Speicherprojekt anhängen. Dies ändert nicht den Speicherort des Projekts.
* Sie können eine Adobe-Speichervorlage an ein Workfront-Speicherprojekt anhängen. Dadurch wird der Speicherort für das Projekt nicht geändert. Dokumente im Ordner &quot;Adobe-Storage“ für die Vorlage werden dem Projekt direkt und ohne den Ordner hinzugefügt, während die Dokumente in den Vorlagenaufgabenordnern den Ordnern hinzugefügt werden, die an die Projektaufgaben im Abschnitt Dokumente der Aufgaben angehängt sind.

### Dokumentverwaltung für Vorlagenaufgaben

Beachten Sie beim Arbeiten mit Vorlagenaufgaben Folgendes:

* Vorlagenaufgaben übernehmen den Speichertyp aus Vorlagen.
* Wenn Sie ein Dokument zu einer Vorlagenaufgabe auf einer Adobe-Speichervorlage hochladen, erstellt Workfront automatisch einen Ordner im Abschnitt Dokumente der Vorlagenaufgabe. Der Ordnername entspricht dem der Vorlagenaufgabe.
* Sie können den Dokumentordner umbenennen und aus der Adobe-Vorlagenaufgabe für die Unternehmensspeicherung löschen, wodurch auch die Dokumente im Ordner gelöscht werden. Nachdem Sie der Vorlagenaufgabe neue Dokumente hinzugefügt haben, wird der Ordner automatisch neu erstellt. Gelöschte Dokumente werden nicht wieder im Ordner abgelegt.
* Bei Adobe-Enterprise-Storage-Vorlagen wird der Dokumentordner in einer Vorlagenaufgabe als Unterordner in dem automatisch für die Vorlage erstellten Dokumentenordner angezeigt.
* Sie können eine Vorlagenaufgabe nicht von einer Workfront-Speichervorlage in eine Adobe-Speichervorlage kopieren oder verschieben. Auch das Gegenteil ist nicht möglich.
* Wenn Sie ein Dokument an ein Problem anhängen, das Sie an eine mit dem Adobe-Speicher verknüpfte Anfrage-Warteschlange senden, wird für jedes gesendete Problem ein Ordner erstellt, in dem die Dokumente gespeichert werden. Der Ordner wird auch als Unterordner zum automatisch erstellten Projektordner in der Anfrage-Warteschlange hinzugefügt.
