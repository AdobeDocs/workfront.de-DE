---
title: Benutzereinstellungen zurücksetzen
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: Als Adobe Workfront-Administrator können Sie die Benutzervoreinstellungen für alle Benutzer im Workfront-System zurücksetzen oder entfernen. Einzelne Benutzer können auch ihre eigenen Benutzervoreinstellungen zurücksetzen.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: abe026d0-3584-49f3-a6db-ef88b3aab186
source-git-commit: a9d507bfcc0a602e71bcdd3142d63cc40175ebf4
workflow-type: tm+mt
source-wordcount: '407'
ht-degree: 2%

---

# Voreinstellungen eines Benutzers zurücksetzen

<!-- Audited: 12/2023 -->

Als Adobe Workfront-Administrator können Sie die Benutzervoreinstellungen für alle Benutzer im Workfront-System zurücksetzen oder entfernen.

Einzelne Benutzer können auch ihre eigenen Benutzervoreinstellungen zurücksetzen.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Abo</td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td><p>Neu: Standard</p>
       <p>oder</p>
       <p>Aktuell: Plan</p></td>
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Sie müssen Workfront-Administrator sein.</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Über die betroffenen Einstellungen

Wenn Sie die Benutzereinstellungen zurücksetzen, werden einige Voreinstellungen auf den Systemstandard zurückgesetzt und andere werden gelöscht oder entfernt:

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
   <td> <p> Auf den Systemstandard zurückgesetzt</p> <p>Vorhandene Ansichten werden nicht gelöscht. Sie können sie erneut auswählen.</p> </td> 
  </tr> 
  <tr> 
   <td>Filter</td> 
   <td> <p>Auf den Systemstandard zurückgesetzt</p> <p>Vorhandene Filter werden nicht gelöscht. Sie können sie erneut auswählen.</p> </td> 
  </tr> 
  <tr> 
   <td>Gruppierungen</td> 
   <td> <p>Auf den Systemstandard zurückgesetzt</p> <p>Bestehende Gruppierungen werden nicht gelöscht. Sie können sie erneut auswählen.</p> </td> 
  </tr> 
  <tr> 
   <td>Liste der letzten Elemente</td> 
   <td>Bereinigt</td> 
  </tr> 
  <tr> 
   <td>Favoritenliste</td> 
   <td>Nicht betroffen</td> 
  </tr> 
  <tr> 
   <td>Benutzereinstellungen</td> 
   <td> <p>Auf den Systemstandard zurückgesetzt</p> <p>E-Mail-Benachrichtigungen werden wieder auf die Systemstandardwerte zurückgesetzt. Die Standardbenachrichtigungen sind in <a href="/help/quicksilver/administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md">In Adobe Workfront</a> verfügbare Ereignisbenachrichtigungen aufgeführt.</p> </td> 
  </tr> 
  <tr> 
   <td>Benutzerdefinierte benutzerdefinierte Registerkarten</td> 
   <td>Entfernt</td> 
  </tr> 
  <tr> 
   <td>Benutzerdefinierte globale Navigationsoptionen</td> 
   <td>Setzen Sie die Layout-Vorlagendefinition zurück oder setzen Sie den Systemstandard, wenn keine Layoutvorlage zugewiesen ist.</td> 
  </tr> 
 </tbody> 
</table>

## Benutzereinstellungen zurücksetzen

{{step-1-to-setup}}

1. Wählen Sie **Anmelden als** aus.
1. Geben Sie den Namen des Benutzers ein, dessen Voreinstellungen Sie zurücksetzen möchten, und klicken Sie dann auf den Namen, wenn er in der Dropdown-Liste angezeigt wird.
1. Wählen Sie **Anmelden** aus.
1. Wenn Ihr Unternehmen nicht in das Adobe Unified Experience integriert wurde, führen Sie diesen Schritt aus:

   * Fügen Sie im Feld URL oben im Webbrowser `/resetUser` nach `workfront.com` hinzu.

     >[!NOTE]
     >
     >Dabei wird zwischen Groß- und Kleinschreibung unterschieden. Die U muss großgeschrieben werden, die übrigen Zeichen müssen in Kleinbuchstaben geschrieben werden. Beispiel:
     >
     >`https://company_domain.my.workfront.com/resetUser`

1. Wenn Ihr Unternehmen in das Adobe Unified Experience integriert wurde, führen Sie diesen Schritt aus:

   * Fügen Sie im Feld URL oben im Webbrowser den Wert `/resetUser` nach `workfront` hinzu.

     >[!NOTE]
     >
     >Dabei wird zwischen Groß- und Kleinschreibung unterschieden. Die U muss großgeschrieben werden, die übrigen Zeichen müssen in Kleinbuchstaben geschrieben werden. Beispiel:
     >
     >`https://experience.adobe.com/#/@company/so:(domain)-(environment)/workfront/resetUser`

1. Drücken Sie die Taste **Enter**.
1. Um alle Benutzereinstellungen zurückzusetzen, wählen Sie **Zurücksetzen** aus.

   Oder

   Um nur benutzerdefinierte Registerkarten zurückzusetzen, wählen Sie **Registerkarten zurücksetzen** aus.
