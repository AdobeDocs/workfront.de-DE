---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: "Gruppierung: Aufschlüsselung nach Aufgabenprozentsatz 2"
description: '''In dieser benutzerdefinierten Aufgabengruppierung können Sie Aufgaben anzeigen, die nach einem Bereich ihrer vollständigen Prozentwerte gruppiert sind. Die Aufschlüsselungen zeigen den vollständigen Prozentwert von 10 Prozentpunkten (1-10 %, 11-20 % usw.) an."'
author: Nolan
feature: Reports and Dashboards
exl-id: 7d5a40dd-d451-48c7-9323-af52aa387709
source-git-commit: a6874c3a2dfda02b8a25f78056767d8c59c888e9
workflow-type: tm+mt
source-wordcount: '268'
ht-degree: 0%

---

# Gruppierung: Aufschlüsselung nach Aufgabenprozentsatz 2

<!--Audited: 10/2024-->

Bei dieser benutzerdefinierten Aufgabengruppierung können Sie Aufgaben anzeigen, die nach einem Bereich der vollständigen Prozentwerte gruppiert sind. Die Aufschlüsselungen zeigen den vollständigen Prozentwert von 10 Prozentpunkten (1-10 %, 11-20 % usw.).

Die folgende Gruppierung organisiert Projekte nach dem vollständigen Prozentwert in einer dieser Gruppierungen:

* 0%
* 1-10 %
* 11-20 %
* 21-30 %
* 31-40 %
* 41-50%
* 51-60 %
* 61-70 %
* 71-80 %
* 81-90%
* 91-99%
* 100%

![task_10__failure_grouping.png](assets/task-10--breakdown-grouping-350x547.png)

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Abo</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> 
    <p>Neu:</p>
   <ul><li><p>Mitwirkende bei der Änderung eines Filters </p></li>
   <li><p>Standard zum Ändern eines Berichts</p></li> </ul>

<p>Aktuell:</p>
   <ul><li><p>Filteranforderung </p></li>
   <li><p>Berichtänderung planen</p></li> </ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Zugriff auf Berichte, Dashboards und Kalender bearbeiten, um einen Bericht zu ändern</p> <p>Zugriff auf Filter, Ansichten und Gruppierungen bearbeiten, um einen Filter zu ändern</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Berechtigungen für einen Bericht verwalten</p>  </td> 
  </tr> 
 </tbody> 
</table>

*Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Aufschlüsselung nach Aufgabenprozentsatz

So wenden Sie diese Gruppierung an:

1. Gehen Sie zu einer Liste von Aufgaben.
1. Wählen Sie aus dem Dropdownmenü **Gruppierung** die Option **Neue Gruppierung** aus.
1. Klicken Sie auf **Gruppierung hinzufügen**.

1. Klicken Sie auf **Wechseln zum Textmodus**.
1. Entfernen Sie den Text im Bereich **Gruppieren nach** .
1. Ersetzen Sie den Text durch den folgenden Code:

   ```
   group.0.linkedname=direct
   group.0.name=Percent Breakdown
   group.0.notime=false
   group.0.valueexpression=IF({percentComplete}=0,"0 %",IF({percentComplete}<=11,"1-10 %",IF({percentComplete}<=21,"11-20 %",IF({percentComplete}<=31,"21-30 %",IF({percentComplete}<41,"31-40 %",IF({percentComplete}<51,"41-50 %",IF({percentComplete}<61,"51-60 %",IF({percentComplete}<71,"61-70 %",IF({percentComplete}<81,"71-80 %",IF({percentComplete}<91,"81-90 %",IF({percentComplete}<100,"91-99 %","100 %")))))))))))
   textmode=true
   ```

1. Klicken Sie auf **Fertig** > **Gruppierung speichern**.
1. (Optional) Aktualisieren Sie den Gruppierungsnamen und klicken Sie dann auf **Gruppierung speichern**.
