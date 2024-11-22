---
title: Gelöschte Datensätze wiederherstellen
description: Sie können gelöschte Datensätze aus dem kürzlich gelöschten Bereich in der Adobe Workfront-Planung wiederherstellen.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
source-git-commit: 6327e5625481ce7ff8d744bc6eb50d417cbb4413
workflow-type: tm+mt
source-wordcount: '534'
ht-degree: 1%

---


# Gelöschte Datensätze wiederherstellen

<span class="preview">Die Informationen auf dieser Seite beziehen sich auf Funktionen, die noch nicht allgemein verfügbar sind. Sie ist nur in der Vorschau -Umgebung für alle Kunden verfügbar. Nach den monatlichen Versionen für die Produktion sind in der Produktionsumgebung dieselben Funktionen auch für Kunden verfügbar, die schnelle Versionen aktiviert haben. </span>

<span class="preview">Informationen zu schnellen Versionen finden Sie unter [Schnellversionen für Ihr Unternehmen aktivieren oder deaktivieren](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md) </span>.

{{planning-important-intro}}

Sie können gelöschte Datensätze aus dem kürzlich gelöschten Bereich in der Adobe Workfront-Planung wiederherstellen.

Informationen zum Löschen von Datensätzen finden Sie unter [Datensätze löschen](/help/quicksilver/planning/records/delete-records.md).

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
   <td><p> Standard</p>
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
   <p>Systemadministratoren haben Berechtigungen für alle Arbeitsbereiche, einschließlich derjenigen, die sie nicht erstellt haben</p> </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Layout-Vorlage</p></td> 
   <td> <p>Allen Benutzern, einschließlich Workfront-Administratoren, muss eine Layoutvorlage zugewiesen werden, die den Planungsbereich im Hauptmenü enthält. </p> </td> 
  </tr> 
</tbody> 
</table>

*Weitere Informationen zu den Zugriffsanforderungen für Workfront finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Überlegungen zum Wiederherstellen gelöschter Datensätze

* Datensätze werden in der kürzlich gelöschten Klasse 30 Tage lang gespeichert. Nach 30 Tagen werden die Datensätze dauerhaft aus der Workfront-Planung gelöscht.
* Wenn die gelöschten Datensätze mit anderen Datensätzen verknüpft sind, werden die verknüpften Datensätze nicht gelöscht, aber auch die Informationen aus dem gelöschten Datensatz werden gelöscht. Durch die Wiederherstellung der gelöschten Datensätze werden die Informationen aus den verbundenen Datensätzen wiederhergestellt.
* Sie können Datensätze stapelweise wiederherstellen.
* Wenn die Datensätze gelöscht werden, werden die folgenden Informationen in der kürzlich gelöschten Klasse gespeichert:
   * **Name**: Dies sind die Informationen im Primären Feld des Datensatzes. Weitere Informationen zu Primären Datensatzfeldern finden Sie unter [Primäre Feldübersicht](/help/quicksilver/planning/fields/primary-field-overview.md).
   * **Gelöschtes Datum**: Uhrzeit und Datum des Löschens des Datensatzes.
   * **Zeit in kürzlich gelöschtem**: Die Zeit seit dem Löschen des Datensatzes. Datensätze, die mehr als 30 Tage vor dem aktuellen Datum gelöscht wurden, werden nicht in der kürzlich gelöschten Klasse angezeigt.
   * **Gelöscht von**: Der Name des Benutzers, der den Datensatz gelöscht hat.

## Gelöschte Datensätze wiederherstellen

1. Gehen Sie zur Seite mit dem Datensatztyp, auf der Sie die Datensätze gelöscht haben.
1. Klicken Sie auf das Symbol **Rückgängig** ![](assets/undo-icon.png) in der oberen rechten Ecke einer jeden Datensatztyp-Seitenansicht und klicken Sie dann auf **Kürzlich gelöscht**.

   Das Feld **Kürzlich gelöscht** wird angezeigt.

   ![](assets/recently-deleted-box.png)

1. Wählen Sie die Datensätze aus, die Sie löschen möchten, und klicken Sie dann auf **Wiederherstellen** > **Wiederherstellen**. Sie können mehrere Datensätze auswählen.

   Wenn die Wiederherstellung erfolgreich war, erhalten Sie am unteren Bildschirmrand eine Erfolgsbenachrichtigung.
1. Gehen Sie zur Tabellenansicht und überprüfen Sie die wiederhergestellten Datensätze.
