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
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 18301970abddd8ed98abccf42562d950422bfa7c
workflow-type: tm+mt
source-wordcount: '377'
ht-degree: 0%

---

# Export historischer Daten aus [!DNL Adobe Workfront]: Vor- und Nachteile

<!-- Audited: 5/2025 -->

In diesem Artikel werden die Vor- und Nachteile von vier Optionen erläutert, mit denen Sie historische Daten aus Adobe Workfront exportieren können.

## Verwenden Sie einen unserer Partner

[!DNL AtAppStore] ([www.atappstore.com](https://www.atappstore.com)) verfügt über eine benutzerfreundliche App (die [Workfront Snapshot](https://store.atappstore.com/product/workfront-snapshot/)-Lösung), mit der Sie Ihre Daten selbst herunterladen können. Ein optionaler Viewer (die [Workfront Snapshot Viewer](https://store.atappstore.com/product/workfront-snapshot-viewer/)-Lösung) ermöglicht eine einfache Offline-Anzeige Ihrer Daten.

* **Positiv**: Alle Ihre [!DNL Workfront]-Kernobjekte, einschließlich der benutzerdefinierten Felder und Notizen, werden exportiert und in einer leicht zugänglichen [!DNL MS Access]-Datenbank gespeichert. Die Benutzeroberfläche des Viewers ist einfach zu bedienen und zu lesen. Das Extrahieren von Dokumenten ist auch separat als Service verfügbar, wobei die Ausgabe in einer logischen Ordnerstruktur organisiert ist, die jedem Dokument und seinen vorherigen Versionen zugeordnet ist.

* **Nachteile:** Es gibt eine technische Einschränkung von 2 GB an Daten, aber AtAppStore ermöglicht Ihnen nur das zu kaufen, was Sie benötigen.

* **Kosten:** Weitere Informationen finden Sie unter [https://store.atappstore.com/product/workfront-snapshot/](https://store.atappstore.com/product/workfront-snapshot/).



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

* **Kosten**: Es ist unternehmensintern.
