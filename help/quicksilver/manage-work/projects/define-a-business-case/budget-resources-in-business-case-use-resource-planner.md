---
navigation-topic: business-case-and-scorecards
title: Budgetressourcen im Business Case mit dem Ressourcenplaner
description: Im Rahmen der Ressourcenplanung können Sie mit dem Ressourcenplaner auf Projektebene die Aufgabengebiete budgetieren, die zum Abschließen der Arbeit in einem Projekt beim Erstellen des Business Case erforderlich sind.
author: Alina
feature: Work Management
exl-id: 51ebb940-111c-442f-a8a6-287a04d2db68
source-git-commit: f97c989f57d864252adf6e24f8e6b03f56d26901
workflow-type: tm+mt
source-wordcount: '1240'
ht-degree: 0%

---

# Budgetressourcen im Business Case mit dem Ressourcenplaner

<!--Audited: 06/2025-->

Im Rahmen der Ressourcenplanung können Sie mit dem Ressourcenplaner auf Projektebene die Aufgabengebiete budgetieren, die zum Abschließen der Arbeit in einem Projekt beim Erstellen des Business Case erforderlich sind.

Weitere Informationen zum Erstellen eines Business-Case finden Sie unter [Erstellen eines Business-Case für ein Projekt](../../../manage-work/projects/define-a-business-case/create-business-case.md).

>[!TIP]
>
>Die Informationen, die Sie im Ressourcenplaner auf Projektebene eingeben, sind auch im Ressourcenplaner auf Systemebene sichtbar. Auch das Gegenteil ist wahr. Weitere Informationen zum Ressourcenplaner finden Sie unter [Ressourcenplaner - Übersicht](../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

Sie können Ressourcen auch im Business Case mit dem Adobe Workfront-Szenarioplaner budgetieren. Weitere Informationen finden Sie unter [Budgetressourcen im Business Case mit dem Szenario-Planer](../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case-use-scenario-planner.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-Plan*</p></td> 
   <td> <p>Aktuell: Prime oder höher</p>
   <p>Legacy: Pro oder höher</p> 
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-Lizenz*</p></td> 
   <td> <p>Strom: Licht oder höher</p>
   <p>Legacy: Überprüfung oder höher</p>

<p><b>WICHTIG:</b></p> 
   <p>Aktuell: Sie müssen über eine Standardlizenz verfügen, um die Informationen zur Ressourcenbudgetierung zu ändern. </p> 
   <p>Legacy: Sie müssen über eine Planlizenz verfügen, um die Informationen zur Ressourcenbudgetierung zu ändern. </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Konfigurationen der Zugriffsebene</p></td> 
   <td> <p>Zugriff auf Folgendes bearbeiten: </p> 
    <ul> 
     <li> <p>Projekte</p> </li> 
     <li> <p>Ressourcenverwaltung</p> </li> 
     <li> <p>Finanzielle Daten</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Objektberechtigungen</p></td> 
   <td> <p>Verwalten von Berechtigungen für das Projekt</p> </td> 
  </tr> 
 </tbody> 
</table>

*Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Voraussetzungen

Bevor Sie beginnen, müssen Sie Folgendes tun:

* Erfüllen Sie alle Voraussetzungen für die Ressourcenplanung in Adobe Workfront. Weitere Informationen finden Sie unter [Ressourcenplaner - Übersicht](../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

* Verknüpfen Sie Ressourcenpools mit dem Projekt.

  <!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:(you must have tasks assigned to job roles and users on the project - this is optional because the users and their roles come from the pools))</p>
  -->

  >[!NOTE]
  >
  >Sie können keine Ressourcen budgetieren, die Problemen im Business Case zugewiesen sind. Sie können sie im Ressourcenplaner auf Systemebene budgetieren. Weitere Informationen zum Ressourcenplaner finden Sie unter [Ressourcenplaner - Übersicht](../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

* Obwohl dies keine Voraussetzung ist, empfehlen wir Ihnen auch, die geplanten Stunden für die Aufgaben im Projekt anzugeben. Auf diese Weise lässt sich erkennen, wie viel Arbeit eine Aufgabe ggf. abschließen muss. Dies erleichtert die Entscheidung, wie viel Zeit die Ressourcen in Anspruch nehmen sollen, um die Aufgabe abzuschließen. Informationen zum Verknüpfen von Aufgaben mit geplanten Stunden finden Sie unter [Aufgaben bearbeiten](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

## Anwenden von Ressourcenpools auf ein Projekt und Budgetressourcen im Business Case

>[!IMPORTANT]
>
>Sie können Ihre Ressourcen für einen Zeitraum von 15 Jahren budgetieren. Wenn Sie Ressourcen für ein Projekt mit einer Laufzeit von mehr als 15 Jahren budgetieren, sind die Budgetierungsinformationen möglicherweise nicht korrekt.

So wenden Sie Ressourcenpools und Budgetprojektressourcen im Business Case auf ein Projekt ohne Ressourcenpool an:

1. Wechseln Sie zu dem Projekt, für das Sie Ressourcen budgetieren möchten.
1. Klicken Sie **linken Bedienfeld** Business Case“.
1. (Bedingt) Wenn Ihr Unternehmen nicht über eine Lizenz für den Workfront-Szenarioplaner verfügt, klicken Sie **Ressourcenbudgetierung bearbeiten** im Abschnitt **Ressourcenbudgetierung** und fahren Sie dann mit Schritt 5 fort.

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode,QuicksilverOrClassic.Quicksilver">(NOTE: ensure it stays right - this is 5 instead of 6 because step 2 won't print for nwe)</p>
   -->

1. (Optional und bedingt) Wenn die Projektinformationen von einer Initiative im Szenario-Planer veröffentlicht wurden, führen Sie einen der folgenden Schritte aus:

   * Wählen Sie Ressourcenplaner im Feld **Wählen Sie die Stunden aus, die zur Berechnung der budgetierten Lohnkosten des Projekts verwendet werden sollen** und klicken Sie dann auf **Wählen > Ressourcenbudgetierung bearbeiten**.

     ![Business Case im Ressourcenplaner](assets/business-case-rp-selected-with-choose-button-350x120.png)

   * Wenn der Szenario-Planer für die Budgetierung von Ressourcen für das Projekt ausgewählt wurde, klicken Sie auf **Ändern** > **Ressourcenbudgetierung bearbeiten**.

     ![Business Case im Szenario-Planer](assets/business-case-sp-selected-change-option-to-switch-to-rp-highlighted-350x88.png)

   Hierbei werden die budgetierten Stunden des Projekts verwendet, um die budgetierten Lohnkosten für das Projekt zu berechnen.

   Der Szenario-Planer ist nur in der neuen Adobe Workfront-Version verfügbar und erfordert eine zusätzliche Lizenz. Weitere Informationen zum Workfront-Szenarioplaner finden Sie unter [Szenarioplaner - Übersicht](../../../scenario-planner/scenario-planner-overview.md).

   >[!NOTE]
   >
   >Es wird empfohlen, dass Sie bei Beginn der Arbeit an einem Projekt entscheiden, ob Sie den Ressourcen- oder den Szenario-Planer verwenden. Wenn Sie während der Laufzeit eines Projekts häufig zwischen beiden wechseln, kann dies zu Inkonsistenzen in der Budgetierung Ihrer Ressourcen für das Projekt führen.

1. Geben **im Feld „Ressourcenpool auswählen** einen oder mehrere **Ressourcenpools** an.

   Sie dürfen nur Ressourcenpools angeben, die mit aktiven Benutzern gefüllt sind.

   >[!TIP]
   >
   >Wenn das Projekt bereits mit Ressourcenpools verknüpft ist, wird der Ressourcenplaner standardmäßig angezeigt. Um dem Projekt weitere Ressourcenpools hinzuzufügen, bearbeiten Sie das Projekt. Informationen zum Bearbeiten eines Projekts finden Sie unter [Projekte bearbeiten](../../../manage-work/projects/manage-projects/edit-projects.md).

1. Klicken Sie **Apply**.

   Der Ressourcenplaner wird für das ausgewählte Projekt angezeigt.

   Standardmäßig werden die ersten 20 Aufgabengebiete, die mit diesem Projekt verknüpft sind, im Abschnitt Ressourcenbudgetierung in alphabetischer Reihenfolge aufgeführt. 

   Weitere Informationen zum Ressourcenplaner finden Sie unter [Ressourcenplaner - Übersicht](../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

   ![BC_resource_budgeting_area.png](assets/bc-resource-budgeting-area-350x276.png)

1. (Optional und bedingt) Erweitern Sie die Aufgabengebiete, um die ihnen zugeordneten Benutzer anzuzeigen.

   >[!NOTE]
   >
   >Aktive Benutzer werden nur dann unter den ihnen zugeordneten Aufgabengebieten angezeigt, wenn sie die folgenden Kriterien erfüllen:
   >
   >   
   >   
   >   * Sie gehören zu einem der Ressourcenpools des Projekts.
   >   * Ihnen wurden budgetierte Stunden zugewiesen.
   >   * Sie sind mit einem der Aufgabengebiete des Projekts verknüpft.
   >   
   >

    

1. Klicken Sie **Heute**, um zum heutigen Zeitrahmen zurückzukehren.
1. (Optional) Klicken Sie auf **Woche**, **Monat** oder **Quartal**, um Informationen zum Projekt in verschiedenen Zeitrahmen anzuzeigen.
1. (Optional) Klicken Sie auf das **Stunden** Dropdown-Menü und wählen Sie **Stunden**, **FTE** oder **Kosten**, um die Anzeige von Informationen im Ressourcenplaner zu ändern. Standardmäßig werden Stunden angezeigt.

1. (Optional) Klicken Sie auf **Exportieren**, um den Ressourcenplaner in eine Excel-Datei zu exportieren.

   >[!NOTE]
   >
   >Sie können Daten für bis zu 12 Zeiträume gleichzeitig exportieren.

1. (Optional) Klicken Sie auf das **Vollbild**-Symbol ![full_screen_RP_in_BC.png](assets/full-screen-rp-in-bc.png), um den Ressourcenplaner im Vollbildmodus anzuzeigen.

1. Aktualisieren Sie das **BDG**-Feld (Budgetierte Stunden) mit Stunden-, FTE- oder Kostenwerten für die Benutzer, Funktionen oder das Projekt, indem Sie einen der folgenden Schritte ausführen:

   * Schätzen Sie die Anzahl der Stunden, FTE oder Kostenwerte für Funktionen, Benutzer oder das Projekt manuell.

     Oder

   * Klicken Sie auf **Optionen**-Symbol für das Projekt oder die Aufgabengebiete und wählen Sie eine Option aus, um die Stunden für Rollen, Benutzer oder das Projekt automatisch zu budgetieren.

   Weitere Informationen zur Budgetierung in der Projektansicht des Ressourcenplaners finden Sie unter [Budgetressourcen im Ressourcenplaner mithilfe der Projekt- und Aufgabenansichten](../../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md).

   >[!NOTE]
   >
   >Sie können Stunden, FTEs oder Kosten für Ihre Ressourcen für jeden Zeitrahmen budgetieren, der im Bereich Ressourcenbudgetierung angezeigt wird, unabhängig von der Zeitleiste des Projekts. Wenn Sie beispielsweise angeben möchten, dass Ihre Ressourcen möglicherweise nicht während der Zeitleiste des Projekts verfügbar sind (wo sie mit den geplanten Stunden verknüpft sind), aber möglicherweise während einer anderen Zeit verfügbar sind, können Sie dies tun, indem Sie sie für Zeitrahmen budgetieren, in denen die geplanten Stunden null sind, wenn diese für die Arbeit verfügbar werden.

1. (Optional) Um zu verstehen, ob Sie die budgetierten Stunden, FTEs oder Kosten in einen anderen Zeitrahmen verschieben können, klicken Sie auf das Symbol **Optionen** und dann **Budgetierungsdaten anpassen**.

   Weitere Informationen zum Anpassen budgetierter Termine finden Sie unter [Anpassen von Budgetierungsdaten im Ressourcenplaner](../../../resource-mgmt/resource-planning/adjust-budgeting-dates.md).

1. Klicken Sie auf **Speichern**.

   Wenn Sie mit Ihren Aufgabengebieten Stundensätze für Kosten pro Stunde verknüpft haben, berechnet die Budgetierung der Ressourcen im Bereich Ressourcenbudgetierung die **budgetierten Lohnkosten** des Projekts. Die budgetierten Lohnkosten werden im Bereich Ressourcenbudgetierung des Business Case und in der Business Case-Zusammenfassung angezeigt.

   >[!TIP]
   >
   >Kosten werden im Business Case in der Währung des Projekts angezeigt.

   Die im Business Case angegebenen Budgetierungsinformationen werden auch im Ressourcenplaner angezeigt.

   Wenn Sie ein Projekt kopieren, haben Sie die Möglichkeit, auch die budgetierten Stunden in das neue Projekt zu kopieren. Nur im Ressourcenplaner budgetierte Stunden werden kopiert. Weitere Informationen finden Sie unter [Kopieren eines Projekts](../manage-projects/copy-project.md).
