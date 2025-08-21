---
title: Audit-Protokolle anzeigen und exportieren
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: Sie können alle Audit-Protokolle im System oder diejenigen anzeigen, die bestimmte Filterkriterien erfüllen. Sie können auch Auditprotokolle exportieren. Audit-Protokolle enthalten Benutzeränderungen, die in den letzten 90 Tagen im System ausgelöst wurden.
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: b04e8ba5-c3f2-4838-8df1-35e90de5c7bd
source-git-commit: 4569b5bd004a93396257f3f1f8964831f69399dc
workflow-type: tm+mt
source-wordcount: '424'
ht-degree: 2%

---

# Auditprotokolle anzeigen und exportieren

<!--
**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **
-->

Sie können alle Audit-Protokolle im System oder diejenigen anzeigen, die bestimmte Filterkriterien erfüllen. Sie können Auditprotokolle auch in eine CSV-Datei exportieren.

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
   <td role="rowheader">Adobe Workfront-Paket</td> 
   <td><p>Beliebig</p></td> 
  </tr> 
  <tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td><p>Standard</p>
       <p>Plan</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td><p>Systemadministrator</p></td>
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Audit-Protokolle anzeigen

{{step-1-to-setup}}

1. Klicken Sie im linken Bedienfeld auf **System > Auditprotokolle**.
1. Wählen **in der Dropdown** Liste „Aktionstyp“ den Audit-Typ aus, den Sie anzeigen möchten.

   >[!NOTE]
   >
   >Die Optionen im Dropdown-Menü Aktionstyp variieren je nach ausgewähltem Auditprotokoll.

1. Wählen **im Dropdown-Menü** Protokolltyp“ den Typ des Administratorprotokolls aus, den Sie anzeigen möchten.

   **Alle Protokolltypen** ist standardmäßig ausgewählt.

   Eine Liste aller Prüfprotokolltypen, die angezeigt werden können, und der darin enthaltenen Informationen finden Sie unter [Prüfprotokolle](../../../administration-and-setup/add-users/create-and-manage-users/audit-logs.md).

1. (Optional) Legen Sie einen der verfügbaren Filter für die folgenden Felder fest:

   * **Benutzer**: Geben Sie den Namen des Benutzers ein, der eine Änderung vorgenommen hat.
   * **Von**: Startdatum des Zeitrahmens, in dem die Änderung vorgenommen wurde.
   * **An**: Enddatum des Zeitrahmens, in dem die Änderung vorgenommen wurde.

   ![Administratorprotokolle](assets/audit-logs.png)

1. Klicken Sie auf **Übernehmen**.
1. (Optional) Klicken Sie auf **Löschen**, um die an den Filtern vorgenommenen Änderungen zurückzusetzen.

## Auditprotokolle exportieren

{{step-1-to-setup}}

1. Klicken Sie im linken Bedienfeld auf **System** > **Auditprotokolle**.

1. Wählen Sie **Dropdown-Menü** Protokolltyp) ein Administratorprotokoll aus.

   **Alle Protokolltypen** ist standardmäßig ausgewählt.

1. Legen Sie einen der verfügbaren Filter fest und klicken Sie dann auf **Anwenden**.

   >[!IMPORTANT]
   >
   >Sie können nicht mehr als 50.000 Protokolle gleichzeitig exportieren. Workfront exportiert Protokolle basierend auf den von Ihnen festgelegten Filtern und nicht auf der Anzahl der auf der Seite angezeigten Protokolle. Sie können die Gesamtzahl der gefilterten Protokolle in der rechten unteren Ecke der Seite anzeigen.

1. Klicken Sie **Exportieren**.

   Das Feld Datei speichern wird geöffnet, und Sie können die exportierte Datei auf Ihrem Computer speichern.

   Auditprotokolle können nur im CSV-Format gespeichert werden.

   Speichern der exportierten Datei beenden Sie können ihn jetzt auf Ihrem Computer finden und für andere freigeben.
