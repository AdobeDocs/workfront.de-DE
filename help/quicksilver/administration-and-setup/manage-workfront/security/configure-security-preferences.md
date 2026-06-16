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
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/46D3BBajFk39FP-dMDk0SuSSGM5nYPKas11Bs159R9Y
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
  - id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
subfeature_v2:
  - id: e147ce9d-7675-49bd-8a32-44f27d865560
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: b5ce8718-c3af-4fdb-a1a9-fca32f83a87c
  - id: bce87dde-a4ab-44c9-8a18-ad66e4ddb377
  - id: d095671a-1355-40aa-8b5f-06c33c68080b
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 9d28f52ace4d443bdffc475baf79d482152d4157
workflow-type: tm+mt
source-wordcount: 964
ht-degree: 13%

---

# Systemvoreinstellungen konfigurieren

{{preview-fast-release-general}}

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
      <td role="rowheader">Benutzer dürfen die mobilen Anwendungen von Workfront nutzen</td> 
      <td> <p>Ermöglicht Benutzenden den Zugriff auf die Mobile Apps (Workfront View für iPad und Mobile Apps)</p> <p>Standardmäßig ist diese Option aktiviert. </p> <p>Weitere Informationen zur Workfront-Ansicht finden Sie unter <a href="../../../workfront-basics/mobile-apps/using-workfront-view/use-workfront-view.md" class="MCXref xref">Verwenden der Adobe Workfront-Ansicht</a>. Weitere Informationen zu den Mobile Apps finden Sie unter <a href="../../../workfront-basics/mobile-apps/using-the-workfront-mobile-app/use-the-mobile-app.md" class="MCXref xref">Verwenden der Adobe Workfront Mobile App: Artikelindex</a>.</p> </td> 
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
     <!--
     <tr> 
      <td role="rowheader">Require external users to register with a password</td> 
      <td> <p>Requires external users to register before they are able to view items in Workfront. By default, this option is disabled. When you enable this option, people without a Workfront account who are included in certain updates by their email address, will be prompted to create an account before they can view the item they are included on. This creates an External User account for them.</p> <p>This option is disabled by default.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Automatically log users out after</td> 
      <td> Lets you specify when a user is logged out of Workfront, after a period of inactivity. By default, users are logged out after 8 hours of inactivity. <p>This option also affects Workfront customers who are using a single sign-on solution.</p> <p>This setting is not available to organizations that have been migrated to Adobe IMS.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Automatically log mobile users out after </td> 
      <td>Lets you specify when a user is logged out of the Workfront application, after a period of inactivity. By default, users are logged out after 7 days of inactivity. <p>This option also affects Workfront customers who are using a single sign-on solution.</p> <p>This setting is not available to organizations that have been migrated to Adobe IMS.</p></td> 
     </tr>
     -->
     <tr> 
      <td role="rowheader">Hilfe-URL</td> 
      <td>Ermöglicht die Definition einer internen benutzerdefinierten Hilfeseite, zu der das Hilfesymbol des Hauptmenüs wechseln soll. Weitere Informationen finden Sie unter <a href="/help/quicksilver/administration-and-setup/customize-workfront/brand-workfront/configure-custom-help-url.md">Konfigurieren einer benutzerdefinierten Hilfe-URL</a>.</p></td> 
     </tr>
     <tr> 
      <td role="rowheader">Arbeitsliste „Prioritäten“ aktivieren </td> 
      <td>Ermöglicht die Auswahl oder Deaktivierung der Liste „Prioritäten“ für die Benutzer. Die Benutzer sehen weiterhin die Prioritätssymbole in Workfront, haben jedoch keinen Zugriff auf die Funktion. Weitere Informationen zu Prioritäten finden Sie unter <a href="/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md">Erste Schritte mit Prioritäten</a>.</td> 
     </tr>
     <tr>
      <td><span class="preview">Erforderliche Felder in Massenbearbeitung immer erzwingen</span></td>
      <td><span class="preview"><p>Hier können Sie auswählen, ob Benutzer bei der Massenbearbeitung von Objekten zur Eingabe von Informationen in erforderliche Felder gezwungen werden sollen.</p> <p>Wenn diese Option ausgewählt ist, müssen die erforderlichen Felder vor dem Speichern im Massenbearbeitungsmodus Werte aufweisen. Wenn im erforderlichen Feld ein Wert für mindestens ein Massenobjekt fehlt, ist das Speichern nicht zulässig.</p> <p>Wenn diese Option nicht ausgewählt ist, werden erforderliche Felder nur erzwungen, wenn ein Benutzer das Feld ändert. Wenn ein Feld nicht geändert wird, wird es als optional behandelt und nicht validiert.</p></span></td>
     </tr>
     <tr> 
      <td role="rowheader">Aktivieren von Adobe Cloud Storage </td> 
      <td>Ermöglicht die Aktivierung oder Deaktivierung der Adobe-Cloud-Datenspeicherung für das gesamte Unternehmen oder für bestimmte Gruppen. Weitere Informationen zu Adobe Cloud-Speicher finden Sie unter <a href="/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-esm.md">Aktivieren von Adobe Cloud-Speicher für Ihr Unternehmen</a>.</td> 
     </tr>
     <tr> 
      <td role="rowheader">Portfolios auswählen, die in Adobe Cloud-Speicher konvertiert werden sollen </td> 
      <td>Ermöglicht die Konvertierung vorhandener Workfront-Speicherportfolios in Adobe Cloud-Speicher. Weitere Informationen finden Sie unter <a href="/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/convert-portfolios-to-acs.md">Ältere Portfolios in Adobe Cloud-Speicher </a>.</td> 
     </tr>
     <tr> 
      <td role="rowheader">KI aktivieren </td> 
      <td>Ermöglicht die Auswahl der Aktivierung von KI, einschließlich des KI-Assistenten. <p><b>Hinweis</b>: Ihr Unternehmen muss bestimmte Anforderungen erfüllen, um KI zu aktivieren. Weitere Informationen zu KI, einschließlich der Anforderungen, finden Sie unter <a href="/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md">KI-Assistent - Übersicht</a>.</p></td> 
     </tr>
     <tr> 
      <td role="rowheader">Formular automatisch ausfüllen </td> 
      <td>Ermöglicht die Auswahl der Möglichkeit, Anfrageformulare basierend auf den Daten einer vorherigen Anfrage automatisch auszufüllen. Weitere Informationen zum automatischen Vervollständigen von Formularen finden Sie unter <a href="/help/quicksilver/manage-work/requests/create-requests/autofill-suggestions-from-previous.md">Automatisches Ausfüllen einer Anfrage aus vorherigen Daten</a>.</td> 
     </tr>
     <tr> 
      <td role="rowheader">Opt-in für KI-Betaversionen </td> 
      <td>Ermöglicht die Auswahl von KI-Funktionen, die sich derzeit in Beta befinden. Wenn Sie diese Option aktivieren, können Sie auswählen, welche KI-Beta-Funktionen aktiviert werden sollen. Um weitere Informationen zu den einzelnen KI-Beta-Funktionen zu erhalten, klicken Sie auf das Informationssymbol neben dieser Funktion.</td> 
     </tr>
     <tr> 
      <td role="rowheader"><span class="preview">Schreibgeschützte MCP-Tools</span></td> 
      <td><span class="preview">Ermöglicht dem Workfront MCP-Server die Durchführung von Leseaktionen für Workfront-Daten, z. B. das Suchen oder Auflisten von Projekten, Aufgaben oder anderen Elementen. Standardmäßig ist diese Option aktiviert.<p>Weitere Informationen zum Workfront MCP-Server finden Sie unter <a href="/help/quicksilver/workfront-basics/workfront-mcp-server/configure-workfront-mcp-server.md">Konfigurieren des Adobe Workfront MCP-Servers</a>.</p></span></td> 
     </tr>
     <tr> 
      <td role="rowheader"><span class="preview">MCP-Tools schreiben</span></td> 
      <td><span class="preview">Ermöglicht dem Workfront-MCP-Server das Erstellen, Aktualisieren und Löschen von Aktionen für Workfront-Daten. Standardmäßig ist diese Option deaktiviert.<p>Weitere Informationen zum Workfront MCP-Server finden Sie unter <a href="/help/quicksilver/workfront-basics/workfront-mcp-server/configure-workfront-mcp-server.md">Konfigurieren des Adobe Workfront MCP-Servers</a>.</p></span></td> 
     </tr>
     <tr> 
      <td role="rowheader">Testumgebungen</td> 
      <td>Ermöglicht den Zugriff auf Ihre Workfront-Testumgebungen. Weitere Informationen finden Sie unter <a href="/help/quicksilver/workfront-basics/priorities/get-started-with-priorities.md">Die Adobe Workfront-Sandbox-Umgebung in der Vorschau</a>.</p></td> 
    </tbody> 
   </table>

1. Klicken Sie auf **Speichern**.

   Die Änderungen, die Sie hier gespeichert haben, wirken sich auf das Erlebnis aller Benutzenden in Workfront und auf alle Benutzenden aus, die als externe Benutzende mit dem System interagieren.
