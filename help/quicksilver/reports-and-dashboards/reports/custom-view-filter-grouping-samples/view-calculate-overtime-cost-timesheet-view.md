---
content-type: reference
product-area: reporting;timesheets
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Ansicht: Überstundenkosten in einer Arbeitszeittabellen-Ansicht berechnen'
description: In Adobe Workfront werden Überstunden nicht standardmäßig berechnet. Sie können jedoch einen Arbeitszeittabellen-Bericht erstellen, der die Überstunden berechnet.
author: Nolan
feature: Reports and Dashboards
exl-id: ad6205cd-7534-49e5-b142-09f90bf672ce
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '345'
ht-degree: 1%

---

# Ansicht: Überstundenkosten in einer Arbeitszeittabellen-Ansicht berechnen

<!--Audited: 11/2024-->

In Adobe Workfront werden Überstunden nicht standardmäßig berechnet. Sie können jedoch einen Arbeitszeittabellen-Bericht erstellen, der die Überstunden berechnet.

Wenn der/die Benutzende in seinem/ihrem Profil einem Stundensatz zugeordnet ist, können Sie auch den Kostenbetrag für die Überstunden dieses/r Benutzenden berechnen.\
Informationen zur Zuordnung von Kosten pro Stunde zu Benutzerinnen und Benutzern finden Sie im Artikel [Konfigurieren meiner Einstellungen](../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md).

>[!NOTE]
>
>Das Feld Überstunden , das Sie einer Arbeitszeittabellen-Ansicht in einer Liste oder einem Bericht hinzufügen können, zeigt die Informationen im Feld Überstunden der Arbeitszeittabelle an. Diese Informationen werden manuell von einem Benutzer aktualisiert, der Zugriff hat, um die Arbeitszeittabelle zu ändern. Weitere Informationen zum Feld „Überstunden“ in einer Arbeitszeittabelle finden Sie im Artikel [Arbeitszeittabellen-Layout - Übersicht](../../../timesheets/timesheets/timesheet-layout.md).

![calculated_overtime_cost_in_timesheet_report.png](assets/calculated-overtime-cost-in-timesheet-report-350x92.png)

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen. 

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
   <p>Mitwirkender oder Anfrage zum Ändern eines Filters </p>
   <p>Standard oder Plan zum Ändern eines Berichts</p>
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriff auf Berichte, Dashboards und Kalender bearbeiten, um einen Bericht zu ändern</p> <p>Zugriff auf Filter, Ansichten, Gruppierungen bearbeiten, um einen Filter zu ändern</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Verwalten von Berechtigungen für einen Bericht</p>  </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).
+++

## Überstundenkosten in einer Arbeitszeittabellen-Ansicht berechnen

So fügen Sie einer Arbeitszeittabellen-Ansicht eine berechnete Spalte für Überstunden hinzu:

1. Zu einer Liste von Arbeitszeittabellen wechseln.

1. Klicken Sie auf **Dropdown** Menü Ansicht und dann auf **Neue Ansicht**.

1. Klicken Sie auf **Spalte hinzufügen**.
1. Klicken Sie **Wechseln Sie in den Textmodus** und klicken Sie dann auf **Textmodus bearbeiten**.
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
   >Bei dieser Berechnung wird davon ausgegangen, dass der/die Benutzende normalerweise eine 40-Stunden-Woche arbeitet.

1. Klicken Sie **Fertig** benennen Sie dann die neue Ansicht und klicken Sie **Ansicht speichern** in einer Liste von Arbeitszeittabellen.

   Die Kosten der Überstunden jedes/r Benutzenden werden in der Spalte **Berechnete Überstundenkosten** angezeigt.


