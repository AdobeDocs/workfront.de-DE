---
title: Feldeinstellungen bearbeiten
description: In Adobe Workfront Planning können Sie die Feldeinstellungen für Felder bearbeiten, die bereits erstellt wurden. Dieser Artikel beschreibt, wie Sie die Einstellungen für Workfront Planning-Felder bearbeiten können.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 6c35c313-d6ed-428b-b70d-2ea242da4e8f
source-git-commit: fd8e5d3baf6af0dbdd1275494fad54b204abd1a5
workflow-type: tm+mt
source-wordcount: '708'
ht-degree: 1%

---


# Bearbeiten von Feldeinstellungen

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>   -->

{{planning-important-intro}}

Sie können die Feldeinstellungen für Felder bearbeiten, die bereits in Adobe Workfront Planning erstellt wurden.

Informationen zum Erstellen von Adobe Workfront Planning-Feldern finden Sie unter [Felder erstellen](/help/quicksilver/planning/fields/create-fields.md).

Dieser Artikel beschreibt, wie Sie die Einstellungen für Workfront Planning-Felder bearbeiten können. Informationen zum Bearbeiten von Feldwerten für Datensätze finden Sie unter [Datensätze bearbeiten](/help/quicksilver/planning/records/edit-records.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen anzuzeigen.

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
<p>Weitere Informationen finden Sie unter <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-Lizenz*</p></td> 
   <td><p> Standard </p>
   <p>Workfront Planning ist nicht für ältere Workfront-Lizenzen verfügbar</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Konfiguration der Zugriffsebene</p></td> 
   <td> <p>Es gibt keine Zugriffssteuerungsebenen für Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Objektberechtigungen</p></td> 
   <td>   <p>Verwalten von Berechtigungen für einen Arbeitsbereich <!--<span class="preview">and record type</span>--> </a> </p>  
   <p>Systemadministratoren haben Berechtigungen für alle Arbeitsbereiche, einschließlich der nicht erstellten</p></td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Layoutvorlage</p></td> 
   <td> <p>Allen Benutzern, einschließlich Workfront-Administratoren, muss eine Layoutvorlage zugewiesen werden, die den Bereich Planung im Hauptmenü enthält. </p> </td> 
  </tr> 
</tbody> 
</table>

*Weitere Informationen zu Zugriffsanforderungen für Workfront finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


<!--
OLD

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Product</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront agreement</p></td>
   <td>
<p>Your organization must be enrolled in the early access stage for Workfront Planning </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront plan</p></td>
   <td>
<p>Any</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront license*</p></td>
   <td>
   <p>New: Standard</p>
   <p>Current: Plan</p> 
  </td>
  </tr>
  
  <tr>
   <td role="rowheader"><p>Access level configuration</p></td>
   <td> <p>There are no access controls for Workfront Planning</p>  
</td>
  </tr>

  <tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>Manage permissions to a workspace</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>Your Workfront or group administrator must add the Planning area in your layout template. For information, see <a href="/help/quicksilver/planning/access/access-overview.md">Access overview</a>. </p>  
</td>
  </tr>

 </tbody>
</table>

*For more information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). 

-->

## Überlegungen zum Bearbeiten von Feldeinstellungen

Bevor Sie die Konfiguration eines Felds ändern, müssen Sie Folgendes beachten:

* Sie können von Ihnen erstellte Felder oder Felder, die von anderen Benutzern erstellt wurden, bearbeiten, wenn Sie über Verwaltungsberechtigungen für den Arbeitsbereich verfügen, zu dem die Felder gehören.
* Sie können ein Feld in der Datensatztyp-Tabelle bearbeiten.
* Ein Feld kann weder auf der Datensatzseite noch in einer anderen Ansicht außerhalb der Tabellenansicht bearbeitet werden.
* Nach dem Speichern des Felds ist keine Bearbeitung des Feldtyps möglich.
* Sie können die Auswahl der Einstellung Negative Zahlen zulassen , die zuvor für ein Feld vom Typ Zahl, Prozentsatz oder Währung ausgewählt wurde, nicht aufheben, wenn bereits negative Werte für die Datensätze gespeichert sind, an die sie angehängt ist.
* Sie können die Konfiguration der folgenden Feldelemente bearbeiten, nachdem Sie das Feld gespeichert haben:

   * Der Name oder die Beschreibung eines beliebigen Felds
   * Die Optionen eines Einzelauswahl- oder Mehrfachauswahl-Felds.
   * Der Ausdruck eines Formelfelds.

  >[!WARNING]
  >
  >Wenn Formelausdrücke geändert werden oder Optionen einem Feld vom Typ Auswahl hinzugefügt oder daraus entfernt werden, gehen Daten für die Datensätze verloren, die bereits Informationen in den Feldern enthalten, deren Konfiguration geändert wird.
  >
  >Es gibt keine Warnung oder Anzeige dafür, dass dieser Datenverlust auftreten könnte, wenn Sie die Konfiguration von Feldern ändern.
  >
  >Andere Benutzer werden nicht darüber informiert, dass sich die Feldkonfiguration geändert hat.

<!--this is not yet true, but it might come later:
* You can deselect Allow negative numbers option from a Number, Percentage, or Currency field after you save the field. 
-->

## Bearbeiten von Feldeinstellungen

{{step1-to-planning}}

1. Klicken Sie auf den Arbeitsbereich, dessen Datensatzfelder Sie bearbeiten möchten.

   Der Arbeitsbereich wird geöffnet und alle Datensatztypen im Arbeitsbereich werden auf Karten angezeigt.

1. Klicken Sie auf die Karte eines Datensatztyps.

   Dadurch wird die Seite des Datensatztyps geöffnet.

1. (Bedingt) Klicken Sie auf die Registerkarte einer **Tabellenansicht**.

   Alle vorhandenen Datensätze, die mit dem Datensatztyp verknüpft sind, werden in den Zeilen der Tabellenansicht angezeigt.
1. Bewegen Sie den Mauszeiger über die Spaltenüberschrift eines Felds, das Sie bearbeiten möchten, klicken Sie dann auf den nach unten zeigenden Pfeil nach dem Feldnamen und dann auf **Feld bearbeiten**

   Oder

   Doppelklicken Sie auf die Spaltenüberschrift für das Feld.

   ![](assets/arrow-menu-after-name-of-field-in-table-header-highlighted.png)

1. Aktualisieren Sie die Informationen zum Feld und klicken Sie auf **Speichern**. <!--insert screen shot when finalized-->

   >[!TIP]
   >
   >* Sie können den Feldtyp nach dem Speichern des Felds nicht mehr aktualisieren.
   >
   >* Wenn Sie Feldkonfigurationen ändern (Feldoptionen oder Formelausdrücke), werden die Werte von Datensätzen, die bereits Informationen in den geänderten Feldern enthalten, in Echtzeit aktualisiert. Es gibt keine Warnung und kein Administratorprotokoll für die Wertänderungen, die durch Änderungen der Feldkonfiguration ausgelöst werden. Alle Benutzer, die die Felder anzeigen, sehen sofort die neuen Werte mit den Änderungen.

   Die Feldinformationen werden für alle Benutzer aktualisiert, die Zugriff auf den Arbeitsbereich haben.

1. (Bedingt) Klicken Sie bei verknüpften Datensatzfeldern auf **Suchfelder bearbeiten** und fügen Sie dem verknüpften Datensatztyp beliebige Felder hinzu oder entfernen Sie sie.

   Weitere Informationen finden Sie unter [Verbinden von Datensatztypen](/help/quicksilver/planning/architecture/connect-record-types.md).

