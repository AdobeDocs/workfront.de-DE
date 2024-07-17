---
product-area: dashboards
navigation-topic: create-and-manage-dashboards
title: Dashboard kopieren
description: Sie können ein Dashboard und alle zugehörigen Inhalte (Berichte, Kalender und externe Seiten) kopieren. Wenn Sie den Inhalt eines Dashboards kopieren, können Sie festlegen, dass die Inhalte so bleiben, wie sie im Original-Dashboard erscheinen, oder neue Elemente erstellen, die Kopien davon im Original-Dashboard sind. Sie können auch festlegen, dass keine Elemente in das neue Dashboard übertragen oder kopiert werden.
author: Nolan
feature: Reports and Dashboards
exl-id: a88cc171-2bb1-40f0-a778-8dac7eecb718
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '901'
ht-degree: 0%

---

# Dashboard kopieren

Sie können ein Dashboard und alle zugehörigen Inhalte (Berichte, Kalender und externe Seiten) kopieren. Wenn Sie den Inhalt eines Dashboards kopieren, können Sie festlegen, dass die Inhalte so bleiben, wie sie im Original-Dashboard erscheinen, oder neue Elemente erstellen, die Kopien davon im Original-Dashboard sind. Sie können auch festlegen, dass keine Elemente in das neue Dashboard übertragen oder kopiert werden.

## Zugriffsanforderungen

Sie müssen über Folgendes verfügen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront-Plan*</strong></td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront-Lizenz*</strong></td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Konfigurationen auf Zugriffsebene*</strong></td> 
   <td> <p>Zugriff auf Berichte, Dashboards und Kalender bearbeiten</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Objektberechtigungen</strong></td> 
   <td> <p>Zugriff auf ein Dashboard anzeigen</p> <p>Sie erhalten Zugriff auf das kopierte Dashboard verwalten .</p> <p>Weitere Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Anfordern des Zugriffs auf Objekte </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Voraussetzungen

Sie müssen ein Dashboard erstellen, bevor Sie es kopieren können.

Informationen zum Erstellen von Dashboards finden Sie unter [Dashboards erstellen](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md).

## Dashboard kopieren

1. Klicken Sie auf das Symbol **Hauptmenü** ![](assets/main-menu-icon.png) und dann auf **Dashboards**.

1. Wählen Sie das Dashboard aus, das Sie kopieren möchten, und klicken Sie dann auf **Kopieren** ![](assets/copy-icon.png).\
   Oder\
   Öffnen Sie das Dashboard, das Sie kopieren möchten, und klicken Sie dann auf **Dashboard-Aktionen** > **Kopieren** .\
   Das Dialogfeld Dashboard kopieren wird angezeigt. Alle Elemente im ursprünglichen Dashboard werden angezeigt.

1. Geben Sie im Feld **Dashboard-Name** einen neuen Namen für das Dashboard an.
1. Lassen Sie die Option &quot;**Alle auswählen**&quot;aktiviert, um alle Elemente im vorhandenen Dashboard auszuwählen und in das kopierte Dashboard zu kopieren. Standardmäßig werden die Berichte, Kalender oder Listen im vorhandenen Dashboard in das neue Dashboard kopiert.\
   Oder\
   Um nur bestimmte Elemente aus dem ursprünglichen Dashboard in das neue zu übertragen, deaktivieren Sie die Elemente, die nicht im neuen Dashboard angezeigt werden sollen, und wählen Sie dann für jedes ausgewählte Element eine der folgenden Optionen aus:

   * **Kopieren:** Das Element wird aus dem ursprünglichen Dashboard kopiert und eine neue Version dieses Elements wird im neuen Dashboard angezeigt. Änderungen am Element im neuen Dashboard werden nicht im Element im ursprünglichen Dashboard übernommen. Ebenso werden Änderungen am Element im ursprünglichen Dashboard nicht im Element im neuen Dashboard übernommen.\
     Verwenden Sie diese Option, wenn Sie den ursprünglichen Bericht im Original-Dashboard ändern möchten.\
     Sie kopieren beispielsweise ein Dashboard namens &quot;Team B&quot;und benennen es in &quot;Team A&quot;um. Im Dashboard &quot;Team B&quot;befindet sich ein Bericht namens &quot;Team B Report&quot;. Da dieser Bericht Daten enthält, die spezifisch für Team B sind, wählen Sie die Option, eine Kopie dieses Berichts zu erstellen, damit Sie ihn für Team A anpassen und später in &quot;Team A Report&quot;umbenennen können.\
     Mit dieser Option entfernen Sie die Freigabeberechtigungen des ursprünglichen Berichts aus dem kopierten Bericht. Die Option Diesen Bericht mit Informationsrechten ausführen bleibt im kopierten Bericht intakt.

   * **Original verwenden:** Zeigt das ursprüngliche Element im neuen Dashboard an. Änderungen am Element im neuen Dashboard werden auch im Element im ursprünglichen Dashboard übernommen. Ebenso werden Änderungen am Artikel im ursprünglichen Dashboard im neuen Dashboard angezeigt.\
     Mit dieser Option behalten Sie die Freigabeberechtigungen des ursprünglichen Berichts bei. Die Option Bericht ausführen mit Informationsrechten bleibt intakt.

1. (Optional) Benennen Sie alle ausgewählten Elemente um.
1. Klicken Sie auf **Dashboard kopieren**.
1. (Optional) Wenn Sie einen der kopierten Berichte, Kalender und externen Seiten des kopierten Dashboards bearbeiten möchten, führen Sie einen der folgenden Schritte aus:

   * Um Informationen für einen der kopierten Berichte zu bearbeiten, klicken Sie auf den Berichtsnamen im Dashboard und dann auf **Berichtaktionen** > **Bearbeiten**.

     Sie können beispielsweise den Bericht Ansicht, Filter, Gruppierung, Aufforderung oder Diagramm oder einen kopierten Bericht bearbeiten.

   * Um die Berechtigungen für die kopierten Berichte erneut zu aktivieren, klicken Sie im neuen Dashboard auf den Berichtsnamen, klicken Sie dann auf **Berichtaktionen** > **Freigabe** und aktualisieren Sie die Berechtigungen für den Bericht.

     Wenn Sie einen Bericht kopieren, während Sie ein Dashboard kopieren, werden die Berechtigungen für diesen Bericht entfernt.

   * Um den Bericht Ausführen mit Informationsrechten zu ändern, klicken Sie auf den Namen des Berichts im neuen Dashboard und dann auf **Berichtaktionen** > **Bearbeiten** > **Berichtsoptionen**.\
     Nach dem Kopieren eines Berichts wird der Bericht Ausführen mit Zugriffsrechten nur unter den folgenden Umständen beibehalten:

     (Wenn keine dieser Bedingungen zutrifft, wird der Bericht Ausführen mit den Zugriffsrechten entfernt und der neue Bericht Ausführen mit den Zugriffsrechten von wird in den Benutzer geändert, der den kopierten Bericht erstellt hat.)

     Wenn der Benutzer, der das Dashboard und seine Berichte kopiert, über Administratorrechte verfügt.

      * Wenn der Benutzer, der das Dashboard und seine Berichte kopiert, über Administratorrechte verfügt.
      * Wenn der Benutzer, der das Dashboard und seine Berichte kopiert, derzeit als &quot;Bericht ausführen&quot;mit den Zugriffsrechten von für die kopierten Berichte festgelegt ist.
      * Wenn der Benutzer, der den Bericht kopiert, über Verwaltungsberechtigungen für den Bericht verfügt.
