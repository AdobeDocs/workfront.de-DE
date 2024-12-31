---
title: Melden Sie sich als anderer Benutzer an
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: Als Adobe Workfront-Administrator benötigen Sie manchmal Zugriff auf Workfront im Namen eines anderen Benutzers.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 2f8dd132-1086-4980-9b56-993a68231e96
source-git-commit: dc64fef83c2b1e9f8bf9438017155bd47b83ab23
workflow-type: tm+mt
source-wordcount: '738'
ht-degree: 0%

---

# Anmelden als eine andere Benutzerin bzw. ein anderer Benutzer

<!--Audited: April, 2024-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available for all users only in the Preview environment.</span> -->

<!--
**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. Also linked to other articles: Creating and Managing Groups, etc.</p>
-->

Als Adobe Workfront-Administrator benötigen Sie manchmal Zugriff auf Workfront im Namen eines anderen Benutzers.

Oder Sie als Gruppenadministrator müssen möglicherweise auf Workfront im Namen einer Benutzerin oder eines Benutzers zugreifen, die bzw. der Mitglied einer von Ihnen verwalteten Gruppe ist.

Wenn eine Aufgabe beispielsweise erst fortgesetzt werden kann, nachdem ein Benutzer im Urlaub eine bestimmte Aktion ausgeführt hat, können Sie sich als dieser Benutzer anmelden und stattdessen die Aktion ausführen.

<!--
<note type="note">
Some users, such as executives, need to be able to control which administrators can log in to their accounts, and for how long. Working with your organization, Workfront configures settings that allow this control for these users. When a Workfront administrator or group administrator (associated with one of the user's groups) tries to log in as one of these users, an on-screen message prompts the administrator to contact the user for access. From the user profile area, the user can then grant access to the administrator and specify an expiration time for it. For more information on how the user does this, see
<a href="../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md#access" class="MCXref xref">Access</a> in
<a href="../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md" class="MCXref xref">Configure My Settings</a>.
<span class="PinkDraftNote">[Add a note about this being only for the Enterprise package if they decide to do it that way]</span>
</note>
-->

>[!NOTE]
>
>Da eine Dokumentenintegration möglicherweise eine Verbindung zu privaten persönlichen Dateien herstellt, können Admins nicht auf Dokumentenintegrationen zugreifen, während sie als ein anderer Benutzer angemeldet sind.
>
>Weitere Informationen zu Dokumentintegrationen finden Sie unter [Konfigurieren von Dokumentintegrationen](../../../administration-and-setup/configure-integrations/configure-document-integrations.md)

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über Folgendes verfügen, um die Schritte in diesem Artikel auszuführen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan</td> 
   <td>Beliebig</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td> <p>Neu: Standard</p>
   <p>Oder</p>
   <p>Aktuell: Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Mit der Zugriffsebene „Systemadministrator“ können Sie sich wie jeder andere anmelden.</p> <p>Bei einer Standard- oder Planerzugriffsebene können Sie sich als Benutzer mit einer niedrigeren Lizenzstufe anmelden, wenn die Einstellung <b>Benutzer</b> auf der Zugriffsebene für den <b>Bearbeiten</b>-Zugriff konfiguriert ist, wobei <b>Erstellen</b> und mindestens eine der beiden <b>Benutzeradministratoroptionen</b> unter <b>Optimieren Sie Ihre Einstellungen</b> <img src="assets/gear-icon-in-access-levels.png"> aktiviert ist. </p> 
   <p><b>HINWEIS</b>: Wenn die Option <b>Benutzeradmin (Gruppenbenutzer)</b> aktiviert ist, müssen Sie Gruppenadministrator einer Gruppe sein, in der der Benutzer Mitglied ist.</p></td>
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Anmelden und Ausführen von Aktionen als anderer Benutzer

1. Melden Sie sich bei Workfront als Workfront-Administrator oder Gruppenadministrator an.

   >[!NOTE]
   >
   >* Wenn Sie Gruppenadministrator sind, können Sie sich nur als Benutzer in den von Ihnen verwalteten Gruppen anmelden. Außerdem muss in Ihrer Zugriffsebene die Berechtigung Benutzeradmin (Gruppenbenutzer) aktiviert sein:
   >   
   >  ![](assets/group-admin-user.png)
   >   
   >  Diese Einstellung ist standardmäßig deaktiviert. Weitere Informationen finden Sie unter [Erstellen oder Ändern benutzerdefinierter Zugriffsebenen](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
   >   
   >* Das Kennwort eines Workfront-Administrators kann nicht zurückgesetzt werden.

{{step-1-to-setup}}

1. Klicken Sie im linken Bedienfeld auf **Anmelden als**.

1. Beginnen Sie in das Feld **Benutzer** auf der Registerkarte **Anmelden als** mit der Eingabe des Benutzernamens und klicken Sie dann auf den Namen, wenn er in der Dropdown-Liste angezeigt wird.

   Für den Benutzer muss eine Zugriffsebene in Workfront definiert sein. Sie können sich nicht als ein Benutzer beim Workfront-System anmelden, der nicht berechtigt ist, sich anzumelden.

   >[!NOTE]
   >
   >Gruppenadministratoren können sich nur als Benutzer anmelden, die Mitglieder der von ihnen verwalteten Gruppen sind. Sie können sich nicht als Workfront-Admin anmelden.

1. Klicken Sie **Anmelden.**

   <!--
   <p> Might come in a future story:</p>
   -->

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">click an Access period and then click Request to ask the user for access to log as him or her for the specified period of time. Continue these steps after the user grants access. Specify somewhere here that this is only for the Enterprise package if they decide on that</p>
   -->

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Or </p>
   -->

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">If a prompt appears indicating that the user has restricted access to their account, contact the user to request access.</p>
   -->

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">The user can then can grant you "Log in as" access in their user profile. They can also specify an expiration date and time for the access period. </p>
   -->

   <!--
   This triggers an email to let you know that you have access to log in as the user, depending on how your event notifications are enabled. For more information, see <a href="../../../workfront-basics/using-notifications/event-notifications.md" class="MCXref xref">Event notifications</a>.
   </div>
   -->

   Wenn Sie als ein anderer Benutzer angemeldet sind, wird oben im Bildschirm eine Benachrichtigung angezeigt, die dies angibt.

1. Nachdem Sie als Benutzer die erforderlichen Aktionen ausgeführt haben, klicken Sie auf **Abmelden.**

## Tracking und Auditing von Aktivitäten, während ein Administrator als ein anderer Benutzer angemeldet ist

Workfront bietet Mechanismen zum Tracking und Auditing von Aktivitäten, die stattfinden, während Admins als andere Benutzende angemeldet sind.

Wenn Sie sich als ein anderer Benutzer anmelden, wird das letzte Anmeldedatum für diesen Benutzer auf das Datum geändert, an dem sich der System- oder Gruppenadministrator als dieser Benutzer anmeldet.

* [Anzeigen von Indikatoren zu Elementen](#view-indicators-on-items)
* [Audit-Informationen anzeigen](#view-audit-information)

### Anzeigen von Indikatoren zu Elementen {#view-indicators-on-items}

Wenn Sie sich als ein anderer Benutzer bei Workfront anmelden und eine Aktion ausführen, zeigt Workfront eindeutig an, dass alle Aktionen, die Sie durchführen, von Ihnen im Namen der Person durchgeführt werden, als die Sie angemeldet sind.

Wenn Sie beispielsweise einen Kommentar zu einem Element abgeben, während Sie als ein anderer Benutzer angemeldet sind, gibt eine -Anweisung an, dass der Kommentar von Ihnen im Namen der Benutzerin bzw. des Benutzers beim Anzeigen des Abschnitts Aktualisierungen eines Objekts abgegeben wurde.

### Audit-Informationen anzeigen {#view-audit-information}

1. Melden Sie sich bei Workfront als Workfront-Administrator oder Gruppenadministrator an.
1. Klicken Sie auf **Hauptmenü** Symbol ![](assets/main-menu-icon.png) oben rechts in Adobe Workfront und dann auf **Setup** ![](assets/gear-icon-settings.png).

1. Klicken Sie auf **Anmelden als** und anschließend auf die Registerkarte **Zugriffsprotokoll**.

   Jedes Mal, wenn sich ein System- oder Gruppenadministrator bzw. eine Systemadministratorin als ein anderer Benutzer bei Workfront anmeldet, wird das Ereignis im Audit-Protokoll protokolliert. Darüber hinaus werden alle überprüfbaren Aktionen, die stattfinden, während der Administrator als ein anderer Benutzer angemeldet ist, im Audit-Protokoll protokolliert.

1. (Optional) Sie können die im Audit-Protokoll angezeigten Ergebnisse wie folgt filtern:

   * Nach Benutzer, der sich angemeldet hat
   * Von Benutzer, der angemeldet ist als
   * Nach Datum
