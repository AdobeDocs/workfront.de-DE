---
product-area: dashboards
navigation-topic: create-and-manage-dashboards
title: Dashboard freigeben
description: Ihr Adobe Workfront-Administrator gewährt Benutzern Zugriff auf das Anzeigen oder Bearbeiten von Dashboards, wenn sie Zugriffsebenen zuweisen. Neben der Zugriffsebene, die Benutzern gewährt wird, können Sie ihnen auch Berechtigungen zum Anzeigen oder Verwalten bestimmter Dashboards erteilen, auf die Sie Zugriff haben.
author: Nolan
feature: Reports and Dashboards
exl-id: 21bd531f-8732-4d6c-b91f-990887285447
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '542'
ht-degree: 0%

---

# Dashboard freigeben

Ihr Adobe Workfront-Administrator gewährt Benutzern Zugriff auf das Anzeigen oder Bearbeiten von Dashboards, wenn sie Zugriffsebenen zuweisen. Weitere Informationen zur Gewährung des Zugriffs auf Probleme finden Sie unter [Gewähren des Zugriffs auf Berichte, Dashboards und Kalender](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md).

Neben der Zugriffsebene, die Benutzern gewährt wird, können Sie ihnen auch Berechtigungen zum Anzeigen oder Verwalten bestimmter Dashboards erteilen, auf die Sie Zugriff haben. Weitere Informationen zu Zugriffsebenen und Berechtigungen finden Sie unter [Wie Zugriffsebenen und -berechtigungen zusammenarbeiten](../../../administration-and-setup/add-users/access-levels-and-object-permissions/how-access-levels-permissions-work-together.md).

Berechtigungen beziehen sich auf ein Element in Workfront und legen fest, welche Aktionen für dieses Element durchgeführt werden können.

>[!NOTE]
>
>Ein Workfront-Administrator kann allen Elementen im System Berechtigungen hinzufügen oder entfernen, ohne Eigentümer dieser Elemente zu sein.

## Zugriffsanforderungen

Sie müssen über Folgendes verfügen, um Objekte freizugeben:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront-Plan*</strong></td> 
   <td> <p>Alle </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront-Lizenz*</strong></td> 
   <td> <p>Überprüfen oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Konfigurationen auf Zugriffsebene*</strong></td> 
   <td> <p>Zugriff auf Berichte, Dashboards, Kalender oder höher anzeigen</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Objektberechtigungen</strong></td> 
   <td> <p>Anzeigen von Berechtigungen oder höher im Dashboard</p> <p>Weitere Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Anfordern des Zugriffs auf Objekte </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Voraussetzungen

Das Dashboard muss vor der Freigabe erstellt werden.

Informationen zum Erstellen von Dashboards finden Sie unter [Dashboards erstellen](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md).

## Überlegungen zum Freigeben von Dashboards

Weitere Informationen finden Sie unter [Berichte, Dashboards und Kalender freigeben](../../../workfront-basics/grant-and-request-access-to-objects/permissions-reports-dashboards-calendars.md).

* Der Ersteller eines Dashboards verfügt standardmäßig über die Berechtigung &quot;Verwalten&quot;.

* Sie können Dashboards, die Sie erstellen, für andere Personen, Teams, Gruppen, Rollen oder Unternehmen freigeben. Sie können auch Dashboards freigeben, die von anderen erstellt und für Sie freigegeben wurden.
* Sie können sie auch für Ihre gesamte Organisation freigeben, indem Sie sie systemweit sichtbar machen.
* Sie können ein einzelnes Dashboard oder mehrere Dashboards aus einer Liste freigeben.
* Wenn Sie ein Dashboard freigeben, erben Benutzer standardmäßig Anzeigeberechtigungen für alle Berichtobjekte im Dashboard.

  Weitere Informationen zur Hierarchie von Objekten in Workfront finden Sie unter [Objekte in Adobe Workfront verstehen](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

  Informationen zum Anzeigen von geerbten Berechtigungen finden Sie unter [Anzeigen von geerbten Berechtigungen für Objekte](../../../workfront-basics/grant-and-request-access-to-objects/view-inherited-permissions-on-objects.md).

## Dashboard freigeben

Die Freigabe eines oder mehrerer Dashboards aus einer Liste ist identisch.

1. Gehen Sie zu einer Liste von Dashboards und wählen Sie ein oder mehrere Dashboards aus. Klicken Sie dann auf **Freigeben** ![](assets/share-icon.png) .

   Oder

   Klicken Sie auf den Namen eines Dashboards und dann auf **Dashboard-Aktionen >****Freigeben**.

   ![](assets/qs-dashboard-actions-menu-350x318.png)

1. Geben Sie im Feld &quot;**Personen, Teams, Rollen, Gruppen oder Unternehmen hinzufügen...**&quot;den Namen des Benutzers, Teams, der Rolle, der Gruppe oder des Unternehmens ein, für den bzw. die Sie das Dashboard freigeben möchten, und klicken Sie dann auf den Namen, wenn er in der Dropdownliste angezeigt wird.
1. (Optional) Um das Dashboard für alle Benutzer im System zugänglich zu machen, klicken Sie auf das Symbol **Einstellungen** in der oberen rechten Ecke des Dialogfelds &quot;Freigabe&quot;und wählen Sie dann **Dieses Dashboard systemweit anzeigen**.

1. Klicken Sie auf **Speichern**.
