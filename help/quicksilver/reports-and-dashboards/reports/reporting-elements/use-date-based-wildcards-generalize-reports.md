---
product-area: reporting
navigation-topic: reporting-elements
title: Verwenden datumsbasierter Platzhalter zum Generalisieren von Berichten
description: Sie können einen Bericht beim Erstellen bestimmter Berichterstellungselemente durch Verwendung von Platzhaltern anstelle spezifischer Informationen verallgemeinern.
author: Nolan
feature: Reports and Dashboards
exl-id: 759b0bea-729e-4206-808c-0a7216ded4ff
source-git-commit: 3cee374b68b26f2a423d41101300ec8b6685fadd
workflow-type: tm+mt
source-wordcount: '644'
ht-degree: 1%

---

# Verwenden datumsbasierter Platzhalter zum Generalisieren von Berichten

<!-- Audited: 11/2024 -->

Sie können einen Bericht beim Erstellen bestimmter Berichterstellungselemente durch Verwendung von Platzhaltern anstelle spezifischer Informationen verallgemeinern.

Wenn Sie beispielsweise einen Bericht erstellen möchten, der die Aufgaben mit einem bestimmten geplanten Startdatum anzeigt, können Sie mit der Datumsauswahl im Kalender in einem Filter ein bestimmtes Datum auswählen. Wenn Sie jedoch einen Bericht erstellen möchten, der Aufgaben anzeigt, bei denen das geplante Startdatum innerhalb eines bestimmten Zeitraums ab dem Datum des Zugriffs auf den Bericht liegt, können Sie einen Platzhalter verwenden, der angibt, dass bei der Anzeige des Berichts durch einen Benutzer Informationen für einen Zeitraum angezeigt werden, der für den Moment relevant ist, in dem der Bericht angezeigt wird.

Zum Beispiel in der vergangenen Woche, im letzten Jahr, in den nächsten zwei Wochen usw. Auf diese Weise erstellen Sie den Bericht einmal. Da Sie jedoch einen Platzhalter im Filter verwenden, werden bei jedem Lesen unterschiedliche Ergebnisse ausgegeben, da er sich an den Tag anpasst, an dem der Bericht ausgeführt wird.

Beim Erstellen der folgenden Berichterstellungselemente können Sie datumsbasierte Platzhalter verwenden:

* Filter
* Benutzerdefinierte Eingabeaufforderungen
* Ansichten beim Hinzufügen von Regeln für Spalten

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront-Plan*</strong></td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront-Lizenz*</strong></td> 
   <td> 
      <p>Neu:</p>
         <ul>
         <li><p>Standard</p></li>
         </ul>
      <p>Aktuell:</p>
         <ul>
         <li><p>Plan</p></li>
         </ul>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Konfigurationen auf Zugriffsebene*</strong></td> 
   <td> <p>Zugriff auf Filter, Ansichten, Gruppierungen bearbeiten</p> <p>Zugriff auf Berichte, Dashboards und Kalender bearbeiten, um Berichterstellungselemente in einem Bericht zu bearbeiten</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Objektberechtigungen</strong></td> 
   <td> <p>Berechtigungen für einen Bericht zum Bearbeiten von Berichterstellungselementen in einem Bericht verwalten</p> <p>Berechtigungen für Ansichten oder Filter verwalten, um sie zu bearbeiten</p></td> 
  </tr> 
 </tbody> 
</table>

*Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Voraussetzungen

Sie müssen einen Bericht erstellen, bevor Sie ihm Platzhaltervariablen hinzufügen können.

Informationen zum Erstellen eines Berichts finden Sie unter [Erstellen eines Berichts](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md).

## Schritte

So fügen Sie einen datumsbasierten Platzhalter in einen Bericht ein:

1. Gehen Sie zu einem Bericht, für den Sie einen datumsbasierten Platzhalter einfügen möchten.
1. Klicken Sie auf **Berichtaktionen** und dann auf **Bearbeiten**.
1. Klicken Sie auf die Registerkarte **Filter**.
1. Klicken Sie auf **Filterregel hinzufügen**.
1. Geben Sie den Namen des Felds ein, nach dem Sie filtern möchten.\
   Sie müssen Felder eingeben, die auf ein Datum verweisen.
1. Wählen Sie **Equal** im Dropdownmenü für die Filtervariable aus.

   >[!TIP]
   >
   >Sie müssen beim Arbeiten mit Platzhaltern in Adobe Workfront immer die Filtervariable **Equal** auswählen.

1. Klicken Sie auf den Umschalter **relatives Datum festlegen** und geben Sie dann im angezeigten Textfeld `$$TODAY` ein, wenn Sie Informationen zu etwas anzeigen möchten, das am selben Tag wie der Bericht ausgeführt wird.

   Oder

   Geben Sie `$$NOW` ein, wenn Sie Informationen zu etwas anzeigen möchten, das zu dem Zeitpunkt auftritt, zu dem der Bericht ausgeführt wird.

   Dieses Datum unterscheidet sich immer, da es sich mit dem Datum ändert, an dem der Bericht von einem Benutzer angezeigt wird. sodass sich die Informationen im Bericht von Tag zu Tag unterscheiden.

1. (Optional) Wenn Sie Informationen anzeigen möchten, die innerhalb eines Zeitraums nach dem Datum der Berichterstellung auftreten, geben Sie &quot;`$$TODAY+1w`&quot;ein, um Informationen in der folgenden Woche anzuzeigen, oder &quot;`$$TODAY+2m`&quot;, um Informationen in den nächsten zwei Monaten anzuzeigen. Sie können auch Zeitrahmen für Quartale, Stunden, Tage oder Jahre angeben.
1. (Optional) Wenn Sie Informationen zu etwas anzeigen möchten, das innerhalb eines Zeitraums vor dem Datum der Berichterstellung aufgetreten ist, geben Sie `$$TODAY-1w` ein, um Informationen aus der vorherigen Woche anzuzeigen, oder `$$TODAY-2m`, um Informationen aus den letzten zwei Monaten anzuzeigen. Sie können auch Zeitrahmen für Quartale, Stunden, Tage oder Jahre angeben.

   Eine vollständige Liste der Attribute, Kennungen und Operatoren, die Sie in datumsbasierten Platzhaltern verwenden können, finden Sie im Artikel [Übersicht über Wildcard-Filtervariablen](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).

1. Klicken Sie auf **Speichern + schließen**.

## Weitere Informationen

Siehe auch:

<!--outdated: * [Basic Report Creation Program](https://one.workfront.com/s/basic-report-creation-program) -->
* [Übersicht über Platzhalterfiltervariablen](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md)
* [Erstellen oder Bearbeiten von Filtern in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/create-filters.md)
* [Hinzufügen einer Eingabeaufforderung zu einem Bericht](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md)
* [Bedingte Formatierung in Ansichten verwenden](../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md)
