---
title: Voreinstellungen eines Benutzers zurücksetzen
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: Als Adobe Workfront-Administrator können Sie die Benutzervoreinstellungen für alle Benutzer im Workfront-System zurücksetzen oder entfernen. Einzelne Benutzer können auch ihre eigenen Benutzervoreinstellungen zurücksetzen.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: abe026d0-3584-49f3-a6db-ef88b3aab186
source-git-commit: e20934501c2117455ca7950834d868f78576dee7
workflow-type: tm+mt
source-wordcount: '358'
ht-degree: 2%

---

# Voreinstellungen eines Benutzers zurücksetzen

Als Adobe Workfront-Administrator können Sie die Benutzervoreinstellungen für alle Benutzer im Workfront-System zurücksetzen oder entfernen.

Einzelne Benutzer können auch ihre eigenen Benutzervoreinstellungen zurücksetzen.

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

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
   <td> <p>Sie müssen Workfront-Administrator sein.</p> <p><b>NOTE</b>: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Über betroffene Einstellungen

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
   <td> <p>Auf den Systemstandard zurückgesetzt</p> <p>E-Mail-Benachrichtigungen werden wieder auf die Systemstandardwerte zurückgesetzt</p> </td> 
  </tr> 
  <tr> 
   <td>Benutzerdefinierte benutzerdefinierte Registerkarten</td> 
   <td>Entfernt</td> 
  </tr> 
  <tr> 
   <td>Benutzerdefinierte globale Navigationsoptionen</td> 
   <td>Setzen Sie die Layoutvorlage wieder auf die Definition oder den Systemstandard zurück, wenn keine Layoutvorlage zugewiesen ist.</td> 
  </tr> 
 </tbody> 
</table>

## Benutzereinstellungen zurücksetzen

1. Klicken Sie auf **Hauptmenü** icon ![](assets/main-menu-icon.png) Klicken Sie oben rechts in Adobe Workfront auf **Einrichtung** ![](assets/gear-icon-settings.png).

1. Auswählen **Anmelden als**.
1. Beginnen Sie mit der Eingabe des Namens des Benutzers, dessen Voreinstellungen Sie zurücksetzen möchten, und klicken Sie dann auf den Namen, wenn er in der Dropdown-Liste angezeigt wird.
1. Auswählen  **Anmelden**.
1. Fügen Sie im Feld URL oben im Webbrowser `/resetUser` after `workfront.com`.

   >[!NOTE]
   >
   >Dabei wird zwischen Groß- und Kleinschreibung unterschieden. Die U muss großgeschrieben werden, die übrigen Zeichen müssen in Kleinbuchstaben geschrieben werden. Beispiel:
   >
   >
   ```
   >https://company_domain.my.workfront.com/resetUser
   >```

1. Presse **Eingabe**.
1. Um alle Benutzereinstellungen zurückzusetzen, wählen Sie **Zurücksetzen**.

   Oder

   Um nur benutzerdefinierte Registerkarten zurückzusetzen, wählen Sie **Zurücksetzen von Registerkarten**.
