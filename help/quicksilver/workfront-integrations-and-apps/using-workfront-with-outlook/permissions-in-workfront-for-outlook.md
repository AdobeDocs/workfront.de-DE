---
product-area: workfront-integrations
navigation-topic: workfront-for-outlook
title: Berechtigungsebenen für  [!DNL Workfront] für Outlook
description: Das [!DNL Workfront for Outlook] Add-in erfordert Lese-/Schreibpostfachzugriff. Für die Integration von [!DNL Workfront for Outlook] sind die höchsten Berechtigungen erforderlich, da sie über die Funktion zum Herunterladen von E-Mail-Anhängen vom Outlook-Exchange-Server und zum Hochladen dieser Dateien in [!DNL Workfront] verfügt, wenn der Benutzer eine Anforderung von einer E-Mail mit Anhängen sendet.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 704da044-21ed-4ca1-be6f-0e0aa832e069
source-git-commit: 177bf9271dca0310653b73b9100607a82290c326
workflow-type: tm+mt
source-wordcount: '437'
ht-degree: 0%

---

# Berechtigungsebenen für [!DNL Workfront for Outlook]

[!DNL Workfront for Outlook] erfordert die höchste der vier in [!DNL Outlook] -Add-Ins zulässigen Berechtigungsebenen.

Weitere Informationen zu Berechtigungen in [!DNL Outlook] Add-Ins finden Sie unter [Datenschutz, Berechtigungen und Sicherheit für  [!DNL Outlook] Add-Ins](https://docs.microsoft.com/en-us/office/dev/add-ins/outlook/privacy-and-security) in der Dokumentation zu [!DNL Microsoft].

Für das Add-in [!DNL Workfront for Outlook] ist der Lese-/Schreibpostfachzugriff (`ReadWriteMailbox`) erforderlich, der den höchsten Berechtigungsbereich aufweist.
Für die Integration von [!DNL Workfront for Outlook] sind die höchsten Berechtigungen erforderlich, da sie über die Funktion zum Herunterladen von E-Mail-Anhängen vom [!DNL Outlook] Exchange-Server und zum Hochladen dieser Dateien in [!DNL Workfront] verfügt, wenn der Benutzer eine Anforderung von einer E-Mail mit Anhängen sendet. Damit diese Funktion funktioniert, verwendet [!DNL Workfront for Outlook] die Funktion `mailbox.getCallbackTokenAsync()` aus der Add-in-JavaScript-API, um das Token abzurufen und diese zum Herunterladen von E-Mail-Anhängen vom Exchange-Server zu verwenden. [!DNL Office] Die einzige Berechtigung, die die Verwendung dieser Funktion zulässt, ist `ReadWriteMailbox`. Weitere Informationen finden Sie unter [Datenschutz, Berechtigungen und Sicherheit für Outlook-Add-Ins](https://docs.microsoft.com/en-us/office/dev/add-ins/outlook/privacy-and-security) in der Microsoft-Dokumentation.

Für das Add-in [!DNL Workfront for Outlook] ist auch die Berechtigung `ReadWriteItem` erforderlich (enthalten in `ReadWriteMailbox`), die zum Lesen des E-Mail-Hauptteils und zum Lesen/Aktualisieren von E-Mail-Metadaten verwendet wird:

* E-Mail-Textkörper lesen:

  [!DNL Workfront for Outlook] liest den E-Mail-Textkörper, wenn ein Benutzer die Anfrage sendet oder den E-Mail-Textkörper als Update an das [!DNL Adobe Workfront] -Objekt sendet.
* E-Mail-Metadaten lesen/aktualisieren:

  [!DNL Workfront for Outlook] aktualisiert E-Mail-Header, wenn ein Benutzer eine E-Mail-Anforderung sendet. Dadurch werden Informationen zum gesendeten [!DNL Adobe Workfront] -Objekt gespeichert, sodass beim nächsten Öffnen des Add-Ins für dieselbe E-Mail die Informationen zu vorherigen Aktionen mit dieser E-Mail angezeigt werden.

[!DNL Workfront for Outlook] greift nur dann auf das Postfach eines Benutzers zu, wenn der Benutzer eine Aktion innerhalb des Add-ons ausführt. Sie verfügt über keine Hintergrundfunktionalität. Workfront for Outlook greift nur im folgenden Szenario auf das Postfach des Benutzers zu:

* Der Benutzer versucht, eine Anforderung zu senden, eine Aufgabe zu erstellen oder eine E-Mail als Update von [!DNL Workfront for Outlook] zu senden (Öffnen des Add-Ins und Auswählen einer Aktion)
   * [!DNL Workfront for Outlook] liest den E-Mail-Textkörper, der im Formular innerhalb des Add-Ins eingefügt werden soll.
   * [!DNL Workfront for Outlook] liest E-Mail-Metadaten, um Informationen über das Add-In zu den vorherigen Aktionen anzuzeigen, die im Add-In mit derselben E-Mail durchgeführt wurden.
* Wenn ein Benutzer eine Anforderung sendet, eine Aufgabe erstellt oder eine E-Mail als Update von [!DNL Workfront for Outlook] sendet (indem er auf die Schaltfläche [!UICONTROL submit] im Add-In klickt):
   * [!DNL Workfront for Outlook] liest den E-Mail-Textkörper, um ihn als Anfragebeschreibung oder Kommentar an Workfront zu senden.
   * [!DNL Workfront for Outlook] aktualisiert die E-Mail-Metadaten, um Informationen zu den gesendeten Anforderungen oder dem aktualisierten Objekt zu speichern.
   * [!DNL Workfront for Outlook] lädt E-Mail-Anhänge vom Exchange-Server herunter, um sie in gesendete Anfragen, erstellte Aufgaben oder aktualisierte Objekte hochzuladen.
