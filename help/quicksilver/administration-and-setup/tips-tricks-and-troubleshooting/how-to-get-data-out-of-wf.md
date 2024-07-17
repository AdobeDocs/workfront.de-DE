---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: "Exportieren von historischen Daten aus Adobe Workfront: Vor- und Nachteile"
description: In diesem Artikel werden die Vor- und Nachteile von 4 Optionen erläutert, mit denen Sie historische Daten aus Workfront exportieren können.
author: Courtney
feature: System Setup and Administration
role: Admin
exl-id: ed40984f-602a-46e9-a72b-141936de8fcb
source-git-commit: 5d7ff744ed0721ffa6d793a224226f28a76c57a0
workflow-type: tm+mt
source-wordcount: '504'
ht-degree: 0%

---

# Exportieren Sie historische Daten aus [!DNL Adobe Workfron]t: Vor und Nachteile

In diesem Artikel werden die Vor- und Nachteile von 4 Optionen erläutert, mit denen Sie historische Daten aus [!DNL Workfront] exportieren können.

## Verwenden Sie einen unserer Partner

[!DNL AtAppStore], ein [!DNL Workfront] zertifizierter Partner, verfügt über eine benutzerfreundliche App, mit der Sie Ihre Daten herunterladen können. Diese App enthält auch einen Viewer, mit dem Sie Ihre Daten einfach anzeigen können.

* **Vorteile:** Alle Ihre [!DNL Workfront] Objekte werden exportiert, einschließlich der benutzerdefinierten Felder. Die Benutzeroberfläche des Viewers ist einfach zu verwenden und zu lesen, und sie ist einfach in einer [!DNL MS Access]-Datenbank zu importieren.

* **Nachteile:** Dokumente werden nicht exportiert. Sie müssen sie separat herunterladen. Weitere Informationen finden Sie unter [http://www.atappstore.com/App/snapshot-to-msaccess/Default.aspx.](https://www.atappstore.com/App/snapshot-to-msaccess/Default.aspx)

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
