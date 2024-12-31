---
product-area: reporting
navigation-topic: reporting-elements
title: Verwenden benutzerbasierter Platzhalter zur Generalisierung von Berichten
description: Sie können einen Bericht generalisieren, indem Sie beim Erstellen bestimmter Berichtelemente Platzhalter anstelle spezifischer Informationen verwenden.
author: Nolan
feature: Reports and Dashboards
exl-id: 216e2869-b4f8-4cc7-9497-a12ebe00fe49
source-git-commit: 3cee374b68b26f2a423d41101300ec8b6685fadd
workflow-type: tm+mt
source-wordcount: '456'
ht-degree: 1%

---

# Verwenden benutzerbasierter Platzhalter zur Generalisierung von Berichten

<!-- Audited: 11/2024 -->

Sie können einen Bericht generalisieren, indem Sie beim Erstellen bestimmter Berichtelemente Platzhalter anstelle spezifischer Informationen verwenden. Wenn Sie beispielsweise einen Bericht erstellen möchten, der die einem bestimmten Benutzer zugewiesenen Aufgaben anzeigt, können Sie den Namen des Benutzers im Feld Zugewiesen an des Filters verwenden. Wenn Sie jedoch einen Bericht erstellen möchten, der dem angemeldeten Benutzer zugewiesene Aufgaben unabhängig davon anzeigt, wer dieser Benutzer ist, können Sie einen Platzhalter verwenden, der angibt, dass bei der Anzeige des Berichts durch eine Person nur diese betreffende Informationen angezeigt werden. Auf diese Weise erstellen Sie den Bericht nur einmal, aber da Sie im Filter einen Platzhalter verwenden, liefert er jedes Mal, wenn ihn jemand anderes liest, andere Ergebnisse.

Sie können beim Erstellen der folgenden Berichterstellungselemente benutzerbasierte Platzhalter verwenden:

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
* [Filter - Übersicht](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)
* [Eingabeaufforderung zu einem Bericht hinzufügen](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md)
* [Verwenden der bedingten Formatierung in Ansichten](../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md)
