---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Gruppierung: Projektaufschlüsselung in Prozent 1'
description: In dieser benutzerdefinierten Projektgruppierung können Sie Projekte gruppiert nach einem Bereich der Werte für den abgeschlossenen Prozentsatz anzeigen.
author: Nolan
feature: Reports and Dashboards
exl-id: 7cdc8e56-3486-4e78-b494-b2ba9389c1f7
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '227'
ht-degree: 1%

---

# Gruppierung: Projektaufschlüsselung in Prozent 1

<!--Audited: 10/2024-->

In dieser benutzerdefinierten Projektgruppierung können Sie Projekte gruppiert nach einem Bereich der Werte für den abgeschlossenen Prozentsatz anzeigen. Die Aufschlüsselungen zeigen den prozentualen Abschlusswert von 25 Prozentpunktinkrementen: 0-25 %, 26-50 %, 51-75 % usw.

Mit der folgenden Gruppierung werden Projekte nach dem Wert „Prozent abgeschlossen“ in eine der folgenden Gruppierungen organisiert:

* 0%
* 1-25 %
* 26-50 %
* 51-75 %
* 76-99 %
* 100%

![percent_complete_break_custom_project_grouping_25__increments.png](assets/percent-complete-breakdown-custom-350x56.png)

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Paket</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td> 
   <p>Mitwirkender oder Anfrage zum Ändern eines Filters </p>
   <p>Standard oder Plan zum Ändern eines Berichts</p>
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriff auf Berichte, Dashboards und Kalender bearbeiten, um einen Bericht zu ändern</p> <p>Zugriff auf Filter, Ansichten, Gruppierungen bearbeiten, um einen Filter zu ändern</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Verwalten von Berechtigungen für einen Bericht</p>  </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Nach Projekt gruppieren (prozentuale Aufschlüsselung)

Um diese Gruppierung anzuwenden:

1. Zu einer Projektliste gehen.
1. Wählen Sie **Dropdown-Menü** Gruppierung“ **Neue Gruppierung** aus.

1. Klicken Sie **In Textmodus wechseln**.
1. Entfernen Sie den Text im Feld und fügen Sie den folgenden Code in den verfügbaren Bereich ein:

   ```
   group.0.linkedname=direct
   group.0.name=Percent Breakdown
   group.0.notime=false
   group.0.valueexpression=IF({percentComplete}=0,"0 %",IF({percentComplete}<=26,"0-25 %",IF({percentComplete}<=51,"26-50 %",IF({percentComplete}<=76,"51-75 %",IF({percentComplete}<100,"76-99 %","100 %")))))
   group.0.valueformat=string
   ```

1. Klicken Sie **Fertig** > **Gruppierung speichern**.
1. (Optional) Aktualisieren Sie den Namen der Gruppierung und klicken Sie dann auf **Gruppierung speichern**.
