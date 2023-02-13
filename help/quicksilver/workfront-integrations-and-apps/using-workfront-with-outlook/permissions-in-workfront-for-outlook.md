---
product-area: workfront-integrations
navigation-topic: workfront-for-outlook
title: Berechtigungsebenen für [!DNL Workfront] für Outlook
description: Die [!DNL Workfront for Outlook] -Add-in erfordert Lese-/Schreibpostfachzugriff. Die [!DNL Workfront for Outlook] Die Integration erfordert die höchsten Berechtigungen, da sie über die Funktionalität zum Herunterladen von E-Mail-Anhängen vom Outlook Exchange-Server und zum Hochladen in verfügt. [!DNL Workfront], wenn der Benutzer eine Anforderung von einer E-Mail mit Anhängen sendet.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 704da044-21ed-4ca1-be6f-0e0aa832e069
source-git-commit: 177bf9271dca0310653b73b9100607a82290c326
workflow-type: tm+mt
source-wordcount: '451'
ht-degree: 0%

---

# Berechtigungsebenen für [!DNL Workfront for Outlook]

[!DNL Workfront for Outlook] erfordert die höchste der vier in [!DNL Outlook] -Add-Ins.

Weitere Informationen zu Berechtigungen finden Sie unter [!DNL Outlook] Add-Ins, siehe [Datenschutz, Berechtigungen und Sicherheit für [!DNL Outlook] Add-ins](https://docs.microsoft.com/en-us/office/dev/add-ins/outlook/privacy-and-security) im [!DNL Microsoft] Dokumentation.

Die [!DNL Workfront for Outlook] -Add-In erfordert Lesezugriff auf das Lese-/Schreibpostfach (`ReadWriteMailbox`), der höchste Perimeter.
Die [!DNL Workfront for Outlook] Die Integration erfordert die Berechtigungen auf höchster Ebene, da sie über die Funktion zum Herunterladen von E-Mail-Anhängen von der [!DNL Outlook] Server austauschen und sie in [!DNL Workfront], wenn der Benutzer eine Anforderung von einer E-Mail mit Anhängen sendet. Damit diese Funktion funktioniert, [!DNL Workfront for Outlook] verwendet die Funktion `mailbox.getCallbackTokenAsync()` von [!DNL Office] Add-in-JavaScript-API zum Abrufen des Tokens und Verwenden dieses API zum Herunterladen von E-Mail-Anhängen vom Exchange-Server. Die einzige Berechtigung, die die Verwendung dieser Funktion zulässt, ist `ReadWriteMailbox`. Weitere Informationen finden Sie unter [Datenschutz, Berechtigungen und Sicherheit für Outlook-Add-Ins](https://docs.microsoft.com/en-us/office/dev/add-ins/outlook/privacy-and-security) in der Microsoft-Dokumentation.

Die [!DNL Workfront for Outlook] -Add-In erfordert auch `ReadWriteItem` Berechtigung (enthalten in `ReadWriteMailbox`), das zum Lesen des E-Mail-Textteils und zum Lesen/Aktualisieren von E-Mail-Metadaten verwendet wird:

* E-Mail-Textkörper lesen:

   [!DNL Workfront for Outlook] liest den E-Mail-Textkörper, wenn ein Benutzer die Anfrage sendet oder den E-Mail-Textkörper als Update an sendet. [!DNL Adobe Workfront] Objekt.
* E-Mail-Metadaten lesen/aktualisieren:

   [!DNL Workfront for Outlook] aktualisiert E-Mail-Header, wenn ein Benutzer eine E-Mail-Anforderung sendet. Dies erfolgt zum Speichern von Informationen über die gesendeten [!DNL Adobe Workfront] -Objekt ein. Wenn der Benutzer das Add-In für dieselbe E-Mail das nächste Mal öffnet, werden die Informationen zu vorherigen Aktionen mit dieser E-Mail angezeigt.

[!DNL Workfront for Outlook] greift nur dann auf das Postfach eines Benutzers zu, wenn der Benutzer eine Aktion im Add-on ausführt. Sie verfügt über keine Hintergrundfunktionalität. Workfront for Outlook greift nur im folgenden Szenario auf das Postfach des Benutzers zu:

* Der Benutzer versucht, eine Anforderung zu senden, eine Aufgabe zu erstellen oder eine E-Mail als Update von zu senden [!DNL Workfront for Outlook] (Öffnen des Add-Ins und Auswählen einer Aktion)
   * [!DNL Workfront for Outlook] liest den E-Mail-Textkörper, der im Formular innerhalb des Add-Ins eingefügt werden soll.
   * [!DNL Workfront for Outlook] liest E-Mail-Metadaten, um Informationen zum Add-In über die vorherigen Aktionen anzuzeigen, die im Add-In mit derselben E-Mail durchgeführt wurden.
* Wenn ein Benutzer eine Anforderung sendet, eine Aufgabe erstellt oder eine E-Mail als Update von sendet [!DNL Workfront for Outlook] (Klicken Sie auf [!UICONTROL submit] im Add-In):
   * [!DNL Workfront for Outlook] liest den E-Mail-Textkörper, um ihn als Anfragebeschreibung oder Kommentar an Workfront zu senden.
   * [!DNL Workfront for Outlook] aktualisiert die E-Mail-Metadaten, um Informationen zu den gesendeten Anforderungen oder dem aktualisierten Objekt zu speichern.
   * [!DNL Workfront for Outlook] lädt E-Mail-Anhänge vom Exchange-Server herunter, um sie in gesendete Anfragen, erstellte Aufgaben oder aktualisierte Objekte hochzuladen.
