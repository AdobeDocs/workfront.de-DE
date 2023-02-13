---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '"Gruppierung: Aufgabengruppierung auf 4 Ebenen für Portfolio-Inhaber, Programmeigentümer, Projekteigentümer und Projektstatus'
description: Diese Aufgabengruppierung bietet vier Gruppierungsebenen. In diesem Fall werden Aufgaben nach Portfolio-Eigentümer, Programmeigentümer, Projekteigentümer und Projektstatus gruppiert. Die Standardschnittstelle bietet nur bis zu drei Gruppierungsebenen. Um eine vierte Ebene hinzuzufügen, müssen Sie den Textmodus verwenden. Sie können Berichte nicht nach mehr als 4 Kriterien gleichzeitig gruppieren.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: a1780a57-b94c-4d3a-b526-9bf45dba21f1
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '401'
ht-degree: 0%

---

# Gruppierung: Aufgabengruppierung auf 4 Ebenen für Portfolio-Inhaber, Programmeigentümer, Projekteigentümer und Projektstatus

Diese Aufgabengruppierung bietet vier Gruppierungsebenen. In diesem Fall werden Aufgaben nach Portfolio-Eigentümer, Programmeigentümer, Projekteigentümer und Projektstatus gruppiert. Die Standardschnittstelle bietet nur bis zu drei Gruppierungsebenen. Um eine vierte Ebene hinzuzufügen, müssen Sie den Textmodus verwenden. Sie können Berichte nicht nach mehr als 4 Kriterien gleichzeitig gruppieren.

![four_tier_grouping_for_tasks.png](assets/four-tier-grouping-for-tasks-350x239.png)

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

## Erstellen einer Aufgabengruppierung auf 4 Ebenen für Portfolio-Eigentümer, Programmeigentümer, Projekteigentümer und Projektstatus

So wenden Sie diese Gruppierung an:

1. Gehen Sie zu einer Liste von Aufgaben.
1. Aus dem **Gruppierung** Dropdown-Menü auswählen **Neue Gruppierung**.

1. Klicken **In den Textmodus wechseln**.
1. Entfernen Sie den Text im **Gruppieren Ihres Berichts** Bereich.
1. Ersetzen Sie den Text durch den folgenden Code:

   <pre>group.0.linkedname=project<br>group.0.name=Portfolio Owner<br>group.0.notime=false<br>group.0.valueField=project:portfolio:owner:name<br>group.0.valueFormat=string<br>group.1.linkedname=project<br>group.1.name=Programmeigentümer<br>group.1.notime=false<br>group.1.valueField=project:program:owner:name<br>group.1.valueFormat=string<br>group.2.linkedname=projectOwnerMM<br>group.2.listgrouingparsedmethod=nested(project).nested(owner).string(name)<br>group.2.namekey=projektownermm<br>group.2.notime=false<br>group.2.valueField=projectOwnerMM:name<br>group.2.valueFormat=string<br>group.3.enumclass=com.attask.common.constants.ProjectStatusEnum<br>group.3.linkedname=project<br>group.3.namekey=view.relatedcolumn<br>group.3.namekeyargkey.0=project<br>group.3.namekeyargkey.1=status<br>group.3.notime=false<br>group.3.valueField=project:status<br>group.3.valueFormat=val</pre>

1. Klicken **Gruppierung speichern**.
