---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: "Exportieren historischer Daten aus Adobe Workfront: Vorteile und Nachteile"
description: In diesem Artikel werden die Vor- und Nachteile von 4 Optionen erläutert, mit denen Sie historische Daten aus Workfront exportieren können.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: ed40984f-602a-46e9-a72b-141936de8fcb
source-git-commit: 55c8a3e5d0041a0e975bfd979a2d2e38930fea8d
workflow-type: tm+mt
source-wordcount: '557'
ht-degree: 0%

---

# Exportieren Sie historische Daten aus [!DNL Adobe Workfron]t: Vor und Nachteile

In diesem Artikel werden die Vor- und Nachteile von vier Optionen erläutert, mit denen Sie historische Daten aus [!DNL Workfront] exportieren können.

## Verwenden Sie einen unserer Partner

[!DNL AtAppStore] ([www.atappstore.com](https://www.atappstore.com)) verfügt über eine benutzerfreundliche App (ihre [Workfront Snapshot](https://store.atappstore.com/product/workfront-snapshot/) -Lösung), mit der Sie Ihre Daten selbst herunterladen können. Mit einem optionalen Viewer (mit der Lösung [Workfront Snapshot Viewer](https://store.atappstore.com/product/workfront-snapshot-viewer/) ) können Sie Ihre Daten einfach offline anzeigen.

* **Vorteile:** Alle Ihre Core [!DNL Workfront]-Objekte werden exportiert, einschließlich der benutzerdefinierten Felder und Hinweise, die alle dann in einer leicht zugänglichen [!DNL MS Access]-Datenbank gespeichert werden. Die Benutzeroberfläche des Viewers ist einfach zu verwenden und zu lesen. Das Extrahieren von Dokumenten ist auch separat als Dienst verfügbar, wobei die Ausgabe in einer logischen Ordnerstruktur organisiert ist, die den einzelnen Dokumenten (und optional den vorherigen Versionen) zugeordnet ist.

* **Nachteile:** Es gibt eine technische Beschränkung von 2 GB an Daten. Mit AtAppStore können Sie jedoch nur das kaufen, was Sie benötigen.

* **Kosten:** Weitere Informationen finden Sie unter [https://store.atappstore.com/product/workfront-snapshot/](https://store.atappstore.com/product/workfront-snapshot/).

## Eine [!DNL Postgres]-Datendump-Datei von unserem Datenbankteam anfordern

Ihr Kundenbetreuer kann eine Anfrage an unser Datenbankteam senden, um eine Datenbank-Dump-Datei (.dmp [!DNL Postgres] -Datei) mit Ihren Daten zu exportieren. Eine zusätzliche Anfrage wird an unser AOS-Team gesendet, um alle gespeicherten Dokumente abzurufen.

* **Vorteile**: Sie erhalten die gesamte Datenladung, einschließlich benutzerdefinierter Felder, sowie Dokumente, die im System gespeichert sind.

* **Nachteile**: Die Datenbankdatei ist schwer zu lesen: Sie können diese Datei nur lesen, wenn Sie sie in eine [!DNL Postgres] -Datenbank hochladen und die Beziehungen zwischen den Tabellen wiederherstellen. Die Dokumente werden auf einem separaten Dateiserver gespeichert und müssen separat mithilfe eines separaten Prozesses vom AOS-Team extrahiert werden. Dabei gibt es keine Organisation für die Dokumente, und alle werden durch ihre GUID referenziert.

* **Kosten**: Dieser Download verursacht Kosten, die davon abhängen, wie lange das Team benötigt, um die Datei zu erstellen. Wenden Sie sich an Ihren AEM/CAE, um weitere Informationen zu erhalten oder diesen Prozess zu starten.

## Export über [!UICONTROL Kick-Starts]

Unabhängig davon, ob Sie über Remote-Beratungszeiten verfügen oder nicht, können Sie Ihre Daten mit einem unserer Berater in Form von Berichten oder [!UICONTROL kick-starts] exportieren oder diese Berichte selbst ausführen:

* **Vorteile**: Berichte sind einfach zu lesen und können in verschiedenen Anwendungen importiert werden. Sie können angepasst werden, um beliebige Gruppierungen und Ansichten einzuschließen.

* **Nachteile**: Dokumente müssen separat heruntergeladen werden.

* **Kosten**: Es ist kostenlos, wenn Sie die Berichte selbst ausführen können (Sie benötigen lediglich eine Systemadministratoranmeldung) oder die verbleibenden Remote-Beratungszeiten nutzen können. Wenn Sie sich für eine Remote-Beratung interessieren, sprechen Sie bitte mit Ihrem AE/CAE.

  Weitere Informationen zur Verwendung von Kick-Starts zum Exportieren von Daten finden Sie unter [Exportieren von Daten aus  [!DNL Adobe Workfront] über [!UICONTROL Kick-Starts]](../../administration-and-setup/manage-workfront/using-kick-starts/export-data-from-wf-via-kick-starts.md).

## Verwenden der offenen API

Wenn Sie über die richtigen Ressourcen in Ihrer Organisation verfügen, können diese eine benutzerdefinierte API erstellen, um alle Ihre Daten aus Workfront abzurufen:

* **Vorteile**: Sie steuern, welche Exporte aus dem System ausgeführt werden.

* **Nachteile**: Die Zeit wird auf Ihrer Seite verbracht. Sie müssen Ressourcen finden, um die API zu codieren und den Export durchzuführen.

* **Kosten**: Intern zu Ihrem Unternehmen.
