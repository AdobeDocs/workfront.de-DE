---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '''Filter: Nur Elemente im Genehmigungsstatus anzeigen"'
description: Sie können nur Elemente mit einem bestimmten Status anzeigen, der sich derzeit in "Ausstehende Genehmigung"befindet. Dies gilt für alle anderen Objekte mit Genehmigungsstatus.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: c1de5193-d3d5-406c-aa68-e6ba6d6751ae
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '315'
ht-degree: 1%

---

# Filter: Nur Elemente im Genehmigungsstatus anzeigen

Sie können nur Elemente mit einem bestimmten Status anzeigen, der sich derzeit in &quot;Ausstehende Genehmigung&quot;befindet. Dies gilt für alle anderen Objekte mit Genehmigungsstatus.

Sie können die folgenden Objekte in einen Genehmigungsstatus platzieren:

* Aufgaben
* Probleme
* Projekte

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
   <td> <p>Filteränderung anfordern </p>
   <p>Berichtänderung planen</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf Berichte, Dashboards und Kalender bearbeiten, um einen Bericht zu ändern</p> <p>Zugriff auf Filter, Ansichten und Gruppierungen bearbeiten, um einen Filter zu ändern</p> <p><b>NOTIZ</b>

Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td>
</tr>
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Berechtigungen für einen Bericht verwalten</p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Nur Elemente im Genehmigungsstatus anzeigen

1. Navigieren Sie zum Filter, den Sie für eine Liste von Projekten anpassen möchten, z. B. .
1. Klicken **Filterregel hinzufügen** für **Status** -Feld des Listenobjekts.\
   Fügen Sie beispielsweise in einem Projektbericht **Status Gleiche Planung**, wenn Sie nur Projekte anzeigen möchten, die sich im Status **Planung - Ausstehende Genehmigung**.

1. Klicken **In den Textmodus wechseln**.
1. Ändern Sie die

   ```
   status
   ```

   Zeile durch Hinzufügen **:A** zum 3-Buchstaben-Schlüssel des Status:
   <pre>status=PLN:A<br>status_Mod=in</pre>

1. Klicken **Fertig**, dann **Filter speichern**.

   In der Liste werden nur Projekte angezeigt, die den Status Planung - Ausstehende Genehmigung aufweisen.
