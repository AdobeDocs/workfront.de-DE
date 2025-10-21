---
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-system-defaults
title: Einstellungen für die Ressourcenverwaltung konfigurieren
description: Als  [!DNL Adobe Workfront]  können Sie die Voreinstellungen für die Ressourcenverwaltung für Ihr System konfigurieren. Diese Ressourcenverwaltungsvoreinstellungen bestimmen, wie die Benutzerverfügbarkeit oder -kapazität und das FTE für die  [!DNL Workfront] - und Planungstools berechnet werden.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 7cde2238-cb34-4bee-baba-69d256a3912d
source-git-commit: cd0214917620e0b147d0da3402ea2d34e28bc9c3
workflow-type: tm+mt
source-wordcount: '628'
ht-degree: 0%

---

# Einstellungen [!UICONTROL Ressourcenverwaltung] konfigurieren

<!-- Audited: 5/2025 -->

<!--Linked to lots of articles for resource planning and LINKED TO CONTEXT SENSITIVE HELP - DO NOT CHANGE OR REMOVE!</p>
Edit the first part, once they add more settings in the Res Management Preferences - right now, only the FTE calculation is the
-->

Als [!DNL Adobe Workfront] können Sie die Voreinstellungen [!UICONTROL Ressourcenverwaltung] für Ihr System konfigurieren. Diese Voreinstellungen bestimmen, wie die Verfügbarkeit oder Kapazität der Benutzerstunden bzw. FTE für die [!DNL Workfront] Ressourcenplanungs- und Planungstools berechnet wird.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] Packstück</td> 
   <td><p>Beliebig</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] Lizenz</td> 
   <td><p>[!UICONTROL Standard]</p>
       <p>[!UICONTROL-Plan]</p></td>
  </tr> 
  <tr> 
   <td>Konfigurationen der Zugriffsebene</td> 
   <td>[!UICONTROL Systemadministrator]</td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Bei der Berechnung der Kapazität eines Benutzers berücksichtigte Informationen

Bei der Berechnung der Kapazität eines Benutzers berücksichtigt Workfront die folgenden Informationen:

* Die Anzahl der geplanten Stunden, wie im Zeitplan des Benutzers oder im Standardzeitplan des Workfront-Systems definiert.
* Zeitplanausnahmen (je nachdem, welcher Zeitplan verwendet wird, können dies die Ausnahmen des Zeitplans des Benutzers oder die mit dem Workfront-Standardzeitplan verknüpften sein).
* Die Urlaubszeit des Benutzers.
* Der Wert des Vollzeitäquivalents ([!UICONTROL FTE]) des Benutzers oder des [!DNL Workfront]. Der [!UICONTROL FTE] entspricht 1, wenn der Benutzer wie im Zeitplan definiert Vollzeit arbeitet.
* Der Wert von [!UICONTROL Arbeitszeit] für den Benutzer, der sich auf die Zeit bezieht, die der Benutzer für projektbezogene Arbeit aufwendet. Dazu gehören keine Overhead-Zeit wie Meetings und Schulungen. Die [!UICONTROL Arbeitszeit] ist gleich 1, wenn der Benutzer die gesamte Zeit für Arbeit zur Verfügung steht, wie im [!UICONTROL FTE] oder Zeitplan angegeben, was bedeutet, dass er keine Zeit mit nicht projektbezogener Arbeit wie Meetings oder Schulungen verbringt.


Informationen zur Planung und Planung von Ressourcen in [!DNL Workfront] finden Sie unter [Erste Schritte mit dem Ressourcen-Management](../../../resource-mgmt/resource-mgmt-overview/get-started-resource-management.md).


## Einstellungen [!UICONTROL Ressourcenverwaltung] konfigurieren

>[!NOTE]
>
>Da es sich um eine globale Einstellung handelt, wirkt sich diese Auswahl auf alle Berechnungen für das gesamte System, für alle Benutzer und für alle Ressourcen-Management-Tools aus.

{{step-1-to-setup}}

1. Klicken Sie **[!UICONTROL Ressourcenverwaltung]**.
1. Wählen Sie eine der folgenden Methoden, um die Verfügbarkeit der Benutzer in [!DNL Workfront] zu berechnen:

   * **Standardzeitplan**: [!DNL Workfront] berechnet mithilfe des Standardzeitplans des Systems und des individuellen FTE des Benutzers die verfügbaren Stunden des Benutzers in Ressourcen-Management-Tools.

     Weitere Informationen finden Sie unter [Erstellen eines Zeitplans](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md) und [Bearbeiten des Benutzerprofils](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

     Wenn diese Option aktiviert ist, berechnet Workfront die verfügbaren Stunden des Benutzers anhand der folgenden Formel:


     `User Available Hours = [([!UICONTROL Default Schedule] Hours - [!UICONTROL Exceptions]) * [!UICONTROL FTE] - Time off hours] * [!UICONTROL Work Time]`


     >[!INFO]
     >
     >Wenn der Standardzeitplan beispielsweise 40 Stunden pro Woche beträgt, hat der FTE im Benutzerprofil 0,5, der Benutzer hat einen Tag Ausfallzeit von einer Stunde und die [!UICONTROL Arbeitszeit] im Benutzerprofil beträgt 0,5, und der Benutzer steht 9,5 Stunden pro Woche für die tatsächliche Projektarbeit zur Verfügung.
     >
     >Wenn der/die Benutzende an einem Tag 1 Stunde Ausfallzeit hat, werden die verfügbaren Stunden wie folgt berechnet:
     >
     >
     >`User Available Hours = [((40 - 0) * 0.5) - 1] * 0.5 = 9.5 hours`
     >

     <!--
      This used to be the calculation before we implemented the Work Time field: 
    
      ```
      User Available Hours = ([!UICONTROL Default Schedule] Hours - Exceptions) * FTE - Time off hours
      ```

      >[!INFO]
      >
      > For example, if the [!UICONTROL Default Schedule] is 40 hours a week and the [!UICONTROL FTE] in the profile of the user is 0.5, the user is available to work for 20 hours a week.
      >If the user has 1 hour of Time off one day, their Available Hours will be calculated as follows:
      >
      >
      >User Available Hours = [(40 - 0) * 0.5)] - 1 = 19 hours
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

   * **Der Zeitplan des Benutzers**: [!DNL Workfront] verwendet den Zeitplan des Benutzers sowie den [!UICONTROL Standardzeitplan] des Systems, um den Wert „Verfügbar [!UICONTROL VZÄ] des Benutzers in Ressourcen-Management-Tools zu berechnen. Die verfügbaren Stunden werden nur gemäß dem Zeitplan des Benutzers berechnet, und der Wert des [!UICONTROL  (VZÄ] des Benutzers wird ignoriert. Dies ist die Standardeinstellung.

     Weitere Informationen finden Sie unter [Erstellen eines Zeitplans](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md) und [Bearbeiten des Benutzerprofils](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

     >[!NOTE]
     >
     >Wenn der/die Benutzende keinem Zeitplan zugeordnet ist, werden die verfügbaren Stunden für den/die Benutzende(n) nur anhand des [!UICONTROL Standardzeitplans] berechnet.

     Die verfügbaren Stunden für den Benutzer werden anhand der folgenden Formel berechnet:


     `User Available Hours = (Hours from the [!UICONTROL Schedule] of the User - Schedule Exceptions - Time off hours) * [!UICONTROL Work Time]`


     Der verfügbare [!UICONTROL  (VZÄ] für den Benutzer wird anhand der folgenden Formel berechnet:


     `User Available [!UICONTROL FTE] = [(Hours from the [!UICONTROL Schedule] of the User - Schedule Exceptions - Time off hours) * [!UICONTROL Work Time]] / [!UICONTROL Default Schedule] hours`


     >[!INFO]
     >
     >Wenn der [!UICONTROL Standardzeitplan] beispielsweise 40 Stunden pro Woche beträgt, hat der Benutzer einen Zeitplan von 30 Stunden pro Woche, die [!UICONTROL Arbeitszeit] des Benutzers ist 0,5 und der [!UICONTROL VZÄ] des Benutzers ist 0,35.
     >
     >Wenn der/die Benutzende an einem Tag 2 Stunden Ausfallzeit hat, wird sein/ihr wöchentlich verfügbarer [!UICONTROL FTE] wie folgt berechnet:
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
