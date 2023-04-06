---
product-area: reporting
navigation-topic: reporting-elements
title: Verwenden benutzerbasierter Platzhalter zum Generalisieren von Berichten
description: Sie können einen Bericht beim Erstellen bestimmter Berichterstellungselemente durch Verwendung von Platzhaltern anstelle spezifischer Informationen verallgemeinern.
author: Nolan
feature: Reports and Dashboards
exl-id: 216e2869-b4f8-4cc7-9497-a12ebe00fe49
source-git-commit: 302771f4d64b386149623f87a3436d0c40f421d5
workflow-type: tm+mt
source-wordcount: '508'
ht-degree: 0%

---

# Verwenden benutzerbasierter Platzhalter zum Generalisieren von Berichten

Sie können einen Bericht beim Erstellen bestimmter Berichterstellungselemente durch Verwendung von Platzhaltern anstelle spezifischer Informationen verallgemeinern. Wenn Sie beispielsweise einen Bericht erstellen möchten, der die einem bestimmten Benutzer zugewiesenen Aufgaben anzeigt, können Sie den Namen des Benutzers im Feld Zugeordneter Benutzer des Filters verwenden. Wenn Sie jedoch einen Bericht erstellen möchten, der dem angemeldeten Benutzer zugewiesene Aufgaben anzeigt, können Sie unabhängig davon, wer dieser Benutzer ist, einen Platzhalter verwenden, der anzeigt, dass bei der Anzeige des Berichts nur für ihn relevante Informationen angezeigt werden. Auf diese Weise erstellen Sie den Bericht nur einmal. Da Sie jedoch einen Platzhalter im Filter verwenden, werden bei jedem Lesen eines anderen unterschiedliche Ergebnisse ausgegeben.

Beim Erstellen der folgenden Berichterstellungselemente können Sie benutzerbasierte Platzhalter verwenden:

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

Sie müssen einen Bericht erstellen, bevor Sie ihm eine Platzhaltervariable hinzufügen können.

Anweisungen zum Erstellen von Berichten finden Sie unter [Bericht erstellen](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md).

## Anleitungsschritte

So fügen Sie einen benutzerbasierten Platzhalter in einen Bericht ein:

1. Gehen Sie zu einem Bericht, für den Sie einen benutzerbasierten Platzhalter einfügen möchten.
1. Klicken **Berichtaktionen**, dann **Bearbeiten**.

1. Klicken Sie auf **Filter** Registerkarte.
1. Klicken **Filterregel hinzufügen**.
1. Geben Sie den Namen des Felds ein, nach dem Sie filtern möchten.\
   Sie müssen Felder eingeben, die auf das Benutzerobjekt oder Informationen zu Benutzern verweisen.
1. Auswählen **Gleich** im Dropdown-Menü für die Filtervariable.

   >[!TIP]
   >
   >Sie müssen immer die **Gleich** Filtervariable beim Arbeiten mit Platzhaltern in Adobe Workfront verwenden.

1. Im **Eingabe des Namens beginnen ...** Feld, Typ: `$$USER.ID` oder `$$USER.name` , wenn der Bericht Informationen über den Benutzer anzeigen soll, der sich anmeldet, basierend auf seinem Namen. Sie können andere Platzhalter einfügen, die auf die Gruppe, das Team, das Unternehmen oder andere Informationen des angemeldeten Benutzers verweisen.

   Eine vollständige Liste der nutzerbasierten Platzhalter finden Sie unter [Platzhalterfiltervariablen](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).

   ![](assets/user-based-wildcard-in-project-filter-350x74.png)

1. Klicken **Speichern und schließen**.

## Zusätzliche Informationen

Siehe auch:

* [Grundlegendes Programm zur Berichterstellung](https://one.workfront.com/s/basic-report-creation-program)
* [Platzhalterfiltervariablen](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md)
* [Filter in Adobe Workfront erstellen oder bearbeiten](../../../reports-and-dashboards/reports/reporting-elements/create-filters.md)
* [Filterübersicht in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)
* [Hinzufügen einer Eingabeaufforderung zu einem Bericht](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md)
* [Bedingte Formatierung in Ansichten verwenden](../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md)
