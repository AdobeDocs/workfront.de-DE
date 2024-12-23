---
product-area: reporting;setup
navigation-topic: create-and-manage-reports
title: Planen eines automatischen Berichtversands
description: Planen eines automatischen Berichtversands
author: Nolan
feature: Reports and Dashboards
exl-id: 5b8e382c-bfe8-43aa-aa09-a2aa0c4d56cc
source-git-commit: 12e8bc389c42510b5adbb0190eb71c9f6a9f52a7
workflow-type: tm+mt
source-wordcount: '1197'
ht-degree: 2%

---

# Planen eines automatischen Berichtversands

<!-- Audited: 11/2024 -->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: If this stays, fix links which now go to the reference article)</p>
-->

Sie können Berichte so planen, dass sie den Benutzern automatisch nach einem festgelegten Zeitplan bereitgestellt werden, oder Sie können Berichte manuell einmalig versenden. Wenn Sie einen Bericht von Adobe Workfront senden, erhält der Benutzer eine E-Mail mit dem Workfront-Bericht in einem separaten Anhang.

Weitere Informationen, einschließlich Größenbeschränkungen, die sich auf die Bereitstellung Ihrer Berichte auswirken können, finden Sie unter [Übersicht über die Berichtbereitstellung](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
      <td> 
      <p>Neu:</p>
         <ul>
         <li><p>Standard</p></li>
         </ul>
      <p>Aktuell:</p>
         <ul>
         <li><p>Plan</p></li>
         </ul>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf Berichte, Dashboards und Kalender bearbeiten</p> <p>Zugriff auf Filter, Ansichten, Gruppierungen bearbeiten</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Berechtigungen für einen Bericht verwalten</p></td> 
  </tr> 
 </tbody> 
</table>

*Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Voraussetzungen

Bevor Sie beginnen, müssen Sie einen Bericht erstellen. Weitere Informationen zum Erstellen von Berichten finden Sie unter [Benutzerdefinierten Bericht erstellen](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

## Berichtversand planen

So planen Sie einen Bericht für die automatische Bereitstellung oder zum Bearbeiten oder Löschen eines vorhandenen Berichtversands: &#x200B;

1. Gehen Sie zu einem Bericht, den Sie für die Bereitstellung planen möchten.

   >[!NOTE]
   >
   >Berichtbereitstellungen enthalten keine Eingabeaufforderungen. Wenn Sie Daten in einem Berichtversand begrenzen möchten, empfehlen wir, Filter auf den Bericht anzuwenden, den Sie senden möchten.

1. Klicken Sie auf **Berichtaktionen** und dann auf **Bericht senden**.

   Das Dialogfeld **Bericht senden** wird angezeigt.

   >[!TIP]
   >
   >Um einen Bericht jederzeit manuell zu senden, gehen Sie zum Bericht und klicken Sie dann auf **Berichtaktionen** > **Bericht senden** > **Jetzt senden** .

1. Wählen Sie den Tab **Sendungen wiederholen** aus.
1. (Bedingt) Um einen vorhandenen wiederholten Berichtversand zu ändern, wählen Sie den Berichtversand im Abschnitt **Sendungen wiederholen** aus.
1. Geben Sie die folgenden Informationen an:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>Senden an</p> </td> 
      <td> <p>Beginnen Sie mit der Eingabe des Namens des Benutzers, der Gruppe, des Teams oder der Rolle, an den/die Sie den Bericht senden möchten, und klicken Sie dann auf den Namen, wenn er in der Dropdownliste angezeigt wird.</p> <p>Oder</p> <p>Geben Sie die E-Mail-Adresse einer außerhalb des Workfront-Systems befindlichen Person an, die Zugriff auf den Bericht erhalten soll.</p> <p>Wiederholen Sie diesen Vorgang, um den Bericht an mehrere Benutzer, Gruppen, Teams oder Rollen zu senden.</p> <p>Hinweis:  <p>Beachten Sie beim Hinzufügen von Empfängern für die Berichtbereitstellung Folgendes:</p> 
        <ul> 
         <li>Wenn Ihre Organisation Workfront-Benachrichtigungen auf bestimmte E-Mail-Domänen beschränkt, können Sie Berichte nur an die in der E-Mail-Zulassungsliste aufgelisteten E-Mail-Adressen senden.<p>Informationen dazu, wie ein Workfront-Administrator die E-Mail-Zulassungsliste aktualisiert, finden Sie im Abschnitt <a href="../../../administration-and-setup/get-started-wf-administration/configure-your-email-allowlist.md#configur" class="MCXref xref">E-Mail konfigurieren</a>.</p></li> 
         <li> <p>Das Hinzufügen einer großen Anzahl von Benutzern als Empfänger kann dazu führen, dass der Versand fehlschlägt. Wenn bei Ihnen Versandfehler auftreten, können Sie mehrere Berichtbereitstellungen mit kleineren Benutzergruppen planen.</p> </li> 
        </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>E-Mail-Betreff</p> </td> 
      <td> <p>Geben Sie einen Betreff für die E-Mail-Benachrichtigung an.</p> <p>Standardmäßig lautet der E-Mail-Betreff:</p> <p><em>Workfront-Bericht: [Name des Berichts] [Datum]</em> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>E-Mail-Nachricht</p> </td> 
      <td> <p>Geben Sie eine Nachricht an, die in die E-Mail aufgenommen werden soll.</p> <p>Standardmäßig lautet die E-Mail-Nachricht:</p> <p><em>Angehängt ist der [Berichtsfrequenz]-Bericht [Name des Berichts], der von Workfront am [Datum] generiert wurde.</em> </p> <p>Hinweis: Bei Berichten, die nur als Excel-Datei gesendet werden, wird der E-Mail auch die folgende Meldung hinzugefügt: "Beachten Sie, dass bei MS Excel (XLS)-Dateitypen die Anzahl der Hyperlinks, die diese Dateitypen unterstützen, begrenzt ist (65.530). Wenn Sie diese Beschränkungen überschreiten, wird Ihre Datei nicht geöffnet und es wird empfohlen, ohne die Hyperlinks erneut zu senden. Gehen Sie zurück zur Planung des Berichts, um Hyperlinks zu entfernen und den Bericht erneut zu senden." Die Wortgruppe "Bitte gehen Sie zurück zur Berichtsplanung" ist ein Link zurück zum Bericht.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Bereitstellen dieses Berichts mit den Zugriffsrechten von</p> </td> 
      <td> <p>Geben Sie den Namen eines Benutzers ein, der Zugriff auf den Bericht hat, und klicken Sie dann auf den Namen, wenn er in der Dropdown-Liste angezeigt wird. Benutzern, die den Bericht erhalten, wird derselbe Zugriff auf den Bericht gewährt wie dem Benutzer, den Sie hier angeben.<br> Weitere Informationen finden Sie unter <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/run-deliver-report-access-rights-another-user.md" class="MCXref xref">Ausführen und Bereitstellen eines Berichts mit den Zugriffsrechten eines anderen Benutzers</a>.</p> <p>Hinweis: Dieses Feld unterstützt keine Platzhalter. Beispielsweise führt die Verwendung des Platzhalters $$User.ID den Bericht nicht mit den Zugriffsrechten des Benutzers aus, der den Bericht erhält.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Format</p> </td> 
      <td> <p>Wählen Sie das Format für den gelieferten Bericht aus:</p> 
       <ul> 
        <li> <p>HTML</p> </li> 
        <li> <p>PDF</p> <p>Wenn Sie diese Option auswählen, können Sie die Ausgabe mit den zusätzlichen angezeigten Optionen <strong>Papiergröße</strong> und <strong>Ausrichtung</strong> formatieren.</p> </li> 
        <li> <p>MS Excel (.xlsx)</p> </li> 
        <li> <p>TSV</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Links einbeziehen</p> </td> 
      <td> <p>Diese Option ist nur verfügbar, wenn im Dropdown-Menü <strong>Format</strong> die Option <strong>MS Excel</strong> ausgewählt ist. Wenn diese Option aktiviert ist, werden alle Hyperlinks in das exportierte Excel-Dokument aufgenommen.</p> <p>Dokumente mit mehr als 65.530 Links können nicht geöffnet werden. Wenn das exportierte Dokument mehr als 65.530 Links enthält, deaktivieren Sie diese Option.</p> <p>Diese Option ist standardmäßig aktiviert.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Zusammenfassung</p> </td> 
      <td> <p>Zeigt eine Zusammenfassung des Zeitpunkts an, zu dem der Versand wiederholt wird.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Wiederholungen</p> </td> 
      <td> <p>Wählen Sie aus, ob der Bericht täglich, wöchentlich, monatlich oder jährlich bereitgestellt werden soll.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Wiederholung alle</p> </td> 
      <td> <p>Wählen Sie die Häufigkeit aus, mit der der Versand wiederholt werden soll. Der Wert, den Sie für diese Option auswählen, basiert auf der Option, die in der Dropdownliste <strong>Wiederholungen</strong> ausgewählt ist.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Uhrzeit</p> </td> 
      <td> <p>Wählen Sie die Tageszeit für den Versand aus.</p> <p>Tipp: Da sich das Laden des Systems auf die Bereitstellungszeiten des Berichts auswirken kann, kann es zwischen der geplanten und der tatsächlichen Bereitstellungszeit zu einer Verzögerung von bis zu 24 Stunden kommen. Wenn Sie einen Bericht zu einem bestimmten Zeitpunkt bereitstellen möchten, empfehlen wir, den Versand vor dem gewünschten Zeitpunkt zu planen. Im Allgemeinen empfehlen wir, den Versand mindestens einen Tag vor dem gewünschten Datum zu planen.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Wiederholung am</p> </td> 
      <td> <p>Diese Option ist verfügbar, wenn die Option <strong>Wiederholungen</strong> auf <strong>Wöchentlich</strong> oder <strong>Monatlich</strong> festgelegt ist:</p> 
       <ul> 
        <li> <p>Wenn die Option <strong>Wiederholungen</strong> auf <strong>Wöchentlich</strong> eingestellt ist: Wählen Sie die Wochentage aus, an die der Versand durchgeführt wird.</p> </li> 
        <li> <p>Wenn die Option <strong>Wiederholungen</strong> auf <strong>Monatlich</strong> eingestellt ist: Wählen Sie aus, ob der Versand am Tag des Monats, des Wochentags oder des letzten Tages des Monats erfolgt (bei diesen Optionen wird das im Feld <strong>Starts am</strong> ausgewählte Datum verwendet).</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Beginnt am</p> </td> 
      <td>Wählen Sie das Datum aus, an dem der geplante Versand beginnen soll.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>endet am</p> </td> 
      <td>Wählen Sie ein Datum aus, an dem der geplante Versand enden soll.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Nie</p> </td> 
      <td>Wählen Sie <strong>Nie</strong> aus, wenn der geplante Versand unbegrenzt lange dauern soll.</td> 
     </tr> 
    </tbody> 
   </table>

1. Klicken Sie auf **Speichern** , um die Berichtbereitstellung zu speichern.

   Der Bericht wird im Abschnitt **Wiederholende Sendungen** (im Dialogfeld **Bericht senden** ) angezeigt und zum geplanten Zeitpunkt gesendet.

   Informationen zu Größenbeschränkungen, die sich auf die Bereitstellung Ihrer Berichte auswirken können, finden Sie in den Abschnitten [Einschränkungen bei der Berichtauslieferung](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md#understanding-export-limits) und [Exportbeschränkungen](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md#export).

>[!IMPORTANT]
>
>Terminierte Berichte unterliegen bei der Versandverarbeitung einer internen Zeitbegrenzung. Sollte der Versand eines Berichts länger dauern als begrenzt, erhalten Sie eine Benachrichtigung und der Bericht wird unabhängig von den restlichen geplanten Sendungen nicht mehr zugestellt. Um mit dem Versand des Berichts fortzufahren, versuchen Sie zunächst, die Größe des Berichts durch Filter und Ansichten zu reduzieren, und erstellen Sie dann einen neuen geplanten Versand.
>
>Wenn Sie einen geplanten Berichtversand verwenden, um Workfront-Daten über ein BI-Tool zu analysieren, empfehlen wir stattdessen die Verwendung von Workfront Data Connect . Weitere Informationen finden Sie unter [Übersicht über Workfront Data Connect](/help/quicksilver/reports-and-dashboards/data-lake/data-lake-overview.md).

1. (Optional) So löschen Sie einen geplanten Versand:

   1. Klicken Sie im Bedienfeld **Sich wiederholende Sendungen** auf den geplanten Versand und dann auf **Löschen**.
   1. Klicken Sie zur Bestätigung auf **Löschen** .

<!--## Video walk-through

View the following video to learn how to schedule a report delivery. This video was recorded in Workfront Classic. However, the content also applies to the new Workfront experience.

[ ![](assets/video-walk-through--350x197.png)](https://workfront-video.wistia.com/medias/45jffmll62)


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
