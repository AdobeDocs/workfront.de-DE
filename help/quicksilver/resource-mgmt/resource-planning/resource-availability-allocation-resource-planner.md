---
product-area: resource-management
navigation-topic: resource-planning
title: Ressourcenverfügbarkeit und -zuordnung mit dem Adobe Workfront-Ressourcenplaner überprüfen
description: Sie können die Verfügbarkeit Ihrer Ressourcen und den Umfang der geplanten oder budgetierten Arbeit für Ihre Projekte im Ressourcenplaner anzeigen. Diese Werte werden in Stunden, FTE (Vollzeitäquivalent) oder Kostenbeträgen angezeigt und in Spalten organisiert.
author: Lisa
feature: Resource Management
exl-id: 5b3e52a6-af9b-4e68-8d6e-43a5151a2a2c
source-git-commit: 987b6e9b5f6b1feb323906cf7c24f5024fc84663
workflow-type: tm+mt
source-wordcount: '1199'
ht-degree: 5%

---

# Ressourcenverfügbarkeit und -zuordnung mit dem Adobe Workfront-Ressourcenplaner überprüfen

Sie können die Verfügbarkeit Ihrer Ressourcen und den Umfang der geplanten oder budgetierten Arbeit für Ihre Projekte im Ressourcenplaner anzeigen. Diese Werte werden in Stunden, FTE (Vollzeitäquivalent) oder Kostenbeträgen angezeigt und in Spalten organisiert.

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
   <td><p>Licht oder höher</p>
       <p>Überprüfen oder höher</p></td>
  </tr> 
  <tr> 
   <td>Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriff auf Folgendes anzeigen oder höher:</p> 
    <ul> 
     <li> <p>Ressourcenverwaltung</p> </li> 
     <li> <p>Finanzielle Daten</p> </li> 
     <li> <p>Benutzende</p> </li> 
     <li> <p>Projekte</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Objektberechtigungen</td> 
   <td> <p>Zeigen Sie Berechtigungen oder höhere Berechtigungen für die Projekte an, die Sie im Ressourcenplaner anzeigen möchten</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Voraussetzungen

Sie müssen alle Voraussetzungen erfüllen, um mit dem Ressourcenplaner arbeiten zu können. Weitere Informationen finden Sie unter [Ressourcenplaner - Übersicht](../../resource-mgmt/resource-planning/get-started-resource-planner.md).

>[!IMPORTANT]
>
>Wenn eine der Voraussetzungen für die korrekte Funktionalität des Ressourcenplaners fehlt, können einige der Zahlen null sein oder die budgetierten Stunden werden abgeblendet.

## Verfügbarkeit und Zuweisung von Ressourcen

Die Spalten, die die Verfügbarkeit und Zuordnung Ihrer Ressourcen anzeigen, ändern sich je nachdem, welche Ansicht Sie auf den Ressourcenplaner anwenden. Informationen zum Anzeigen der Informationen im Ressourcenplaner nach Projekt, Rolle oder Benutzer finden Sie unter [Übersicht über die Ressourcenplaner-](../../resource-mgmt/resource-planning/resource-planner-navigation.md).

Beachten Sie beim Ändern Ihrer Ansicht in den Ressourcenplaner Folgendes:

* Wenn Sie die Ansichten **Nach Projekt anzeigen** oder **Nach Rolle anzeigen** anwenden, werden die folgenden Spalten angezeigt:

  <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  (NOTE: Alina: (some of the information in this area is also covered in Calculating Costs in the RP - https://workfront.zendesk.com/hc/en-us/articles/115004186433 - update this article also, when changes here occur)
  </MadCap:conditionalText>
  -->



   * Verfügbare Stunden, FTE oder Kosten
   * Geplante Stunden, FTE oder Kosten
   * Budgetierte Stunden, FTE oder Kosten
   * Stunden, FTE oder Kostenabweichung
   * Nettostunden, FTE oder Kosten

* Wenn Sie die Ansicht **Nach Benutzer anzeigen** anwenden, werden die folgenden Spalten angezeigt:

   * Verfügbare Stunden oder FTE
   * Geplante Stunden oder VZÄ
   * Stunden- oder FTE-Differenz
   * Geplante Stunden Zuteilungsprozentsatz

>[!TIP]
>
>Diese Informationen sind nicht als Kosten verfügbar, wenn die Ansicht **Nach Benutzer anzeigen** auf den Ressourcenplaner angewendet wird.
>
>Um weitere Informationen darüber zu erhalten, was in den einzelnen Spalten angezeigt wird, bewegen Sie den Mauszeiger über den Namen der Spalte, in der die Zahl angezeigt wird.\
>![Net_hours_res_planner_mouse_over.png](assets/net-hours-res-planner-mouse-over-350x95.png)
>
>Weitere Informationen zu den in den einzelnen Spalten angezeigten Daten finden Sie in den folgenden Artikeln:
>
>* [Übersicht über Stunden, FTE und Kosteninformationen in der Projekt- und Rollenansicht des Ressourcenplaners](../../resource-mgmt/resource-planning/overview-of-planner-hour-fte-cost-information-in-role-project-views.md)
>* [Verfügbare, geplante und tatsächliche Stunden oder FTE im Ressourcenplaner anzeigen, wenn Sie die Benutzeransicht verwenden](../../resource-mgmt/resource-planning/view-hours-fte-user-view-resource-planner.md)
>

## Informationen nach Stunde, FTE oder Kosten anzeigen

1. Wechseln Sie zum Ressourcenplaner.

   Standardmäßig werden Informationen im Ressourcenplaner nach Stunden angezeigt.

1. Erweitern Sie das Dropdown-Menü.\
   ![Hours_fte_or_cost_dropdown.png](assets/hours-fte-or-cost-dropdown.png)

1. Wählen Sie aus den folgenden Optionen aus:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Stunden</td> 
      <td>Zeigt Informationen zu Verfügbarkeit und Zuordnung in Stunden an.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">FTE</td> 
      <td> <p>Zeigt Verfügbarkeits- und Zuordnungsinformationen in FTE an.</p> <p>Weitere Informationen zur FTE-Berechnung im Ressourcenplaner finden Sie unter <a href="../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">Übersicht über die Berechnung von Stunden und FTE für Benutzer und Funktionen im Ressourcenplaner</a>. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Kosten</td> 
      <td> <p>Zeigt Verfügbarkeits- und Zuordnungsinformationen nach Kosten an, wenn Sie den Ressourcenplaner in der Projekt- oder Aufgabenansicht anzeigen. Die Informationen zeigen Werte in der Währung Ihres Systems an. Ihr Workfront-Administrator definiert die Systemwährung. Weitere Informationen zum Einrichten der Systemwährung in Workfront finden Sie unter <a href="../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md" class="MCXref xref">Einrichten von Wechselkursen</a>.</p> <p><b>NOTIZ</b>

   Sie müssen Benutzer und Aufgabengebiete mit Kosten pro Stunde verknüpfen, um Kosteninformationen im Ressourcenplaner anzeigen zu können.<br style="font-style: italic;">Weitere Informationen zum Verknüpfen der Stundensätze für Kosten pro Stunde mit Aufgabengebieten finden Sie unter <a href="../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Erstellen und Verwalten von Aufgabengebieten</a>.<br style="font-style: italic;">Weitere Informationen zum Verknüpfen von Stundensätzen mit Benutzern finden Sie unter <a href="../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Bearbeiten des Benutzerprofils</a>.<br style="font-style: italic;">Weitere Informationen zur Kostenberechnung im Ressourcenplaner finden Sie unter <a href="../../resource-mgmt/resource-planning/calculate-costs-resource-planner.md" class="MCXref xref">Kosten berechnen im Ressourcenplaner </a>.</p> </td>
   </tr> 
     <tr> 
      <td role="rowheader">Anpassen</td> 
      <td>Erstellt eine benutzerdefinierte Ansicht der Spalten, die im Ressourcenplaner angezeigt werden Wählen Sie die Optionen aus, die Sie im Ressourcenplaner anzeigen möchten, wie in den folgenden Schritten beschrieben. </td> 
     </tr> 
    </tbody> 
   </table>

1. (Bedingt) Wenn Sie **Anpassen** ausgewählt haben, geben Sie Optionen im Feld **Angezeigte Metriken anpassen** an, um Ihre benutzerdefinierte Ansicht einzurichten.

   ![Ansichtsfeld anpassen](assets/planner-customize-view-box-350x114.png)

1. Wählen **in der Spalte** Ansichtstyp“ links eine der folgenden Ansichten aus:

   * Projekt
   * Rolle
   * Benutzerin bzw. Benutzer

1. Wählen **Abschnitt „Ausgewählte Elemente anzeigen** den Typ der Informationen aus, die in den Spalten der ausgewählten Ansicht angezeigt werden sollen. Die folgende Tabelle zeigt, welche Optionen in den einzelnen Ansichten verfügbar sind:

   | **Option** | Benutzeransicht | Projektansicht | Rollenansicht |
   |---|---|---|---|
   | Verfügbar | ✔ | ✔ | ✔ |
   | Geplant | ✔ | ✔ | ✔ |
   | Budgetiert |   | ✔ | ✔ |
   | Variance |   | ✔ | ✔ |
   | Netto |   | ✔ | ✔ |
   | Tatsächlich | ✔ |   |   |
   | Differenz | ✔ |   |   |
   | Prozent | ✔ |   |   |

1. Wählen Sie **Geplante (PLN) Werte in NET-Berechnungen verwenden**, um bei der Berechnung der Nettowerte in den Projekt- und Funktionsansichten die Daten „Geplant“ anstelle der budgetierten Daten zu verwenden.

   Bei Auswahl dieser Option berechnet Workfront die Nettowerte anhand der folgenden Formel:

   `Net = Available - Planned`

   >[!TIP]
   >
   >**Diese Option wird nur angewendet, wenn Sie mindestens eine Option auswählen, um die Ansicht im Abschnitt Ausgewählte Elemente anzeigen anzupassen.**

1. Klicken Sie auf **Speichern**.

   Die benutzerdefinierte Ansicht, die Ihre ausgewählten Spalten enthält, wird angezeigt.

   Der Ressourcenplaner listet die angepasste Ansicht im Dropdown-Menü Stunden als Benutzerdefiniert auf.

   >[!NOTE]
   >
   >Sie können nur eine benutzerdefinierte Ansicht haben.

   ![Dropdown-Liste „Planerstunden“](assets/planner-hours-drop-down-with-custom-and-customize-option-183x281.png)

## Anzeigen des Diagramms für die Benutzerzuordnung

Sie können die geplante Zuordnung von Benutzern und deren Verfügbarkeit in einem Diagramm anzeigen.

So zeigen Sie die Benutzerzuordnung in einem Diagramm an:

1. Wechseln Sie zum Ressourcenplaner.

   Weitere Informationen zum Zugriff auf den Ressourcenplaner finden Sie im Abschnitt [Suchen des ](../../resource-mgmt/resource-planning/get-started-resource-planner.md#accessing-the-resource-planner)) im Artikel [Ressourcenplaner - Übersicht](../../resource-mgmt/resource-planning/get-started-resource-planner.md).

1. Wählen Sie **Nach Benutzer anzeigen** aus.

   >[!TIP]
   >
   >Das Benutzerzuordnungsdiagramm kann nur in der Benutzeransicht angezeigt werden.

1. Klicken Sie auf das **Benutzerzuordnungsdiagramm**-Symbol ![RP_USER_ALLOCATION_chart.png](assets/rp-user-allocation-chart.png), um die folgenden Informationen anzuzeigen:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Verfügbarkeit (%) ohne Überallokation für alle Benutzenden</td> 
      <td>Dies ist die Zeit, die alle Benutzenden in einem bestimmten Zeitraum für die Arbeit zur Verfügung stehen, angezeigt als Prozentsatz der insgesamt verfügbaren Zeit. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Überallokation (%) für alle Benutzenden </td> 
      <td> <p>Dies ist die Zeit, die Benutzende in einem Zeitraum überlastet sind, angezeigt als Prozentsatz der gesamten verfügbaren Zeit.</p> <p><b>NOTIZ</b>

   Eine Überallokation tritt auf, wenn die geplanten Stunden höher sind als die verfügbaren Stunden. </p> </td>
   </tr> 
     <tr> 
      <td role="rowheader">Nichtauslastung (%) für alle Benutzenden</td> 
      <td> <p>Dies ist die Zeit, die Benutzende in einem bestimmten Zeitraum nicht ausgelastet sind, angezeigt als Prozentsatz der gesamten verfügbaren Zeit.</p> <p><b>NOTIZ</b>

   Eine unzureichende Auslastung tritt auf, wenn die geplanten Stunden unter den verfügbaren Stunden liegen. </p> </td>
   </tr> 
     <tr> 
      <td role="rowheader">In diesem Zeitraum gibt es eine Überallokation für mindestens einen Benutzer/eine Benutzerin</td> 
      <td>Dies zeigt an, dass für mindestens einen Benutzer in einem Zeitraum eine Überallokation vorliegt, obwohl die Gesamtdauer aller Benutzer für den Zeitraum nicht überallokiert ist.<br>Sie müssen durch die Liste der Benutzer scrollen, und die Stunden für den Benutzer, der überlastet ist, sind rot hervorgehoben.</td> 
     </tr> 
    </tbody> 
   </table>

   ![RP__user_allocation_chart_Dec._7__2017.png](assets/rp--user-allocation-chart-dec.-7--2017-350x148.png)

1. (Optional) Klicken Sie auf den **Überallokation % für alle Benutzer** Bereich im Diagramm.\
   Alle Benutzer, die überlastet sind, werden rot hervorgehoben.
1. (Optional) Klicken Sie auf den **Nichtauslastung % für alle Benutzer** Bereich im Diagramm.\
   Alle nicht ausgelasteten Benutzenden werden blau hervorgehoben.

1. (Optional) Klicken Sie auf das Indikatorsymbol ![one_user_overallocation_marker.png](assets/one-user-overallocation-marker.png), das anzeigt, wo mindestens ein Benutzer überlastet ist.\
   Die überlasteten Benutzenden werden rot hervorgehoben.

1. (Optional) Aktualisieren Sie die Seite, um das Diagramm zu reduzieren.
