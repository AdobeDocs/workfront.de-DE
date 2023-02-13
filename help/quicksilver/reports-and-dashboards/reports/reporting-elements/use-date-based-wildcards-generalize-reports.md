---
product-area: reporting
navigation-topic: reporting-elements
title: Verwenden datumsbasierter Platzhalter zum Generalisieren von Berichten
description: Sie können einen Bericht beim Erstellen bestimmter Berichterstellungselemente durch Verwendung von Platzhaltern anstelle spezifischer Informationen verallgemeinern.
author: Lisa
feature: Reports and Dashboards
exl-id: 759b0bea-729e-4206-808c-0a7216ded4ff
source-git-commit: 442e0b8fde9e4acaa2686ccd292fb003f72be623
workflow-type: tm+mt
source-wordcount: '686'
ht-degree: 0%

---

# Verwenden datumsbasierter Platzhalter zum Generalisieren von Berichten

Sie können einen Bericht beim Erstellen bestimmter Berichterstellungselemente durch Verwendung von Platzhaltern anstelle spezifischer Informationen verallgemeinern.

Wenn Sie beispielsweise einen Bericht erstellen möchten, der die Aufgaben mit einem bestimmten geplanten Startdatum anzeigt, können Sie mit der Datumsauswahl im Kalender in einem Filter ein bestimmtes Datum auswählen. Wenn Sie jedoch einen Bericht erstellen möchten, der Aufgaben anzeigt, bei denen das geplante Startdatum innerhalb eines bestimmten Zeitraums ab dem Datum des Zugriffs auf den Bericht liegt, können Sie einen Platzhalter verwenden, der angibt, dass bei der Anzeige des Berichts durch einen Benutzer Informationen für einen Zeitraum angezeigt werden, der für den Moment relevant ist, in dem der Bericht angezeigt wird.

Zum Beispiel in der vergangenen Woche, im letzten Jahr, in den nächsten zwei Wochen usw. Auf diese Weise erstellen Sie den Bericht einmal. Da Sie jedoch einen Platzhalter im Filter verwenden, werden bei jedem Lesen unterschiedliche Ergebnisse ausgegeben, da er sich an den Tag anpasst, an dem der Bericht ausgeführt wird.

Beim Erstellen der folgenden Berichterstellungselemente können Sie datumsbasierte Platzhalter verwenden:

* Filter
* Benutzerdefinierte Eingabeaufforderungen
* Ansichten beim Hinzufügen von Regeln für Spalten

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront-Plan*</strong></td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront-Lizenz*</strong></td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Konfigurationen auf Zugriffsebene*</strong></td> 
   <td> <p>Zugriff auf Filter, Ansichten, Gruppierungen bearbeiten</p> <p>Zugriff auf Berichte, Dashboards und Kalender bearbeiten, um Berichterstellungselemente in einem Bericht zu bearbeiten</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Objektberechtigungen</strong></td> 
   <td> <p>Berechtigungen für einen Bericht zum Bearbeiten von Berichterstellungselementen in einem Bericht verwalten</p> <p>Berechtigungen für Ansichten oder Filter verwalten, um sie zu bearbeiten</p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Voraussetzungen

Sie müssen einen Bericht erstellen, bevor Sie ihm Platzhaltervariablen hinzufügen können.

Informationen zum Erstellen eines Berichts finden Sie unter [Bericht erstellen](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md).

## Anleitungsschritte

So fügen Sie einen datumsbasierten Platzhalter in einen Bericht ein:

1. Gehen Sie zu einem Bericht, für den Sie einen datumsbasierten Platzhalter einfügen möchten.
1. Klicken **Berichtaktionen**, dann **Bearbeiten**.

1. Klicken Sie auf **Filter** Registerkarte.
1. Klicken **Filterregel hinzufügen**.
1. Geben Sie den Namen des Felds ein, nach dem Sie filtern möchten.\
   Sie müssen Felder eingeben, die auf ein Datum verweisen.
1. Auswählen **Gleich** im Dropdown-Menü für die Filtervariable.

   >[!TIP]
   >
   >Sie müssen immer die **Gleich** Filtervariable beim Arbeiten mit Platzhaltern in Adobe Workfront verwenden.

1. Im **Eingabe des Namens beginnen ...** Feld, Typ: `$$TODAY` , wenn Sie Informationen zu etwas anzeigen möchten, das am selben Tag auftritt, an dem der Bericht ausgeführt wird.

   Oder

   Typ `$$NOW` , wenn Sie Informationen zu etwas anzeigen möchten, das zu dem Zeitpunkt auftritt, zu dem der Bericht ausgeführt wird.

   Dieses Datum unterscheidet sich immer, da es sich mit dem Datum ändert, an dem der Bericht von einem Benutzer angezeigt wird. sodass sich die Informationen im Bericht von Tag zu Tag unterscheiden.

1. (Optional) Wenn Sie Informationen anzeigen möchten, die innerhalb eines Zeitraums nach dem Datum der Berichtsausführung auftreten, geben Sie `$$TODAY+1w` zur Anzeige von Informationen in der folgenden Woche oder `$$TODAY+2m` um Informationen in den nächsten zwei Monaten anzuzeigen. Sie können auch Zeitrahmen für Quartale, Stunden, Tage oder Jahre angeben.
1. (Optional) Wenn Sie Informationen zu etwas anzeigen möchten, das innerhalb eines Zeitraums vor dem Datum der Ausführung des Berichts aufgetreten ist, geben Sie `$$TODAY-1w` zur Anzeige von Informationen aus der Vorwoche oder `$$TODAY-2m` , um Informationen aus den beiden Vormonaten anzuzeigen. Sie können auch Zeitrahmen für Quartale, Stunden, Tage oder Jahre angeben.

   Eine vollständige Liste der Attribute, Kennungen und Operatoren, die Sie in datumsbasierten Platzhaltern verwenden können, finden Sie im Artikel [Platzhalterfiltervariablen](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).

   ![](assets/video-date-based-wildcard-in-task-filter-350x81.png)

1. Klicken **Speichern und schließen**.

## Zusätzliche Informationen

Siehe auch:

* [Grundlegendes Programm zur Berichterstellung](https://one.workfront.com/s/basic-report-creation-program)
* [Platzhalterfiltervariablen](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md)
* [Filter in Adobe Workfront erstellen oder bearbeiten](../../../reports-and-dashboards/reports/reporting-elements/create-filters.md)
* [Hinzufügen einer Eingabeaufforderung zu einem Bericht](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md)
* [Bedingte Formatierung in Ansichten verwenden](../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md)
