---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: organization-setup
title: Deaktivieren oder Reaktivieren eines Unternehmens
description: Sie können ein Unternehmen, das Sie nicht mehr verwenden, deaktivieren und dabei alle zugehörigen historischen Daten beibehalten. Wenn Sie ein Unternehmen deaktivieren, das bereits irgendwo im System verwendet wird, funktioniert es weiterhin wie immer. Es wird nicht entfernt oder blockiert.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 479dfb9d-0e47-4790-a33a-336b415fbf6e
source-git-commit: 439303273239549bb326c171be44eea321f5bb5f
workflow-type: tm+mt
source-wordcount: '371'
ht-degree: 1%

---

# Unternehmen deaktivieren oder reaktivieren

Sie können ein Unternehmen, das Sie nicht mehr verwenden, deaktivieren und dabei alle zugehörigen historischen Daten beibehalten. Wenn Sie ein Unternehmen deaktivieren, das bereits irgendwo im System verwendet wird, funktioniert es weiterhin wie immer. Es wird nicht entfernt oder blockiert.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto">
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Workfront] Plan</p> </td> 
   <td><p>Aktuell: [!UICONTROL Team] oder höher</p>
   <p>Oder</p>
   <p>Neu: Beliebig</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Adobe Workfront] Lizenz</p> </td> 
   <td><p>Aktuell: [!UICONTROL Plan]</p>
   <p>Oder</p>
   <p>Neu: [!UICONTROL Standard]</p>
   </td> 
  </tr>
  <tr data-mc-conditions=""> 
   <td role="rowheader"><strong>Konfigurationen der Zugriffsebene</strong> </td> 
   <td> <p>Eine der folgenden Möglichkeiten:</p> 
    <ul> 
     <li> <p>Die Zugriffsebene [!UICONTROL Systemadministrator], mit der Sie jede Firma im System bearbeiten können.</p> </li> 
     <li> <p>Administrativer Zugriff auf die Verwaltung von Unternehmen, wodurch Sie jedes Unternehmen im System bearbeiten können.</p> </li> 
    </ul> <p><b>HINWEIS</b>:  
     <ul> 
      <li> <p>Sie können auch Firmen verwalten, die mit einer beliebigen Gruppe verknüpft sind, der Sie als Gruppenadministrator zugewiesen sind.</p> </li> 
      <li> <p>Um Benutzer zum [!DNL Workfront] hinzuzufügen und daraus zu entfernen, benötigen Sie eine der folgenden Eigenschaften:</p> 
       <ul> 
        <li> <p>Zugriffsebene des [!UICONTROL Systemadministrators].</p> </li> 
        <li> <p>In Ihrer Zugriffsebene muss [!UICONTROL Bearbeiten] für die Einstellung [!UICONTROL Benutzer] ausgewählt sein. Außerdem müssen für die Einstellung [!UICONTROL Users] unter [!UICONTROL Feinabstimmung der Einstellungen] <img src="assets/gear-icon-in-access-levels.png"> die Option [!UICONTROL Create] und mindestens eine der beiden [!UICONTROL User Admin]-Optionen aktiviert sein. </p> <p> <img src="assets/access-req-users.png"> </p> <p>Wenn Sie die Option [!UICONTROL Benutzeradmin (Gruppenbenutzer)] verwenden, müssen Sie Gruppenadministrator einer Gruppe sein, in der der Benutzer Mitglied ist.</p> </li> 
       </ul>
       </li> 
     </ul> </p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Unternehmen deaktivieren oder reaktivieren

{{step-1-to-setup}}

1. Klicken Sie im linken Bedienfeld auf **[!UICONTROL Firmen]** ![](assets/companies-icon-left-panel.png).

1. Wählen Sie ein oder mehrere Unternehmen zum Deaktivieren oder Reaktivieren aus.
1. Klicken Sie **[!UICONTROL Bearbeiten]**.
1. Deaktivieren Sie für ein einzelnes Unternehmen die Option **[!UICONTROL Ist aktiv]**, um sie zu deaktivieren, oder aktivieren Sie die Option, um sie zu aktivieren.

   Oder

   Bei mehreren Unternehmen wählen Sie **[!UICONTROL Nein]** aus dem Dropdown-Menü **[!UICONTROL Ist aktiv]** aus, um sie zu deaktivieren, oder **[!UICONTROL Ja]**, um sie zu aktivieren.

1. Klicken Sie auf **[!UICONTROL Änderungen speichern]**.
