---
product-area: projects
navigation-topic: create-projects
title: Erstellen von Projektgrundlagen
description: Eine Grundlinie ist ein Projekt-Schnappschuss, der wichtige Informationen darstellt, die im ursprünglichen Projektplan oder zu einem bestimmten Zeitpunkt während der Laufzeit des Projekts enthalten sind.
author: Alina
feature: Work Management
exl-id: 422bd7a5-d7a0-4c24-8624-bd0fe6e79d7b
source-git-commit: bbd64e9deed1b89d720272508b3562c354578704
workflow-type: tm+mt
source-wordcount: '810'
ht-degree: 0%

---

# Erstellen von Projektgrundlagen

Eine Grundlinie ist ein Projekt-Schnappschuss, der wichtige Informationen darstellt, die im ursprünglichen Projektplan oder zu einem bestimmten Zeitpunkt während der Laufzeit des Projekts enthalten sind.

Sie können die Grundlinie verwenden, um diese Informationen aus dem aktuellen Plan mit dem ursprünglichen Plan oder einem anderen Zeitpunkt zu vergleichen, um Problemaufgaben, Schlupflöcher und andere Trends im Zeitverlauf zu identifizieren.

## Zugriffsanforderungen

<!--
drafted for P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Standard </p> 
   Or
   <p>Legacy license: Plan </p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level*</td> 
   <td> <p>Edit access to Projects</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information about access to projects, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md" class="MCXref xref">Grant access to projects</a>. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View permissions to the project or higher to view baselines</p> <p>Manage permissions to the project to create baselines</p> <p> For information about project permissions, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Share a project in Adobe Workfront</a>.</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Zugriffsebene*</td> 
   <td> <p>Zugriff auf Projekte bearbeiten</p> <p><b>NOTE</b>
   Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen zum Zugriff auf Projekte finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md" class="MCXref xref">Projektzugriff gewähren</a>. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsstufe ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Berechtigungen für das Projekt oder höher anzeigen, um Grundlinien anzuzeigen</p> <p>Verwalten von Berechtigungen für das Projekt zum Erstellen von Grundlinien</p> <p> Weitere Informationen zu Projektberechtigungen finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Freigeben eines Projekts in Adobe Workfront</a>.</p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Überlegungen zum Arbeiten mit Grundlinien

* Sie können während der Projektlaufzeit mehrmals eine Momentaufnahme des Projektfortschritts erstellen und dabei mehrere Grundlinien erstellen.
* Sie können die in den Grundlinien eines Projekts enthaltenen Informationen anzeigen, indem Sie eine Grundlinie erstellen oder einen Baseline-Bericht erstellen.
* Wenn Sie eine Grundlinie erstellen, werden die Aufgabeninformationen auch in den Grundaufgaben dieser Grundlinie erfasst.
* Sie können die Informationen zu den Grundaufgaben anzeigen, indem Sie einen Baseline-Aufgabenbericht erstellen.

>[!IMPORTANT]
>
>Eine Grundlinie erstellt eine Momentaufnahme des Namens, der Daten und der finanziellen Informationen des Projekts. Die Grundlinie enthält nicht die Werte von benutzerdefinierten Feldern im Projekt. Informationen zu den Finanzinformationen, die in der Grundlinie enthalten sind, finden Sie unter [Projektfinanzen in Projektgrundlagen](../../../manage-work/projects/project-finances/project-finances-included-in-project-baselines.md).

## Erstellen einer Grundlinie

Sie können eine Grundlinie wie folgt erstellen:

* **Automatisch**: Ihr Workfront-Administrator oder Gruppenadministrator legt die Projektvoreinstellung für Workfront fest, um automatisch eine Grundlinie zu erstellen, sobald ein Projekt aktuell wird. Wenn diese Einstellung aktiviert ist, wird eine Grundlinie erstellt, sobald der Projektstatus &quot;Aktuell&quot;wird. Wenn diese Einstellung nicht aktiviert ist, müssen Sie Grundlinien manuell erstellen.

   Weitere Informationen zum Konfigurieren von Projektvoreinstellungen und zum Einrichten der automatischen Grundlagenerstellung finden Sie unter [Systemweite Projektvoreinstellungen konfigurieren](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

   >[!CAUTION]
   >
   >Durch Aktivierung dieser Einstellung wird automatisch eine Grundlinie für ein Projekt erstellt, sobald sich der Status eines Projekts in &quot;Aktuell&quot;ändert. Die erste erstellte Grundlinie ist die Standardgrundlinie. Sie müssen während der Projektlaufzeit alle anderen Grundlinien manuell erstellen .

* **Manuell**: Sie können nach Bedarf neue Grundlinien für das Projekt erstellen, während das Projekt weitergeht. Anschließend können Sie die Grundlinien vergleichen, um zu sehen, wie das Projekt im Laufe der Zeit vorangeschritten ist.

So erstellen Sie eine Grundlinie:

1. Navigieren Sie zu einem Projekt.
1. Klicken Sie im linken Bereich auf **Grundlinien**.

   Oder

   Klicken **Mehr anzeigen** Klicken Sie auf **Grundlinien**.

   ![](assets/nwe-baselines-section-on-project-with-header-350x78.png)

1. Klicken **Neue Grundlinie.**
1. Geben Sie den Namen für die Grundlinie an.
1. (Optional) Wenn dies die erste Grundlinie ist, können Sie sie als Standard auswählen.
1. Klicken Sie auf **Speichern**.

   Standardmäßig werden die folgenden Informationen zur von Ihnen erstellten Grundlinie angezeigt:

   * Baseline-Name
   * Basiseintragsdatum
   * Geplantes Anfangsdatum des Projekts, an dem die Grundlinie erstellt wurde
   * Voraussichtlicher Projektbeginn Datum der Erstellung der Grundlinie
   * Tatsächliche Projektdauer bei der Erstellung der Grundlinie
   * % Abschluss des Projekts bei Erstellung der Grundlinie
   * Standardindikator für die Grundlinie, der anzeigt, ob eine Grundlinie die Standardgrundlinie des Projekts ist

      >[!TIP]
      >
      >Es ist nicht möglich, Informationen aus zwei Grundlinien gleichzeitig in derselben Ansicht oder demselben Bericht anzuzeigen. Sie können nur Informationen aus einer bestimmten Grundlinie und der Standardgrundlinie im selben Bericht anzeigen. Sie können jederzeit während der Laufzeit des Projekts ändern, welche Grundlinie Sie als Standardgrundlinie betrachten.

1. (Optional) Klicken Sie neben der Ansicht auf den Dropdownpfeil und anschließend **Ansicht anpassen** , um Ihrer Ansicht Felder hinzuzufügen und zusätzliche Informationen zwischen Grundlinien zu vergleichen.

## Erstellen eines Baseline- oder Baseline-Aufgabenberichts

Um Basisinformationen anzuzeigen, können Sie auch einen Baseline- oder Baseline-Aufgabenbericht erstellen. Auf diese Weise können Sie eine beliebige Anzahl von Feldern über die Grundlinien oder Grundlinien-Aufgaben anzeigen, um sie in einer Ansicht zu vergleichen.

>[!TIP]
>
>Sie müssen eine Grundlinie erstellen, bevor Sie einen Baseline- oder Baseline-Aufgabenbericht erstellen können.

Informationen zum Erstellen eines Berichts finden Sie unter [Benutzerdefinierten Bericht erstellen](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

Es wird empfohlen, dem Bericht &quot;Grundlinie&quot;oder &quot;Grundlinie&quot;eine Gruppierung &quot;Projektname&quot;hinzuzufügen, um das Lesen zu vereinfachen.

Informationen zum Erstellen einer Gruppierung finden Sie unter [Erstellen von Gruppierungen in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/create-groupings.md).
