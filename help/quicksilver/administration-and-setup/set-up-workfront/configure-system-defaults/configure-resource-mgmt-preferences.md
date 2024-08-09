---
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-system-defaults
title: Voreinstellungen für die Ressourcenverwaltung konfigurieren
description: Als [!DNL Adobe Workfront] Administrator können Sie die Voreinstellungen für die Ressourcenverwaltung für Ihr System konfigurieren. Diese Voreinstellungen für die Ressourcenverwaltung bestimmen, wie die Benutzerverfügbarkeit oder -kapazität und die FTE für die [!DNL Workfront] Tools zur Ressourcenplanung und -planung berechnet werden.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 7cde2238-cb34-4bee-baba-69d256a3912d
source-git-commit: f036fbfc203f942fa5a22070860c3a20035a183b
workflow-type: tm+mt
source-wordcount: '711'
ht-degree: 0%

---

# Voreinstellungen für die [!UICONTROL Ressourcenverwaltung] konfigurieren

<!--Linked to lots of articles for resource planning and LINKED TO CONTEXT SENSITIVE HELP - DO NOT CHANGE OR REMOVE!</p>
Edit the first part, once they add more settings in the Res Management Preferences - right now, only the FTE calculation is the
-->

Als [!DNL Adobe Workfront] -Administrator können Sie die Voreinstellungen für die [!UICONTROL Ressourcenverwaltung] für Ihr System konfigurieren. Diese Voreinstellungen bestimmen, wie die Benutzerstundenverfügbarkeit oder -kapazität für die [!DNL Workfront] Ressourcen-Planungs- und -Planungstools berechnet wird.

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

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

Sie müssen über Folgendes verfügen, um die Schritte in diesem Artikel durchzuführen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Plan</td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Lizenz</td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Zugriffsstufe für Systemadministrator</p> <p>Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Gewähren des vollen Administratorzugriffs für einen Benutzer</a>.</p> <p><b>NOTE</b>:

Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren [!DNL Workfront] -Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein [!DNL Workfront] -Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td>
</tr> 
 </tbody> 
</table>

+++

## Bei der Berechnung der Kapazität eines Benutzers berücksichtigte Informationen

Bei der Berechnung der Nutzerkapazität berücksichtigt Workfront die folgenden Informationen:

* Die Anzahl der geplanten Stunden, wie im Benutzerzeitplan oder im [!UICONTROL Standardzeitplan] des Workfront-Systems definiert
* [!UICONTROL Zeitplan] [!UICONTROL Ausnahmen] (je nachdem, welcher [!UICONTROL Zeitplan] verwendet wird, kann es sich um die Ausnahmen des Benutzerzeitplans oder die mit dem [!DNL Workfront] [!UICONTROL Standardzeitplan] verbundenen Ausnahmen handeln)
* Zeitlimit des Benutzers
* Der Wert des Vollzeitäquivalents ([!UICONTROL FTE]) des Benutzers oder des [!DNL Workfront]-Systems. Die [!UICONTROL FTE] entspricht 1, wenn der Benutzer Vollzeit arbeitet, wie im Zeitplan definiert.
* Der Wert von [!UICONTROL Arbeitszeit] für den Benutzer, der auf die Zeit verweist, die der Benutzer für projektbezogene Arbeit verbringt. Dies umfasst keine Zeit mit Mehraufwand, wie z. B. Sitzungen und Schulungen. Die [!UICONTROL Arbeitszeit] entspricht 1, wenn der Benutzer die gesamte Zeit für die Arbeit zur Verfügung steht, wie durch die [!UICONTROL FTE] oder den Zeitplan angegeben. Das bedeutet, dass er keine Zeit für nicht projektbezogene Arbeiten wie Meetings oder Trainings verbringt.


Informationen zur Planung und Planung von Ressourcen in [!DNL Workfront] finden Sie unter [Erste Schritte mit der Ressourcenverwaltung](../../../resource-mgmt/resource-mgmt-overview/get-started-resource-management.md).


## Voreinstellungen für die [!UICONTROL Ressourcenverwaltung] konfigurieren

>[!NOTE]
>
>Da es sich um eine globale Einstellung handelt, wirkt sich diese Auswahl auf alle Berechnungen für das gesamte System aus, für alle Benutzer, in allen Tools zur Ressourcenverwaltung.

{{step-1-to-setup}}

1. Klicken Sie auf **[!UICONTROL Ressourcenverwaltung]**.
1. Wählen Sie eine der folgenden Methoden aus, um die Verfügbarkeit von Benutzern in [!DNL Workfront] zu berechnen:

   * **Der Standardzeitplan**: [!DNL Workfront] verwendet den Standardzeitplan des Systems und die individuelle FTE des Benutzers, um die Verfügbaren Stunden des Benutzers in Tools zur Ressourcenverwaltung zu berechnen.

     Weitere Informationen zu Zeitplänen finden Sie unter [Erstellen eines Zeitplans](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

     Weitere Informationen zum Auffinden des Werts im [!UICONTROL FTE] des Benutzers finden Sie unter [Profil eines Benutzers bearbeiten](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

     Workfront berechnet die Verfügbaren Stunden eines Benutzers anhand der folgenden Formel, wenn der Workfront-Administrator den [!UICONTROL Standardzeitplan] auswählt:


     `User Available Hours = [([!UICONTROL Default Schedule] Hours - [!UICONTROL Exceptions]) * [!UICONTROL FTE] - Time off hours] * [!UICONTROL Work Time]`


     >[!INFO]
     >
     >Wenn der Standardzeitplan beispielsweise 40 Stunden pro Woche beträgt, die FTE im Benutzerprofil 0,5 beträgt, der Benutzer eine Stunde Freizeit von einem Tag hat und die [!UICONTROL Arbeitszeit] im Benutzerprofil 0,5 beträgt, ist der Benutzer für die tatsächliche Projektarbeit 9,5 Stunden pro Woche verfügbar.
     >
     >Wenn der Benutzer eine Stunde Zeit pro Tag hat, werden seine Verfügbaren Stunden wie folgt berechnet:
     >
     >
     >`User Available Hours = [((40 - 0) * 0.5) - 1] * 0.5 = 9.5 hours`
     >

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

   * **Der Zeitplan des Benutzers**: [!DNL Workfront] verwendet den Zeitplan des Benutzers sowie den [!UICONTROL Standardzeitplan] des Systems, um den Wert &quot;Verfügbar&quot;[!UICONTROL FTE] des Benutzers in den Tools für die Ressourcenverwaltung zu berechnen. Die verfügbaren Stunden werden nur nach dem Zeitplan des Benutzers berechnet. Der Wert von [!UICONTROL FTE] des Benutzers wird ignoriert. Dies ist die Standardeinstellung.

     Weitere Informationen zu Zeitplänen finden Sie unter [Erstellen eines Zeitplans](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

     Weitere Informationen zum [!UICONTROL Zeitplan] eines Benutzers finden Sie unter [Profil eines Benutzers bearbeiten](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

     >[!NOTE]
     >
     >Wenn der Benutzer keinem Zeitplan zugeordnet ist, werden die Verfügbaren Stunden für den Benutzer nur mit dem [!UICONTROL Standardzeitplan] berechnet.

     Die verfügbaren Stunden für den Benutzer werden anhand der folgenden Formel berechnet:


     `User Available Hours = (Hours from the [!UICONTROL Schedule] of the User - Schedule Exceptions - Time off hours) * [!UICONTROL Work Time]`


     Die verfügbare [!UICONTROL FTE] für den Benutzer wird anhand der folgenden Formel berechnet:


     `User Available [!UICONTROL FTE] = [(Hours from the [!UICONTROL Schedule] of the User - Schedule Exceptions - Time off hours) * [!UICONTROL Work Time]] / [!UICONTROL Default Schedule] hours`


     >[!INFO]
     >
     >Wenn der [!UICONTROL Standardzeitplan] beispielsweise 40 Stunden pro Woche beträgt, beträgt der Zeitplan des Benutzers 30 Stunden pro Woche und die [!UICONTROL Arbeitszeit] des Benutzers beträgt 0,5, die [!UICONTROL FTE] des Benutzers beträgt 0,35.
     >
     >Wenn der Benutzer zwei Stunden Zeit pro Tag hat, wird seine wöchentliche Verfügbarkeit [!UICONTROL FTE] wie folgt berechnet:
     >
     >
     >`User Weekly Available [!UICONTROL FTE] = [(30-2) * 0.5] / 40 = 0.35`
     >

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
