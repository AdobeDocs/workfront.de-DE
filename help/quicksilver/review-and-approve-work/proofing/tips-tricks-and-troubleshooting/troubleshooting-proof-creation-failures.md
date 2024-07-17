---
filename: troubleshooting-proof-creation-failures
content-type: tips-tricks-troubleshooting
product-area: documents
navigation-topic: use-the-desktop-proofing-viewer
title: Fehlerbehebung bei Fehlern bei der Testversand-Erstellung
description: Der Testversand-Erstellungsprozess umfasst sowohl die Import- als auch die Testversand-Generierung. Gelegentlich kann es bei der Erstellung eines Testversands vorkommen, dass eine Datei nicht importiert wird oder der Testversand nach dem Import der Datei fehlschlägt.
author: Courtney
source-git-commit: de30bd970bda06c706e5156d5195e8568558e593
workflow-type: tm+mt
source-wordcount: '415'
ht-degree: 0%

---


# Fehlerbehebung bei Fehlern bei der Testversand-Erstellung

Der Testversand-Erstellungsprozess umfasst sowohl die Import- als auch die Testversand-Generierung. Gelegentlich kann es bei der Erstellung eines Testversands vorkommen, dass eine Datei nicht importiert wird oder der Testversand nach dem Import der Datei fehlschlägt.

>[!NOTE]
>
> Wenn das Dokument, das Sie zum Testen versuchen, keines der in diesem Abschnitt aufgelisteten Kriterien erfüllt, wenden Sie sich für weitere Informationen an den Adobe Workfront-Support.

## Gründe für Importfehler

* Sie haben einen kombinierten Testversand mit mehr als 50 Dateien erstellt.

## Gründe für den Fehler bei der Testversand-Generierung

* Der Dateityp wird nicht unterstützt.\
  Eine Liste der unterstützten Dateitypen finden Sie unter [Unterstützte Testversand-Dateitypen und Größenbeschränkungen - Übersicht](../../../review-and-approve-work/proofing/proofing-overview/supported-proofing-file-types.md).

* Die Dateistruktur ist eine nicht standardmäßige Struktur für den Dateityp.
* Die Datei ist durch ein Kennwort geschützt oder das Kopieren von Inhalten ist deaktiviert.

  Im Gegensatz zu anderen Dateitypen können PDF-Dateien in Testsendungen generiert werden, wenn Ihre Sicherheitseinstellung für das Kopieren von Inhalten auf der PDF auf Zulässig gesetzt ist.

* Die Seitenlänge oder Seitenzahl überschreitet das Limit.

  Die maximal zulässige Seitenlänge beträgt 195 Zoll nach der Rasterung. Die maximal zulässige Seitenzahl beträgt 1.000 Seiten für einen einzelnen Testversand.

* Die Datei ist beschädigt oder beschädigt.
* Der Workflow-Termin für eine neue Testversion liegt in der Vergangenheit.

  Dies tritt auf, wenn Sie eine neue Testversand-Version mit einer Methode des schnellen Testversands erstellen und **beim Hochladen von Dokumenten automatisch Testsendungen generieren** ausgewählt ist. Die neue Testversand-Version versucht, die Workflow-Fristen aus dem zuvor erstellten Testversand zu übernehmen. Die Erstellung von Testsendungen schlägt fehl, wenn diese Frist in der Vergangenheit liegt. Um dieses Problem zu beheben, können Sie die Workflow-Fristen für die vorherige Version in der Zukunft festlegen oder eine neue Testversion erstellen. Wenn Sie eine neue Version generieren, verwenden Sie **Mehr > Neue Version > Testversand** und wählen Sie **Workflow-Termine in der Zukunft** aus.

* Beim Testen von PDF-Dateien gibt es folgende Gründe für den Fehler bei der Testversand-Generierung:

   * Schriftarten und Bilder werden aus externen Quellen verknüpft (z. B. aus Ihrem lokalen Dateisystem)

     Schriftarten und Bilder müssen in die PDF-Datei eingebettet sein, damit sie auf einem anderen Computer oder in Workfront Proof angezeigt werden können.

   * Ihre PDF-Datei enthält leere Ebenen oder transparente oder überlappende Felder.

     Wenn Sie nicht ermitteln können, welche Ebene oder welches Objekt dies verursacht, exportieren Sie das Design/Dokument als optimierte PDF (dadurch werden alle unerwünschten Elemente entfernt).

