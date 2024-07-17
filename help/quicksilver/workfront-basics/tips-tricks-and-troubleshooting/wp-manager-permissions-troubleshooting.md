---
content-type: tips-tricks-troubleshooting
product-previous: workfront;workfront-proof
product-area: user-management
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: Fehlerbehebung bei Berechtigungen für Workfront Proof Manager
description: Die Berechtigungsprofile, die in [!DNL Adobe] Workfront für Testbenutzer verfügbar sind, sind "Administrator", "Supervisor"und "Manager".
feature: Get Started with Workfront
exl-id: 913241d0-f5b0-4674-b078-9a1ad3682aff
source-git-commit: 114d306d99ae9ba0a18abd63a6137ad0568ab202
workflow-type: tm+mt
source-wordcount: '256'
ht-degree: 0%

---

# [!UICONTROL [!DNL Workfront] Fehlerbehebung bei Zugriffsberechtigungen für den Proof Manager]

Im Folgenden finden Sie die Berechtigungsprofile, die in [!DNL Adobe Workfront] für Testversand-Benutzer verfügbar sind:

* [!UICONTROL Administrator]
* [!UICONTROL Supervisor]
* [!UICONTROL Manager]

<!--For detailed information about these options and how to configure them, see .-->

Wenn Sie einem Benutzer [!UICONTROL Manager] -Berechtigungen erteilen, sind die folgenden Informationen zur Fehlerbehebung verfügbar:

* **PROBLEM:** Benutzer mit [!UICONTROL Manager] -Berechtigungen können keine von anderen Benutzern erstellten Testsendungen anzeigen. Stattdessen wird der Bildschirm [!UICONTROL Zugriff verweigert] angezeigt.

  ![](assets/access-denied-350x161.png)

  **LÖSUNG:** Benutzer mit [!UICONTROL Manager] -Berechtigungen müssen explizit zu den Testsendungen hinzugefügt werden. Testsendungen sollten immer über das Fenster [!UICONTROL Erweiterte Testoptionen] erstellt werden und Benutzer sollten immer über diese Option hinzugefügt werden.

* **PROBLEM:** Benutzer mit [!UICONTROL Manager] -Berechtigungen können den von anderen Benutzern erstellten Testsendungen keine Testversionen hinzufügen. (Sie können möglicherweise einen Testversand im Dokumentsatz durchführen, aber die Versionen sind NICHT mit dem von einem anderen Benutzer erstellten Originalsatz verbunden.)\
   **LÖSUNG:** Benutzer mit [!UICONTROL Manager] -Berechtigungen können die Versionen nur dann an den Testversand eines anderen Benutzers senden, wenn der Benutzer über [!UICONTROL Manager] -Berechtigungen verfügt, wenn beide der folgenden Bedingungen erfüllt sind:

   * Explizit zu Testsendungen hinzugefügt
   * Wird auf den Testsendungen als [!UICONTROL Autoren] (Testversandrolle) eingestellt

* **PROBLEM:** Benutzer mit [!UICONTROL Manager] -Berechtigungen können Kommentare anderer Benutzer nicht für einen Testversand bearbeiten, dessen Inhaber sie nicht sind oder den sie nicht erstellt haben.\
   **LÖSUNG:** Wenn Benutzer mit [!UICONTROL Manager] -Berechtigungen nicht Inhaber der Testsendungen sind, aber Kommentare bearbeiten können sollen, fügen Sie sie als [!UICONTROL Autoren] (oder [!UICONTROL Moderatoren]) hinzu.\
   Diese drei Berechtigungstypen sind in [!DNL Workfront] für Lizenzen vom Typ [!UICONTROL Planer], [!UICONTROL Worker], [!UICONTROL Anforderer], [!UICONTROL Überprüfer] verfügbar. Systemadministrator oder Benutzeradministrator in [!DNL Workfront] können die Profile der Benutzer bearbeiten und die [!DNL Workfront Proof] -Berechtigungen von dort aus anpassen.
