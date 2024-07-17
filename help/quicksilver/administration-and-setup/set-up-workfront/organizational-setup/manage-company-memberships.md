---
user-type: administrator
product-area: system-administration
navigation-topic: organization-setup
title: Verwalten von Firmenmitgliedschaften
description: Im Bereich [!UICONTROL Unternehmen] im Setup können Sie die Mitglieder eines Unternehmens hinzufügen und entfernen. Sie können auch ihre Benutzerprofile bearbeiten und sie daran erinnern, sich im [!DNL Workfront], deactivate them in [!DNL Workfront], and remove them from the [!DNL Workfront] System zu registrieren.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: f0efd985-76e3-435e-bf19-87008f6a5e9d
source-git-commit: b6f6964bb80f172849434c669df2b0ecd735a590
workflow-type: tm+mt
source-wordcount: '910'
ht-degree: 1%

---

# Verwalten von Firmenmitgliedschaften

Im Bereich [!UICONTROL Unternehmen] in der [!UICONTROL Einrichtung] können Sie die Mitglieder eines Unternehmens hinzufügen und entfernen. Sie können auch ihre Benutzerprofile bearbeiten, sie daran erinnern, sich in [!DNL Workfront] zu registrieren, sie in [!DNL Workfront] deaktivieren und aus dem System [!DNL Workfront] entfernen.

Informationen zum Erstellen eines neuen Unternehmens finden Sie unter [Erstellen und Bearbeiten von Unternehmen](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

## Zugriffsanforderungen

Sie müssen über Folgendes verfügen, um Unternehmen in [!DNL Workfront] zu verwalten:

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Workfront] plan*</p> </td> 
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
     <li> <p>Die Zugriffsstufe [!UICONTROL Systemadministrator], mit der Sie jedes Unternehmen im System bearbeiten können. Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Gewähren des vollen Administratorzugriffs für einen Benutzer</a>. </p> </li> 
     <li> <p>Verwaltungszugriff zur Verwaltung von Unternehmen, mit dem Sie jedes Unternehmen im System bearbeiten können. Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Gewähren von Benutzern administrativen Zugriff auf bestimmte Bereiche</a>.</p> </li> 
    </ul> <p><b>NOTE</b>:  
     <ul> 
      <li> <p>Sie können auch Unternehmen verwalten, die mit einer beliebigen Gruppe verbunden sind, der Sie als Gruppenadministrator zugewiesen sind.</p> </li> 
      <li> <p>Um Benutzer zum System [!DNL Workfront] hinzuzufügen und daraus zu entfernen, müssen Sie über einen der folgenden Schritte verfügen:</p> 
       <ul> 
        <li> <p>Die Zugriffsstufe des [!UICONTROL Systemadministrators]. Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Gewähren des vollen Administratorzugriffs für einen Benutzer</a>. </p> </li> 
        <li> <p>In Ihrer Zugriffsebene muss [!UICONTROL Bearbeiten] für die Einstellung [!UICONTROL Benutzer] ausgewählt sein. Außerdem müssen für die Einstellung [!UICONTROL Benutzer] unter [!UICONTROL Feinabstimmung Ihrer Einstellungen] <img src="assets/gear-icon-in-access-levels.png"> die Option [!UICONTROL Erstellen] und mindestens eine der beiden Optionen [!UICONTROL Benutzeradministrator] aktiviert sein. </p> <p> <img src="assets/access-req-users.png"> </p> <p>Wenn Sie die Option [!UICONTROL Benutzeradministrator (Gruppenbenutzer)] verwenden, müssen Sie Gruppenadministrator einer Gruppe sein, der der Benutzer angehört.</p> </li> 
       </ul> <p>Weitere Informationen zur Einstellung "Benutzer"auf einer Zugriffsebene finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Gewähren des Zugriffs für Benutzer</a>.</p> </li> 
     </ul> </p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren [!DNL Workfront] -Administrator, um herauszufinden, welche Konfigurationen für Plan, Lizenztyp oder Zugriffsstufe Sie haben.

## Verwalten von Firmenmitgliedschaften

1. Klicken Sie auf das Symbol **[!UICONTROL Hauptmenü]** oben rechts in [!DNL Adobe Workfront] und dann auf **[!UICONTROL Setup]** ![](assets/gear-icon-settings.png).![](assets/main-menu-icon.png)

1. Klicken Sie auf **[!UICONTROL Unternehmen]**.
1. Klicken Sie auf den Namen des Unternehmens.
1. Führen Sie bei ausgewähltem Abschnitt **[!UICONTROL Unternehmensmitglieder]** im linken Bereich einen der folgenden Schritte aus:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Mitglied hinzufügen</td> 
      <td> <p>Klicken Sie auf <b>[!UICONTROL Add Member]</b> und wählen Sie dann eine der folgenden Optionen im angezeigten Dropdownmenü aus:</p> 
       <ul> 
        <li> <p><b>[!UICONTROL Neuer Benutzer]</b>: Fügen Sie einen Benutzer hinzu, der noch nicht zu [!DNL Workfront] hinzugefügt wurde.</p> <p>Weitere Informationen zum Hinzufügen von Benutzern zu [!DNL Workfront] finden Sie unter <a href="../../../administration-and-setup/add-users/create-and-manage-users/add-users.md" class="MCXref xref">Benutzer hinzufügen</a> und <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Profil eines Benutzers bearbeiten</a>.</p> </li> 
        <li> <p><b>[!DNL Existing user]</b>: Fügen Sie einen Benutzer hinzu, der bereits im System vorhanden ist und auf den Sie Zugriff haben.</p> <p><b>WICHTIG</b>: Wenn der Benutzer bereits Mitglied eines anderen Unternehmens ist, überschreibt die neue Zuweisung die alte. Der Benutzer verliert den Zugriff auf Artikel, die für das vorherige Unternehmen freigegeben wurden, und erhält Zugriff auf Artikel, die für dieses Unternehmen freigegeben wurden.</p> </li> 
        <li> <p><b>[!UICONTROL Benutzer importieren]</b>: Importieren Sie Benutzer, indem Sie eine Tabellenimportdatei hochladen. Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/add-users/create-and-manage-users/import-users.md" class="MCXref xref">Benutzer importieren</a>.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Mitglieder bearbeiten</td> 
      <td> 
       <ol> 
        <li value="1"> <p>Wählen Sie mindestens einen Benutzer aus und klicken Sie dann in der Symbolleiste auf das Symbol [!UICONTROL Bearbeiten] <img src="assets/edit-icon.png"> .</p> </li> 
        <li value="2"> <p>Konfigurieren Sie die Optionen im angezeigten Feld <b>[!UICONTROL Benutzer bearbeiten]</b> .</p> <p>Weitere Informationen zu diesen Optionen finden Sie unter <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Profil eines Benutzers bearbeiten</a>.</p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Mitglied kopieren</td> 
      <td> <p>Sie können ein Unternehmensmitglied erstellen, indem Sie ein vorhandenes kopieren. </p> <p><b>NOTE</b>:  <p>Wenn Sie einen Benutzer auf diese Weise erstellen, werden alle Informationen vom ursprünglichen Benutzer in den neu erstellten Benutzer kopiert, mit Ausnahme der folgenden:</p> 
        <ul> 
         <li>Die Informationen im Abschnitt [!UICONTROL Persönliche Informationen] .</li> 
         <li>[!UICONTROL Beim Anmelden anzeigen]: In diesem Feld wird die Standard-Landingpage für die Zugriffsebene ausgewählt.</li> 
         <li>[!UICONTROL Direkte Berichte]</li> 
        </ul> </p> 
       <ol> 
        <li value="1"> <p>Wählen Sie den Benutzer aus und klicken Sie dann auf das Symbol [!UICONTROL Kopieren] <img src="assets/copy-icon.png">. </p> </li> 
        <li value="2"> <p>Bearbeiten Sie im angezeigten Feld <b>[!UICONTROL Neuer Benutzer]</b> die für den neuen Benutzer verfügbaren Felder.</p> <p>Informationen zu allen Feldern, die mit einem Benutzer verknüpft sind, finden Sie unter <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Profil eines Benutzers bearbeiten</a>.</p> </li> 
        <li value="3"> <p>Klicken Sie auf <strong>[!UICONTROL Diesen Benutzer hinzufügen]</strong>.</p> <p>Oder</p> <p>Klicken Sie auf <strong>[!UICONTROL Benutzer hinzufügen und einen anderen starten]</strong> , um den neuen Benutzer zu speichern und einen weiteren hinzuzufügen.</p> </li> 
       </ol> <p>Dadurch wird ein neues Konto in [!DNL Workfront] für den Benutzer erstellt.</p> <p>Wenn Sie die Option zum Senden einer Einladung an den Benutzer ausgewählt haben, sollte dieser eine E-Mail erhalten, über die er einem Link folgen kann, um sein [!DNL Workfront]-Kennwort zu erstellen.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Benutzer entfernen</td> 
      <td> 
       <div> 
        <p>Wählen Sie mindestens einen Benutzer aus, klicken Sie auf <b>[!UICONTROL Benutzer entfernen]</b> und wählen Sie dann eine der folgenden Optionen im angezeigten Dropdownmenü aus:</p> 
        <ul> 
         <li> <p><b>[!UICONTROL Aus Unternehmen entfernen]</b>: Entfernt den Benutzer oder die Benutzer aus dem Unternehmen.</p> </li> 
         <li> <p><b>[!UICONTROL Löschen]</b>: Löscht den Benutzer oder die Benutzer aus dem [!DNL Workfront] System.</p> <p><b>WICHTIG</b>: Durch Löschen eines Benutzers aus dem System werden auch Informationen gelöscht, die mit dem Benutzer verknüpft sind, den Sie möglicherweise beibehalten möchten. Es wird empfohlen, Benutzer zu deaktivieren, anstatt sie zu löschen. Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">Deaktivieren oder Reaktivieren eines Benutzers</a>.</p> </li> 
        </ul> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Senden Sie einen Kommentar an Benutzer und deren [!UICONTROL Updates]-Bereiche.</td> 
      <td> 
       <ol> 
        <li value="1"> <p>Wählen Sie mindestens einen Benutzer aus und klicken Sie dann in der Symbolleiste auf das [!UICONTROL Kommentar]-Symbol <img src="assets/comment-icon.png"> .</p> </li> 
        <li value="2"> <p>Geben Sie den Kommentar ein, den Sie den Benutzern und im Bereich [!UICONTROL Updates] ihrer Benutzerprofile senden möchten.</p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Liste der Unternehmensmitglieder exportieren</td> 
      <td> <p>Klicken Sie in der Symbolleiste auf das [!UICONTROL Export]-Symbol <img src="assets/export.png"> und wählen Sie dann das Format für die exportierte Datei aus.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Mitglieder im System deaktivieren</td> 
      <td> <p>Wählen Sie mindestens einen Benutzer aus, klicken Sie in der Symbolleiste auf das Symbol [!UICONTROL Mehr] <img src="assets/more-icon.png"> und wählen Sie dann <b>[!UICONTROL Deactivate]</b> aus.</p> <p>Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">Deaktivieren oder Reaktivieren eines Benutzers</a>.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Benutzer daran erinnern, sich im System anzumelden</td> 
      <td> <p> In der Spalte <b>[!UICONTROL Name]</b> wird neben dem Namen jedes nicht registrierten Benutzers <b>[!UICONTROL Unregistered]</b> angezeigt. Um diese Benutzer daran zu erinnern, sich im System zu registrieren, wählen Sie die Benutzer aus, klicken Sie auf das [!UICONTROL Mehr]-Symbol <img src="assets/more-icon.png"> in der Symbolleiste und wählen Sie dann <b>[!UICONTROL Benutzer zur Registrierung erinnern]</b> aus.</p> </td> 
     </tr> 
    </tbody> 
   </table>
