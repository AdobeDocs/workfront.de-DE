---
title: Ideenraum mit anderen teilen
description: Adobe Workfront Planning bietet jetzt eine zusätzliche Funktion, mit der Sie Ideen ausarbeiten können, bevor Sie Ihre Kampagnen starten. Nutzen Sie die Leistungsfähigkeit von KI, um Ideen zu erstellen und mit anderen zusammenzuarbeiten, bevor sie zu Planungsdatensätzen werden.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
source-git-commit: 02ea2cad43b1064e30a7356feaa194f98d448092
workflow-type: tm+mt
source-wordcount: '607'
ht-degree: 4%

---


# Ideenraum mit anderen teilen

<!--add to TOC and miniTOC-->

<span class="preview">Die Informationen auf dieser Seite beziehen sich auf Funktionen, die noch nicht allgemein verfügbar sind. Es ist nur im Rahmen des Programms **Ideation Space Beta** verfügbar. </span>

<span class="preview">Weitere Informationen finden Sie unter [Erste Schritte mit dem Ideenraum für Adobe Workfront Planning](/help/quicksilver/planning/ideation/get-started-with-planning-ideation.md).</span>

{{planning-important-intro}}

<!--ome of this information is also duplicated in the section for Ideation space permissions in the Access needed to use Ideation space article-->

Workfront Planning-Datensatzberechtigungen werden in den Ideenraum eines Datensatzes übertragen.

Darüber hinaus können Sie anderen Benutzern die Berechtigung erteilen, den Ideenraum zu verwenden und ihm Ideen hinzuzufügen.

Beachten Sie Folgendes:

* Die Ersteller von Ideen haben immer Editor-Berechtigungen für ihre eigenen Ideen.

* Sie müssen über Editor-Berechtigungen für einen Ideenraum verfügen, um Briefs zu erstellen und sie in andere Programme zu exportieren.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktion in diesem Artikel anzuzeigen. 

<!--
are there additional license restrictions or packages to be purchased to have access to Ideation space?? If yes, update the table below
-->

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
</tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront-Paket</p></td> 
   <td> 
<ul> 
<li><p>Beliebige Workfront oder Workflows mit einem Planungspaket</p></li>
ODER
<li><p>Jedes Planungspaket, wenn es als eigenständiges Produkt gekauft wird</p></li></ul>
   </td>

<tr> 
   <td role="rowheader"><p>Zusätzliche Produkte</p></td> 
   <td><ul>
   <li><p>Adobe GenStudio for Performance Marketing</p></li>
   <!--
   <li><p>Adobe Customer Journey Analytics</p></li>
   -->
   </ul>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workflow-Lizenz</p></td> 
   <td><p>Standard</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Adobe Planning-Lizenz</p></td> 
   <td><p>Standard</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Konfiguration der Zugriffsebene</p></td> 
   <td> 
   <ul>
   <li><p>Sie müssen der Zugriffsebene sowohl einen Workflow- als auch einen Planning-Lizenztyp hinzufügen, wenn Sie sowohl einen Workflow als auch ein Planning-Paket haben</p>   </li>
   <li><p>Die Einstellung Ideenraum deaktivieren in Ihrer Zugriffsebene muss deaktiviert sein</p></li>
</td> 
  </tr>  
   <tr> 
   <td role="rowheader"><p>Objektberechtigungen</p></td> 
   <td> <p>Tragen Sie Berechtigungen oder höhere Berechtigungen zum Arbeitsbereich und Datensatztyp bei, dem Sie Datensätze hinzufügen möchten </p>
      <p>Systemadministratoren haben Berechtigungen für alle Arbeitsbereiche, einschließlich der nicht erstellten</p>
      <p>Anzeigen von Berechtigungen für Workfront-Objekte, um sie zu Briefs hinzuzufügen <!--not sure if this is available--></p>
      <p>Editor-Berechtigungen für den Ideenraum zum Erstellen von Briefs</p>
   </td> 
  </tr>  
   <tr> 
   <td role="rowheader"><p>Adobe GenStudio for Performance Marketing-Benutzerrollen</p></td> 
   <td><p><ul><li>Jede GenStudio-Benutzerrolle für den Zugriff auf Kampagnen, Produkte und Personas</li>
   <li>GenStudio System Manager für den Zugriff auf Aktivierungen <!--and Events--></li></ul>
   Weitere Informationen finden Sie unter <a href="https://experienceleague.adobe.com/de/docs/genstudio-for-performance-marketing/user-guide/intro/user-roles">Benutzerrollen und -berechtigungen</a>. 
   </p>
  </td> 
  </tr> 
</tbody> 
</table>

Weitere Informationen zu Zugriffsanforderungen für Workfront finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++  

## Ideenraum teilen

1. Zugriff auf den Ideenraum eines Planungsdatensatzes.

   Weitere Informationen finden Sie in einem der folgenden Artikel:

   * [Erstellen von Planungsdatensätzen aus Ideation Space Briefs](/help/quicksilver/planning/ideation/create-records-in-ideation-space-for-planning.md)
   * [Erstellen von Briefs im Ideationsbereich](/help/quicksilver/planning/ideation/create-briefs-in-ideation-space.md)

1. Klicken **oben rechts auf** Freigeben“ und dann auf das Symbol **Einstellungen** ![Einstellungen](assets/setting-icon.png) in der oberen rechten Ecke des Felds **Dokument freigeben**.
1. Wählen Sie in der Liste „Wer hat Zugriff“ eine der folgenden Optionen aus:

   * **Nur eingeladene Personen können darauf zugreifen**

     Sie müssen einzelne Benutzer zum Ideationsbereich hinzufügen und ihnen eine Berechtigungsstufe zuweisen.
   * **Jeder unter &lt; Workfront-Umgebung Ihres Unternehmens > kann einen Kommentar abgeben**

     Jeder Benutzer in Ihrem Unternehmen, der über einen Workflow und eine Planungslizenz auf der Zugriffsebene verfügt, kann die Idee finden und kommentieren.
   * **Jeder mit dem Link kann einen Kommentar abgeben**

     Jeder, den Sie über einen Link auf die Idee informieren, kann diese kommentieren, auch externe Personen in Ihrem Unternehmen.

1. Klicken Sie **Link kopieren**, um einen Link zu der Idee zu erstellen und sie für andere freizugeben. Der Link wird der Zwischenablage hinzugefügt.
1. Klicken Sie im Feld Einstellungen auf den Pfeil nach hinten, um zur Freigabe zurückzukehren.
1. (Bedingt) Wenn Sie den Ideenraum für bestimmte Personen freigeben möchten, geben Sie zunächst deren Namen oder E-Mail-Adresse ein und wählen Sie dann eine der folgenden Berechtigungsebenen aus:

   | Ideationsraum-Berechtigung | Funktionen |
   |---|---|
   | **Editor** | Kann den Ideenraum bearbeiten, herunterladen und freigeben |
   | **Kommentator** | Kann den Ideenraum anzeigen und kommentieren |
   | **Viewer** | Kann den Ideenraum anzeigen |

1. (Optional) Fügen Sie Ihrer Zuweisung eine Nachricht hinzu und klicken Sie dann auf **Einladen**.

   Die eingeladenen Benutzer erhalten eine E-Mail-Benachrichtigung über ihre Berechtigungszuweisung.

1. Klicken Sie auf das **X**-Symbol, um das Feld **Dokument freigeben** zu schließen.











