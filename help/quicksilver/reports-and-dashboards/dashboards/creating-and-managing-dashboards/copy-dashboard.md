---
product-area: dashboards
navigation-topic: create-and-manage-dashboards
title: Dashboard kopieren
description: Sie können ein Dashboard und alle zugehörigen Inhalte (Berichte, Kalender und externe Seiten) kopieren. Wenn Sie den Inhalt eines Dashboards kopieren, können Sie diese Elemente so beibehalten, wie sie im ursprünglichen Dashboard angezeigt werden, oder neue Elemente erstellen, bei denen es sich um Kopien der Elemente im ursprünglichen Dashboard handelt. Sie können auch festlegen, dass Elemente nicht in das neue Dashboard übertragen oder kopiert werden.
author: Nolan
feature: Reports and Dashboards
exl-id: a88cc171-2bb1-40f0-a778-8dac7eecb718
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '901'
ht-degree: 0%

---

# Dashboard kopieren

Sie können ein Dashboard und alle zugehörigen Inhalte (Berichte, Kalender und externe Seiten) kopieren. Wenn Sie den Inhalt eines Dashboards kopieren, können Sie diese Elemente so beibehalten, wie sie im ursprünglichen Dashboard angezeigt werden, oder neue Elemente erstellen, bei denen es sich um Kopien der Elemente im ursprünglichen Dashboard handelt. Sie können auch festlegen, dass Elemente nicht in das neue Dashboard übertragen oder kopiert werden.

## Zugriffsanforderungen

Sie müssen über Folgendes verfügen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront-Plan*</strong></td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront-Lizenz*</strong></td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Konfigurationen der Zugriffsebene*</strong></td> 
   <td> <p>Zugriff auf Berichte, Dashboards und Kalender bearbeiten</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Einschränkungen in Ihrer Zugriffsebene festgelegt hat. Informationen dazu, wie Workfront-Admins Ihre Zugriffsebene ändern können, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Erstellen oder Ändern benutzerdefinierter Zugriffsebenen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Objektberechtigungen</strong></td> 
   <td> <p>Anzeigen des Zugriffs auf ein Dashboard</p> <p>Sie erhalten Verwaltungszugriff auf das kopierte Dashboard</p> <p>Informationen zum Anfordern zusätzlicher Zugriffsberechtigungen finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Anfordern von Zugriffsberechtigungen für Objekte </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Voraussetzungen

Sie müssen ein Dashboard erstellen, bevor Sie es kopieren können.

Informationen zum Erstellen von Dashboards finden Sie unter [Erstellen eines Dashboards](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md).

## Dashboard kopieren

1. Klicken Sie auf das **Hauptmenü**-Symbol ![](assets/main-menu-icon.png) und dann auf **Dashboards**.

1. Wählen Sie das Dashboard aus, das Sie kopieren möchten, und klicken Sie dann auf **Kopieren** ![](assets/copy-icon.png).\
   Oder\
   Öffnen Sie das Dashboard, das Sie kopieren möchten, und klicken Sie dann auf **Dashboard-Aktionen** > **Kopieren**.\
   Das Dialogfeld Dashboard-Kopie wird angezeigt. Alle Elemente im ursprünglichen Dashboard werden angezeigt.

1. Geben Sie **Feld Dashboard-Name** einen neuen Namen für das Dashboard an.
1. Wenn Sie alle Elemente im vorhandenen Dashboard auswählen und in das kopierte Dashboard kopieren möchten, lassen Sie **Alle auswählen** ausgewählt. Standardmäßig werden die Berichte, Kalender oder Listen im vorhandenen Dashboard in das neue Dashboard kopiert.\
   Oder\
   Um nur bestimmte Elemente aus dem ursprünglichen Dashboard auf das neue zu übertragen, heben Sie die Auswahl der Elemente auf, die nicht im neuen Dashboard angezeigt werden sollen, und wählen Sie dann für jedes ausgewählte Element eine der folgenden Optionen aus:

   * **Kopie erstellen** Das Element wird aus dem ursprünglichen Dashboard kopiert, und eine neue Version dieses Elements wird im neuen Dashboard angezeigt. Änderungen am Element im neuen Dashboard werden nicht im Element im ursprünglichen Dashboard übernommen. Ebenso werden Änderungen am Element im ursprünglichen Dashboard nicht im Element im neuen Dashboard übernommen.\
     Verwenden Sie diese Option, wenn Sie den ursprünglichen Bericht im ursprünglichen Dashboard ändern möchten.\
     Kopieren Sie beispielsweise ein Dashboard namens „Team B“ und benennen Sie es in „Team A“ um. Auf dem Dashboard „Team B“ befindet sich ein Bericht mit dem Namen „Team B-Bericht“. Da dieser Bericht für Team B spezifische Daten enthält, wählen Sie die Option aus, eine Kopie dieses Berichts zu erstellen, damit Sie ihn für Team A anpassen und später in „Team A-Bericht“ umbenennen können.\
     Mit dieser Option entfernen Sie die Freigabeberechtigungen des ursprünglichen Berichts aus dem kopierten Bericht. Die Funktion Diesen Bericht ausführen mit den Zugriffsrechten für Informationen bleibt auf dem kopierten Bericht intakt.

   * **Original verwenden:** Zeigt das ursprüngliche Element im neuen Dashboard an. Änderungen, die am Element im neuen Dashboard vorgenommen werden, werden auch im Element im ursprünglichen Dashboard angezeigt. Ebenso werden Änderungen am Element im ursprünglichen Dashboard im Element im neuen Dashboard widergespiegelt.\
     Mit dieser Option behalten Sie die Freigabeberechtigungen des ursprünglichen Berichts bei. Die Ausführung dieses Berichts mit den Zugriffsrechten für Informationen bleibt ebenfalls intakt.

1. (Optional) Benennen Sie die ausgewählten Elemente um.
1. Klicken Sie **Dashboard kopieren**.
1. (Optional) Wenn Sie einen der kopierten Berichte, Kalender oder externen Seiten im kopierten Dashboard bearbeiten möchten, führen Sie einen der folgenden Schritte aus:

   * Um Informationen für einen der kopierten Berichte zu bearbeiten, klicken Sie auf den Berichtsnamen im Dashboard und anschließend auf **Berichtsaktionen** > **Bearbeiten**.

     Angenommen, Sie möchten die Ansicht, den Filter, die Gruppierung, die Eingabeaufforderung oder das Diagramm oder einen kopierten Bericht bearbeiten.

   * Um die Berechtigungen für die kopierten Berichte wiederherzustellen, klicken Sie auf den Berichtsnamen im neuen Dashboard und anschließend auf **Berichtsaktionen** > **Freigabe** und aktualisieren Sie die Berechtigungen für den Bericht.

     Wenn Sie einen Bericht kopieren, während Sie ein Dashboard kopieren, werden die Berechtigungen für diesen Bericht entfernt.

   * Um die Funktion Diesen Bericht ausführen mit den Zugriffsrechten für Informationen zu ändern, klicken Sie im neuen Dashboard auf den Namen des Berichts und anschließend auf **Berichtsaktionen** > **Bearbeiten** > **Berichtsoptionen**.\
     Nachdem Sie einen Bericht kopiert haben, können Sie diesen Bericht mit den Zugriffsrechten von Berechtigungen nur unter folgenden Umständen ausführen:

     (Wenn keine dieser Bedingungen erfüllt ist, werden die Berechtigungen „Diesen Bericht ausführen“ mit den Zugriffsrechten entfernt und die neue Option Diesen Bericht ausführen mit den Zugriffsrechten von wird für den Benutzer geändert, der den kopierten Bericht erstellt hat.)

     Wenn der Benutzer, der das Dashboard und die zugehörigen Berichte kopiert, über Administratorzugriffsrechte verfügt.

      * Wenn der Benutzer, der das Dashboard und die zugehörigen Berichte kopiert, über Administratorzugriffsrechte verfügt.
      * Wenn der/die Benutzende, der/die das Dashboard und die zugehörigen Berichte kopiert, derzeit als „Diesen Bericht ausführen“ mit den Zugriffsrechten von für die zu kopierenden Berichte festgelegt ist.
      * Wenn der Benutzer, der den Bericht kopiert, über Verwaltungsberechtigungen für den Bericht verfügt.
