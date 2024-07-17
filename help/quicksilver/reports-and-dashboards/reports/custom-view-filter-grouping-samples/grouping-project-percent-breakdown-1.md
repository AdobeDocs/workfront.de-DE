---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: "Gruppierung: Projektprozentuale Aufschlüsselung 1"
description: Bei dieser benutzerdefinierten Projektgruppierung können Sie Projekte anzeigen, die nach einem Bereich ihrer vollständigen Prozentwerte gruppiert sind.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 7cdc8e56-3486-4e78-b494-b2ba9389c1f7
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '280'
ht-degree: 1%

---

# Gruppierung: Projekt-Prozentverteilung 1

Bei dieser benutzerdefinierten Projektgruppierung können Sie Projekte anzeigen, die nach einem Bereich ihrer vollständigen Prozentwerte gruppiert sind.

Die folgende Gruppierung organisiert Projekte nach dem vollständigen Prozentwert in einer dieser Gruppierungen:

* 0%
* 1-25 %
* 26-50 %
* 51-75%
* 76-99%
* 100%

![percent_complete_break_custom_project_grouping_25_inkrements.png](assets/percent-complete-breakdown-custom-350x56.png)

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Anforderung zur Änderung einer Gruppierung </p>
   <p>Berichtänderung planen</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf Berichte, Dashboards und Kalender bearbeiten, um einen Bericht zu ändern</p> <p>Zugriff auf Filter, Ansichten und Gruppierungen bearbeiten, um eine Gruppierung zu ändern</p> <p><b>NOTIZ</b>

Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td>
</tr>  
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Berechtigungen für einen Bericht verwalten</p> <p>Weitere Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Anfordern des Zugriffs auf Objekte </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Verteilung nach Projekt in Prozent

So wenden Sie diese Gruppierung an:

1. Gehen Sie zu einer Projektliste.
1. Wählen Sie aus dem Dropdownmenü **Gruppierung** die Option **Neue Gruppierung** aus.

1. Klicken Sie auf **Wechseln zum Textmodus**.
1. Entfernen Sie den Text in das Feld und fügen Sie den folgenden Code in den verfügbaren Bereich ein:
   <pre>group.0.linkedname=direct<br>group.0.name=Percent Breakdown<br>group.0.notime=false<br>group.0.valueExpression=IF({percentComplete}=0,"0 %",IF({percentComplete}&lt;=26,"0-25 %",IF({percentComplete}&lt;=51,"25-50 %",({percentComplete}&lt;=76,"50-75 %",IF({percentComplete}&lt;100,"75-99 %","100 %")))<br>group.0.valueFormat=string</pre>

1. Klicken Sie auf **Gruppierung speichern**.
