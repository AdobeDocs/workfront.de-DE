---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: "Ansicht: Übermittlungspfad für Probleme"
description: Sie können den Pfad, über den ein Problem gesendet wurde, in der Ansicht eines Problemberichts anzeigen. Der Pfad gibt die Warteschlange, die Themengruppe und das Warteschlangenthema an, an das das Problem ursprünglich gesendet wurde.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: bee1e066-c3f4-4d74-92b0-ab7f43d52a50
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '292'
ht-degree: 1%

---

# Ansicht: Übermittlungspfad für Probleme

Sie können den Pfad, über den ein Problem gesendet wurde, in der Ansicht eines Problemberichts anzeigen. Der Pfad gibt die Warteschlange, die Themengruppe und das Warteschlangenthema an, an das das Problem ursprünglich gesendet wurde.

![issue_submission_path.png](assets/issue-submission-path-350x66.png)

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
   <td> <p>Anforderung zum Ändern einer Ansicht </p>
   <p>Berichtänderung planen</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf Berichte, Dashboards und Kalender bearbeiten, um einen Bericht zu ändern</p> <p>Zugriff auf Filter, Ansichten und Gruppierungen bearbeiten, um eine Ansicht zu ändern</p> <p><b>NOTIZ</b>

Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td>
</tr>   
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Berechtigungen für einen Bericht verwalten</p> <p>Weitere Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Anfordern des Zugriffs auf Objekte </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Übermittlungspfad für Probleme anzeigen

1. Gehen Sie zu einer Liste von Problemen.
1. Wählen Sie aus dem Dropdownmenü **Ansicht** die Option **Neue Ansicht** aus.

1. Klicken Sie im Bereich **Spaltenvorschau** auf **Spalte hinzufügen**.

1. Klicken Sie auf die Kopfzeile der neuen Spalte und dann auf **In Textmodus wechseln**.
1. Bewegen Sie den Mauszeiger über den Textmodusbereich und klicken Sie auf **Klicken, um Text zu bearbeiten**.
1. Entfernen Sie den Text, den Sie im Feld **Textmodus** finden, und ersetzen Sie ihn durch den folgenden Code:
   <pre>displayName= Issue Path<br>linkedname=direct <br>namekey=displayQueueBreadcrumb <br>valueField=displayQueueBreadcrumb <br>valueFormat=HTML<br></pre>

1. Klicken Sie auf **Ansicht speichern**.
