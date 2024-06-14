---
user-type: administrator
product-area: system-administration;setup
navigation-topic: start-with-workfront-administration
title: Grundlegende Informationen für Ihr System konfigurieren
description: Im Rahmen der Konfiguration Ihres Adobe Workfront-Systems können Sie Details zu Ihrem Unternehmen im Abschnitt "Basisinformationen"auf Ihrer Seite "Kundeninformationen"verwalten.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: bad5e700-79a6-49ed-bcf9-f0b5b3eaa909
source-git-commit: 84c5772d130be78d9f9b9aef342c57183d5ec985
workflow-type: tm+mt
source-wordcount: '832'
ht-degree: 1%

---

# Grundlegende Informationen für Ihr System konfigurieren

<!-- Audited: 2/2024 -->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.</p>-->

Im Rahmen der Konfiguration Ihres Adobe Workfront-Systems können Sie Details zu Ihrem Unternehmen im Abschnitt &quot;Basisinformationen&quot;auf Ihrer Seite &quot;Kundeninformationen&quot;verwalten.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Abo</td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td>
   <p>Neu: Standard</p>
   Oder
   <p>Aktuell: Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Sie müssen Workfront-Administrator sein.</p></td> 
  </tr> 
 </tbody> 
</table>

+++

## Auf Kundeninformationen zugreifen

Der Kunde stellt die Workfront-Instanz für Ihr Unternehmen dar. Die Optionen in diesem Bereich sind für Sie als Workfront-Kunde einzigartig.

So greifen Sie auf die Seite &quot;Kundeninformationen&quot;zu:

{{step-1-to-setup}}

1. Klicken Sie im linken Bereich auf **System** > **Kundeninformationen**.

   Je nach dem von Ihnen erworbenen Workfront-Plan fehlen möglicherweise einige Abschnitte auf der Seite &quot;Kundeninformationen&quot;. Wenden Sie sich an Ihren Kundenbetreuer, wenn Sie herausfinden möchten, welchen Workfront-Plan Ihr Unternehmen verwendet.

   Die im Bereich &quot;Kundeninformationen&quot;verfügbaren Abschnitte sind:

   * **Grundlegende Informationen**

     Informationen zum Konfigurieren grundlegender Informationen in Workfront finden Sie unter [Grundlegende Informationen konfigurieren](#configure-basic-info).

   * **API-Schlüsseleinstellungen**

     Informationen zu den API-Schlüsseleinstellungen finden Sie unter [Verwalten von API-Schlüsseln](../../administration-and-setup/manage-workfront/security/manage-api-keys.md).

   * **IP-Zulassungsliste**

     Informationen zum Hinzufügen der IP-Adressen zu Ihrer Zulassungsliste, für die Ihre Benutzer auf Workfront zugreifen können, finden Sie unter [Konfigurieren der Zulassungsliste Ihrer Firewall](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

   * **Lizenz**

     Weitere Informationen zu Lizenzen finden Sie unter [Verwalten der verfügbaren Lizenzen in Ihrem System](../../administration-and-setup/get-started-wf-administration/manage-available-licenses-in-your-system.md).

## Grundlegende Informationen konfigurieren {#configure-basic-info}

Im Bereich &quot;Grundlegende Informationen&quot;Ihrer Seite &quot;Kundeninformationen&quot;werden einige Details zu Ihrem Kunden von Workfront konfiguriert und in einem schreibgeschützten Modus angezeigt. Andere Details können von Ihnen konfiguriert werden. Alle Optionen, die Sie in diesem Bereich bearbeiten können, wirken sich global auf alle Benutzer in Workfront aus.

So konfigurieren Sie Ihren Abschnitt &quot;Grundlegende Informationen&quot;im Bereich &quot;Kundeninformationen&quot;:

{{step-1-to-setup}}

1. Klicken Sie im linken Bereich auf **System** > **Kundeninformationen**.

1. Im **Grundlegende Informationen** -Abschnitt am oberen Rand des **Kundeninformationen** finden Sie die folgenden Informationen zu Ihrer Instanz mit Workfront:

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
      <td> <p>Die E-Mail-Adresse Ihres Workfront-Administrators. Sie können dieses Feld entsprechend der E-Mail-Adresse eines Workfront-Administratoren bearbeiten. Der mit dieser E-Mail-Adresse verknüpfte Benutzer gilt als Workfront-Hauptadministrator Ihres Workfront-Systems. Jede Site-weite Kommunikation von Workfront wird an diese E-Mail-Adresse geleitet. Daher ist es wichtig, sie auf dem neuesten Stand zu halten.</p> <p><b>NOTE</b>: Sie können die Zugriffsebene des mit der Admin-E-Mail verknüpften Benutzers nicht deaktivieren, löschen oder ändern.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Domäne</td> 
      <td> <p>Die Domäne wird von Workfront bei der Erstellung des Kontos festgelegt.</p> <p>Die Domäne identifiziert Ihre eindeutige Subdomäne der URL, die Sie für den Zugriff auf Workfront verwenden.<p>Wenn Ihrem Unternehmen beispielsweise die Domäne "mycompany"zugewiesen wurde, lautet die URL, die Sie für den Zugriff auf Workfront verwenden <i>https://mycompany.my.workfront.com</i></p><p>Sie können die Domäne nicht selbst bearbeiten. Wenn Sie Ihre Domäne ändern möchten, wenden Sie sich an den Workfront-Support. Weitere Informationen zur Kontaktaufnahme mit dem Workfront-Support finden Sie unter <a href="../../workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md" class="MCXref xref">Support kontaktieren</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Zeitzone</td> 
      <td> <p>Dies ist die Standardzeitzone Ihrer Workfront-Instanz. Sie können dieses Feld entsprechend der Zeitzone Ihres primären Workfront-Standorts bearbeiten. Die ausgewählte Zeitzone bestimmt Folgendes: </p> 
       <ul> 
        <li>Datum und Uhrzeit der ausgehenden E-Mails</li> 
        <li>Die Standardzeitzone für neue Benutzer bei ihrer Erstellung</li> 
       </ul> <p>Benutzer können die Zeitzone für ihre Workfront-Instanz unter ihrem Profil ändern. Wenn Benutzer ihre Zeitzone ändern, stimmen Datum und Uhrzeit in ihren E-Mails aus Workfront mit ihren Profilvoreinstellungen überein. Weitere Informationen zum Ändern der Benutzerprofilinformationen finden Sie unter <a href="../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md" class="MCXref xref">Meine Einstellungen konfigurieren</a>. Sie wird bei der Erstellung eines neuen Zeitplans als Standardzeitzone ausgewählt. Weitere Informationen zum Erstellen von Zeitplänen finden Sie unter <a href="../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Zeitplan erstellen</a>.</p> <p>Informationen zur Verwendung von Zeitplänen zur Unterstützung der Zusammenarbeit von Benutzern in Workfront über Zeitzonen hinweg finden Sie unter <a href="../../workfront-basics/tips-tricks-and-troubleshooting/working-across-timezones.md" class="MCXref xref">Arbeiten über Zeitzonen hinweg</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Gebiet</td> 
      <td>Steuert das in ausgehenden E-Mail-Nachrichten verwendete Sprache-, Datums- und Zahlenformat. Das hier ausgewählte Gebietsschema ist das Standardgebietsschema bei der Erstellung neuer Benutzer. Benutzer können ihr Gebietsschema in ihrem Benutzerprofil ändern. Wenn Benutzer ihr Gebietsschema ändern, stimmen Sprache, Datum und Anzahl in ihren E-Mails aus Workfront mit ihren Profilvoreinstellungen überein. Weitere Informationen zum Ändern Ihrer Profilvoreinstellungen finden Sie unter <a href="../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md" class="MCXref xref">Meine Einstellungen konfigurieren</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Speicherquote</td> 
      <td> <p>Dies ist die Menge an Dokumentspeicherplatz, die in Ihrer Workfront-Instanz verfügbar ist.<br>Das Kontingent enthält Dokumente, die Sie direkt in Workfront hochladen.<br>Er umfasst nicht:</p> 
       <ul> 
        <li>Dokumente, die Sie von einem anderen Drittanbieter (SharePoint, Google Drive, Webdam, Box, Dropbox, einem anderen Document Asset Management-Anbieter) mit Workfront verknüpfen.</li> 
        <li>Ihre Workfront-Daten (Projekte, Aufgaben, Probleme, Benutzer usw.).</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Produktversion</td> 
      <td>Dies ist der Typ der Workfront-Instanz, die Ihnen zugewiesen ist. Die Produktversion für die meisten Workfront-Kunden ist <strong>Unternehmen</strong>.</td> 
     </tr> 
    </tbody> 
   </table>

1. Klicken Sie auf **Speichern**.
