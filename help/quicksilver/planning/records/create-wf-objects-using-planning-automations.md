---
title: Erstellen von Workfront-Objekten mithilfe von Adobe Workfront Planning-Datensatzautomatisierungen
description: Sie können Automatisierungen in Adobe Workfront Planning konfigurieren, die, wenn sie aktiviert sind, Objekte in Workfront oder Datensätze in Workfront Planning erstellen. Die erstellten Objekte und Datensätze werden automatisch mit den vorhandenen Planungsdatensätzen verbunden.
hide: true
hidefromtoc: true
exl-id: c669217a-40e2-471f-951d-93157a34f1ee
source-git-commit: 7c1bd52c6d1878b556bc92849b5d65fd0e89f51b
workflow-type: tm+mt
source-wordcount: '1307'
ht-degree: 3%

---

# Erstellen von Objekten mithilfe von Adobe Workfront Planning-Datensatzautomatisierungen

<!--add screen shots when UI is finalized AND redo all the steps - some things got changed and moved around-->
<!--when you make this public, add this to the metadata above (and take the "hide" tags out):

feature: Workfront Planning
role: User, Admin
author: Alina, Becky
recommendations: noDisplay, noCatalog

-->

<!--add a new section to this article to mention a new way to create objects: help/quicksilver/planning/records/create-records.md-->
<!-- add a new section to this article to mention a new way to create WF objects from Planning: help/quicksilver/planning/records/create-workfront-objects-from-workfront-planning.md-->

<!-- if they give access to use the automation to people with LESS than Manage permissions to a workspace, split this article in two: the Configure section should be for admins and the "Use a Workfront Planning automation to create an object" should be for all other users-->

Sie können Automatisierungen in Adobe Workfront Planning konfigurieren, die, wenn sie aktiviert sind, Objekte in Workfront erstellen oder Workfront Planning aufzeichnen. Die erstellten Objekte oder Datensätze werden automatisch mit den Datensätzen verknüpft, für die Sie die Automatisierung auslösen.

Sie können die Automatisierung auf der Seite des Datensatzes in Workfront Planning konfigurieren und aktivieren. Das erstellte verbundene Objekt wird im verbundenen Feld des Datensatztyps platziert, von dem aus die Automatisierung ausgeführt wird.

Sie können beispielsweise eine Automatisierung erstellen, die eine Workfront Planning-Kampagne benötigt und in Workfront ein Projekt erstellt, um den Fortschritt dieser Kampagne zu verfolgen. Das Projekt wird mit der Workfront Planning-Kampagne im Feld Verbundenes Projekt der Kampagne verbunden.

Weitere Informationen zu verbundenen Datensätzen finden Sie unter [Übersicht über verbundene Datensätze](/help/quicksilver/planning/records/connected-records-overview.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für Workfront Planning anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> Produkte</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront-Planung<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront-Plan*</p></td> 
   <td> 
<p>Einer der folgenden Workfront-Pläne:</p> 
<ul><li>Auswählen</li> 
<li>Erstklassig</li> 
<li>Ultimativ</li></ul> 
<p>Workfront Planning ist nicht für ältere Workfront-Pläne verfügbar</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront-Planungspaket*</p></td> 
   <td> 
<p>Beliebig </p> 
<p>Weitere Informationen zu den einzelnen Workfront-Planungsplänen erhalten Sie von Ihrem Workfront Account Manager. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront-Plattform</p></td> 
   <td> 
<p>Um auf alle Funktionen von Workfront zugreifen zu können, muss die Workfront-Instanz Ihres Unternehmens in das einheitliche Adobe-Erlebnis integriert sein.</p> 
<p>Weitere Informationen finden Sie unter <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience für Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-Lizenz*</p></td> 
   <td> Standard
   <p>Workfront Planning ist nicht für ältere Workfront-Lizenzen verfügbar</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Konfiguration der Zugriffsebene</p></td> 
   <td> <p>Es gibt keine Zugriffssteuerungsebenen für Adobe Workfront Planning</p> 
   <p>Bearbeitungszugriff in Workfront für die Objekttypen, die Sie erstellen möchten (Projekte, Portfolios, Programme). </p>  
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Objektberechtigungen</p></td> 
   <td> <p>Verwalten Sie die Berechtigungen für den Arbeitsbereich, dem Sie Datensätze hinzufügen möchten. </p>  
   <p>Systemadministratoren haben Berechtigungen für alle Arbeitsbereiche, einschließlich der nicht erstellten</p>
   <p>Verwalten Sie Berechtigungen für Workfront-Objekte (Portfolios), um untergeordnete Objekte (Projekte) hinzuzufügen.</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Layoutvorlage</p></td> 
   <td> <p>Allen Benutzern, einschließlich Workfront-Administratoren, muss eine Layoutvorlage zugewiesen werden, die den Bereich Planung im Hauptmenü enthält </p> </td> 
  </tr> 
</tbody> 
</table>

*Weitere Informationen zu Zugriffsanforderungen für Workfront finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


## Überlegungen zum Erstellen von Objekten und Datensätzen mithilfe einer Automatisierung

* Der neue Objekt- oder Datensatzname ist mit dem Datensatznamen identisch, aus dem Sie ihn erstellen. <!--take this out when they add the field mapping - no longer just the name of the original record-->
* Neue Objekte überschreiben nicht vorhandene Objekte im selben Feld.
* Die Automatisierung erstellt zusätzliche Objekte nur in den Feldern vom Typ Viele zu viele oder Eins zu viele Verbindungstypen.

## Automatisierung in Workfront Planning konfigurieren

Sie müssen in Workfront Planning eine Automatisierung für einen Datensatztyp konfigurieren, bevor Sie ihn zum Erstellen von Objekten verwenden können.

{{step1-to-planning}}

1. Klicken Sie auf eine Karte für den Datensatztyp und dann auf den Namen eines Datensatzes.

   Die Seite mit dem Datensatztyp wird geöffnet.
1. Klicken Sie auf das **Mehr**-Menü ![](assets/more-menu.png) rechts neben dem Namen des Datensatztyps und dann auf **Automatisierungen verwalten**.

   Die Liste der verfügbaren Automatisierungen wird geöffnet.

1. Klicken Sie **Neue Automatisierung** in der oberen rechten Ecke des Bildschirms. Das Feld **Neue**&quot; wird geöffnet.
1. Aktualisieren Sie die folgenden Felder:

   * Ersetzen **Nicht benannte Automatisierung** durch den Text, der auf der Schaltfläche „Automatisierung“ angezeigt werden soll. Benutzer klicken auf diese Schaltfläche, wenn sie die Automatisierung zum Erstellen eines Workfront-Objekts oder eines Planungsdatensatzes verwenden.
   * **Beschreibung**: Fügen Sie eine Beschreibung hinzu, um den Zweck der Automatisierung anzugeben.
1. Klicken Sie **Speichern**.
Die Seite mit den Automatisierungsdetails wird geöffnet.

1. Aktualisieren Sie auf der Detailseite der Automatisierung die folgenden Felder im Abschnitt **Trigger**:

   * **Trigger**: Wählen Sie die Aktion aus, durch die die Automatisierung Trigger werden soll. Wählen Sie beispielsweise **Schaltflächen-Klick** aus. <!--update this step with a list of all possible triggers; right not only Button click is available-->

1. Aktualisieren Sie die folgenden Felder im Abschnitt **Aktionen**: <!--submitted bugs for these fields - see if they need changing here-->
   * **Objekttyp**: Wählen Sie das Objekt aus, das die Automatisierung erstellen soll. Dies ist ein Pflichtfeld.

     Sie können die folgenden Objekte aus Workfront Planning-Datensätzen erstellen:

      * Projekt
      * Portfolio
      * Programm
      * Gruppe
      * Eintrag
1. (Bedingt) Aktualisieren Sie je nachdem, welchen Objekttyp Sie erstellen möchten, die folgenden Felder:

   * **Projekt**:
      * **Verbundenes Feld, in dem das Objekt erstellt wird**: Dies ist das verbundene Feld, in dem das neue Projekt angezeigt wird. Dies ist ein Pflichtfeld
      * **Vorlage, aus der das Projekt erstellt werden soll**: Wählen Sie eine Projektvorlage aus, die Workfront zum Erstellen des Projekts verwenden soll.
   * **Portfolio**:
      * **Verbundenes Feld, in dem das Objekt erstellt wird**: Dies ist das verbundene Feld, in dem das neue Portfolio angezeigt wird. Dies ist ein Pflichtfeld.
      * **Benutzerdefiniertes Formular, das an das neue Portfolio angehängt werden soll**: Wählen Sie ein benutzerdefiniertes Formular aus, das an das neue Portfolio angehängt werden soll. Sie müssen ein benutzerdefiniertes Portfolio-Formular erstellen, bevor Sie es auswählen können.
   * **Programm**:
      * **Verbundenes Feld, in dem das Objekt erstellt wird**: Dies ist das verbundene Feld, in dem das neue Programm angezeigt wird. Dies ist ein Pflichtfeld.
      * **Programm-**: Wählen Sie ein Portfolio aus, in dem das neue Programm hinzugefügt werden soll. Dies ist ein Pflichtfeld.
      * 
         * **Benutzerdefiniertes Formular, das an das neue Programm angehängt werden soll**: Wählen Sie ein benutzerdefiniertes Formular aus, das an das neue Programm angehängt werden soll. Sie müssen ein benutzerdefiniertes Programmformular erstellen, bevor Sie es auswählen können.
   * **Gruppe**:
      * **Verbundenes Feld, in dem das Objekt erstellt wird**: Dies ist das verbundene Feld, in dem die neue Gruppe angezeigt wird. Dies ist ein Pflichtfeld.
      * **Benutzerdefiniertes Formular, das an die neue Gruppe angehängt werden soll**: Wählen Sie ein benutzerdefiniertes Formular aus, das an das neue Programm angehängt werden soll. Sie müssen ein benutzerdefiniertes Programmformular erstellen, bevor Sie es auswählen können.
   * **Eintrag**:
      * **Verbundener Datensatztyp**: Wählen Sie den Datensatztyp aus, den Sie erstellen möchten.
      * **Verbundenes Feld, in dem der Datensatz erstellt wird**: Dies ist das verbundene Feld, in dem der neue Datensatz angezeigt wird. Dies ist ein Pflichtfeld. <!--this might need revision as right now it shows the field on the connected record table where the current record will display; submitted a bug to correct this label-->
      * **Felder zuordnen**
         * **Übertragen von**: Wählen Sie Felder aus dem Datensatztyp aus, für den die Automatisierung erstellt wird, um sie den Feldern des verbundenen Datensatztyps zuzuordnen.
      * **Übertragen an**: Wählen Sie Felder aus dem neu erstellten Datensatz aus, die mit Informationen aus dem Datensatz gefüllt werden, für den Sie die Automatisierung ausführen.
1. (Optional und bedingt) Wenn Sie ausgewählt haben, einen Datensatz zu erstellen, klicken Sie auf **Felder hinzufügen**, um zusätzliche Suchfelder von einem Datensatz einem anderen zuzuordnen.
1. (Optional und bedingt) Wenn Sie kein Verbindungsfeld für einen Workfront-Objekttyp haben, klicken Sie auf das Symbol **Verbindungsfeld erstellen**, ![](assets/create-a-connection-field-icon.png) ein Feld hinzuzufügen.
1. Klicken **oben** auf der Seite mit den Automatisierungsdetails auf „Speichern“.

   Die Automatisierung wird in der Liste der Automatisierungen angezeigt und kann in Datensätzen verwendet werden.
1. (Optional) Gehen Sie wie folgt vor, um eine Automatisierung zu bearbeiten, zu deaktivieren oder zu löschen:

   1. Bewegen Sie in der Liste der Automatisierungen den Mauszeiger über den Namen einer gespeicherten Automatisierung und klicken Sie dann auf das **Mehr**-![](assets/more-menu.png).

   1. Klicken Sie **Bearbeiten**, um Informationen über Felder in der Automatisierung zu aktualisieren und sie zu konfigurieren.
   1. Klicken Sie auf **Deaktivieren**, um die Automatisierung aus der Tabellenansicht zu entfernen und zu verhindern, dass Benutzer sie zum Erstellen von Datensätzen oder Objekten verwenden. Um sie wieder verfügbar zu machen, klicken Sie erneut auf das **Mehr**-Menü ![](assets/more-menu.png) anschließend auf **Aktivieren**.
   1. Klicken Sie **Löschen**, um die Automatisierung zu löschen. Eine gelöschte Automatisierung kann nicht wiederhergestellt werden. Datensätze, die mithilfe der Automatisierung erstellt wurden, bleiben mit dem ursprünglich ausgewählten Datensatz verbunden.

## Verwenden einer Workfront Planning-Automatisierung, um ein Objekt oder einen Datensatz zu erstellen

1. Öffnen Sie in Workfront Planning die Seite „Datensatztyp“, die die Datensätze enthält, die Sie zum Erstellen von Workfront-Objekten oder Planning-Datensätzen verwenden möchten.
1. Öffnen Sie die Tabellenansicht.
1. Einen oder mehrere Datensätze auswählen.

   Unten in der Tabelle wird ein blauer Balken mit zusätzlichen Schaltflächen, einschließlich Automatisierungsschaltflächen, angezeigt.
1. Klicken Sie auf die Schaltfläche Automatisierung in der rechten unteren Ecke des Bildschirms.

   ![Schaltfläche „Automatisierung](assets/automation-custom-button.png)

   Wenn die Automatisierung ein Objekt oder einen Datensatz erfolgreich erstellt hat, wird unten im Bildschirm eine Bestätigungsmeldung angezeigt.

   Das neue Objekt wird in dem verbundenen Feld angezeigt, das Sie beim Einrichten der Automatisierungsschaltfläche angegeben haben. Möglicherweise müssen Sie die Seite aktualisieren, bevor Sie das neue Objekt anzeigen.

   >[!NOTE]
   >
   >Es wird empfohlen zu überprüfen, ob das Objekt erwartungsgemäß erstellt und verbunden wurde.

1. (Optional) Klicken Sie auf das neue Objekt im verbundenen Feld. Die Seite „Objekt“ wird geöffnet, und Sie können zusätzliche Änderungen am neuen Objekt vornehmen.

<!--you might need to add something about notifications and emails?!-->
