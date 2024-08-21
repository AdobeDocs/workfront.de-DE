---
user-type: administrator
product-area: system-administration;user-management;setup
navigation-topic: security
title: Systemvoreinstellungen konfigurieren
description: Als Adobe Workfront-Administrator können Sie die Voreinstellungen für Ihr Workfront-System, einschließlich der Sicherheitseinstellungen, konfigurieren.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: f92ceed7-b191-425b-9fff-1b0947f32db8
source-git-commit: 206ea3ad1398849e26dea7fe77f6d7c027825b6f
workflow-type: tm+mt
source-wordcount: '877'
ht-degree: 4%

---

# Systemvoreinstellungen konfigurieren

<!--
DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.</p>
-->

<!--Audited: 05/2024-->

{{important-admin-console-onboard}}

Als Adobe Workfront-Administrator können Sie die Voreinstellungen für Ihr Workfront-System konfigurieren, darunter:

* Zugriff auf Workfront über mobile Apps und andere integrierte Anwendungen
* Regeln zum Einbetten von Workfront in einen iFrame

Änderungen, die Sie an den Systemvoreinstellungen vornehmen, wirken sich auf alle Benutzer in Ihrem System und deren Erlebnis in Workfront aus.

Es wird empfohlen, die Systemvoreinstellungen während der Workfront-Implementierung zu konfigurieren und sie anschließend nur gelegentlich erneut aufzurufen.

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
   <td> <p>Sie müssen Workfront-Administrator sein.</p></td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Systemvoreinstellungen konfigurieren

{{step-1-to-setup}}

1. Klicken Sie im linken Bereich auf **System** > **Voreinstellungen**.

1. Wählen Sie eines der folgenden Felder aus, um die Einstellungen für Ihre Organisation festzulegen:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>Schnellen Release-Prozess aktivieren</p> </td> 
      <td>Ermöglicht die Aktivierung der monatlichen Workfront-Versionen für Ihr Unternehmen anstelle der vierteljährlichen Versionen.</p><p>Weitere Informationen zum Prozess der schnellen Veröffentlichung finden Sie unter <a href="/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md" class="MCXref xref">Schnelle Versionen für Ihr Unternehmen aktivieren oder deaktivieren</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Einbetten von Workfront in einen iFrame zulassen</p> </td> 
      <td>Ermöglicht die Einbettung von Workfront in einen iFrame.<p>Diese Option ist standardmäßig deaktiviert.</p><p><b>WICHTIG</b>: Durch das Anzeigen einer webbasierten Anwendung in einem iframe ist die Anwendung anfällig für eine Sicherheitslücke durch Klickjacking.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">SAML 2.0-Authentifizierung in Office 365-Add-ins zulassen.</td> 
      <td> <p>Hiermit können Sie Workfront nur für Office 365-Add-Ins in einen iframe einbetten, wenn Workfront mit einer SAML 2.0-Single-Sign-On-Lösung integriert ist. </p> <p>Diese Option ist standardmäßig aktiviert.</p> <p><b>HINWEIS</b>: Wenn Sie die obige Option aktivieren, <strong>Einbetten von Workfront in einen iframe zulassen</strong>, ist die Option <strong>SAML 2.0-Authentifizierung in Office 365-Add-Ins zulassen</strong> aktiviert und abgeblendet.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Aktivieren der Verwendung von Sitzungsinformationen beim Erstellen von URLs externer Seiten</td> 
      <td> <p>Ermöglicht Benutzern die Verwendung der Sitzungs-ID-Informationen einer Site beim Hinzufügen einer externen Seite zu einem Dashboard.</p> <p>Diese Option ist unsicher und standardmäßig deaktiviert. Es wird empfohlen, stattdessen OAuth für Integrationen zu verwenden.</p> <p>Weitere Informationen zum Hinzufügen externer Seiten zu einem Dashboard finden Sie unter <a href="../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md" class="MCXref xref">Einbetten einer externen Webseite in ein Dashboard</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Verwenden von Workfronts Mobile Apps und dem Workfront Outlook-Add-In</td> 
      <td> <p>Ermöglicht Benutzern den Zugriff auf die mobilen Apps (Workfront-Ansicht für iPad- und Mobilfunk-Apps) und die Workfront Outlook-App.</p> <p>Diese Option ist standardmäßig aktiviert. </p> <p>Weitere Informationen zur Workfront-Ansicht finden Sie unter <a href="../../../workfront-basics/mobile-apps/using-workfront-view/use-workfront-view.md" class="MCXref xref">Verwenden der Adobe Workfront-Ansicht</a>. Weitere Informationen zu mobilen Apps finden Sie unter <a href="../../../workfront-basics/mobile-apps/using-the-workfront-mobile-app/use-the-mobile-app.md" class="MCXref xref">Verwenden der mobilen Adobe Workfront-App: Artikelindex</a>.</p> <p>Weitere Informationen zum Outlook-Plugin finden Sie unter <a href="../../../workfront-integrations-and-apps/using-workfront-with-outlook/set-up-workfront-for-outlook.md" class="MCXref xref">Einrichten von Adobe Workfront für Outlook</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Zusammenarbeit mit Personen ohne Workfront-Konten mithilfe von E-Mail-Adressen</p> </td> 
      <td>Ermöglicht Benutzern von Workfront, bestimmte Elemente für Personen ohne Workfront-Konto freizugeben, indem sie ihre E-Mail-Adresse anstelle ihres Namens angeben. Benutzer können die folgenden Elemente über ihre E-Mail-Adresse für externe Benutzer freigeben:
       <ul>
        <li>Dokument<br></li>
        <li>Dokumentanfrage<br></li>
        <li>Dokumentenvalidierung</li>
        <li>Kalender</li>
       </ul><p>Diese Option ist standardmäßig aktiviert.</p> <p><b>Wichtig</b>: Die Zugriffsebene externer Benutzer ist in Ihrer Workfront-Instanz nicht verfügbar, wenn diese Option deaktiviert ist. Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/default-access-levels-in-workfront.md" class="MCXref xref">Integrierte Zugriffsebenen</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Externe Benutzer müssen sich mit einem Kennwort registrieren</td> 
      <td> <p>Externe Benutzer müssen sich registrieren, bevor sie Artikel in Workfront anzeigen können. Standardmäßig ist diese Option deaktiviert. Wenn Sie diese Option aktivieren, werden Personen ohne Workfront-Konto, die in bestimmten Aktualisierungen ihrer E-Mail-Adresse enthalten sind, aufgefordert, ein Konto zu erstellen, bevor sie das Element anzeigen können, in dem sie enthalten sind. Dadurch wird ein externes Benutzerkonto für sie erstellt.</p> <p>Diese Option ist standardmäßig deaktiviert.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Benutzer automatisch abmelden nach</td> 
      <td> Hiermit können Sie festlegen, wann ein Benutzer nach einer Inaktivität von Workfront abgemeldet wird. Standardmäßig werden Benutzer nach 8 Stunden Inaktivität abgemeldet. <p>Diese Option betrifft auch Workfront-Kunden, die eine Single Sign-On-Lösung verwenden.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Mobile Benutzer automatisch abmelden nach </td> 
      <td>Hiermit können Sie festlegen, wann ein Benutzer nach einer Inaktivität von der Workfront-Anwendung abgemeldet wird. Standardmäßig werden Benutzer nach 7 Tagen Inaktivität abgemeldet. <p>Diese Option betrifft auch Workfront-Kunden, die eine Single Sign-On-Lösung verwenden.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Hilfe-URL</td> 
      <td>Ermöglicht Ihnen die Definition einer internen benutzerspezifischen Hilfeseite für das Hilfesymbol im Hauptmenü, zu der Sie wechseln können. Weitere Informationen finden Sie unter <a href="/help/quicksilver/administration-and-setup/customize-workfront/brand-workfront/configure-custom-help-url.md">Konfigurieren einer benutzerdefinierten Hilfe-URL</a>.</p></td> 
     </tr>
     <tr> 
      <td role="rowheader">Benutzern im System wird standardmäßig das Erlebnis "Neue Startseite"angezeigt </td> 
      <td>Hiermit können Sie festlegen, ob Benutzern standardmäßig das Erlebnis "Neue Startseite"angezeigt wird. Wenn diese Option aktiviert ist, sehen die Benutzer standardmäßig das Erlebnis "Neues Home", können jedoch weiterhin auf individueller Basis die Option Neues Home aktivieren oder deaktivieren. Wenn diese Option deaktiviert ist, wird Benutzern das Banner nicht angezeigt, über das sie zur neuen Startseite wechseln können. Sie können jedoch dennoch zu ihrer neuen Startseite navigieren, indem sie manuell <code>/home/workspaces</code> am Ende ihrer Instanz-URL eingeben. Diese Einstellung ist standardmäßig aktiviert.</td> 
     </tr>
     <tr> 
      <td role="rowheader">Testumgebungen</td> 
      <td>Ermöglicht Ihnen den Zugriff auf Ihre Workfront-Testumgebungen. Weitere Informationen finden Sie unter <a href="/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md">Die Adobe Workfront-Vorschau-Sandbox-Umgebung</a>.</p></td> 
    </tbody> 
   </table>

1. Klicken Sie auf **Speichern**.

   Die Änderungen, die Sie hier gespeichert haben, wirken sich auf das Erlebnis aller Benutzer in Workfront und aller Benutzer aus, die mit dem System als externer Benutzer interagieren.
