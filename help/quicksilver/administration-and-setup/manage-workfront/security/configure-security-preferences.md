---
user-type: administrator
product-area: system-administration;user-management;setup
navigation-topic: security
title: Systemsicherheitsvoreinstellungen konfigurieren
description: Als Adobe Workfront-Administrator können Sie Sicherheitseinstellungen für Ihr Workfront-System konfigurieren.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: f92ceed7-b191-425b-9fff-1b0947f32db8
source-git-commit: 04cf9d37c681398f5a0e2b9d7d45c0f8b93ab44b
workflow-type: tm+mt
source-wordcount: '709'
ht-degree: 5%

---

# Systemsicherheitsvoreinstellungen konfigurieren

<!--
DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.</p>
-->

{{important-admin-console-onboard}}

Als Adobe Workfront-Administrator können Sie Sicherheitseinstellungen für Ihr Workfront-System konfigurieren:

* Zugriff auf Workfront über mobile Apps und andere integrierte Anwendungen
* Regeln zum Einbetten von Workfront in einen iFrame

Änderungen, die Sie an den Systemvoreinstellungen vornehmen, wirken sich auf alle Benutzer in Ihrem System und deren Erlebnis in Workfront aus.

Es wird empfohlen, die Sicherheitseinstellungen des Systems während der Workfront-Implementierung zu konfigurieren und diese anschließend nur gelegentlich erneut aufzurufen.

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

## Systemsicherheitsvoreinstellungen konfigurieren

1. Klicken Sie auf **Hauptmenü** icon ![](assets/main-menu-icon.png) Klicken Sie oben rechts in Adobe Workfront auf **Einrichtung** ![](assets/gear-icon-settings.png).

1. Klicken Sie im linken Bereich auf **System** > **Voreinstellungen**.

1. Im **Sicherheit** Wählen Sie eines der folgenden Felder aus, um die Sicherheitseinstellungen für Ihr Unternehmen festzulegen:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>Einbetten von <strong>Workfront</strong> in einem iFrame</p> </td> 
      <td>Ermöglicht die Einbettung von Workfront in einen iFrame.<p>Diese Option ist standardmäßig deaktiviert.</p><p><b>WICHTIG</b>: Durch die Anzeige einer webbasierten Anwendung in einem iframe ist die Anwendung anfällig für eine Clickjacking-Sicherheitslücke.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">SAML 2.0-Authentifizierung in Office 365-Add-ins zulassen.</td> 
      <td> <p>Hiermit können Sie Workfront nur für Office 365-Add-Ins in einen iframe einbetten, wenn Workfront mit einer SAML 2.0-Single-Sign-On-Lösung integriert ist. </p> <p>Diese Option ist standardmäßig aktiviert.</p> <p><b>NOTE</b>: Wenn Sie die obige Option aktivieren, <strong>Einbetten von Workfront in einen iFrame zulassen</strong>, die Option <strong>SAML 2.0-Authentifizierung in Office 365-Add-Ins zulassen</strong> aktiviert und abgeblendet ist.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Beim Erstellen von URLs für externe Seiten die Verwendung von Sitzungsinformationen aktivieren</td> 
      <td> <p>Ermöglicht Benutzern die Verwendung der Sitzungs-ID-Informationen einer Site beim Hinzufügen einer externen Seite zu einem Dashboard.</p> <p>Weitere Informationen zum Hinzufügen externer Seiten zu einem Dashboard finden Sie unter <a href="../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md" class="MCXref xref">Einbetten einer externen Webseite in ein Dashboard</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Lassen Sie die Benutzer die mobilen Anwendungen von Workfront und die <strong>Workfront</strong> Outlook-Add-In</td> 
      <td> <p>Ermöglicht Benutzern den Zugriff auf die mobilen Apps (Workfront-Ansicht für iPad- und Mobilfunk-Apps) und die Workfront Outlook-App.</p> <p>Diese Option ist standardmäßig aktiviert. </p> <p>Weitere Informationen zur Workfront-Ansicht finden Sie unter <a href="../../../workfront-basics/mobile-apps/using-workfront-view/use-workfront-view.md" class="MCXref xref">Adobe Workfront-Ansicht verwenden</a>. Weitere Informationen zu Mobile Apps finden Sie unter <a href="../../../workfront-basics/mobile-apps/using-the-workfront-mobile-app/use-the-mobile-app.md" class="MCXref xref">Verwenden der mobilen Adobe Workfront-App</a>.</p> <p>Weitere Informationen zum Outlook-Plugin finden Sie unter <a href="../../../workfront-integrations-and-apps/using-workfront-with-outlook/set-up-workfront-for-outlook.md" class="MCXref xref">Einrichten von Adobe Workfront für Outlook</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Zusammenarbeit mit Personen ohne Workfront-Konten mithilfe von E-Mail-Adressen</p> </td> 
      <td>Ermöglicht Benutzern von Workfront, bestimmte Elemente für Personen ohne Workfront-Konto freizugeben, indem sie ihre E-Mail-Adresse anstelle ihres Namens angeben. Benutzer können die folgenden Elemente über ihre E-Mail-Adresse für externe Benutzer freigeben:
       <ul>
        <li>Dokument<br></li>
        <li>Dokumentanfrage<br></li>
        <li>Dokumentenvalidierung</li>
        <li>Kalender</li>
       </ul><p>Diese Option ist standardmäßig aktiviert.</p> <p><b>Wichtig</b>: Die Zugriffsebene externer Benutzer ist in Ihrer Workfront-Instanz nicht verfügbar, wenn diese Option deaktiviert ist. Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/default-access-levels-in-workfront.md" class="MCXref xref">Integrierte Zugriffsebenen in Workfront</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Externe Benutzer auffordern, sich mit einem Kennwort zu registrieren</td> 
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
    </tbody> 
   </table>

1. Klicken Sie auf **Speichern**.

   Die hier gespeicherten Änderungen wirken sich auf das Erlebnis aller Benutzer in Workfront und aller Benutzer aus, die mit ihnen als externer Benutzer interagieren.
