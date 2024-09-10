---
navigation-topic: use-the-gantt-chart
title: Gantt-Diagramm in PDF exportieren
description: Sie können das Gantt-Diagramm in eine PDF exportieren. Nachdem Sie das Gantt-Diagramm auf PDF exportiert haben, können Sie es drucken oder an eine E-Mail anhängen, um es für andere Benutzer freizugeben.
author: Alina
feature: Work Management
exl-id: 91aad9e0-25c9-4eae-aa66-8aab763d3b76
source-git-commit: 3097aca9b8fd856bbf3f91a354b5083fa7b23830
workflow-type: tm+mt
source-wordcount: '1045'
ht-degree: 1%

---

# Exportieren des [!UICONTROL Gantt-Diagramms] in PDF

<!--Audited: 09/2024-->

Sie können das [!UICONTROL Gantt-Diagramm] in eine PDF exportieren.

Nach dem Export des [!UICONTROL Gantt-Diagramms] in PDF können Sie es drucken oder an eine E-Mail anhängen, um es für andere Benutzer freizugeben.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

Sie müssen über Folgendes verfügen, um die Schritte in diesem Artikel zu befolgen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront] Plan*</td> 
   <td> <p>Alle </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront] Lizenz*</td> 
   <td> <p>Neu:[!UICONTROL Light] oder höher</p>
   <p>Aktuell:[!UICONTROL Review] oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>[!UICONTROL Ansicht] oder höherer Zugriff auf Projekte und Aufgaben</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>[!UICONTROL Ansicht] oder höherer Zugriff auf das Projekt</p> </td> 
  </tr> 
 </tbody> 
</table>

*Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Exportieren des [!UICONTROL Gantt-Diagramms]

1. Greifen Sie auf das [!UICONTROL Gantt-Diagramm] zu, das Sie auf PDF exportieren möchten, wie unter [Erste Schritte mit dem [!UICONTROL Gantt-Diagramm]](../../../manage-work/gantt-chart/use-the-gantt-chart/get-started-with-gantt.md) beschrieben.
1. Stellen Sie sicher, dass Sie das [!UICONTROL Gantt-Diagramm] so konfiguriert haben, dass die entsprechenden Informationen angezeigt werden, bevor Sie es exportieren.

   >[!NOTE]
   >
   >Wenn Sie das [!UICONTROL Gantt-Diagramm] aus einer Projektliste exportieren, enthält die PDF-Datei nur die-Projekte in der Liste, nicht die Aufgaben in den einzelnen Projekten. Wenn Sie eine Aufgabenliste exportieren möchten, können Sie dies aus dem Projekt tun, mit dem sie verknüpft sind, oder indem Sie einen Aufgabenbericht erstellen und die Ergebnisse des Berichts in der [!UICONTROL Gantt-Ansicht] anzeigen.

   Konfigurieren Sie eine der folgenden Informationen:

   * Klicken Sie auf die Symbole **Filter**, **Ansicht** und **Gruppierung** oberhalb des [!UICONTROL Gantt-Diagramms] und fügen Sie den vorhandenen Filter, die Ansicht oder die Gruppierung, die auf die Liste der Elemente im [!UICONTROL Gantt-Diagramm] angewendet werden, hinzu oder bearbeiten Sie ihn.

     Alle in der Listenansicht ausgewählten Filter und Gruppierungen werden beim Anzeigen des [!UICONTROL Gantt-Diagramms] beibehalten. Ansichten werden im exportierten [!UICONTROL Gantt-Diagramm] nur innerhalb der Liste angezeigt, die neben dem [!UICONTROL Gantt-Diagramm] auf der ersten Seite angezeigt wird. Ansichten werden nicht im [!UICONTROL Gantt-Diagramm] selbst angezeigt.

     >[!TIP]
     >
     >Um dem [!UICONTROL Gantt-Diagramm] selbst mehr Platz zu geben, wenden Sie eine Ansicht an, die so wenige Spalten wie möglich enthält.

   * Wählen Sie die Option **Zu den geplanten Daten wechseln** aus, um anstelle der geplanten Datumswerte die Option &quot;Geplant&quot;anzuzeigen. Standardmäßig werden Geplante Datumswerte angezeigt.

   * Klicken Sie oben rechts im Gantt-Diagramm auf das Symbol **Einstellungen** ![](assets/settings-icon.png) und wählen Sie aus, welche Informationen im Gantt-Diagramm angezeigt werden sollen. Nach der Auswahl sind diese Informationen in der exportierten Gantt-PDF-Datei enthalten.

     Wählen Sie aus den folgenden Optionen aus:

      * Tatsächliche Termine
      * Arbeitsaufträge
      * Ausgangsbasis
      * Verpflichtungsdatum
      * % abgeschlossen
      * Kritischer Pfad
      * Meilenstein-Diamanten
      * Meilenstein-Linien
      * Vorgänger
      * Fortschrittsstatus
      * Geplante Daten

     Weitere Informationen finden Sie unter   [Konfigurieren Sie, wie Informationen im [!UICONTROL Gantt-Diagramm]](../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md) angezeigt werden.

     >[!NOTE]
     >
     > Zuweisungen werden nicht im [!UICONTROL Gantt-Diagramm] angezeigt, wenn das [!UICONTROL Gantt-Diagramm] nach PDF exportiert wird. Wenn das [!UICONTROL Gantt-Diagramm] nach PDF exportiert wird, werden Zuweisungen nur in der Listenansicht angezeigt.

   * Der Zeitraum, der im [!UICONTROL Gantt-Diagramm] angezeigt wird.

     Weitere Informationen finden Sie unter [Anzeigen von Informationen im [!UICONTROL Gantt-Diagramm]](../../../manage-work/gantt-chart/use-the-gantt-chart/view-info-in-gantt.md).

     Wie der Zeitraum in der Exportdatei angezeigt wird, hängt davon ab, ob Sie in einem späteren Schritt **[!UICONTROL Was ich sehe]** oder **[!UICONTROL Mehrere Seiten]** auswählen.

1. (Optional) Wenn Sie nur bestimmte Aufgaben in die exportierte PDF aufnehmen möchten, wählen Sie die Aufgaben aus, die Sie einbeziehen möchten.

   Wenn Sie keine Aufgaben auswählen, werden alle Aufgaben in die exportierte PDF eingeschlossen.

   Wenn Sie beispielsweise das [!UICONTROL Gantt-Diagramm] für ein Projekt anzeigen, das 50 Aufgaben enthält, aber nur 10 Aufgaben für das exportierte [!UICONTROL Gantt-Diagramm] anzeigen möchten, wählen Sie die 10 Aufgaben aus, die angezeigt werden sollen.

1. Klicken Sie oben rechts im Gantt-Diagramm auf das Druckersymbol ![](assets/printer-icon.png).
Das Dialogfeld **[!UICONTROL In PDF exportieren]** wird angezeigt.

   ![export_gantt_UI.png](assets/exported-gantt-ui-350x225.png)

1. Wählen Sie im Abschnitt **Exportieren** aus den folgenden Optionen aus, um anzugeben, ob Sie nur das, was Sie sehen, oder das gesamte [!UICONTROL Gantt-Diagramm] exportieren möchten:

   * **[!UICONTROL Was ich sehe]:** Exportiert alle Aufgaben (einschließlich aller Unteraufgaben), die vor dem Export von bis zu 500 Elementen auf dem Bildschirm angezeigt werden. (Dies wird nicht im Abschnitt **[!UICONTROL Vorschau]** angezeigt; der Abschnitt [!UICONTROL Vorschau] enthält nur Beispieldaten.)

     Unteraufgaben werden in die exportierte PDF eingeschlossen, selbst wenn die übergeordnete Aufgabe ausgeblendet ist und die Unteraufgaben nicht sichtbar sind. Um nur übergeordnete Aufgaben einzubeziehen, wählen Sie die übergeordneten Aufgaben aus, die Sie einbeziehen möchten, und lassen Sie die Auswahl aller Unteraufgaben aufheben.

     >[!TIP]
     >
     >Sie können das Dropdown-Menü **[!UICONTROL Zoom auf]** oder das Regler-Tool verwenden, um nur einen Teil des [!UICONTROL Gantt-Diagramms] anzuzeigen, wie in [Anzeigen von Informationen im [!UICONTROL Gantt-Diagramm]](../../../manage-work/gantt-chart/use-the-gantt-chart/view-info-in-gantt.md) beschrieben.


   * **[!UICONTROL Mehrere Seiten]:** Exportiert das gesamte [!UICONTROL Gantt-Diagramm], auch wenn es auf dem aktuellen Bildschirm bis zu 500 Elemente nicht sichtbar ist.

     >[!NOTE]
     >
     >* Sie können das Dropdownmenü **[!UICONTROL Zoom auf]** oder das Regler-Tool verwenden, um zu bestimmen, wie viele Informationen auf jeder Seite angezeigt werden, wie unter [Konfigurieren der Anzeige von Informationen im [!UICONTROL Gantt-Diagramm]](../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md) beschrieben. Wählen Sie eine detailliertere Option aus, um mehr zu exportierende Seiten anzuzeigen, oder wählen Sie eine weniger detaillierte Option, um weniger zu exportierende Seiten anzuzeigen.
     >
     >* Wenn Sie ein [!UICONTROL Gantt-Diagramm] exportieren müssen, das mehr als 500 Elemente enthält, wenden Sie einen Filter auf die Liste an, bevor Sie das [!UICONTROL Gantt-Diagramm] anzeigen, damit weniger als 500 Elemente oder 250 Seiten angezeigt werden. Informationen zum Anwenden eines Filters finden Sie unter [Filterübersicht](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).
     >
     >
     >* In den folgenden Fällen ist es nicht möglich, das gesamte Gantt-Diagramm zu exportieren:
     >   
     >   * Wenn er mehr als 250 Seiten umfasst
     >   * Wenn es mehr als 500 Elemente enthält


1. Wenn die PDF gedruckt wird, nachdem sie auf PDF exportiert wurde, wählen Sie im Dropdown-Menü **[!UICONTROL Seitengröße]** die gewünschte Papiergröße aus.
Sie können aus den folgenden Optionen auswählen:

   * **[!UICONTROL Brief]**
   * **[!UICONTROL Legal]**
   * **[!UICONTROL Ledger]**
   * **[!UICONTROL A1]**
   * **[!UICONTROL A2]**
   * **[!UICONTROL A3]** (nur für einige Sprachen verfügbar)
   * **[!UICONTROL A4]**
1. Wählen Sie im Abschnitt **[!UICONTROL Seitenausrichtung]** aus, ob die PDF im Querformat oder Hochformat exportiert werden soll.
1. Wählen Sie **[!UICONTROL Legende anzeigen]** aus, wenn Sie die Legende in Ihre exportierte PDF aufnehmen möchten.
1. Klicken Sie auf **[!UICONTROL Exportieren]**.

   Das pdf der [!UICONTROL Gantt-Grafik] wird erstellt und auf Ihren Computer heruntergeladen.

   Beachten Sie die Legende am unteren Rand der exportierten Datei. Es werden nur die Optionen erläutert, die Sie in Ihrem [!UICONTROL Gantt-Diagramm] aktiviert haben und die in Ihrer Aufgabenliste verfügbar sind.

   Beispielsweise werden Meilensteine nur dann in der Legende angezeigt, wenn mindestens eine Aufgabe mit einem Meilenstein verknüpft ist.

   ![gantt_chart_with_updated__limited_legend.png](assets/gantt-chart-with-updated--limited--legend-350x271.png)
