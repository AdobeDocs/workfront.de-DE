---
product-area: reporting;user-management
keywords: save,new,report,copy
navigation-topic: create-and-manage-reports
title: Berichtkopie erstellen
description: Sie können eine Kopie jedes Berichts erstellen, auf den Sie Zugriff haben. Sie können entweder eine exakte Kopie eines benutzerspezifischen Berichts erstellen oder eine neue Version eines Standardberichts speichern. Nachdem Sie einen Bericht kopiert haben, werden Sie zum Eigentümer des kopierten Berichts und dieser wird im Abschnitt Meine Berichte angezeigt.
author: Nolan
feature: Reports and Dashboards
exl-id: 84737f48-efc5-45f1-acd1-b9f5d353f80f
source-git-commit: 548e713700fda79070f59f3dc3457410d2c50133
workflow-type: tm+mt
source-wordcount: '676'
ht-degree: 0%

---

# Berichtkopie erstellen

Sie können eine Kopie jedes Berichts erstellen, auf den Sie Zugriff haben. Sie können entweder eine exakte Kopie eines benutzerspezifischen Berichts erstellen oder eine neue Version eines Standardberichts speichern. Nachdem Sie einen Bericht kopiert haben, werden Sie zum Eigentümer des kopierten Berichts und dieser wird im Abschnitt Meine Berichte angezeigt.

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
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf Berichte, Dashboards und Kalender bearbeiten</p> <p>Zugriff auf Filter, Ansichten, Gruppierungen bearbeiten</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Berechtigungen für einen Bericht anzeigen</p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Erstellen einer exakten Kopie eines Berichts

Wenn Sie eine Kopie eines Berichts erstellen möchten, dessen Eigentümer Sie sind, gehen Sie wie folgt vor:

1. Klicken Sie auf **Hauptmenü** icon ![](assets/main-menu-icon.png) in der oberen rechten Ecke von Adobe Workfront.

1. Klicks **Berichte**, dann **Alle Berichte**.
1. Öffnen Sie einen Bericht.
1. Klicks **Berichtaktionen**, dann **Kopieren**.

   >[!TIP]
   >
   >Wenn es sich bei dem Bericht um einen Standardbericht handelt, wird die Option Kopieren nicht im Menü Berichtaktionen angezeigt.\
   >Informationen zum Erstellen einer Kopie eines Standardberichts finden Sie unter [Neue Berichtversion erstellen](#create-a-new-version-of-a-report).

   ![Bericht kopieren](assets/nwe-fulllistofreportactions-2022.png)

   Eine Kopie des ursprünglichen Berichts wird mit dem Standardnamen *Kopie von [Name des ursprünglichen Berichts]*. Zum Beispiel hätte der Bericht &quot;Abgeschlossene Aufgaben im 4. Quartal&quot;den Namen &quot;Kopie der abgeschlossenen Aufgaben im 4. Quartal&quot;.

1. (Optional) Um den Bericht umzubenennen, geben Sie einen neuen Namen ein.

   >[!TIP]
   >
   >Wenn Sie die Auswahl des Titels aufheben, bevor Sie den neuen Namen eingeben, wählen Sie den Berichtstitel aus, löschen Sie den Namen und geben Sie den neuen Namen ein.

1. (Optional) Um die neue Version des Berichts für andere Benutzer freizugeben, klicken Sie auf **Berichtaktionen**, dann **Freigabe**.

   >[!NOTE]
   >
   >Die Freigabeinformationen werden nicht von der Originalversion in den kopierten Bericht übertragen.\
   >Informationen dazu, wie Sie sehen, für wen der vorherige Bericht freigegeben wurde, finden Sie unter [Erstellen eines Berichts über Berichtsaktivitäten](../../../reports-and-dashboards/reports/report-usage/create-report-reporting-activities.md#identify).

1. (Optional) Wenn Sie über Verwaltungsberechtigungen für den ursprünglichen Bericht verfügen und der Originalbericht nicht mehr benötigt wird, können Sie ihn löschen, um unnötige duplizierte Berichte in Workfront zu entfernen.

   Gehen Sie wie folgt vor, um den ursprünglichen Bericht zu löschen:

   1. Navigieren Sie zum Bericht.
   1. Klicks **Berichtaktionen**, dann **Löschen**.

   1. Klicks **Ja, löschen** , um zu bestätigen, dass Sie den Bericht löschen möchten.

## Neue Berichtversion erstellen {#create-a-new-version-of-a-report}

Wenn Sie eine Kopie eines Standardberichts erstellen möchten, gehen Sie wie folgt vor:

1. Klicken Sie auf **Hauptmenü** icon ![](assets/main-menu-icon.png) in der oberen rechten Ecke von Adobe Workfront.

1. Klicks **Berichte**, dann **Alle Berichte**.
1. Klicken Sie auf den Namen eines Standardberichts, um ihn zu öffnen.
1. Klicks **Berichtaktionen**, dann **Bearbeiten**.

   ![Bericht bearbeiten](assets/nwe-reportactionsfordefaultreport-2022.png)

1. Nehmen Sie in den folgenden Registerkarten des Berichts die erforderlichen Änderungen vor:

   * **Spalten (Ansicht)**: Weitere Informationen zum Anpassen von Ansichten finden Sie im Artikel [Ansichten - Übersicht in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).
   * **Gruppierungen**: Weitere Informationen zum Anpassen von Gruppierungen finden Sie im Artikel [Gruppierungsübersicht in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).
   * **Filter**: Weitere Informationen zum Anpassen von Filtern finden Sie im Artikel [Filterübersicht](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).
   * **Diagramm**: Weitere Informationen zum Anpassen eines Berichtdiagramms finden Sie im Artikel [Diagramm zu einem Bericht hinzufügen](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md).

1. Klicken Sie oben rechts auf **Berichtseinstellungen**.
1. Im **Berichttitel** einen neuen Namen für den Bericht eingeben.
1. Klicks **Fertig**.
1. Klicks **Als neuen Bericht speichern**.

   ![](assets/nwe-save-as-new-report-350x220.png)

1. (Optional) Um die neue Version des Berichts für andere Benutzer freizugeben, klicken Sie auf **Berichtaktionen**, dann **Freigabe**.
