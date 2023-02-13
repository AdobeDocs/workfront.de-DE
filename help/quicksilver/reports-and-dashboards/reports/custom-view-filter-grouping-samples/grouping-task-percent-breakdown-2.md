---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '"Gruppierung: Aufschlüsselung nach Aufgabenprozentsatz 2'
description: '''In dieser benutzerdefinierten Aufgabengruppierung können Sie Aufgaben anzeigen, die nach einem Bereich ihrer vollständigen Prozentwerte gruppiert sind. Die Aufschlüsselungen zeigen den vollständigen prozentualen Wert von 10 Prozentpunktinkrementen an: 1-10 %, 11-20 % usw."'
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 7d5a40dd-d451-48c7-9323-af52aa387709
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '289'
ht-degree: 4%

---

# Gruppierung: Aufschlüsselung nach Aufgabenprozentsatz 2

Bei dieser benutzerdefinierten Aufgabengruppierung können Sie Aufgaben anzeigen, die nach einem Bereich der vollständigen Prozentwerte gruppiert sind. Die Aufschlüsselungen zeigen den vollständigen prozentualen Wert von 10 Prozentpunktinkrementen an: 1-10 %, 11-20 % usw.

Die folgende Gruppierung organisiert Projekte nach dem vollständigen Prozentwert in einer dieser Gruppierungen:

* 0%
* 1 - 10%
* 11-20%
* 21-30%
* 31-40%
* 41-50%
* 51-60%
* 61-70%
* 71-80%
* 81-90%
* 91-99%
* 100%

![task_10_Aufschlüsselung_grouping.png](assets/task-10--breakdown-grouping-350x547.png)

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf Berichte, Dashboards und Kalender bearbeiten</p> <p>Zugriff auf Filter, Ansichten, Gruppierungen bearbeiten</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Berechtigungen für einen Bericht verwalten</p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Aufschlüsselung nach Aufgabenprozentsatz nach Gruppe

So wenden Sie diese Gruppierung an:

1. Gehen Sie zu einer Liste von Aufgaben.
1. Aus dem **Gruppierung** Dropdown-Menü auswählen **Neue Gruppierung**.

1. Klicken **In den Textmodus wechseln**.
1. Entfernen Sie den Text im **Gruppieren Ihres Berichts** Bereich.
1. Ersetzen Sie den Text durch den folgenden Code:

   <pre>group.0.linkedname=direct<br>group.0.name=Prozentuale Aufschlüsselung<br>group.0.notime=false<br>group.0.valueExpression=IF({percentComplete}=0,"0 %",IF({percentComplete}&lt;=11,"1-10 %",IF({percentComplete}&lt;=21,"11-20 %",IF({percentComplete}&lt;=31,"21-30 %",IF({percentComplete}&lt;41,"31-40 %",IF({percentComplete}&lt;51,"41-50 %",IF({percentComplete}&lt;61,"51-60 %",IF({percentComplete}&lt;71,"61-70 %",IF({percentComplete}&lt;81,"7 1-80 %",IF({percentComplete}&lt;91,"81-90 %",IF({percentComplete}&lt;100,"91-99 %","100 %")))))))))<br>textmode=true</pre>

1. Klicken **Gruppierung speichern**.
