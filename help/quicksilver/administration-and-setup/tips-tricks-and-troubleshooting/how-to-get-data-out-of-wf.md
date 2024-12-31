---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 'Exportieren von historischen Daten aus Adobe Workfront: Vor- und Nachteile'
description: In diesem Artikel werden die Vor- und Nachteile von vier Optionen erläutert, mit denen Sie historische Daten aus Workfront exportieren können.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: ed40984f-602a-46e9-a72b-141936de8fcb
source-git-commit: db0aab0e6e7e896a8e7c0afe2da709de7c3c2a4e
workflow-type: tm+mt
source-wordcount: '565'
ht-degree: 0%

---

# Export historischer Daten aus [!DNL Adobe Workfront]: Vor- und Nachteile

In diesem Artikel werden die Vor- und Nachteile von vier Optionen erläutert, mit denen Sie historische Daten aus [!DNL Workfront] exportieren können.

## Verwenden Sie einen unserer Partner

[!DNL AtAppStore] ([www.atappstore.com](https://www.atappstore.com)) verfügt über eine benutzerfreundliche App (die [Workfront Snapshot](https://store.atappstore.com/product/workfront-snapshot/)-Lösung), mit der Sie Ihre Daten selbst herunterladen können. Ein optionaler Viewer (die [Workfront Snapshot Viewer](https://store.atappstore.com/product/workfront-snapshot-viewer/)-Lösung) ermöglicht eine einfache Offline-Anzeige Ihrer Daten.

* **Positiv** Alle Ihre [!DNL Workfront]-Kernobjekte werden exportiert, einschließlich der benutzerdefinierten Felder und Notizen, die alle in einer leicht zugänglichen [!DNL MS Access]-Datenbank gespeichert werden. Die Benutzeroberfläche des Viewers ist einfach zu bedienen und zu lesen. Das Extrahieren von Dokumenten ist auch separat als Service verfügbar, wobei die Ausgabe in einer logischen Ordnerstruktur organisiert ist, die jedem Dokument (und optional seinen vorherigen Versionen) zugeordnet ist.

* **Nachteile:** Es gibt eine technische Einschränkung von 2 GB an Daten, aber AtAppStore ermöglicht Ihnen nur das zu kaufen, was Sie benötigen.

* **Kosten:** Weitere Informationen finden Sie unter [https://store.atappstore.com/product/workfront-snapshot/](https://store.atappstore.com/product/workfront-snapshot/).

## Fordern Sie eine [!DNL Postgres]-Daten-Dump-Datei von unserem Datenbank-Team an

Sie müssen eine Anfrage an unser Kundensupportteam senden, das dann eine Anfrage an unser Datenbankteam sendet, um eine Datenbank-Dump-Datei (.dmp-[!DNL Postgres]-Datei) mit Ihren Daten zu exportieren. Eine zusätzliche Anfrage wird an unser NOC-Team gesendet, um alle Ihre gespeicherten Dokumente abzurufen.

* **Vorteile**: Sie erhalten Ihre gesamte Datenlast, einschließlich benutzerdefinierter Felder sowie Dokumente, die im System gespeichert sind.

* **Nachteile**: Die Datenbankdatei ist schwer lesbar: Sie können diese Datei nur lesen, wenn Sie sie in eine [!DNL Postgres] Datenbank hochladen und die Beziehungen zwischen den Tabellen wiederherstellen. Die Dokumente werden auf einem separaten Dateiserver gespeichert und müssen vom NOC-Team in einem separaten Prozess separat extrahiert werden. Dadurch gibt es keine Organisation für die Dokumente, und sie werden alle durch ihre GUID referenziert.

* **Kosten**: Mit diesem Download sind Kosten verbunden, je nachdem, wie lange das Team braucht, um die Datei zu erstellen. Wenden Sie sich an Ihren AEM/CAE, um weitere Informationen zu erhalten oder diesen Prozess zu starten.

## Exportieren über [!UICONTROL Kickstarts]

Unabhängig davon, ob Sie Remote-Beratungszeiten haben oder nicht, können Sie einen unserer Berater verwenden, um Ihre Daten in Form von Berichten oder [!UICONTROL Kickstarts] zu exportieren, oder Sie können diese Berichte selbst ausführen:

* **Positiv**: Die Berichte sind einfach zu lesen und können in eine Vielzahl von Anwendungen importiert werden. Sie können so angepasst werden, dass sie beliebige Gruppierungen und Ansichten enthalten.

* **Nachteile**: Dokumente müssen separat heruntergeladen werden.

* **Kosten**: Es ist kostenlos, wenn Sie die Berichte selbst ausführen können (Sie benötigen lediglich eine Anmeldung als Systemadministrator) oder wenn Sie die verbleibenden Stunden der Remote-Beratung nutzen können. Wenn Sie daran interessiert sind, Remote-Beratung für diese zu erwerben, wenden Sie sich bitte an Ihren AE/CAE.

  Weitere Informationen zur Verwendung von Kickstarts zum Exportieren von Daten finden Sie unter [Exportieren von Daten  [!DNL Adobe Workfront] über [!UICONTROL Kickstarts]](../../administration-and-setup/manage-workfront/using-kick-starts/export-data-from-wf-via-kick-starts.md).

## Verwenden unserer offenen API

Wenn Sie in Ihrem Unternehmen über die richtigen Ressourcen verfügen, können diese eine benutzerdefinierte API zum Abrufen aller Daten aus Workfront erstellen:

* **Vorteile**: Sie haben die Kontrolle darüber, was aus dem System exportiert.

* **Nachteile**: Die Zeit wird auf Ihrer Seite verbracht, und Sie müssen Ressourcen finden, um die API zu codieren und den Export durchzuführen.

* **Kosten**: Intern in Ihrer Organisation.
