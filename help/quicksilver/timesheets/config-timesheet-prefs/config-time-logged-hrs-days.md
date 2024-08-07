---
product-area: timesheets;setup
navigation-topic: configure-timesheet-preferences
title: Konfigurieren, ob die Zeit in Stunden oder Tagen protokolliert wird
description: Als Benutzer mit einer Planungslizenz können Sie konfigurieren, ob Sie die Zeit in Adobe Workfront in Stunden oder Tagen anmelden. Systemadministratoren können diese Einstellung für einzelne Benutzer oder für mehrere Benutzer in ihrer Organisation konfigurieren. Standardmäßig protokollieren Benutzer die Zeit in Stunden.
author: Alina
feature: Timesheets
exl-id: 4f801a13-182d-4e06-98ea-f6863f6a8edf
source-git-commit: b4ab350af22afa44774f06d82daf1c3fb266d2b9
workflow-type: tm+mt
source-wordcount: '451'
ht-degree: 1%

---

# Konfigurieren, ob die Zeit in Stunden oder Tagen protokolliert wird

Als Benutzer mit einer Planner-Lizenz können Sie konfigurieren, ob Sie die Zeit in Adobe Workfront in Stunden oder Tagen anmelden. Systemadministratoren können diese Einstellung für einzelne Benutzer oder für mehrere Benutzer in ihrer Organisation konfigurieren. Standardmäßig protokollieren Benutzer die Zeit in Stunden. Informationen zur Protokollzeit in Workfront finden Sie unter [Protokollzeit](../../timesheets/create-and-manage-timesheets/log-time.md).

>[!NOTE]
>
>Es wird empfohlen, die Protokollierungszeit in der gesamten Organisation auf die gleiche Weise (entweder Stunden oder Tage) zu verwenden, um die Genauigkeit der Berichterstellung sicherzustellen.

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Planer können Zeit für sich selbst konfigurieren. Nur ein Workfront-Administrator kann die Zeit für andere Benutzer konfigurieren.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

1. Führen Sie je nach Ziel und Zugriffsstufe im System einen der folgenden Schritte aus:

   * **Planen Sie den Benutzer beim Konfigurieren der Zeitprotokollierung für sich selbst:** Klicken Sie auf das Symbol **Hauptmenü** ![](assets/main-menu-icon.png) oben rechts in Adobe Workfront und klicken Sie dann auf Ihren Benutzernamen neben Ihrem Profilbild. Klicken Sie dann auf das Symbol **Mehr** neben Ihrem Namen und wählen Sie **Bearbeiten** aus.

   * **Systemadministrator, der die Zeitprotokollierung für andere konfiguriert:** Beginnen Sie mit der Bearbeitung eines oder mehrerer Benutzerkonten, wie in [Profil eines Benutzers bearbeiten](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md) beschrieben.

1. Suchen Sie im daraufhin angezeigten Dialogfeld im Abschnitt **Ressourcenplanung** die Option **Log Time in** .

   ![](assets/new-timesheet-log-hours-350x249.png)

1. (Bedingt) Wenn Sie ein Systemadministrator sind, der mehrere Benutzer gleichzeitig bearbeitet, wählen Sie **Protokollzeit in** aus.
1. Wählen Sie aus den folgenden Optionen für die Protokollierungszeit aus:

   | Option | Beschreibung |
   |---|---|
   | **Stunden** | Benutzer geben Stunden bei der Protokollierung in Workfront an. |
   | **Tage** | Benutzer geben Tage bei der Protokollierung in Workfront an. |

1. (Bedingt) Wenn Sie die Protokollzeit in Tagen ausgewählt haben, geben Sie im Feld **Entsprechende Stunden für vollständige Workday** die Anzahl der Stunden ein, die einem vollen Tag entsprechen. Ein Tag auf dem Timesheet eines Benutzers entspricht der Anzahl der Stunden, die Sie hier eingeben.

   Beachten Sie beim Konfigurieren dieser Einstellung Folgendes:

   * Diese Option ist nicht verfügbar, wenn konfiguriert wird, die Uhrzeit in Stunden zu protokollieren.
   * Diese Option wird nur zum Zwecke der Protokollierung verwendet. Diese Option steht nicht in Zusammenhang mit der Option **Zeitplan** , die auch beim Bearbeiten eines Benutzers verfügbar ist. Die Option **Zeitplan** wird bei der Berechnung von Zeitleisten und in anderen Bereichen von Workfront verwendet. (Weitere Informationen zur Verwendung der Option **Zeitplan** finden Sie unter [Zeitplan erstellen](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).) 

1. Klicken Sie auf **Änderungen speichern**.
