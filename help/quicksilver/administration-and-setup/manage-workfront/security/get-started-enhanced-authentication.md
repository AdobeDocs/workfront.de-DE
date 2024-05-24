---
title: Verbesserte Authentifizierung - Übersicht
description: Ausgeblendet aus der Suche und aus der linken Navigationsleiste
hidefromtoc: true
hide: true
feature: System Setup and Administration
role: Admin
exl-id: bf3c6c6f-ddd5-42d0-9efe-b5eb94549f85
source-git-commit: bf8e6c2b8a45cf65840a2ac8b3c25d11266d49f9
workflow-type: tm+mt
source-wordcount: '537'
ht-degree: 0%

---

# Verbesserte Authentifizierung - Übersicht

<!-- enhanced authentication is no longer available for workfront customers -->

{{important-admin-console-onboard}}

Adobe Workfront ändert die Systemverwaltung von Benutzern und Kennwörtern. Diese Änderungen werden in einer stufenweisen Version mit dem Namen **Erweiterte Authentifizierung** Erlebnis. Die erweiterte Authentifizierung bietet Benutzern eine konsistentere und sicherere Anmeldeerfahrung für alle Workfront-Produkte und -Dienste.

Die folgende Tabelle enthält Details zur aktuellen und zukünftigen Funktionalität:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col data-mc-conditions=""> 
 <thead> 
  <tr> 
   <th> <p><strong>Funktion</strong> </p> </th> 
   <th><strong>Alte Authentifizierung</strong> </th> 
   <th><strong>Erweiterte Authentifizierung 1.0</strong> </th> 
   <th> <p>Erweiterte Authentifizierung 2.0</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td colspan="3"> <p><strong>Anmeldeoptionen</strong> </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aktivieren Sie einen einzigen Benutzernamen, der für alle Workfront-Produkte und -Dienste verwendet werden soll, einschließlich Schulung, Support und anderen</p> </td> 
   <td>Nicht verfügbar</td> 
   <td> <p>Nicht verfügbar</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Verwendung derselben E-Mail-Adresse in Workfront-Instanzen zulassen</p> </td> 
   <td> <p>✓</p> <p>Verfügbar ab Version 2019.3</p> </td> 
   <td> <p>✓</p> <p>Verfügbar ab Version 2019.3</p> </td> 
   <td> <p>✓</p> <p>Verfügbar ab Version 2019.3</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Bei E-Mail-Adressen wird nicht zwischen Groß- und Kleinschreibung unterschieden</p> </td> 
   <td> <p>✓</p> <p>Verfügbar ab Version 2019.3</p> </td> 
   <td> <p>✓</p> <p>Mehrere Benutzer können nicht dieselbe E-Mail-Adresse haben, wenn sich die Adresse nur von Fall zu Fall unterscheidet. </p> </td> 
   <td> <p>✓</p> <p>Mehrere Benutzer können nicht dieselbe E-Mail-Adresse haben, wenn sich die Adresse nur von Fall zu Fall unterscheidet. </p> <p>Workfront-Administratoren werden Ende 2019 benachrichtigt, damit sie mit der Behebung doppelter E-Mail-Adressen beginnen können.</p> </td> 
  </tr> 
  <tr> 
   <td colspan="3"> <p><strong>Optionen zur Kennwortverwaltung</strong> </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>E-Mail zum Zurücksetzen des Kennworts für einen Benutzer als Workfront-Administrator aktivieren</p> </td> 
   <td> <p>Nicht verfügbar </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Festlegen eines temporären Kennworts für einen Benutzer als Workfront-Administrator</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>Nicht geplant</p> <p>Diese Funktion ist keine Best Practice für Sicherheitsmaßnahmen</p> </td> 
   <td> <p>Nicht geplant</p> <p>Diese Funktion ist keine Best Practice für Sicherheitsmaßnahmen</p> </td> 
  </tr> 
  <tr> 
   <td colspan="3"> <p><strong>Anforderungen für Passwortrichtlinien</strong> </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Benutzer müssen Kennwörter nach einem bestimmten Zeitraum zurücksetzen</p> </td> 
   <td>✓</td> 
   <td> <p>Nicht geplant</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Benutzer daran hindern, ein vorheriges Kennwort zu verwenden </p> </td> 
   <td>✓</td> 
   <td>Nicht geplant </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Schutz vor falschen Kennworteintragungsversuchen </p> </td> 
   <td> <p>✓ </p> <p>Sperrt das Konto nach fünf falschen Kennworteintragungsversuchen. Die nach der Sperrung benötigte Wartezeit wird vom Workfront-Administrator konfiguriert</p> </td> 
   <td> <p>✓</p> <p>Die Wartezeit wird exponentiell nach jedem aufeinander folgenden fehlerhaften Passwort erhöht, das auf Best Practices der Branche basiert. Die erforderliche Zeit kann vom Workfront-Administrator nicht konfiguriert werden.</p> </td> 
   <td> <p>✓</p> <p>Verwendet einen Sperralgorithmus, der eine Vielzahl verdächtiger Verhaltensweisen proaktiv blockiert.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Muss aus Kleinbuchstaben, Großbuchstaben, Zahlen und Sonderzeichen bestehen</p> </td> 
   <td>✓</td> 
   <td> <p>✓ </p> <p>Höhere Flexibilität bei der Auswahl bestimmter Anforderungen</p> </td> 
   <td> <p>✓</p> <p> 
     </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Mindestens Kennwortlänge festlegen </p> </td> 
   <td> Nicht verfügbar </td> 
   <td> ✓ </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td>Restrict users from using more than 2 identical characters in a row</td> 
    <td>Not available</td> 
    <td>Not available</td> 
    <td> <p>✓</p> </td> 
   </tr>
  --> 
  <tr> 
   <td colspan="3"> <p><strong>Unterstützung des Single Sign-On-Protokolls</strong></p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Unterstützt SSO-Integrationen, die mit Active Directory- und LDAP-Protokollen konform sind</p> </td> 
   <td> ✓ </td> 
   <td> <p> Veraltet</p> <p>Active Directory-, Azure- und LDAP-Systeme sollten SAML 2.0 verwenden</p> </td> 
   <td> <p>Veraltet</p> <p>Active Directory-, Azure- und LDAP-Systeme können mit verschlüsseltem SAML 2.0 oder OpenID Connect konfiguriert werden.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Unterstützt SSO-Protokolle, die mit SAML 2.0 konform sind </p> </td> 
   <td>✓</td> 
   <td> ✓ </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Unterstützt offene ID Connect-Protokolle</p> </td> 
   <td> <p>Nicht verfügbar</p> </td> 
   <td> <p>Nicht verfügbar</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p> Konfigurieren der Workfront-Anmeldeseite, um immer zur Anmeldeseite des Identitätsanbieters umzuleiten </p> </td> 
   <td> Standardmäßig aktiviert und kann nicht deaktiviert werden</td> 
   <td> <p>✓</p> <p>Der Workfront-Administrator kann die Anmeldeseite konfigurieren, um zur Anmeldeseite des Identitätsanbieters umzuleiten, oder eine Anmelde-Schaltfläche oder Schaltflächen konfigurieren.</p> </td> 
   <td> <p>✓</p> <p> Workfront-Administratoren können die Anmeldeseite so konfigurieren, dass sie zur Anmeldeseite des Identitätsanbieters weitergeleitet wird, oder eine Anmelde-Schaltfläche oder Schaltflächen konfigurieren.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Jede Instanz kann mehrere SSO-Anbieter aktivieren</p> </td> 
   <td> <p>K. A.</p> </td> 
   <td> <p>Nicht geplant</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td colspan="3"> <p><strong>Umgebungsunterstützung</strong> </p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Ein einziger Benutzername und ein Kennwort für die Vorschau von Umgebungen</p> </td> 
   <td> <p>Nicht verfügbar</p> </td> 
   <td> <p>Nicht verfügbar</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Ein einzelner Benutzername und ein Kennwort für Sandbox-Umgebungen</p> </td> 
   <td> <p>Nicht verfügbar</p> </td> 
   <td> <p>Nicht verfügbar</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <!--
   <tr> 
    <td> <p>Available for Production environments</p> </td> 
    <td>✓</td> 
    <td> ✓&nbsp;</td> 
    <td> <p>✓</p> </td> 
   </tr>
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td> Available for Preview and Sandbox environments&nbsp;</td> 
    <td> ✓&nbsp;</td> 
    <td> ✓</td> 
    <td> <p>✓</p> </td> 
   </tr>
  --> 
 </tbody> 
</table>
