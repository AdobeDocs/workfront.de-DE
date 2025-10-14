---
product-previous: workfront-proof
product-area: documents
navigation-topic: manage-your-work-workfront-proof
title: Berichte ausführen in [!DNL Workfront Proof]
description: Mit Workfront Proof können Sie Berichte anzeigen, um den Arbeitsfortschritt und die Effizienz Ihrer Teams zu verfolgen.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 342f9282-b6f5-425e-a7ef-e23bd011d284
source-git-commit: a0d76692f9e9d12ed0d538c1344638dbc208d625
workflow-type: tm+mt
source-wordcount: '691'
ht-degree: 0%

---

# Berichte in [!DNL Workfront Proof] ausführen


>[!IMPORTANT]
>
>* <span class="previe">Die Reporting-Funktion ist in [!DNL Workfront Proof] nicht mehr verfügbar. Die Registerkarte Reporting wird weiterhin angezeigt, aber die Daten sind nicht korrekt.</span>
> 
>* Dieser Artikel bezieht sich auf Funktionen im eigenständigen [!DNL Workfront Proof]. Informationen zu Proofing in [!DNL Adobe Workfront] finden Sie unter [Proofing](../../../review-and-approve-work/proofing/proofing.md).

Mit Workfront Proof können Sie Berichte anzeigen, um den Arbeitsfortschritt und die Effizienz Ihrer Teams zu verfolgen.

Sie können auf einfache Weise die Anzahl der Korrekturabzüge anzeigen, die in Ihrem [!DNL Workfront Proof]-Konto erstellt wurden, wie viele Versionen mit jedem Korrekturabzug verknüpft sind, die Durchlaufzeit und mehr.

## Voraussetzungen

Ob Berichte verfügbar sind, hängt von der Art des [!DNL Workfront Proof] Kontos und den Benutzerberechtigungsebenen ab.

* [Voraussetzungen für das Konto](#account-prerequisites)
* [Voraussetzungen für den Benutzer](#user-prerequisites)

### Voraussetzungen für das Konto {#account-prerequisites}

Reporting-Informationen sind nur bei Premium-Plänen verfügbar.

### Voraussetzungen für den Benutzer {#user-prerequisites}

Berichtsinformationen sind nur für Benutzer mit vollem Zugriff auf alle Korrekturabzüge in Ihrem Konto verfügbar (d. h. für Benutzer mit mindestens [Korrekturabzugsberechtigungen in Profilen [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md)).

In diesem Bedienfeld haben Sie folgende Möglichkeiten

* Steuerung der Zeitspanne der angezeigten Daten
* Analysieren von Änderungen der Metriken im Zeitverlauf
* Überprüfen Sie die Details eines ausgewählten Zeitpunkts, indem Sie den Mauszeiger darüber bewegen
* Überprüfen Sie die Gesamtzahl der in Ihrem ausgewählten Zeitraum erstellten Korrekturabzüge
* Durchschnittliche Anzahl der Versionen überprüfen, die in den abgeschlossenen Testsendungen enthalten sind

## Anzeigen von Berichten {#viewing-reports}

1. Navigieren Sie zur Seite **[!UICONTROL Dashboards]** .
1. Klicken Sie auf die **[!UICONTROL Berichte]**.\
   ![proof_reports.png](assets/proof-reports-350x193.png)

1. Wählen **[!UICONTROL Dropdown-Menü Zeitrahmen]** aus, ob Sie Informationen zu Korrekturabzügen anzeigen möchten, die innerhalb der letzten 24 Stunden, 7 Tage, 30 Tage, 90 Tage oder eines benutzerdefinierten Zeitraums erstellt wurden.\
   Wenn Sie einen benutzerdefinierten Zeitraum auswählen, wählen Sie das Start- und Enddatum aus und klicken Sie dann auf **[!UICONTROL Übernehmen]**.\
   Die folgenden Informationen werden für den ausgewählten Zeitraum angezeigt:\
   **Korrekturabzug erstellt:** Anzahl der Korrekturabzüge, die innerhalb des ausgewählten Zeitraums erstellt wurden.\
   **Versionen pro Korrekturabzug:** Durchschnittliche Anzahl der Versionen pro Korrekturabzug für alle abgeschlossenen Korrekturabzüge (genehmigt oder mit Änderungen genehmigt) innerhalb des ausgewählten Zeitraums.\
   **Durchschnittliche Zeit für das Drehen:** Durchschnittliche Zeit vom Zeitpunkt der Erstellung der ersten Version bis zum Zeitpunkt der Entscheidung über die endgültige Version.\
   **Zeit der ersten Aktivität:** Durchschnittliche Zeit vom Zeitpunkt der Erstellung des Korrekturabzugs bis zur ersten Aktivität auf dem Korrekturabzug.\
   **Korrekturabzüge verspätet:** Durchschnittlicher Prozentsatz der abgeschlossenen Korrekturabzüge (genehmigt oder mit Änderungen genehmigt), die mindestens eine Version hatten, die innerhalb des ausgewählten Zeitraums zu spät war.\
   **Kommentare und Antworten:** Durchschnittliche Anzahl der Kommentare und Antworten, die innerhalb des ausgewählten Zeitraums zu allen Korrekturabzügen gemacht wurden.

1. (Optional) Wählen Sie die Option **[!UICONTROL Min-Max-Bereich anzeigen]** aus, um zu bestimmen, ob Mindest- und Höchstwerte im Diagramm angezeigt werden.\
   Bei Auswahl dieser Option wird zwischen den minimalen und maximalen Werten eine blaue Schattierung angezeigt.

1. (Optional) Sie können die angezeigten Daten filtern, wie unter [Filterberichte“ &#x200B;](#filtering-reports).

## Berichte filtern {#filtering-reports}

Standardmäßig enthalten die in Berichten angezeigten Daten alle Informationen aus Ihrem [!DNL Workfront Proof]. Sie können Filter verwenden, um nur Informationen anzuzeigen, die für Ihre Anforderungen relevant sind.

So filtern Sie Berichtsinformationen:

1. Navigieren Sie zur Seite **[!UICONTROL Dashboards]** .
1. Klicken Sie auf die **[!UICONTROL Berichte]**.\
   ![proof_reports.png](assets/proof-reports-350x193.png)

1. Führen Sie einen Bericht aus, wie in [Anzeigen von Berichten](#viewing-reports) beschrieben.
1. Klicken Sie **[!UICONTROL Filter]**.

1. Wählen Sie links auf der Seite eine der folgenden Filteroptionen aus:\
   **[!UICONTROL Testversand-]:** Sie den Testversand-Typ aus, den Sie in den Bericht aufnehmen möchten.\
   **[!UICONTROL Entscheidungen]:** Wählen Sie Optionen aus, um festzustellen, ob nur Korrekturabzüge, die bestimmte Entscheidungen enthalten, durchgeführt wurden.\
   **[!UICONTROL Empfänger]:** Wählen Sie einzelne Benutzer aus, um Informationen zu Korrekturabzügen anzuzeigen, die für die ausgewählten Benutzer freigegeben wurden.\
   **[!UICONTROL Testversand-Verantwortliche]:** Sie einzelne Benutzer aus, um Informationen zu Testsendungen anzuzeigen, die den ausgewählten Benutzern gehören.\
   **[!UICONTROL Korrekturabzug-Ersteller]:** Sie einzelne Benutzer aus, um Informationen zu den von den ausgewählten Benutzern erstellten Korrekturabzügen anzuzeigen.\
   **[!UICONTROL Konten]:** Wählen Sie aus, welche Konten Sie in den Bericht aufnehmen möchten.

1. Klicken Sie **[!UICONTROL Apply]**.
1. (Optional) Wählen Sie die Option **[!UICONTROL Min-Max-Bereich anzeigen]** aus, um zu bestimmen, ob Mindest- und Höchstwerte im Diagramm angezeigt werden.\
   Bei Auswahl dieser Option wird zwischen den minimalen und maximalen Werten eine blaue Schattierung angezeigt.

## Berichte drucken

1. Navigieren Sie zur Seite **[!UICONTROL Dashboards]** .
1. Klicken Sie auf die **[!UICONTROL Berichte]** und dann auf **[!UICONTROL Drucken]**.\
   ![PROOF_REPORTS_PRINT.png](assets/proof-reports-print-350x191.png)

1. Wählen Sie aus den verschiedenen verfügbaren Druckoptionen.\
   Die Druckoptionen variieren je nach verwendetem Browser und Browser-Version.
