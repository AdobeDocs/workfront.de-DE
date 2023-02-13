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
source-git-commit: 80ad604330e8b55037f1607b754cc8bb34f6a3ec
workflow-type: tm+mt
source-wordcount: '502'
ht-degree: 0%

---

# Konfigurieren [!UICONTROL Ressourcenverwaltung] Voreinstellungen

<!--Linked to lots of articles for resource planning and LINKED TO CONTEXT SENSITIVE HELP - DO NOT CHANGE OR REMOVE!</p>
Edit the first part, once they add more settings in the Res Management Preferences - right now, only the FTE calculation is the
-->

<!--drafted for Work time field: <span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment.</span> -->

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

<!--drafted for Work time field: 

## Information taken into account when calculating user's capacity

When calculating a user's capacity, Workfront takes into account the following information:

* The number of scheduled hours, as defined in either the Schedule of the user or the Workfront system's [!UICONTROL Default Schedule]
* [!UICONTROL Schedule] [!UICONTROL Exceptions] (depending on which [!UICONTROL Schedule] is used, it can be the exceptions of the user's schedule, or those associated with the [!DNL Workfront] [!UICONTROL Default Schedule])
* User's time off
* The value of the Full Time Equivalent ([!UICONTROL FTE]) of the user or that of the [!DNL Workfront] system. The [!UICONTROL FTE] equals 1 when the user works full time, as defined in the schedule. 

<!-drafted for Work Time field  

* <span class="preview">The value of [!UICONTROL Work Time] for the user which refers to time that the user spends on project-related work. This does not include overhead time, like meetings and training. The [!UICONTROL Work Time] equals 1 when the user is available for work the entire time as indicated by the [!UICONTROL FTE] or the schedule, which means they don't spend any time in non-project-related work like meetings or trainings.</span>

-->

Informationen zur Planung und Planung von Ressourcen finden Sie unter [!DNL Workfront], siehe [Erste Schritte mit der Ressourcenverwaltung](../../../resource-mgmt/resource-mgmt-overview/get-started-resource-management.md).

—>

## Konfigurieren [!UICONTROL Ressourcenverwaltung] Voreinstellungen

>[!NOTE]
>
>Da es sich um eine globale Einstellung handelt, wirkt sich diese Auswahl auf alle Berechnungen für das gesamte System, für alle Benutzer, für alle Ressourcen-Management-Tools und für alle Ressourcen-Pools aus.

1. Klicken Sie auf **[!UICONTROL Hauptmenü]** icon ![](assets/main-menu-icon.png) in der oberen rechten Ecke von [!DNL Workfront]Klicken Sie auf **[!UICONTROL Einrichtung]** ![](assets/gear-icon-settings.png).
1. Klicken **[!UICONTROL Ressourcenverwaltung]**.
1. Wählen Sie eine der folgenden Methoden, um die Verfügbarkeit der Benutzer in [!DNL Workfront]:

   * **Standardzeitplan**: [!DNL Workfront] verwendet den Standardzeitplan des Systems und die individuelle FTE des Benutzers, um die Verfügbaren Stunden des Benutzers in den Tools zur Ressourcenverwaltung zu berechnen.

      Weitere Informationen zu Zeitplänen finden Sie unter [Zeitplan erstellen](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

      Weitere Informationen zum Wert des Benutzers [!UICONTROL FTE], siehe  [Benutzerprofil bearbeiten](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

      Workfront berechnet die Verfügbaren Stunden eines Benutzers anhand der folgenden Formel, wenn der Workfront-Administrator die Option [!UICONTROL Standardzeitplan]:

      <!--drafted for Work Time field:
      In the Production environment: 
      -->

      ```
      User Available Hours = ([!UICONTROL Default Schedule] Hours - Exceptions) * FTE - Time off hours
      ```

      >[!INFO]
      >
      > Wenn beispielsweise die Variable [!UICONTROL Standardzeitplan] ist 40 Stunden pro Woche und die Variable [!UICONTROL FTE] im Benutzerprofil 0.5 ist der Benutzer 20 Stunden pro Woche für die Arbeit verfügbar.
      >Wenn der Benutzer eine Stunde Zeit pro Tag hat, werden seine Verfügbaren Stunden wie folgt berechnet:
      >
      >
      ```
      >User Available Hours = [(40 - 0) * 0.5)] - 1 = 19 hours
      >```
   <!--drafted for Work Time field

      <div class="preview">
      
      In the Preview environment: 

      ```
      User Available Hours = [([!UICONTROL Default Schedule] Hours - [!UICONTROL Exceptions]) * [!UICONTROL FTE] - Time off hours] * Work Time
      ```

      >[!INFO]
      >
      >For example, if the Default Schedule is 40 hours a week,  the FTE in the profile of the user is 0.5, the user has 1 hour of Time off one day, and the [!UICONTROL Work Time] in the profile of the user is 0.5, the user is available for actual project work for 9.5 hours a week.
      >
      >If the user has 1 hour of Time off one day, their Available Hours will be calculated as follows:
      >
      >```
      >User Available Hours = [(40 - 0) * 0.5) - 1] * 0.5 = 9.5 hours
      >```

      </div>

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
      >Wenn der Benutzer keinem Zeitplan zugeordnet ist, werden die für den Benutzer verfügbaren Stunden anhand der Variablen [!UICONTROL Standardzeitplan].

      <!--drafted for Work Time field:
      In the Production environment: 
      -->

      Die verfügbaren [!UICONTROL FTE] für den Benutzer anhand der folgenden Formel berechnet:

      ```
      User Available [!UICONTROL FTE] = (Hours from the [!UICONTROL Schedule] of the User - Time off hours) / [!UICONTROL Default Schedule] hours
      ```

      >[!INFO]
      >
      >Wenn beispielsweise die Variable [!UICONTROL Standardzeitplan] 40 Stunden pro Woche und der Zeitplan des Benutzers 30 Stunden pro Woche beträgt, wird die [!UICONTROL FTE] des Benutzers ist 0,70.
      >  
      >Wenn der Benutzer zwei Stunden Zeit pro Tag hat, ist seine wöchentliche Verfügbarkeit verfügbar [!UICONTROL FTE] wird wie folgt berechnet:
      > 
      >
      ```
      >User Weekly Available [!UICONTROL FTE] = (30-2) / 40 = 0.70
      >```

      <!--drafted for Work Time field:

      <div class="preview">

      In the Preview environment: 
      
      The Available hours for the user is calculated by the following formula:

      ```
      User Available Hours = (Hours from the [!UICONTROL Schedule] of the User - Time off hours) * [!UICONTROL Work Time]
      ```    

      The Available [!UICONTROL FTE] for the user is calculated by the following formula:

      ```
      User Available [!UICONTROL FTE] = [(Hours from the [!UICONTROL Schedule] of the User - Time off hours) * [!UICONTROL Work Time]] / [!UICONTROL Default Schedule] hours
      ```

      >[!INFO]
      >
      >For example, if the [!UICONTROL Default Schedule] is 40 hours a week, the schedule of the user is 30 hours a week, and the user's [!UICONTROL Work Time] is 0.5 the [!UICONTROL FTE] of the user is 0.35.
      >
      >If the user has 2 hours of Time off one day, their Weekly Available [!UICONTROL FTE] will be calculated as follows:
      >
      >```
      >User Weekly Available FTE = [(30-2) * 0.5] / 40 = 0.35
      >```
      (************ checking this second other with Dev/ Artur - not sure where Exceptions fit in **********)

      </div>
      -->
1. Klicken Sie auf **[!UICONTROL Speichern]**.
