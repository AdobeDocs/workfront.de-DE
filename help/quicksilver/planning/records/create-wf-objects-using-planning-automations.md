---
title: Erstellen von Workfront-Objekten mit Adobe Workfront-Planungs-Datensatzautomatisierungen
description: Sie können Automatisierungen in der Workfront-Planung konfigurieren, die bei Aktivierung Objekte in Workfront erstellen.
hide: true
hidefromtoc: true
exl-id: c669217a-40e2-471f-951d-93157a34f1ee
source-git-commit: 03eedb00ab45b95e87670872cf015c0f6840658e
workflow-type: tm+mt
source-wordcount: '1071'
ht-degree: 4%

---

# Erstellen von Objekten mit der Adobe Workfront-Planungs-Datensatzautomatisierung

<!--add screen shots when UI is finalized-->
<!--when you make this public, add this to the metadata above (and take the "hide" tags out):

feature: Workfront Planning
role: User, Admin
author: Alina, Becky
recommendations: noDisplay, noCatalog

-->

Sie können Automatisierungen in der Adobe Workfront-Planung konfigurieren, die bei Aktivierung Objekte in der Workfront- oder Workfront-Planung erstellen.

Sie können die Automatisierung auf der Datensatzseite konfigurieren und aktivieren. Das Objekt, das erstellt wird, ist mit dem Planungsdatensatz verbunden und platziert in dem Feld, das Sie in der Automatisierung angeben.

Sie können beispielsweise eine Automatisierung erstellen, die eine Workfront-Planungs-Kampagne durchführt und in Workfront ein Projekt erstellt, um den Fortschritt dieser Kampagne zu verfolgen. Das Projekt würde mit der Workfront-Planungskampagne verbunden sein.

Weitere Informationen zu verbundenen Datensätzen finden Sie unter [Übersicht über verbundene Datensätze](/help/quicksilver/planning/records/connected-records-overview.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Workfront-Planung anzuzeigen.

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
<p>Die folgenden Workfront-Pläne:</p> 
<ul><li>Auswählen</li> 
<li>Erstklassig</li> 
<li>Ultimativ</li></ul> 
<p>Die Workfront-Planung ist für veraltete Workfront-Pläne nicht verfügbar</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront-Planungspaket*</p></td> 
   <td> 
<p>Alle </p> 
<p>Weitere Informationen zu den Funktionen der einzelnen Workfront-Planungspläne erhalten Sie von Ihrem Workfront-Kundenbetreuer. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront-Plattform</p></td> 
   <td> 
<p>Die Workfront-Instanz Ihres Unternehmens muss in das Adobe Unified Experience integriert sein, damit Sie auf alle Funktionen der Workfront-Planung zugreifen können.</p> 
<p>Weitere Informationen finden Sie unter <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-Lizenz*</p></td> 
   <td> Standard
   <p>Für ältere Workfront-Lizenzen ist die Workfront-Planung nicht verfügbar.</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Konfiguration der Zugriffsebene</p></td> 
   <td> <p>Für die Adobe Workfront-Planung gibt es keine Zugriffssteuerungselemente</p> 
   <p>Bearbeiten Sie den Zugriff in Workfront für die Objekttypen, die Sie erstellen möchten (Projekte, Portfolios, Programme). </p>  
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Objektberechtigungen</p></td> 
   <td> <p>Verwalten Sie Berechtigungen für den Arbeitsbereich, dem Sie Datensätze hinzufügen möchten. </p>  
   <p>Systemadministratoren haben Berechtigungen für alle Arbeitsbereiche, einschließlich derjenigen, die sie nicht erstellt haben</p>
   <p>Verwalten Sie Berechtigungen für Workfront-Objekte (Portfolios), um untergeordnete Objekte (Projekte) hinzuzufügen.</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Layout-Vorlage</p></td> 
   <td> <p>Allen Benutzern, einschließlich Workfront-Administratoren, muss eine Layoutvorlage zugewiesen werden, die den Planungsbereich im Hauptmenü enthält </p> </td> 
  </tr> 
</tbody> 
</table>

*Weitere Informationen zu den Zugriffsanforderungen für Workfront finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


## Überlegungen zum Erstellen von Objekten und Datensätzen mithilfe einer Automatisierung

* Der neue Objekt- oder Datensatzname entspricht dem Datensatznamen, aus dem Sie ihn erstellen.
* Wenn der Datensatz, für den Sie die Automatisierung verwenden, bereits Objekte desselben Typs in dem Feld verknüpft hat, das Sie zum Hinzufügen neuer Objekte auswählen, werden die neuen Objekte zum Verbindungsfeld hinzugefügt und vorhandene Objekte bleiben ebenfalls verbunden.


## Automatisierung in der Workfront-Planung konfigurieren

Sie müssen eine Automatisierung in der Workfront-Planung konfigurieren, bevor Sie sie zum Erstellen von Objekten verwenden können.

{{step1-to-planning}}

1. Klicken Sie auf eine Karte vom Typ Datensatz und dann auf den Namen eines Datensatzes.

   Die Seite mit dem Datensatztyp wird geöffnet.
1. Klicken Sie auf das Menü **Mehr** rechts neben dem Namen des Datensatztyps und dann auf **Automatisierung verwalten**.![](assets/more-menu.png)

   Die Liste der verfügbaren Automatisierungen wird geöffnet.

1. Klicken Sie oben rechts im Bildschirm auf **Neue Automatisierung** .
1. Aktualisieren Sie die folgenden Felder:

   * **Schaltflächentext**: Geben Sie den Text ein, der auf der Automatisierungsschaltfläche angezeigt werden soll. Benutzer klicken auf diese Schaltfläche, wenn sie die Automatisierung zum Erstellen eines Workfront-Objekts verwenden.
   * **Schaltflächensymbol**: Wählen Sie ein Symbol für die Schaltfläche aus. Standardmäßig ist ein Symbol ausgewählt.
   * **Objekttyp**: Wählen Sie das Objekt aus, das durch die Automatisierung erstellt werden soll. Dies ist ein Pflichtfeld.

     Sie können die folgenden Objekte aus Workfront Planning-Datensätzen erstellen:

      * Projekt
      * Portfolio
      * Programm
      * Gruppe
      * Datensatz
1. (Bedingt) Abhängig vom Objekttyp, den Sie erstellen möchten, aktualisieren Sie die folgenden Felder:

   * **Projekt**:
      * **Verbundenes Feld, in dem das Objekt erstellt wird**: Dies ist das verbundene Feld, in dem das neue Projekt angezeigt wird. Dies ist ein Pflichtfeld
      * **Vorlage, aus der das Projekt erstellt werden**: Wählen Sie eine Projektvorlage aus, die Workfront zum Erstellen des Projekts verwendet.
   * **Portfolio**:
      * **Verbundenes Feld, in dem das Objekt erstellt wird**: Dies ist das verbundene Feld, in dem das neue Portfolio angezeigt wird. Dies ist ein Pflichtfeld.
      * **Benutzerdefiniertes Formular, das an das neue Portfolio angehängt wird**: Wählen Sie ein benutzerdefiniertes Formular aus, das an das neue Portfolio angehängt werden soll. Sie müssen ein benutzerdefiniertes Portfolio-Formular erstellen, bevor Sie es auswählen können.
   * **Programm**:
      * **Verbundenes Feld, in dem das Objekt erstellt wird**: Dies ist das verbundene Feld, in dem das neue Programm angezeigt wird. Dies ist ein Pflichtfeld.
      * **Programmportfolio**: Wählen Sie ein Portfolio aus, in dem das neue Programm hinzugefügt wird. Dies ist ein Pflichtfeld.
      * 
         * **Benutzerdefiniertes Formular zum Anhängen an das neue Programm**: Wählen Sie ein benutzerdefiniertes Formular aus, das an das neue Programm angehängt werden soll. Sie müssen ein benutzerdefiniertes Programmformular erstellen, bevor Sie es auswählen können.
   * **Gruppe**:
      * **Verbundenes Feld, in dem das Objekt erstellt wird**: Dies ist das verbundene Feld, in dem die neue Gruppe angezeigt wird. Dies ist ein Pflichtfeld.
      * **Benutzerdefiniertes Formular, das an die neue Gruppe angehängt werden soll**: Wählen Sie ein benutzerdefiniertes Formular aus, das an das neue Programm angehängt werden soll. Sie müssen ein benutzerdefiniertes Programmformular erstellen, bevor Sie es auswählen können.
   * **Record**:
      * **Connected record type**: Wählen Sie den zu erstellenden Datensatztyp aus.
      * **Verbundenes Feld, in dem der Datensatz erstellt wird**: Dies ist das verbundene Feld, in dem der neue Datensatz angezeigt wird. Dies ist ein Pflichtfeld.
      * **Feld zuordnen**: Wählen Sie Felder aus dem Datensatztyp aus, für den die Automatisierung erstellt wird, um sie den Feldern des verbundenen Datensatztyps zuzuordnen.
      * **An das Feld für den verbundenen Datensatz**: Wählen Sie Felder aus dem verbundenen Datensatz aus, die den Feldern des Datensatztyps entsprechen, für den Sie die Automatisierung erstellen.
1. (Optional und bedingt) Wenn Sie kein Verbindungsfeld für einen Workfront-Objekttyp haben, klicken Sie auf das Symbol **Verbindungsfeld erstellen** ![](assets/create-a-connection-field-icon.png) , um ein Feld hinzuzufügen.
1. (Optional und bedingt) Wenn Sie ausgewählt haben, um einen Datensatz hinzuzufügen, klicken Sie im Bereich **Zugeordnete Felder zuordnen** auf **Hinzufügen** , um weitere Felder hinzuzufügen und zuzuordnen.
1. Klicken Sie auf **Erstellen**

Die Automatisierung wird in der Liste der Automatisierungen angezeigt und kann in Datensätzen verwendet werden.

## Verwenden einer Workfront-Planungs-Automatisierung zum Erstellen eines Objekts

1. Öffnen Sie in der Workfront-Planung die Seite &quot;Record Type&quot;, die die Datensätze enthält, die Sie zum Erstellen von Workfront-Objekten verwenden möchten.
1. Öffnen Sie die Tabellenansicht.
1. Wählen Sie mindestens einen Datensatz aus.

   Unten in der Tabelle wird ein blauer Balken mit zusätzlichen Schaltflächen, einschließlich Automatisierungsschaltflächen, angezeigt.
1. Klicken Sie unten rechts im Bildschirm auf die Schaltfläche Automatisierung .

   ![Automatisierungsschaltfläche](assets/automation-custom-button.png)

   Das neue Objekt wird im verbundenen Feld angezeigt, das Sie in der Einrichtung der Automatisierungsschaltfläche angegeben haben.

   >[!NOTE]
   >
   >Es wird empfohlen, zu überprüfen, ob das Objekt erwartungsgemäß erstellt und verbunden wurde.

1. (Optional) Klicken Sie auf das neue Objekt im verbundenen Feld. Die Objektseite wird geöffnet und Sie können zusätzliche Änderungen am neuen Objekt vornehmen.

<!--you might need to add something about notifications and emails?!-->
