---
title: Verwalten von Benutzern in Adobe Admin Console
description: Als Adobe-Administrator können Sie Adobe Workfront-Benutzer und Systemadministratoren mit der Adobe Admin Console erstellen.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: ae657964-d4a5-4c3b-afc6-8dde7695955d
source-git-commit: dfd8dd07e1a88da872550163051e703f6aea5f74
workflow-type: tm+mt
source-wordcount: '1121'
ht-degree: 0%

---

# Verwalten von Benutzern in Adobe Admin Console

>[!IMPORTANT]
>
>Die Funktion in diesem Artikel ist nur verfügbar, wenn die Workfront-Instanz Ihres Unternehmens in der Adobe Business Platform integriert wurde.
>
>Eine Liste der Verfahren, die je nachdem, ob Ihr Unternehmen in die Adobe Business Platform integriert wurde, unterschiedlich sind, finden Sie unter [Plattformbasierte Verwaltungsunterschiede (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

Als Adobe-Administrator können Sie Adobe Workfront-Benutzer und Systemadministratoren mit der Adobe Admin Console erstellen. Die Konsole ist ein zentraler Speicherort für die Verwaltung der Adobe-Berechtigungen in Ihrem gesamten Unternehmen. Weitere Informationen finden Sie unter [Übersicht über Admin Consolen](https://helpx.adobe.com/de/enterprise/using/admin-console.html).

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Abo</td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe-Administratorrechte</td> 
   <td> <p>Sie müssen Produktkonfigurationsadministrator für Adobe-Produkte für Ihr Unternehmen sein.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Voraussetzungen

Bevor Sie die Admin Console für Workfront verwenden, sollten Sie eine E-Mail erhalten, in der Sie zur Konsole eingeladen werden.

1. Wenn Sie mit dem Adobe noch nicht vertraut sind und eine E-Mail erhalten haben, in der Sie darüber informiert werden, dass Sie nun über Administratorrechte für Adobe-Software und -Dienste für Ihr Unternehmen verfügen, klicken Sie auf die Schaltfläche in der E-Mail, um ein Adobe-Konto zu erstellen und die Admin Console zu öffnen.

   Oder

   Wenn Sie bereits über ein Adobe-Konto verfügen, gehen Sie zum [Adobe Admin Console-Seite](https://adminconsole.adobe.com/).

## Weitere Informationen zum Adobe Admin Console

* Workfront-Systemadministratoren können einen Workfront-Benutzer in Workfront deaktivieren, dies deaktiviert jedoch nicht den Benutzer in der Admin Console.

  <!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For information about deactivating a user in Workfront, see </p>
  -->

* Der Benutzer **Startseite** wird anhand des Benutzers bestimmt, der sie erstellt hat. Dies kann nicht innerhalb der Admin Console angepasst werden.
* Die Zugriffsstufe &quot;Systemadministrator&quot;von Workfront kann nur in der Adobe Admin Console bearbeitet werden.

  <!--
  DRAFTED IN FLARE:
  How is this done?
  
  -->

* Das Ändern des Benutzerzugriffs von Systemadministrator auf eine andere Zugriffsebene muss zuerst über die Admin Console erfolgen.

  <!--
   This is not clear
  -->

* Um den Systemadministratorzugriff von einem Benutzer in Workfront zu entfernen, müssen Sie den Adobe Admin Console verwenden, um den Benutzer als Produktprofiladministrator zu entfernen. Dadurch wird die Workfront-Zugriffsstufe des Benutzers von &quot;Systemadministrator&quot;in &quot;Anforderer&quot;geändert.

  >[!IMPORTANT]
  >
  >Nehmen Sie keine Änderungen am Produktprofil selbst vor.

## Zugriff auf den Benutzer- und Administratorbereich für Ihre Produktionsinstanz von Workfront {#access-the-user-and-admin-area-for-your-production-instance-of-workfront}

1. Aus dem [Adobe Admin Console-Seite](https://adminconsole.adobe.com/), wählen Sie die **Produkte** in der oberen Navigationsleiste ein und wählen Sie dann die **Workfront** Produktkachel.

   ![](assets/admin-product-1.png)

1. Wählen Sie in der angezeigten Liste den Link oben aus.

   Dies ist Ihre Produktionsinstanz, in der Ihre Benutzer arbeiten.

   ![](assets/instances-1.png)

   >[!TIP]
   >
   >Der zweite Link in der Liste, Ihre Vorschauinstanz, ist eine Testumgebung, die Ihre Live-Produktionsumgebung repliziert. Weitere Informationen finden Sie unter [Die Adobe Workfront-Vorschau-Sandbox-Umgebung](../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md).
   >
   >
   >Möglicherweise werden in der Liste auch Links zu Sandbox-Umgebungen angezeigt. Weitere Informationen finden Sie unter [Die Adobe Workfront-Vorschau-Sandbox-Umgebung](../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md).

1. In der Liste, die angezeigt wird, mit dem **Produktprofile** auf den Namen des Workfront-Produktprofils klicken.

   ![](assets/prod-profile-1.png)

   Diese Liste enthält alle Benutzer, die bereits Ihrer Produktionsinstanz von Workfront zugewiesen sind.

   >[!IMPORTANT]
   >
   >Nehmen Sie keine Änderungen am Produktprofil selbst vor.

1. Fahren Sie mit einem der folgenden Abschnitte in diesem Artikel fort:

   * [Erstellen von Benutzern in Workfront mit Adobe Admin Console](#create-users-in-workfront-with-the-adobe-admin-console)
   * [Erstellen von Systemadministratoren in Workfront mit Adobe Admin Console](#create-system-administrators-in-workfront-with-the-adobe-admin-console)

## Erstellen von Benutzern in Workfront mit Adobe Admin Console {#create-users-in-workfront-with-the-adobe-admin-console}

Workfront-Benutzer müssen der Adobe Admin Console hinzugefügt werden. Ein Administrator kann den Benutzer direkt in der Adobe Admin Console erstellen. Gruppenadministratoren erstellen Benutzer in Workfront, die dann zur Genehmigung eingereicht werden. Nach der Genehmigung wird der Benutzer der Adobe Admin Console hinzugefügt.

* [Erstellen von Benutzern in Workfront direkt in der Adobe Admin Console](#create-users-in-workfront-directly-in-the-adobe-admin-console)
* [Benutzer in Workfront erstellen und für die Adobe Admin Console genehmigen](#create-users-in-workfront-and-approve-them-for-the-adobe-admin-console)

### Erstellen von Benutzern in Workfront direkt in der Adobe Admin Console

1. Navigieren Sie zum Benutzer- und Administratorbereich der Admin Console, wie im Abschnitt beschrieben. [Zugriff auf den Benutzer- und Administratorbereich für Ihre Produktionsinstanz von Workfront](#access-the-user-and-admin-area-for-your-production-instance-of-workfront) in diesem Artikel.
1. Mit dem **Benutzer** oberhalb der Liste ausgewählte Registerkarte, wählen Sie **Benutzer hinzufügen**.
1. Im **Benutzer zu diesem Produktprofil hinzufügen** Geben Sie die E-Mail-Adresse oder den Namen eines Benutzers ein, den Sie hinzufügen möchten, und wählen Sie **Speichern**.

   Der Benutzer wird in Workfront mit der Zugriffsstufe Anforderer erstellt.

   >[!IMPORTANT]
   >
   >Nehmen Sie keine Änderungen am Produktprofil selbst vor.

1. Ändern Sie in Workfront die Zugriffsebene des Benutzers.

   Anweisungen dazu, wie ein Workfront-Administrator die Zugriffsstufe eines Benutzers ändern kann, finden Sie unter [Profil eines Benutzers bearbeiten](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

1. Wiederholen Sie die Schritte 3 und 4, um weitere Benutzer hinzuzufügen.

   >[!NOTE]
   >
   >Für neue Adobe-Benutzer stellt die Admin Console eine E-Mail bereit, um sie zum Abschluss des Registrierungsprozesses einzuladen. Alle Benutzer müssen den Registrierungsprozess abschließen, um auf eine beliebige Adobe-Anwendung zugreifen zu können.
   >
   >Für bestehende Adobe-Benutzer kann der Benutzer eine E-Mail über die Verfügbarkeit von Workfront erhalten oder auch nicht. Dies ist eine vom Adobe-Administrator kontrollierte Voreinstellung für das Produkt.

### Benutzer in Workfront erstellen und für die Adobe Admin Console genehmigen

Mit diesem Workflow können Gruppenadministratoren, die keinen Zugriff auf die Adobe Admin Console haben, Benutzer erstellen.

Zuerst erstellt der Gruppenadministrator den Benutzer in Workfront. Dadurch wird der Benutzer im Status Deaktiviert und Ausstehende Genehmigung erstellt.

Anschließend genehmigt ein Workfront-Administrator den Benutzer. Dadurch wird der Benutzer in Workfront aktiviert und zur Adobe Admin Console hinzugefügt.

#### Benutzer in Workfront erstellen (Gruppenadministrator)

Anweisungen zum Erstellen eines Benutzers in Workfront finden Sie unter [Benutzer hinzufügen](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/add-users.md).

#### Benutzer genehmigen (Workfront-Administrator)

So genehmigen Sie einen Benutzer:

{{step-1-to-users}}

1. Wählen Sie den Benutzer aus und klicken Sie auf das M **o** Symbol &quot;re&quot; ![](assets/more-icon.png).

1. Klicken Sie zur Genehmigung des Benutzers auf **Genehmigen** Klicken Sie auf **Einsenden**.

   Oder

   Um den Benutzer abzulehnen und ihn aus Workfront zu löschen, klicken Sie auf **Ablehnen** Klicken Sie auf **Einsenden**.

   Genehmigte Benutzer werden automatisch zur Adobe Admin Console hinzugefügt.

   Abgelehnte Benutzer werden automatisch aus Workfront gelöscht.



## Erstellen von Systemadministratoren in Workfront mit Adobe Admin Console {#create-system-administrators-in-workfront-with-the-adobe-admin-console}

Die Zugriffsebene für Systemadministratoren wird nur auf der Adobe Admin Console gewährt. Sie können in Workfront keinen Administratorzugriff gewähren oder entfernen.

Sie müssen einen Benutzer zu Ihrer Produktionsinstanz von Workfront hinzufügen, bevor Sie ihn zu einem Workfront-Systemadministrator machen können. Anweisungen finden Sie im Abschnitt . [Erstellen von Benutzern in Workfront mit Adobe Admin Console](#create-users-in-workfront-with-the-adobe-admin-console) in diesem Artikel.

1. Navigieren Sie zum Benutzer- und Administratorbereich der Admin Console, wie im Abschnitt beschrieben. [Zugriff auf den Benutzer- und Administratorbereich für Ihre Produktionsinstanz von Workfront](#access-the-user-and-admin-area-for-your-production-instance-of-workfront) in diesem Artikel.
1. Wählen Sie die **Administratoren** oberhalb der Benutzerliste.
1. Auswählen **Admin hinzufügen**.
1. Im **Produktprofiladministratoren hinzufügen** Geben Sie die E-Mail-Adressen oder Namen der Administratoren ein, die Sie hinzufügen möchten, und wählen Sie **Speichern**.

   ![](assets/add-admin-1.png)

   Die Systemadministratoren werden in Workfront erstellt.

   >[!IMPORTANT]
   >
   >Nehmen Sie keine Änderungen am Produktprofil selbst vor.



<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>&nbsp;</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<p>You can create Adobe Workfront users and system administrators with the <a href="https://adminconsole.adobe.com/" alt="Admin Console link">Adobe Admin Console</a>. The console is a central location for managing the Adobe entitlements across your organization. For more information, see the <a href="https://helpx.adobe.com/enterprise/using/admin-console.html" alt="Admin Console Overview">Admin Console Overview</a>.</p>
<p>Before using the Admin Console for Workfront, you should receive a receive an email inviting you to the console. Click in the invitation to accept it and create an account. You can also use an existing account, if already available.</p>
<h2>Create users</h2>
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Create users in WF with the Adobe admin console</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">May need to add something about oging throug WF -- check with Jonah</p>

<p>To create users in Workfront with the Admin Console:</p>
<ol>
<li value="1"> <p>From the <a href="https://adminconsole.adobe.com/">Admin Console page</a>, select the <b>Products</b> tab and then select the <b>Workfront</b> product tile.</p> </li>
<li value="2"> <p>Select the link to the Workfront instance you want to change.</p> </li>
<li value="3"> <p>Select the Product profile link. This shows a list of the currently-assigned users. If the list is very long, you can also search for users in the search field above the list.</p> </li>
<li value="4"> <p>Select the <b>Add User</b> button.</p> </li>
<li value="5"> <p>In the <b>Add users</b> box, enter the email address or name of the user you want to add. Select <b>Save</b>. The administrator is created in Workfront with <b>Requestor</b> access level.</p> </li>
</ol>
<h2>Create system administrators</h2>
<p>To create system administrators:</p>
<ol>
<li value="1"> <p>Make product profile assignments first. To be a Workfront System Administrator, the user must be assigned the Workfront product profile and be an admin for that product profile.</p> </li>
<li value="2"> <p>From the console, select the <b>Products</b> tab and then select the <b>Admins</b> tab. </p> </li>
<li value="3"> <p>Select <b>Add Admin</b>.</p> </li>
<li value="4"> <p>In the <b>Add product profile administrators</b> box, enter the email address or name of the administrator you want to add. Select <b>Save</b>. The user is created in Workfront with <b>Requestor</b> access level.</p> </li>
</ol>
<h2>Additional details for the Admin Console</h2>
<ul>
<li> <p>System Administrator access level is granted only on the Admin Console. You cannot grant or remove admin access from within Workfront.</p> </li>
</ul>
<ul>
<li> <p>Creating and deleting users inside Workfront is only possible through the Admin Console.</p> </li>
<li> <p>Workfront System Administrators can deactivate Workfront users from within Workfront, but this does not deactivate the user in the Admin Console.</p> </li>
<li> <p>All new users are are assigned <b>Requestor</b> access level upon creation. Also, the user <b>Home Group</b> is determined based on the user who created them. This is currently not customizable from within the Admin Console.</p> </li>
<li> <p>The Workfront System Administrator access level can only be edited from within the Adobe Admin Console.</p> </li>
<li> <p>Editing a user who is a system admin to any other access level must be done through the Admin Console first.</p> </li>
<li> <p>To remove Workfront system admin access, remove users as Product Profile Administrators. This action changes the user access level in Workfront from a system admin to a <b>Requestor</b>.</p> </li>
</ul>
</div>
-->
