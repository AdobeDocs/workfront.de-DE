---
product-area: workfront-integrations;agile-and-teams;user-management
navigation-topic: workfront-for-microsoft-teams
title: Zugriff auf [!DNL Adobe Workfront]  über [!DNL Microsoft] Teams
description: Sie können von  [!DNL Microsoft Teams] aus auf [!DNL Adobe Workfront] zugreifen und mehrere Aktionen in [!DNL Workfront] ausführen, indem Sie Befehle entweder in den Workfront-Bot-Kanal oder in einen anderen Teamkanal eingeben.
author: Becky
feature: Workfront Integrations and Apps
exl-id: a12277e8-2c2e-4b53-990f-6ee9a6541492
source-git-commit: 4572ea9bb0679c599a55d5a87c1397c7b819c963
workflow-type: tm+mt
source-wordcount: '466'
ht-degree: 1%

---

# Zugriff auf [!DNL Adobe Workfront] von [!DNL Microsoft Teams]

<!--Audited: 01/2024-->

>[!NOTE]
>
>Die Adobe Workfront für Microsoft Teams-Integration wird derzeit nur für das klassische Microsoft Teams-Erlebnis unterstützt.

Sie können über [!DNL Microsoft Teams] auf [!DNL Adobe Workfront] zugreifen und mehrere Aktionen in [!DNL Workfront] ausführen, indem Sie Befehle entweder in den Bot-Kanal [!DNL Workfront] oder in einen anderen Team-Kanal eingeben.

Sie können Folgendes in [!DNL Workfront] von [!DNL Microsoft Teams] ausführen:

* Suchen nach Projekten, Aufgaben oder Problemen
* Persönliche Aufgaben erstellen
* Auf Benachrichtigungen antworten
* Dokumentgenehmigungen verwalten

Die Befehle, die Sie über [!DNL Microsoft Teams] verwenden, um diese Aktionen durchzuführen, unterscheiden sich je nachdem, von welchem Kanal Sie auf [!DNL Workfront] zugreifen möchten.

>[!NOTE]
>
>[!DNL Microsoft Teams] unterstützt [!DNL Internet Explorer] nicht mehr. Um den [!DNL Adobe Workfront for Microsoft Teams integration] zu verwenden, müssen Sie einen anderen Webbrowser als [!DNL Internet Explorer] verwenden.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td> <p>Neu: [!UICONTROL Standard]</p>
   <p>Aktuell: [!UICONTROL Arbeit], [!UICONTROL Plan]</p> </td> 
  </tr> 
 </tbody> 
</table>

*Wenden Sie sich an Ihren [!DNL Workfront] -Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

*Weitere Informationen zu den Zugriffsanforderungen für Workfront finden Sie unter [Übersicht über die Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Voraussetzungen

Sie können persönliche Aufgaben in [!DNL Adobe Workfront] von [!DNL Microsoft Teams] erstellen, wenn die folgenden Bedingungen erfüllt sind:

* Ein Teaminhaber hat [!DNL Workfront for Microsoft Teams] für Ihr Team installiert und konfiguriert.
* Sie sind von [!DNL Microsoft Teams] bei [!DNL Workfront] angemeldet.

## Zugriff auf [!DNL Workfront] über den Bot-Chat-Kanal [!DNL Workfront]

Sie müssen bei Workfront angemeldet sein.

1. Öffnen Sie den Bot-Chat-Kanal **[!DNL Workfront]** .
1. Klicken Sie unter dem Textfeld auf das Symbol &quot;**[!DNL Workfront]**&quot;, um das Suchfeld anzuzeigen.

   ![teams_search_box_in_the_bot_channel.PNG](assets/teams-search-box-in-the-bot-channel-350x456.png)

1. Beginnen Sie mit der Eingabe des Namens eines Projekts, einer Aufgabe oder eines Problems.

   Informationen zum Suchen nach Elementen finden Sie im Abschnitt [Suchen nach und Freigeben [!DNL Adobe Workfront] von Elementen in [!DNL Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/search-for-and-share-wf-items-in-ms-teams.md) in the article [Search for and share [!DNL Adobe Workfront] Elementen in [!DNL Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/search-for-and-share-wf-items-in-ms-teams.md).

1. Klicken Sie auf das Feld **[!UICONTROL Geben Sie Ihre Fragen hier ein]** .

   ![ms_teams_type_your_questions_here_and_what_can_I_do_fields.png](assets/ms-teams-type-your-questions-here-and-what-can-i-do-fields-350x71.png)

1. Führen Sie einen der folgenden Schritte aus:

   * Klicken Sie auf **[!UICONTROL Was kann ich tun?]**, dann **[!UICONTROL Anmelden]** oder **[!UICONTROL Abmelden]** von [!DNL Workfront], erstellen Sie eine **[!UICONTROL neue Aufgabe]** (persönliche Aufgabe) in [!DNL Workfront] oder erhalten Sie **[!UICONTROL Hilfe]**, indem Sie die verfügbaren Befehle auflisten.

   * Greifen Sie direkt auf [!DNL Workfront] zu, indem Sie einen Befehl in das Feld **[!UICONTROL Geben Sie Ihre Fragen hier ein]** ein.

     Bei Befehlen wird nicht zwischen Groß- und Kleinschreibung unterschieden.

     Der Bot [!DNL Workfront] antwortet mit Ihrer Anfrage im Bot-Chat-Kanal [!DNL Workfront] .

## Zugriff auf [!DNL Workfront] über einen Teamkanal

Sie müssen bei Workfront angemeldet sein.

1. Öffnen Sie einen Teamkanal und geben Sie **@[!DNL Workfront]** ein, und wählen Sie dann **[!DNL Workfront].**.

1. Klicken Sie auf **[!UICONTROL Suchen]** , um nach einem Projekt, einer Aufgabe oder einem Problem zu suchen.

   Weitere Informationen zum Suchen nach Elementen finden Sie im Artikel [Suchen nach und Freigeben [!DNL Adobe Workfront] von Elementen in [!DNL Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/search-for-and-share-wf-items-in-ms-teams.md) section in the [Search for and share [!DNL Adobe Workfront] Elementen in [!DNL Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/search-for-and-share-wf-items-in-ms-teams.md).

1. Geben Sie einen der folgenden Befehle ein, um diese Aktionen in Workfront durchzuführen.\
   Bei Befehlen wird nicht zwischen Groß- und Kleinschreibung unterschieden:

   * **[!UICONTROL Anmelden]** , um sich bei [!DNL Workfront] anzumelden
   * **[!DNL Log out]** für die Abmeldung von Workfront
   * **[!DNL New task]** , um eine neue persönliche Aufgabe zu erstellen

     Informationen zum Erstellen von Aufgaben aus [!DNL Microsoft Teams] finden Sie unter [Erstellen [!DNL Adobe Workfront] von Aufgaben aus  [!DNL Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/create-workfront-tasks-from-ms-teams.md).

   * **[!UICONTROL Hilfe]** zum Anzeigen einer Liste aller verfügbaren Befehle.

     Der Bot [!DNL Workfront] antwortet mit Ihrer Anfrage im Bot-Chat-Kanal [!DNL Workfront] .

1. Wechseln Sie zum Bot-Chat-Kanal [!DNL Workfront] , um auf [!DNL Workfront] zuzugreifen und Ihre Anfrage abzuschließen.
