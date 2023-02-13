---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: organization-setup
title: Deaktivieren oder Reaktivieren eines Unternehmens
description: Sie können ein Unternehmen deaktivieren, das Sie nicht mehr verwenden, während Sie alle zugehörigen historischen Daten beibehalten. Wenn Sie ein Unternehmen deaktivieren, das bereits irgendwo im System verwendet wird, funktioniert es wie immer. Es wird nicht entfernt oder blockiert.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 479dfb9d-0e47-4790-a33a-336b415fbf6e
source-git-commit: b6f6964bb80f172849434c669df2b0ecd735a590
workflow-type: tm+mt
source-wordcount: '410'
ht-degree: 0%

---

# Deaktivieren oder Reaktivieren eines Unternehmens

Sie können ein Unternehmen deaktivieren, das Sie nicht mehr verwenden, während Sie alle zugehörigen historischen Daten beibehalten. Wenn Sie ein Unternehmen deaktivieren, das bereits irgendwo im System verwendet wird, funktioniert es wie immer. Es wird nicht entfernt oder blockiert.

## Zugriffsanforderungen

Sie müssen über Folgendes verfügen, um Unternehmen in [!DNL Workfront]:

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Workfront] Plan*</p> </td> 
   <td>[!UICONTROL Team] oder höher</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Adobe Workfront] license*</p> </td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"><strong>Konfigurationen auf Zugriffsebene*</strong> </td> 
   <td> <p>Eine der folgenden Optionen:</p> 
    <ul> 
     <li> <p>Die Zugriffsstufe [!UICONTROL Systemadministrator], mit der Sie jedes Unternehmen im System bearbeiten können. Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Gewähren eines vollen Administratorzugriffs</a>. </p> </li> 
     <li> <p>Verwaltungszugriff zur Verwaltung von Unternehmen, mit dem Sie jedes Unternehmen im System bearbeiten können. Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Benutzern administrativen Zugriff auf bestimmte Bereiche gewähren</a>.</p> </li> 
    </ul> <p><b>NOTIZ</b>:  
     <ul> 
      <li> <p>Sie können auch Unternehmen verwalten, die mit einer beliebigen Gruppe verbunden sind, der Sie als Gruppenadministrator zugewiesen sind.</p> </li> 
      <li> <p>Um Benutzer zum [!DNL Workfront] -System verwenden, müssen Sie über einen der folgenden Schritte verfügen:</p> 
       <ul> 
        <li> <p>Die Zugriffsstufe des [!UICONTROL Systemadministrators]. Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Gewähren eines vollen Administratorzugriffs</a>. </p> </li> 
        <li> <p>In Ihrer Zugriffsebene muss [!UICONTROL Bearbeiten] für die Einstellung [!UICONTROL Benutzer] ausgewählt sein. Außerdem können Sie für die Einstellung [!UICONTROL Benutzer] unter [!UICONTROL Feinabstimmung Ihrer Einstellungen] <img src="assets/gear-icon-in-access-levels.png"> , müssen die Option [!UICONTROL Erstellen] und mindestens eine der beiden [!UICONTROL User Admin]-Optionen aktiviert sein. </p> <p> <img src="assets/access-req-users.png" style="width: 350;height: 101;"> </p> <p>Wenn Sie die Option [!UICONTROL Benutzeradministrator (Gruppenbenutzer)] verwenden, müssen Sie Gruppenadministrator einer Gruppe sein, der der Benutzer angehört.</p> </li> 
       </ul> <p>Informationen zur Benutzereinstellung auf Zugriffsebene finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Benutzern Zugriff gewähren</a>.</p> </li> 
     </ul> </p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren [!DNL Workfront] Administrator.

## Deaktivieren oder Reaktivieren eines Unternehmens

1. Klicken Sie auf **[!UICONTROL Hauptmenü]** icon ![](assets/main-menu-icon.png) in der oberen rechten Ecke von [!DNL Adobe] Workfront, und klicken Sie dann auf **[!UICONTROL Einrichtung]** ![](assets/gear-icon-settings.png).

1. Klicken Sie im linken Bereich auf **[!UICONTROL Unternehmen]** ![](assets/companies-icon-left-panel.png).

1. Wählen Sie ein oder mehrere Unternehmen aus, die deaktiviert oder reaktiviert werden sollen.
1. Klicken **[!UICONTROL Bearbeiten]**.
1. Bei einem einzelnen Unternehmen deaktivieren Sie die **[!UICONTROL Ist aktiv]** , um sie zu deaktivieren oder die Option zu aktivieren.

   Oder

   Wählen Sie für mehrere Unternehmen **[!UICONTROL Nein]** von **[!UICONTROL Ist aktiv]** Dropdown-Menü, um sie zu deaktivieren, oder **[!UICONTROL Ja]** , um sie zu aktivieren.

1. Klicken **[!UICONTROL Änderungen speichern]**.
