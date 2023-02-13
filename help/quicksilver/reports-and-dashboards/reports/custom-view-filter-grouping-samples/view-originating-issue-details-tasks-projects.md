---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '"Ansicht: Informationen zur Ausgangsausgabe für Aufgaben und Projekte'
description: Wenn ein Problem in eine Aufgabe oder ein Projekt konvertiert wird, wird eine aufgelöste Objektbeziehung zwischen der Aufgabe oder dem Projekt und dem Problem hergestellt. In dieser Ansicht werden die folgenden Felder des Problems angezeigt, die automatisch abgeschlossen werden, wenn die Aufgabe oder das Projekt abgeschlossen ist - BEARBEITEN SIE MICH.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 5fefb174-3a18-408f-aa12-3f4aff23acfa
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '333'
ht-degree: 3%

---

# Ansicht: Informationen zur ursprünglichen Ausgabe für Aufgaben und Projekte

Wenn ein Problem in eine Aufgabe oder ein Projekt konvertiert wird, wird eine aufgelöste Objektbeziehung zwischen der Aufgabe oder dem Projekt und dem Problem hergestellt. In dieser Ansicht werden die folgenden Felder des Problems angezeigt, die automatisch abgeschlossen werden, wenn die Aufgabe oder das Projekt abgeschlossen ist:

* Name
* Eingabedatum
* Geplantes Abschlussdatum
* Tatsächliches Abschlussdatum
* Anfragetyp
* Urheber-Name
* Dem Benutzer zugewiesen

![task_with_resolving_issue_fields.png](assets/task-with-resolving-issue-fields-350x38.png)

Weitere Informationen finden Sie auch unter [Ansicht: Originalausgabeinformationen zu Aufgaben- und Projektlisten anzeigen](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-display-original-issue-info-task-project-list.md).

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

## Details zu Ausgangsthemen für Aufgaben und Projekte anzeigen

1. Gehen Sie zu einer Liste von Aufgaben oder einer Liste von Projekten.
1. Aus dem **Ansicht** Dropdown-Menü auswählen **Neue Ansicht**.

1. Im **Spaltenvorschau** -Bereich, alle Spalten außer einer entfernen.
1. Klicken Sie auf die Kopfzeile der verbleibenden Spalte und dann auf **In den Textmodus wechseln**.
1. Bewegen Sie den Mauszeiger über den Textmodusbereich und klicken Sie auf **Klicken, um Text zu bearbeiten**.
1. Entfernen Sie den Text, den Sie im **Textmodus** und ersetzen Sie sie durch den folgenden Code:

   <!-- [Copy](javascript:void(0);) -->
   <pre></pre>

1. Klicken **Ansicht speichern**.
