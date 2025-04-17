---
title: Gelöschte Einträge wiederherstellen
description: Sie können gelöschte Datensätze aus dem kürzlich gelöschten Bereich in Adobe Workfront Planning wiederherstellen.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 8b6df633-eb05-4d3e-bfe6-76cedabdb76d
source-git-commit: 5a4ceb3bd7a5f121312d26775b6cf91604585775
workflow-type: tm+mt
source-wordcount: '542'
ht-degree: 1%

---

# Gelöschte Einträge wiederherstellen

<span class="preview">Die hervorgehobenen Informationen auf dieser Seite beziehen sich auf Funktionen, die noch nicht allgemein verfügbar sind. Sie ist nur in der Vorschau -Umgebung für alle Kunden verfügbar. Nach den monatlichen Releases in der Produktion stehen dieselben Funktionen auch in der Produktionsumgebung für Kunden zur Verfügung, die schnelle Releases aktiviert haben. </span>

<span class="preview">Informationen zu Schnellversionen finden Sie unter [Aktivieren oder Deaktivieren von Schnellversionen für Ihre Organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

Sie können gelöschte Datensätze aus dem kürzlich gelöschten Bereich in Adobe Workfront Planning wiederherstellen.

Informationen zum Löschen von Datensätzen finden Sie unter [Löschen von Datensätzen](/help/quicksilver/planning/records/delete-records.md).

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
   <td><p> Standard</p>
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
   <td>   <p>Mitwirken an oder höhere Berechtigungen für einen Arbeitsbereich <span class="preview">und einen Datensatztyp</span> </a> </p>  
   <p>Systemadministratoren haben Berechtigungen für alle Arbeitsbereiche, einschließlich der nicht erstellten</p> </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Layout-Vorlage</p></td> 
   <td> <p>Allen Benutzern, einschließlich Workfront-Administratoren, muss eine Layoutvorlage zugewiesen werden, die den Bereich Planung im Hauptmenü enthält. </p> </td> 
  </tr> 
</tbody> 
</table>

*Weitere Informationen zu Zugriffsanforderungen für Workfront finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Überlegungen zum Wiederherstellen gelöschter Datensätze

* Datensätze werden 30 Tage lang im kürzlich gelöschten Bin gespeichert. Nach 30 Tagen werden die Datensätze dauerhaft aus Workfront Planning gelöscht.
* Wenn die gelöschten Datensätze mit anderen Datensätzen verknüpft sind, werden die verknüpften Datensätze nicht gelöscht, aber die Informationen aus dem gelöschten Datensatz werden ebenfalls gelöscht. Beim Wiederherstellen der gelöschten Datensätze werden die Informationen aus den verbundenen Datensätzen wiederhergestellt.
* Sie können Einträge stapelweise wiederherstellen.
* Wenn die Datensätze gelöscht werden, werden die folgenden Informationen im zuletzt gelöschten Bin gespeichert:
   * **Name**: Dies sind die Informationen im Primären Feld des Datensatzes. Weitere Informationen zu Primären Datensatzfeldern finden Sie unter Übersicht über Primäre Felder [](/help/quicksilver/planning/fields/primary-field-overview.md).
   * **Löschdatum**: Uhrzeit und Datum, an dem der Datensatz gelöscht wurde.
   * **Zeit in kürzlich gelöschten**: Die Zeit seit dem Löschen des Datensatzes. Datensätze, die mehr als 30 Tage vor dem aktuellen Datum gelöscht wurden, werden nicht im kürzlich gelöschten Bin angezeigt.
   * **Gelöscht von**: Der Name des Benutzers, der den Datensatz gelöscht hat.

## Gelöschte Einträge wiederherstellen

1. Navigieren Sie zur Seite „Datensatztyp“, auf der Sie Datensätze gelöscht haben.
1. Klicken Sie auf **Rückgängig**-Symbol ![Rückgängig](assets/undo-icon.png) in der oberen rechten Ecke einer beliebigen Seitenansicht des Datensatztyps und dann auf **Zuletzt gelöscht**.

   Das Feld **Kürzlich gelöscht** wird angezeigt.

   ![Kürzlich gelöschtes Feld](assets/recently-deleted-box.png)

1. Wählen Sie die zu löschenden Datensätze aus und klicken Sie dann auf **Wiederherstellen** > **Wiederherstellen**. Sie können mehrere Datensätze auswählen.

   Wenn die Wiederherstellung erfolgreich war, erhalten Sie eine Erfolgsbenachrichtigung am unteren Bildschirmrand.
1. Wechseln Sie zur Tabellenansicht und überprüfen Sie die wiederhergestellten Datensätze.
