---
product-area: timesheets;system-administration
navigation-topic: create-and-manage-timesheets
title: Arbeitszeittabellen-Profile erstellen, bearbeiten und zuweisen
description: Sie können Arbeitszeittabellen-Profile erstellen, bearbeiten und zuweisen, die ohne weiteres Eingreifen von Ihnen wiederkehrende Arbeitszeittabellen für Ihre Benutzer generieren. Dies spart Ihnen Zeit und sorgt für Konsistenz zwischen den Benutzern.
author: Lisa
feature: Timesheets
exl-id: 8f4826bd-82b4-4157-a7d4-a7c94b8fc879
source-git-commit: d7af8c5888147e847b4e239b629373b4b72541f7
workflow-type: tm+mt
source-wordcount: '1695'
ht-degree: 2%

---

# Arbeitszeittabellen-Profile erstellen, bearbeiten und zuweisen

<!--Audited: 06/2025-->

<!--at the Prod release, remove the Production and Preview references from this article-->

<div class="preview">

Die hervorgehobenen Informationen auf dieser Seite beziehen sich auf Funktionen, die noch nicht allgemein verfügbar sind. Sie ist nur in der Vorschau -Umgebung für alle Kunden verfügbar. Dieselben Funktionen werden nach einer Woche ab der Vorschau-Version auch in der Produktionsumgebung für alle Kunden verfügbar sein.

Weitere Informationen finden Sie unter [Schnittstellenmodernisierung](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md).

</div>

Sie können Arbeitszeittabellen-Profile erstellen, bearbeiten und zuweisen, die ohne weiteres Eingreifen von Ihnen wiederkehrende Arbeitszeittabellen für Ihre Benutzer generieren. Dies spart Zeit und stellt sicher, dass Folgendes zwischen den Benutzern konsistent ist:

* Arbeitszeittabellen-Zeitrahmen
* Genehmigende Personen
* Allgemeine Stundentypen

Weitere Informationen zum manuellen Erstellen einer Arbeitszeittabelle finden Sie unter [Erstellen einer Arbeitszeittabelle zur einmaligen Verwendung](../../timesheets/create-and-manage-timesheets/create-tmshts.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
   <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Neu: Standard </p>
 <p>oder</p> 
<p>Aktuell: Plan </p> 
</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Sie müssen administrativen Zugriff auf Arbeitszeittabellen haben. </p> </td> 
  </tr> 
 </tbody> 
</table>

*Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Arbeitszeittabellen-Profil erstellen oder bearbeiten

<!--Old info: 
<div style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p style="color: #ff1493;">Alina drafted an Important note under this heading because Tracy/WorkEx said this is not working as designed - the changes WILL take effect the minute to make them for existing timesheets - see this issue - https://hub.workfront.com/issue/5dba59f600c401cca536567c368aa299/overview</p>
<p style="color: #ff1493;">Important: The changes you make to an existing timesheet profile are not automatically applied to timesheets that have already been generated. The changes you make to a timesheet prile are applied only to the timesheets that are&nbsp;generated after the timesheet profiles changes are made. To&nbsp;apply your&nbsp;changes to the timesheet profile for the timesheets that are already generated, you must delete the existing timesheets and manually generate&nbsp;them.For more information about deleting and manually generating timesheets, see&nbsp;Delete and manually generating Timesheets.</p>
</div>
-->

>[!IMPORTANT]
>
>Um Arbeitszeittabellen-Profiländerungen in aktuellen Arbeitszeittabellen zu aktivieren, müssen Sie zunächst die vorhandenen Arbeitszeittabellen löschen, bevor Sie die Änderungen an den Arbeitszeittabellen-Profilen vornehmen, und dann neue Arbeitszeittabellen erstellen. Anweisungen finden Sie unter [Arbeitszeittabellen in Adobe Workfront löschen](../../timesheets/create-and-manage-timesheets/delete-timesheets.md) und [Arbeitszeittabellen manuell generieren](../../timesheets/create-and-manage-timesheets/manually-generate-timesheets.md).

{{step-1-to-setup}}

1. Wenn Sie ein Arbeitszeittabellen-Profil zur Verwendung im gesamten System erstellen oder bearbeiten, klicken Sie auf **Arbeitszeittabelle und Stunden**.

   Oder

   Wenn Sie ein Arbeitszeittabellen-Profil für eine Gruppe erstellen oder bearbeiten, klicken Sie auf **Gruppen** und dann auf den Namen der Gruppe.

1. Klicken Sie **Arbeitszeittabellen-Profile**.
1. Um ein Arbeitszeittabellen-Profil zu erstellen, klicken Sie auf **Neues Profil**.

   Oder

   Um ein vorhandenes Arbeitszeittabellen-Profil zu bearbeiten, wählen Sie das zu bearbeitende Arbeitszeittabellen-Profil aus und klicken Sie dann auf **Bearbeiten**.

   Die Seite mit dem neuen oder vorhandenen Arbeitszeittabellen-Profil wird angezeigt.


1. Klicken Sie auf **Details festlegen** und aktualisieren Sie dann die folgenden Informationen: <!-- at the Production release, change the order of some of these rows, as they changed in the unshimmed UI-->

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Name</strong> </td> 
      <td> <p> Fügen Sie einen Namen für das Arbeitszeittabellen-Profil hinzu. Dabei kann es sich um den Namen eines Teams oder einer Gruppe handeln, dessen Personen für ihre Arbeitszeittabellen denselben Zeitrahmen verwenden. </p> <p>Dies ist ein Pflichtfeld.</p> </td> 
     </tr>

   <tr> 
      <td role="rowheader"><strong>Beschreibung</strong> </td> 
      <td> <p> Fügen Sie weitere Informationen zum Arbeitszeittabellen-Profil hinzu.     
      </p> </td> 
     </tr>

   <tr> 
   <td role="rowheader"><strong>Gruppe mit Administratorzugriff</strong> </td> 
      <td> <p> 
      <ul> 
      <li> <p>Wenn Sie ein Arbeitszeittabellen-Profil auf Systemebene erstellen, lassen Sie dieses Feld leer.</p> <p>Jeder Benutzer, der Benutzerkonten bearbeiten kann, kann anderen Benutzern eine Arbeitszeittabelle auf Systemebene anhängen.</p> <p>Nur ein Workfront-Administrator kann ein Arbeitszeittabellen-Profil auf Systemebene bearbeiten.</p> </li> 
      </ul> 
     <ul> 
      <li> <p>Wenn Sie ein Arbeitszeittabellen-Profil für eine von Ihnen verwaltete Gruppe erstellen, identifizieren Sie die Gruppe hier.</p> <p>Dadurch wird das Arbeitszeittabellen-Profil nicht den Benutzenden in der Gruppe zugewiesen, sondern nur den Gruppenadministratoren, das Arbeitszeittabellen-Profil zu ändern. Sie weisen das Profil in Schritt 6 Benutzern zu.</p>

   <p><b>HINWEIS</b>: Wenn Benutzende außerhalb der Gruppe Arbeitszeittabellen-Profile an andere Benutzende anhängen, können sie dieses Arbeitszeittabellen-Profil nicht anzeigen oder anhängen.</p> </li> 
      </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Arbeitszeittabellen erstellen</strong> </td> 
      <td> <p> <p>Geben Sie an, wann das Arbeitszeittabellen-Profil die Arbeitszeittabellen generieren soll. Eine Arbeitszeittabelle kann so eingerichtet werden, dass sie automatisch auf wöchentlicher, zweiwöchentlicher, halbmonatlicher oder monatlicher Basis generiert wird. Wählen Sie den Wochentag aus, an dem die Arbeitszeittabelle erstellt werden soll.</p>
      <p>Eine wöchentliche Arbeitszeittabelle beginnt mit dem Datum ihrer Erstellung. Wenn Sie beispielsweise wöchentliche Arbeitszeittabellen jeden Donnerstag erstellen, ist der erste Wochentag auf der Arbeitszeittabelle Donnerstag.</p>


   <p><b>HINWEIS</b>: Workfront erstellt immer zwei Arbeitszeittabellen gleichzeitig: Die erste Arbeitszeittabelle enthält immer das aktuelle Datum, und die zweite Arbeitszeittabelle beginnt, wenn der Zeitrahmen der ersten endet.</p> </p> </td> 
   </tr> 
     <tr> 
      <td role="rowheader"><p><strong>Genehmigende Personen</strong></p> </td> 
      <td> <p> <p>Genehmigende Personen sind Benutzer, die die Arbeitszeittabelle für die mit der Arbeitszeittabelle verbundenen Benutzer genehmigen. Sie können bis zu 7 Benutzer in einer Arbeitszeittabelle als genehmigende Personen angeben. Die Identifizierung mehrerer Benutzer ist nützlich, um sicherzustellen, dass eine genehmigende Person verfügbar ist, wenn jemand abwesend ist. Alle genehmigenden Personen werden benachrichtigt, wenn ein Benutzer die Arbeitszeittabelle zur Genehmigung einreicht. Nur ein Benutzer muss die Arbeitszeittabelle genehmigen, damit sie genehmigt werden kann.</p> <p>Nur Benutzer mit Verwaltungsrechten für Arbeitszeittabellen können als genehmigende Personen festgelegt werden. Weitere Informationen zu Arbeitszeittabellen-Administratorrechten finden Sie unter <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Gewähren von administrativem Zugriff für Benutzer auf bestimmte Bereiche</a>.</p> <p>Wählen Sie im Dropdown-Menü die genehmigende Person für die Arbeitszeittabelle aus (wenn eine genehmigende Person erforderlich ist). Sie können aus den folgenden Optionen auswählen:</p> 
      <ul> 
      <li><strong>Keine</strong>: Die Arbeitszeittabelle muss nicht genehmigt werden.</li> 
      <li><strong>Ihr Manager</strong>: Dies ist die vom System festgelegte standardmäßige genehmigende Person. In diesem Fall genehmigt der als Manager benannte Benutzer die Arbeitszeittabelle, wenn sie zur Genehmigung eingereicht wird.</li> 
      <li><strong>Spezifische Personen</strong> Sie können bestimmte Benutzer bzw. Benutzerinnen nach Namen als Arbeitszeittabellen-Genehmiger bzw. -Genehmigerinnen bestimmen. Eine Arbeitszeittabelle kann mehrere genehmigende Personen enthalten. Wenn eine der genehmigenden Personen die Arbeitszeittabelle genehmigt hat, wird diese als "<strong>" </strong> und verschwindet aus der Liste der Arbeitszeittabellen-Genehmigungen aller verbleibenden genehmigenden Personen.</li> 
       </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Kann </strong> bearbeiten </td> 
      <td> <p> <p>Wählen Sie diese Option aus, damit die genehmigenden Personen Stunden auf der Arbeitszeittabelle bearbeiten können.

   <p>Diese Option funktioniert zusammen mit der Einstellung **Bearbeitung von Arbeitszeittabellen auf Inhaber und Administratoren beschränken** im Bereich Setup &gt; Arbeitszeittabellen und Stunden &gt; Voreinstellungen. Weitere Informationen finden Sie unter <a href="../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md">Arbeitszeittabelle und Stundenvoreinstellungen konfigurieren</a>.</p>

   <p>Die folgenden Szenarien sind vorhanden: </p>

   <ul>
      <li>Wenn die <b>Bearbeitung von Arbeitszeittabellen auf Eigentümer und Administratoren beschränken</b> aktiviert ist:</li>
      <ul><li>Genehmigende Personen können Arbeitszeittabellen nur genehmigen und ablehnen, unabhängig davon, ob <b>Kann Zeit bearbeiten</b> aktiviert ist oder nicht. </li>
      <li>Die Manager der Arbeitszeittabellen-Besitzer können nur die Arbeitszeittabellen ihrer direkt unterstellten Mitarbeiter anzeigen.</li></ul>
      <li>Wenn die <b>Bearbeitung von Arbeitszeittabellen auf Eigentümer und Administratoren beschränken</b> deaktiviert ist:</li>
    <ul><li>Wenn die <b>Kann die Zeit bearbeiten</b> aktiviert ist, können die genehmigenden Personen die Arbeitszeittabelle senden, erneut öffnen oder schließen und die Zeit bearbeiten.</li>
      <li>Wenn die <b>Kann die Zeit bearbeiten</b> deaktiviert ist, können genehmigende Personen die Arbeitszeittabelle nicht senden, erneut öffnen oder schließen und können die Zeit auch nicht bearbeiten. Genehmigende Personen können die Arbeitszeittabelle nur genehmigen oder ablehnen. </li>
      <li>Die Manager von Arbeitszeittabellen-Besitzern können die Arbeitszeittabellen ihrer direkt unterstellten Mitarbeiter senden, zurückrufen, erneut öffnen und bearbeiten.</li></ul>
      </ul>

   <p>

   <b>HINWEIS</b>: Nachdem Sie eine Arbeitszeittabelle zur Genehmigung eingereicht haben, können Sie die Stunden nicht mehr bearbeiten. Um eine übermittelte Arbeitszeittabelle in den bearbeitbaren Status zurückzuversetzen, rufen Sie die Arbeitszeittabelle zurück oder bitten Sie die genehmigende Person, die Arbeitszeittabelle abzulehnen. Weitere Informationen finden Sie unter <a href="../../timesheets/create-and-manage-timesheets/submit-timesheet-for-approval.md">Arbeitszeittabelle zur Genehmigung einreichen</a> und <a href="../../timesheets/create-and-manage-timesheets/timesheet-approvals.md">Arbeitszeittabelle genehmigen</a>.</p> </p> </td>
   </tr> 
     <tr> 
      <td role="rowheader"><strong>Verfügbare Stundentypen</strong> </td> 
      <td><p>Diese Einstellung bezieht sich nur auf allgemeine Stundentypen und nicht auf projektspezifische Stundentypen. </p>
      <p>Standardmäßig sehen Benutzer alle allgemeinen Stunden auf einer Arbeitszeittabelle. Wenn Ihr Unternehmen jedoch möchte, dass nur bestimmte allgemeine Stunden für eine bestimmte Benutzergruppe angezeigt werden, können Sie die allgemeinen Stunden auswählen, die in den Arbeitszeittabellen angezeigt werden sollen, indem Sie sie in diesem Feld in ihrem Arbeitszeittabellen-Profil auswählen. Wenn Sie alle allgemeinen Stunden deaktivieren möchten, heben Sie die Auswahl aller Stundentypen auf, um die Arbeitszeittabelle ohne Abschnitt für allgemeine Stunden zu erstellen.</p></td> 
     </tr>

   <tr> 
      <td role="rowheader"><strong>Erinnerungsnachrichten</strong> </td> 
      <td> <p> Erinnerungsnachricht hinzufügen. Workfront sendet Benutzern Erinnerungen, damit diese ihre Arbeitszeittabellen ausfüllen oder genehmigen können. Sie müssen Erinnerungsnachrichten erstellen, bevor Sie sie mit einem Arbeitszeittabellen-Profil verknüpfen können.  </p> </td> 
     </tr>

   <tr data-mc-conditions=""> 
      <td role="rowheader"><span style="font-weight: bold;">Überstunden</span> </td> 
      <td>Sie können das Feld „Überstunden“ in den Arbeitszeittabellen ausblenden. Standardmäßig ist diese Option deaktiviert.</td> 
     </tr> 
    </tbody> 
    </table>

1. Klicken Sie in der Produktionsumgebung oder beim Erstellen von Arbeitszeittabellenprofilen auf Gruppenebene auf die Registerkarte **Personen zuweisen**, um das Arbeitszeittabellenprofil mit bestimmten Benutzenden, Gruppen oder (wenn Sie Workfront-Administrator sind) Teams zu verknüpfen. <!--Keep the reference to the group upon release to Prod, for now, until they unshim the group Timesheet Profiles-->

   <span class="preview">Scrollen Sie in der Vorschau-Umgebung beim Erstellen von Arbeitszeittabellen-Profilen für das System nach unten auf der Seite und suchen Sie den Abschnitt **Personen zuweisen**.</span> <!--Keep the reference to the system when releasing to Prod, until they unshim the group Timesheet Profile-->

   Beginnen Sie mit der Eingabe des Namens des Benutzers, der Gruppe oder des Teams und klicken Sie dann auf den Namen, wenn er in der Dropdown-Liste angezeigt wird.

   Wenn Sie Gruppenadministrator sind, können Sie das Arbeitszeittabellen-Profil Gruppen zuweisen, die Sie verwalten, jedoch nicht Teams. Weitere Informationen finden Sie unter [ für einen Gruppenadministrator beim Zuweisen eines Arbeitszeittabellen-Profils ](#limitations-for-a-group-administrator-assigning-a-timesheet-profile) diesem Artikel.

   >[!NOTE]
   >
   >* Sie können einen Benutzer auch mit einem Arbeitszeittabellen-Profil verknüpfen, indem Sie das Benutzerprofil bearbeiten. Weitere Informationen finden Sie [Bearbeiten des Benutzerprofils](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).
   >* Wenn Sie eine Gruppe hinzufügen, wird nur der Gruppenname auf der Registerkarte Personen zuweisen angezeigt, nicht die Liste der Gruppenmitglieder. Wenn Sie die hier aufgeführten Gruppenmitglieder sehen möchten, klicken Sie auf Änderungen speichern und dann auf den Namen des soeben erstellten Arbeitszeittabellen-Profils.
   >* Wenn Sie diese Schritte abgeschlossen haben, generiert das Arbeitszeittabellen-Profil Arbeitszeittabellen nur für die zugewiesenen Benutzer oder Gruppenmitglieder, die für den aktuellen Zeitraum keine Arbeitszeittabellen haben.

1. Klicken Sie auf **Speichern**.

1. Klicken Sie oben in der Liste der Arbeitszeittabellen-Profile auf das Symbol **Mehr** ![Mehr](assets/more-icon.png) für Arbeitszeittabellen-Profile auf Systemebene oder **Mehr** für Arbeitszeittabellen-Profile und klicken Sie dann auf **Arbeitszeittabellen erstellen**.

   Unten im Bildschirm wird eine Bestätigung angezeigt, dass Arbeitszeittabellen erfolgreich generiert wurden. Neue Arbeitszeittabellen werden auf der Grundlage der von Ihnen erstellten neuen Profile generiert.

   Weitere Informationen finden Sie unter [Arbeitszeittabellen manuell generieren](/help/quicksilver/timesheets/create-and-manage-timesheets/manually-generate-timesheets.md).

   Wenn das Arbeitszeittabellen-Profil zum ersten Mal Arbeitszeittabellen generiert, werden für jeden Benutzer zwei Arbeitszeittabellen erstellt, und zwar sowohl für den Zeitrahmen, der die aktuelle Zeit enthält, als auch für den folgenden Zeitrahmen.

   Danach wird jedes Mal, wenn neue Arbeitszeittabellen erstellt werden, eine Arbeitszeittabelle pro Benutzer erstellt.

   <!--the content in the table above will need to match the content in the Create timesheets article-->

## Einschränkungen für die Zuweisung eines Arbeitszeittabellen-Profils durch einen Gruppenadministrator {#limitations-for-a-group-administrator-assigning-a-timesheet-profile}

Wenn Sie Gruppenadministrator sind und die Zugriffsoption „Arbeitszeittabellen und Stunden“ auf Ihrer Zugriffsebene deaktiviert ist, können Sie Arbeitszeittabellen-Profile erstellen, diese jedoch nur folgenden Benutzern zuweisen:

* Von Ihnen verwaltete Gruppen
* Einzelne Benutzende, die Sie bearbeiten können und die sich in einer von Ihnen verwalteten Gruppe befinden

Für diese Gruppen und Benutzer haben Sie keinen Zugriff auf die Arbeitszeittabellen, die das Arbeitszeittabellen-Profil generiert.

Wenn außerdem die Option Benutzerverwaltung (Gruppenbenutzer) auf Ihrer Zugriffsebene deaktiviert ist, können Sie das Arbeitszeittabellen-Profil einer von Ihnen verwalteten Gruppe zuweisen, dies wirkt sich jedoch nur auf die Benutzer in der Gruppe aus, auf die Sie Zugriff haben, um es zu bearbeiten. Wenn die Gruppe Benutzer enthält, auf die Sie keinen Zugriff haben, um sie zu bearbeiten, wird ihnen das Arbeitszeittabellen-Profil nicht zusammen mit dem Rest der Gruppe zugewiesen.

Informationen zur Option Arbeitszeittabellen und Stunden in Ihrer Zugriffsebene finden Sie unter [Gewähren von administrativem Zugriff für Benutzer auf bestimmte Bereiche](../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

Informationen zur Option Benutzeradmin. (Gruppenbenutzer) in Ihrer Zugriffsebene finden Sie unter [Gewähren des Zugriffs für Benutzer](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

## Mehrere wiederkehrende Arbeitszeittabellen-Profile

Sie können über mehr als ein Arbeitszeittabellen-Profil für Ihre Organisation verfügen, wenn Folgendes zutrifft:

* Eindeutige Zahlungszeiträume für verschiedene Benutzergruppen
* Eindeutige genehmigende Personen für verschiedene Benutzergruppen
* Eindeutige allgemeine Stundenanforderungen für verschiedene Benutzergruppen

Ein Benutzer kann nicht gleichzeitig mit mehr als einem Arbeitszeittabellen-Profil verknüpft werden.
