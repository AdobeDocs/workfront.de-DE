---
user-type: administrator
content-type: reference;overview
product-area: system-administration;setup;user-management
navigation-topic: configure-proofing-functionality
title: Zugriff auf die Proofing-Funktion in Workfront
description: Welche Proofing-Funktion Ihren Benutzern zur Verfügung steht, hängt davon ab, welchen Workfront-Plan Ihr Unternehmen erworben hat.
author: Courtney
feature: System Setup and Administration, Digital Content and Documents
role: Admin
exl-id: 30a41ae9-9755-4c7b-9e3b-d4a8b0ad7ee8
source-git-commit: ab774e937a15aaa04704e872579df880a9b80aaf
workflow-type: tm+mt
source-wordcount: '453'
ht-degree: 0%

---

# Zugriff auf die Proofing-Funktion in Workfront

Welche Proofing-Funktion Ihren Benutzern zur Verfügung steht, hängt davon ab, welchen Workfront-Plan Ihr Unternehmen erworben hat.

## Proofing in Workfront

Derzeit gibt es drei Planungsoptionen für das Proofing in Workfront:

* **Neue Workfront-Pläne**: In den neuen Workfront-Plänen wird automatisch ein Proofing für alle Lizenzen durchgeführt.
* **Aktuelle Workfront Pro+-Pläne**: Proofing ist automatisch für Arbeits- und Planlizenzen enthalten, wenn Sie die Pro-, Business- oder Enterprise Workfront-Pläne haben.
* **Legacy Workfront Premium-Pläne**: Diese Option ist für ältere Workfront-Pläne - Select, Enterprise, Premium. In diesem Plan ist das Proofing nicht automatisch mit Lizenzen enthalten. Sie müssen Proofing-Zugriff für bestimmte Benutzer in deren Benutzerprofil gewähren.

  Wenn Sie Workfront-Administrator sind, können Sie unter Einrichtung > System > Lizenzen prüfen, welchen Plan Ihre Instanz verwendet.

### Proofing-Funktionen in Workfront

Informationen zum Gewähren und Sperren des Benutzerzugriffs auf das Erstellen und Anzeigen von Korrekturabzügen in Workfront finden Sie [Konfigurieren des Korrekturabzugszugriffs einer Benutzerin bzw. eines Benutzers](../../../administration-and-setup/manage-workfront/configure-proofing/configure-a-users-proofing-access.md).

* Erstellen Sie statische oder interaktive Korrekturabzüge für nach außen gerichtete URLs und Dokumente. Weitere Informationen finden Sie unter [Testsendungen erstellen](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-proofs-in-wf.md).
* Automatisierte Workflows in Korrekturabzüge einbeziehen. Weitere Informationen finden Sie unter [Automatisierter Workflow - Übersicht](../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md).
* Zugriffs- und Abonnementeinstellungen für Korrekturabzüge festlegen. Weitere Informationen finden Sie unter [Konfigurieren von Zugriffs- und Abonnementeinstellungen für einen Korrekturabzug](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/configure-access-subscription-settings-proof.md).
* Weisen Sie benutzerdefinierte Berechtigungsprofile für Korrekturabzüge zu, wenn Sie die Korrekturabzugsfunktionen für einen Benutzer in Workfront aktivieren. Weitere Informationen finden Sie unter [Aktivieren und Deaktivieren des Proofings für Benutzende (nur für veraltete Pläne)](../../../administration-and-setup/manage-workfront/configure-proofing/configure-a-users-proofing-access.md#enabling-and-disabling-proofing-for-a-user) in [Konfigurieren des Proofing-Zugriffs für Benutzende](../../../administration-and-setup/manage-workfront/configure-proofing/configure-a-users-proofing-access.md).
* Verfolgen Sie den Fortschritt und Status des Testversands. Weitere Informationen finden Sie unter [Testversand-Fortschritt und Statusübersicht](../../../review-and-approve-work/proofing/proofing-overview/view-progress-status-proof.md).
* Legen Sie das Workfront Proof-Berechtigungsprofil beim Erstellen von Proofing-Benutzern in Workfront fest, wie in diesem Abschnitt beschrieben.

  Diese Profile wirken sich nur auf Berechtigungen in Workfront Proof aus, nicht auf Berechtigungen in Workfront.

* Vergleichen Sie zwei Korrekturabzüge oder zwei Versionen desselben Korrekturabzugs. Weitere Informationen finden Sie unter [Testsendungen vergleichen](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/compare-proofs.md).
* Erstellen eines Berichts zur Korrekturabzugsgenehmigung Weitere Informationen finden Sie unter [Erstellen eines benutzerdefinierten Berichts](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
* Zeigt die Korrekturphase an, die derzeit für jede Dokumentversion im Bericht Dokumentversion aktiv ist. Der Name des Schritts wird in der Spalte „Aktive Korrekturabzugsschritte“ angezeigt. Wenn derzeit kein Schritt in der Dokumentversion aktiv ist, ist die Spalte leer. Weitere Informationen zu den verfügbaren Feldern in Ansichten und Berichten finden Sie im [Glossar der Adobe Workfront-Terminologie](../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).
* Konfigurieren Sie, wann Testsendungen mit einem automatisierten Workflow für Benutzende sichtbar sind, die mit einem bestimmten Schritt verknüpft sind. Weitere Informationen finden Sie unter [Konfigurieren der Sichtbarkeit von Korrekturabzügen basierend auf der Workflow-](../../../administration-and-setup/manage-workfront/configure-proofing/configure-sharing-settings-users.md#configuring-proof-visibility-based-on-workflow-stage-activity)&quot; in [Konfigurieren von Freigabeeinstellungen für Ihre Benutzer](../../../administration-and-setup/manage-workfront/configure-proofing/configure-sharing-settings-users.md).
* Nahtloser Zugriff auf Workfront Proof direkt über die globale Navigationsleiste von Workfront (keine zusätzliche Anmeldung erforderlich). Weitere Informationen finden Sie unter [Zugriff auf Workfront Proof über Adobe Workfront](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/access-wf-proof-in-workfront.md).

<!--
>[!NOTE]
>
>There are some capabilities included in Workfront Proof standalone that are not included in Proofing in Workfront. To learn more, see [Standalone Workfront Proof to Integrated Proofing in Workfront overview](../../../administration-and-setup/manage-workfront/configure-proofing/move-to-proofing-in-workfront.md)
-->
