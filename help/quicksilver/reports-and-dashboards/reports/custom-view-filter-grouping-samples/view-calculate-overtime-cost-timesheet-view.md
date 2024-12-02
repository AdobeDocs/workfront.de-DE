---
content-type: reference
product-area: reporting;timesheets
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Ansicht: Berechnung der Zeitüberschreitungskosten in einer Timesheet-Ansicht'
description: Die Zeitüberschreitung wird in Adobe Workfront nicht standardmäßig berechnet, Sie können jedoch einen Zeitplanbericht erstellen, der die Zeitdauer berechnet.
author: Nolan
feature: Reports and Dashboards
exl-id: ad6205cd-7534-49e5-b142-09f90bf672ce
source-git-commit: ecce7484423419823effa2cb41da892ba3fb207c
workflow-type: tm+mt
source-wordcount: '359'
ht-degree: 0%

---

# Ansicht: Berechnung der Zeitüberschreitungskosten in einer Timesheet-Ansicht

<!--Audited: 11/2024-->

Die Zeitüberschreitung wird in Adobe Workfront nicht standardmäßig berechnet, Sie können jedoch einen Zeitplanbericht erstellen, der die Zeitdauer berechnet.

Wenn der Benutzer in seinem Profil mit einer Rate der Kosten pro Stunde verknüpft ist, können Sie auch die Kosten für die Überstunden dieses Benutzers berechnen.\
Informationen zum Verknüpfen von Benutzern mit den Kosten pro Stunde finden Sie im Artikel [Meine Einstellungen konfigurieren](../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md).

>[!NOTE]
>
>Das Feld Überstunden , das Sie einer Timesheet-Ansicht in einer Liste oder einem Bericht hinzufügen können, zeigt die im Feld Überstunden des Zeitplans enthaltenen Informationen an. Diese Informationen werden von einem Benutzer, der Zugriff auf die Änderung des Zeitblatts hat, manuell aktualisiert. Weitere Informationen zum Feld &quot;Zeitüberschreitung&quot;in einem Zeitblatt finden Sie im Artikel [Übersicht über das Zeitblatt-Layout](../../../timesheets/timesheets/timesheet-layout.md).

![calculated_overtime_cost_in_timesheet_report.png](assets/calculated-overtime-cost-in-timesheet-report-350x92.png)

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Abo</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> 
    <p>Neu:</p>
   <ul><li><p>Mitwirkende bei der Änderung eines Filters </p></li>
   <li><p>Standard zum Ändern eines Berichts</p></li> </ul>

<p>Aktuell:</p>
   <ul><li><p>Filteranforderung </p></li>
   <li><p>Berichtänderung planen</p></li> </ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Zugriff auf Berichte, Dashboards und Kalender bearbeiten, um einen Bericht zu ändern</p> <p>Zugriff auf Filter, Ansichten und Gruppierungen bearbeiten, um einen Filter zu ändern</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Berechtigungen für einen Bericht verwalten</p>  </td> 
  </tr> 
 </tbody> 
</table>

*Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Berechnung der Überstunden in einer Timesheet-Ansicht

So fügen Sie einer Timesheet-Ansicht eine Spalte für die berechnete Zeitdauer hinzu:

1. Gehen Sie zu einer Liste von Timesheets.

1. Klicken Sie auf das Dropdownmenü **Ansicht** und dann auf **Neue Ansicht**.

1. Klicken Sie auf **Spalte hinzufügen**.
1. Klicken Sie auf **Wechseln zum Textmodus** und dann auf **Textmodus bearbeiten**.
1. Entfernen Sie im Feld **Textmodus bearbeiten** den Text im Feld, kopieren Sie dann den folgenden Textmoduscode und fügen Sie ihn ein:

   ```
   displayname=Calculated Overtime Cost
   linkedname=direct
   namekey=totalHours
   querysort=totalHours 
   textmode=true
   valueexpression=IF({totalHours}>40,({totalHours}-40)*{user}.{costPerHour},{totalHours}*{user}.{costPerHour})
   valueformat=currencyStringCurrencyRounded
   ```

   >[!NOTE]
   >
   >Bei dieser Berechnung wird davon ausgegangen, dass der Benutzer normalerweise eine Woche mit 40 Stunden arbeitet.

1. Klicken Sie auf **Fertig**, geben Sie der neuen Ansicht einen Namen und klicken Sie in einer Liste mit Timesheets auf **Ansicht speichern** .

   Die Kosten der Überstunden der einzelnen Benutzer werden in der Spalte **Berechnete Überstunden-Kosten** angezeigt.


