---
product-area: dashboards
navigation-topic: create-and-manage-dashboards
title: Kopieren eines Dashboards
description: Sie können ein Dashboard samt Inhalt (Berichte, Kalender und externe Seiten) kopieren. Wenn Sie den Inhalt eines Dashboards kopieren, können Sie festlegen, dass er so bleibt, wie er im ursprünglichen Dashboard angezeigt wird, oder neue Elemente erstellen, bei denen es sich um Kopien dieser Elemente im ursprünglichen Dashboard handelt. Sie können auch festlegen, dass Elemente im neuen Dashboard nicht übertragen oder kopiert werden.
author: Courtney
feature: Reports and Dashboards
exl-id: a88cc171-2bb1-40f0-a778-8dac7eecb718
source-git-commit: 6a6d3d47ed5741e3202c44b7240a2e67b687ea95
workflow-type: tm+mt
source-wordcount: '889'
ht-degree: 6%

---

# Kopieren eines Dashboards

<!-- Audited: 1/2025 -->

Sie können ein Dashboard samt Inhalt (Berichte, Kalender und externe Seiten) kopieren. Wenn Sie den Inhalt eines Dashboards kopieren, können Sie diese Elemente so beibehalten, wie sie im ursprünglichen Dashboard angezeigt werden, oder neue Elemente erstellen, bei denen es sich um Kopien der Elemente im ursprünglichen Dashboard handelt. Sie können auch festlegen, dass Elemente nicht in das neue Dashboard übertragen oder kopiert werden.

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
      <p>Standard</p>
      <p>Abo</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriff auf Berichte, Dashboards und Kalender bearbeiten</p></td> 
  </tr>  
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Anzeigen des Zugriffs auf ein Dashboard</p></td> 
  </tr> 
 </tbody> 
</table>

Weitere Details zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Voraussetzungen

Sie müssen ein Dashboard erstellen, bevor Sie es kopieren können.

Informationen zum Erstellen von Dashboards finden Sie unter [Erstellen eines Dashboards](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md).

## Kopieren eines Dashboards

1. Klicken Sie auf das **[!UICONTROL Hauptmenü]**-Symbol ![Hauptmenü](/help/_includes/assets/main-menu-icon.png) in der oberen rechten Ecke von Adobe Workfront oder (falls verfügbar) klicken Sie auf das **[!UICONTROL Hauptmenü]**-Symbol ![Hauptmenü](/help/_includes/assets/main-menu-icon-left-nav.png) in der oberen linken Ecke und klicken Sie dann auf **[!UICONTROL Dashboards]**.

1. Wählen Sie das Dashboard aus, das Sie kopieren möchten, und klicken Sie dann auf **Kopieren** ![Symbol kopieren](assets/copy-icon.png).\
   ODER\
   Öffnen Sie das Dashboard, das Sie kopieren möchten, und klicken Sie dann auf **Dashboard-Aktionen** > **Kopieren**.\
   Das Dialogfeld &quot;Dashboard-Kopie&quot; wird angezeigt. Alle Elemente im ursprünglichen Dashboard werden angezeigt.

1. Geben Sie **Feld Dashboard-Name** einen neuen Namen für das Dashboard an.
1. Wenn Sie alle Elemente im vorhandenen Dashboard auswählen und in das kopierte Dashboard kopieren möchten, lassen Sie **Alle auswählen** ausgewählt. Standardmäßig werden die Berichte, Kalender oder Listen im vorhandenen Dashboard in das neue Dashboard kopiert.\
   ODER\
   Um nur bestimmte Elemente aus dem ursprünglichen Dashboard auf das neue zu übertragen, heben Sie die Auswahl der Elemente auf, die nicht im neuen Dashboard angezeigt werden sollen, und wählen Sie dann für jedes ausgewählte Element eine der folgenden Optionen aus:

   * **Kopie erstellen** Das Element wird aus dem ursprünglichen Dashboard kopiert, und eine neue Version dieses Elements wird im neuen Dashboard angezeigt. Änderungen am Element im neuen Dashboard werden nicht im Element im ursprünglichen Dashboard übernommen. Ebenso werden Änderungen am Element im ursprünglichen Dashboard nicht im Element im neuen Dashboard übernommen.\
     Verwenden Sie diese Option, wenn Sie den ursprünglichen Bericht im ursprünglichen Dashboard ändern möchten.\
     Sie kopieren beispielsweise ein Dashboard mit dem Namen &quot;Team B&quot; und benennen es in &quot;Team A&quot; um. Auf dem Team B-Dashboard befindet sich ein Bericht mit dem Namen &quot;Team B-Bericht&quot;. Da dieser Bericht spezifische Daten für Team B enthält, wählen Sie die Option, eine Kopie dieses Berichts zu erstellen, damit Sie ihn für Team A anpassen und später in &quot;Team A-Bericht&quot; umbenennen können.\
     Mit dieser Option entfernen Sie die Freigabeberechtigungen des ursprünglichen Berichts aus dem kopierten Bericht. Der Bericht &quot;Diesen Bericht ausführen&quot; mit den Zugriffsrechten für Informationen bleibt im kopierten Bericht intakt.

   * **Original verwenden:** Zeigt das ursprüngliche Element im neuen Dashboard an. Änderungen, die am Element im neuen Dashboard vorgenommen werden, werden auch im Element im ursprünglichen Dashboard angezeigt. Ebenso werden Änderungen am Element im ursprünglichen Dashboard im Element im neuen Dashboard widergespiegelt.\
     Mit dieser Option behalten Sie die Freigabeberechtigungen des ursprünglichen Berichts bei. Die Ausführung dieses Berichts mit den Zugriffsrechten für Informationen bleibt ebenfalls intakt.

1. (Optional) Benennen Sie die ausgewählten Elemente um.
1. Klicken Sie **Dashboard kopieren**.
1. (Optional) Wenn Sie einen der kopierten Berichte, Kalender oder externen Seiten im kopierten Dashboard bearbeiten möchten, führen Sie einen der folgenden Schritte aus:

   * Um Informationen für einen der kopierten Berichte zu bearbeiten, klicken Sie auf den Namen des Berichts im Dashboard und anschließend auf **Berichtsaktionen** > **Bearbeiten**.

     Beispielsweise können Sie den Bericht &quot;Ansicht&quot;, &quot;Filter&quot;, &quot;Gruppierung&quot;, &quot;Eingabeaufforderung&quot; oder &quot;Diagramm&quot; oder einen kopierten Bericht bearbeiten.

   * Um die Berechtigungen für die kopierten Berichte erneut zu aktivieren, klicken Sie im neuen Dashboard auf den Berichtsnamen und dann auf **Berichtsaktionen** > **Freigabe** und aktualisieren Sie die Berechtigungen für den Bericht.

     Wenn Sie einen Bericht kopieren, während Sie ein Dashboard kopieren, werden die Berechtigungen für diesen Bericht entfernt.

   * Um die Funktion Diesen Bericht ausführen mit den Zugriffsrechten für Informationen zu ändern, klicken Sie im neuen Dashboard auf den Namen des Berichts und anschließend auf **Berichtsaktionen** > **Bearbeiten** > **Berichtsoptionen**.\
     Nachdem Sie einen Bericht kopiert haben, können Sie diesen Bericht mit den Zugriffsrechten von Berechtigungen nur unter folgenden Umständen ausführen:

     (Wenn keine dieser Bedingungen zutrifft, wird dieser Bericht mit den Zugriffsrechten von Berechtigungen ausführen entfernt und der neue Bericht mit den Zugriffsrechten von wird in den Benutzer geändert, der den kopierten Bericht erstellt hat.)

     Wenn der Benutzer, der das Dashboard und seine Berichte kopiert, über Administratorzugriffsrechte verfügt.

      * Wenn der Benutzer, der das Dashboard und seine Berichte kopiert, über Administratorzugriffsrechte verfügt.
      * Wenn der Benutzer, der das Dashboard und seine Berichte kopiert, derzeit als &quot;Diesen Bericht ausführen&quot; mit den Zugriffsrechten von für die zu kopierenden Berichte festgelegt ist.
      * Wenn der Benutzer, der den Bericht kopiert, über Verwaltungsberechtigungen für den Bericht verfügt.
