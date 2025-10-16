---
product-area: timesheets;setup
navigation-topic: configure-timesheet-preferences
title: Konfigurieren, ob die Zeit in Stunden oder Tagen protokolliert wird
description: Als Anwender mit Planlizenz können Sie konfigurieren, ob Sie die Zeit in Adobe Workfront in Stunden oder Tagen protokollieren. Systemadministratoren können diese Einstellung für einzelne Benutzer oder für mehrere Benutzer in ihrer Organisation konfigurieren. Standardmäßig protokollieren Benutzer die Zeit in Stunden.
author: Lisa
feature: Timesheets
exl-id: 4f801a13-182d-4e06-98ea-f6863f6a8edf
source-git-commit: b0a3a11a3c04a0969bee99f8e1cea231911f0e6a
workflow-type: tm+mt
source-wordcount: '457'
ht-degree: 1%

---

# Konfigurieren, ob die Zeit in Stunden oder Tagen protokolliert wird

Als Benutzer mit einer Standard- oder Planlizenz können Sie konfigurieren, ob Sie die Zeit in Adobe Workfront in Stunden oder Tagen protokollieren. Systemadministratoren können diese Einstellung für einzelne Benutzer oder für mehrere Benutzer in ihrer Organisation konfigurieren. Standardmäßig protokollieren Benutzer die Zeit in Stunden. Informationen zum Protokollieren der Zeit in Workfront finden Sie unter [Zeit protokollieren](../../timesheets/create-and-manage-timesheets/log-time.md).

>[!NOTE]
>
>Es wird empfohlen, die Zeit im gesamten Unternehmen auf die gleiche Weise zu protokollieren, entweder Stunden oder Tage, um die Genauigkeit des Reportings sicherzustellen.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

<table style="table-layout:auto">
 <col> 
 <col>
 <tbody> 
  <tr> 
   <td>Adobe Workfront-Paket</td> 
   <td><p>Beliebig</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront-Lizenz</td> 
   <td>
   <p>Standard</p>
   <p>Plan</p></td>
  </tr> 
  <tr> 
   <td>Konfigurationen der Zugriffsebene</td> 
   <td><p>Standard- und Planbenutzer können die Zeit selbst konfigurieren. Nur ein Workfront-Administrator kann Zeit für andere Benutzer konfigurieren.</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

1. Führen Sie je nach Ziel und Zugriffsebene im System einen der folgenden Schritte aus:

   * **Standard- oder Planen Sie, wie Sie die Zeiterfassung für sich selbst konfigurieren** Klicken Sie oben rechts in Adobe Workfront auf das **[!UICONTROL Hauptmenü]**-Symbol ![Hauptmenü](assets/main-menu-icon.png) und klicken Sie dann auf Ihren Benutzernamen neben Ihrem Profilbild. Oder (falls verfügbar) klicken Sie auf Ihr Profilbild im oberen Navigationsbereich und dann auf **[!UICONTROL Workfront-Profil]**. Klicken Sie dann auf das Symbol **Mehr** neben Ihrem Namen und wählen Sie **Bearbeiten** aus.

   * **Systemadministrator, der die Zeitprotokollierung für andere konfiguriert** Beginnen Sie mit der Bearbeitung eines oder mehrerer Benutzerkonten, wie [Bearbeiten des Benutzerprofils](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md) beschrieben.

1. Suchen Sie im daraufhin angezeigten Dialogfeld im Abschnitt **Ressourcenplanung** die Option **Zeit erfassen**.

   ![Zeit in Optionen erfassen](assets/user-profile-log-time-options.png)

1. Wählen Sie aus den folgenden Optionen für die Zeitprotokollierung aus:

   | Option | Beschreibung |
   |---|---|
   | **Stunden** | Benutzende geben Stunden zum Protokollieren der Zeit in Workfront an. |
   | **Tage** | Benutzende geben Tage für die Zeitprotokollierung in Workfront an. |

1. (Bedingt) Wenn Sie die Zeit in Tagen protokollieren möchten, geben Sie in das Feld **Äquivalente Stunden für vollständige Workday** die Anzahl der Stunden ein, die einem ganzen Tag entsprechen. Ein Tag auf der Arbeitszeittabelle eines Benutzers entspricht der Anzahl der Stunden, die Sie hier eingeben.

   Beachten Sie beim Konfigurieren dieser Einstellung Folgendes:

   * Diese Option ist beim Konfigurieren von für die Zeiterfassung in Stunden nicht verfügbar.
   * Diese Option wird nur zum Protokollieren der Zeit verwendet. Diese Option bezieht sich nicht auf die Option **Zeitplan**, die auch beim Bearbeiten eines Benutzers verfügbar ist. Die **Zeitplan**-Option wird bei der Berechnung von Timelines und in anderen Bereichen von Workfront verwendet. (Weitere Informationen zur Verwendung der Option **Zeitplan** finden Sie unter [Erstellen eines Zeitplans](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).) 

1. Klicken Sie auf **Änderungen speichern**.
