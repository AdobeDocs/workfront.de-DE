---
product-area: workfront-integrations;agile-and-teams;user-management
navigation-topic: workfront-for-microsoft-teams
title: Create [!DNL Adobe Workfront] tasks from [!DNL Microsoft] Teams
description: Sie können persönliche Aufgaben in Adobe [!DNL Workfront] von Microsoft Teams erstellen, wenn ein Teambesitzer Microsoft Teams für Ihr  [!DNL Workfront]  installiert und konfiguriert hat und Sie von Microsoft Teams aus bei Workfront angemeldet sind.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 31b86c8d-967a-446a-86f2-3d38e44c45e1
source-git-commit: 940cbfb34f12eacd5ba698f60fb7a3e67eb62b22
workflow-type: tm+mt
source-wordcount: '447'
ht-degree: 0%

---

# [!DNL Adobe Workfront] Aufgaben aus [!DNL Microsoft Teams] erstellen

>[!IMPORTANT]
>
>Da [Microsoft auf den neuen Teams-Client umstellt](https://learn.microsoft.com/en-us/microsoftteams/teams-classic-client-end-of-availability) ist der Classic Teams-Client nach dem 1. Juli 2025 nicht mehr verfügbar. Um Microsoft Teams und integrierte Apps wie Workfront weiterhin verwenden zu können, müssen Kunden vor diesem Datum zum neuen Teams-Client wechseln.
>
>Die aktualisierte Workfront-Integration ist jetzt verfügbar und vollständig mit der neuen Team-Erfahrung kompatibel. In den meisten Fällen wird Workfront automatisch angezeigt, sobald Benutzende den Wechsel vollzogen haben. Ist dies nicht der Fall, kann die Integration manuell über die Microsoft Teams App Store installiert werden. Informationen zum Installieren oder Überprüfen der Workfront-Integration im neuen Team-Client finden Sie unter [Installieren [!DNL Adobe Workfront]  für Microsoft Teams](/help/quicksilver/workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md).

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Plan*</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Lizenz*</td> 
   <td> <p>[!UICONTROL Arbeit], [!UICONTROL Plan]</p> </td> 
  </tr>
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren [!DNL Workfront], um herauszufinden, über welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie verfügen.

## Voraussetzungen

Sie können persönliche Aufgaben in [!DNL Adobe Workfront] aus [!DNL Microsoft Teams] erstellen, wenn die folgenden Bedingungen erfüllt sind:

* Ein Teambesitzer hat [!DNL Workfront for Microsoft Teams] für Ihr Team installiert und konfiguriert.
* Sie sind von [!DNL Microsoft Teams] aus bei [!DNL Workfront] angemeldet.

>[!NOTE]
>
>[!DNL Microsoft Teams] unterstützt [!DNL Internet Explorer] nicht mehr. Um die [!DNL Adobe Workfront for Microsoft Teams]-Integration zu verwenden, müssen Sie einen anderen Webbrowser als [!DNL Internet Explorer] verwenden.

Informationen zum Installieren von [!DNL Workfront for Microsoft Teams] und zum Anmelden bei [!UICONTROL Workfront] von [!DNL Microsoft Teams] finden Sie unter [Installieren [!DNL Adobe Workfront for Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md).

## Persönliche Aufgaben aus [!DNL Microsoft Teams] erstellen

1. Melden Sie sich von [!DNL Microsoft Teams] aus bei [!DNL Workfront] an.

   Informationen zur Anmeldung bei [!DNL Workfront] finden Sie unter [Installieren [!DNL Adobe Workfront for Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md).

1. So öffnen Sie eine **[!UICONTROL Neue Aufgabe]** Karte:

   * Wenn Sie sich im [!DNL Workfront] Bot-Chat-Kanal befinden, geben Sie **[!UICONTROL Neue Aufgabe]** in das Feld [!UICONTROL Konversation] ein, um eine neue Aufgabe zu erstellen.
   * Wenn Sie sich in einem anderen Chat-Kanal als dem [!DNL Workfront] Bot-Chat-Kanal befinden:

      * Beginnen Sie, **[!DNL @workfront]** in das Feld [!UICONTROL Konversation] einzugeben, und wählen Sie dann den gewünschten [!DNL Workfront] Bot-Kanal aus.
      * Fahren Sie mit der Eingabe **[!UICONTROL Neue Aufgabe]** in das Feld [!UICONTROL Konversation] fort, um eine neue Aufgabe zu erstellen.

        Die Karte [!UICONTROL Neue Aufgabe] wird im [!DNL Workfront] Bot-Kanal angezeigt.

        ![ms_teams_new_task_card.png](assets/ms-teams-new-task-card-350x181.png)

1. Geben Sie im Bot- Workfront die folgenden Informationen auf der Karte [!UICONTROL Neue Aufgabe] an:

   * Aufgabenname im Feld **[!UICONTROL Den Titel der Aufgabe]**.
   * Beschreibung der Aufgabe im Feld **[!UICONTROL Beschreibung der Aufgabe]**.
   * Das Datum, bis zu dem die Aufgabe abgeschlossen sein muss, im Feld **[!UICONTROL Fälligkeitsdatum]**.

1. Klicken Sie **[!UICONTROL Speichern].**

   Die neue persönliche Aufgabe wird in [!DNL Workfront] erstellt. Eine [!UICONTROL Referenznummer] wird ihm zugewiesen und auf der Karte [!UICONTROL Neue Aufgabe] angezeigt.

   Informationen zu Referenznummern finden Sie im Abschnitt [[!UICONTROL Referenznummern] von Objekten ](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#understanding-reference-numbers-of-objects) Abschnitt im Artikel [Grundlegendes zu Objekten in [!DNL Adobe Workfront]](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

1. (Optional) Klicken Sie auf **[!UICONTROL Bearbeiten]**, um die Aufgabeninformationen weiter zu bearbeiten.
1. (Optional) Klicken Sie auf **[!UICONTROL In[!DNL Workfront]]** anzeigen , um die Aufgabe in einer neuen Registerkarte in [!DNL Workfront] zu öffnen und die Aufgabe weiter zu bearbeiten, in ein Projekt zu verschieben oder sie einer anderen Person zuzuweisen.
