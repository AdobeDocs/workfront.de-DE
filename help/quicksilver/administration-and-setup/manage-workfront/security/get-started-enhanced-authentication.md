---
title: Erweiterte Authentifizierung - Übersicht
description: Ausgeblendet für die Suche und in der linken Navigationsleiste
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

# Erweiterte Authentifizierung - Übersicht

<!-- enhanced authentication is no longer available for workfront customers -->

{{important-admin-console-onboard}}

Adobe Workfront verändert die Systemverwaltung von Benutzenden und Kennwörtern. Diese Änderungen werden in einer stufenweisen Veröffentlichung mit der Bezeichnung **Erweiterte Authentifizierung** eingeführt. Die verbesserte Authentifizierung bietet Benutzenden ein konsistenteres und sichereres Anmeldeerlebnis für alle Workfront-Produkte und -Services.

Die folgende Tabelle enthält Details zur aktuellen und künftigen Funktionalität:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col data-mc-conditions=""> 
 <thead> 
  <tr> 
   <th> <p><strong>Funktion</strong> </p> </th> 
   <th><strong>Legacy-Authentifizierung</strong> </th> 
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
   <td> <p>Verwendung eines einzigen Benutzernamens für alle Workfront-Produkte und -Services aktivieren, einschließlich Schulung, Support und andere</p> </td> 
   <td>Nicht verfügbar</td> 
   <td> <p>Nicht verfügbar</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Verwendung derselben E-Mail-Adresse in allen Workfront-Instanzen zulassen</p> </td> 
   <td> <p>✓</p> <p>Ab Version 2019.3 verfügbar</p> </td> 
   <td> <p>✓</p> <p>Ab Version 2019.3 verfügbar</p> </td> 
   <td> <p>✓</p> <p>Ab Version 2019.3 verfügbar</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Bei E-Mail-Adressen wird nicht zwischen Groß- und Kleinschreibung unterschieden</p> </td> 
   <td> <p>✓</p> <p>Ab Version 2019.3 verfügbar</p> </td> 
   <td> <p>✓</p> <p>Mehrere Benutzer können nicht dieselbe E-Mail-Adresse haben, wenn sich die Adresse nur durch die Groß-/Kleinschreibung unterscheidet. </p> </td> 
   <td> <p>✓</p> <p>Mehrere Benutzer können nicht dieselbe E-Mail-Adresse haben, wenn sich die Adresse nur durch die Groß-/Kleinschreibung unterscheidet. </p> <p>Workfront-Administratoren werden Ende 2019 benachrichtigt, wenn sie mit der Behebung doppelter E-Mail-Adressen beginnen.</p> </td> 
  </tr> 
  <tr> 
   <td colspan="3"> <p><strong>Kennwortverwaltungsoptionen</strong> </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Initiieren einer E-Mail zum Zurücksetzen des Kennworts für einen Benutzer als Workfront-Administrator</p> </td> 
   <td> <p>Nicht verfügbar </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Legen Sie ein temporäres Kennwort für einen Benutzer als Workfront-Administrator fest</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>Nicht geplant</p> <p>Diese Funktion ist keine Best Practice für die Sicherheit</p> </td> 
   <td> <p>Nicht geplant</p> <p>Diese Funktion ist keine Best Practice für die Sicherheit</p> </td> 
  </tr> 
  <tr> 
   <td colspan="3"> <p><strong>Anforderungen an Passwortrichtlinien</strong> </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Benutzer auffordern, Kennwörter nach einem bestimmten Zeitraum zurückzusetzen</p> </td> 
   <td>✓</td> 
   <td> <p>Nicht geplant</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Benutzer von der Verwendung eines früheren Kennworts abhalten </p> </td> 
   <td>✓</td> 
   <td>Nicht geplant </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Schutz vor falschen Passworteingabeversuchen </p> </td> 
   <td> <p>✓ </p> <p>Sperrt das Konto nach 5 falschen Passworteingabeversuchen. Die nach der Sperrung erforderliche Wartezeit wird vom Workfront-Administrator konfiguriert</p> </td> 
   <td> <p>✓</p> <p>Die Wartezeit wird nach jedem aufeinander folgenden falschen Kennwort auf der Grundlage von Best Practices der Branche exponentiell erhöht. Die erforderliche Zeit kann vom Workfront-Administrator nicht konfiguriert werden</p> </td> 
   <td> <p>✓</p> <p>Verwendet einen Sperralgorithmus, der proaktiv eine Vielzahl verdächtiger Verhaltensweisen blockiert.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Kombination aus Kleinbuchstaben, Großbuchstaben, Zahlen und Sonderzeichen erforderlich</p> </td> 
   <td>✓</td> 
   <td> <p>✓ </p> <p>Höhere Flexibilität bei der Auswahl spezifischer Anforderungen</p> </td> 
   <td> <p>✓</p> <p> 
     </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Festlegen einer Mindestkennwortlänge </p> </td> 
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
   <td colspan="3"> <p><strong>Unterstützung des Single Sign-On Protokolls</strong></p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Unterstützt SSO-Integrationen, die mit Active Directory- und LDAP-Protokollen konform sind</p> </td> 
   <td> ✓ </td> 
   <td> <p> Veraltet</p> <p>Active Directory-, Azure- und LDAP-Systeme sollten SAML 2.0 verwenden.</p> </td> 
   <td> <p>Veraltet</p> <p>Active Directory-, Azure- und LDAP-Systeme können mit verschlüsseltem SAML 2.0 oder OpenID Connect konfiguriert werden.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Unterstützt SSO-Protokolle, die mit SAML 2.0 konform sind </p> </td> 
   <td>✓</td> 
   <td> ✓ </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Unterstützt Open ID Connect-Protokolle</p> </td> 
   <td> <p>Nicht verfügbar</p> </td> 
   <td> <p>Nicht verfügbar</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p> Konfigurieren Sie die Anmeldeseite von Workfront so, dass sie immer zur Anmeldeseite von Identity Provider umgeleitet wird </p> </td> 
   <td> Standardmäßig aktiviert und nicht deaktiviert werden</td> 
   <td> <p>✓</p> <p>Workfront-Admins können die Anmeldeseite so konfigurieren, dass sie zur Anmeldeseite des Identitätsanbieters weiterleitet, oder sie können eine Anmelde-Schaltfläche oder Schaltflächen konfigurieren.</p> </td> 
   <td> <p>✓</p> <p> Workfront-Admins können die Anmeldeseite so konfigurieren, dass sie zur Anmeldeseite des Identitätsanbieters weiterleitet, oder sie können eine Anmelde-Schaltfläche oder Schaltflächen konfigurieren.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Zulassen, dass jede Instanz mehrere SSO-Provider aktiviert</p> </td> 
   <td> <p>K. A.</p> </td> 
   <td> <p>Nicht geplant</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td colspan="3"> <p><strong>Umgebungsunterstützung</strong> </p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Ein einzelner Benutzername und ein Passwort für die Vorschau-Umgebung</p> </td> 
   <td> <p>Nicht verfügbar</p> </td> 
   <td> <p>Nicht verfügbar</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Ein einzelner Benutzername und ein Passwort für Sandbox-Umgebungen</p> </td> 
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
