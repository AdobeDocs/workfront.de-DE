---
title: Audit-Protokolle anzeigen und exportieren
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: Sie können alle Audit-Protokolle im System oder diejenigen anzeigen, die bestimmte Filterkriterien erfüllen. Sie können auch Auditprotokolle exportieren. Audit-Protokolle enthalten Benutzeränderungen, die in den letzten 90 Tagen im System ausgelöst wurden.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: b04e8ba5-c3f2-4838-8df1-35e90de5c7bd
source-git-commit: d2ca099e78d5adb707a0a5a53ccb2e6dd06698f8
workflow-type: tm+mt
source-wordcount: '328'
ht-degree: 0%

---

# Auditprotokolle anzeigen und exportieren

<!--
**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **
-->

Sie können alle Audit-Protokolle im System oder diejenigen anzeigen, die bestimmte Filterkriterien erfüllen. Sie können auch Auditprotokolle exportieren.

Audit-Protokolle enthalten Benutzeränderungen, die in den letzten 90 Tagen im System ausgelöst wurden.

Informationen zu allen Prüfprotokolltypen und deren Generierung finden Sie unter [Prüfprotokolle](../../../administration-and-setup/add-users/create-and-manage-users/audit-logs.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan</td> 
   <td>Beliebig</td> 
  </tr> 
  <tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td><p>Neu: Standard</p>
       <p>Oder</p>
       <p>Aktuell: Plan</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td>[!UICONTROL Systemadministrator]</td>
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Audit-Protokolle anzeigen

{{step-1-to-setup}}

1. Klicken Sie im linken Bedienfeld auf **System > Auditprotokolle**.
1. Wählen **im Dropdown-Menü** Protokolltyp“ den Typ des Administratorprotokolls aus, den Sie anzeigen möchten.

   **Alle Protokolltypen** ist standardmäßig ausgewählt.

   Eine Liste aller Prüfprotokolltypen, die angezeigt werden können, und der darin enthaltenen Informationen finden Sie unter [Prüfprotokolle](../../../administration-and-setup/add-users/create-and-manage-users/audit-logs.md).

1. (Optional) Legen Sie einen der verfügbaren Filter fest.

   >[!NOTE]
   >
   >Die Optionen im Dropdown-Menü Aktionstyp variieren je nach ausgewähltem Auditprotokoll.

   ![Auditprotokolle](assets/audit-logs.jpg)

1. Klicken Sie **Apply**.
1. (Optional) Klicken Sie auf **Filter löschen**, um die an den Filtern vorgenommenen Änderungen zurückzusetzen.

## Auditprotokolle exportieren

{{step-1-to-setup}}

1. Klicken Sie im linken Bedienfeld auf **System > Auditprotokolle**.

1. Wählen Sie **Dropdown-Menü** Protokolltyp) ein Administratorprotokoll aus.

   **Alle Protokolltypen** ist standardmäßig ausgewählt.

1. Legen Sie einen der verfügbaren Filter fest und klicken Sie dann auf **Anwenden**.

   >[!IMPORTANT]
   >
   >Sie können nicht mehr als 50.000 Protokolle gleichzeitig exportieren. Workfront exportiert Protokolle basierend auf den von Ihnen festgelegten Filtern und nicht auf der Anzahl der auf der Seite angezeigten Protokolle. Sie können die Gesamtzahl der gefilterten Protokolle in der rechten unteren Ecke der Seite anzeigen.

1. Klicken Sie **Exportieren**.
