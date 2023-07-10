---
title: Anmelden als anderer Benutzer
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: Als Adobe Workfront-Administrator müssen Sie manchmal im Namen eines anderen Benutzers auf Workfront zugreifen.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 2f8dd132-1086-4980-9b56-993a68231e96
source-git-commit: 82f42d81970c7572f43519423ec3a8c0889aaff4
workflow-type: tm+mt
source-wordcount: '895'
ht-degree: 0%

---

# Anmelden als anderer Benutzer


<span class="preview">Die hervorgehobenen Informationen auf dieser Seite beziehen sich auf Funktionen, die noch nicht allgemein verfügbar sind. Sie ist nur für alle Benutzer in der Vorschauumgebung verfügbar.</span>
<!--
**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. Also linked to other articles: Creating and Managing Groups, etc.</p>
-->

>[!IMPORTANT]
>
>Das auf dieser Seite beschriebene Verfahren gilt nur für Organisationen, die noch nicht in der Adobe Admin Console integriert wurden. Wenn Ihr Unternehmen in der Adobe Admin Console integriert wurde, ist diese Aktion nicht verfügbar.
>
>Eine Liste der Verfahren, die je nachdem, ob Ihr Unternehmen in die Adobe Admin Console integriert wurde, unterschiedlich sind, finden Sie unter [Plattformbasierte Verwaltungsunterschiede (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

Als Adobe Workfront-Administrator müssen Sie manchmal im Namen eines anderen Benutzers auf Workfront zugreifen.

Als Gruppenadministrator müssen Sie möglicherweise im Namen eines Benutzers auf Workfront zugreifen, der Mitglied einer von Ihnen verwalteten Gruppe ist.

Wenn beispielsweise eine Aufgabe erst ausgeführt werden kann, wenn ein Benutzer im Urlaub eine bestimmte Aktion durchführt, können Sie sich als dieser Benutzer anmelden und stattdessen die Aktion durchführen.

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
>Da eine Dokumentintegration eine Verbindung zu privaten persönlichen Dateien herstellen kann, können Administratoren nicht auf Dokumentintegrationen zugreifen, während sie als ein anderer Benutzer angemeldet sind.
>
>Weitere Informationen zu Dokumentintegrationen finden Sie unter [Dokumentintegrationen konfigurieren](../../../administration-and-setup/configure-integrations/configure-document-integrations.md)

## Zugriffsanforderungen

Sie müssen über Folgendes verfügen, um die Schritte in diesem Artikel durchzuführen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Abo</td> 
   <td>Beliebig</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Mit der Zugriffsebene des Systemadministrators können Sie sich wie jeder andere anmelden. Weitere Informationen zu dieser Zugriffsebene finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Gewähren eines vollen Administratorzugriffs</a>. </p> <p>Mit einer Planer-Zugriffsebene können Sie sich als Benutzer mit einer niedrigeren Lizenzstufe anmelden, wenn die <b>Benutzer</b> -Einstellung in der Zugriffsebene ist so konfiguriert, dass <b>Bearbeiten</b> Zugriff, mit <b>Erstellen</b> und mindestens eines der beiden <b>Benutzer-Admin</b> Optionen aktiviert unter <b>Einstellungen anpassen</b> <img src="assets/gear-icon-in-access-levels.png">. </p> 
   <p><b>NOTE</b>: Wenn Benutzer <b>Admin (Gruppenbenutzer)</b> aktiviert ist, müssen Sie ein Gruppenadministrator einer Gruppe sein, in der der Benutzer Mitglied ist.</p> 
   <p>Weitere Informationen zum <b>Benutzer</b> auf einer Zugriffsebene festzulegen, siehe <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Benutzern Zugriff gewähren</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Anmelden und Aktionen als anderer Benutzer ausführen

1. Melden Sie sich bei Workfront als Workfront-Administrator oder Gruppenadministrator an.

   >[!NOTE]
   >
   >* Als Gruppenadministrator können Sie sich nur als Benutzer in den von Ihnen verwalteten Gruppen anmelden. Außerdem muss die Berechtigung &quot;Benutzeradministrator (Gruppenbenutzer)&quot;in Ihrer Zugriffsebene aktiviert sein:
   >   
   >  ![](assets/group-admin-user.png)
   >   
   >  Diese Einstellung ist standardmäßig deaktiviert. Weitere Informationen finden Sie unter [Benutzerdefinierte Zugriffsebenen erstellen oder ändern](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
   >   
   >* Sie können das Kennwort eines Workfront-Administrators nicht zurücksetzen.

1. Klicken Sie auf **Hauptmenü** icon ![](assets/main-menu-icon.png) Klicken Sie oben rechts in Adobe Workfront auf **Einrichtung** ![](assets/gear-icon-settings.png).

1. Klicken Sie im linken Bereich auf **Anmelden als**.

1. Im **Benutzer** auf der **Anmelden als** eingeben, den Namen des Benutzers eingeben und auf den Namen klicken, wenn er in der Dropdown-Liste angezeigt wird.

   Der Benutzer muss über eine in Workfront definierte Zugriffsstufe verfügen. Sie können sich nicht beim Workfront-System als Benutzer anmelden, der nicht über die entsprechenden Anmelderechte verfügt.

   >[!NOTE]
   >
   >Gruppenadministratoren können sich nur als Benutzer anmelden, die Mitglieder der von ihnen verwalteten Gruppen sind. Sie können sich nicht als Workfront-Administrator anmelden.

1. Klicken **Melden Sie sich an.**

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Might come in a future story:</p>
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

   Wenn Sie als ein anderer Benutzer angemeldet sind, wird oben auf dem Bildschirm eine Benachrichtigung angezeigt, um dies anzuzeigen.

1. Nachdem Sie die erforderlichen Aktionen als Benutzer ausgeführt haben, klicken Sie auf **Abmelden.**

## Aktivitäten zur Verfolgung und Prüfung, während ein Administrator als ein anderer Benutzer angemeldet ist

Workfront bietet Mechanismen zur Verfolgung und Prüfung von Aktivitäten, die während der Anmeldung des Administrators als anderer Benutzer stattfinden.

Wenn Sie sich als ein anderer Benutzer anmelden, wird das letzte Anmeldedatum für diesen Benutzer bis zu dem Datum geändert, an dem sich der System- oder Gruppenadministrator als dieser Benutzer anmeldet.

* [Anzeigen von Indikatoren zu Artikeln](#view-indicators-on-items)
* [Prüfungsinformationen anzeigen](#view-audit-information)

### Anzeigen von Indikatoren zu Artikeln {#view-indicators-on-items}

Wenn Sie sich bei Workfront als ein anderer Benutzer anmelden und eine Aktion ausführen, zeigt Workfront eindeutig an, dass jede Aktion, die Sie ausführen, von Ihnen im Namen des Benutzers ausgeführt wird, als der Sie angemeldet sind.

Wenn Sie beispielsweise einen Kommentar zu einem Element abgeben, während Sie als ein anderer Benutzer angemeldet sind, zeigt eine Anweisung an, dass der Kommentar von Ihnen im Namen des Benutzers abgegeben wurde.

>[!NOTE]
>
><span class="preview">Bei Verwendung des neuen Kommentar-Erlebnisses wird der Kommentar als Benutzer hinzugefügt, der sich als ein anderer Benutzer angemeldet hat. Es gibt keinen Hinweis darauf, dass er einen Kommentar für den Namen einer anderen Person hinzufügt.
>
>Wenn sich beispielsweise ein Workfront-Administrator als ein anderer Benutzer anmeldet, ist der mit dem Kommentar verknüpfte Benutzer der Workfront-Administrator. Weitere Informationen finden Sie unter [Neues Kommentierungserlebnis](../../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md). </span>


### Prüfungsinformationen anzeigen {#view-audit-information}

1. Melden Sie sich bei Workfront als Workfront-Administrator oder Gruppenadministrator an.
1. Klicken Sie auf **Hauptmenü** icon ![](assets/main-menu-icon.png) Klicken Sie oben rechts in Adobe Workfront auf **Einrichtung** ![](assets/gear-icon-settings.png).

1. Klicken **Anmelden als** Klicken Sie dann auf **Zugriffsprotokoll** Registerkarte.

   Jedes Mal, wenn sich ein System- oder Gruppenadministrator bei Workfront als einem anderen Benutzer anmeldet, wird das Ereignis im Audit-Protokoll protokolliert. Darüber hinaus werden alle geprüfbaren Aktionen, die ausgeführt werden, während der Administrator als ein anderer Benutzer angemeldet ist, im Audit-Protokoll protokolliert.

1. (Optional) Sie können die im Audit-Protokoll angezeigten Ergebnisse wie folgt filtern:

   * Von Benutzer, der sich angemeldet hat
   * Von Benutzer, der angemeldet ist als
   * Nach Datum
