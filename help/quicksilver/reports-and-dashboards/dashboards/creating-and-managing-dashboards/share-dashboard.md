---
product-area: dashboards
navigation-topic: create-and-manage-dashboards
title: Freigeben eines Dashboards
description: Ihr Adobe Workfront-Administrator gewährt Benutzenden Zugriff zum Anzeigen oder Bearbeiten von Dashboards, wenn sie Zugriffsebenen zuweisen. Neben der Zugriffsebene, die Benutzern gewährt wird, können Sie ihnen auch Berechtigungen zum Anzeigen oder Verwalten bestimmter Dashboards erteilen, auf die Sie Zugriff haben.
author: Courtney
feature: Reports and Dashboards
exl-id: 21bd531f-8732-4d6c-b91f-990887285447
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/KuO7OCJCKBreuWLgVgppDM1SdtvDgrA1gDmf3HC1Nx8
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550ccid: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 503
ht-degree: 10%

---

# Freigeben eines Dashboards

<!-- Audited: 1/2025 -->

Ihr Adobe Workfront-Administrator gewährt Benutzenden Zugriff zum Anzeigen oder Bearbeiten von Dashboards, wenn sie Zugriffsebenen zuweisen. Weitere Informationen zum Gewähren des Zugriffs auf Probleme finden Sie unter [Gewähren des Zugriffs auf Berichte, Dashboards und Kalender](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md).

Neben der Zugriffsebene, die Benutzern gewährt wird, können Sie ihnen auch Berechtigungen zum Anzeigen oder Verwalten bestimmter Dashboards erteilen, auf die Sie Zugriff haben. Weitere Informationen zu Zugriffsebenen und Berechtigungen finden Sie unter [Funktionsweise von Zugriffsebenen und Berechtigungen](../../../administration-and-setup/add-users/access-levels-and-object-permissions/how-access-levels-permissions-work-together.md).

Berechtigungen sind für ein Element in Workfront spezifisch und definieren, welche Aktionen man für dieses Element ausführen kann.

>[!NOTE]
>
>Ein Workfront-Administrator kann für alle Benutzenden Berechtigungen zu Elementen im System hinzufügen oder entfernen, ohne Besitzer dieser Elemente zu sein.

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Paket</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
    <td> 
   <p>Licht oder höher</p>
   <p>Überprüfen oder höher</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Anzeigen des Zugriffs auf Berichte, Dashboards, Kalender oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Anzeigen von Berechtigungen oder höher für das Dashboard</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Details zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Voraussetzungen

Das Dashboard muss erstellt werden, bevor Sie es freigeben können.

Informationen zum Erstellen von Dashboards finden Sie unter [Erstellen eines Dashboards](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md).

## Überlegungen zur Freigabe von Dashboards

Zusätzlich zu den unten stehenden Überlegungen finden Sie weitere Informationen unter [Freigeben von Berichten, Dashboards und Kalendern](../../../workfront-basics/grant-and-request-access-to-objects/permissions-reports-dashboards-calendars.md).

* Der Ersteller eines Dashboards hat standardmäßig Verwaltungsberechtigungen dafür.

* Sie können Dashboards, die Sie erstellen, für andere Einzelpersonen, Teams, Gruppen, Aufgabengebiete oder Unternehmen freigeben. Sie können auch Dashboards freigeben, die andere erstellt haben und die für Sie freigegeben wurden.
* Sie können sie auch für Ihr gesamtes Unternehmen freigeben, indem Sie sie systemweit sichtbar machen.
* Sie können ein einzelnes Dashboard oder mehrere Dashboards aus einer Liste freigeben.
* Wenn Sie ein Dashboard freigeben, erben Benutzer standardmäßig die Ansichtsberechtigungen für alle Berichtsobjekte im Dashboard.

  Weitere Informationen zur Objekthierarchie in Workfront finden Sie unter [Grundlegendes zu Objekten in Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

  Weitere Informationen zum Anzeigen geerbter Berechtigungen finden Sie unter [Anzeigen geerbter Berechtigungen für Objekte](../../../workfront-basics/grant-and-request-access-to-objects/view-inherited-permissions-on-objects.md).

## Freigeben eines Dashboards

Die Freigabe eines Dashboards oder mehrerer Dashboards aus einer Liste ist identisch.

1. Gehen Sie zu einer Liste von Dashboards, wählen Sie ein oder mehrere Dashboards aus und klicken Sie dann auf **Freigeben** ![](assets/share-icon.png).

   ODER

   Klicken Sie auf den Namen eines Dashboards und dann auf **Dashboard-Aktionen** > **Freigabe**.

   ![](assets/unshimmed-share-dashboard.png)

1. Beginnen Sie im Feld **Personen, Teams, Rollen, Gruppen oder Firmen hinzufügen** mit der Eingabe des Namens des Benutzers, Teams, der Rolle, Gruppe oder Firma, für den Sie das Dashboard freigeben möchten, und klicken Sie dann auf den Namen, wenn er in der Dropdown-Liste angezeigt wird.
1. (Optional) Um das Dashboard für alle Benutzer im System zugänglich zu machen, klicken Sie auf das Dropdown-Menü **Nur eingeladene Benutzer können darauf zugreifen** im Freigabedialogfeld und wählen Sie dann **Alle Benutzer im System können anzeigen**.

1. Klicken Sie auf **Speichern**.
