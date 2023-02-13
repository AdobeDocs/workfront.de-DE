---
content-type: tips-tricks-troubleshooting
product-previous: workfront;workfront-proof
product-area: user-management
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: Fehlerbehebung bei Berechtigungen für Workfront Proof Manager
description: Im Folgenden finden Sie die Berechtigungsprofile, die in [!DNL Adobe] Workfront für Testbenutzer - BEARBEITEN SIE MICH.
feature: Get Started with Workfront
exl-id: 913241d0-f5b0-4674-b078-9a1ad3682aff
source-git-commit: ecb6928c946203b03a93cf5687fd53abf8e6a8f3
workflow-type: tm+mt
source-wordcount: '255'
ht-degree: 1%

---

# [!UICONTROL [!DNL Workfront] Proof Manager] Fehlerbehebung bei Berechtigungen

Im Folgenden finden Sie die Berechtigungsprofile, die in [!DNL Adobe Workfront] für Benutzer von Testsendungen:

* [!UICONTROL Administrator]
* [!UICONTROL Supervisor]
* [!UICONTROL Manager]

<!--For detailed information about these options and how to configure them, see .-->

Beim Zuweisen eines Benutzers [!UICONTROL Manager] -Berechtigungen, sind die folgenden Informationen zur Fehlerbehebung verfügbar:

* **PROBLEM:** Benutzer mit [!UICONTROL Manager] -Berechtigungen können keine von anderen Benutzern erstellten Testsendungen anzeigen. Stattdessen sehen sie die [!UICONTROL Zugriff verweigert] angezeigt.

   ![](assets/access-denied-350x161.png)

   **LÖSUNG:** Benutzer mit [!UICONTROL Manager] -Berechtigungen müssen explizit zu den Testsendungen hinzugefügt werden. Testsendungen sollten immer über die [!UICONTROL Erweiterte Testoptionen] -Fenster und -Benutzer sollten immer über diese Option hinzugefügt werden.

* **PROBLEM:** Benutzer mit [!UICONTROL Manager] -Berechtigungen können Testversandversionen nicht zu Testsendungen hinzufügen, die von anderen Benutzern erstellt wurden (sie können möglicherweise einen Testversand im Dokumentsatz durchführen, aber die Versionen wären NICHT mit dem von einem anderen Benutzer erstellten Originalsatz verbunden).\
   **LÖSUNG:** Benutzer mit [!UICONTROL Manager] -Berechtigungen können die Versionen nur dann an den Testversand eines anderen Benutzers senden, wenn der Benutzer mit [!UICONTROL Manager] -Berechtigungen, wenn beide der folgenden Bedingungen erfüllt sind:

   * Explizit zu Testsendungen hinzugefügt
   * Legen Sie als [!UICONTROL Autoren] (Testversandrolle) auf den Testsendungen

* **PROBLEM:** Benutzer mit [!UICONTROL Manager] -Berechtigungen können keine Kommentare anderer Benutzer zu einem Testversand bearbeiten, dessen Inhaber sie nicht sind oder die sie nicht erstellt haben.\
   **LÖSUNG:** Wenn Benutzer mit [!UICONTROL Manager] Berechtigungen besitzen nicht die Testsendungen, sollten jedoch Kommentare bearbeiten und sie wie folgt hinzufügen können: [!UICONTROL Autoren] (oder [!UICONTROL Moderatoren]).\
   Diese drei Arten von Berechtigungen sind in verfügbar. [!DNL Workfront] für [!UICONTROL Planen], [!UICONTROL Worker], [!UICONTROL Antragsteller], [!UICONTROL Überprüfer] Typlizenzen. Systemadministrator oder Benutzeradministrator in [!DNL Workfront] Sie können Benutzerprofile bearbeiten und [!DNL Workfront Proof] Berechtigungen von dort aus.
