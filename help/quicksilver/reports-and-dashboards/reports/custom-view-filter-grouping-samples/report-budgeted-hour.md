---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Bericht: Budgetierte Stunde'
description: 'Bericht: Budgetierte Stunde'
author: Nolan
feature: Reports and Dashboards
exl-id: 2c0b60a6-fae4-4b29-8243-2a7f7d1f574b
source-git-commit: a6874c3a2dfda02b8a25f78056767d8c59c888e9
workflow-type: tm+mt
source-wordcount: '658'
ht-degree: 1%

---

# Bericht: Budgetierte Stunde

<!--Audited: 10/2024-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: From&nbsp;Alina: This is my article, but since it's about building a report, it is in the Reporting section. Please don't remove it -it's linked to Resource Management and it is super important.) </p>
-->

Wenn Sie Informationen zu budgetierten Stunden für andere Benutzer freigeben möchten, die keinen Zugriff auf den Ressourcenplaner haben, können Sie dies tun, indem Sie einen Bericht zu budgetierten Stunden erstellen. Anschließend können Sie den Bericht für sie freigeben.

>[!IMPORTANT]
>
>Budgetierte Stunden werden in der Adobe Workfront-Datenbank normalerweise stündlich aktualisiert (selten, es kann maximal drei Stunden dauern). Durch Aktualisieren des Berichts werden die darin enthaltenen Stundeninformationen nicht unbedingt aktualisiert. Sie können die seit der letzten Aktualisierung verstrichene Zeit in der oberen rechten Ecke jedes Berichts Budgetierte Stunde anzeigen. Durch die Aktualisierung des Berichts werden die darin enthaltenen Informationen nur dann aktualisiert, wenn seit der letzten Aktualisierung mehr als eine Stunde vergangen ist.
>
>![](assets/budgeted-hour-report-time-sync-warning-350x74.png)

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> 
    <p>Neu:</p>
   <ul><li><p>Mitwirkender zum Ändern eines Filters </p></li>
   <li><p>Standard zum Ändern eines Berichts</p></li> </ul>

<p>Aktuell:</p>
   <ul><li><p>Filter ändern </p></li>
   <li><p>Planen der Änderung eines Berichts</p></li> </ul></td> 
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

*Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Erstellen eines Berichts zur budgetierten Stunde

1. Klicken Sie auf das **Hauptmenü**-Symbol ![](assets/main-menu-icon.png) in der oberen rechten Ecke oder auf das **Hauptmenü**-Symbol ![](assets/lines-main-menu.png) in der oberen linken Ecke, falls verfügbar, und klicken Sie dann auf **Berichte**.

1. Klicken Sie auf **Neuer Bericht** > **Mehr** > **Budgetierte Stunde**.

   Die Standardansicht wird auf den Bericht angewendet.

1. (Optional) Um die Lesbarkeit des Berichts zu vereinfachen, klicken Sie auf **Bud. Stunden** Spalte, **Wechseln Sie in den Textmodus** und klicken Sie dann auf **Textmodus bearbeiten**.
1. Ändern Sie die `valuefield` in `valueexpreesion` und geben Sie den Rundungsausdruck ein.

   Dadurch wird die Anzahl der budgetierten Stunden auf eine von Ihnen angegebene Anzahl von Dezimalstellen gerundet.

   Informationen zum Runden einer Zahl in Workfront finden Sie im Artikel [Übersicht über berechnete Datenausdrücke](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

1. Klicken Sie **Fertig**.
1. (Optional) Klicken Sie auf **Spalte hinzufügen**, um weitere Spalten hinzuzufügen.
1. (Optional) Um die Lesbarkeit des Berichts zu vereinfachen, wird empfohlen, eine Gruppierung hinzuzufügen. Wir schlagen folgende Gruppierung vor:

   Klicken Sie auf **Registerkarte** Gruppierungen“ und führen Sie dann einen oder mehrere der folgenden Schritte aus:

   * Klicken Sie auf **Gruppierung hinzufügen** und geben Sie „Projektname“ ein. Wählen Sie dann aus, wenn er in der Liste angezeigt wird.
   * Klicken Sie auf **Gruppierung hinzufügen** und geben Sie zunächst „Name des Aufgabengebiets“ ein. Wählen Sie diesen aus, wenn er in der Liste angezeigt wird.
   * Klicken Sie auf **Gruppierung hinzufügen** und geben Sie „Zuteilungsdatum“ ein, wählen Sie es aus, wenn es in der Liste angezeigt wird, und wählen Sie dann den Zeitrahmen, nach dem Sie gruppieren möchten, aus dem Feld **Gruppierungsdatum nach** aus.

1. (Optional) Klicken Sie auf **Filter**, um dem Bericht Filter hinzuzufügen.
1. (Optional) Klicken Sie auf **Diagramm**, um dem Bericht ein Diagramm hinzuzufügen.
1. Klicken Sie auf **Speichern + schließen**.

## Bericht zur budgetierten Stunde prüfen

Im Bericht „Budgetierte Stunde“ sind standardmäßig die folgenden Informationen verfügbar:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Projekt </td> 
   <td>Dies ist der Name des Projekts, das mit der budgetierten Stunde verknüpft ist.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Aufgabengebiet</p> </td> 
   <td>Dies ist der Name des Aufgabengebiets, das mit der budgetierten Stunde verknüpft ist. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Benutzerin oder Benutzer</td> 
   <td>Dies ist der Name des Benutzers, der mit der budgetierten Stunde verknüpft ist.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Zuteilungsdt.</td> 
   <td> <p>Dies ist das Zuteilungsdatum. Es ist der erste Tag (ein Sonntag) der Woche, für die Sie die Stunden budgetiert haben.</p> <p>Tipp:  <p>Wenn sich eine Woche über zwei Monate erstreckt, werden zwei Zeilen im Bericht generiert: eine Zeile, die dem ersten Tag der Woche entspricht (der Sonntag der Woche, der während des ersten Monats liegt), und eine zweite, die dem ersten Tag des zweiten Monats entspricht (und der ein beliebiger Tag der Woche sein kann).</p> <p>Wenn Sie beispielsweise 8 Stunden für einen Benutzer für die Woche vom 30. Juni (Sonntag) bis zum 6. Juli (Samstag) budgetieren, zeigen die beiden Zeilen das Zuordnungsdatum 30. Juni und 1. Juli an.</p> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Bdg. Stunden</td> 
   <td>Dies sind die budgetierten Stunden, die dem Benutzer im Ressourcenplaner zugeordnet sind.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Gpl. Bdg. Stunden</td> 
   <td>Dies sind die budgetierten Stunden, die dem Aufgabengebiet oder Projekt im Ressourcenplaner zugeordnet sind.</td> 
  </tr> 
 </tbody> 
</table>
