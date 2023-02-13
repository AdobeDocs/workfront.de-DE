---
user-type: administrator
product-area: system-administration
navigation-topic: organization-setup
title: Verwalten von Firmenmitgliedschaften
description: Im [!UICONTROL Unternehmen] -Bereich unter Einrichtung können Sie die Mitglieder eines Unternehmens hinzufügen und entfernen. Sie können auch ihre Benutzerprofile bearbeiten und sie daran erinnern, sich bei [!DNL Workfront], deactivate them in [!DNL Workfront], and remove them from the [!DNL Workfront] System.
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

Im [!UICONTROL Unternehmen] Gebiet in [!UICONTROL Einrichtung], können Sie die Mitglieder eines Unternehmens hinzufügen und entfernen. Sie können auch ihre Benutzerprofile bearbeiten und sie daran erinnern, sich bei [!DNL Workfront], deaktivieren Sie sie in [!DNL Workfront]und entfernen Sie sie aus dem [!DNL Workfront] System.

Informationen zum Erstellen eines neuen Unternehmens finden Sie unter [Erstellen und Bearbeiten von Unternehmen](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

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
        <li> <p>In Ihrer Zugriffsebene muss [!UICONTROL Bearbeiten] für die Einstellung [!UICONTROL Benutzer] ausgewählt sein. Außerdem können Sie für die Einstellung [!UICONTROL Benutzer] unter [!UICONTROL Feinabstimmung Ihrer Einstellungen] <img src="assets/gear-icon-in-access-levels.png"> , müssen die Option [!UICONTROL Erstellen] und mindestens eine der beiden [!UICONTROL User Admin]-Optionen aktiviert sein. </p> <p> <img src="assets/access-req-users.png"> </p> <p>Wenn Sie die Option [!UICONTROL Benutzeradministrator (Gruppenbenutzer)] verwenden, müssen Sie Gruppenadministrator einer Gruppe sein, der der Benutzer angehört.</p> </li> 
       </ul> <p>Informationen zur Benutzereinstellung auf Zugriffsebene finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Benutzern Zugriff gewähren</a>.</p> </li> 
     </ul> </p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren [!DNL Workfront] Administrator.

## Verwalten von Firmenmitgliedschaften

1. Klicken Sie auf **[!UICONTROL Hauptmenü]** icon ![](assets/main-menu-icon.png) in der oberen rechten Ecke von [!DNL Adobe Workfront]Klicken Sie auf **[!UICONTROL Einrichtung]** ![](assets/gear-icon-settings.png).

1. Klicken **[!UICONTROL Unternehmen]**.
1. Klicken Sie auf den Namen des Unternehmens.
1. Mit dem **[!UICONTROL Firmenmitglieder]** im linken Bereich ausgewählt sind, führen Sie einen der folgenden Schritte aus:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Mitglied hinzufügen</td> 
      <td> <p>Klicken <b>[!UICONTROL Add member]</b>und wählen Sie dann eine der folgenden Optionen im angezeigten Dropdownmenü aus:</p> 
       <ul> 
        <li> <p><b>[!UICONTROL Neuer Benutzer]</b>: Einen Benutzer hinzufügen, der noch nicht zu hinzugefügt wurde [!DNL Workfront].</p> <p>Informationen zum Hinzufügen von Benutzern zu [!DNL Workfront], siehe <a href="../../../administration-and-setup/add-users/create-and-manage-users/add-users.md" class="MCXref xref">Benutzer hinzufügen</a> und <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Benutzerprofil bearbeiten</a>.</p> </li> 
        <li> <p><b>[!DNL Existing user]</b>: Fügen Sie einen bereits im System vorhandenen Benutzer hinzu, auf den Sie Zugriff haben, um ihn zu bearbeiten.</p> <p><b>WICHTIG</b>: Wenn der Benutzer bereits Mitglied eines anderen Unternehmens ist, überschreibt die neue Zuweisung die alte. Der Benutzer verliert den Zugriff auf Artikel, die für das vorherige Unternehmen freigegeben wurden, und erhält Zugriff auf Artikel, die für dieses Unternehmen freigegeben wurden.</p> </li> 
        <li> <p><b>[!UICONTROL Benutzer importieren]</b>: Importieren Sie Benutzer, indem Sie eine Datei für den Tabellenimport hochladen. Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/add-users/create-and-manage-users/import-users.md" class="MCXref xref">Benutzer importieren</a>.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Mitglieder bearbeiten</td> 
      <td> 
       <ol> 
        <li value="1"> <p>Wählen Sie mindestens einen Benutzer aus und klicken Sie dann auf das Symbol [!UICONTROL Bearbeiten] . <img src="assets/edit-icon.png"> in der Symbolleiste.</p> </li> 
        <li value="2"> <p>Konfigurieren Sie die Optionen im <b>[!UICONTROL Benutzer bearbeiten]</b> angezeigt.</p> <p>Weitere Informationen zu diesen Optionen finden Sie unter <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Benutzerprofil bearbeiten</a>.</p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Mitglied kopieren</td> 
      <td> <p>Sie können ein Unternehmensmitglied erstellen, indem Sie ein vorhandenes kopieren. </p> <p><b>NOTIZ</b>:  <p>Wenn Sie einen Benutzer auf diese Weise erstellen, werden alle Informationen vom ursprünglichen Benutzer in den neu erstellten Benutzer kopiert, mit Ausnahme der folgenden:</p> 
        <ul> 
         <li>Die Informationen im Abschnitt [!UICONTROL Persönliche Informationen] .</li> 
         <li>[!UICONTROL Wenn ich mich anmelde, zeigen Sie]: In diesem Feld wird der Standard-Landingtab für die Zugriffsebene ausgewählt.</li> 
         <li>[!UICONTROL Direkte Berichte]</li> 
        </ul> </p> 
       <ol> 
        <li value="1"> <p>Wählen Sie den Benutzer aus und klicken Sie auf das Symbol [!UICONTROL Kopieren] . <img src="assets/copy-icon.png">. </p> </li> 
        <li value="2"> <p>Im <b>[!UICONTROL Neuer Benutzer]</b> die Felder, die für den neuen Benutzer verfügbar sind, bearbeiten.</p> <p>Informationen zu allen Feldern, die mit einem Benutzer verknüpft sind, finden Sie unter <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Benutzerprofil bearbeiten</a>.</p> </li> 
        <li value="3"> <p>Klicken <strong>[!UICONTROL Diesen Benutzer hinzufügen]</strong>.</p> <p>Oder</p> <p>Klicken <strong>[!UICONTROL Benutzer hinzufügen und einen anderen starten]</strong> , um den neuen Benutzer zu speichern und einen weiteren hinzuzufügen.</p> </li> 
       </ol> <p>Dadurch wird ein neues Konto in [!DNL Workfront] für den Benutzer.</p> <p>Wenn Sie die Option zum Senden einer Einladung an den Benutzer ausgewählt haben, sollte dieser eine E-Mail erhalten, über die er einem Link folgen kann, um seine [!DNL Workfront] Kennwort.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Benutzer entfernen</td> 
      <td> 
       <div> 
        <p>Wählen Sie mindestens einen Benutzer aus, klicken Sie auf <b>[!UICONTROL Benutzer entfernen]</b>und wählen Sie dann eine der folgenden Optionen im angezeigten Dropdownmenü aus:</p> 
        <ul> 
         <li> <p><b>[!UICONTROL Aus Unternehmen löschen]</b>: Entfernt den Benutzer aus dem Unternehmen.</p> </li> 
         <li> <p><b>[!UICONTROL Löschen]</b>: Löscht den Benutzer aus der [!DNL Workfront] System.</p> <p><b>WICHTIG</b>: Durch das Löschen eines Benutzers aus dem System werden auch Informationen gelöscht, die mit dem Benutzer verknüpft sind, den Sie möglicherweise beibehalten möchten. Es wird empfohlen, Benutzer zu deaktivieren, anstatt sie zu löschen. Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">Benutzer deaktivieren oder reaktivieren</a>.</p> </li> 
        </ul> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Senden Sie einen Kommentar an Benutzer und deren [!UICONTROL Updates]-Bereiche.</td> 
      <td> 
       <ol> 
        <li value="1"> <p>Wählen Sie mindestens einen Benutzer aus und klicken Sie dann auf das Symbol [!UICONTROL Kommentar] . <img src="assets/comment-icon.png"> in der Symbolleiste.</p> </li> 
        <li value="2"> <p>Geben Sie den Kommentar ein, den Sie den Benutzern und im Bereich [!UICONTROL Updates] ihrer Benutzerprofile senden möchten.</p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Liste der Unternehmensmitglieder exportieren</td> 
      <td> <p>Klicken Sie auf das Symbol [!UICONTROL Export] . <img src="assets/export.png"> Wählen Sie in der Symbolleiste das gewünschte Format für die exportierte Datei aus.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Mitglieder im System deaktivieren</td> 
      <td> <p>Wählen Sie mindestens einen Benutzer aus und klicken Sie auf das Symbol [!UICONTROL Mehr] . <img src="assets/more-icon.png"> Wählen Sie in der Symbolleiste die Option <b>[!UICONTROL Deactivate]</b>.</p> <p>Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">Benutzer deaktivieren oder reaktivieren</a>.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Benutzer daran erinnern, sich im System zu registrieren</td> 
      <td> <p> Im <b>[!UICONTROL Name]</b> Spalte, <b>[!UICONTROL Abgemeldet]</b> neben dem Namen jedes abgemeldeten Benutzers angezeigt. Um diese Benutzer daran zu erinnern, sich im System zu registrieren, wählen Sie die Benutzer aus und klicken Sie auf das Symbol [!UICONTROL Mehr] . <img src="assets/more-icon.png"> Wählen Sie in der Symbolleiste die Option <b>[!UICONTROL Benutzer zur Registrierung erinnern]</b>.</p> </td> 
     </tr> 
    </tbody> 
   </table>
