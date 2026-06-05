---
user-type: administrator
product-area: system-administration;user-management;setup
navigation-topic: security
title: Kennwortrichtlinien für Authentifizierung konfigurieren
description: Als Adobe Workfront-Administrator können Sie Kennwortrichtlinienoptionen konfigurieren, um das Authentifizierungserlebnis an Ihr Workfront-System anzupassen.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 7832986b-a5e8-4f14-8802-d3b8e32b14bc
TQID: https://experienceleague.adobe.com/F74fLR5wH7a3X27WU5kAcgysO6R6ymJ895TCTHri1OA
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2:
  - id: b5ce8718-c3af-4fdb-a1a9-fca32f83a87c
  - id: bce87dde-a4ab-44c9-8a18-ad66e4ddb377
  - id: d095671a-1355-40aa-8b5f-06c33c68080b
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 662
ht-degree: 8%

---

# Kennwortrichtlinien für Authentifizierung konfigurieren

{{important-admin-console-onboard}}

Als Adobe Workfront-Administrator können Sie Kennwortrichtlinienoptionen konfigurieren, um das Authentifizierungserlebnis an Ihr Workfront-System anzupassen.

Es wird empfohlen, Authentifizierungseinstellungen während der Workfront-Implementierung zu konfigurieren und sie danach nur gelegentlich erneut aufzurufen.

Verbesserte Kennwortverwaltungsfunktionen werden in Kürze verfügbar sein oder sind möglicherweise bereits für Ihr Unternehmen verfügbar. Verwenden Sie einen der folgenden Abschnitte, je nachdem, ob Ihr Unternehmen Zugriff auf das neue Authentifizierungserlebnis hat.

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Paket</td> 
   <td><p>Beliebig</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td><p>Standard</p><p>Abo</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Sie müssen ein Workfront-Administrator sein.</p> </p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) in der Dokumentation zu Workfront.

+++

## Konfigurieren der Authentifizierung (für alle Kunden verfügbar) {#configure-authentication-available-for-all-customers}

Authentifizierungsoptionen werden für alle Kundinnen und Kunden angezeigt. Verbesserte Kennwortverwaltungsfunktionen werden in Kürze verfügbar sein oder sind möglicherweise bereits für Ihre Organisation verfügbar, wie im Abschnitt [Konfigurieren der erweiterten Authentifizierung)](#configure-enhanced-authentication-coming-soon) in diesem Artikel beschrieben.

So konfigurieren Sie Authentifizierungseinstellungen:

{{step-1-to-setup}}

1. Klicken Sie auf **System** > **Authentifizierung**.

1. Wählen Sie eines der folgenden Felder aus, um die Authentifizierungseinstellungen für Ihre Organisation festzulegen:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Benutzer zwingen, ihr Kennwort alle <em>&lt;value&gt;</em> Tage zurückzusetzen</td> 
      <td>Dadurch wird der Zeitrahmen festgelegt, in dem Benutzende ihr Workfront-Kennwort zurücksetzen können. Standardmäßig ist diese Option deaktiviert. Nach der Aktivierung können Sie zwischen 30, 60, 90, 120 oder 180 Tagen wählen. Der Standardwert ist 30 Tage.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Benutzern nicht erlauben, dasselbe Kennwort festzulegen wie bei allen vorherigen <em>&lt;value&gt;</em> Kennwörtern</td> 
      <td> <p>In diesem Feld ist die Wiederverwendung von Kennwörtern für eine bestimmte Anzahl von Zurücksetzungen untersagt. Standardmäßig ist dieses Feld deaktiviert. Wenn Sie sie aktivieren, können Sie diesen Wert auf 5, 10 oder 15 zurücksetzen, bevor ein Kennwort wiederverwendet werden kann.</p> <p>Wenn diese Option ausgewählt ist, können Benutzer ihre Kennwörter nicht öfter als einmal an einem bestimmten Tag zurücksetzen</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Wenn ein Kennwort fünfmal in Folge falsch eingegeben wurde, Konto für <em>&lt;value&gt;</em> Minuten sperren: </td> 
      <td> <p>Wählen Sie aus, wie lange ein Benutzer von Workfront gesperrt werden soll, nachdem er fünfmal in Folge ein falsches Kennwort eingegeben hat. Standardmäßig ist diese Option aktiviert und die Wartezeit beträgt 10 Minuten. Sie können Konten für 10 Minuten, 30 Minuten, 1 Stunde, 8 Stunden oder 24 Stunden sperren. </p> <p>Durch das manuelle Zurücksetzen des Kennworts für den Benutzer wird dieser standardmäßige Wartewert überschrieben. <br>Benutzer können ihre eigenen Kennwörter zurücksetzen, wenn sie über den Anmeldebildschirm gesperrt werden. Weitere Informationen zum Zurücksetzen des Kennworts, falls das Kennwort vergessen wurde, finden Sie unter <a href="../../../workfront-basics/manage-your-account-and-profile/managing-your-workfront-account/reset-your-password.md" class="MCXref xref">Kennwort zurücksetzen</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Kennwörter müssen mindestens <em>&lt;value&gt;</em> verschiedene Zeichentypen enthalten:</td> 
      <td> <p>Bestimmt, wie stark Benutzerkennwörter sein müssen, indem Sie die Anzahl der verschiedenen Zeichentypen auswählen, die für Ihre Kennwörter erforderlich sind.</p> <p>Ein erkennbares Wörterbuch kann nicht als Kennwort verwendet werden.<br>Standardmäßig erfordert Workfront, dass mindestens 2 der folgenden Zeichen in Kennwörtern vorhanden sind (Sie können auch festlegen, dass 3 dieser Zeichen für ein gültiges Kennwort vorhanden sein müssen): </p> 
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

## Konfigurieren der erweiterten Authentifizierung{#configure-enhanced-authentication-coming-soon}

In diesem Abschnitt wird die erweiterte Authentifizierung beschrieben, die für Ihre Organisation möglicherweise noch nicht verfügbar ist. Wenn Ihre Organisation nicht zum neuen Authentifizierungserlebnis migriert wurde, müssen Sie die Authentifizierungseinstellungen konfigurieren, wie in [Konfigurieren der Authentifizierung (für alle Kunden verfügbar)](#configure-authentication-available-for-all-customers) beschrieben.

So konfigurieren Sie erweiterte Authentifizierungseinstellungen:

{{step-1-to-setup}}

1. Klicken Sie auf **System** > **Erweiterte Authentifizierung**.
1. Geben Sie **Feld „Kennwortlänge** die Mindestanzahl von Zeichen ein, die für ein gültiges Kennwort erforderlich ist.

   Workfront erfordert mindestens 6 Zeichen.

1. (Optional) Wählen Sie im Abschnitt **Kennwortanforderungen** die in Benutzerkennwörtern erforderlichen Zeichentypen aus.

   Sie können die Stärke von Benutzerkennwörtern erhöhen, indem Sie einen oder alle Zeichentypen im Abschnitt „Kennwortanforderung“ erfordern. Die folgenden Optionen sind verfügbar:

   | Kleinbuchstaben | Mindestens einen Kleinbuchstaben erfordern |
   |---|---|
   | Großbuchstaben | Mindestens einen Großbuchstaben erfordern |
   | Zahlen | Mindestens eine Zahl erfordern |
   | Sonderzeichen | Mindestens ein Sonderzeichen erfordern |

   {style="table-layout:auto"}

1. Klicken Sie auf **Speichern**.
