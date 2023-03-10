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
source-git-commit: 921749caf6a61fa4f0efae9357c6e05c581421c5
workflow-type: tm+mt
source-wordcount: '700'
ht-degree: 0%

---

# Konfigurieren [!UICONTROL Ressourcenverwaltung] Voreinstellungen

<!--Linked to lots of articles for resource planning and LINKED TO CONTEXT SENSITIVE HELP - DO NOT CHANGE OR REMOVE!</p>
Edit the first part, once they add more settings in the Res Management Preferences - right now, only the FTE calculation is the
-->

Als [!DNL Adobe Workfront] Administrator können Sie die [!UICONTROL Ressourcenverwaltung] Voreinstellungen für Ihr System. Diese Voreinstellungen bestimmen, wie die Benutzerstunde oder die FTE-Verfügbarkeit oder -Kapazität für die [!DNL Workfront] Tools zur Ressourcenplanung und -planung.

## Zugriffsanforderungen

<!--drafted for P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td>Any</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] license</td> 
   <td>
   <p>Current license: [!UICONTROL Standard]</p>
   
   Or
   
   <p>Legacy license: [!UICONTROL Plan]</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>System Administrator access level</p> <p>For more information, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p> <p><b>NOTE</b>: 
   
   If you still don't have access, ask your [!DNL Workfront] administrator if they set additional restrictions in your access level. For information on how a [!DNL Workfront] administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

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
   <td> <p>Zugriffsstufe für Systemadministrator</p> <p>Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Gewähren eines vollen Administratorzugriffs</a>.</p> <p><b>NOTIZ</b>:

Wenn Sie noch keinen Zugriff haben, fragen Sie Ihren [!DNL Workfront] Administrator , wenn sie zusätzliche Einschränkungen für Ihre Zugriffsebene festlegen. Für Informationen zur [!DNL Workfront] Administrator kann Ihre Zugriffsebene ändern, siehe <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td>
</tr> 
 </tbody> 
</table>

## Bei der Berechnung der Kapazität eines Benutzers berücksichtigte Informationen

Bei der Berechnung der Nutzerkapazität berücksichtigt Workfront die folgenden Informationen:

* Die Anzahl der geplanten Stunden, wie im Benutzerplan oder im Workfront-System [!UICONTROL Standardzeitplan]
* [!UICONTROL Zeitplan] [!UICONTROL Ausnahmen] (abhängig von [!UICONTROL Zeitplan] verwendet wird, kann es sich um die Ausnahmen des Benutzerzeitplans oder um die mit dem [!DNL Workfront] [!UICONTROL Standardzeitplan])
* Zeitlimit des Benutzers
* Der Wert des Vollzeitäquivalents ([!UICONTROL FTE]) des Benutzers oder des [!DNL Workfront] System. Die [!UICONTROL FTE] entspricht 1, wenn der Benutzer Vollzeit arbeitet, wie im Zeitplan definiert.
* Der Wert von [!UICONTROL Arbeitszeit] für den Benutzer, der sich auf die Zeit bezieht, die der Benutzer für projektbezogene Arbeit verbringt. Dies umfasst keine Zeit mit Mehraufwand, wie z. B. Sitzungen und Schulungen. Die [!UICONTROL Arbeitszeit] gleich 1, wenn der Benutzer für die gesamte Arbeitszeit verfügbar ist, wie durch die [!UICONTROL FTE] oder dem Zeitplan, was bedeutet, dass sie keine Zeit für nicht projektbezogene Arbeiten wie Meetings oder Trainings verbringen.


Informationen zur Planung und Planung von Ressourcen finden Sie unter [!DNL Workfront], siehe [Erste Schritte mit der Ressourcenverwaltung](../../../resource-mgmt/resource-mgmt-overview/get-started-resource-management.md).


## Konfigurieren [!UICONTROL Ressourcenverwaltung] Voreinstellungen

>[!NOTE]
>
>Da es sich um eine globale Einstellung handelt, wirkt sich diese Auswahl auf alle Berechnungen für das gesamte System aus, für alle Benutzer, in allen Tools zur Ressourcenverwaltung.

1. Klicken Sie auf **[!UICONTROL Hauptmenü]** icon ![](assets/main-menu-icon.png) in der oberen rechten Ecke von [!DNL Workfront]Klicken Sie auf **[!UICONTROL Einrichtung]** ![](assets/gear-icon-settings.png).
1. Klicken **[!UICONTROL Ressourcenverwaltung]**.
1. Wählen Sie eine der folgenden Methoden, um die Verfügbarkeit der Benutzer in [!DNL Workfront]:

   * **Standardzeitplan**: [!DNL Workfront] verwendet den Standardzeitplan des Systems und die individuelle FTE des Benutzers, um die Verfügbaren Stunden des Benutzers in den Tools zur Ressourcenverwaltung zu berechnen.

      Weitere Informationen zu Zeitplänen finden Sie unter [Zeitplan erstellen](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

      Weitere Informationen zum Auffinden des Werts des [!UICONTROL FTE], siehe  [Benutzerprofil bearbeiten](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

      Workfront berechnet die Verfügbaren Stunden eines Benutzers anhand der folgenden Formel, wenn der Workfront-Administrator die Option [!UICONTROL Standardzeitplan]:


      `User Available Hours = [([!UICONTROL Default Schedule] Hours - [!UICONTROL Exceptions]) * [!UICONTROL FTE] - Time off hours] * [!UICONTROL Work Time]`


      >[!INFO]
      >
      >Wenn der Standardzeitplan beispielsweise 40 Stunden pro Woche beträgt, beträgt die VZÄ im Benutzerprofil 0,5, der Benutzer hat eine Stunde Freizeit von einem Tag und die [!UICONTROL Arbeitszeit] im Benutzerprofil 0,5 ist der Benutzer für die tatsächliche Projektarbeit 9,5 Stunden pro Woche verfügbar.
      >
      >Wenn der Benutzer eine Stunde Zeit pro Tag hat, werden seine Verfügbaren Stunden wie folgt berechnet:
      >
      >
      >`User Available Hours = [((40 - 0) * 0.5) - 1] * 0.5 = 9.5 hours`

      <!--This used to be the calculation before we implemented the Work Time field: 
    
      ```
      User Available Hours = ([!UICONTROL Default Schedule] Hours - Exceptions) * FTE - Time off hours
      ```

      >[!INFO]
      >
      > For example, if the [!UICONTROL Default Schedule] is 40 hours a week and the [!UICONTROL FTE] in the profile of the user is 0.5, the user is available to work for 20 hours a week.
      >If the user has 1 hour of Time off one day, their Available Hours will be calculated as follows:
      >
      >```
      >User Available Hours = [(40 - 0) * 0.5)] - 1 = 19 hours
      >```
      -->



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

   * **Zeitplan des Benutzers**: [!DNL Workfront] verwendet den Zeitplan des Benutzers sowie die [!UICONTROL Standardzeitplan] des Systems zur Berechnung der verfügbaren [!UICONTROL FTE] Wert des Benutzers in den Tools zur Ressourcenverwaltung. Die verfügbaren Stunden werden nur nach dem Zeitplan des Benutzers berechnet. Der Wert der [!UICONTROL FTE] des Benutzers ignoriert wird. Dies ist die Standardeinstellung.

      Weitere Informationen zu Zeitplänen finden Sie unter [Zeitplan erstellen](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

      Weitere Informationen zu den [!UICONTROL Zeitplan], siehe  [Benutzerprofil bearbeiten](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

      >[!NOTE]
      >
      >Wenn der Benutzer keinem Zeitplan zugeordnet ist, werden die verfügbaren Stunden für den Benutzer nur anhand der Variablen [!UICONTROL Standardzeitplan].

      Die verfügbaren Stunden für den Benutzer werden anhand der folgenden Formel berechnet:


      `User Available Hours = (Hours from the [!UICONTROL Schedule] of the User - Schedule Exceptions - Time off hours) * [!UICONTROL Work Time]`


      Die verfügbaren [!UICONTROL FTE] für den Benutzer anhand der folgenden Formel berechnet:


      `User Available [!UICONTROL FTE] = [(Hours from the [!UICONTROL Schedule] of the User - Schedule Exceptions - Time off hours) * [!UICONTROL Work Time]] / [!UICONTROL Default Schedule] hours`


      >[!INFO]
      >
      >Wenn beispielsweise die Variable [!UICONTROL Standardzeitplan] ist 40 Stunden pro Woche, der Zeitplan des Benutzers 30 Stunden pro Woche und der des Benutzers [!UICONTROL Arbeitszeit] ist 0,5. [!UICONTROL FTE] des Benutzers ist 0,35.
      >
      >Wenn der Benutzer zwei Stunden Zeit pro Tag hat, ist seine wöchentliche Verfügbarkeit verfügbar [!UICONTROL FTE] wird wie folgt berechnet:
      >
      >
      >`User Weekly Available [!UICONTROL FTE] = [(30-2) * 0.5] / 40 = 0.35`

      <!--This used to be the calculation before we implemented the Work Time field: 
      

      The Available hours for the user are calculated by the following formula:

      ```
      User Available Hours = Hours from the [!UICONTROL Schedule] of the User - [!UICONTROL Schedule Exceptions] - Time off hours
      ```  

      The Available [!UICONTROL FTE] for the user is calculated by the following formula:

      ```
      User Available [!UICONTROL FTE] = (Hours from the [!UICONTROL Schedule] of the User - [!UICONTROL Schedule Exceptions] - Time off hours) / [!UICONTROL Default Schedule] hours
      ```

      >[!INFO]
      >
      >For example, if the [!UICONTROL Default Schedule] is 40 hours a week and the schedule of the user is 30 hours a week, the [!UICONTROL FTE] of the user is 0.70.
      >  
      >If the user has 2 hours of Time off one day, their Weekly Available [!UICONTROL FTE] will be calculated as follows:
      > 
      >```
      >User Weekly Available [!UICONTROL FTE] = (30-2) / 40 = 0.70
      >```
      -->

1. Klicken Sie auf **[!UICONTROL Speichern]**.
