---
content-type: reference
product-area: reporting;timesheets
navigation-topic: custom-view-filter-and-grouping-samples
title: "Ansicht: Berechnung der Überstunden in einer Timesheet-Ansicht"
description: Die Zeitüberschreitung wird in Adobe Workfront nicht standardmäßig berechnet, Sie können jedoch einen Zeitplanbericht erstellen, der die Zeitdauer berechnet.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: ad6205cd-7534-49e5-b142-09f90bf672ce
source-git-commit: c49b545938a78716084296ef1b4e7c0fc075ef95
workflow-type: tm+mt
source-wordcount: '472'
ht-degree: 1%

---

# Ansicht: Berechnung der Zeitüberschreitungskosten in einer Timesheet-Ansicht

Die Zeitüberschreitung wird in Adobe Workfront nicht standardmäßig berechnet, Sie können jedoch einen Zeitplanbericht erstellen, der die Zeitdauer berechnet.

Wenn der Benutzer in seinem Profil mit einer Rate der Kosten pro Stunde verknüpft ist, können Sie auch die Kosten für die Überstunden dieses Benutzers berechnen.\
Informationen zum Verknüpfen von Benutzern mit den Kosten pro Stunde finden Sie im Artikel [Meine Einstellungen konfigurieren](../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md).

>[!NOTE]
>
>Das Feld Überstunden , das Sie einer Timesheet-Ansicht in einer Liste oder einem Bericht hinzufügen können, zeigt die im Feld Überstunden des Zeitplans enthaltenen Informationen an. Diese Informationen werden von einem Benutzer, der Zugriff auf die Änderung des Zeitblatts hat, manuell aktualisiert. Weitere Informationen zum Feld &quot;Zeitüberschreitung&quot;in einem Zeitblatt finden Sie im Artikel [Übersicht über das Zeitblatt-Layout](../../../timesheets/timesheets/timesheet-layout.md).

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
   <td> <p>Anforderung zum Ändern einer Ansicht </p>
   <p>Berichtänderung planen</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf Berichte, Dashboards und Kalender bearbeiten, um einen Bericht zu ändern</p> <p>Zugriff auf Filter, Ansichten und Gruppierungen bearbeiten, um eine Ansicht zu ändern</p> <p><b>NOTIZ</b>

Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Berechtigungen für einen Bericht verwalten</p> <p>Weitere Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Anfordern des Zugriffs auf Objekte </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Berechnung der Überstunden in einer Timesheet-Ansicht

So fügen Sie einer Timesheet-Ansicht eine Spalte für die berechnete Zeitdauer hinzu:

1. Gehen Sie zu einer Liste von Timesheets oder erstellen Sie einen Timesheet-Bericht.

   Informationen zum Erstellen von Berichten finden Sie im Artikel [Benutzerspezifischen Bericht erstellen](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. Klicken Sie in einer Liste mit Timesheets auf **Ansicht anpassen** .

   Oder

   Wählen Sie die Registerkarte **Spalten (Ansicht)** in einem Zeitblatt-Bericht aus.

1. Klicken Sie auf **Spalte hinzufügen**.
1. Klicken Sie auf **Wechseln zum Textmodus**.
1. Klicken Sie im Bereich **In dieser Spalte anzeigen** auf **Klicken, um Text zu bearbeiten**.
1. Kopieren Sie den folgenden Textmoduscode und fügen Sie ihn im Dialogfeld **Textmodus** ein.
   <pre>displayName=Calculated Overtime Cost<br>linkedname=direct<br>namekey=totalHours<br>querysort=totalHours <br>textmode=true<br>valueExpression=IF({totalHours}&gt;40,({totalHours}-40)*{user}.{costPerHour}, {totalHours}*{user}.{costPerHour})<br>valueFormat=currencyStringCurrencyRounded</pre>

   >[!NOTE]
   >
   >Bei dieser Berechnung wird davon ausgegangen, dass der Benutzer normalerweise eine Woche mit 40 Stunden arbeitet.

1. Klicken Sie auf &quot;**Speichern**&quot;, geben Sie der neuen Ansicht einen Namen und klicken Sie in einer Liste mit Zeitleisten auf &quot;**Ansicht speichern**&quot;.

   Oder

   Klicken Sie in einem Timesheet-Bericht auf **Speichern + Schließen** .

1. (Optional und bedingt) Wenn Sie einen Timesheet-Bericht erstellen, geben Sie einen Namen für den Bericht ein und klicken Sie dann auf **Bericht speichern**.

   Die Kosten der Überstunden der einzelnen Benutzer werden in der Spalte **Berechnete Überstunden-Kosten** angezeigt.

   ![calculated_overtime_cost_in_timesheet_report.png](assets/calculated-overtime-cost-in-timesheet-report-350x92.png)
