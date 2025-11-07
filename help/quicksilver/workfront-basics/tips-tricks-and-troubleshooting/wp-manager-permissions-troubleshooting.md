---
content-type: tips-tricks-troubleshooting
product-previous: workfront;workfront-proof
product-area: user-management
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: Fehlerbehebung bei Workfront Proof Manager-Berechtigungen
description: Die in  [!DNL Adobe] Workfront für Proofing-Benutzer verfügbaren Berechtigungsprofile sind „Administrator“, „Supervisor“ und „Manager“.
feature: Get Started with Workfront
auhor: Courtney
exl-id: 913241d0-f5b0-4674-b078-9a1ad3682aff
source-git-commit: 883ec4eaa2258de2e464acf14b6b4083db05b99a
workflow-type: tm+mt
source-wordcount: '256'
ht-degree: 0%

---

# [!UICONTROL [!DNL Workfront]-Korrekturabzug-Manager] Fehlerbehebung bei Berechtigungen

Im Folgenden finden Sie die in [!DNL Adobe Workfront] für Proofing-Benutzer verfügbaren Berechtigungsprofile:

* [!UICONTROL Administrator]
* [!UICONTROL Verantwortlicher]
* [!UICONTROL Manager]

<!--For detailed information about these options and how to configure them, see .-->

Wenn Sie einem Benutzer [!UICONTROL Manager] Berechtigungen erteilen, sind die folgenden Informationen zur Fehlerbehebung verfügbar:

* **PROBLEM:** Benutzende mit [!UICONTROL Manager]-Berechtigungen können von anderen Benutzenden erstellte Korrekturabzüge nicht anzeigen. Stattdessen wird der Bildschirm [!UICONTROL Zugriff verweigert] angezeigt.

  ![](assets/access-denied-350x161.png)

  **LÖSUNG:** Benutzer mit [!UICONTROL Manager]-Berechtigungen müssen den Korrekturabzügen explizit hinzugefügt werden. Korrekturabzüge sollten immer über das Fenster [!UICONTROL Erweiterte Korrekturabzugsoptionen] erstellt werden und Benutzer sollten immer über diese Option hinzugefügt werden.

* **PROBLEM:** Benutzende mit [!UICONTROL Manager]-Berechtigungen können keine Korrekturabzugsversionen zu den von anderen Benutzenden erstellten Korrekturabzügen hinzufügen (sie können möglicherweise einen Korrekturabzug im Dokumentensatz senden, die Versionen werden jedoch NICHT mit dem ursprünglichen Satz verbunden, der von einem anderen Benutzenden erstellt wurde).\
   **LÖSUNG:** Benutzer mit [!UICONTROL Manager]-Berechtigungen können die Versionen nur dann an den Korrekturabzug eines anderen Benutzers senden, wenn der Benutzer über [!UICONTROL Manager]-Berechtigungen verfügt und die beiden folgenden Bedingungen erfüllt sind:

   * Explizit zu den Testsendungen hinzugefügt
   * Als [!UICONTROL Autoren] (Korrekturabzugsrolle) für die Korrekturabzüge festlegen

* **PROBLEM:** Benutzende mit [!UICONTROL Manager]-Berechtigungen können keine Kommentare anderer Benutzender zu einem Korrekturabzug bearbeiten, dessen Inhaber sie nicht sind oder den sie nicht erstellt haben.\
   **LÖSUNG:** Wenn Benutzende mit [!UICONTROL Manager]-Berechtigungen nicht Eigentümer der Korrekturabzüge sind, sie jedoch Kommentare bearbeiten können, fügen Sie sie als [!UICONTROL Autoren] (oder [!UICONTROL Moderatoren]) hinzu.\
   Diese drei Arten von Berechtigungen sind in [!DNL Workfront] für [!UICONTROL Planer], [!UICONTROL Arbeiter], [!UICONTROL Anforderer], [!UICONTROL Reviewer] verfügbar. Systemadministrator oder Benutzeradministrator in [!DNL Workfront] kann die Profile von Benutzern bearbeiten und [!DNL Workfront Proof] Berechtigungen von dort aus anpassen.
