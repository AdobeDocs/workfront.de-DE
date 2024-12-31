---
title: Importieren von Feldern aus Adobe Workfront
description: In Adobe Workfront Planning können Sie benutzerdefinierte Felder für jede Art von Datensatztyp erstellen. Anschließend können Sie das Feld mit Workfront Planning-Datensätzen verknüpfen.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 994594f2-a888-423a-bf66-0d14baf57c55
source-git-commit: 8425f8be7d30d36986ac1c062603e680c69902c6
workflow-type: tm+mt
source-wordcount: '760'
ht-degree: 6%

---

<!--add to TOC-->

# Importieren von Feldern aus Adobe Workfront

<span class="preview">Die Informationen auf dieser Seite beziehen sich auf Funktionen, die noch nicht allgemein verfügbar sind. Sie ist nur in der Vorschau -Umgebung für alle Kunden verfügbar. Nach den monatlichen Releases in der Produktion stehen dieselben Funktionen auch in der Produktionsumgebung für Kunden zur Verfügung, die schnelle Releases aktiviert haben. </span>

<span class="preview">Informationen zu Schnellversionen finden Sie unter [Aktivieren oder Deaktivieren von Schnellversionen für Ihre Organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>


{{planning-important-intro}}

Sie können Kopien bestehender Workfront-Felder importieren. Beim Importieren von Feldern aus Workfront wird von jedem Feld eine Kopie für einen Workfront Planning-Datensatztyp erstellt.


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
   <td>   <p>Verwalten von Berechtigungen für einen Arbeitsbereich</a> </p>  
   <p>Systemadministratoren haben Berechtigungen für alle Arbeitsbereiche, einschließlich der nicht erstellten.</p> </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Layoutvorlage</p></td> 
   <td> <p>Allen Benutzern, einschließlich Workfront-Administratoren, muss eine Layoutvorlage zugewiesen werden, die den Bereich Planung im Hauptmenü enthält. </p> </td> 
  </tr> 
</tbody> 
</table>

*Weitere Informationen zu Zugriffsanforderungen für Workfront finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Überlegungen zum Importieren von Feldern aus Workfront

* In Workfront Planning können Sie native oder benutzerdefinierte Workfront-Felder in einen Datensatztyp importieren.
* Beim Importieren von Workfront-Feldern werden Kopien derselben Felder erstellt und der Feldname wird in Workfront Planning beibehalten. Nachdem sie in Workfront Planning kopiert wurden, sind die Felder von den Workfront-Originalfeldern unabhängig und geben keine Informationen weiter.
<!--check this: * You do not need permissions or access to Workfront objects to be able to add their fields to Workfront Planning. -->
* Sie können native oder benutzerdefinierte Felder aus den folgenden Workfront-Objekten hinzufügen:
   * Portfolio
   * Programm
   * Projekt
   * Aufgabe
   * Problem
   * Dokument
   * Firma
   * Gruppe
   * Benutzerin oder Benutzer
   * Aufgabengebiet
   * Zuweisung
   * Stunde
   * Abrechnungseintrag
     <!--Available only to Preview, but might not come to Prod:* Rate card-->
   * Ausgabe
   * Wiederholung
     <!--* Non-labor resource-->
     <!--* Non-labour resource category-->
* Workfront-Felder behalten ihren Feldtyp möglicherweise nicht bei, nachdem sie in Workfront Planning importiert wurden.

  Die nachstehende Tabelle zeigt die Workfront-Feldtypen und den entsprechenden Workfront Planning-Feldtyp.

  | Workfront-Feldtyp | Workfront Planning-Feldtyp |
  |------------------------------------------|-------------------------------|
  | Textformatierter einzeiliger Text | Einzeiliger Text |
  | Zahlenformatierter einzeiliger Text | Zahl |
  | Währungsformatierter einzeiliger Text | Währung |
  | Absatz | Absatz |
  | Text mit Formatierung | Absatz |
  | Einfachauswahl-Dropdown | Einzelauswahl |
  | Mehrfachauswahl-Dropdown | Mehrfachauswahl |
  | Filter mit automatischer Textvervollständigung werden nicht unterstützt | Personen |
  | Berechnet* | Formel |
  | Datum | Datum |
  | Kontrollkästchen-Gruppe | Mehrfachauswahl |
  | Optionsfeld | Mehrfachauswahl |

  *Berechnete Felder stehen zu einem späteren Zeitpunkt zur Verfügung.
Alle anderen Workfront-Feldtypen werden in Workfront Planning nicht unterstützt.


## Felder aus Workfront importieren

<!--the first 3 steps are the same as in Create fields-->

{{step1-to-planning}}

1. Klicken Sie auf den Arbeitsbereich, für dessen Datensatztypen Sie Felder erstellen möchten.

   Der Arbeitsbereich wird geöffnet und die Datensatztypen werden angezeigt.

1. Klicken Sie auf die Karte eines Datensatztyps.

   Alle vorhandenen Datensätze, die mit dem Datensatztyp verknüpft sind, werden in den Zeilen der Tabellenansicht angezeigt.

   >[!TIP]
   >
   >    Einige Felder sind möglicherweise ausgeblendet. Klicken Sie **Felder** und aktivieren Sie den Umschalter für die Felder, die als Spalten in der Tabellenansicht angezeigt werden sollen.

1. Klicken Sie oben rechts in der Tabellenansicht auf das Symbol **+** .

   Oder

   Bewegen Sie den Mauszeiger über die Kopfzeile einer Spalte, klicken Sie auf den nach unten zeigenden Pfeil nach dem Feldnamen und klicken Sie dann auf **Links einfügen** oder **Rechts einfügen** um das neue Feld hinzuzufügen.
1. Klicken Sie **Vorhandenes** hinzufügen“ in der rechten unteren Ecke der Registerkarte **Neues Feld**. <!--check UI - did they change this??-->

   ![](assets/add-existing-fields-from-workfront-modal.png)

1. Beginnen Sie mit der Eingabe des Namens eines bestehenden Workfront-Felds in den Suchbereich und klicken Sie dann auf **+**, wenn es in der Liste angezeigt wird.
1. (Optional) Geben Sie ein anderes Feld ein und klicken Sie dann auf **+**, wenn es in der Liste angezeigt wird.
1. (Optional) Klicken Sie auf **Filter**-Symbol ![](assets/filters-in-import-fields-icon.png) und aktualisieren Sie dann eines oder beide der folgenden Felder:

   * Objekttyp: Wählen Sie einen Workfront-Objekttyp aus, dessen Felder Sie importieren möchten.
   * Benutzerdefiniertes Formular: Wählen Sie ein oder mehrere benutzerdefinierte Formulare in Workfront aus. Sie können ein benutzerdefiniertes Formular auswählen, ohne zuerst einen Objekttyp auszuwählen.
1. Klicken Sie auf **+** und dann auf **Felder hinzufügen**.
Die Felder werden der Tabellenansicht und den Detailseiten der Datensätze hinzugefügt.

   >[!IMPORTANT]
   >
   >    Für jeden Datensatztyp sind maximal 500 Felder zulässig. Die vorhandenen Felder zusammen mit den importierten Feldern tragen zu dieser Beschränkung bei.

   Die hinzugefügten Felder sind Kopien der Workfront-Felder und stellen keine Verbindung mehr zu den Originalfeldern in Workfront her.