---
title: Zurücksetzen der Benutzereinstellungen
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: Als Adobe Workfront-Administrator können Sie die Benutzereinstellungen für beliebige Benutzende im Workfront-System zurücksetzen oder entfernen. Einzelne Benutzer können auch ihre eigenen Benutzereinstellungen zurücksetzen.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: abe026d0-3584-49f3-a6db-ef88b3aab186
source-git-commit: 0bc2817255b8879de377c3916bb36be760f28f4c
workflow-type: tm+mt
source-wordcount: '404'
ht-degree: 2%

---

# Zurücksetzen der Benutzereinstellungen

<!-- Audited: 12/2023 -->

Als Adobe Workfront-Administrator können Sie die Benutzereinstellungen für beliebige Benutzende im Workfront-System zurücksetzen oder entfernen.

Einzelne Benutzer können auch ihre eigenen Benutzereinstellungen zurücksetzen.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

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
   <td><p>Neu: Standard</p>
       <p>Oder</p>
       <p>Aktuell: Plan</p></td>
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td>[!UICONTROL Systemadministrator]</td>
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Über betroffene Einstellungen

Wenn Sie die Benutzereinstellungen zurücksetzen, werden einige Einstellungen auf den Systemstandard zurückgesetzt und andere gelöscht oder entfernt:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Voreinstellung</strong> </th> 
   <th><strong>Status nach dem Zurücksetzen</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Ansichten</td> 
   <td> <p> Auf Systemstandard zurückgesetzt</p> <p>Vorhandene Ansichten werden nicht gelöscht. Sie können sie erneut auswählen.</p> </td> 
  </tr> 
  <tr> 
   <td>Filter</td> 
   <td> <p>Auf Systemstandard zurückgesetzt</p> <p>Vorhandene Filter werden nicht gelöscht. Sie können sie erneut auswählen.</p> </td> 
  </tr> 
  <tr> 
   <td>Gruppierungen</td> 
   <td> <p>Auf Systemstandard zurückgesetzt</p> <p>Vorhandene Gruppierungen werden nicht gelöscht. Sie können sie erneut auswählen.</p> </td> 
  </tr> 
  <tr> 
   <td>Liste der letzten Elemente</td> 
   <td>Gelöscht</td> 
  </tr> 
  <tr> 
   <td>Favoritenliste</td> 
   <td>unberührt</td> 
  </tr> 
  <tr> 
   <td>Benutzervoreinstellungen</td> 
   <td> <p>Auf Systemstandard zurückgesetzt</p> <p>E-Mail-Benachrichtigungen werden auf die Systemstandardwerte zurückgesetzt. Die Standardbenachrichtigungen werden unter <a href="/help/quicksilver/administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md">Ereignisbenachrichtigungen in Adobe Workfront verfügbar</a> aufgeführt.</p> </td> 
  </tr> 
  <tr> 
   <td>Benutzerdefinierte Registerkarten</td> 
   <td>entfernt</td> 
  </tr> 
  <tr> 
   <td>Benutzerdefinierte globale Navigationsoptionen</td> 
   <td>Setzen Sie zurück auf Layout-Vorlagendefinition oder auf Systemstandard , wenn keine Layout-Vorlage zugewiesen ist.</td> 
  </tr> 
 </tbody> 
</table>

## Benutzereinstellungen zurücksetzen

{{step-1-to-setup}}

1. Wählen Sie **Anmelden als** aus.
1. Geben Sie den Namen des Benutzers ein, dessen Voreinstellungen Sie zurücksetzen möchten, und klicken Sie auf den Namen, wenn er in der Dropdown-Liste angezeigt wird.
1. Wählen Sie **Anmelden** aus.
1. Wenn Ihr Unternehmen nicht zum einheitlichen Adobe-Erlebnis hinzugefügt wurde, führen Sie diesen Schritt aus:

   * Fügen Sie im URL-Feld oben in Ihrem Webbrowser nach der `workfront.com` `/resetUser` hinzu.

     >[!NOTE]
     >
     >Hierbei wird zwischen Groß- und Kleinschreibung unterschieden. Das U muss großgeschrieben werden und die restlichen Zeichen müssen in Kleinbuchstaben geschrieben werden. Beispiel:
     >
     >`https://company_domain.my.workfront.com/resetUser`

1. Wenn Ihr Unternehmen zum einheitlichen Adobe-Erlebnis hinzugefügt wurde, führen Sie diesen Schritt aus:

   * Fügen Sie im URL-Feld oben in Ihrem Webbrowser nach der `workfront` `/resetUser` hinzu.

     >[!NOTE]
     >
     >Hierbei wird zwischen Groß- und Kleinschreibung unterschieden. Das U muss großgeschrieben werden und die restlichen Zeichen müssen in Kleinbuchstaben geschrieben werden. Beispiel:
     >
     >`https://experience.adobe.com/#/@company/so:(domain)-(environment)/workfront/resetUser`

1. Drücken Sie **ENTER**.
1. Um alle Benutzereinstellungen zurückzusetzen, klicken Sie auf **Zurücksetzen**.

   Oder

   Um nur benutzerdefinierte Registerkarten zurückzusetzen, wählen Sie **Registerkarten zurücksetzen**.
