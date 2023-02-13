---
content-type: overview
product-area: reporting;dashboards
navigation-topic: report-usage
title: So organisieren Sie Berichte in einem Dashboard
description: Sie können sehen, ob einem Dashboard in Adobe Workfront ein Bericht hinzugefügt wird. Dies kann bei der Entscheidung nützlich sein, welche Berichte Sie beibehalten und welche aus dem System gelöscht werden können. Wenn sich Berichte in Dashboards befinden, verlassen sich Benutzer möglicherweise weiterhin auf sie. Es wird empfohlen, keine Berichte zu löschen, die in von Benutzern verwendeten Dashboards aufgeführt sind. Weitere Informationen zum Hinzufügen von Berichten zu Dashboards finden Sie im Artikel Bericht zu einem Dashboard hinzufügen .
author: Nolan
feature: Reports and Dashboards
exl-id: ce00c307-9e64-49f5-997b-f7fc461c960c
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '621'
ht-degree: 0%

---

# So organisieren Sie Berichte in einem Dashboard

## Zugriff auf Dashboard-Informationen in einer Berichtsliste

Sie können sehen, ob einem Dashboard in Adobe Workfront ein Bericht hinzugefügt wird. Dies kann bei der Entscheidung nützlich sein, welche Berichte Sie beibehalten und welche aus dem System gelöscht werden können. Wenn sich Berichte in Dashboards befinden, verlassen sich Benutzer möglicherweise weiterhin auf sie. Es wird empfohlen, keine Berichte zu löschen, die in von Benutzern verwendeten Dashboards aufgeführt sind.\
Weitere Informationen zum Hinzufügen von Berichten zu Dashboards finden Sie im Artikel [Einen Bericht zu einem Dashboard hinzufügen](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/add-report-dashboard.md).

Sie können sehen, ob einem Dashboard ein Bericht hinzugefügt wird, indem Sie einen der folgenden Schritte ausführen:

* Erstellen einer Ansicht für eine Liste von Berichten und Einschließen von Dashboard-Informationen in die Spalten
* Filtern einer Liste von Berichten nach einem oder mehreren bestimmten Dashboards, von denen Sie wissen, dass sie aktiv verwendet werden
* Berichterstellung für das Berichtsobjekt mithilfe einer Ansicht oder eines Filters mit Dashboard-Informationen

Jeder kann eine Ansicht oder einen Filter erstellen. Sie müssen jedoch Zugriff auf Berichte bearbeiten auf Ihrer Zugriffsebene haben, um einen Bericht zu erstellen.\
Weitere Informationen zum Zugriff auf Berichte finden Sie im Artikel [Zugriff auf Berichte, Dashboards und Kalender gewähren](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md).\
Weitere Informationen zum Erstellen eines Berichts finden Sie im Artikel [Benutzerdefinierten Bericht erstellen](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

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

## Anzeigen von Dashboard-Informationen in der Berichtsliste

So erstellen Sie eine Ansicht mit Dashboard-Informationen für eine Berichtsliste:

1. Klicken Sie auf **Hauptmenü** icon ![](assets/main-menu-icon.png) Klicken Sie oben rechts in Workfront auf **Berichte**.

1. Klicken Sie in der Liste der Berichte auf die **Ansicht** Dropdown-Menü.
1. Klicken **Neue Ansicht**.
1. Klicken **Spalte hinzufügen**.
1. Beginnen Sie mit der Eingabe von &quot;Dashboards&quot;im **Eingabe des Feldnamens beginnen** -Feld.
1. Unter dem **Bericht** Objekt, auswählen **Dashboards**.

1. Klicken **Ansicht speichern**.\
   Die Dashboards, in denen ein Bericht angezeigt wird, werden in der Spalte Dashboards der Berichtsliste angezeigt.\
   ![](assets/qs-dashboards-in-report-view.png)

## Berichtsliste nach Dashboard-Informationen filtern

So filtern Sie eine Liste von Berichten nach Dashboard-Informationen:

1. Klicken Sie auf **Hauptmenü** icon ![](assets/main-menu-icon.png) Klicken Sie oben rechts in Workfront auf **Berichte**.

1. Klicken Sie in der Liste der Berichte auf die **Filter** Dropdown-Menü.
1. Klicken **Neuer Filter** Klicken Sie auf **Filterregel hinzufügen**.

1. Beginnen Sie mit der Eingabe von &quot;Dashboards&quot;im **Eingabe des Feldnamens beginnen** -Feld.

1. Unter dem **Dashboards** Objekt, auswählen **Name**.

1. Auswählen **Gleich** Geben Sie im Dropdown-Menü &quot;Modifikator&quot;den Namen des Dashboards ein, nach dem Sie filtern möchten. Sie können mehrere Dashboards für Ihren Filter auswählen.\
   ![](assets/qs-dashboards-in-report-filters-350x143.png)

1. Klicken **Speichern und schließen**.\
   Dadurch wird eine Liste von Berichten angezeigt, die nur in den angegebenen Dashboards aufgeführt sind.\
   Sie können auch einen Bericht für das Berichtsobjekt erstellen und diesen Filter im Bericht verwenden.
