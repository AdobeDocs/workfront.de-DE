---
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-system-defaults
title: Voreinstellungen für die Ressourcenverwaltung konfigurieren
description: Als [!DNL Adobe Workfront] -Administrator können Sie die Voreinstellungen für die Ressourcenverwaltung für Ihr System konfigurieren. Diese Voreinstellungen für die Ressourcenverwaltung bestimmen, wie die Benutzerverfügbarkeit oder -kapazität und die FTE für die [!DNL Workfront] Tools zur Ressourcenplanung und -planung.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 7cde2238-cb34-4bee-baba-69d256a3912d
source-git-commit: 2fd772ffc667c4f32c6a7b0de9c87676ee6dd65b
workflow-type: tm+mt
source-wordcount: '482'
ht-degree: 1%

---

# Konfigurieren [!UICONTROL Ressourcenverwaltung] Voreinstellungen

<!--Linked to lots of articles for resource planning and LINKED TO CONTEXT SENSITIVE HELP - DO NOT CHANGE OR REMOVE!</p>
Edit the first part, once they add more settings in the Res Management Preferences - right now, only the FTE calculation is the
-->

Als [!DNL Adobe Workfront] Administrator können Sie die [!UICONTROL Ressourcenverwaltung] Voreinstellungen für Ihr System. Diese Voreinstellungen bestimmen, wie die Nutzerverfügbarkeit oder -kapazität berechnet wird, und die VZÄ für die [!DNL Workfront] Tools zur Ressourcenplanung und -planung.

Informationen zur Planung und Planung von Ressourcen finden Sie unter [!DNL Workfront], siehe [Erste Schritte mit der Ressourcenverwaltung](../../../resource-mgmt/resource-mgmt-overview/get-started-resource-management.md).

## Zugriffsanforderungen

Sie müssen über Folgendes verfügen, um die Schritte in diesem Artikel durchzuführen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Plan</td> 
   <td>Beliebig</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Lizenz</td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Zugriffsstufe für Systemadministrator</p> <p>Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Gewähren eines vollen Administratorzugriffs</a>.</p> <p><b>NOTE</b>: Wenn Sie noch keinen Zugriff haben, fragen Sie Ihren [!DNL Workfront] Administrator , wenn sie zusätzliche Einschränkungen für Ihre Zugriffsebene festlegen. Für Informationen zur [!DNL Workfront] Administrator kann Ihre Zugriffsebene ändern, siehe <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Konfigurieren [!UICONTROL Ressourcenverwaltung] Voreinstellungen

>[!NOTE]
>
>Da es sich um eine globale Einstellung handelt, wirkt sich diese Auswahl auf alle Berechnungen für das gesamte System, für alle Benutzer, für alle Ressourcen-Management-Tools und für alle Ressourcen-Pools aus.

1. Klicken Sie auf **[!UICONTROL Hauptmenü]** icon ![](assets/main-menu-icon.png) in der oberen rechten Ecke von [!DNL Workfront]Klicken Sie auf **[!UICONTROL Einrichtung]** ![](assets/gear-icon-settings.png).
1. Klicken **[!UICONTROL Ressourcenverwaltung]**.
1. Wählen Sie eine der folgenden Methoden, um die Verfügbarkeit der Benutzer in [!DNL Workfront]:

   * **Standardzeitplan**: [!DNL Workfront] verwendet den Standardzeitplan des Systems und die individuelle FTE des Benutzers, um die Verfügbaren Stunden des Benutzers in Tools zur Ressourcenverwaltung zu berechnen.\

      Weitere Informationen zu Zeitplänen finden Sie unter [Zeitplan erstellen](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

      Weitere Informationen über den Wert der FTE des Nutzers finden Sie unter  [Benutzerprofil bearbeiten](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

      Workfront berechnet die Verfügbaren Stunden eines Benutzers anhand der folgenden Formel, wenn der Workfront-Administrator den Standardzeitplan auswählt:

      ```
      User Available Hours = (Default Schedule Hours - Exceptions) * FTE - Time off hours
      ```

      **Beispiel:**\
      Wenn der Standardzeitplan beispielsweise 40 Stunden pro Woche beträgt und die FTE im Benutzerprofil 0,5 beträgt, kann der Benutzer 20 Stunden pro Woche arbeiten.

      Wenn der Benutzer eine Stunde Zeit pro Tag hat, werden seine Verfügbaren Stunden wie folgt berechnet:

      ```
      User Available Hours = (40 * 0.5) - 1 = 19 hours
      ```

      <!--      
        <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><p>In the Production environment: (NOTE: this is the old way it was working, before the 22.2 release)</p><p><code>User Available Hours = (Default Schedule Hours - (Schedule Exceptions + Time off hours)) * User FTE value</code></p>      
        <div class="example" data-mc-autonum="<b>Example: </b>">      
        <span class="autonumber"><span><b>Example: </b></span></span>      
        <div>      
        <p>For example, if the Default Schedule is 40 hours a week and the FTE in the profile of the user is 0.5, the user is available to work for 20 hours a week.</p>      
        <p>If the user has 1 hour of Time off one day, their Available Hours will be calculated as follows:</p>      
        <p><code>User Daily Available Hours = (40 - 1)* 0.5 = 19.5 hours</code></p>      
        </div>      
        </div></li>      
        -->

   * **Zeitplan des Benutzers**: [!DNL Workfront] verwendet den Benutzerplan sowie den Standardplan des Systems, um den verfügbaren FTE-Wert des Benutzers in Tools zur Ressourcenverwaltung zu berechnen. Die verfügbaren Stunden werden nur nach dem Zeitplan des Benutzers berechnet. Der Wert der FTE des Benutzers wird ignoriert. Dies ist die Standardeinstellung.

      >[!NOTE]
      >
      >Wenn der Benutzer keinem Zeitplan zugeordnet ist, werden die für den Benutzer verfügbaren Stunden anhand des Standardzeitplans berechnet.

      Die für den Benutzer verfügbare FTE wird nach folgender Formel berechnet:

      ```
      User Available FTE = (Hours from the Schedule of the User - Time off hours) / Default Schedule Hours
      ```

      **Beispiel:** Wenn der Standardzeitplan beispielsweise 40 Stunden pro Woche beträgt und der Benutzerzeitplan 30 Stunden pro Woche beträgt, beträgt die FTE des Benutzers 0,75.

      Wenn der Benutzer zwei Stunden Zeit pro Tag hat, wird seine wöchentlich verfügbare FTE wie folgt berechnet:

      ```
      User Weekly Available FTE = (30-2) / 40 = 0.70
      ```

1. Klicken Sie auf **[!UICONTROL Speichern]**.
