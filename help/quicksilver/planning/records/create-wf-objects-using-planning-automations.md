---
title: Erstellen von Workfront-Objekten mithilfe von Adobe Workfront Planning-Datensatzautomatisierungen
description: Sie können Automatisierungen in Workfront Planning konfigurieren, die, wenn sie aktiviert sind, Objekte in Workfront erstellen.
hide: true
hidefromtoc: true
exl-id: c669217a-40e2-471f-951d-93157a34f1ee
source-git-commit: 03eedb00ab45b95e87670872cf015c0f6840658e
workflow-type: tm+mt
source-wordcount: '1071'
ht-degree: 4%

---

# Erstellen von Objekten mithilfe von Adobe Workfront Planning-Datensatzautomatisierungen

<!--add screen shots when UI is finalized-->
<!--when you make this public, add this to the metadata above (and take the "hide" tags out):

feature: Workfront Planning
role: User, Admin
author: Alina, Becky
recommendations: noDisplay, noCatalog

-->

Sie können Automatisierungen in Adobe Workfront Planning konfigurieren, die, wenn sie aktiviert sind, Objekte in Workfront oder Workfront Planning erstellen.

Sie können die Automatisierung auf der Seite des Datensatzes konfigurieren und aktivieren. Das erstellte Objekt wird mit dem Planungsdatensatz verbunden und in dem Feld platziert, das Sie in der Automatisierung angeben.

Sie können beispielsweise eine Automatisierung erstellen, die eine Workfront Planning-Kampagne benötigt und in Workfront ein Projekt erstellt, um den Fortschritt dieser Kampagne zu verfolgen. Das Projekt würde mit der Workfront-Planungskampagne verbunden.

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

* Der neue Objekt- oder Datensatzname ist mit dem Datensatznamen identisch, aus dem Sie ihn erstellen.
* Wenn der Datensatz, für den Sie die Automatisierung verwenden, bereits Objekte desselben Typs in dem Feld, das Sie zum Hinzufügen neuer Objekte auswählen, verbunden hat, werden die neuen Objekte zum Verbindungsfeld hinzugefügt und die vorhandenen Objekte bleiben ebenfalls verbunden.


## Automatisierung in Workfront Planning konfigurieren

Sie müssen eine Automatisierung in Workfront Planning konfigurieren, bevor Sie sie zum Erstellen von Objekten verwenden können.

{{step1-to-planning}}

1. Klicken Sie auf eine Karte für den Datensatztyp und dann auf den Namen eines Datensatzes.

   Die Seite mit dem Datensatztyp wird geöffnet.
1. Klicken Sie auf das **Mehr**-Menü ![](assets/more-menu.png) rechts neben dem Namen des Datensatztyps und dann auf **Automatisierungen verwalten**.

   Die Liste der verfügbaren Automatisierungen wird geöffnet.

1. Klicken Sie **Neue Automatisierung** in der oberen rechten Ecke des Bildschirms.
1. Aktualisieren Sie die folgenden Felder:

   * **Schaltflächentext**: Geben Sie den Text ein, der auf der Automatisierungsschaltfläche angezeigt werden soll. Benutzer klicken auf diese Schaltfläche, wenn sie die Automatisierung zum Erstellen eines Workfront-Objekts verwenden.
   * **Schaltflächensymbol**: Wählen Sie ein Symbol für die Schaltfläche aus. Standardmäßig ist ein Symbol ausgewählt.
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
      * **Verbundenes Feld, in dem der Datensatz erstellt wird**: Dies ist das verbundene Feld, in dem der neue Datensatz angezeigt wird. Dies ist ein Pflichtfeld.
      * **Feld zuordnen**: Wählen Sie Felder aus dem Datensatztyp aus, für den die Automatisierung erstellt wird, um sie den Feldern des verbundenen Datensatztyps zuzuordnen.
      * **Feld „Zu verbundenem Datensatz**: Wählen Sie Felder aus dem verbundenen Datensatz aus, die den Feldern des Datensatztyps entsprechen, für den Sie die Automatisierung erstellen.
1. (Optional und bedingt) Wenn Sie kein Verbindungsfeld für einen Workfront-Objekttyp haben, klicken Sie auf das Symbol **Verbindungsfeld erstellen**, ![](assets/create-a-connection-field-icon.png) ein Feld hinzuzufügen.
1. (Optional und bedingt) Wenn Sie einen Datensatz hinzufügen möchten, klicken Sie auf **Hinzufügen** im Bereich **Verbundene Felder zuordnen**, um zusätzliche Felder hinzuzufügen und zuzuordnen.
1. Klicken Sie auf **Erstellen**

Die Automatisierung wird in der Liste der Automatisierungen angezeigt und kann in Datensätzen verwendet werden.

## Verwenden einer Workfront Planning Automation, um ein Objekt zu erstellen

1. Öffnen Sie in Workfront Planning die Seite „Datensatztyp“, die die Datensätze enthält, die Sie zum Erstellen von Workfront-Objekten verwenden möchten.
1. Öffnen Sie die Tabellenansicht.
1. Einen oder mehrere Datensätze auswählen.

   Unten in der Tabelle wird ein blauer Balken mit zusätzlichen Schaltflächen, einschließlich Automatisierungsschaltflächen, angezeigt.
1. Klicken Sie auf die Schaltfläche Automatisierung in der rechten unteren Ecke des Bildschirms.

   ![Schaltfläche „Automatisierung](assets/automation-custom-button.png)

   Das neue Objekt wird in dem verbundenen Feld angezeigt, das Sie beim Einrichten der Automatisierungsschaltfläche angegeben haben.

   >[!NOTE]
   >
   >Es wird empfohlen zu überprüfen, ob das Objekt erwartungsgemäß erstellt und verbunden wurde.

1. (Optional) Klicken Sie auf das neue Objekt im verbundenen Feld. Die Seite „Objekt“ wird geöffnet, und Sie können zusätzliche Änderungen am neuen Objekt vornehmen.

<!--you might need to add something about notifications and emails?!-->
