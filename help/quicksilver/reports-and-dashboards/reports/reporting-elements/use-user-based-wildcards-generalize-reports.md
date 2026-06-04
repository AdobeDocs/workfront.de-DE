---
product-area: reporting
navigation-topic: reporting-elements
title: Verwenden von benutzerbasierten Platzhalten zum Generalisieren von Berichten
description: Sie können einen Bericht generalisieren, indem Sie beim Erstellen bestimmter Berichtelemente Platzhalter anstelle spezifischer Informationen verwenden.
author: Courtney
feature: Reports and Dashboards
exl-id: 216e2869-b4f8-4cc7-9497-a12ebe00fe49
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/S5vsXfapgDf4fjhAPV6iet9kobyEUCM14QMF-ZvvaDc
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 457
ht-degree: 15%

---

# Verwenden von benutzerbasierten Platzhalten zum Generalisieren von Berichten

<!-- Audited: 11/2024 -->

Sie können einen Bericht generalisieren, indem Sie beim Erstellen bestimmter Berichtelemente Platzhalter anstelle spezifischer Informationen verwenden. Wenn Sie beispielsweise einen Bericht erstellen möchten, der die einem bestimmten Benutzer zugewiesenen Aufgaben anzeigt, können Sie den Namen des Benutzers im Feld Zugewiesen an des Filters verwenden. Wenn Sie jedoch einen Bericht erstellen möchten, der dem angemeldeten Benutzer zugewiesene Aufgaben unabhängig davon anzeigt, wer dieser Benutzer ist, können Sie einen Platzhalter verwenden, der angibt, dass bei der Anzeige des Berichts durch eine Person nur diese betreffende Informationen angezeigt werden. Auf diese Weise erstellen Sie den Bericht nur einmal, aber da Sie im Filter einen Platzhalter verwenden, liefert er jedes Mal, wenn ihn jemand anderes liest, andere Ergebnisse.

Sie können beim Erstellen der folgenden Berichterstellungselemente benutzerbasierte Platzhalter verwenden:

* Filter
* Benutzerdefinierte Eingabeaufforderungen
* Ansichten beim Hinzufügen von Regeln für Spalten

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Paket</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</strong></td> 
   <td> 
    <p>Standard</p>
    <p>Abo</p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriff auf Filter, Ansichten, Gruppierungen bearbeiten</p> <p>Zugriff auf Berichte, Dashboards und Kalender bearbeiten, um Berichtselemente in einem Bericht zu bearbeiten</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
    <td> <p>Verwalten der Berechtigungen für einen Bericht zum Bearbeiten von Berichtselementen in einem Bericht</p> <p>Verwalten von Berechtigungen für eine Ansicht oder einen Filter, um sie zu bearbeiten</p></td> 
   </td> 
  </tr> 
 </tbody> 
</table>

Weitere Details zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Voraussetzungen

Sie müssen einen Bericht erstellen, bevor Sie ihm eine Platzhaltervariable hinzufügen können.

Anweisungen zum Erstellen von Berichten finden Sie [Erstellen eines Berichts](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md).

## Anleitungsschritte

So fügen Sie einen benutzerbasierten Platzhalter in einen Bericht ein:

1. Navigieren Sie zu einem Bericht, für den Sie einen benutzerbasierten Platzhalter einfügen möchten.
1. Klicken Sie **Berichtsaktionen** und dann **Bearbeiten**.

1. Klicken Sie auf **Registerkarte** Filter“.
1. Klicken Sie **Filterregel hinzufügen**.
1. Geben Sie den Namen des Felds ein, nach dem Sie filtern möchten.\
   Sie müssen Felder eingeben, die auf das Benutzerobjekt oder Benutzerinformationen verweisen.
1. Wählen **im**-Menü für die Filtervariable „Gleich“ aus.

   >[!TIP]
   >
   >Bei der Arbeit mit Platzhaltern in Adobe Workfront müssen Sie immer **Filtervariable** Gleich“ auswählen.

1. Geben Sie in das Feld **Beginnen Sie mit der Eingabe des Namens…** ein: `$$USER.ID` oder `$$USER.name`, wenn der Bericht je nach Name Informationen zu dem angemeldeten Benutzer enthalten soll. Sie können auch andere Platzhalter einfügen, die sich auf die Gruppe, das Team, die Firma oder andere Informationen des angemeldeten Benutzers beziehen.

   Eine vollständige Liste der benutzerbasierten Platzhalter finden Sie unter [Übersicht über Platzhalterfiltervariablen](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).

1. Klicken Sie auf **Speichern + schließen**.

## Weitere Informationen

Siehe auch:

<!--outdated: * [Basic Report Creation Program](https://one.workfront.com/s/basic-report-creation-program) -->
* [Übersicht über Platzhalterfiltervariablen](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md)
* [Erstellen oder Bearbeiten von Filtern in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/create-filters.md)
* [Übersicht über Filter](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)
* [Eingabeaufforderung zu einem Bericht hinzufügen](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md)
* [Verwenden der bedingten Formatierung in Ansichten](../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md)
