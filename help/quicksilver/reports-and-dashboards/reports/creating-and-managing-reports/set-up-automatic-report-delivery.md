---
product-area: reporting;setup
navigation-topic: create-and-manage-reports
title: Planen eines automatischen Berichtversands
description: Planen eines automatischen Berichtversands
author: Nolan
feature: Reports and Dashboards
exl-id: 5b8e382c-bfe8-43aa-aa09-a2aa0c4d56cc
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '1164'
ht-degree: 3%

---

# Planen eines automatischen Berichtversands

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: If this stays, fix links which now go to the reference article)</p>
-->

Sie können Berichte so planen, dass sie den Benutzern automatisch nach einem festgelegten Zeitplan bereitgestellt werden, oder Sie können Berichte manuell einmalig versenden. Wenn Sie einen Bericht von Adobe Workfront senden, erhält der Benutzer eine E-Mail mit dem Workfront-Bericht in einem separaten Anhang.

Weitere Informationen, einschließlich Größenbeschränkungen, die sich auf die Bereitstellung Ihrer Berichte auswirken können, finden Sie unter [Berichtversand - Übersicht](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf Berichte, Dashboards und Kalender bearbeiten</p> <p>Zugriff auf Filter, Ansichten, Gruppierungen bearbeiten</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Berechtigungen für einen Bericht verwalten</p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Voraussetzungen

Bevor Sie beginnen, müssen Sie einen Bericht erstellen. Weitere Informationen zum Erstellen von Berichten finden Sie unter [Benutzerdefinierten Bericht erstellen](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

## Berichtversand planen

So planen Sie einen Bericht für die automatische Bereitstellung oder zum Bearbeiten oder Löschen eines vorhandenen Berichtversands: &#x200B;

1. Gehen Sie zu einem Bericht, den Sie für die Bereitstellung planen möchten.

   >[!NOTE]
   >
   >Berichtbereitstellungen enthalten keine Eingabeaufforderungen. Wenn Sie Daten in einem Berichtversand begrenzen möchten, empfehlen wir, Filter auf den Bericht anzuwenden, den Sie senden möchten.

1. Klicken **Berichtaktionen**, dann **Bericht senden**.

   Die **Bericht senden** angezeigt.

   >[!TIP]
   >
   >Um einen Bericht zu einem beliebigen Zeitpunkt manuell zu senden, rufen Sie den Bericht auf und klicken Sie auf **Berichtaktionen** > **Bericht senden** > **Jetzt senden**.

1. Wählen Sie die **Wiederholen von Sendungen** Registerkarte.
1. (Bedingt) Um einen vorhandenen wiederholten Berichtversand zu ändern, wählen Sie den Berichtversand im **Wiederholen von Sendungen** Abschnitt.
1. Geben Sie die folgenden Informationen an:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>Senden an</p> </td> 
      <td> <p>Beginnen Sie mit der Eingabe des Namens des Benutzers, der Gruppe, des Teams oder der Rolle, an den/die Sie den Bericht senden möchten, und klicken Sie dann auf den Namen, wenn er in der Dropdownliste angezeigt wird.</p> <p>Oder</p> <p>Geben Sie die E-Mail-Adresse einer außerhalb des Workfront-Systems befindlichen Person an, die Zugriff auf den Bericht erhalten soll.</p> <p>Wiederholen Sie diesen Vorgang, um den Bericht an mehrere Benutzer, Gruppen, Teams oder Rollen zu senden.</p> <p>Notiz:  <p>Beachten Sie beim Hinzufügen von Empfängern für die Berichtbereitstellung Folgendes:</p> 
        <ul> 
         <li>Wenn Ihre Organisation Workfront-Benachrichtigungen auf bestimmte E-Mail-Domänen beschränkt, können Sie Berichte nur an die in der E-Mail-Zulassungsliste aufgelisteten E-Mail-Adressen senden.<p>Informationen dazu, wie ein Workfront-Administrator die E-Mail-Zulassungsliste aktualisiert, finden Sie im Abschnitt . <a href="../../../administration-and-setup/get-started-wf-administration/configure-your-email-allowlist.md#configur" class="MCXref xref">Konfigurieren der E-Mail-Zulassungsliste</a>.</p></li> 
         <li> <p>Das Hinzufügen einer großen Anzahl von Benutzern als Empfänger kann dazu führen, dass der Versand fehlschlägt. Wenn bei Ihnen Versandfehler auftreten, können Sie mehrere Berichtbereitstellungen mit kleineren Benutzergruppen planen.</p> </li> 
        </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>E-Mail-Betreff</p> </td> 
      <td> <p>Geben Sie einen Betreff für die E-Mail-Benachrichtigung an.</p> <p>Standardmäßig lautet der E-Mail-Betreff:</p> <p><em>Workfront-Bericht: [Name des Berichts] [Datum]</em> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>E-Mail-Nachricht</p> </td> 
      <td> <p>Geben Sie eine Nachricht an, die in die E-Mail aufgenommen werden soll.</p> <p>Standardmäßig lautet die E-Mail-Nachricht:</p> <p><em>Angehängt ist der [Berichtsfrequenz]-Bericht [Name des Berichts], der von Workfront am [Datum] generiert wurde.</em> </p> <p>Hinweis: Nur für Berichte, die als Excel-Datei übermittelt werden, wird die folgende Nachricht der E-Mail hinzugefügt: "Bitte beachten Sie, dass bei MS Excel (XLS)-Dateitypen die Anzahl der von diesen Dateitypen unterstützten Hyperlinks (65.530) begrenzt ist. Wenn Sie diese Beschränkungen überschreiten, wird Ihre Datei nicht geöffnet und es wird empfohlen, ohne die Hyperlinks erneut zu senden. Gehen Sie zurück zur Planung des Berichts, um Hyperlinks zu entfernen und den Bericht erneut zu senden." Die Wortgruppe "Bitte gehen Sie zurück zur Berichtsplanung" ist ein Link zurück zum Bericht.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Diesen Bericht senden mit Zugriffsrechten von</p> </td> 
      <td> <p>Beginnen Sie mit der Eingabe des Namens eines Benutzers, der Zugriff auf den Bericht hat, und klicken Sie dann auf den Namen, wenn er in der Dropdown-Liste angezeigt wird. Benutzern, die den Bericht erhalten, wird derselbe Zugriff auf den Bericht gewährt wie dem Benutzer, den Sie hier angeben.<br> Weitere Informationen finden Sie unter <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/run-deliver-report-access-rights-another-user.md" class="MCXref xref">Einen Bericht mit Zugriffsrechten für einen anderen Benutzer ausführen und bereitstellen</a>.</p> <p>Hinweis: Dieses Feld unterstützt keine Platzhalter. Beispielsweise führt die Verwendung des Platzhalters $$User.ID den Bericht nicht mit den Zugriffsrechten des Benutzers aus, der den Bericht erhält.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Format</p> </td> 
      <td> <p>Wählen Sie das Format für den gelieferten Bericht aus:</p> 
       <ul> 
        <li> <p>HTML</p> </li> 
        <li> <p>PDF</p> <p>Wenn Sie diese Option auswählen, können Sie die Ausgabe mit dem zusätzlichen <strong>Papierformat</strong> und <strong>Ausrichtung</strong> Optionen, die angezeigt werden.</p> </li> 
        <li> <p>MS Excel (.xlsx)</p> </li> 
        <li> <p>TSV</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Links einbeziehen</p> </td> 
      <td> <p>Diese Option ist nur verfügbar, wenn <strong>MS Excel</strong> wird im <strong>Format</strong> Dropdown-Menü. Wenn diese Option aktiviert ist, werden alle Hyperlinks in das exportierte Excel-Dokument aufgenommen.</p> <p>Dokumente mit mehr als 65.530 Links können nicht geöffnet werden. Wenn das exportierte Dokument mehr als 65.530 Links enthält, deaktivieren Sie diese Option.</p> <p>Diese Option ist standardmäßig aktiviert.</p> </td> 
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
      <td> <p>Wählen Sie die Häufigkeit aus, mit der der Versand wiederholt werden soll. Der Wert, den Sie für diese Option auswählen, basiert auf der in der Variablen <strong>Wiederholungen</strong> Dropdown-Liste.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Uhrzeit</p> </td> 
      <td> <p>Wählen Sie die Tageszeit für den Versand aus.</p> <p>Tipp: Da sich das Laden des Systems auf die Bereitstellungszeiten des Berichts auswirken kann, kann es zu einer Verzögerung zwischen der geplanten und der tatsächlichen Bereitstellungszeit kommen. Wenn Sie einen Bericht zu einem bestimmten Zeitpunkt bereitstellen möchten, empfehlen wir, den Versand vor dem gewünschten Zeitpunkt zu planen. Beispielsweise wird empfohlen, den Versand einen Tag vor dem gewünschten Datum zu planen.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Wiederholung am</p> </td> 
      <td> <p>Diese Option ist verfügbar, wenn die Variable <strong>Wiederholungen</strong> ist auf <strong>Wöchentlich</strong> oder <strong>Monatlich</strong>:</p> 
       <ul> 
        <li> <p>Wenn die <strong>Wiederholungen</strong> ist auf <strong>Wöchentlich</strong>: Wählen Sie die Wochentage aus, an die der Versand durchgeführt wird.</p> </li> 
        <li> <p>Wenn die <strong>Wiederholungen</strong> ist auf <strong>Monatlich</strong>: Wählen Sie aus, ob der Versand am Tag des Monats, des Wochentags oder des letzten Tages des Monats erfolgt (bei diesen Optionen wird das im <strong>Beginnt bei</strong> -Feld).</p> </li> 
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
      <td>Auswählen <strong>Nie</strong> , wenn der geplante Versand unbegrenzt halten soll.</td> 
     </tr> 
    </tbody> 
   </table>

1. Klicken **Speichern** , um den Berichtversand zu speichern.

   Der Bericht wird im **Wiederholen von Sendungen** -Abschnitt (im Abschnitt **Bericht senden** ) und wird zum geplanten Zeitpunkt gesendet.

   Informationen zu Größenbeschränkungen, die sich auf die Bereitstellung Ihrer Berichte auswirken können, finden Sie in den Abschnitten . [Versandbeschränkungen für Berichte](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md#understanding-export-limits) und [Ausfuhrbeschränkungen](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md#export).

1. (Optional) So löschen Sie einen geplanten Versand:

   1. Im **Wiederholen von Sendungen** Bereich, klicken Sie auf den terminierten Versand und dann auf **Löschen**.
   1. Klicken **Löschen** zur Bestätigung.

## Video-Beispiel

Sehen Sie sich das folgende Video an, um zu erfahren, wie Sie einen Berichtversand planen. Dieses Video wurde in Workfront Classic aufgezeichnet. Der Inhalt gilt jedoch auch für das neue Workfront-Erlebnis.

[ ![](assets/video-walk-through--350x197.png)](https://workfront-video.wistia.com/medias/45jffmll62)

<!--
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
