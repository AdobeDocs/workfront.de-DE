---
user-type: administrator
product-area: system-administration;user-management;setup
navigation-topic: security
title: Systemeinstellungen konfigurieren
description: Als Adobe Workfront-Administrator können Sie Voreinstellungen für Ihr Workfront-System konfigurieren, einschließlich Sicherheitseinstellungen.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: f92ceed7-b191-425b-9fff-1b0947f32db8
source-git-commit: 945fa710e98b094a37258d5c94f7b1a2eb056abb
workflow-type: tm+mt
source-wordcount: '951'
ht-degree: 7%

---

# Systemvoreinstellungen konfigurieren

<!--
DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.</p>
-->

<!--Audited: 05/2024-->

{{important-admin-console-onboard}}

Als Adobe Workfront-Administrator können Sie Voreinstellungen für Ihr Workfront-System konfigurieren, darunter:

* Zugriff auf Workfront über Mobile Apps und andere integrierte Anwendungen
* Regeln für das Einbetten von Workfront in einen iframe

Änderungen an den Systemvoreinstellungen wirken sich auf alle Benutzenden in Ihrem System und deren Erlebnis in Workfront aus.

Es wird empfohlen, Ihre Systemeinstellungen während der Workfront-Implementierung zu konfigurieren und sie danach nur gelegentlich erneut aufzurufen.

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
   <p>oder</p>
   <p>Aktuell: Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Sie müssen ein Workfront-Administrator sein.</p></td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Systemeinstellungen konfigurieren

{{step-1-to-setup}}

1. Klicken Sie im linken Bedienfeld auf **System** > **Voreinstellungen**.

1. Wählen Sie eines der folgenden Felder aus, um die Einstellungen für Ihre Organisation festzulegen:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>Schnellen Release-Prozess aktivieren</p> </td> 
      <td>Ermöglicht die Aktivierung monatlicher Workfront-Versionen für Ihr Unternehmen anstelle vierteljährlicher Versionen.</p><p>Weitere Informationen zum Schnellveröffentlichungsprozess finden Sie unter <a href="/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md" class="MCXref xref">Aktivieren oder Deaktivieren von Schnellversionen für Ihre Organisation</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Einbetten von Workfront in einen iframe zulassen</p> </td> 
      <td>Ermöglicht das Einbetten von Workfront in einen iframe.<p>Standardmäßig ist diese Option deaktiviert.</p><p><b>WICHTIG</b>: Wenn eine Web-basierte Anwendung in einem iframe angezeigt wird, wird die Anwendung anfällig für eine Sicherheitslücke durch Clickjacking.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">SAML 2.0-Authentifizierung in Office 365-Add-ins zulassen.</td> 
      <td> <p>Ermöglicht das Einbetten von Workfront in einen iframe nur für Office 365-Add-Ins, wenn Workfront mit einer SAML 2.0-Lösung für einmaliges Anmelden integriert ist. </p> <p>Standardmäßig ist diese Option aktiviert.</p> <p><b>HINWEIS</b>: Wenn Sie die obige Option <strong>Einbetten von Workfront in einen iframe zulassen</strong> aktivieren, wird die Option <strong>SAML 2.0-Authentifizierung in Office 365-Add-</strong> zulassen) aktiviert und abgeblendet.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Verwendung von Sitzungsinformationen beim Erstellen von URLs für externe Seiten aktivieren</td> 
      <td> <p>Ermöglicht Benutzern die Verwendung der Sitzungs-ID-Informationen einer Site beim Hinzufügen einer externen Seite zu einem Dashboard.</p> <p>Diese Option ist nicht sicher und standardmäßig deaktiviert. Es wird empfohlen, stattdessen OAuth für Integrationen zu verwenden.</p> <p>Weitere Informationen zum Hinzufügen externer Seiten zu einem Dashboard finden Sie unter <a href="../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md" class="MCXref xref">Externe Webseite in ein Dashboard einbetten</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Benutzer dürfen die mobilen Anwendungen von Workfront und das Workfront Outlook-Add-in verwenden</td> 
      <td> <p>Ermöglicht Benutzenden den Zugriff auf die mobilen Apps (Workfront View für iPad und Apps für Mobiltelefone) und die Workfront Outlook-App.</p> <p>Standardmäßig ist diese Option aktiviert. </p> <p>Weitere Informationen zur Workfront-Ansicht finden Sie unter <a href="../../../workfront-basics/mobile-apps/using-workfront-view/use-workfront-view.md" class="MCXref xref">Verwenden der Adobe Workfront-Ansicht</a>. Weitere Informationen zu den Mobile Apps finden Sie unter <a href="../../../workfront-basics/mobile-apps/using-the-workfront-mobile-app/use-the-mobile-app.md" class="MCXref xref">Verwenden der Adobe Workfront Mobile App: Artikelindex</a>.</p> <p>Weitere Informationen zum Outlook-Plug-in finden Sie unter <a href="../../../workfront-integrations-and-apps/using-workfront-with-outlook/set-up-workfront-for-outlook.md" class="MCXref xref">Einrichten von Adobe Workfront für Outlook</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Mit Personen ohne Workfront-Konto über E-Mail-Adressen zusammenarbeiten</p> </td> 
      <td>Ermöglicht es Workfront-Benutzern, bestimmte Elemente für Personen ohne Workfront-Konto freizugeben, indem ihre E-Mail-Adresse anstelle ihres Namens angegeben wird. Benutzer können die folgenden Elemente über ihre E-Mail-Adresse für externe Benutzer freigeben:
       <ul>
        <li>Dokument<br></li>
        <li>Dokumentanforderung<br></li>
        <li>Dokumentengenehmigung</li>
        <li>Kalender</li>
       </ul><p>Standardmäßig ist diese Option aktiviert.</p> <p><b>Wichtig</b>: Die Zugriffsebene Externe Benutzer ist in Ihrer Workfront-Instanz nicht verfügbar, wenn diese Option deaktiviert ist. Weitere Informationen finden Sie <a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/default-access-levels-in-workfront.md" class="MCXref xref">Integrierte Zugriffsebenen</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Externe Benutzer auffordern, sich mit einem Kennwort zu registrieren</td> 
      <td> <p>Externe Benutzer müssen sich registrieren, bevor sie Elemente in Workfront anzeigen können. Standardmäßig ist diese Option deaktiviert. Wenn Sie diese Option aktivieren, werden Personen ohne Workfront-Konto, die über ihre E-Mail-Adresse in bestimmte Updates eingebunden sind, aufgefordert, ein Konto zu erstellen, bevor sie das Element anzeigen können, in dem sie enthalten sind. Dadurch wird ein externes Benutzerkonto für sie erstellt.</p> <p>Standardmäßig ist diese Option deaktiviert.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Benutzer automatisch abmelden nach</td> 
      <td> Hier können Sie angeben, wann ein Benutzer nach einer gewissen Zeit der Inaktivität von Workfront abgemeldet wird. Standardmäßig werden Benutzer nach 8 Stunden Inaktivität abgemeldet. <p>Diese Option wirkt sich auch auf Workfront-Kunden aus, die eine Single Sign-on-Lösung verwenden.</p> <p>Diese Einstellung ist nicht für Organisationen verfügbar, die zu Adobe IMS migriert wurden.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Mobile Benutzer automatisch abmelden nach </td> 
      <td>Hier können Sie angeben, wann ein Benutzer nach einer gewissen Zeit der Inaktivität bei der Workfront-Anwendung abgemeldet wird. Standardmäßig werden Benutzer nach 7 Tagen Inaktivität abgemeldet. <p>Diese Option wirkt sich auch auf Workfront-Kunden aus, die eine Single Sign-on-Lösung verwenden.</p> <p>Diese Einstellung ist nicht für Organisationen verfügbar, die zu Adobe IMS migriert wurden.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Hilfe-URL</td> 
      <td>Ermöglicht die Definition einer internen benutzerdefinierten Hilfeseite, zu der das Hilfesymbol des Hauptmenüs wechseln soll. Weitere Informationen finden Sie unter <a href="/help/quicksilver/administration-and-setup/customize-workfront/brand-workfront/configure-custom-help-url.md">Konfigurieren einer benutzerdefinierten Hilfe-URL</a>.</p></td> 
     </tr>
     <tr> 
      <td role="rowheader">Benutzer im System sehen standardmäßig die neue Startseite </td> 
      <td>Hier können Sie angeben, ob Benutzern das neue Startseiten-Erlebnis standardmäßig angezeigt wird. Wenn diese Option aktiviert ist, wird den Benutzenden standardmäßig die neue Startseite angezeigt, sie können sich jedoch auch einzeln für die Aktivierung oder Deaktivierung der neuen Startseite entscheiden. Wenn diese Option deaktiviert ist, wird den Benutzenden das Banner, das ihnen den Wechsel zur neuen Startseite ermöglicht, nicht angezeigt. Sie können jedoch weiterhin zur neuen Startseite navigieren, indem sie am Ende ihrer Instanz-URL manuell <code>/home/workspaces</code> eingeben. Diese Einstellung ist standardmäßig aktiviert.</td> 
     </tr>
     <tr> 
      <td role="rowheader">Arbeitsliste „Prioritäten“ aktivieren </td> 
      <td>Ermöglicht die Auswahl oder Deaktivierung der Liste „Prioritäten“ für die Benutzer. Die Benutzer sehen weiterhin die Prioritätssymbole in Workfront, haben jedoch keinen Zugriff auf die Funktion. Weitere Informationen zu Prioritäten finden Sie unter <a href="/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md">Erste Schritte mit Prioritäten</a>.</td> 
     </tr>
     <tr> 
      <td role="rowheader">Testumgebungen</td> 
      <td>Ermöglicht den Zugriff auf Ihre Workfront-Testumgebungen. Weitere Informationen finden Sie unter <a href="/help/quicksilver/workfront-basics/priorities/get-started-with-priorities.md">Die Adobe Workfront-Vorschau-Sandbox-Umgebung</a>.</p></td> 
    </tbody> 
   </table>

1. Klicken Sie auf **Speichern**.

   Die Änderungen, die Sie hier gespeichert haben, wirken sich auf das Erlebnis aller Benutzenden in Workfront und auf alle Benutzenden aus, die als externe Benutzende mit dem System interagieren.
