---
product-area: resource-management
navigation-topic: resource-planning
title: Überprüfen der Ressourcenverfügbarkeit und -zuordnung mithilfe des Adobe Workfront Resource Planner
description: Im Ressourcenplaner können Sie die Verfügbarkeit Ihrer Ressourcen und die geplante oder geplante Arbeit für Ihre Projekte einsehen. Diese Werte werden in Stunden-, FTE- (Vollzeitäquivalent) oder Kostenbeträgen angezeigt und sind in Spalten unterteilt.
author: Alina
feature: Resource Management
exl-id: 5b3e52a6-af9b-4e68-8d6e-43a5151a2a2c
source-git-commit: 24cc3ece515fd778a9bc9e8afbcd534f48b24230
workflow-type: tm+mt
source-wordcount: '1266'
ht-degree: 4%

---

# Überprüfen der Ressourcenverfügbarkeit und -zuordnung mithilfe des Adobe Workfront Resource Planner

Im Ressourcenplaner können Sie die Verfügbarkeit Ihrer Ressourcen und die geplante oder geplante Arbeit für Ihre Projekte einsehen. Diese Werte werden in Stunden-, FTE- (Vollzeitäquivalent) oder Kostenbeträgen angezeigt und sind in Spalten unterteilt.

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Pro und höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Überprüfen oder höher </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zeigen Sie den Zugriff auf Folgendes an oder höher:</p> 
    <ul> 
     <li> <p>Ressourcenverwaltung</p> </li> 
     <li> <p>Finanzielle Daten</p> </li> 
     <li> <p>Benutzende</p> </li> 
     <li> <p>Projekte</p> </li> 
    </ul> <p><b>NOTIZ</b>

Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Anzeigen oder Höhere Berechtigungen für die Projekte, die Sie im Ressourcenplaner anzeigen möchten</p> <p>Weitere Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Anfordern des Zugriffs auf Objekte </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

<!--note from the table about the license: Review or higher: 
      <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
       (waiting on Vazgen to confirm - working differenly in classic)
      </MadCap:conditionalText>
     -->

## Voraussetzungen

Sie müssen alle Voraussetzungen erfüllen, die für die Arbeit mit dem Ressourcenplaner erforderlich sind. Weitere Informationen finden Sie unter [Ressourcenplaner - Übersicht](../../resource-mgmt/resource-planning/get-started-resource-planner.md).

>[!IMPORTANT]
>
>Wenn eine der Voraussetzungen für die korrekte Funktionalität des Ressourcen-Planers fehlt, kann es vorkommen, dass einige der Zahlen null sind oder die Budgetzeit abgeblendet ist.

## Verfügbarkeit und Zuordnung von Ressourcen

Die Spalten, die die Verfügbarkeit und Zuordnung Ihrer Ressourcen anzeigen, ändern sich je nach Ansicht, die Sie auf den Ressourcenplaner anwenden. Informationen zum Anzeigen der Informationen im Ressourcenplaner nach Projekt, Rolle oder Benutzer finden Sie unter [Navigationsübersicht für Ressourcenplaner](../../resource-mgmt/resource-planning/resource-planner-navigation.md).

Beachten Sie Folgendes, wenn Sie Ihre Ansicht in den Ressourcenplaner ändern:

* Wenn Sie die Ansichten **Nach Projekt anzeigen** oder **Nach Rolle anzeigen** anwenden, werden die folgenden Spalten angezeigt:

  <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  (NOTE: Alina: (some of the information in this area is also covered in Calculating Costs in the RP - https://workfront.zendesk.com/hc/en-us/articles/115004186433 - update this article also, when changes here occur)
  </MadCap:conditionalText>
  -->



   * Verfügbare Stunden, FTE oder Kosten
   * Geplante Stunden, VZÄ oder Kosten
   * Budgetierte Stunden, VZÄ oder Kosten
   * Stunden, VZÄ oder Kostenabweichung
   * Nettozeiten, VZÄ oder Kosten

* Wenn Sie die Ansicht **Nach Benutzer anzeigen** anwenden, werden die folgenden Spalten angezeigt:

   * Verfügbare Stunden oder FTE
   * Geplante Stunden oder VZÄ
   * Hour- oder FTE-Differenz
   * Prozentsatz der geplanten Stundenzuweisung

>[!TIP]
>
>Die Informationen sind nicht als Kosten verfügbar, wenn die Ansicht **Nach Benutzer anzeigen** auf den Ressourcenplaner angewendet wird.
>
>Wenn Sie weitere Informationen dazu erhalten möchten, wie die einzelnen Spalten angezeigt werden, bewegen Sie den Mauszeiger über den Namen der Spalte, in der die Zahl angezeigt wird.\
>![Net_hours_res_planner_mouse_over.png](assets/net-hours-res-planner-mouse-over-350x95.png)
>
>Weitere Informationen zu den in den einzelnen Spalten angezeigten Daten finden Sie in den folgenden Artikeln:
>
>* [Überblick über Stunden, FTE und Kosteninformationen in den Projekt- und Rollenansichten des Ressourcenplaners](../../resource-mgmt/resource-planning/overview-of-planner-hour-fte-cost-information-in-role-project-views.md)
>* [Verfügbare, geplante und tatsächliche Stunden oder FTE im Ressourcenplaner bei Verwendung der Benutzeransicht anzeigen](../../resource-mgmt/resource-planning/view-hours-fte-user-view-resource-planner.md)
>

## Anzeigen von Informationen nach Stunde, FTE oder Kosten

1. Wechseln Sie zum Ressourcen-Planer.

   Standardmäßig werden Informationen nach Stunden im Ressourcenplaner angezeigt.

1. Erweitern Sie das Dropdown-Menü.\
   ![Hours_fte_or_cost_dropdown.png](assets/hours-fte-or-cost-dropdown.png)

1. Wählen Sie aus den folgenden Optionen aus:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Stunden</td> 
      <td>Zeigt Informationen zur Verfügbarkeit und Zuordnung in Stunden an.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">FTE</td> 
      <td> <p>Zeigt Verfügbarkeits- und Zuweisungsinformationen in VZÄ an.</p> <p>Weitere Informationen zur Berechnung der FTE im Ressourcenplaner finden Sie unter <a href="../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">Übersicht über die Berechnung der Stunden und der FTE für Benutzer und Rollen im Ressourcenplaner</a>. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Kosten</td> 
      <td> <p>Zeigt Verfügbarkeits- und Zuordnungsinformationen nach Kosten an, wenn Sie den Ressourcenplaner in der Projekt- oder Rollenansicht anzeigen. Die Informationen zeigen Werte in der Währung Ihres Systems an. Ihr Workfront-Administrator definiert die Systemwährung. Weitere Informationen zur Einrichtung der Systemwährung in Workfront finden Sie unter <a href="../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md" class="MCXref xref">Einrichten von Wechselkursen</a>.</p> <p><b>NOTIZ</b>

   Sie müssen Benutzer und Stellenrollen mit den Kosten pro Stunde-Raten verknüpfen, um Kosteninformationen im Ressourcenplaner anzuzeigen.<br style="font-style: italic;">Weitere Informationen zum Verknüpfen von Kosten pro Stunde mit Auftragsrollen finden Sie unter <a href="../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Erstellen und Verwalten von Auftragsrollen</a>.<br style="font-style: italic;">Weitere Informationen zum Zuordnen der Kosten pro Stunde zu Benutzern finden Sie unter <a href="../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Profil eines Benutzers bearbeiten</a>.<br style="font-style: italic;">Weitere Informationen zur Berechnung der Kosten im Ressourcenplaner finden Sie unter <a href="../../resource-mgmt/resource-planning/calculate-costs-resource-planner.md" class="MCXref xref">Berechnen der Kosten im Ressourcenplaner </a>.</p> </td>
   </tr> 
     <tr> 
      <td role="rowheader">Anpassen</td> 
      <td>Erstellt eine benutzerdefinierte Ansicht der im Ressourcenplaner angezeigten Spalten. Wählen Sie die Optionen aus, die im Ressourcenplaner angezeigt werden sollen, wie in den folgenden Schritten beschrieben. </td> 
     </tr> 
    </tbody> 
   </table>

1. (Bedingt) Wenn Sie **Anpassen** ausgewählt haben, zeigen Sie Optionen im Feld **Angezeigte Metriken anpassen** an, um Ihre benutzerdefinierte Ansicht einzurichten.

   ![](assets/planner-customize-view-box-350x114.png)

1. Wählen Sie links in der Spalte **Ansichtstyp** eine der folgenden Ansichten aus:

   * Projekt
   * Funktion
   * Benutzerin oder Benutzer

1. Wählen Sie im Abschnitt **Ausgewählte Elemente anzeigen** den Informationstyp aus, der in den Spalten der ausgewählten Ansicht angezeigt werden soll. Die folgende Tabelle zeigt, welche Optionen in den einzelnen Ansichten verfügbar sind:

   | **Option** | Benutzeransicht | Projektansicht | Rollenansicht |
   |---|---|---|---|
   | Verfügbar | ms | ms | ms |
   | Geplant | ms | ms | ms |
   | Budgetiert |   | ms | ms |
   | Abweichung |   | ms | ms |
   | Net |   | ms | ms |
   | Tatsächlich | ms |   |   |
   | Differenz | ms |   |   |
   | Prozent | ms |   |   |

1. Wählen Sie **PLN (Geplante Werte) in NET-Berechnungen verwenden** aus, um bei der Berechnung der Netzwerte in den Projekt- und Rollenansichten die Option Geplant anstelle der Budgetinformationen zu verwenden.

   Bei Auswahl dieser Option berechnet Workfront die Nettowerte anhand der folgenden Formel:

   ```
   Net = Available - Planned
   ```

   >[!TIP]
   >
   >**Diese Option wird nur angewendet, wenn Sie mindestens eine Option auswählen, um die Ansicht im Abschnitt &quot;Ausgewählte Elemente anzeigen&quot;anzupassen.**

1. Klicken Sie auf **Speichern**.

   Die angepasste Ansicht, die Ihre ausgewählten Spalten enthält, wird angezeigt.

   Der Ressourcen-Planer listet die benutzerdefinierte Ansicht im Dropdownmenü Stunden als benutzerdefiniert auf.

   >[!NOTE]
   >
   >Sie können nur eine benutzerdefinierte Ansicht verwenden.

   ![](assets/planner-hours-drop-down-with-custom-and-customize-option-183x281.png)

## Anzeigen des Diagramms &quot;Benutzerzuordnung&quot;

Sie können die geplante Zuordnung von Benutzern anhand ihrer Verfügbarkeit in einer Grafik anzeigen.

So zeigen Sie die Zuordnung der Benutzer in einer Grafik an:

1. Wechseln Sie zum Ressourcen-Planer.

   Weitere Informationen zum Zugriff auf den Ressourcen-Planer finden Sie im Abschnitt [Suchen des Ressourcen-Planers](../../resource-mgmt/resource-planning/get-started-resource-planner.md#accessing-the-resource-planner) im Artikel [Überblick über den Ressourcen-Planer](../../resource-mgmt/resource-planning/get-started-resource-planner.md).

1. Wählen Sie **Nach Benutzer anzeigen** aus.

   >[!TIP]
   >
   >Sie können das Diagramm Benutzerzuordnung nur in der Benutzeransicht anzeigen.

1. Klicken Sie auf das Symbol **Benutzerzuordnungsdiagramm** ![RP_user_allocation_chart.png](assets/rp-user-allocation-chart.png), um die folgenden Informationen anzuzeigen:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Verfügbarkeit (%) ohne Überallokation für alle Benutzenden</td> 
      <td>Dies ist die Zeit, die alle Benutzer für die Arbeit in einem Zeitraum zur Verfügung stehen, in Prozent der gesamten verfügbaren Zeit. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Überallokation (%) für alle Benutzenden </td> 
      <td> <p>Dies ist die Zeit, die Benutzer in einem Zeitraum überverteilt werden, in Prozent der gesamten verfügbaren Zeit.</p> <p><b>NOTIZ</b>

   Eine Überzuweisung erfolgt, wenn die geplanten Stunden höher als die verfügbaren Stunden sind. </p> </td>
   </tr> 
     <tr> 
      <td role="rowheader">Nichtauslastung (%) für alle Benutzenden</td> 
      <td> <p>Dies ist die Zeit, die Benutzer in einem Zeitraum nicht ausreichend genutzt werden (in Prozent der gesamten verfügbaren Zeit).</p> <p><b>NOTIZ</b>

   Eine Unterauslastung tritt auf, wenn die geplanten Stunden unter den verfügbaren Stunden liegen. </p> </td>
   </tr> 
     <tr> 
      <td role="rowheader">In diesem Zeitraum gibt es eine Überallokation für mindestens einen Benutzer/eine Benutzerin</td> 
      <td>Dies weist darauf hin, dass für mindestens einen Benutzer in einem Zeitraum eine Überzuweisung erfolgt, obwohl die Gesamtdauer aller Benutzer für den Zeitraum nicht übermäßig verteilt ist.<br>Sie müssen durch die Liste der Benutzer blättern, und die Stunden für den Benutzer, der übergeordnet ist, sind rot hervorgehoben.</td> 
     </tr> 
    </tbody> 
   </table>

   ![RP__user_allocation_chart_Dec._7__2017.png](assets/rp--user-allocation-chart-dec.-7--2017-350x148.png)

1. (Optional) Klicken Sie im Diagramm auf den Bereich **Überzuweisung % für alle Benutzer** .\
   Alle Benutzer, die übergeordnet sind, werden rot hervorgehoben.
1. (Optional) Klicken Sie im Diagramm auf den Bereich **Unterauslastung % für alle Benutzer** .\
   Alle Benutzer, die nicht verwendet werden, werden blau hervorgehoben.

1. (Optional) Klicken Sie auf das Indikatorsymbol ![one_user_overallocation_marker.png](assets/one-user-overallocation-marker.png) , das anzeigt, wo mindestens ein Benutzer übergeordnet ist.\
   Die Benutzer, die übergeordnet sind, werden rot hervorgehoben.

1. (Optional) Aktualisieren Sie die Seite, um das Diagramm zu reduzieren.
