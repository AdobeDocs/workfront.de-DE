---
product-area: reporting
navigation-topic: reporting-elements
title: Verwenden benutzerbasierter Platzhalter zum Generalisieren von Berichten
description: Sie können einen Bericht beim Erstellen bestimmter Berichterstellungselemente durch Verwendung von Platzhaltern anstelle spezifischer Informationen verallgemeinern.
author: Nolan
feature: Reports and Dashboards
exl-id: 216e2869-b4f8-4cc7-9497-a12ebe00fe49
source-git-commit: 3cee374b68b26f2a423d41101300ec8b6685fadd
workflow-type: tm+mt
source-wordcount: '456'
ht-degree: 1%

---

# Verwenden benutzerbasierter Platzhalter zum Generalisieren von Berichten

<!-- Audited: 11/2024 -->

Sie können einen Bericht beim Erstellen bestimmter Berichterstellungselemente durch Verwendung von Platzhaltern anstelle spezifischer Informationen verallgemeinern. Wenn Sie beispielsweise einen Bericht erstellen möchten, der die einem bestimmten Benutzer zugewiesenen Aufgaben anzeigt, können Sie den Namen des Benutzers im Feld Zugeordneter Benutzer des Filters verwenden. Wenn Sie jedoch einen Bericht erstellen möchten, der dem angemeldeten Benutzer zugewiesene Aufgaben anzeigt, können Sie unabhängig davon, wer dieser Benutzer ist, einen Platzhalter verwenden, der anzeigt, dass bei der Anzeige des Berichts nur für ihn relevante Informationen angezeigt werden. Auf diese Weise erstellen Sie den Bericht nur einmal. Da Sie jedoch einen Platzhalter im Filter verwenden, werden bei jedem Lesen eines anderen unterschiedliche Ergebnisse ausgegeben.

Beim Erstellen der folgenden Berichterstellungselemente können Sie benutzerbasierte Platzhalter verwenden:

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

Sie müssen einen Bericht erstellen, bevor Sie ihm eine Platzhaltervariable hinzufügen können.

Anweisungen zum Erstellen von Berichten finden Sie unter [Erstellen eines Berichts](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md).

## Schritte

So fügen Sie einen benutzerbasierten Platzhalter in einen Bericht ein:

1. Gehen Sie zu einem Bericht, für den Sie einen benutzerbasierten Platzhalter einfügen möchten.
1. Klicken Sie auf **Berichtaktionen** und dann auf **Bearbeiten**.

1. Klicken Sie auf die Registerkarte **Filter**.
1. Klicken Sie auf **Filterregel hinzufügen**.
1. Geben Sie den Namen des Felds ein, nach dem Sie filtern möchten.\
   Sie müssen Felder eingeben, die auf das Benutzerobjekt oder Informationen zu Benutzern verweisen.
1. Wählen Sie **Equal** im Dropdownmenü für die Filtervariable aus.

   >[!TIP]
   >
   >Sie müssen beim Arbeiten mit Platzhaltern in Adobe Workfront immer die Filtervariable **Equal** auswählen.

1. Geben Sie in das Feld **Name der Eingabe eingeben..** Folgendes ein: `$$USER.ID` oder `$$USER.name`, wenn der Bericht Informationen über den Benutzer anzeigen soll, der sich anmeldet, basierend auf seinem Namen. Sie können andere Platzhalter einfügen, die auf die Gruppe, das Team, das Unternehmen oder andere Informationen des angemeldeten Benutzers verweisen.

   Eine vollständige Liste der nutzerbasierten Platzhalter finden Sie unter [Übersicht über Wildcard-Filtervariablen](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).

1. Klicken Sie auf **Speichern + schließen**.

## Weitere Informationen

Siehe auch:

<!--outdated: * [Basic Report Creation Program](https://one.workfront.com/s/basic-report-creation-program) -->
* [Übersicht über Platzhalterfiltervariablen](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md)
* [Erstellen oder Bearbeiten von Filtern in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/create-filters.md)
* [Filterübersicht](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)
* [Hinzufügen einer Eingabeaufforderung zu einem Bericht](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md)
* [Bedingte Formatierung in Ansichten verwenden](../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md)
