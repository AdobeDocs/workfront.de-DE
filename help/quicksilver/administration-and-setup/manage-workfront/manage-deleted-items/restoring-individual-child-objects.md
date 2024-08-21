---
user-type: administrator
product-area: system-administration
navigation-topic: manage-deleted-items
title: Einzelne untergeordnete Objekte wiederherstellen
description: In diesem Dokument wird beschrieben, wie Sie Hilfe beim Wiederherstellen einzelner untergeordneter Objekte erhalten, die in weniger als 30 Tagen zuvor aus Ihrer Adobe Workfront-Produktions- oder Vorschau-Umgebung gelöscht wurden.
feature: System Setup and Administration
role: Admin
author: Lisa
exl-id: e2e4fbb7-5433-4d88-8e36-d82f4cc8a194
source-git-commit: 01487bb9cb195d6fa89bbe0fbdb7678254642714
workflow-type: tm+mt
source-wordcount: '582'
ht-degree: 0%

---

# Einzelne untergeordnete Objekte wiederherstellen

In diesem Dokument wird beschrieben, wie Sie Hilfe beim Wiederherstellen einzelner untergeordneter Objekte erhalten, die in weniger als 30 Tagen zuvor aus Ihrer Adobe Workfront-Produktions- oder Vorschau-Umgebung gelöscht wurden.

Ein Workfront-Administrator kann Projekte, Aufgaben, Probleme und Dokumente in jeder Workfront-Instanz wiederherstellen, wie unter [Gelöschte Elemente wiederherstellen](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md) beschrieben. Nur das Workfront-Datenbankteam kann Objekte wie Aufgaben, Probleme, Dokumente, benutzerdefinierte Formulare, Stunden und Notizen unabhängig vom übergeordneten Objekt wiederherstellen.

Daten aus Ihrer Live-Umgebung stehen in der Vorschau-Sandbox für bis zu 7 Tage zur Verfügung. Dies bedeutet, dass Sie die eigenständigen Daten mithilfe der folgenden Methoden aus der Sandbox-Vorschau exportieren können:

* Kickstarts
* Erstellen eines Berichts und Exportieren der Ergebnisse

Weitere Informationen zum Exportieren von Daten aus Workfront finden Sie unter [Daten exportieren](../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md).

Sie können die exportierten Daten wie folgt importieren:

* Manuell, wenn Sie exportierte Berichte verwenden
* Wenn Sie Kick-Starts gemeinsam verwenden

  Weitere Informationen zum Importieren von Daten in Workfront mithilfe von Kick-Starts finden Sie unter [Importieren von Daten in Adobe Workfront mithilfe einer Kick-Start-Vorlage](../../../administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md).

Die Vorschau-Sandbox-Umgebung wird während unserer Wartungsfenster am Wochenende aktualisiert.

Weitere Informationen zu den Wartungsfenstern für die Vorschau-Sandbox-Umgebung finden Sie unter [Adobe-Status-Site](https://status.adobe.com/de).

>[!IMPORTANT]
>
>Dokumente bilden eine Ausnahme zu diesen Wiederherstellungsmethoden. Sie können sie manuell aus der Vorschau-Umgebung herunterladen und erneut in die Produktionsumgebung hochladen. Wenn Sie Dokumente stapelweise herunterladen und hochladen möchten, müssen Sie eine Datenwiederherstellung von Workfront anfordern.

## Für die Wiederherstellung benötigte Informationen

Nachdem Sie festgestellt haben, dass ein gelöschtes Objekt von unserem Datenbankteam wiederhergestellt werden muss, sammeln Sie so viele Informationen wie Sie darüber haben. Die folgenden Informationen sind erforderlich, damit unsere Datenbankadministratoren das Objekt finden und eine Wiederherstellung starten können:

* Objektname
* Objekttyp (Aufgabe, Problem, Projekt usw.)
* Geschätztes Datum und Uhrzeit der Löschung
* Objekt-GUID (sofern möglich)

  Beachten Sie beim Suchen der GUID eines Objekts die folgenden Informationen:

   * Die GUID kann gefunden werden, indem auf E-Mail-Benachrichtigungen verwiesen wird, die durch die Interaktion mit dem Objekt ausgelöst werden (Zuweisungen an , Kommentare usw.)
   * Beispiel einer GUID am Ende einer URL: `yourdomain.my.workfront.com/issue/view?ID=568bfa96011220154c8ca4c4e691556b`

Wenn Sie diese Informationen gesammelt haben oder Hilfe benötigen, wenden Sie sich bitte an unser Support-Team unter 844-306-HELP(4357) oder senden Sie ein Ticket online.

## Datenwiederherstellungsprozess

1. Nachdem unser Support-Team Ihre Informationen erhalten hat, wird es an unser Support-Team eskalieren.
1. Unser Support-Team wird sich an unser Datenbankteam wenden.
1. Sobald das Datenbankteam die Möglichkeit hatte, die wiederhergestellten Daten zu überprüfen, kann eine genauere Schätzung für die ETA bereitgestellt werden. Eine Wiederherstellung dauert in der Regel drei Tage, kann jedoch je nach Art und Umfang der wiederherzustellenden Daten länger dauern.
1. Das Datenbankteam stellt die Informationen in Ihrer Sandbox-Vorschau-Umgebung wieder her, in der Sie die wiederhergestellten Daten überprüfen können. Unser Support-Team teilt Ihnen mit, wann die Daten in der Vorschau-Sandbox zu finden sind.
1. Sobald Sie mit der Wiederherstellung in der Sandbox zufrieden sind, teilen Sie dies unserem Support-Team mit. Dieses wird sich dann an unser Datenbankteam wenden, um Ihnen mitzuteilen, dass es die Daten in Ihrer Produktionsumgebung wiederherstellen kann.
1. Sie haben die Möglichkeit, die wiederhergestellten Daten zu überprüfen, bevor die Anfrage geschlossen wird.
