---
content-type: reference
product-area: reporting;projects;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: '"Ansicht: Liste der Projektbenutzer mit Auftragsrollen'
description: Sie können diese Ansicht in einer Projektliste oder einem Bericht anwenden, um eine Liste der mit dem Projekt verknüpften Benutzer sowie eine Liste der vom Projekt ausgeführten Auftragsrollen anzuzeigen.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: a3f59f69-7f39-4814-bd2f-7734d620081e
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '460'
ht-degree: 0%

---

# Ansicht: Liste der Projektbenutzer mit Auftragsprofilen

Sie können diese Ansicht in einer Projektliste oder einem Bericht anwenden, um eine Liste der mit dem Projekt verknüpften Benutzer sowie eine Liste der vom Projekt ausgeführten Auftragsrollen anzuzeigen.

Die Informationen in diesem Bericht finden Sie auch im Bereich Personen des Projekts.

>[!TIP]
>
>Wenn für die Benutzer keine Jobrollen aufgelistet sind, Sie jedoch wissen, dass sie mit Berufsrollen in ihren Benutzerprofilen verknüpft sind, kann dies bedeuten, dass sie Aufgaben und Problemen zugewiesen sind, sie jedoch möglicherweise nicht mit einer Job-Rolle für die Aufgabe oder das Problem verknüpft sind, oder die im Bericht aufgelisteten Benutzer sind nicht die Verantwortlichen für Aufgaben und Probleme, sondern erfüllen andere Rollen im Projekt (z. B. Inhaber oder Sponsor).

![project_with_user_and_role_information_report.png](assets/project-with-user-and-role-information-report-350x100.png)

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

## Anzeigen einer Liste von Projektbenutzern mit Aufgabenrollen

1. Gehen Sie zu einer Projektliste.
1. Aus dem **Ansicht** Dropdown-Menü auswählen **Neue Ansicht**.

1. Im **Spaltenvorschau** -Bereich, alle Spalten außer einer entfernen.
1. Klicken Sie auf die Kopfzeile der verbleibenden Spalte und dann auf **In den Textmodus wechseln**.
1. Bewegen Sie den Mauszeiger über den Textmodusbereich und klicken Sie auf **Klicken, um Text zu bearbeiten**.
1. Entfernen Sie den Text, den Sie im **Textmodus** und ersetzen Sie sie durch den folgenden Code:
   <pre>column.0.link.valueFormat=val<br>column.0.linkedname=direct<br>column.0.listsort=string(name)<br>column.0.namekey=name.abbr<br>column.0.querysort=name<br>column.0.section=0<br>column.0.shortview=false<br>column.0.gestreckch=100<br>column.0.valueField=name<br>column.0.valueFormat=HTML<br>column.0.width=200<br>column.1.displayName=Project Users<br>column.1.listdelimiter=&lt;br&gt;<br>column.1.listmethod=nested(projectUsers).lists<br>column.1.textmode=true<br>column.1.type=iterate<br>column.1.valueExpression={user}.{name}<br>column.1.valueFormat=HTML<br>column.2.displayName=Projektrollen<br>column.2.listdelimiter=&lt;br&gt;<br>column.2.listmethod=nested(projectUserRoles).lists<br>column.2.textmode=true<br>column.2.type=iterate<br>column.2.valueExpression={role}.{name}<br>column.2.valueFormat=HTML</pre>

1. Klicken **Ansicht speichern**.
