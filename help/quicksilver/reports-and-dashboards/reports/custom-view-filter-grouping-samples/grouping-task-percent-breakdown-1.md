---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '"Gruppierung: Aufschlüsselung nach Aufgabenprozentsatz 1'
description: '''In dieser benutzerdefinierten Projektgruppierung können Sie Projekte anzeigen, die nach einem Bereich ihrer vollständigen Prozentwerte gruppiert sind. Die Aufschlüsselungen zeigen den vollständigen prozentualen Wert von 25 Prozentpunktinkrementen an: 0-25 %, 25-50 % usw."'
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: ddb9496c-9347-4dc9-a4ce-b9017abd0bb2
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '270'
ht-degree: 2%

---

# Gruppierung: Aufschlüsselung nach Aufgabenprozentsatz 1

Bei dieser benutzerdefinierten Projektgruppierung können Sie Projekte anzeigen, die nach einem Bereich ihrer vollständigen Prozentwerte gruppiert sind. Die Aufschlüsselungen zeigen den vollständigen prozentualen Wert von 25 Prozentpunktinkrementen an: 0-25 %, 25-50 % usw. 

Die folgende Gruppierung gliedert Aufgaben nach dem vollständigen Prozentwert in 6 verschiedene Gruppierungen:

* 0%
* 1-25%
* 26-50%
* 51-75%
* 76-99%
* 100%

![task_25_Aufschlüsselung_grouping.png](assets/task-25--breakdown-grouping-350x412.png)

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

   <pre>group.0.linkedname=direct<br>group.0.name=Prozentuale Aufschlüsselung<br>group.0.notime=false<br>group.0.valueExpression=IF({percentComplete}=0,"0 %",IF({percentComplete}&lt;=26,"0-25 %",IF({percentComplete}&lt;=51,"25-50 %",IF({percentComplete}&lt;=76,"50-75 %",IF({percentComplete}&lt;100,"75-99 %","100 %"))))<br>group.0.valueFormat=string</pre>

1. Klicken **Gruppierung speichern**.
