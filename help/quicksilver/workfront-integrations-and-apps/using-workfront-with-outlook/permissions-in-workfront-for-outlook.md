---
product-area: workfront-integrations
navigation-topic: workfront-for-outlook
title: Berechtigungsebenen für  [!DNL Workfront]  Outlook
description: Das  [!DNL Workfront for Outlook] -Add-In erfordert Lese-/Schreibzugriff auf das Postfach. Die  [!DNL Workfront for Outlook] -Integration erfordert Berechtigungen auf höchster Ebene, da sie über die Funktion verfügt, E-Mail-Anhänge vom Outlook Exchange-Server herunterzuladen und in hochzuladen [!DNL Workfront] wenn der Benutzer eine Anfrage über eine E-Mail mit Anhängen sendet.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 704da044-21ed-4ca1-be6f-0e0aa832e069
source-git-commit: b4b45bbc8bb68dbac35488c1777fca85fa0cc7e3
workflow-type: tm+mt
source-wordcount: '548'
ht-degree: 0%

---

# Berechtigungsebenen für [!DNL Workfront for Outlook]

>[!IMPORTANT]
>
>[Microsoft deaktiviert die Unterstützung für veraltete Exchange Online-Token](https://learn.microsoft.com/en-us/office/dev/add-ins/outlook/faq-nested-app-auth-outlook-legacy-tokens), die derzeit vom Workfront Outlook-Add-in zur Authentifizierung verwendet werden. Diese Änderung durch Microsoft hat bereits Auswirkungen auf Kunden und wird bis Oktober 2025 schrittweise eingeführt.
>
>* **Nachdem Microsoft diese Token vollständig deaktiviert hat, funktioniert die Integration von Workfront für Microsoft Outlook nicht mehr.**
>
>Im Rahmen dieser Änderung hat Microsoft die Entscheidung getroffen, die Art und Weise zu ändern, wie Token wieder aktiviert werden. Nach dem **30. Juni** können Administratoren Token nicht mehr selbst erneut aktivieren - nur der Microsoft-Support kann Ausnahmen gewähren. **Am 1. Oktober 2025 werden alte Token für alle Mandanten deaktiviert. Ausnahmen werden nicht gewährt.**


[!DNL Workfront for Outlook] erfordert die höchste der vier in [!DNL Outlook] Add-Ins zulässigen Berechtigungsebenen.

Weitere Informationen zu Berechtigungen in [!DNL Outlook]-Add-Ins finden Sie [Datenschutz, Berechtigungen und Sicherheit für  [!DNL Outlook] -Add-Ins](https://docs.microsoft.com/en-us/office/dev/add-ins/outlook/privacy-and-security) in der [!DNL Microsoft].

Das [!DNL Workfront for Outlook]-Add-in erfordert Lese-/Schreibzugriff auf das Postfach (`ReadWriteMailbox`), was der höchste Berechtigungsumfang ist.
Die [!DNL Workfront for Outlook]-Integration erfordert Berechtigungen auf höchster Ebene, da sie die Möglichkeit bietet, E-Mail-Anhänge vom [!DNL Outlook] Exchange-Server herunterzuladen und in [!DNL Workfront] hochzuladen, wenn der Benutzer eine Anfrage über eine E-Mail mit Anhängen sendet. Damit diese Funktion funktioniert, verwendet [!DNL Workfront for Outlook] die Funktion `mailbox.getCallbackTokenAsync()` von [!DNL Office] Add-In-JavaScript-API , um das Token abzurufen, und verwendet dieses, um E-Mail-Anhänge vom Exchange-Server herunterzuladen. Die einzige Berechtigung, die die Verwendung dieser Funktion zulässt, ist `ReadWriteMailbox`. Weitere Informationen finden Sie unter [Datenschutz, Berechtigungen und Sicherheit für Outlook-Add](https://docs.microsoft.com/en-us/office/dev/add-ins/outlook/privacy-and-security) in der Dokumentation zu Microsoft.

Das [!DNL Workfront for Outlook]-Add-in erfordert außerdem `ReadWriteItem` Berechtigung (in `ReadWriteMailbox` enthalten), mit der der E-Mail-Textkörper gelesen und E-Mail-Metadaten gelesen/aktualisiert werden können:

* E-Mail-Text lesen:

  [!DNL Workfront for Outlook] liest den E-Mail-Textkörper, wenn ein Benutzer die Anfrage sendet, oder sendet den E-Mail-Textkörper als Aktualisierung an [!DNL Adobe Workfront] Objekt.
* E-Mail-Metadaten lesen/aktualisieren:

  [!DNL Workfront for Outlook] aktualisiert E-Mail-Kopfzeilen, wenn ein Benutzer eine Anfrage über eine E-Mail sendet. Dies dient dazu, Informationen über das gesendete [!DNL Adobe Workfront] zu speichern. Wenn der Benutzer also das Add-In für dieselbe E-Mail das nächste Mal öffnet, werden die Informationen zu vorherigen Aktionen mit dieser E-Mail angezeigt.

[!DNL Workfront for Outlook] greift nur dann auf das Postfach eines Benutzers zu, wenn der Benutzer eine Aktion im Add-on ausführt. Es hat keine Hintergrundfunktion. Workfront für Outlook greift nur in folgendem Szenario auf das Postfach des Benutzers zu:

* Der/die Benutzende versucht, eine Anfrage zu senden, eine Aufgabe zu erstellen oder eine E-Mail als Aktualisierung über [!DNL Workfront for Outlook] zu senden (Öffnen des Add-Ins und Auswahl einer Aktion)
   * [!DNL Workfront for Outlook] liest den E-Mail-Textkörper, der im Formular innerhalb des Add-Ins ausgefüllt werden soll.
   * [!DNL Workfront for Outlook] liest E-Mail-Metadaten, um Informationen über das Add-In und die vorherigen Aktionen anzuzeigen, die im Add-In mit derselben E-Mail durchgeführt wurden.
* Wenn ein(e) Benutzende(r) eine Anfrage sendet, eine Aufgabe erstellt oder eine E-Mail als Aktualisierung von [!DNL Workfront for Outlook] sendet (klicken Sie im Add-In auf [!UICONTROL Senden]-Schaltfläche):
   * [!DNL Workfront for Outlook] liest den Textkörper der E-Mail, um ihn als Anfragebeschreibung oder Kommentar an Workfront zu senden.
   * [!DNL Workfront for Outlook] aktualisiert die E-Mail-Metadaten, um Informationen über die gesendeten Anfragen oder das aktualisierte Objekt zu speichern.
   * [!DNL Workfront for Outlook] lädt E-Mail-Anhänge vom Exchange-Server herunter, um sie in gesendete Anfragen, erstellte Aufgaben oder aktualisierte Objekte hochzuladen.
