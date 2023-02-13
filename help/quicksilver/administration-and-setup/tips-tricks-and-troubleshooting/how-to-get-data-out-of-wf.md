---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: '"Exportieren Sie historische Daten aus Adobe Workfront: Vor- und Nachteile'
description: In diesem Artikel werden die Vor- und Nachteile von 4 Optionen erläutert, mit denen Sie historische Daten aus Workfront exportieren können.
author: Courtney
feature: System Setup and Administration
role: Admin
exl-id: ed40984f-602a-46e9-a72b-141936de8fcb
source-git-commit: f3af39e760b2b407cda5ab78497cdc775defdcf6
workflow-type: tm+mt
source-wordcount: '510'
ht-degree: 0%

---

# Exportieren Sie historische Daten aus [!DNL Adobe Workfron]t: Vor- und Nachteile

In diesem Artikel werden die Vor- und Nachteile von 4 Optionen erläutert, mit denen Sie historische Daten aus [!DNL Workfront].

## Verwenden Sie einen unserer Partner

[!DNL AtAppStore], [!DNL Workfront] zertifizierter Partner verfügt über eine benutzerfreundliche App, mit der Sie Ihre Daten herunterladen können. Diese App enthält auch einen Viewer, mit dem Sie Ihre Daten einfach anzeigen können.

* **Vorteile:** All Ihre [!DNL Workfront] -Objekte, einschließlich der benutzerdefinierten Felder, exportiert werden. Die Benutzeroberfläche des Viewers ist einfach zu verwenden und zu lesen, und sie ist leicht in einer [!DNL MS Access] Datenbank.

* **Nachteile:** Dokumente werden nicht exportiert. Sie müssen sie separat herunterladen. Weitere Informationen finden Sie unter [http://www.atappstore.com/App/snapshot-to-msaccess/Default.aspx](http://www.atappstore.com/App/snapshot-to-msaccess/Default.aspx)

## Anfordern einer [!DNL Postgres] Datendump-Datei aus unserem Datenbankteam

Ihr Kundenbetreuer kann eine Anfrage an unser Datenbankteam senden, um eine Datenbank-Dump-Datei (.dmp [!DNL Postgres] -Datei) mit Ihren Daten. Eine zusätzliche Anfrage wird an unser AOS-Team gesendet, um alle gespeicherten Dokumente abzurufen.

* **Vorteile**: Sie erhalten die gesamte Datenladezeit, einschließlich benutzerdefinierter Felder sowie von im System gespeicherten Dokumenten.

* **Nachteile**: Die Datenbankdatei ist schwer zu lesen: Sie können diese Datei nur lesen, wenn Sie sie in eine [!DNL Postgres] Datenbank erstellen und die Beziehungen zwischen den Tabellen wiederherstellen. Die Dokumente werden auf einem separaten Dateiserver gespeichert und müssen separat mithilfe eines separaten Prozesses vom AOS-Team extrahiert werden. Dabei gibt es keine Organisation für die Dokumente, und alle werden durch ihre GUID referenziert.
* **Kosten**: Dieser Download verursacht Kosten, abhängig davon, wie lange das Team benötigt, um die Datei zu erstellen. Wenden Sie sich an Ihren AEM/CAE, um weitere Informationen zu erhalten oder diesen Prozess zu starten.

## Export über [!UICONTROL Kick-Starts]

Unabhängig davon, ob Sie Remote-Beratungszeiten haben oder nicht, können Sie mit einem unserer Berater Ihre Daten in Form von Berichten exportieren oder [!UICONTROL kick-starts]oder Sie können diese Berichte selbst ausführen:

* **Vorteile**: Die Berichte sind einfach zu lesen und können in verschiedenen Anwendungen importiert werden. Sie können angepasst werden, um beliebige Gruppierungen und Ansichten einzuschließen.

* **Nachteile**: Dokumente müssen separat heruntergeladen werden.

* **Kosten**: Es ist kostenlos, wenn Sie die Berichte selbst ausführen können (Sie benötigen lediglich eine Systemadministratoranmeldung) oder die verbleibenden Remote-Beratungszeiten nutzen können. Wenn Sie sich für eine Remote-Beratung interessieren, sprechen Sie bitte mit Ihrem AE/CAE.

   Weitere Informationen zur Verwendung von Kick-Starts zum Exportieren von Daten finden Sie unter [Daten exportieren aus [!DNL Adobe Workfront] via [!UICONTROL Kick-Starts]](../../administration-and-setup/manage-workfront/using-kick-starts/export-data-from-wf-via-kick-starts.md).

## Verwenden der offenen API

Wenn Sie über die richtigen Ressourcen in Ihrer Organisation verfügen, können diese eine benutzerdefinierte API erstellen, um alle Ihre Daten aus Workfront abzurufen:

* **Vorteile**: Sie steuern, welche Exporte aus dem System ausgeführt werden.

* **Nachteile**: Die Zeit wird auf Ihrer Seite verbracht. Sie müssen Ressourcen finden, um die API zu codieren und den Export durchzuführen.

* **Kosten**: Intern zu Ihrer Organisation.
