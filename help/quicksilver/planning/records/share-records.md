---
title: Datensätze freigeben
description: Sie können Datensätze für andere freigeben, um die Zusammenarbeit zu verbessern.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 83ff53ac-f18e-4b71-bdb2-57e05d69ed29
source-git-commit: bd202821687453288c96147933331c8a7a6b3acb
workflow-type: tm+mt
source-wordcount: '516'
ht-degree: 1%

---


<!--should this move to the Access folder when we have sharing for ALL the objects???-->

# Datensätze freigeben

{{planning-important-intro}}

Um mit anderen Benutzern zusammenzuarbeiten, können Sie Datensätze für andere freigeben.

Sie können einen Adobe Workfront-Planungsdatensatz wie folgt freigeben:

* Kopieren Sie den Link der Datensatzseite aus Ihrem Browser, wenn die Seite geöffnet ist.

* Kopieren Sie einen Link auf die Datensatzseite, wenn Sie Datensätze in der Tabellenansicht des Datensatztyps anzeigen.

* Sie können alle Datensätze in einem Arbeitsbereich für andere Benutzer freigeben, indem Sie den Arbeitsbereich freigeben. Weitere Informationen finden Sie unter [Freigeben eines Arbeitsbereichs](/help/quicksilver/planning/access/share-workspaces.md).

In diesem Artikel wird beschrieben, wie Sie einen Link von der Tabellenansicht eines Datensatztyps auf die Seite eines Datensatzes kopieren können.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Workfront-Planung anzuzeigen.

Für den Zugriff auf die Workfront-Planung benötigen Sie Folgendes:

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
   <td><p> Mitwirkende, Licht oder Standard </p>
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
   <td>  <p>Anzeigen von oder höheren Berechtigungen für einen Arbeitsbereich zum Freigeben eines Datensatzes mithilfe eines Links </p>
   <p>Verwalten von Berechtigungen für einen Arbeitsbereich zum Freigeben von Datensätzen beim Freigeben des Arbeitsbereichs, zu dem der Datensatz gehört </p>
   <p>Systemadministratoren haben Berechtigungen für alle Arbeitsbereiche, einschließlich derjenigen, die sie nicht erstellt haben</p>  </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Layout-Vorlage</p></td> 
   <td> <p>Allen Benutzern, einschließlich Workfront-Administratoren, muss eine Layoutvorlage zugewiesen werden, die den Planungsbereich im Hauptmenü enthält. </p> </td> 
  </tr> 
</tbody> 
</table>

*Weitere Informationen zu den Zugriffsanforderungen für Workfront finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


<!--OLD:

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
   <td role="rowheader"><p>Adobe Workfront license</p></td>
   <td>
   <p>Any</p> 
  </td>
  </tr>
  
  <tr>
   <td role="rowheader"><p>Access level configuration</p></td>
   <td> <p>There are no access level controls for Workfront Planning</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>View or higher permissions to a workspace to share a record using a link </p>
   <p>Manage permissions to a workspace to share records while sharing the workspace the record belongs to </p>
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

-->

## Freigeben von Datensatzlinks aus der Tabellenansicht des Datensatztyps

{{step1-to-planning}}

Der zuletzt aufgerufene Arbeitsbereich wird geöffnet.
1. Klicken Sie auf eine Karte vom Typ Datensatz.

   Die Seite mit dem Datensatztyp wird geöffnet.
1. (Bedingt) Wählen Sie aus dem Dropdownmenü **Ansicht** in der oberen rechten Ecke der Tabelle eine Tabellenansicht aus. Dies sollte die Standardansicht sein, es sei denn, Sie haben den Datensatztyp in der Timeline-Ansicht angezeigt, als Sie zuletzt darauf zugegriffen haben.

   Die mit dem ausgewählten Datensatztyp verknüpften Datensätze werden in der Tabellenansicht angezeigt.
1. Rechtsklick auf eine Datensatzzeile

   Oder

   Bewegen Sie den Mauszeiger über den Namen eines Datensatzes, klicken Sie auf das Menü **Mehr** und anschließend auf **Link kopieren**.![](assets/more-menu.png)

   ![](assets/contextual-menu-for-record-row.png)

   Der Link wird in die Zwischenablage kopiert.

1. Fügen Sie den Link in ein E-Mail- oder Chat-Fenster ein, um ihn für andere Benutzer freizugeben. Wenn Benutzer den Link erhalten, wird die Datensatzseite geöffnet.

   >[!TIP]
   >
   >Die Felder auf der Datensatzseite sind dieselben Felder, die in der Tabellenansicht des Datensatzes verfügbar sind.


   <!--add there when it will be available: if they have access to this record-->

## Freigeben aller Datensätze in einem Arbeitsbereich durch Freigeben des Arbeitsbereichs

Sie können alle Datensätze in einem Arbeitsbereich freigeben, wenn Sie den Arbeitsbereich für andere freigeben.

Nur Benutzer mit Verwaltungsberechtigungen für einen Arbeitsbereich können ihn für andere freigeben.

Weitere Informationen finden Sie unter [Freigeben eines Arbeitsbereichs](/help/quicksilver/planning/access/share-workspaces.md).
