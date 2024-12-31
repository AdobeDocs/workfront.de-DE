---
filename: troubleshooting-proof-creation-failures
content-type: tips-tricks-troubleshooting
product-area: documents
navigation-topic: use-the-desktop-proofing-viewer
title: Fehlerbehebung bei Fehlern bei der Erstellung von Korrekturabzügen
description: Der Erstellungsprozess des Korrekturabzugs umfasst sowohl den Import als auch die Erstellung des Korrekturabzugs. Wenn Sie einen Korrekturabzug erstellen, kann es vorkommen, dass eine Datei nicht importiert werden kann oder der Korrekturabzug nach dem Import der Datei nicht erstellt werden kann.
author: Courtney
source-git-commit: de30bd970bda06c706e5156d5195e8568558e593
workflow-type: tm+mt
source-wordcount: '415'
ht-degree: 0%

---


# Fehlerbehebung bei Fehlern bei der Erstellung von Korrekturabzügen

Der Erstellungsprozess des Korrekturabzugs umfasst sowohl den Import als auch die Erstellung des Korrekturabzugs. Wenn Sie einen Korrekturabzug erstellen, kann es vorkommen, dass eine Datei nicht importiert werden kann oder der Korrekturabzug nach dem Import der Datei nicht erstellt werden kann.

>[!NOTE]
>
> Wenn das Dokument, das Sie prüfen möchten, keinem der in diesem Abschnitt aufgeführten Kriterien entspricht, wenden Sie sich an den Adobe Workfront-Support, um weitere Informationen zu erhalten.

## Gründe für einen fehlgeschlagenen Import

* Sie haben einen kombinierten Korrekturabzug mit über 50 Dateien erstellt.

## Gründe für das Fehlschlagen der Korrekturabzugsgenerierung

* Der Dateityp wird nicht unterstützt.\
  Eine Liste der unterstützten Dateitypen finden Sie unter [Unterstützte Proofing-Dateitypen und Größenbeschränkungen - Übersicht](../../../review-and-approve-work/proofing/proofing-overview/supported-proofing-file-types.md).

* Die Dateistruktur ist keine Standardstruktur für den Dateityp.
* Die Datei ist durch ein Passwort geschützt oder das Kopieren von Inhalten ist deaktiviert.

  Im Gegensatz zu anderen Dateitypen können PDF-Dateien zu Korrekturabzügen generiert werden, wenn Ihre Sicherheitseinstellung für das Kopieren von Inhalten auf der PDF auf Zulässig festgelegt ist.

* Die Seitenlänge oder die Seitenzahl überschreitet das Limit.

  Die maximal zulässige Seitenlänge nach dem Rastern beträgt 195 Zoll. Für einen einzelnen Korrekturabzug ist eine maximale Seitenanzahl von 1.000 Seiten zulässig.

* Die Datei ist beschädigt oder beschädigt.
* Die Workflowfrist für eine neue Korrekturabzugsversion liegt in der Vergangenheit.

  Dies tritt auf, wenn Sie eine neue Korrekturabzugsversion mit einer Schnellkorrekturmethode erstellen und **Beim Hochladen von Dokumenten automatisch Korrekturabzüge generieren** ausgewählt ist. Die neue Korrekturabzugsversion versucht, die Workflow-Fristen aus dem zuvor generierten Korrekturabzug zu übernehmen. Die Erstellung des Korrekturabzugs schlägt fehl, wenn diese Fristen in der Vergangenheit liegen. Um dies zu beheben, können Sie die Workflow-Fristen für die vorherige Version in der Zukunft festlegen oder eine neue Korrekturabzugsversion erstellen. Wenn Sie eine neue Version erstellen, verwenden Sie **Mehr > Neue Version > Korrekturabzug** und wählen Sie **Workflow-Fristen in der Zukunft** aus.

* Beim Proofing von PDF-Dateien gibt es folgende Gründe für das Fehlschlagen der Erstellung von Korrekturabzügen:

   * Schriftarten und Bilder werden von externen Quellen verknüpft (z. B. aus Ihrem lokalen Dateisystem)

     Schriftarten und Bilder müssen in die PDF-Datei eingebettet werden, damit sie auf einem anderen Computer oder in Workfront Proof angezeigt werden können.

   * Ihre PDF-Datei enthält leere Ebenen oder transparente oder überlappende Felder.

     Wenn Sie nicht feststellen können, welche Ebene oder welches Objekt dies verursacht, exportieren Sie das Design/Dokument als optimierte PDF (dadurch werden alle unerwünschten Elemente entfernt).

