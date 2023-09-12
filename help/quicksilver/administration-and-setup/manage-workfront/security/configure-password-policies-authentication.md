---
user-type: administrator
product-area: system-administration;user-management;setup
navigation-topic: security
title: Kennwortrichtlinien für die Authentifizierung konfigurieren
description: Als Adobe Workfront-Administrator können Sie Optionen für Kennwortrichtlinien konfigurieren, um die Authentifizierungserfahrung auf Ihr Workfront-System anzupassen.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 7832986b-a5e8-4f14-8802-d3b8e32b14bc
source-git-commit: 970cc86b00dc1afe0473ac3a387e7ce47e4a2433
workflow-type: tm+mt
source-wordcount: '706'
ht-degree: 1%

---

# Kennwortrichtlinien für die Authentifizierung konfigurieren

{{important-admin-console-onboard}}

Als Adobe Workfront-Administrator können Sie Optionen für Kennwortrichtlinien konfigurieren, um die Authentifizierungserfahrung auf Ihr Workfront-System anzupassen.

Es wird empfohlen, die Authentifizierungseinstellungen während der Workfront-Implementierung zu konfigurieren und sie anschließend nur gelegentlich erneut aufzurufen.

Verbesserte Funktionen zur Kennwortverwaltung stehen in Kürze zur Verfügung oder stehen möglicherweise bereits für Ihre Organisation zur Verfügung. Verwenden Sie einen der folgenden Abschnitte, je nachdem, ob Ihr Unternehmen Zugriff auf das neue Authentifizierungs-Erlebnis hat.

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
   <td> <p>Sie müssen Workfront-Administrator sein.</p> <p><b>NOTE</b>: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsstufe festgelegt hat. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Authentifizierung konfigurieren (für alle Kunden verfügbar) {#configure-authentication-available-for-all-customers}

Authentifizierungsoptionen werden für alle Kunden angezeigt. Verbesserte Funktionen zur Kennwortverwaltung stehen in Kürze zur Verfügung oder stehen möglicherweise bereits für Ihre Organisation zur Verfügung, wie im Abschnitt beschrieben. [Erweiterte Authentifizierung konfigurieren)](#configure-enhanced-authentication-coming-soon) in diesem Artikel.

So konfigurieren Sie Authentifizierungsvoreinstellungen:

1. Klicken Sie auf **Hauptmenü** icon ![](assets/main-menu-icon.png) Klicken Sie oben rechts in Adobe Workfront auf **Einrichtung** ![](assets/gear-icon-settings.png).

1. Klicks **System** > **Authentifizierung**.

1. Wählen Sie eines der folgenden Felder aus, um die Authentifizierungseinstellungen für Ihr Unternehmen festzulegen:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Erzwingen, dass Benutzer jedes Mal ihr Kennwort zurücksetzen <em>&lt;value&gt;</em> Tage</td> 
      <td>Dadurch wird der Zeitrahmen für das Zurücksetzen des Workfront-Kennworts festgelegt. Standardmäßig ist diese Option deaktiviert. Wenn Sie sie aktivieren, können Sie zwischen 30, 60, 90, 120, 180 Tagen wählen. Der Standardwert ist 30 Tage.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Erlauben Sie Benutzern nicht, dasselbe Kennwort wie für die vorherigen festzulegen <em>&lt;value&gt;</em> passwords</td> 
      <td> <p>Dieses Feld untersagt Benutzern, Kennwörter für eine bestimmte Anzahl von Zurücksetzungen wiederzuverwenden. Standardmäßig ist dieses Feld deaktiviert. Wenn Sie sie aktivieren, können Sie diesen Wert auf 5, 10 oder 15 Zurücksetzungen setzen, bevor ein Kennwort wiederverwendet werden kann.</p> <p>Wenn diese Option aktiviert ist, können Benutzer ihre Kennwörter nicht mehr als einmal an einem bestimmten Tag zurücksetzen</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Wenn ein falsches Kennwort fünf Mal hintereinander eingegeben wird, sperren Sie das Konto für <em>&lt;value&gt;</em> Minuten: </td> 
      <td> <p>Wählen Sie aus, wie lange ein Benutzer fünf Mal hintereinander aus Workfront ausgesperrt wird, nachdem er ein falsches Kennwort eingegeben hat. Standardmäßig ist diese Option aktiviert und die Wartezeit beträgt 10 Minuten. Sie können Konten für 10 Minuten, 30 Minuten, 1 Stunde, 8 Stunden oder 24 Stunden sperren. </p> <p>Durch das manuelle Zurücksetzen des Kennworts für den Benutzer wird dieser standardmäßige Wartewert überschrieben. <br>Benutzer können ihre eigenen Kennwörter zurücksetzen, wenn sie über den Anmeldebildschirm gesperrt werden. Weitere Informationen dazu, wie sie ihr Kennwort zurücksetzen können, finden Sie unter <a href="../../../workfront-basics/manage-your-account-and-profile/managing-your-workfront-account/reset-your-password.md" class="MCXref xref">Passwort zurücksetzen</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Passwörter müssen mindestens enthalten <em>&lt;value&gt;</em> verschiedene Arten von Zeichen:</td> 
      <td> <p>Bestimmt, wie stark Passwörter für Benutzer sein müssen, indem Sie die Anzahl der verschiedenen Arten von Zeichen auswählen können, die in Ihren Passwörtern erforderlich sind.</p> <p>Ein erkennbares Wörterbuchwort kann nicht als Kennwort verwendet werden.<br>Standardmäßig erfordert Workfront, dass mindestens 2 der folgenden Zeichen in Passwörtern vorhanden sind (Sie können auch verlangen, dass 3 dieser Zeichen für ein gültiges Passwort vorhanden sind): </p> 
       <ul> 
        <li>Großbuchstaben</li> 
        <li>Kleinbuchstaben</li> 
        <li>Zahlen</li> 
        <li>Symbole</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. Klicken Sie auf **Speichern**.

## Erweiterte Authentifizierung konfigurieren{#configure-enhanced-authentication-coming-soon}

In diesem Abschnitt wird die erweiterte Authentifizierungserfahrung beschrieben, die möglicherweise noch nicht für Ihr Unternehmen verfügbar ist. Wenn Ihre Organisation nicht zur neuen Authentifizierungserfahrung migriert wurde, müssen Sie die Authentifizierungseinstellungen konfigurieren, wie beschrieben in [Authentifizierung konfigurieren (für alle Kunden verfügbar)](#configure-authentication-available-for-all-customers).

So konfigurieren Sie erweiterte Authentifizierungseinstellungen:

1. Klicken Sie auf **Hauptmenü** icon ![](assets/main-menu-icon.png) Klicken Sie oben rechts in Adobe Workfront auf **Einrichtung** ![](assets/gear-icon-settings.png).

1. Klicks **System** > **Erweiterte Authentifizierung**.
1. Im **Kennwortlänge** Geben Sie die für ein gültiges Passwort erforderliche Mindestanzahl von Zeichen ein.

   Workfront erfordert mindestens 6 Zeichen.

1. (Optional) Im **Passwortanforderungen** wählen Sie die für Benutzerkennwörter erforderlichen Zeichentypen aus.

   Sie können die Stärke von Benutzerkennwörtern erhöhen, indem Sie einen oder alle im Abschnitt &quot;Passwortanforderungen&quot;aufgeführten Zeichentypen benötigen. Die folgenden Optionen sind verfügbar:

   | Kleinbuchstaben | Mindestens einen Kleinbuchstaben anfordern |
   |---|---|
   | Großbuchstaben | Mindestens einen Großbuchstaben anfordern |
   | Zahlen | Mindestens eine Zahl erforderlich |
   | Sonderzeichen | Mindestens ein Sonderzeichen erforderlich |

   {style="table-layout:auto"}

1. Klicken Sie auf **Speichern**.
