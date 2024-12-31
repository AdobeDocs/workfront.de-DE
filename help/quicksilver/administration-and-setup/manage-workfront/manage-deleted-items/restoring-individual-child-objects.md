---
user-type: administrator
product-area: system-administration
navigation-topic: manage-deleted-items
title: Wiederherstellen einzelner untergeordneter Objekte
description: In diesem Artikel wird beschrieben, wie Sie Hilfe beim Wiederherstellen einzelner untergeordneter Objekte erhalten können, die vor weniger als 30 Tagen aus Ihrer Adobe Workfront-Produktions- oder Vorschau-Umgebung gelöscht wurden.
feature: System Setup and Administration
role: Admin
author: Lisa
exl-id: e2e4fbb7-5433-4d88-8e36-d82f4cc8a194
source-git-commit: dc64fef83c2b1e9f8bf9438017155bd47b83ab23
workflow-type: tm+mt
source-wordcount: '641'
ht-degree: 0%

---

# Wiederherstellen einzelner untergeordneter Objekte

In diesem Artikel wird beschrieben, wie Sie Hilfe beim Wiederherstellen einzelner untergeordneter Objekte erhalten können, die vor weniger als 30 Tagen aus Ihrer Adobe Workfront-Produktions- oder Vorschau-Umgebung gelöscht wurden.

Ein Workfront-Administrator kann Projekte, Aufgaben, Probleme und Dokumente in jeder Workfront-Instanz wiederherstellen, wie in [Wiederherstellen gelöschter Elemente](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md) beschrieben. Nur das Workfront-Datenbankteam kann jedoch Objekte wie Aufgaben, Probleme, Dokumente, benutzerdefinierte Formulare, Stunden und Notizen unabhängig vom übergeordneten Objekt wiederherstellen.

Daten aus Ihrer Live-Umgebung sind in der Sandbox-Vorschau bis zu sieben Tage lang verfügbar. Das bedeutet, dass Sie die eigenständigen Daten aus der Sandbox-Vorschau-Umgebung mit den folgenden Methoden exportieren können:

* Kickstarts
* Erstellen eines Berichts und Exportieren der Ergebnisse

Weitere Informationen zum Exportieren von Daten aus Workfront finden Sie unter [Exportieren von Daten](../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md).

Sie können die exportierten Daten wie folgt importieren:

* Manuell, wenn Sie exportierte Berichte verwenden
* Wenn Sie Kickstarts massenweise verwenden,

  Weitere Informationen zum Importieren von Daten in Workfront mithilfe von Kickstarts finden Sie unter [Importieren von Daten in Adobe Workfront mithilfe einer Kickstart-Vorlage](../../../administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md).

Die Sandbox-Vorschau-Umgebung wird während unserer Wartungsfenster am Wochenende aktualisiert.

Weitere Informationen zu den Wartungsfenstern für die Sandbox-Vorschau-Umgebung finden Sie auf [der Adobe-Status-Site](https://status.adobe.com/de).

>[!IMPORTANT]
>
>Dokumente stellen eine Ausnahme zu diesen Wiederherstellungsmethoden dar. Sie können sie manuell aus der Vorschau-Umgebung herunterladen und erneut in die Produktionsumgebung hochladen. Wenn Sie Dokumente stapelweise herunterladen und hochladen möchten, müssen Sie eine Datenwiederherstellung von Workfront anfordern.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan</td> 
   <td>Beliebig</td> 
  </tr> 
  <tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td><p>Neu: Standard</p>
       <p>Oder</p>
       <p>Aktuell: Plan</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td>[!UICONTROL Systemadministrator]</td>
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Für eine Datenwiederherstellung erforderliche Informationen

Nachdem Sie festgestellt haben, dass ein gelöschtes Objekt von unserem Datenbank-Team wiederhergestellt werden muss, sammeln Sie so viele Informationen wie möglich darüber. Die folgenden Informationen sind für unsere Datenbankadministratoren erforderlich, um das Objekt zu finden und eine Wiederherstellung zu starten:

* Objektname
* Objekttyp (Aufgabe, Problem, Projekt usw.)
* Geschätztes Datum und voraussichtliche Uhrzeit des Löschvorgangs
* Objekt-GUID (falls möglich)

  Siehe die folgenden Informationen, wenn Sie die GUID eines -Objekts finden:

   * Die GUID finden Sie durch Referenzieren von E-Mail-Benachrichtigungen, die durch die Interaktion mit dem -Objekt ausgelöst werden (Zuweisungen an , Kommentare zu usw.).
   * Beispiel einer GUID am Ende einer URL: `yourdomain.my.workfront.com/issue/view?ID=568bfa96011220154c8ca4c4e691556b`

Wenn Sie diese Informationen gesammelt haben oder Hilfe benötigen, wenden Sie sich bitte an unser Kundensupportteam unter 844-306-HELP(4357) oder reichen Sie ein Ticket online ein.

## Datenwiederherstellungsprozess

1. Nachdem unser Kundensupportteam Ihre Informationen erhalten hat, wird es sie an unser Kundensupportteam weiterleiten.
1. Unser Kundensupportteam wird sich mit unserem Datenbankteam in Verbindung setzen.
1. Sobald das Datenbank-Team die Möglichkeit hatte, die wiederherzustellenden Daten zu überprüfen, kann eine genauere Schätzung für die ETA bereitgestellt werden. Eine Wiederherstellung dauert in der Regel drei Tage, kann jedoch je nach Typ und Volumen der wiederherzustellenden Daten länger dauern.
1. Das Datenbank-Team stellt die Informationen in Ihrer Sandbox-Vorschau-Umgebung wieder her, in der Sie die wiederhergestellten Daten überprüfen können. Unser Support-Team teilt Ihnen mit, wann die Daten in der Vorschau-Sandbox zu finden sind.
1. Wenn Sie mit der Wiederherstellung in der Sandbox zufrieden sind, informieren Sie unser Kunden-Support-Team darüber. Dieses wird sich dann an unser Datenbank-Team wenden, um es darüber zu informieren, dass es die Daten in Ihrer Produktionsumgebung wiederherstellen kann.
1. Sie haben die Möglichkeit, die wiederhergestellten Daten zu überprüfen, bevor die Anfrage geschlossen wird.
