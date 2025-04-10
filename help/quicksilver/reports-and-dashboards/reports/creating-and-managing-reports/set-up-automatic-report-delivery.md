---
product-area: reporting;setup
navigation-topic: create-and-manage-reports
title: Planen eines automatischen Berichtversands
description: Planen eines automatischen Berichtversands
author: Courtney
feature: Reports and Dashboards
exl-id: 5b8e382c-bfe8-43aa-aa09-a2aa0c4d56cc
source-git-commit: f78a86dcdf7b63e98bec5216fb5ab7622775a053
workflow-type: tm+mt
source-wordcount: '1268'
ht-degree: 2%

---

# Planen eines automatischen Berichtversands

<!-- Audited: 4/2025 -->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: If this stays, fix links which now go to the reference article)</p>
-->

Sie können Berichte so planen, dass sie automatisch nach einem festgelegten Zeitplan an die Benutzer gesendet werden, oder Sie können Berichte manuell einmal senden. Wenn Sie einen Bericht über Adobe Workfront senden, erhält der/die Benutzende eine E-Mail mit dem Workfront-Bericht in einer separaten Anlage.

Weitere Informationen, einschließlich Größenbeschränkungen, die sich auf die Bereitstellung Ihrer Berichte auswirken können, finden Sie unter [Übersicht über die Berichtsbereitstellung](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
      <td> 
      <p>Neu: Standard</p>
      <p>Oder</p>

<p>Aktuell: Plan</p>

</td>
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriff auf Berichte, Dashboards, Kalender bearbeiten</p> <p>Zugriff auf Filter, Ansichten, Gruppierungen bearbeiten</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Verwalten von Berechtigungen für einen Bericht</p></td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Voraussetzungen

Bevor Sie beginnen, müssen Sie einen Bericht erstellen. Weitere Informationen zum Erstellen von Berichten finden Sie unter [Erstellen eines benutzerdefinierten Berichts](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

## Planen eines Berichtversands


So planen Sie einen Bericht für den automatischen Versand&#x200B;

{{step1-to-reports}}

>[!NOTE]
>
>Berichtsendungen enthalten keine Eingabeaufforderungen. Wenn Sie die Daten eines Berichtsversands einschränken möchten, empfehlen wir, Filter auf den Bericht anzuwenden, den Sie senden möchten.

1. Wählen Sie auf **Seite** einen Bericht aus.
1. Klicken Sie oben im Bildschirm in der angezeigten Dropdown **Liste auf** Berichtsaktionen **und dann** Bericht senden“. Das **Bericht senden** wird angezeigt.

   >[!TIP]
   >
   >Wenn Sie einen Bericht jederzeit manuell senden möchten, gehen Sie zum Bericht und klicken Sie auf **Berichtsaktionen** > **Bericht senden** > **Jetzt senden**.

1. Wählen Sie die **Wiederholte Sendungen** aus.
1. (Bedingt) Um einen vorhandenen sich wiederholenden Berichtversand zu ändern, wählen Sie den **im Abschnitt** Sende-Wiederholung) auf der rechten Seite des Dialogfelds aus.
1. Geben Sie die folgenden Informationen an:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>Senden an</p> </td> 
      <td> <p>Geben Sie zunächst den Namen des Benutzers, der Gruppe, des Teams oder der Rolle ein, an den bzw. die Sie den Bericht senden möchten, und klicken Sie dann auf den Namen, wenn er in der Dropdown-Liste angezeigt wird.</p> <p>Oder</p> <p>Geben Sie die E-Mail-Adresse einer Person außerhalb des Workfront-Systems ein, der Sie Zugriff auf den Bericht gewähren möchten.</p> <p>Wiederholen Sie diesen Vorgang, um den Bericht an mehrere Benutzer, Gruppen, Teams oder Rollen zu senden.</p> <p>Hinweis:  <p>Beachten Sie beim Hinzufügen von Berichtsversand-Empfängern Folgendes:</p> 
        <ul> 
         <li>Wenn Ihr Unternehmen Workfront-Benachrichtigungen auf bestimmte E-Mail-Domains beschränkt, können Sie Berichte möglicherweise nur an die in der E-Mail-Zulassungsliste aufgeführten E-Mail-Adressen senden.<p>Informationen dazu, wie Workfront-Admins die E-Mail-Zulassungsliste auf die Zulassungsliste setzte aktualisieren, finden Sie im Abschnitt <a href="../../../administration-and-setup/get-started-wf-administration/configure-your-email-allowlist.md#configur" class="MCXref xref">Konfigurieren Ihrer E-Mail</a>.</p></li> 
         <li> <p>Wenn Sie als Empfänger eine große Anzahl von Benutzern hinzufügen, kann dies zum Fehlschlagen des Versands führen. Wenn der Versand fehlschlägt, können Sie mehrere Berichtsendungen mit kleineren Benutzergruppen planen.</p> </li> 
        </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>E-Mail-Betreff</p> </td> 
      <td> <p>Geben Sie einen Betreff für die E-Mail-Benachrichtigung ein.</p> <p>Standardmäßig lautet der Betreff der E-Mail:</p> <p><em>Workfront-Bericht: [Name des Berichts] [Datum]</em> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>E-Mail-Nachricht</p> </td> 
      <td> <p>Geben Sie eine Nachricht ein, die in die E-Mail aufgenommen werden soll.</p> <p>Standardmäßig lautet die E-Mail-Nachricht:</p> <p><em>Beigefügt ist der am [Datum] von Workfront generierte [Berichtshäufigkeit] Bericht [Name des Berichts].</em> </p> <p>Hinweis: Bei Berichten, die nur als Excel-Datei bereitgestellt werden, wird der E-Mail die folgende Meldung hinzugefügt: „Beachten Sie, dass es bei MS Excel (XLS)-Dateitypen eine Begrenzung (65.530) für die Anzahl der Hyperlinks gibt, die diese Dateitypen unterstützen. Wenn Sie diese Beschränkungen überschreiten, wird die Datei nicht geöffnet. Es wird empfohlen, einen erneuten Sendeversuch ohne die Hyperlinks durchzuführen. Bitte kehren Sie zum Berichtplaner zurück, um die Hyperlinks zu entfernen, und senden Sie den Bericht erneut.“ Die Phrase „Zurück zur Berichtsplanung“ ist ein Link zurück zum Bericht.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Diesen Bericht senden mit Zugriffsrechten von</p> </td> 
      <td> <p>Geben Sie den Namen eines Benutzers ein, der Zugriff auf den Bericht hat, und klicken Sie dann auf den Namen, wenn er in der Dropdown-Liste angezeigt wird. Benutzern, die den Bericht erhalten, wird derselbe Zugriff auf den Bericht gewährt wie den Benutzern, die Sie hier angeben.<br> Informationen finden Sie unter <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/run-deliver-report-access-rights-another-user.md" class="MCXref xref">Bericht mit den Zugriffsrechten eines anderen Benutzers ausführen und bereitstellen</a>.</p> <p>Hinweis: Dieses Feld unterstützt keine Platzhalter. Beispielsweise wird bei Verwendung des Platzhalters <em>$$User.ID</em> der Bericht nicht mit den Zugriffsrechten des Benutzers ausgeführt, der den Bericht erhält.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Format</p> </td> 
      <td> <p>Wählen Sie das gewünschte Format für den zugestellten Bericht aus:</p> 
       <ul> 
        <li> <p>HTML</p> </li> 
        <li> <p>PDF</p> <p>Wenn Sie PDF auswählen, können Sie die Ausgabe mit den zusätzlichen Optionen <strong>Papiergröße</strong> und <strong>Ausrichtung</strong> formatieren.</p> </li> 
        <li> <p>MS Excel (.xlsx)</p> </li> 
        <li> <p>TSV</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Links einbeziehen</p> </td> 
      <td> <p>Diese Option ist nur verfügbar, wenn <strong>MS Excel</strong> im Dropdown-Menü <strong>Format</strong> ausgewählt ist. Wenn diese Option aktiviert ist, werden alle Hyperlinks in das exportierte Excel-Dokument eingefügt.</p> <p>Dokumente mit mehr als 65.530 Links können nicht geöffnet werden. Deaktivieren Sie diese Option, wenn das exportierte Dokument mehr als 65.530 Links enthalten soll.</p> <p>Diese Option ist standardmäßig aktiviert.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Zusammenfassung</p> </td> 
      <td> <p>Zeigt eine Zusammenfassung der Wiederholung des Versands an.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Wiederholungen</p> </td> 
      <td> <p>Wählen Sie aus, ob der Bericht täglich, wöchentlich, monatlich oder jährlich bereitgestellt werden soll.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Wiederholung alle</p> </td> 
      <td> <p>Wählen Sie die Häufigkeit aus, mit der der Versand wiederholt werden soll. Der Wert, den Sie für diese Option auswählen, basiert auf der Option, die in der Dropdown-Liste <strong>Wiederholungen</strong> ausgewählt wurde.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Uhrzeit</p> </td> 
      <td> <p>Wählen Sie die Tageszeit für den Versand aus.</p> <p>Tipp: Da sich Systemlasten auf die Bereitstellungszeiten von Berichten auswirken können, kann es zu einer Verzögerung von bis zu 24 Stunden zwischen der geplanten Zeit und der tatsächlichen Bereitstellungszeit kommen. Wenn Sie einen Bericht benötigen, der zu einem bestimmten Zeitpunkt geliefert werden soll, empfehlen wir, den Versand vor dem erforderlichen Zeitpunkt zu planen. Im Allgemeinen empfehlen wir, den Versand mindestens einen Tag vor dem erforderlichen Datum zu planen.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Wiederholung am</p> </td> 
      <td> <p>Diese Option ist verfügbar, wenn die Option <strong>Wiederholen</strong> entweder auf <strong>Wöchentlich</strong> oder <strong>Monatlich </strong>:</p> 
       <ul> 
        <li> <p>Wenn die Option <strong>Wiederholungen</strong> auf <strong>Wöchentlich</strong> gesetzt ist: Wählen Sie die Wochentage aus, an denen der Versand durchgeführt wird.</p> </li> 
        <li> <p>Wenn die Option <strong>Wiederholen</strong> auf <strong>Monatlich</strong> festgelegt ist: Wählen Sie aus, ob der Versand am Tag des Monats, am Wochentag oder am letzten Tag des Monats durchgeführt werden soll (diese Optionen nutzen das Datum, das Sie im Feld <strong>Starts am</strong> auswählen).</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Beginnt am</p> </td> 
      <td>Wählen Sie das Datum aus, an dem der geplante Versand beginnen soll.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>endet am</p> </td> 
      <td>Wählen Sie ein Enddatum für den geplanten Versand aus.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Nie</p> </td> 
      <td>Wählen <strong>Nie</strong>, wenn der geplante Versand unbegrenzt dauern soll.</td> 
     </tr> 
    </tbody> 
   </table>

1. Klicken Sie **Speichern**, um den Berichtsversand zu speichern. Der Bericht wird im Abschnitt **Sende** des Dialogfelds **Bericht senden** angezeigt und zum geplanten Zeitpunkt gesendet.

   Informationen zu Größenbeschränkungen, die sich auf die Bereitstellung Ihrer Berichte auswirken können, finden Sie in den Abschnitten [Berichtsbereitstellungsbeschränkungen](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md#understanding-export-limits) und [Exportbeschränkungen](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md#export).

>[!IMPORTANT]
>
>Terminierte Berichte unterliegen einem internen Zeitlimit, wenn sie für die Bereitstellung verarbeitet werden. Sollte ein Bericht länger als zulässig dauern, erhalten Sie eine Benachrichtigung, und der Bericht wird unabhängig von den verbleibenden geplanten Sendungen nicht mehr zugestellt. Um den Versand des Berichts fortzusetzen, reduzieren Sie zunächst den Bericht durch Filter und Ansichten und erstellen Sie dann einen neuen geplanten Versand.
>
>Wenn Sie einen geplanten Berichtsversand verwenden, um Workfront-Daten über ein BI-Tool zu analysieren, empfehlen wir stattdessen Workfront Data Connect . Weitere Informationen finden Sie unter [Übersicht über Workfront Data Connect](/help/quicksilver/reports-and-dashboards/data-lake/data-lake-overview.md).

## Löschen eines terminierten Berichtsversands

So löschen Sie einen geplanten Berichtsversand&#x200B;

{{step1-to-reports}}

1. Wählen Sie auf **Seite** einen Bericht aus.

1. Klicken Sie oben im Bildschirm in der angezeigten Dropdown **Liste auf** Berichtsaktionen **und dann** Bericht senden“. Das **Bericht senden** wird angezeigt.

1. Wählen Sie die **Wiederholte Sendungen** aus.
1. Klicken **im rechten** des Dialogfelds im Abschnitt „Wiederholte Sendungen“ auf den geplanten Versand, den Sie löschen möchten.
1. Klicken **im Abschnitt** Sendungen auf **Löschen**.

1. Klicken Sie **Löschen** zur Bestätigung.

<!--## Video walk-through

View the following video to learn how to schedule a report delivery. This video was recorded in Workfront Classic. However, the content also applies to the new Workfront experience.

[ ![Video walkthrough of report delivery](assets/video-walk-through--350x197.png)](https://workfront-video.wistia.com/medias/45jffmll62)


<h2 data-mc-conditions="QuicksilverOrClassic.Draft mode">Additional information</h2>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">See also:</p>
-->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="https://one.workfront.com/s/learningpath2/workfront-reporting-20Y0z000000blhLEAQ" target="_blank">Learning Path for reports and dashboards</a> </li>
  -->

<!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="https://one.workfront.com/s/basic-report-creation-program">Basic Report Creation Program for the new Workfront experience</a> </p>
  -->
