---
title: Audit-Protokolle anzeigen und exportieren
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: Sie können alle Prüfprotokolle im System oder solche anzeigen, die bestimmte Filterkriterien erfüllen. Sie können auch Prüfprotokolle exportieren. In den Auditprotokollen werden Benutzeränderungen aufgelistet, die in den letzten 90 Tagen im System ausgelöst wurden.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: b04e8ba5-c3f2-4838-8df1-35e90de5c7bd
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '322'
ht-degree: 0%

---

# Audit-Protokolle anzeigen und exportieren

<!--
**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **
-->

Sie können alle Prüfprotokolle im System oder solche anzeigen, die bestimmte Filterkriterien erfüllen. Sie können auch Prüfprotokolle exportieren.

In den Auditprotokollen werden Benutzeränderungen aufgelistet, die in den letzten 90 Tagen im System ausgelöst wurden.

Informationen zu allen Auditprotokolltypen und deren Erstellung finden Sie unter [Auditprotokolle](../../../administration-and-setup/add-users/create-and-manage-users/audit-logs.md).

## Zugriffsanforderungen

Sie müssen über Folgendes verfügen, um die Schritte in diesem Artikel durchzuführen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Abo</td> 
   <td>Beliebig</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td> <p>Plan </p> <p>Sie müssen Workfront-Administrator sein.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Audit-Protokolle anzeigen

1. Klicken Sie auf **Hauptmenü** icon ![](assets/main-menu-icon.png) Klicken Sie oben rechts in Adobe Workfront auf **Einrichtung** ![](assets/gear-icon-settings.png).

1. Klicken Sie im linken Bereich auf **System > Auditprotokolle**.
1. Im **Protokolltyp** aus dem Dropdown-Menü den Typ des Auditprotokolls auswählen, das Sie anzeigen möchten.

   **Alle Protokolltypen** ist standardmäßig ausgewählt.

   Eine Liste aller Prüfprotokolltypen, die Sie anzeigen können, sowie der darin enthaltenen Informationen finden Sie unter [Auditprotokolle](../../../administration-and-setup/add-users/create-and-manage-users/audit-logs.md).

1. (Optional) Legen Sie einen der verfügbaren Filter fest.

   >[!NOTE]
   >
   >Die Optionen im Dropdown-Menü Aktionstyp variieren je nach ausgewähltem Auditprotokoll.

   ![](assets/audit-logs.jpg)

1. Klicken **Anwenden**.
1. (Optional) Klicken Sie auf **Filter löschen** , um an den Filtern vorgenommene Änderungen zurückzusetzen.

## Audit-Protokolle exportieren

1. Klicken Sie auf **Hauptmenü** icon ![](assets/main-menu-icon.png) Klicken Sie oben rechts in Adobe Workfront auf **Einrichtung** ![](assets/gear-icon-settings.png).

1. Klicken Sie im linken Bereich auf **System > Auditprotokolle**.

1. Im **Protokolltyp** ein Auditprotokoll auswählen.

   **Alle Protokolltypen** ist standardmäßig ausgewählt.

1. Legen Sie einen der verfügbaren Filter fest und klicken Sie auf **Anwenden**.

   >[!IMPORTANT]
   >
   >Sie können nicht mehr als 50.000 Protokolle gleichzeitig exportieren. Workfront exportiert Protokolle basierend auf den von Ihnen festgelegten Filtern, nicht auf der Anzahl der Protokolle, die auf der Seite angezeigt werden. Sie können die Gesamtzahl der gefilterten Protokolle in der rechten unteren Ecke der Seite anzeigen.

1. Klicken **Export**.
