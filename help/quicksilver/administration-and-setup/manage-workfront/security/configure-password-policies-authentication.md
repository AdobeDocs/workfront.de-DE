---
user-type: administrator
product-area: system-administration;user-management;setup
navigation-topic: security
title: Kennwortrichtlinien für Authentifizierung konfigurieren
description: Als Adobe Workfront-Administrator können Sie Optionen für Kennwortrichtlinien konfigurieren, um die Authentifizierungserfahrung auf Ihr Workfront-System anzupassen.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 7832986b-a5e8-4f14-8802-d3b8e32b14bc
source-git-commit: 206ea3ad1398849e26dea7fe77f6d7c027825b6f
workflow-type: tm+mt
source-wordcount: '705'
ht-degree: 2%

---

# Kennwortrichtlinien für Authentifizierung konfigurieren

{{important-admin-console-onboard}}

Als Adobe Workfront-Administrator können Sie Optionen für Kennwortrichtlinien konfigurieren, um die Authentifizierungserfahrung auf Ihr Workfront-System anzupassen.

Es wird empfohlen, die Authentifizierungseinstellungen während der Workfront-Implementierung zu konfigurieren und sie anschließend nur gelegentlich erneut aufzurufen.

Verbesserte Funktionen zur Kennwortverwaltung stehen in Kürze zur Verfügung oder stehen möglicherweise bereits für Ihre Organisation zur Verfügung. Verwenden Sie einen der folgenden Abschnitte, je nachdem, ob Ihr Unternehmen Zugriff auf das neue Authentifizierungs-Erlebnis hat.

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
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Sie müssen Workfront-Administrator sein.</p> <p><b>HINWEIS</b>: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## Authentifizierung konfigurieren (für alle Kunden verfügbar) {#configure-authentication-available-for-all-customers}

Authentifizierungsoptionen werden für alle Kunden angezeigt. Verbesserte Funktionen zur Kennwortverwaltung stehen in Kürze zur Verfügung oder sind möglicherweise bereits für Ihre Organisation verfügbar, wie im Abschnitt [Erweiterte Authentifizierung konfigurieren)](#configure-enhanced-authentication-coming-soon) in diesem Artikel beschrieben.

So konfigurieren Sie Authentifizierungsvoreinstellungen:

{{step-1-to-setup}}

1. Klicken Sie auf **System** > **Authentifizierung**.

1. Wählen Sie eines der folgenden Felder aus, um die Authentifizierungseinstellungen für Ihr Unternehmen festzulegen:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Benutzer dazu zwingen, ihr Kennwort alle <em>&lt;Wert&gt;</em> Tage zurückzusetzen</td> 
      <td>Dadurch wird der Zeitrahmen für das Zurücksetzen des Workfront-Kennworts festgelegt. Standardmäßig ist diese Option deaktiviert. Wenn Sie sie aktivieren, können Sie zwischen 30, 60, 90, 120, 180 Tagen wählen. Der Standardwert ist 30 Tage.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Erlauben Sie Benutzern nicht, dasselbe Kennwort wie die vorherigen <em>&lt;Wert&gt;</em>-Kennwörter festzulegen.</td> 
      <td> <p>Dieses Feld untersagt Benutzern, Kennwörter für eine bestimmte Anzahl von Zurücksetzungen wiederzuverwenden. Standardmäßig ist dieses Feld deaktiviert. Wenn Sie sie aktivieren, können Sie diesen Wert auf 5, 10 oder 15 Zurücksetzungen setzen, bevor ein Kennwort wiederverwendet werden kann.</p> <p>Wenn diese Option aktiviert ist, können Benutzer ihre Kennwörter nicht mehr als einmal an einem bestimmten Tag zurücksetzen</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Wenn fünf aufeinander folgende Male ein falsches Kennwort eingegeben wird, sperren Sie das Konto für <em>&lt;Wert&gt;</em> Minuten: </td> 
      <td> <p>Wählen Sie aus, wie lange ein Benutzer fünf Mal hintereinander aus Workfront ausgesperrt wird, nachdem er ein falsches Kennwort eingegeben hat. Standardmäßig ist diese Option aktiviert und die Wartezeit beträgt 10 Minuten. Sie können Konten für 10 Minuten, 30 Minuten, 1 Stunde, 8 Stunden oder 24 Stunden sperren. </p> <p>Durch das manuelle Zurücksetzen des Kennworts für den Benutzer wird dieser standardmäßige Wartewert überschrieben. <br>Benutzer können ihre eigenen Kennwörter zurücksetzen, wenn sie über den Anmeldebildschirm gesperrt werden. Weitere Informationen dazu, wie sie ihr Kennwort zurücksetzen können, wenn sie es vergessen haben, finden Sie unter <a href="../../../workfront-basics/manage-your-account-and-profile/managing-your-workfront-account/reset-your-password.md" class="MCXref xref">Passwort zurücksetzen</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Passwörter müssen mindestens <em>&lt;Wert&gt;</em> verschiedene Arten von Zeichen enthalten:</td> 
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

In diesem Abschnitt wird die erweiterte Authentifizierungserfahrung beschrieben, die möglicherweise noch nicht für Ihr Unternehmen verfügbar ist. Wenn Ihre Organisation nicht zur neuen Authentifizierungserfahrung migriert wurde, müssen Sie die Authentifizierungseinstellungen konfigurieren, wie unter [Authentifizierung konfigurieren (für alle Kunden verfügbar)](#configure-authentication-available-for-all-customers) beschrieben.

So konfigurieren Sie erweiterte Authentifizierungseinstellungen:

{{step-1-to-setup}}

1. Klicken Sie auf **System** > **Erweiterte Authentifizierung**.
1. Geben Sie in das Feld **Kennwortlänge** die Mindestanzahl von Zeichen ein, die für ein gültiges Kennwort erforderlich sind.

   Workfront erfordert mindestens 6 Zeichen.

1. (Optional) Wählen Sie im Abschnitt **Passwortanforderungen** die für Benutzerkennwörter erforderlichen Zeichentypen aus.

   Sie können die Stärke von Benutzerkennwörtern erhöhen, indem Sie einen oder alle im Abschnitt &quot;Passwortanforderungen&quot;aufgeführten Zeichentypen benötigen. Die folgenden Optionen sind verfügbar:

   | Kleinbuchstaben | Mindestens einen Kleinbuchstaben anfordern |
   |---|---|
   | Großbuchstaben | Mindestens einen Großbuchstaben anfordern |
   | Zahlen | Mindestens eine Zahl erforderlich |
   | Sonderzeichen | Mindestens ein Sonderzeichen erforderlich |

   {style="table-layout:auto"}

1. Klicken Sie auf **Speichern**.
