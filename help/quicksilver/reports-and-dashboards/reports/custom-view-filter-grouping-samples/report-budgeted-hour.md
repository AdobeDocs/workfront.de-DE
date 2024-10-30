---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: "Report: Budgeted Hour"
description: "Report: Budgeted Hour"
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

Wenn Sie Budgeted Hour-Informationen mit anderen Benutzern teilen möchten, die keinen Zugriff auf den Resource Planer haben, können Sie dies tun, indem Sie einen Budgeted Hour-Bericht erstellen. Sie können den Bericht dann für sie freigeben.

>[!IMPORTANT]
>
>Budgetierte Stunden werden in der Adobe Workfront-Datenbank in der Regel stündlich aktualisiert (selten kann dies bis zu drei Stunden dauern). Beim Aktualisieren des Berichts werden die Stundeninformationen nicht unbedingt aktualisiert. Sie können die seit der letzten Aktualisierung verstrichene Zeit in der rechten oberen Ecke eines jeden Berichts zur budgetierten Stunde anzeigen. Beim Aktualisieren des Berichts werden die darin enthaltenen Informationen nur aktualisiert, wenn seit der letzten Aktualisierung mehr als eine Stunde vergangen ist.
>
>![](assets/budgeted-hour-report-time-sync-warning-350x74.png)

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Abo</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> 
    <p>Neu:</p>
   <ul><li><p>Mitwirkende bei der Änderung eines Filters </p></li>
   <li><p>Standard zum Ändern eines Berichts</p></li> </ul>

<p>Aktuell:</p>
   <ul><li><p>Filteranforderung </p></li>
   <li><p>Berichtänderung planen</p></li> </ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Zugriff auf Berichte, Dashboards und Kalender bearbeiten, um einen Bericht zu ändern</p> <p>Zugriff auf Filter, Ansichten und Gruppierungen bearbeiten, um einen Filter zu ändern</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Berechtigungen für einen Bericht verwalten</p>  </td> 
  </tr> 
 </tbody> 
</table>

*Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Erstellen eines budgetierten Stundenberichts

1. Klicken Sie auf das Symbol **Hauptmenü** oben rechts oder, falls verfügbar, auf das Symbol **Hauptmenü** oben links, das Symbol ![](assets/lines-main-menu.png) und klicken Sie dann auf **Berichte**.![](assets/main-menu-icon.png)

1. Klicken Sie auf **Neuer Bericht** > **Mehr** > **Budgetierte Stunde**.

   Die Standardansicht wird auf den Bericht angewendet.

1. (Optional) Um den Bericht leichter zu lesen, klicken Sie auf den **Bud. Stunden** , dann **in den Textmodus wechseln** und dann auf **Textmodus bearbeiten** klicken.
1. Ändern Sie die Zeile `valuefield` in `valueexpreesion` und geben Sie den Rundungsausdruck ein.

   Dadurch wird die Anzahl der geplanten Stunden auf eine Anzahl von Dezimalstellen gerundet, die Sie angeben.

   Weitere Informationen zum Umrunden einer Zahl in Workfront finden Sie im Artikel [Übersicht über berechnete Datenausdrücke](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

1. Klicken Sie auf **Fertig**.
1. (Optional) Klicken Sie auf **Spalte hinzufügen** , um zusätzliche Spalten hinzuzufügen.
1. (Optional) Um das Lesen des Berichts zu vereinfachen, wird empfohlen, ihm eine Gruppierung hinzuzufügen. Wir empfehlen die folgende Gruppierung:

   Klicken Sie auf die Registerkarte **Gruppierungen** und führen Sie dann einen oder mehrere der folgenden Schritte aus:

   * Klicken Sie auf **Gruppierung hinzufügen** und beginnen Sie mit der Eingabe von &quot;Projektname&quot;. Wählen Sie ihn dann aus, wenn er in der Liste angezeigt wird.
   * Klicken Sie auf **Gruppierung hinzufügen** und beginnen Sie mit der Eingabe von &quot;Auftragsrollenname&quot;. Wählen Sie ihn dann aus, wenn er in der Liste angezeigt wird.
   * Klicken Sie auf **Gruppierung hinzufügen** und beginnen Sie mit der Eingabe &quot;Zuordnungsdatum&quot;, wählen Sie es aus, wenn es in der Liste angezeigt wird, und wählen Sie dann den Zeitrahmen aus, nach dem Sie die Gruppe im Feld **Datumsgruppen nach** gruppieren möchten.

1. (Optional) Klicken Sie auf **Filter** , um dem Bericht Filter hinzuzufügen.
1. (Optional) Klicken Sie auf **Diagramm** , um dem Bericht ein Diagramm hinzuzufügen.
1. Klicken Sie auf **Speichern + schließen**.

## Überprüfung des Berichts über die budgetierte Stunde

Standardmäßig sind im Bericht &quot;Budgetierte Stunde&quot;folgende Informationen verfügbar:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Projekt </td> 
   <td>Dies ist der Name des Projekts, das mit der budgetierten Stunde verbunden ist.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Auftragsrolle</p> </td> 
   <td>Dies ist der Name der Stellenfunktion, die mit der budgetierten Stunde verbunden ist. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Benutzerin oder Benutzer</td> 
   <td>Dies ist der Name des Benutzers, der mit der budgetierten Stunde verknüpft ist.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Zuteilungsdt.</td> 
   <td> <p>Dies ist das Zuordnungsdatum. Es ist der erste Tag (ein Sonntag) der Woche, für die Sie die Stunden geplant haben.</p> <p>Tipp:  <p>Wenn sich eine Woche über zwei Monate erstreckt, werden im Bericht zwei Zeilen generiert: eine Zeile, die dem ersten Wochentag (dem Sonntag der Woche, der im ersten Monat stattfindet) entspricht, und eine zweite Zeile, die dem ersten Tag des zweiten Monats entspricht (und möglicherweise einem beliebigen Wochentag entspricht).</p> <p>Wenn Sie z. B. für einen Benutzer einen Etat von 8 Stunden für die Woche vom 30. Juni (Sonntag) bis 6. Juli (Samstag) anlegen, zeigen die beiden Zeilen das Zuordnungsdatum 30. Juni und 1. Juli an.</p> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Bdg. Stunden</td> 
   <td>Dies sind die budgetierten Stunden, die dem Benutzer im Ressourcenplaner zugewiesen werden.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Pln. Bdg. Stunden</td> 
   <td>Dies sind die budgetierten Stunden, die der Stellenrolle oder dem Projekt im Ressourcenplaner zugewiesen werden.</td> 
  </tr> 
 </tbody> 
</table>
