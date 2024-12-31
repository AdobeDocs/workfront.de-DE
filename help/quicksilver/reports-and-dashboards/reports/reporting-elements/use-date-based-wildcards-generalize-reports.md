---
product-area: reporting
navigation-topic: reporting-elements
title: Verwenden von datumsbasierten Platzhaltern zum Generalisieren von Berichten
description: Sie können einen Bericht generalisieren, indem Sie beim Erstellen bestimmter Berichtelemente Platzhalter anstelle spezifischer Informationen verwenden.
author: Nolan
feature: Reports and Dashboards
exl-id: 759b0bea-729e-4206-808c-0a7216ded4ff
source-git-commit: 3cee374b68b26f2a423d41101300ec8b6685fadd
workflow-type: tm+mt
source-wordcount: '644'
ht-degree: 1%

---

# Verwenden von datumsbasierten Platzhaltern zum Generalisieren von Berichten

<!-- Audited: 11/2024 -->

Sie können einen Bericht generalisieren, indem Sie beim Erstellen bestimmter Berichtelemente Platzhalter anstelle spezifischer Informationen verwenden.

Wenn Sie beispielsweise einen Bericht erstellen möchten, der die Aufgaben mit einem bestimmten geplanten Startdatum ausgibt, können Sie die Datumsauswahl im Kalender in einem Filter verwenden, um ein bestimmtes Datum auszuwählen. Wenn Sie jedoch einen Bericht erstellen möchten, der Aufgaben ausgibt, die das geplante Startdatum innerhalb eines bestimmten Zeitraums ab dem Datum des Berichtzugriffs haben, können Sie einen Platzhalter verwenden, der angibt, dass Informationen für einen Zeitraum angezeigt werden, der für den Zeitpunkt relevant ist, zu dem der Bericht angezeigt wird, wenn jemand den Bericht aufruft.

Zum Beispiel in der letzten Woche, im letzten Jahr, in den nächsten zwei Wochen usw. Auf diese Weise erstellen Sie den Bericht nur einmal, aber da Sie im Filter einen Platzhalter verwenden, liefert er jedes Mal andere Ergebnisse, wenn jemand ihn liest, da er sich an den Tag anpasst, an dem der Bericht ausgeführt wird.

Sie können beim Erstellen der folgenden Berichterstellungselemente datumsbasierte Platzhalter verwenden:

* Filter
* Benutzerdefinierte Eingabeaufforderungen
* Ansichten beim Hinzufügen von Regeln für Spalten

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

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
   <td role="rowheader"><strong>Konfigurationen der Zugriffsebene*</strong></td> 
   <td> <p>Zugriff auf Filter, Ansichten, Gruppierungen bearbeiten</p> <p>Zugriff auf Berichte, Dashboards und Kalender bearbeiten, um Berichtselemente in einem Bericht zu bearbeiten</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Objektberechtigungen</strong></td> 
   <td> <p>Verwalten der Berechtigungen für einen Bericht zum Bearbeiten von Berichtselementen in einem Bericht</p> <p>Verwalten von Berechtigungen für eine Ansicht oder einen Filter, um sie zu bearbeiten</p></td> 
  </tr> 
 </tbody> 
</table>

*Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Voraussetzungen

Sie müssen einen Bericht erstellen, bevor Sie Platzhaltervariablen hinzufügen können.

Informationen zum Erstellen eines Berichts finden Sie unter [Erstellen eines Berichts](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md).

## Anleitungsschritte

So fügen Sie einen datumsbasierten Platzhalter in einen Bericht ein:

1. Wechseln Sie zu einem Bericht, für den Sie einen datumsbasierten Platzhalter einfügen möchten.
1. Klicken Sie **Berichtsaktionen** und dann **Bearbeiten**.
1. Klicken Sie auf **Registerkarte** Filter“.
1. Klicken Sie **Filterregel hinzufügen**.
1. Geben Sie den Namen des Felds ein, nach dem Sie filtern möchten.\
   Sie müssen Felder eingeben, die auf ein Datum verweisen.
1. Wählen **im**-Menü für die Filtervariable „Gleich“ aus.

   >[!TIP]
   >
   >Bei der Arbeit mit Platzhaltern in Adobe Workfront müssen Sie immer **Filtervariable** Gleich“ auswählen.

1. Klicken Sie auf **Umschalter** Relatives Datum festlegen) und geben Sie in das daraufhin angezeigte Textfeld ein: `$$TODAY`, wenn Sie Informationen zu einem Vorgang anzeigen möchten, der am Tag der Berichtsausführung stattfindet.

   Oder

   Geben Sie `$$NOW` ein, wenn Sie Informationen zu einem Vorgang anzeigen möchten, der zum gleichen Zeitpunkt wie der Bericht erfolgt.

   Dieses Datum ist immer anders, da es sich mit dem Datum ändert, an dem der Bericht von einem Benutzer tatsächlich angezeigt wird. Die Informationen im Bericht unterscheiden sich also von Tag zu Tag.

1. (Optional) Wenn Sie Informationen anzeigen möchten, die innerhalb eines Zeitraums nach dem Datum der Berichtsausführung auftreten, geben Sie `$$TODAY+1w` ein, um Informationen in der folgenden Woche anzuzeigen, oder `$$TODAY+2m`, um Informationen in den nächsten zwei Monaten anzuzeigen. Sie können auch Zeitrahmen für Quartale, Stunden, Tage oder Jahre angeben.
1. (Optional) Wenn Sie Informationen zu einem Vorgang anzeigen möchten, der innerhalb eines Zeitraums vor dem Datum der Berichtsausführung stattgefunden hat, geben Sie `$$TODAY-1w` ein, um Informationen aus der vorherigen Woche anzuzeigen, oder `$$TODAY-2m` Sie Informationen aus den vorherigen zwei Monaten anzeigen. Sie können auch Zeitrahmen für Quartale, Stunden, Tage oder Jahre angeben.

   Eine vollständige Liste der Attribute, Qualifizierer und Operatoren, die Sie in datumsbasierten Platzhaltern verwenden können, finden Sie im Artikel [Übersicht über Platzhalterfiltervariablen](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).

1. Klicken Sie auf **Speichern + schließen**.

## Weitere Informationen

Siehe auch:

<!--outdated: * [Basic Report Creation Program](https://one.workfront.com/s/basic-report-creation-program) -->
* [Übersicht über Platzhalterfiltervariablen](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md)
* [Erstellen oder Bearbeiten von Filtern in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/create-filters.md)
* [Eingabeaufforderung zu einem Bericht hinzufügen](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md)
* [Verwenden der bedingten Formatierung in Ansichten](../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md)
