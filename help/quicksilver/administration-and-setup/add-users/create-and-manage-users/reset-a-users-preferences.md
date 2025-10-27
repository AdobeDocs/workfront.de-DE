---
title: Zurücksetzen der Benutzereinstellungen
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: Als Adobe Workfront-Administrator können Sie die Benutzereinstellungen für beliebige Benutzende im Workfront-System zurücksetzen oder entfernen. Einzelne Benutzer können auch ihre eigenen Benutzereinstellungen zurücksetzen.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: abe026d0-3584-49f3-a6db-ef88b3aab186
source-git-commit: 5706ebd11985b9e67c93686918f8f0327adabdf1
workflow-type: tm+mt
source-wordcount: '397'
ht-degree: 3%

---

# Zurücksetzen der Benutzereinstellungen

<!-- Audited: 12/2023 -->

<span class="preview">Die hervorgehobenen Informationen auf dieser Seite beziehen sich auf Funktionen, die noch nicht allgemein verfügbar sind. Sie ist nur in der Sandbox-Vorschau -Umgebung verfügbar und wird in einem schrittweisen Rollout in die Produktion veröffentlicht.</span>

Als Adobe Workfront-Administrator können Sie die Benutzereinstellungen für beliebige Benutzende im Workfront-System zurücksetzen oder entfernen.

Einzelne Benutzer können auch ihre eigenen Benutzereinstellungen zurücksetzen.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront-Paket</td> 
   <td><p>Beliebig</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront-Lizenz</td> 
   <td><p>Standard</p>
       <p>Plan</p></td>
  </tr> 
  <tr> 
   <td>Konfigurationen der Zugriffsebene</td> 
   <td>Systemadministrator</td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Über betroffene Einstellungen

Wenn Sie die Benutzereinstellungen zurücksetzen, werden einige Einstellungen auf den Systemstandard zurückgesetzt und andere gelöscht oder entfernt:

<!--
<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Preference</strong> </th> 
   <th><strong>Status after the reset</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Views</td> 
   <td> <p> Reverted to the system default</p> <p>Existing views are not deleted. You can select them again.</p> </td> 
  </tr> 
  <tr> 
   <td>Filters</td> 
   <td> <p>Reverted to the system default</p> <p>Existing filters are not deleted. You can select them again.</p> </td> 
  </tr> 
  <tr> 
   <td>Groupings</td> 
   <td> <p>Reverted to the system default</p> <p>Existing groupings are not deleted. You can select them again.</p> </td> 
  </tr> 
  <tr> 
   <td>Recent Items list</td> 
   <td>Cleared</td> 
  </tr> 
  <tr> 
   <td>Favorites list</td> 
   <td>Unaffected</td> 
  </tr> 
  <tr> 
   <td>User Preferences</td> 
   <td> <p>Reverted to the system default</p> <p>Email notifications revert to the system defaults. The default notifications are listed in <a href="/help/quicksilver/administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md">Event notifications available in Adobe Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>User-Defined Custom Tabs</td> 
   <td>Removed</td> 
  </tr> 
  <tr> 
   <td>User-Defined Global Navigation Options</td> 
   <td>Set back to layout template definition, or system default if no layout template is assigned.</td> 
  </tr> 
 </tbody> 
</table>
-->

<!--Display this table and hide the HTML table above, when the unshim is released.-->

<div class="preview">

| Voreinstellung | Status nach dem Zurücksetzen |
| --- | --- |
| Ansichten  | Auf Systemstandard zurückgesetzt <p>Vorhandene Ansichten werden nicht gelöscht. Sie können sie erneut auswählen.</p> |
| Filter | Auf Systemstandard zurückgesetzt <p>Vorhandene Filter werden nicht gelöscht. Sie können sie erneut auswählen.</p> |
| Gruppierungen | Auf Systemstandard zurückgesetzt <p>Vorhandene Gruppierungen werden nicht gelöscht. Sie können sie erneut auswählen.</p> |
| Liste der letzten Elemente | Gelöscht |
| Favoritenliste | unberührt |
| Benutzervoreinstellungen | Auf Systemstandard zurückgesetzt <p>E-Mail-Benachrichtigungen werden auf die Systemstandardwerte zurückgesetzt. Die Standardbenachrichtigungen werden unter [Ereignisbenachrichtigungen in Adobe Workfront verfügbar](/help/quicksilver/administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md) aufgeführt.</p> |

</div>

## Benutzereinstellungen zurücksetzen

{{step-1-to-setup}}

1. Wählen Sie **Anmelden als** aus.
1. Geben Sie den Namen des Benutzers ein, dessen Voreinstellungen Sie zurücksetzen möchten, und klicken Sie auf den Namen, wenn er in der Dropdown-Liste angezeigt wird.
1. Wählen Sie **Anmelden** aus.
1. Wenn Ihr Unternehmen nicht zum einheitlichen Adobe-Erlebnis hinzugefügt wurde, führen Sie die folgenden Schritte aus:

   * Fügen Sie im URL-Feld oben in Ihrem Webbrowser nach der `/resetUser` `workfront.com` hinzu.

     >[!NOTE]
     >
     >Hierbei wird zwischen Groß- und Kleinschreibung unterschieden. Das U muss großgeschrieben werden und die restlichen Zeichen müssen in Kleinbuchstaben geschrieben werden. Beispiel:
     >
     >`https://company_domain.my.workfront.com/resetUser`

1. Wenn Ihre Organisation in das einheitliche Adobe-Erlebnis integriert wurde, führen Sie diesen Schritt aus:

   * Fügen Sie im URL-Feld oben in Ihrem Webbrowser nach der `/resetUser` `workfront` hinzu.

     >[!NOTE]
     >
     >Hierbei wird zwischen Groß- und Kleinschreibung unterschieden. Das U muss großgeschrieben werden und die restlichen Zeichen müssen in Kleinbuchstaben geschrieben werden. Beispiel:
     >
     >`https://experience.adobe.com/#/@company/so:(domain)-(environment)/workfront/resetUser`

1. Drücken Sie **ENTER**.

1. <span class="preview">Um alle Benutzereinstellungen zurückzusetzen, klicken Sie auf **Zurücksetzen**.</span>

   <span class="preview">ODER</span>

   <span class="preview">Um die linke Navigation des Benutzers auf die ursprüngliche Layout-Vorlagenkonfiguration zurückzusetzen, klicken Sie auf **Linke Navigation zurücksetzen**.</span>
