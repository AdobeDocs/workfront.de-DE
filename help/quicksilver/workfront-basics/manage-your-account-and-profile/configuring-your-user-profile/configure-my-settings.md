---
product-area: user-management;setup
navigation-topic: configure-your-user-profile
title: Meine Einstellungen konfigurieren
description: Ihr [!DNL Adobe Workfront] Profil enthält Informationen über Sie (z. B. Ihren Namen, Ihre E-Mail-Adresse, Adresse, Telefonnummer, Titel usw.). Es enthält auch Informationen zu Ihren Interaktionen mit [!DNL Workfront] Benutzern und anderen Benutzern in Ihrem Unternehmen.
author: Lisa
feature: Get Started with Workfront
exl-id: 0199bf74-0611-48f0-9c05-da6afac85033
source-git-commit: 7697327455a7ffdc1a15bfa1676c3a0b091abd04
workflow-type: tm+mt
source-wordcount: '3303'
ht-degree: 1%

---

# Meine Einstellungen konfigurieren

<!-- Audited: 01/2024 -->

<!--
<p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Edit the job role FTE percentage allocation blurbs when more functionality is released: now, it says that the % is that of the user's schedule, but it will be either the user's schedule or the system schedule.</p>
-->

Ihr [!DNL Adobe Workfront] -Profil enthält Informationen über Sie (z. B. Ihren Namen, Ihre E-Mail-Adresse, Adresse, Telefonnummer, Titel usw.). Es enthält auch Informationen zu Ihren Interaktionen mit [!DNL Workfront] und anderen Benutzern in Ihrem Unternehmen (z. B. Ihren Benachrichtigungseinstellungen, den Registerkarten, die Sie in [!DNL Workfront] anzeigen möchten, oder Ihrer Auftrags-, Manager-, Gruppen- und Team-Mitgliedschaft).

Die meisten dieser Informationen wurden bereits von Ihrem [!DNL Workfront] -Administrator bei der Erstellung Ihres [!DNL Workfront] -Kontos festgelegt.

Je nachdem, welche Zugriffsebene Sie in [!DNL Workfront] haben, können Sie einige dieser Informationen bearbeiten, indem Sie Ihren Bereich [!UICONTROL Meine Einstellungen] konfigurieren.

## Auswirkungen der Zugriffsebenen auf die Bearbeitung des Bereichs [!UICONTROL Meine Einstellungen]

Je nachdem, welche Zugriffsebene Sie haben, können Sie Abschnitte in Ihrem Bereich [!UICONTROL Meine Einstellungen] bearbeiten oder nicht.

Einige Felder in bearbeitbaren Abschnitten können je nach anderen Einstellungen, die in Ihrer Zugriffsebene möglicherweise konfiguriert sind oder nicht, nicht bearbeitet werden. Weitere Informationen zum zusätzlichen Zugriff, der für die Bearbeitung einiger der in [!UICONTROL Meine Einstellungen] vorhandenen Felder erforderlich ist, finden Sie in den Abschnitten unter Konfigurieren des Bereichs [!UICONTROL Meine Einstellungen]](#configuring-the-my-settings-area) .[

Wenden Sie sich an Ihren [!DNL Workfront] -Administrator, um zu erfahren, welche Zugriffsebene Sie haben.

Das folgende Raster zeigt, welche Abschnitte im Bereich [!UICONTROL Meine Einstellungen] je nach Zugriffsebene sichtbar oder bearbeitbar sind:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>[!UICONTROL Meine Einstellungen] Bereiche</strong> </th> 
   <th><strong>Sichtbar oder bearbeitbar</strong> </th> 
   <th><strong>[!UICONTROL Systemadministrator]</strong> </th> 
   <th><strong>[!UICONTROL Standard] oder [!UICONTROL Planer]</strong> </th> 
   <th><strong>[!UICONTROL Worker]</strong> </th> 
   <th><strong>[!UICONTROL Light] oder [!UICONTROL Reviewer]</strong> </th> 
   <th><strong>[!UICONTROL Contributor] oder [!UICONTROL Requestor]</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td rowspan="2">[!UICONTROL Persönliche Informationen]</td> 
   <td> <p>Sichtbar</p> </td> 
   <td> <p>ms</p> </td> 
   <td> ms</td> 
   <td>ms </td> 
   <td>ms </td> 
   <td> ms</td> 
  </tr> 
  <tr> 
   <td> <p>Bearbeitbar</p> </td> 
   <td> <p>ms</p> </td> 
   <td> ms</td> 
   <td> ms</td> 
   <td>ms </td> 
   <td>ms </td> 
  </tr> 
  <tr> 
   <td rowspan="2">[!UICONTROL Voreinstellungen]</td> 
   <td> <p>Sichtbar</p> </td> 
   <td> <p>ms</p> </td> 
   <td> ms</td> 
   <td>ms </td> 
   <td>ms </td> 
   <td>ms </td> 
  </tr> 
  <tr> 
   <td> <p>Bearbeitbar</p> </td> 
   <td> <p>ms</p> </td> 
   <td>ms </td> 
   <td>ms </td> 
   <td>ms </td> 
   <td>ms </td> 
  </tr> 
  <tr> 
   <td rowspan="2">[!UICONTROL Benachrichtigungen]</td> 
   <td> <p>Sichtbar</p> </td> 
   <td> <p>ms</p> </td> 
   <td>ms </td> 
   <td>ms </td> 
   <td> ms</td> 
   <td>ms </td> 
  </tr> 
  <tr> 
   <td> <p>Bearbeitbar</p> </td> 
   <td> <p>ms</p> </td> 
   <td>ms </td> 
   <td>ms </td> 
   <td> ms</td> 
   <td> ms</td> 
  </tr> 
  <tr> 
   <td rowspan="2">[!UICONTROL Zugriff]</td> 
   <td>Sichtbar</td> 
   <td> ms</td> 
   <td>ms </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Bearbeitbar</td> 
   <td> ms</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td rowspan="2">[!UICONTROL Organisation]</td> 
   <td>Sichtbar</td> 
   <td>ms</td> 
   <td>ms </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Bearbeitbar</td> 
   <td>ms</td> 
   <td>ms </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td rowspan="2">[!UICONTROL Ressourcenplanung]</td> 
   <td>Sichtbar</td> 
   <td>ms</td> 
   <td>ms </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Bearbeitbar</td> 
   <td>ms</td> 
   <td>ms </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td rowspan="2">[!UICONTROL Custom Forms]</td> 
   <td>Sichtbar</td> 
   <td>ms</td> 
   <td>ms </td> 
   <td>ms</td> 
   <td>ms </td> 
   <td>ms </td> 
  </tr> 
  <tr> 
   <td>Bearbeitbar</td> 
   <td>ms </td> 
   <td>ms </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td rowspan="2">[!UICONTROL Kommentar]</td> 
   <td>Sichtbar</td> 
   <td>ms</td> 
   <td>ms </td> 
   <td>ms </td> 
   <td>ms </td> 
   <td>ms </td> 
  </tr> 
  <tr> 
   <td>Bearbeitbar</td> 
   <td>ms </td> 
   <td>ms </td> 
   <td>ms </td> 
   <td>ms </td> 
   <td>ms </td> 
  </tr> 
 </tbody> 
</table>

## Konfigurieren des Bereichs [!UICONTROL Meine Einstellungen]

{{step1-click-profile-pic}}

1. Klicken Sie auf das Menü **[!UICONTROL Mehr]** neben Ihrem Namen ![Mehr Menü](assets/more-icon.png) und dann auf **[!UICONTROL Bearbeiten]**.

1. Je nach Zugriffsebene können Sie die folgenden Abschnitte aktualisieren:

   * [Persönliche Info](#personal-info)
   * [Einstellungen](#preferences)
   * [Benachrichtigungen](#notifications)
   * [Zugriff](#access)
   * [Organisation](#organization)
   * [Ressourcenplanung](#resource-planning)
   * [Benutzerdefinierte Formulare](#custom-form)
   * [Kommentar](#comment)

1. Klicken Sie auf **[!UICONTROL Speichern]**.

### [!UICONTROL Persönliche Informationen]

Dieser Abschnitt enthält die folgenden Unterabschnitte:

* [Basisinformationen](#basic-info)
* [Auftragsinformationen](#job-info)
* [Kontaktinfos](#contact-info)

#### [!UICONTROL Grundlegende Informationen]

Diese Informationen sollten bereits von Ihrem [!DNL Workfront] -Administrator konfiguriert werden. Alle Felder in diesem Unterabschnitt sind erforderliche Felder.

Sie können Folgendes in diesem Unterabschnitt ändern:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL Vorname]</strong></td> 
   <td>Aktualisieren Sie Ihren Vornamen. Dies ist ein Pflichtfeld.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL Nachname]</strong></td> 
   <td>Aktualisieren Sie Ihren Nachnamen. Dies ist ein Pflichtfeld.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL E-Mail-Adresse]</strong></td> 
   <td> E-Mail-Adresse aktualisieren. Dies ist ein erforderliches Feld. Beachten Sie, dass Ihre E-Mail-Adresse auch Ihr Benutzername für [!DNL Workfront] ist.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL Kennwort zurücksetzen]</strong></td> 
   <td>Setzen Sie Ihr Kennwort in diesem Abschnitt zurück. Weitere Informationen zum Zurücksetzen Ihres Kennworts finden Sie unter <a href="../../../workfront-basics/manage-your-account-and-profile/managing-your-workfront-account/reset-your-password.md" class="MCXref xref">Kennwort zurücksetzen</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>(Bedingt) &lt;SSO-Konfiguration&gt; [!UICONTROL Benutzername]</strong></td> 
   <td> Wenn Ihr [!DNL Workfront] -Administrator eine SSO-Integration mit [!DNL Workfront] aktiviert hat, wird Ihr SSO-Benutzername in diesem Feld angezeigt. Der Typ der SSO-Konfiguration, die für Ihre [!DNL Workfront] -Instanz aktiviert ist, ist in diesem Feld sichtbar.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>(Bedingt) [!UICONTROL Nur &lt;SSO-Konfiguration&gt; Authentifizierung zulassen]</strong></td> 
   <td> <p> Wenn Ihr [!DNL Workfront] -Administrator eine SSO-Integration mit [!DNL Workfront] aktiviert hat und Benutzer für die einmalige Anmeldung aktualisiert hat, ist dieses Feld standardmäßig ausgewählt. Der Typ der SSO-Konfiguration, die für Ihre [!DNL Workfront] -Instanz aktiviert ist, ist in diesem Feld sichtbar.</p> <p>Wenn dieses Feld ausgewählt ist, müssen Sie sich mit Ihren SSO-Anmeldeinformationen bei [!DNL Workfront] anmelden. Wenn Sie diese Option deaktivieren, können Sie sich mit Ihren [!DNL Workfront] -Anmeldedaten bei [!DNL Workfront] anmelden.</p> <p>Weitere Informationen zum Konfigurieren von [!DNL Workfront] mit einer SSO-Lösung finden Sie unter <a href="../../../administration-and-setup/add-users/single-sign-on/single-sign-on.md" class="MCXref xref">Single Sign-on in [!DNL Workfront]: Artikelindex</a>. Weitere Informationen zum Aktualisieren von Benutzern für SSO finden Sie unter <a href="../../../administration-and-setup/add-users/single-sign-on/update-users-sso.md" class="MCXref xref">Aktualisieren von Benutzern für Single Sign-on</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Auftragsinformationen]

Sie können Folgendes in diesem Unterabschnitt ändern:

<table style="table-layout:auto">
    <tr>
        <td><strong>[!UICONTROL Titel]</strong></td>
        <td>Geben Sie Ihren Titel an. Dies entspricht nicht Ihrer beruflichen Rolle. Ihr Titel ist nicht Teil der Ressourcenplanung, während Ihre Rolle bei der Auftragsausführung gehört. Ihr Titel wird in der [!DNL Workfront] -Benutzeroberfläche überall dort angezeigt, wo Ihr Name und Ihr Avatar angezeigt werden. Sie ist für alle Benutzer sichtbar, die Zugriff haben, um Ihr Benutzerprofil anzuzeigen.</td>
    </tr>
    <tr>
        <td><strong>[!UICONTROL Mit mir reden]</strong></td>
        <td>Geben Sie Ihre beruflichen Interessen in diesem Bereich an.</td>
    </tr>
</table>

#### [!UICONTROL Kontaktinformationen]

Sie können Folgendes in diesem Unterabschnitt ändern:

<table style="table-layout:auto">
    <tr>
        <td><strong>[!UICONTROL Telefonnummer]</strong></td>
        <td> </td>
    </tr>
    <tr>
        <td><strong>[!UICONTROL Erweiterung]</strong></td>
        <td> </td>
    </tr>
    <tr>
        <td><strong>[!UICONTROL Mobiltelefonnummer]</strong></td>
        <td> </td>
    </tr>
    <tr>
        <td><strong>[!UICONTROL Adresse]</strong></td>
        <td> </td>
    </tr>
    <tr>
        <td><strong>[!UICONTROL City]</strong></td>
        <td> </td>
    </tr>
    <tr>
        <td><strong>[!UICONTROL State]</strong></td>
        <td> </td>
    </tr>
    <tr>
        <td><strong>[!UICONTROL Postleitzahl]</strong></td>
        <td> </td>
    </tr>
    <tr>
        <td><strong>[!UICONTROL Land]</strong></td>
        <td> </td>
    </tr>
    <tr>
        <td><strong>[!UICONTROL Profil - Bild]</strong></td>
        <td>Ihr Profilbild wird zu Ihrem Avatar und ist im gesamten System [!DNL Workfront] sichtbar, unabhängig davon, wo Ihr Name angezeigt wird.</td>
    </tr>
</table>

### [!UICONTROL Voreinstellungen]

Geben Sie in diesem Abschnitt an, was Sie in Ihrer [!DNL Workfront] -Oberfläche anzeigen möchten.

>[!NOTE]
>
>Benutzer mit der Lizenz [!UICONTROL Contributor] oder [!UICONTROL Requestor] haben keine weiteren Elemente des linken Bedienfelds, die zum Bereich [!UICONTROL Hauptmenü] außerhalb des Bereichs [!UICONTROL Anforderungen] hinzugefügt werden können. Ein [!DNL Workfront] -Administrator kann Benutzer mit der Lizenz [!UICONTROL Contributor] oder [!UICONTROL Requestor] einer Layoutvorlage zuweisen, die alle anderen Bereiche im [!UICONTROL Hauptmenü] enthält. Danach können sie die Bereiche auswählen, die im [!UICONTROL Hauptmenü] angezeigt werden sollen, indem sie ihr Benutzerprofil bearbeiten.

Sie können Folgendes in diesem Unterabschnitt ändern:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody>
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL Zeitzone]</strong> </td> 
   <td><p>Geben Sie Ihre Zeitzone an. Dadurch wird die in Ihren ausgehenden E-Mail-Nachrichten angezeigte Zeit gesteuert.</p>
       <p>Die Zeitzone wirkt sich auch darauf aus, was in einem PTO-Kalenderbericht angezeigt wird.</p></td>
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL E-Mail-Gebietsschema]</strong> </td> 
   <td><p>Geben Sie hier Ihre bevorzugte Sprache an. Damit wird das in ausgehenden E-Mail-Nachrichten verwendete Sprache-, Datums- und Zahlenformat gesteuert.</p>
   <p><strong>HINWEIS:</strong> Wenn sich Ihr Unternehmen auf dem Adobe Unified Experience befindet, werden Sprachvoreinstellungen in Ihrem Adobe-Profil gespeichert und das E-Mail-Gebietsschema wird nicht verwendet. Weitere Informationen finden Sie unter <a href="/help/quicksilver/workfront-basics/supported-languages-in-workfront.md#change-the-adobe-experience-cloud-language">Ändern der Adobe Experience Cloud-Sprache</a> im Artikel <a href="/help/quicksilver/workfront-basics/supported-languages-in-workfront.md">Unterstützte Sprachen in Adobe Workfront</a>.</p></td> 
  </tr>

<tr> 
   <td role="rowheader"><strong>[!UICONTROL Versand der mir zugewiesenen Arbeit an meine Registerkarte "Arbeit an"]</strong> </td> 
   <td>Dieses Feld bezieht sich auf eine veraltete Funktion, die aus [!DNL Workfront] entfernt wurde.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>(Bedingt) Automatisches Generieren von Testsendungen beim Hochladen von Dokumenten</strong></td> 
   <td>Wählen Sie dieses Feld aus, um sofort nach dem Laden des Dokuments in [!DNL Workfront] mit der Erstellung eines Testversands zu beginnen. Dieses Feld ist standardmäßig deaktiviert und kann nur von einem Workfront-Administrator aktualisiert werden.<br>Dieses Feld ist nur verfügbar, wenn Ihr Unternehmen die Workfront Proof-Komponente für Workfront erworben hat und Sie als Testversand-Benutzer aktiviert sind. Weitere Informationen zu Workfront Proof finden Sie unter <a href="../../../review-and-approve-work/proofing/managing-proofs-within-workfront/manage-proofs-in-wf.md" class="MCXref xref">Verwalten von Testsendungen in Adobe Workfront</a>.
   <p><b>Hinweis:</b> In eine Anfrage hochgeladene Dokumente erzeugen keinen Testversand automatisch. </p></td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Benachrichtigungen]

Geben Sie an, welche Benachrichtigungen von [!DNL Workfront] empfangen werden sollen. Weitere Informationen zum Konfigurieren von Benachrichtigungen finden Sie unter [Ändern eigener E-Mail-Benachrichtigungen](../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

### [!UICONTROL Zugriff]

Ihr Zugriff und andere damit verknüpfte Komponenten werden von Ihrem [!DNL Workfront] -Administrator bei der Einrichtung Ihres Kontos konfiguriert.

Nur ein [!DNL Workfront] -Administrator kann alle Felder in diesem Abschnitt anzeigen und bearbeiten.

Sie können Folgendes in diesem Unterabschnitt ändern:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL ist aktiv]</strong> </td> 
   <td>Dieses Feld ist nur für einen Benutzer sichtbar, der auch ein [!DNL Workfront] -Administrator ist, und sollte standardmäßig aktiviert sein. Dies bedeutet, dass der Benutzer aktiv ist und sich bei anmelden kann. [!DNL Workfront]</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL Zugriffsebene]</strong> </td> 
   <td>Dieses Feld ist für Benutzer mit einer Zugriffsstufe von [!UICONTROL Standard], [!UICONTROL Plan] oder [!UICONTROL Workfront-Administrator] sichtbar und kann nur für [!DNL Workfront] -Administratoren bearbeitet werden. Wenn Sie ein [!DNL Workfront] -Administrator sind, achten Sie darauf, Ihre Zugriffsebene beim Ändern dieses Felds nicht auf etwas Geringeres zu ändern. </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL Layout Template]</strong> </td> 
   <td>Dieses Feld ist für Benutzer mit Zugriffsstufe [!UICONTROL Standard], [!UICONTROL Plan] oder [!UICONTROL [!DNL Workfront] Administrator sichtbar und kann nur für [!UICONTROL [!DNL Workfront] Administratoren oder Benutzer mit einer [!UICONTROL Standard]- oder [!UICONTROL Plan]-Lizenz bearbeitet werden, die auch über Administratorzugriff verfügen. Wählen Sie hier eine Layoutvorlage aus, um das Erscheinungsbild und das Feld Ihrer Workfront-Benutzeroberfläche zu aktualisieren. Weitere Informationen zum Einrichten von Benutzern mit Administratorzugriff finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md#configure-users-access-to-edit-users-using-a-custom-access-level" class="MCXref xref">Konfigurieren des Benutzerzugriffs zum Bearbeiten mithilfe einer benutzerdefinierten Zugriffsstufe</a> in <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Gewähren des Zugriffs für Benutzer</a>.<br>Weitere Informationen zu Layoutvorlagen und deren Auswirkungen auf Ihre Benutzeroberfläche finden Sie unter <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">Erstellen und Verwalten von Layoutvorlagen</a></td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader"><strong>Log in as</strong> </td> 
    <td> <p><strong>Add access</strong> for a Workfront administrator or group administrator (associated with a group you are in) to log in as you. Select an <strong>Access expiration date</strong> for the login. </p> <p>You can repeat this to grant login access to multiple administrators.</p> <p>The settings you choose in this section are visible only to you.
       <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
        <span class="PinkDraftNote">Add a note about this being only for the Enterprise package if they decide to do it that way. Functionality that may come in a later sprint: If you want to be notified when the administrator logs in as you, select Receive an email when this user logs in.</span> 
       </MadCap:conditionalText>
      </p> </td> 
   </tr>
  --> 
  <tr> 
   <td role="rowheader"><strong>(Bedingt) [!UICONTROL Benutzer kann Testsendungen durchführen (... aus ... Testlizenzen links)]</strong></td> 
   <td>Dieses Feld ist nur verfügbar, wenn Ihr Unternehmen einen veralteten [!DNL Workfront]-Plan verwendet und die [!DNL Workfront Proof] -Komponente erworben hat. Wenn diese Option ausgewählt ist, sind Sie als Benutzer für die Überprüfung aktiviert. Außerdem wird die Anzahl der in Ihrem System verwendeten Testversandlizenzen unter der Gesamtzahl der erworbenen Testversandlizenzen angezeigt. Dieses Feld ist nur für Benutzer sichtbar und bearbeitbar, die auch [!DNL Workfront] -Administratoren sind. Weitere Informationen zu den Planungsoptionen für Testsendungen in [!DNL Workfront] finden Sie unter <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md">Zugriff auf die Testversandfunktion in [!DNL Workfront]</a>.</td>
  </tr> 
  <tr> 
   <td role="rowheader"><strong>(Bedingt) [!UICONTROL Berechtigungsprofil]</strong></td> 
   <td> <p>Dieses Feld zeigt die Zugriffsstufe an, die Sie in [!DNL Workfront Proof] haben. Sie ist nur verfügbar, wenn:</p> 
    <ul> 
     <li>Ihr Unternehmen verwendet einen veralteten [!DNL Workfront]-Plan und hat die [!DNL Workfront Proof]-Komponente erworben oder Sie verfügen über eine [!UICONTROL Standard]-, [!UICONTROL Work]- oder [!UICONTROL Plan]-Lizenz für einen neueren [!DNL Workfront]-Plan.</li> 
     <li>Sie sind als Testversand-Benutzer aktiviert.</li> 
    </ul> <p>[!DNL Workfront] -Administratoren können das Feld für alle Benutzer mit Ausnahme der Benutzer selbst bearbeiten, sodass alle Benutzer das Feld in ihren eigenen Profilen als schreibgeschützt betrachten. Weitere Informationen zum Berechtigungsprofil finden Sie unter <a href="../../../review-and-approve-work/proofing/proofing-overview/permission-profiles.md" class="MCXref xref">Übersicht über das Profil für Testversand-Berechtigungen</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Organisation]

Diese Informationen werden normalerweise von Ihrem [!DNL Workfront] -Administrator konfiguriert, wenn er Ihr [!DNL Workfront] -Konto erstellt. In diesem Abschnitt können Sie auch Informationen zu Ihrer Organisations- oder Organisationsstruktur aktualisieren. Nur Benutzer mit Zugriffsstufe [!UICONTROL Standard], [!UICONTROL Plan] oder [!UICONTROL Systemadministrator] können diesen Abschnitt bearbeiten.

Sie können Folgendes in diesem Unterabschnitt ändern:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL Company]</strong></td> 
   <td>Wählen Sie aus der Dropdown-Liste den Namen des Unternehmens aus, zu dem Sie gehören.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>(Bedingt) [!UICONTROL Berichte an]</strong></td> 
   <td>Nachdem Sie ein <strong>[!UICONTROL Unternehmen]</strong> für Ihr Profil ausgewählt haben, können Sie auch den Namen Ihres Managers in dieses Feld eingeben. Sie können hier nur einen Namen angeben. Es wird empfohlen, den Namen Ihres unmittelbaren Managers anzugeben. Geben Sie den Namen ein und wählen Sie ihn aus, wenn er in der Liste angezeigt wird.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>(Bedingt) [!UICONTROL Direkte Berichte]</strong></td> 
   <td>Nachdem Sie ein <strong>[!UICONTROL Unternehmen]</strong> für Ihr Profil ausgewählt haben, können Sie auch den Namen Ihrer direkten Berichte in dieses Feld eingeben. Hier können Sie beliebig viele direkte Berichte festlegen. Geben Sie den Namen ein und wählen Sie ihn aus, wenn er in der Liste angezeigt wird.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL Home Team]</strong> </td> 
   <td> <p>Wählen Sie ein <strong>[!UICONTROL Home Team]</strong> aus dem Dropdownmenü aus. Dieses Feld ist für Benutzer mit Zugriffsstufe [!UICONTROL Standard], [!UICONTROL Plan] oder [!UICONTROL Systemadministrator] sichtbar und kann nur für [!DNL Workfront] Administratoren oder Benutzer mit einer [!UICONTROL Standard]- oder [!UICONTROL Plan]-Lizenz bearbeitet werden, die auch über Administratorzugriff verfügen. Weitere Informationen zum Einrichten von Benutzern mit Administratorzugriff finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md#configure-users-access-to-edit-users-using-a-custom-access-level" class="MCXref xref">Konfigurieren des Benutzerzugriffs zum Bearbeiten mithilfe einer benutzerdefinierten Zugriffsstufe</a> in <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Gewähren des Zugriffs für Benutzer</a>.<br></p> <p>Ihr <strong>Startseiten-Team</strong> kann sich auf das Erscheinungsbild Ihrer [!DNL Workfront]-Benutzeroberfläche auswirken, wenn dem Team eine Layoutvorlage zugeordnet ist. </p> <p>Weitere Informationen zu Teams finden Sie unter <a href="../../../people-teams-and-groups/create-and-manage-teams/teams-overview.md" class="MCXref xref">Übersicht über Teams</a>.</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL Sonstige Teams]</strong> </td> 
   <td> <p>Sie können mehreren Teams angehören. Geben Sie zusätzliche Teams an, zu denen Sie in dieses Feld gehören, indem Sie mit der Eingabe des Teamnamens beginnen. Klicken Sie dann auf , um das Team auszuwählen, wenn es in der Liste angezeigt wird. Wenn Sie zu vielen Teams angehören, kann dies zu Verwirrung bei der Arbeit führen, die den Teams zugewiesen wird. Weitere Informationen zu Teams finden Sie unter <a href="../../../people-teams-and-groups/create-and-manage-teams/teams-overview.md" class="MCXref xref">Übersicht über Teams</a>.</p> <p>Dieses Feld ist für Benutzer mit einer [!UICONTROL Standard]-, [!UICONTROL Plan]- oder [!UICONTROL Systemadministrator]-Lizenz sichtbar und kann nur für [!DNL Workfront] -Administratoren oder Benutzer mit einer [!UICONTROL Standard]- oder [!UICONTROL Plan]-Lizenz bearbeitet werden, die auch über Administratorzugriff verfügen. Weitere Informationen zum Einrichten von Benutzern mit Administratorzugriff finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md#configure-users-access-to-edit-users-using-a-custom-access-level" class="MCXref xref">Konfigurieren des Benutzerzugriffs zum Bearbeiten mithilfe einer benutzerdefinierten Zugriffsstufe</a> in <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Gewähren des Zugriffs für Benutzer</a>.</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL Home Group]</strong> </td> 
   <td> <p>Wählen Sie eine <strong>[!UICONTROL Home Group]</strong> aus dem Dropdownmenü aus.</p> <p>Hinweis: Dies ist ein erforderliches Feld. Sie können keinen Benutzer haben, der keiner Gruppe zugeordnet ist.<br></p> <p>Dieses Feld ist für Benutzer mit der Ebene [!UICONTROL Standard], [!UICONTROL Plan] oder [!UICONTROL Systemadministrator] sichtbar. Weitere Informationen darüber, wer das Feld <strong>[!UICONTROL Home Group]</strong> bearbeiten kann, finden Sie unter <a href="/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md"class="MCXref xref">Profil eines Benutzers bearbeiten</a>. Ihre <strong>[!UICONTROL Home Group]</strong> ist die Standardgruppe für alle Projekte und die standardmäßige <strong>[!UICONTROL Home Group]</strong> für alle neuen Benutzer, die Sie erstellen. Alle benutzerdefinierten Formulare, die Sie erstellen, werden standardmäßig für Ihre <strong>[!UICONTROL Home Group]</strong> freigegeben.</p> <p>Weitere Informationen zu Gruppen finden Sie unter <a href="../../../administration-and-setup/manage-groups/groups-overview/groups.md" class="MCXref xref">Gruppenübersicht</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL Sonstige Gruppen]</strong> </td> 
   <td> <p>Sie können mehreren Gruppen angehören. Geben Sie in diesem Feld zusätzliche Gruppen an, denen Sie angehören, indem Sie mit der Eingabe des Gruppennamen beginnen. Klicken Sie auf , um es auszuwählen, wenn es in der Liste angezeigt wird. Dieses Feld ist für Benutzer mit Zugriffsstufe [!UICONTROL Standard], [!UICONTROL Plan] oder [!UICONTROL Systemadministrator] sichtbar. Weitere Informationen darüber, wer das Feld <strong>[!UICONTROL Sonstige Gruppen]</strong> bearbeiten kann, finden Sie unter <a href="/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md"class="MCXref xref">Profil eines Benutzers bearbeiten</a>.</p> <p>Weitere Informationen zu Gruppen finden Sie unter <a href="../../../administration-and-setup/manage-groups/groups-overview/groups.md" class="MCXref xref">Gruppenübersicht</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Ressourcenplanung]

Ihre Informationen zur Ressourcenplanung beeinflussen den Zeitrahmen der Arbeitszuweisungen, die Zeit der Protokollierung, die Kosten und den Umsatz der Projekte, in denen Sie sich befinden. Normalerweise wird dieser Bereich vom [!DNL Workfront] -Administrator, einem Projekt- oder Ressourcen-Manager oder von Ihrem Direktmanager aktualisiert.

Verwenden Sie Folgendes in diesem Abschnitt:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL Deaktivierung des Zeitplans]</strong></td> 
   <td>Aktivieren Sie dieses Kontrollkästchen, wenn Sie planen möchten, dass Ihr Konto nach einem bestimmten Zeitraum deaktiviert werden soll. Im <p><strong>[!UICONTROL Geplantes Deaktivierungsdatum]</strong>, das angezeigt wird, geben Sie das Datum an, nach dem Ihr Konto deaktiviert wird. Informationen zum Deaktivieren von Benutzern finden Sie unter <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md#schedule-users-for-deactivation" class="MCXref xref">Planen von Benutzern für die Deaktivierung</a> in <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">Deaktivieren oder Reaktivieren eines Benutzers</a>. </p><p>Sie können die Deaktivierungsfelder Ihres Kontos bearbeiten, wenn Sie über eine [!UICONTROL Standard]- oder [!UICONTROL Plan]-Lizenz verfügen oder der Administrator [!DNL Workfront] sind. </p></td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL Primäre Rolle]</strong></td> 
   <td> <p>Dies ist die primäre Aufgabe, die Sie in Workfront erfüllen können. Jede Aufgabe und jedes Problem, die Ihnen zugewiesen sind, wird dieser Auftragsrolle standardmäßig ebenfalls zugewiesen. Arbeitsplatzrollen sind im Ressourcenmanagement von entscheidender Bedeutung. Weitere Informationen zu Auftragsrollen finden Sie unter <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Erstellen und Verwalten von Auftragsrollen</a>.</p> <p>Sie können dieses Feld nur aktualisieren, wenn Sie über eine [!UICONTROL Standard] - oder [!UICONTROL Plan] -Lizenz mit Administratorzugriff für Benutzer verfügen oder wenn Sie ein [!DNL Workfront] -Administrator sind. Weitere Informationen zum Einrichten von Benutzern mit Administratorzugriff finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md#configure-users-access-to-edit-users-using-a-custom-access-level" class="MCXref xref">Konfigurieren des Benutzerzugriffs zum Bearbeiten mithilfe einer benutzerdefinierten Zugriffsstufe</a> in <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Gewähren des Zugriffs für Benutzer</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>(Bedingt) Wenn Sie eine Primäre [!UICONTROL Rolle] ausgewählt haben, wird das Feld [!UICONTROL Prozentsatz der FTE-Verfügbarkeit] angezeigt.</strong></td> 
   <td>Geben Sie an, welcher Prozentsatz der geplanten Zeit dieser Auftragsrolle zugewiesen wird. Der Standardwert für [!UICONTROL Prozentsatz der FTE-Verfügbarkeit] für die Primäre Rolle beträgt 100 %.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL Sonstige Rollen]</strong> </td> 
   <td> <p>Sie können mehrere Auftragsrollen in [!DNL Workfront] haben. Arbeitsplatzrollen sind im Ressourcenmanagement von entscheidender Bedeutung. Weitere Informationen zu Auftragsrollen finden Sie unter <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Erstellen und Verwalten von Auftragsrollen</a>.</p> <p>Sie können dieses Feld nur aktualisieren, wenn Sie über eine [!UICONTROL Standard] - oder [!UICONTROL Plan] -Lizenz mit Administratorzugriff für Benutzer verfügen oder wenn Sie ein [!DNL Workfront] -Administrator sind. Weitere Informationen zum Einrichten von Benutzern mit Administratorzugriff finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md#access-to-edit" class="MCXref xref">Konfigurieren des Benutzerzugriffs zum Bearbeiten mithilfe einer benutzerdefinierten Zugriffsstufe</a> in <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Gewähren des Zugriffs für Benutzer</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>(Bedingt) Wenn Sie eine oder mehrere andere Rollen ausgewählt haben, wird für jede Rolle das Feld [!UICONTROL Prozentsatz der FTE-Verfügbarkeit] angezeigt.</strong></td> 
   <td> <p>Geben Sie an, welcher Prozentsatz der geplanten Zeit den einzelnen Auftragsrollen zugewiesen wird. Der Standardwert für [!UICONTROL Prozentsatz der FTE-Verfügbarkeit] für [!UICONTROL Sonstige Rollen] beträgt 0 %.</p> <p> <img src="assets/user-settings-roles-and-dte-boxes-rp-story--1--350x224.png" alt="user_settings_roles_and_dte_boxes_rp_story__1_.png" style="width: 350;height: 224;"> </p> <p>Hinweis:  
     <ul> 
      <li>Wenn [!UICONTROL Sonstige Rollen] eine FTE-Verfügbarkeit von 0 % haben, werden sie nicht im [!UICONTROL Resource Planer] angezeigt, es sei denn, die Benutzer sind Aufgaben in diesen Rollen zugewiesen.</li> 
      <li> <p>Die Summe aller <strong>[!UICONTROL Prozentsätze der FTE-Verfügbarkeit]</strong> für alle Rollen muss 100 % betragen. Jeder [!UICONTROL Prozentsatz der FTE-Verfügbarkeit] berechnet die [!UICONTROL Verfügbaren Stunden] für jede Rolle pro Benutzer im [!UICONTROL Resource Planer]. </p> <p>Die [!UICONTROL Verfügbare Stunden] für jede Rolle pro Benutzer hängt von der für den Benutzer verfügbaren Zeit ab. Die verfügbare Zeit für den Benutzer wird von [!DNL Workfront] abhängig von der Methode berechnet, die vom [!DNL Workfront] -Administrator zur Berechnung der FTE in den [!UICONTROL Resource Management Preferences] ausgewählt wurde. Weitere Informationen zur Berechnung der Verfügbarkeit für den Benutzer finden Sie unter <a href="../../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">Übersicht über die Berechnung der Stunden und der FTE für Benutzer und Rollen im Resource Planer</a>. Weitere Informationen zum Konfigurieren der Voreinstellungen für die Ressourcenverwaltung finden Sie unter <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md" class="MCXref xref">Voreinstellungen für die Ressourcenverwaltung konfigurieren</a>.</p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Zeitplan</strong></td> 
   <td> <p>Dieses Feld kann nur von [!DNL Workfront] Administratoren oder Benutzern mit einer [!UICONTROL Standard]- oder [!UICONTROL Plan]-Lizenz aktualisiert werden, die auch Administratorzugriff für Timesheets und Stunden haben. Weitere Informationen zum administrativen Zugriff für Timesheets und Stunden finden Sie im Abschnitt "Timesheets und Stunden"in <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Gewähren von Benutzern administrativen Zugriff auf bestimmte Bereiche</a>.</p> <p>Wählen Sie aus dem Dropdown-Menü das richtige Zeitblatt für Sie aus. Dadurch wird sichergestellt, dass Ihre Timesheets gemäß den Spezifikationen Ihres [!DNL Workfront] -Administrators automatisch generiert werden. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL Standardstundentyp]</strong> </td> 
   <td>Wählen Sie den Standardstundentyp aus. Dies ist der Stundentyp, den das System standardmäßig bei jeder Anmeldung in Workfront verwendet.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL Verfügbare Stundentypen]</strong> </td> 
   <td>Wählen Sie die Stundentypen aus, die bei der Protokollierung der Zeit ausgewählt werden sollen. Die Stundentypen in diesem Dropdown-Menü werden von Ihrem [!DNL Workfront] -Administrator zur Verfügung gestellt.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL Resource Pool]</strong> </td> 
   <td>Wählen Sie einen Ressourcen-Pool aus, zu dem Sie gehören. Dieses Feld dient nur zu Berichts- und Informationszwecken. Die Planung und Planung von Ressourcen ist davon nicht betroffen.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL FTE]</strong> </td> 
   <td> <p>Die hier angegebene Zahl wird berücksichtigt, um Ihre Verfügbarkeit basierend auf dem Standardzeitplan nur zu berechnen, wenn die [!UICONTROL Voreinstellungen für die Ressourcenverwaltung] auf Systemebene auf <strong>[!UICONTROL Standardzeitplan]</strong> gesetzt sind.</p> <p>Wenn der FTE-Wert beispielsweise 0,5 beträgt und der [!UICONTROL Standardzeitplan] 40 Stunden beträgt, können Sie 20 Stunden pro Woche arbeiten.</p> <p>Wenn die [!UICONTROL Voreinstellungen für die Ressourcenverwaltung] auf Systemebene auf "<strong>[!UICONTROL Der Benutzerplan]</strong>"festgelegt sind, wird der hier angegebene Wert ignoriert und Sie können gemäß dem Zeitplan arbeiten. In diesem Fall wird Ihre FTE für den [!UICONTROL Resource Planer] anhand der folgenden Formel berechnet: </p> <p><code style="font-style: normal;">[!UICONTROL User Available FTE] = [!UICONTROL Hours from the Schedule of the User/ Default Schedule Hours]</code> </p> <p>Weitere Informationen zur Berechnung der FTE für Benutzer finden Sie unter <a href="../../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">Übersicht über die Berechnung der Stunden und der FTE für Benutzer und Rollen im Resource Planer</a>.</p> <p>Weitere Informationen zum Erstellen von Zeitplänen in [!DNL Workfront] finden Sie unter <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Erstellen eines Zeitplans</a>.</p> <p>Weitere Informationen zum Konfigurieren der Voreinstellungen für die Ressourcenverwaltung finden Sie unter <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md" class="MCXref xref">Voreinstellungen für die Ressourcenverwaltung konfigurieren</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL Kosten pro Stunde]</strong> </td> 
   <td>Geben Sie die Kosten pro Stunde für Ihren Benutzer an. Weitere Informationen zu Tracking-Kosten in [!DNL Workfront] finden Sie unter <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Tracking-Kosten</a>. Sie können diese Informationen nur aktualisieren, wenn Sie über Zugriff auf Finanzdaten aus Ihrer Zugriffsebene verfügen oder wenn Sie ein [!DNL Workfront] -Administrator sind. Weitere Informationen zum finanziellen Zugriff finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md" class="MCXref xref">Zugriff auf Finanzdaten gewähren</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL Abrechnung pro Stunde]</strong> </td> 
   <td>Geben Sie den Betrag der Abrechnung pro Stunde für Ihren Benutzer an. Weitere Informationen zum Tracking der Rechnungsstellung und des Umsatzes finden Sie unter <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">Übersicht über Rechnungsstellung und Umsatz</a>. Sie können diese Informationen nur aktualisieren, wenn Sie über Zugriff auf Finanzdaten aus Ihrer Zugriffsebene verfügen oder wenn Sie ein [!DNL Workfront] -Administrator sind. Weitere Informationen zum finanziellen Zugriff finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md" class="MCXref xref">Zugriff auf Finanzdaten gewähren</a>.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Benutzerdefinierte Formulare]

Sie können ein benutzerdefiniertes Formular mit Ihrem Benutzerprofil verknüpfen. Auf diese Weise können Sie zusätzliche Informationen für Ihren Benutzer speichern, die sonst nicht in den oben beschriebenen nativen [!DNL Workfront]-Feldern gespeichert werden können.

Sie müssen über einen der folgenden Zugriff oder eine der folgenden Berechtigungen verfügen, um ein benutzerdefiniertes Formular an Ihr Benutzerprofil anhängen zu können:

* Sie sind ein [!DNL Workfront] -Administrator.
* Sie sind ein Lizenzbenutzer vom Typ [!UICONTROL Standard] oder [!UICONTROL Plan] und das benutzerdefinierte Formular des Benutzers wird für eine Ihrer Gruppen freigegeben.

Alle Benutzer können benutzerdefinierte Formulare sehen, die mit ihren Profilen verknüpft wurden.

Ihr [!DNL Workfront] -Administrator muss benutzerdefinierte Formulare für das Benutzerobjekt konfigurieren, damit Sie ein benutzerdefiniertes Formular an Ihr Benutzerprofil anhängen können. Weitere Informationen zum Erstellen benutzerdefinierter Formulare finden Sie unter [Erstellen eines benutzerdefinierten Formulars](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

### [!UICONTROL Kommentar]

Sie können einen Kommentar zu Ihrem Benutzerprofil aufzeichnen, der auf der Registerkarte [!UICONTROL Aktualisierungen] des Profils gespeichert ist.

Sie können auf das Symbol [!UICONTROL Personen] klicken, um weitere Personen in die Aktualisierung aufzunehmen.

Sie können auf das Symbol [!UICONTROL lock] klicken, um diese Aktualisierung für Benutzer privat zu machen, die sich im selben Unternehmen wie Sie befinden.
