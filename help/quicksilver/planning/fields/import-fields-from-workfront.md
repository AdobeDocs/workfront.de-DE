---
title: Importieren von Feldern aus Adobe Workfront
description: In der Adobe Workfront-Planung können Sie benutzerdefinierte Felder für jeden Datensatztyp erstellen. Anschließend können Sie das Feld mit Workfront-Planungsdatensätzen verknüpfen.
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

<span class="preview">Die Informationen auf dieser Seite beziehen sich auf Funktionen, die noch nicht allgemein verfügbar sind. Sie ist nur in der Vorschau -Umgebung für alle Kunden verfügbar. Nach den monatlichen Versionen für die Produktion sind in der Produktionsumgebung dieselben Funktionen auch für Kunden verfügbar, die schnelle Versionen aktiviert haben. </span>

<span class="preview">Informationen zu schnellen Versionen finden Sie unter [Schnellversionen für Ihr Unternehmen aktivieren oder deaktivieren](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md) </span>.


{{planning-important-intro}}

Sie können Kopien vorhandener Workfront-Felder importieren. Beim Importieren von Feldern aus Workfront wird eine Kopie jedes Felds für den Datensatztyp Workfront Planning erstellt.


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
   <p>Systemadministratoren haben Berechtigungen für alle Arbeitsbereiche, einschließlich der Arbeitsbereiche, die sie nicht erstellt haben.</p> </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Layout-Vorlage</p></td> 
   <td> <p>Allen Benutzern, einschließlich Workfront-Administratoren, muss eine Layoutvorlage zugewiesen werden, die den Planungsbereich im Hauptmenü enthält. </p> </td> 
  </tr> 
</tbody> 
</table>

*Weitere Informationen zu den Zugriffsanforderungen für Workfront finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Überlegungen zum Importieren von Feldern aus Workfront

* Sie können native oder benutzerdefinierte Workfront-Felder in einen Datensatztyp in der Workfront-Planung importieren.
* Beim Importieren von Workfront-Feldern werden Kopien derselben Felder erstellt und der Feldname wird in der Workfront-Planung beibehalten. Nachdem sie in die Workfront-Planung kopiert wurden, sind die Felder unabhängig von den ursprünglichen Workfront-Feldern und sie geben keine Informationen frei.
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
* Workfront-Felder behalten möglicherweise ihren Feldtyp nicht bei, nachdem sie in der Workfront-Planung importiert wurden.

  Die nachstehende Tabelle zeigt die Workfront-Feldtypen und den entsprechenden Feldtyp für die Workfront-Planung.

  | Workfront-Feldtyp | Workfront-Planungstyp |
  |------------------------------------------|-------------------------------|
  | Textformatierter Einzelzeilentext | Einzeiliger Text |
  | Zahlenformatierter einzeiliger Text | Zahl |
  | Währungsformatierter einzeiliger Text | Währung |
  | Absatz | Absatz |
  | Text mit Formatierung | Absatz |
  | Einfachauswahl-Dropdown | Einzelauswahl |
  | Mehrfachauswahl-Dropdown | Mehrfachauswahl |
  | Benutzertypisierungsfilter werden nicht unterstützt | Personen |
  | Berechnet* | Formel |
  | Datum | Datum |
  | Kontrollkästchen-Gruppe | Mehrfachauswahl |
  | Optionsfeld | Mehrfachauswahl |

  *Berechnete Felder stehen zu einem späteren Zeitpunkt zur Verfügung.
Alle anderen Workfront-Feldtypen werden in der Workfront-Planung nicht unterstützt.


## Felder aus Workfront importieren

<!--the first 3 steps are the same as in Create fields-->

{{step1-to-planning}}

1. Klicken Sie auf den Arbeitsbereich, dessen Datensatztypen Sie Felder erstellen möchten.

   Der Arbeitsbereich wird geöffnet und die Datensatztypen werden angezeigt.

1. Klicken Sie auf die Karte eines Datensatztyps.

   Alle vorhandenen Datensätze, die mit dem Datensatztyp verknüpft sind, werden in den Zeilen der Tabellenansicht angezeigt.

   >[!TIP]
   >
   >    Einige Felder sind möglicherweise ausgeblendet. Klicken Sie auf **Felder** und aktivieren Sie den Umschalter für die Felder, die Sie in der Tabellenansicht als Spalten anzeigen möchten.

1. Klicken Sie oben rechts in der Tabellenansicht auf das Symbol **+** .

   Oder

   Bewegen Sie den Mauszeiger über die Kopfzeile einer Spalte, klicken Sie auf den nach unten zeigenden Pfeil nach dem Feldnamen und klicken Sie dann auf **Links einfügen** oder **Rechts einfügen** , um das neue Feld hinzuzufügen.
1. Klicken Sie in der rechten unteren Ecke der Registerkarte **Neues Feld** auf **Vorhandenes hinzufügen** . <!--check UI - did they change this??-->

   ![](assets/add-existing-fields-from-workfront-modal.png)

1. Geben Sie den Namen eines vorhandenen Workfront-Felds im Suchbereich ein und klicken Sie dann auf **+** , wenn es in der Liste angezeigt wird.
1. (Optional) Geben Sie ein weiteres Feld ein und klicken Sie dann auf **+** , wenn es in der Liste angezeigt wird.
1. (Optional) Klicken Sie auf das Symbol **Filter** ![](assets/filters-in-import-fields-icon.png) und aktualisieren Sie dann eines oder beide der folgenden Felder:

   * Objekttyp: Wählen Sie einen Workfront-Objekttyp aus, dessen Felder Sie importieren möchten.
   * Benutzerdefiniertes Formular: Wählen Sie ein oder mehrere benutzerdefinierte Formulare aus Workfront aus. Sie können ein benutzerdefiniertes Formular auswählen, ohne zuerst einen Objekttyp auszuwählen.
1. Klicken Sie auf **+** und dann auf **Felder hinzufügen**.
Die Felder werden der Tabellenansicht und den Detailseiten der Datensätze hinzugefügt.

   >[!IMPORTANT]
   >
   >    Für jeden Datensatztyp sind maximal 500 Felder zulässig. Die vorhandenen Felder sowie die importierten Felder tragen zu dieser Begrenzung bei.

   Die hinzugefügten Felder sind Kopien der Workfront-Felder und stellen keine Verbindung mehr zu den ursprünglichen Feldern in Workfront her.