---
title: Feldeinstellungen bearbeiten
description: In der Adobe Workfront-Planung können Sie die Feldeinstellungen für bereits erstellte Felder bearbeiten. In diesem Artikel wird beschrieben, wie Sie die Einstellungen für die Workfront-Planungsfelder bearbeiten können.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 6c35c313-d6ed-428b-b70d-2ea242da4e8f
source-git-commit: 9debb7c6d9df0f9f4962f3e66f146e5f605d20f0
workflow-type: tm+mt
source-wordcount: '711'
ht-degree: 1%

---


# Feldeinstellungen bearbeiten

{{planning-important-intro}}

Sie können die Feldeinstellungen für Felder bearbeiten, die bereits in der Adobe Workfront-Planung erstellt wurden.

Informationen zum Erstellen von Adobe Workfront-Planungsfeldern finden Sie unter [Felder erstellen](/help/quicksilver/planning/fields/create-fields.md).

In diesem Artikel wird beschrieben, wie Sie die Einstellungen für die Workfront-Planungsfelder bearbeiten können. Informationen zum Bearbeiten von Feldwerten für Datensätze finden Sie unter [Datensätze bearbeiten](/help/quicksilver/planning/records/edit-records.md).

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
   <td role="rowheader"><p>Adobe Workfront-Planungsplan*</p></td> 
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
   <td><p> Standard </p>
   <p>Für ältere Workfront-Lizenzen ist die Workfront-Planung nicht verfügbar.</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Konfiguration der Zugriffsebene</p></td> 
   <td> <p>Für die Adobe Workfront-Planung gibt es keine Zugriffssteuerungselemente</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Objektberechtigungen</p></td> 
   <td>   <p>Berechtigungen für einen Arbeitsbereich verwalten</a> </p>  
   <p>Systemadministratoren haben Berechtigungen für alle Arbeitsbereiche, einschließlich derjenigen, die sie nicht erstellt haben</p></td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Layout-Vorlage</p></td> 
   <td> <p>Allen Benutzern, einschließlich Workfront-Administratoren, muss eine Layoutvorlage zugewiesen werden, die den Planungsbereich im Hauptmenü enthält. </p> </td> 
  </tr> 
</tbody> 
</table>

*Weitere Informationen zu den Zugriffsanforderungen für Workfront finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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

Beachten Sie Folgendes, bevor Sie Änderungen an der Konfiguration eines Felds vornehmen:

* Sie können von Ihnen erstellte Felder oder von anderen Benutzern erstellte Felder bearbeiten, wenn Sie über Verwaltungsberechtigungen für den Arbeitsbereich verfügen, zu dem die Felder gehören.
* Sie können ein Feld in der Tabelle vom Typ Datensatz bearbeiten.
* Sie können ein Feld auf der Datensatzseite oder in einer anderen Ansicht außerhalb der Tabellenansicht nicht bearbeiten.
* Nach dem Speichern des Felds können Sie den Feldtyp nicht mehr bearbeiten.
* Die Auswahl der zuvor ausgewählten Einstellung Negative Zahlen zulassen für ein Feld vom Typ Zahl, Prozentsatz oder Währung kann nicht aufgehoben werden, wenn bereits negative Werte in den Datensätzen gespeichert sind, an die das Feld angehängt ist.
* Nach dem Speichern des Felds können Sie die Konfiguration der folgenden Feldelemente bearbeiten:

   * Der Name oder die Beschreibung eines beliebigen Felds
   * Die Optionen eines Einzelauswahl- oder eines Mehrfachauswahlfelds.
   * Der Ausdruck eines Formelfelds.

  >[!WARNING]
  >
  >Wenn sich Formelausdrücke ändern oder Optionen aus einem Auswahlfeld hinzugefügt oder entfernt werden, gehen Daten für die Datensätze verloren, die bereits über Informationen verfügen, die in den Feldern gespeichert sind, deren Konfiguration geändert wird.
  >
  >Es gibt keine Warnung oder Hinweise darauf, dass dieser Datenverlust auftreten kann, wenn Sie die Konfiguration der Felder ändern.
  >
  >Es gibt keine Benachrichtigung für andere Benutzer, dass die Feldkonfiguration geändert wurde.

<!--this is not yet true, but it might come later:
* You can deselect Allow negative numbers option from a Number, Percentage, or Currency field after you save the field. 
-->

## Feldeinstellungen bearbeiten

{{step1-to-planning}}

1. Klicken Sie auf den Arbeitsbereich, dessen Datensatzfelder Sie bearbeiten möchten.

   Der Arbeitsbereich wird geöffnet und alle Datensatztypen im Arbeitsbereich werden auf Karten angezeigt.

1. Klicken Sie auf die Karte eines Datensatztyps.

   Dadurch wird die Seite des Datensatztyps geöffnet.

1. (Bedingt) Klicken Sie auf die Registerkarte einer **Tabellenansicht**.

   Alle vorhandenen Datensätze, die mit dem Datensatztyp verknüpft sind, werden in den Zeilen der Tabellenansicht angezeigt.
1. Bewegen Sie den Mauszeiger über die Spaltenüberschrift eines Felds, das Sie bearbeiten möchten, und klicken Sie dann auf den nach unten zeigenden Pfeil nach dem Feldnamen und klicken Sie dann auf **Feld bearbeiten**

   Oder

   Doppelklicken Sie auf die Spaltenüberschrift für das Feld.

   ![](assets/arrow-menu-after-name-of-field-in-table-header-highlighted.png)

1. Aktualisieren Sie die Informationen zum Feld und klicken Sie auf **Speichern**. <!--insert screen shot when finalized-->

   >[!TIP]
   >
   >* Nach dem Speichern des Felds kann der Feldtyp nicht mehr aktualisiert werden.
   >
   >* Wenn Sie Feldkonfigurationen ändern (Feldoptionen oder Formelausdrücke), werden Datensätze, die bereits Informationen in den geänderten Feldern enthalten, ihre Werte in Echtzeit aktualisieren. Es gibt keine Warnung und kein Prüfprotokoll für die Wertänderungen, die durch Feldkonfigurationsänderungen ausgelöst werden. Alle Benutzer, die die Felder anzeigen, sehen die neuen Werte mit den Änderungen sofort.

   Die Feldinformationen werden für alle Benutzer mit Zugriff auf den Arbeitsbereich aktualisiert.

1. (Bedingt) Klicken Sie für verknüpfte Datensatzfelder auf **Suchfelder bearbeiten** und fügen Sie eines der Felder aus dem verknüpften Datensatztyp hinzu oder entfernen Sie es.

   Weitere Informationen finden Sie unter [Verbinden von Datensatztypen](/help/quicksilver/planning/architecture/connect-record-types.md).

