---
user-type: administrator
product-area: system-administration
navigation-topic: organization-setup
title: Verwalten von Unternehmensmitgliedschaften
description: Im Bereich [!UICONTROL Firmen] im Setup können Sie die Mitglieder einer Firma hinzufügen und entfernen. Sie können auch ihre Benutzerprofile bearbeiten und sie daran erinnern, sich im System  [!DNL Workfront], deactivate them in [!DNL Workfront], and remove them from the [!DNL Workfront] .
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: f0efd985-76e3-435e-bf19-87008f6a5e9d
source-git-commit: 15063d937a5ba9b5285c66a0987e8deea6cc6d74
workflow-type: tm+mt
source-wordcount: '839'
ht-degree: 1%

---

# Verwalten von Unternehmensmitgliedschaften

Im Bereich [!UICONTROL Firmen] in [!UICONTROL Setup] können Sie die Mitglieder einer Firma hinzufügen und entfernen. Sie können auch ihre Benutzerprofile bearbeiten, sie daran erinnern, sich in [!DNL Workfront] zu registrieren, sie in [!DNL Workfront] deaktivieren und sie aus dem [!DNL Workfront] entfernen.

Informationen zum Erstellen einer neuen Firma finden Sie unter [Erstellen und Bearbeiten von Firmen](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

<table style="table-layout:auto">
 <tbody> 
  <tr> 
   <td> <p>[!DNL Workfront] Packstück</p> </td> 
   <td><p>Beliebig</p>
   </td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] Lizenz</p> </td> 
   <td><p>[!UICONTROL-Plan]</p>
   <p>[!UICONTROL Standard]</p>
   </td> 
  </tr>
  <tr> 
   <td>Konfigurationen der Zugriffsebene</td> 
  <td> <p>Sie müssen eine der folgenden Möglichkeiten haben:</p> 
    <ul> 
     <li> <p>Die Zugriffsebene [!UICONTROL Systemadministrator], mit der Sie jede Firma im System bearbeiten können.</p> </li> 
     <li> <p>Administrativer Zugriff auf die Verwaltung von Unternehmen, wodurch Sie jedes Unternehmen im System bearbeiten können.</p> </li> 
    </ul> <p><b>HINWEIS</b>:  
     <ul> 
      <li> <p>Sie können auch Firmen verwalten, die mit einer beliebigen Gruppe verknüpft sind, der Sie als Gruppenadministrator zugewiesen sind.</p> </li> 
      <li> <p>Um Benutzer zum [!DNL Workfront] hinzuzufügen oder daraus zu entfernen, benötigen Sie eine der folgenden Eigenschaften:</p> 
       <ul> 
        <li> <p>Zugriffsebene des [!UICONTROL Systemadministrators]. </p> </li> 
        <li> <p><b>[!UICONTROL Users]</b> Einstellung in der Zugriffsebene konfiguriert, um den[!UICONTROL Edit]<b>-Zugriff zu </b>, wobei <b>[!UICONTROL Create]</b> und mindestens eine der beiden <b>[!UICONTROL User Admin]</b> Optionen unter <b> </b>[!UICONTROL Feinabstimmung der Einstellungen]<img src="assets/gear-icon-in-access-levels.png"> aktiviert ist. </p> <p> <img src="assets/access-req-users.png"> </p> <p>Wenn <b>[!UICONTROL User Admin (Group Users)]</b> aktiviert ist, müssen Sie unter diesen beiden Optionen Gruppenadministrator einer Gruppe sein, in der der Benutzer Mitglied ist.</p> </li> 
       </ul>
       </li> 
     </ul> </p> </td>
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Verwalten von Unternehmensmitgliedschaften

{{step-1-to-setup}}

1. Klicken Sie auf **[!UICONTROL Firmen]**.
1. Klicken Sie auf den Namen der Firma.
1. Klicken Sie **[!UICONTROL linken]** auf „Firmenmitglieder“.
1. Führen Sie einen der folgenden Schritte aus:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Mitglied hinzufügen</td> 
      <td> <p>Klicken Sie auf <b>[!UICONTROL Mitglied hinzufügen]</b> und wählen Sie dann im angezeigten Dropdown-Menü eine der folgenden Optionen aus:</p> 
       <ul> 
        <li> <p><b>[!UICONTROL Neuer Benutzer]</b>: Fügen Sie einen Benutzer hinzu, der noch nicht zu [!DNL Workfront] hinzugefügt wurde.</p> <p>Informationen zum Hinzufügen von Benutzern zu [!DNL Workfront] finden Sie unter <a href="../../../administration-and-setup/add-users/create-and-manage-users/add-users.md" class="MCXref xref">Hinzufügen von </a> und <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Bearbeiten des Benutzerprofils</a>.</p> </li> 
        <li> <p><b>[!DNL Existing user]</b>: Einen bereits im System vorhandenen Benutzer hinzufügen, auf den Sie Zugriff zur Bearbeitung haben.</p> <p><b>WICHTIG</b>: Wenn der Benutzer bereits Mitglied eines anderen Unternehmens ist, überschreibt die neue Zuweisung die alte. Der Benutzer verliert den Zugriff auf Elemente, die mit der vorherigen Firma freigegeben wurden, und erhält Zugriff auf Elemente, die mit dieser Firma freigegeben wurden.</p> </li> 
        <li> <p><b>[!UICONTROL Benutzer importieren]</b>: Importieren Sie eine Benutzerin oder einen Benutzer durch Hochladen einer Tabellenimportdatei. Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/add-users/create-and-manage-users/import-users.md" class="MCXref xref">Benutzer importieren</a>.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Mitglieder bearbeiten</td> 
      <td> 
       <ol> 
        <li value="1"> <p>Wählen Sie mindestens einen Benutzer aus und klicken Sie dann auf das Symbol [!UICONTROL Bearbeiten] <img src="assets/edit-icon.png"> der Symbolleiste.</p> </li> 
        <li value="2"> <p>Konfigurieren Sie die Optionen im angezeigten Feld <b>[!UICONTROL </b>].</p> <p>Weitere Informationen zu diesen Optionen finden <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref"> unter „Benutzerprofil bearbeiten</a>.</p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Mitglied kopieren</td> 
      <td> <p>Sie können ein Firmenmitglied erstellen, indem Sie ein vorhandenes kopieren. </p> <p><b>HINWEIS</b>:  <p>Wenn Sie einen Benutzer auf diese Weise erstellen, werden alle Informationen vom ursprünglichen Benutzer an den neu erstellten Benutzer kopiert, mit Ausnahme der folgenden:</p> 
        <ul> 
         <li>Die Informationen im Abschnitt [!UICONTROL Persönliche Info].</li> 
         <li>[!UICONTROL Wenn ich mich anmelde, anzeigen]: Die standardmäßige Landing-Registerkarte für die Zugriffsebene wird in diesem Feld ausgewählt.</li> 
         <li>[!UICONTROL Direct Reports]</li> 
        </ul> </p> 
       <ol> 
        <li value="1"> <p>Wählen Sie den Benutzer aus und klicken Sie dann auf das Symbol [!UICONTROL Copy] <img src="assets/copy-icon.png">. </p> </li> 
        <li value="2"> <p>Bearbeiten Sie im angezeigten Feld <b>[!UICONTROL New User]</b> die für den neuen Benutzer verfügbaren Felder.</p> <p>Informationen zu allen mit einem Benutzer verknüpften Feldern finden Sie unter <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Bearbeiten des Benutzerprofils</a>.</p> </li> 
        <li value="3"> <p>Klicken Sie auf <strong>[!UICONTROL Diesen Benutzer hinzufügen]</strong>.</p> <p>Oder</p> <p>Klicken Sie auf <strong>[!UICONTROL Person-Benutzer hinzufügen und einen anderen starten]</strong>, um den neuen Benutzer zu speichern und einen weiteren hinzuzufügen.</p> </li> 
       </ol> <p>Dadurch wird ein neues Konto in [!DNL Workfront] für den Benutzer erstellt.</p> <p>Wenn Sie die Option zum Senden einer Einladung an den Benutzer ausgewählt haben, sollte er eine E-Mail erhalten, in der er einem Link folgen kann, um sein [!DNL Workfront] Kennwort zu erstellen.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Benutzer entfernen</td> 
      <td> 
       <div> 
        <p>Wählen Sie mindestens einen Benutzer aus, klicken Sie auf <b>[!UICONTROL Benutzer entfernen]</b> und wählen Sie dann im angezeigten Dropdown-Menü eine der folgenden Optionen aus:</p> 
        <ul> 
         <li> <p><b>[!UICONTROL Aus Firma entfernen]</b>: Entfernt den/die Benutzer aus der Firma.</p> </li> 
         <li> <p><b>[!UICONTROL Delete]</b>: Löscht den/die Benutzer aus dem [!DNL Workfront].</p> <p><b>WICHTIG</b>: Beim Löschen eines Benutzers aus dem System werden auch mit dem Benutzer verknüpfte Informationen gelöscht, die Sie möglicherweise beibehalten möchten. Es wird empfohlen, Benutzer zu deaktivieren, anstatt sie zu löschen. Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">Deaktivieren oder Reaktivieren eines Benutzers</a>.</p> </li> 
        </ul> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Senden eines Kommentars an Benutzer und deren Bereich [!UICONTROL Updates]</td> 
      <td> 
       <ol> 
        <li value="1"> <p>Wählen Sie mindestens einen Benutzer aus und klicken Sie dann in der Symbolleiste <b>Aktualisierung an </b> senden).</p> </li> 
        <li value="2"> <p>Geben Sie den Kommentar ein, den Sie den Benutzern und dem Bereich [!UICONTROL Updates] ihrer Benutzerprofile senden möchten.</p>
         <p>Weitere Informationen finden Sie unter <a href="/help/quicksilver/people-teams-and-groups/work-directly-with-others/send-direct-messages-to-other-users.md">Senden von Direktnachrichten an andere Benutzer</a>.</p></li> 
       </ol>
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Exportieren der Liste der Firmenmitglieder</td> 
      <td> <p>Klicken Sie auf das Symbol [!UICONTROL Export] <img src="assets/export.png"> der Symbolleiste und wählen Sie dann das Format aus, das Sie für die exportierte Datei verwenden möchten.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Mitglieder im System deaktivieren</td> 
      <td> <p>Wählen Sie mindestens einen Benutzer aus, klicken Sie auf das Symbol [!UICONTROL Mehr] <img src="assets/more-icon.png"> in der Symbolleiste und wählen Sie <b>[!UICONTROL Deaktivieren]</b>.</p> <p>Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">Deaktivieren oder Reaktivieren eines Benutzers</a>.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Benutzer an die Registrierung im System erinnern</td> 
      <td> <p> In der Spalte <b>[!UICONTROL Name]</b> wird <b>[!UICONTROL Unregistered]</b> neben dem Namen jedes nicht registrierten Benutzers angezeigt. Um diese Benutzer daran zu erinnern, sich im System zu registrieren, wählen Sie die Benutzer aus, klicken Sie auf das Symbol [!UICONTROL Mehr] <img src="assets/more-icon.png"> in der Symbolleiste und wählen Sie dann <b>[!UICONTROL Benutzer an die Registrierung erinnern]</b>.</p> </td> 
     </tr> 
    </tbody> 
   </table>
