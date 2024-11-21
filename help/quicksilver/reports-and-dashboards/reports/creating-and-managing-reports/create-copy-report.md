---
product-area: reporting;user-management
keywords: save,new,report,copy
navigation-topic: create-and-manage-reports
title: Berichtkopie erstellen
description: Sie können eine Kopie jedes Berichts erstellen, auf den Sie Zugriff haben. Sie können entweder eine exakte Kopie eines benutzerspezifischen Berichts erstellen oder eine neue Version eines Standardberichts speichern. Nachdem Sie einen Bericht kopiert haben, werden Sie zum Eigentümer des kopierten Berichts und dieser wird im Abschnitt Meine Berichte angezeigt.
author: Nolan
feature: Reports and Dashboards
exl-id: 84737f48-efc5-45f1-acd1-b9f5d353f80f
source-git-commit: 9396cd2ac073a57b7d99618cdf09e54ddcf95130
workflow-type: tm+mt
source-wordcount: '642'
ht-degree: 0%

---

# Berichtkopie erstellen

<!-- Audited: 11/2024 -->

Sie können eine Kopie jedes Berichts erstellen, auf den Sie Zugriff haben. Sie können entweder eine exakte Kopie eines benutzerspezifischen Berichts erstellen oder eine neue Version eines Standardberichts speichern. Nachdem Sie einen Bericht kopiert haben, werden Sie zum Eigentümer des kopierten Berichts und dieser wird im Abschnitt Meine Berichte angezeigt.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

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
   <td> 
      <p>Neu:</p>
         <ul>
         <li><p>Standard</p></li>
         </ul>
      <p>Aktuell:</p>
         <ul>
         <li><p>Plan</p></li>
         </ul>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf Berichte, Dashboards und Kalender bearbeiten</p> <p>Zugriff auf Filter, Ansichten, Gruppierungen bearbeiten</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen*</td> 
   <td><p>Berechtigungen für einen Bericht anzeigen</p></td> 
  </tr> 
 </tbody> 
</table>

*Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Erstellen einer exakten Kopie eines Berichts

Wenn Sie eine Kopie eines benutzerspezifischen Berichts erstellen möchten, gehen Sie wie folgt vor:

1. Klicken Sie auf das Symbol **[!UICONTROL Hauptmenü]** ![Hauptmenü](/help/_includes/assets/main-menu-icon.png) oben rechts in Adobe Workfront oder (falls verfügbar) auf das Symbol **[!UICONTROL Hauptmenü]**, das Symbol ![Hauptmenü](/help/_includes/assets/main-menu-icon-left-nav.png) oben links und klicken Sie dann auf **[!UICONTROL Berichte]**.

1. Klicken Sie auf **Alle Berichte** und öffnen Sie dann einen Bericht.

1. Klicken Sie auf **Berichtaktionen** und dann auf **Kopieren**.

   >[!TIP]
   >
   >Wenn es sich bei dem Bericht um einen Standardbericht handelt, wird die Option Kopieren nicht im Menü Berichtaktionen angezeigt.\
   >Informationen zum Erstellen einer Kopie eines Standardberichts finden Sie unter [Erstellen einer neuen Version eines Berichts](#create-a-new-version-of-a-report).

   ![Bericht kopieren](assets/unshimmed-report-actions-copy.png)

   Eine Kopie des ursprünglichen Berichts wird mit dem Standardnamen _[Name des ursprünglichen Berichts] (Kopie)_ erstellt. Eine Kopie des Berichts &quot;Abgeschlossene Aufgaben im 4. Quartal&quot;würde beispielsweise &quot;Abgeschlossene Aufgaben im 4. Quartal (Kopie)&quot;heißen.

1. (Optional) Um den Bericht umzubenennen, klicken Sie auf **Berichtaktionen** und dann auf **Bearbeiten**. Geben Sie in das Textfeld oben links einen neuen Namen ein und klicken Sie dann zum Abschluss auf **Speichern + Schließen** .

1. (Optional) Um die neue Version des Berichts für andere Benutzer freizugeben, klicken Sie auf **Berichtaktionen** und dann auf **Freigabe**.

   >[!NOTE]
   >
   >Die Freigabeinformationen werden nicht von der Originalversion in den kopierten Bericht übertragen.\
   >Informationen dazu, wie Sie sehen, für wen der vorherige Bericht freigegeben wurde, finden Sie unter [Erstellen eines Berichts über Berichterstellungsaktivitäten](../../../reports-and-dashboards/reports/report-usage/create-report-reporting-activities.md#identify).

1. (Optional) Wenn Sie über Verwaltungsberechtigungen für den ursprünglichen Bericht verfügen und der Originalbericht nicht mehr benötigt wird, können Sie ihn löschen, um unnötige duplizierte Berichte in Workfront zu entfernen.

   Gehen Sie wie folgt vor, um den ursprünglichen Bericht zu löschen:

   1. Navigieren Sie zum Bericht.

   1. Klicken Sie auf **Berichtaktionen** und dann auf **Löschen**.

   1. Klicken Sie auf **Ja, löschen Sie es** , um zu bestätigen, dass Sie den Bericht löschen möchten.

## Neue Berichtversion erstellen {#create-a-new-version-of-a-report}

Wenn Sie eine Kopie eines Standardberichts erstellen möchten, gehen Sie wie folgt vor:

1. Klicken Sie oben rechts in Adobe Workfront auf das Symbol **Hauptmenü** ![](assets/main-menu-icon.png).

1. Klicken Sie auf **Berichte** und dann auf **Alle Berichte**.
1. Klicken Sie auf den Namen eines Standardberichts, um ihn zu öffnen.
1. Klicken Sie auf **Berichtaktionen** und dann auf **Bearbeiten**.

   ![Bericht bearbeiten](assets/unshimmed-report-actions-default-report.png)

1. Nehmen Sie in den folgenden Registerkarten des Berichts die erforderlichen Änderungen vor:

   * **Spalten (Ansicht)**: Weitere Informationen zum Anpassen von Ansichten finden Sie im Artikel [Übersicht über Ansichten in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).
   * **Gruppierungen**: Weitere Informationen zum Anpassen von Gruppierungen finden Sie im Artikel [Gruppierungsübersicht in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).
   * **Filter**: Weitere Informationen zum Anpassen von Filtern finden Sie im Artikel [Filterübersicht](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).
   * **Diagramm**: Weitere Informationen zum Anpassen eines Berichtdiagramms finden Sie im Artikel [Hinzufügen eines Diagramms zu einem Bericht](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md) .

1. Klicken Sie oben rechts auf **Berichtseinstellungen**.
1. Geben Sie im Feld **Berichttitel** einen neuen Namen für den Bericht ein.
1. Klicken Sie auf **Fertig**.
1. Klicken Sie auf **Als neuen Bericht speichern**.

   ![](assets/unshimmed-save-as-new-report.png)

1. (Optional) Um die neue Version des Berichts für andere Benutzer freizugeben, klicken Sie auf **Berichtaktionen** und dann auf **Freigabe**.
