---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: "Report: Budgeted Hour"
description: "Report: Budgeted Hour"
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 2c0b60a6-fae4-4b29-8243-2a7f7d1f574b
source-git-commit: 332c744ab9b760268620461ed2cb2551caf383cf
workflow-type: tm+mt
source-wordcount: '657'
ht-degree: 1%

---

# Bericht: Budgetierte Stunde

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: From&nbsp;Alina: This is my article, but since it's about building a report, it is in the Reporting section. Please don't remove it -it's linked to Resource Management and it is super important.) </p>
-->

Wenn Sie Budgeted Hour-Informationen mit anderen Benutzern teilen möchten, die keinen Zugriff auf den Resource Planer haben, können Sie dies tun, indem Sie einen Budgeted Hour-Bericht erstellen. Sie können den Bericht dann für sie freigeben.

>[!IMPORTANT]
>
>Budgetierte Stunden werden in der Adobe Workfront-Datenbank in der Regel stündlich aktualisiert (selten kann dies bis zu drei Stunden dauern). Beim Aktualisieren des Berichts werden die Stundeninformationen nicht unbedingt aktualisiert. Sie können die seit der letzten Aktualisierung verstrichene Zeit in der rechten oberen Ecke eines jeden Berichts zur budgetierten Stunde anzeigen. Beim Aktualisieren des Berichts werden die darin enthaltenen Informationen nur aktualisiert, wenn seit der letzten Aktualisierung mehr als eine Stunde vergangen ist.
>
>![](assets/budgeted-hour-report-time-sync-warning-350x74.png)>

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf Berichte, Dashboards und Kalender bearbeiten</p> <p>Zugriff auf Filter, Ansichten, Gruppierungen bearbeiten</p> <p><b>NOTIZ</b>

Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Berechtigungen für einen Bericht verwalten</p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Erstellen eines budgetierten Stundenberichts

1. Klicken Sie auf **Hauptmenü** ![](assets/main-menu-icon.png) in der oberen rechten Ecke und klicken Sie auf **Berichte**.

1. Klicks **Neuer Bericht > Budgetzeit**.

   Die Standardansicht wird auf den Bericht angewendet.

1. (Optional) Um den Bericht leichter zu lesen, klicken Sie auf die Schaltfläche **Budgetierte Stunden** Spalte, dann **In den Textmodus wechseln**, ändern Sie dann die

   ```
   valuefield
   ```

   Linie zu

   ```
   valueexpreesion
   ```

   und geben Sie den Rundungsausdruck ein.

   Dadurch wird die Anzahl der geplanten Stunden auf eine Anzahl von Dezimalstellen gerundet, die Sie angeben.

   Informationen zum Umrunden einer Zahl in Workfront finden Sie im Artikel [Übersicht über berechnete Datenausdrücke](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

1. (Optional) Klicken Sie auf **Spalte hinzufügen** , um zusätzliche Spalten hinzuzufügen.
1. (Optional) Um das Lesen des Berichts zu vereinfachen, wird empfohlen, ihm eine Gruppierung hinzuzufügen. Wir empfehlen die folgende Gruppierung:

   Klicken Sie auf **Gruppierungen** und führen Sie dann einen oder mehrere der folgenden Schritte aus:

   1. Klicks **Gruppierung hinzufügen** und beginnen Sie mit der Eingabe von &quot;Projektname&quot;, wählen Sie ihn aus, wenn er in der Liste angezeigt wird.
   1. Klicks **Gruppierung hinzufügen** und beginnen Sie mit der Eingabe von &quot;Auftragsrollenname&quot;und wählen Sie ihn aus, wenn er in der Liste angezeigt wird.
   1. Klicks **Gruppierung hinzufügen** und Eingabe beginnen **Zuordnungsdatum**, wählen Sie es aus, wenn es in der Liste angezeigt wird, und wählen Sie dann den Zeitrahmen aus, nach dem Sie die Gruppe gruppieren möchten. **Gruppierungstermine nach** -Feld.

1. (Optional) Klicken Sie auf **Filter** , um Filter zum Bericht hinzuzufügen.
1. (Optional) Klicken Sie auf **Diagramm** , um dem Bericht ein Diagramm hinzuzufügen.
1. Klicks **Speichern und schließen**.

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
