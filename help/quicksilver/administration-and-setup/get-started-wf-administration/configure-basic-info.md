---
user-type: administrator
product-area: system-administration;setup
navigation-topic: start-with-workfront-administration
title: Konfigurieren grundlegender Informationen für Ihr System
description: Im Rahmen der Konfiguration Ihres Adobe Workfront-Systems können Sie im Abschnitt Grundlegende Informationen auf der Seite Kundeninformationen Details zu Ihrem Unternehmen verwalten.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: bad5e700-79a6-49ed-bcf9-f0b5b3eaa909
source-git-commit: 01a80f6140650ca12aaee14115f79449dcfa2a18
workflow-type: tm+mt
source-wordcount: '805'
ht-degree: 4%

---

# Grundlegende Systeminformationen konfigurieren

<!-- Audited: 2/2024 -->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.</p>-->

Im Rahmen der Konfiguration Ihres Adobe Workfront-Systems können Sie im Abschnitt Grundlegende Informationen auf der Seite Kundeninformationen Details zu Ihrem Unternehmen verwalten.

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Workfront-Paket</td> 
   <td><p>Beliebig</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td><p>Standard</p> <p>Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td>Sie müssen ein Workfront-Administrator sein. </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Zugriff auf Kundeninformationen

Der Kunde stellt die Workfront-Instanz für Ihr Unternehmen dar. Die Optionen in diesem Bereich sind für Sie als Kunde von Workfront einzigartig.

So greifen Sie auf die Seite „Kundeninformationen“ zu:

{{step-1-to-setup}}

1. Klicken Sie im linken Bedienfeld auf **System** > **Kundeninformationen**.

   Je nach dem von Ihnen erworbenen Workfront-Paket fehlen möglicherweise einige Abschnitte auf der Seite „Kundeninformationen“. Wenden Sie sich an Ihren Kundenbetreuer, wenn Sie herausfinden möchten, welches Workfront-Paket Ihr Unternehmen verwendet.

   Die folgenden Abschnitte sind im Bereich „Kundeninformationen“ verfügbar:

   * **Grundlegende Informationen**

     Informationen zum Konfigurieren grundlegender Informationen in Workfront finden Sie unter [Konfigurieren grundlegender Informationen](#configure-basic-info).

   * **API-Schlüsseleinstellungen**

     Informationen zu API-Schlüsseleinstellungen finden Sie unter [Verwalten von API-Schlüsseln](../../administration-and-setup/manage-workfront/security/manage-api-keys.md).

   * **IP-Zulassungsliste**

     Informationen zum Hinzufügen der IP-Adressen zu Ihrer Zulassungsliste, über die Ihre Benutzer auf Workfront zugreifen können, finden Sie [Zulassungsliste Ihrer Firewall konfigurieren](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

   * auf die Zulassungsliste setzen **E-Mail**

     Informationen zum Hinzufügen von E-Mails zu Ihrer Zulassungsliste auf die Zulassungsliste setzte finden Sie unter [Konfigurieren Ihrer E-Mail-](/help/quicksilver/administration-and-setup/get-started-wf-administration/configure-your-email-allowlist.md).

   <!--
   * **License**

     For information about licenses, see [Manage available licenses in your system](../../administration-and-setup/get-started-wf-administration/manage-available-licenses-in-your-system.md).-->

## Konfigurieren grundlegender Informationen {#configure-basic-info}

Im Bereich Grundlegende Informationen auf der Seite Kundeninformationen werden einige Details zu Ihrem Kunden von Workfront konfiguriert und in einem schreibgeschützten Modus angezeigt. Andere Details können von Ihnen konfiguriert werden. Alle Optionen, die Sie in diesem Bereich bearbeiten können, haben globale Auswirkungen auf alle Benutzenden in Workfront.

So konfigurieren Sie den Abschnitt „Allgemeine Informationen“ im Bereich „Kundeninformationen“:

{{step-1-to-setup}}

1. Klicken Sie im linken Bedienfeld auf **System** > **Kundeninformationen**.

1. Im Abschnitt **Grundlegende Informationen** oben auf der Seite **Kundeninformationen** finden Sie die folgenden Informationen zu Ihrer Instanz mit Workfront:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Name</td> 
      <td>Der Name Ihres Unternehmens, der auch mit dem Namen Ihres Unternehmens übereinstimmt. Dieser wird von Workfront hinzugefügt und kann nicht bearbeitet werden.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Cluster-Setup </td> 
      <td>Die Cluster-Nummer für Ihre Instanz.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Admin-E-Mail</td> 
      <td> <p>Die E-Mail-Adresse Ihres Workfront-Administrators. Sie können dieses Feld so bearbeiten, dass es mit der E-Mail-Adresse eines Workfront-Administrators übereinstimmt. Der mit dieser E-Mail-Adresse verknüpfte Benutzer wird als Hauptadministrator von Workfront in Ihrem Workfront-System betrachtet. Jede Site-weite Kommunikation von Workfront wird an diese E-Mail-Adresse geleitet, daher ist es wichtig, sie auf dem neuesten Stand zu halten.</p> <p><b>HINWEIS</b>: Sie können die Zugriffsebene der Benutzenden, die mit der Admin-E-Mail verknüpft sind, nicht deaktivieren, löschen oder ändern.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Domain</td> 
      <td> <p>Die Domain wird von Workfront bei der Kontoerstellung festgelegt.</p> <p>Die Domain identifiziert Ihre eindeutige Subdomain der URL, die Sie für den Zugriff auf Workfront verwenden.<p>Wenn Ihrem Unternehmen beispielsweise die Domain „mycompany“ zugewiesen wurde, lautet die URL für den Zugriff auf Workfront <i>https://mycompany.my.workfront.com.</i></p><p>Sie können die Domain nicht selbst bearbeiten. Wenn Sie Ihre Domain ändern möchten, können Sie sich an den Workfront-Support wenden. Weitere Informationen zur Kontaktaufnahme mit dem Workfront-Support finden Sie unter <a href="../../workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md" class="MCXref xref">Kundensupport kontaktieren</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Zeitzone</td> 
      <td> <p>Dies ist die Standardzeitzone Ihrer Workfront-Instanz. Sie können dieses Feld so bearbeiten, dass es der Zeitzone Ihres primären Workfront-Standorts entspricht. Die ausgewählte Zeitzone bestimmt Folgendes: </p> 
       <ul> 
        <li>Datum und Uhrzeit, die in ausgehenden E-Mails angezeigt werden</li> 
        <li>Die standardmäßige Zeitzone für neue Benutzer bei deren Erstellung</li> 
       </ul> <p>Benutzer können die Zeitzone für ihre Workfront-Instanz unter ihrem Profil ändern. Wenn Benutzende ihre Zeitzone ändern, entsprechen Datum und Uhrzeit in ihren E-Mails aus Workfront ihren Profilvoreinstellungen. Weitere Informationen zum Ändern der Benutzerprofileinstellungen finden Sie unter <a href="../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md" class="MCXref xref">Konfigurieren meiner Einstellungen</a>. Sie wird beim Erstellen eines neuen Zeitplans als Standardzeitzone ausgewählt. Weitere Informationen zum Erstellen von Zeitplänen finden Sie unter <a href="../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Erstellen eines Zeitplans</a>.</p> <p>Informationen zur Verwendung von Zeitplänen für die Zusammenarbeit in Workfront über Zeitzonen hinweg finden Sie <a href="../../workfront-basics/tips-tricks-and-troubleshooting/working-across-timezones.md" class="MCXref xref">Arbeiten über Zeitzonen hinweg</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Standard-Gebietsschema für E-Mail</td> 
      <td>Steuert die Sprache, das Datum- und das Zahlenformat, die in ausgehenden E-Mail-Nachrichten verwendet werden. Das hier ausgewählte Gebietsschema ist der Standard, wenn neue Benutzer erstellt werden. Benutzer können ihr Gebietsschema in ihrem Benutzerprofil ändern. Wenn Benutzende ihr Gebietsschema ändern, entsprechen die Sprache, das Datum und das Zahlenformat in ihren E-Mails aus Workfront ihren Profilvoreinstellungen. Weitere Informationen zum Ändern Ihrer Profilvoreinstellungen finden Sie unter <a href="../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md" class="MCXref xref">Konfigurieren meiner Einstellungen</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Speicherquote</td> 
      <td> <p>Dies ist der Umfang des in Ihrer Workfront-Instanz verfügbaren Dokumentenspeichers.<br>Das Kontingent enthält Dokumente, die Sie direkt in Workfront hochladen.<br>Sie umfasst nicht:</p> 
       <ul> 
        <li>Dokumente, die Sie von einem anderen Drittanbieter (SharePoint, Google Drive, Webdam, Box, Dropbox oder einem anderen Anbieter von Document Asset Management) mit Workfront verknüpfen.</li> 
        <li>Ihre Workfront-Daten (Projekte, Aufgaben, Probleme, Benutzer usw.).</li> 
       </ul> </td> 
     </tr>
    </tbody> 
   </table>

1. Klicken Sie auf **Speichern**.
