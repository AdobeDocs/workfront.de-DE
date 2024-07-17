---
product-previous: workfront-proof
product-area: documents
navigation-topic: manage-your-work-workfront-proof
title: Berichte ausführen in [!DNL Workfront Proof]
description: Mit Workfront Proof können Sie Berichte anzeigen, damit Sie den Arbeitsfortschritt und die Effizienz Ihrer Teams verfolgen können.
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
>* <span class="previe">Die Berichtsfunktion ist in [!DNL Workfront Proof] nicht mehr verfügbar. Die Registerkarte &quot;Berichterstellung&quot;wird weiterhin angezeigt, die Daten sind jedoch nicht genau.</span>
> 
>* Dieser Artikel bezieht sich auf die Funktionalität im eigenständigen Produkt [!DNL Workfront Proof]. Informationen zum Testen innerhalb von [!DNL Adobe Workfront] finden Sie unter [Testversand](../../../review-and-approve-work/proofing/proofing.md).

Mit Workfront Proof können Sie Berichte anzeigen, damit Sie den Arbeitsfortschritt und die Effizienz Ihrer Teams verfolgen können.

Sie können die Anzahl der Testsendungen, die in Ihrem [!DNL Workfront Proof] -Konto erstellt wurden, die Anzahl der Versionen, die mit jedem Testversand verknüpft sind, die Bearbeitungszeit und vieles mehr einfach anzeigen.

## Voraussetzungen

Ob Berichte verfügbar sind, hängt von Ihrem [!DNL Workfront Proof] -Konto- und Benutzerberechtigungsniveau ab.

* [Kontovoraussetzungen](#account-prerequisites)
* [Benutzervoraussetzungen](#user-prerequisites)

### Kontovoraussetzungen {#account-prerequisites}

Berichtinformationen sind nur bei Premium-Plänen verfügbar.

### Benutzervoraussetzungen {#user-prerequisites}

Berichtsinformationen sind nur für Benutzer mit uneingeschränktem Zugriff auf alle Testsendungen in Ihrem Konto verfügbar (d. h. Benutzer mit mindestens [Testberechtigungsprofilen in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md)).

In diesem Bedienfeld können Sie

* Zeitspanne der angezeigten Daten steuern
* Änderungen an Metriken im Zeitverlauf analysieren
* Überprüfen Sie die Details eines ausgewählten Zeitpunkts, indem Sie den Mauszeiger darüber bewegen.
* Überprüfen Sie die Gesamtzahl der in Ihrem ausgewählten Zeitraum erstellten Testsendungen.
* Überprüfen Sie die durchschnittliche Anzahl der Versionen, die in den abgeschlossenen Testsendungen enthalten sind.

## Anzeigen von Berichten {#viewing-reports}

1. Rufen Sie die Seite **[!UICONTROL Dashboards]** auf.
1. Klicken Sie auf die Registerkarte **[!UICONTROL Berichte]**.\
   ![proof_reports.png](assets/proof-reports-350x193.png)

1. Wählen Sie im Dropdown-Menü **[!UICONTROL Zeitrahmen]** aus, ob Sie Informationen zu Testsendungen anzeigen möchten, die in den letzten 24 Stunden, 7 Tagen, 30 Tagen, 90 Tagen oder einem benutzerdefinierten Zeitraum erstellt wurden.\
   Wenn Sie einen benutzerdefinierten Zeitraum auswählen, wählen Sie das Start- und Enddatum aus und klicken Sie dann auf **[!UICONTROL Anwenden]**.\
   Die folgenden Informationen werden für den ausgewählten Zeitraum angezeigt:\
   **Erstellter Testversand:** Anzahl der im ausgewählten Zeitraum erstellten Testsendungen.\
   **Versionen pro Testversand:** Durchschnittliche Anzahl der Versionen pro Testversand für alle durchgeführten Testsendungen (Genehmigt oder Genehmigt mit Änderungen) innerhalb des ausgewählten Zeitraums.\
   **Umschalt um Zeit:** Durchschnittliche Zeit ab der Erstellung der ersten Version bis zum Zeitpunkt der Entscheidungsfindung für die endgültige Version.\
   **Erste Aktivitätszeit:** Durchschnittliche Zeit ab der Erstellung des Testversands bis zur ersten Aktivität des Testversands.\
   **Testsendungen verspätet:** Durchschnittlicher Prozentsatz abgeschlossener Testsendungen (Genehmigt oder Genehmigt mit Änderungen) mit mindestens einer Version, die im ausgewählten Zeitraum zu spät war.\
   **Kommentare und Antworten:** Durchschnittliche Anzahl von Kommentaren und Antworten, die für alle Testsendungen innerhalb des ausgewählten Zeitraums erstellt wurden.

1. (Optional) Aktivieren oder deaktivieren Sie die Option **[!UICONTROL Min-Max-Bereich anzeigen]** , um zu bestimmen, ob Mindest- und Höchstwerte im Diagramm angezeigt werden.\
   Wenn diese Option aktiviert ist, wird zwischen den minimalen und maximalen aufgezeichneten Werten eine blaue Schattierung angezeigt.

1. (Optional) Sie können die angezeigten Daten filtern, wie unter [Filtern von Berichten](#filtering-reports) beschrieben.

## Filtern von Berichten {#filtering-reports}

Standardmäßig enthalten in Berichten angezeigte Daten alle Informationen aus Ihrem [!DNL Workfront Proof] -System. Sie können Filter verwenden, um nur Informationen anzuzeigen, die für Ihre Anforderungen relevant sind.

So filtern Sie Berichtsinformationen:

1. Rufen Sie die Seite **[!UICONTROL Dashboards]** auf.
1. Klicken Sie auf die Registerkarte **[!UICONTROL Berichte]**.\
   ![proof_reports.png](assets/proof-reports-350x193.png)

1. Führen Sie einen Bericht aus, wie unter [Anzeigen von Berichten](#viewing-reports) beschrieben.
1. Klicken Sie auf **[!UICONTROL Filter]**.

1. Wählen Sie auf der linken Seite der Seite aus den folgenden Filteroptionen:\
   **[!UICONTROL Testversand-Typ]:** Wählen Sie den Typ der Testsendungen aus, die in den Bericht aufgenommen werden sollen.\
   **[!UICONTROL Entscheidungen]:** Wählen Sie Optionen aus, um zu bestimmen, ob nur Testsendungen durchgeführt wurden, die bestimmte Entscheidungen enthalten.\
   **[!UICONTROL Empfänger]:** Wählen Sie einzelne Benutzer aus, um Informationen zu Testsendungen anzuzeigen, die für die ausgewählten Benutzer freigegeben wurden.\
   **[!UICONTROL Testversand-Inhaber]:** Wählen Sie einzelne Benutzer aus, um Informationen zu Testsendungen der ausgewählten Benutzer anzuzeigen.\
   **[!UICONTROL Testversand-Ersteller]:** Wählen Sie einzelne Benutzer aus, um Informationen zu Testsendungen anzuzeigen, die von den ausgewählten Benutzern erstellt wurden.\
   **[!UICONTROL Konten]:** Wählen Sie die Konten aus, die Sie in den Bericht aufnehmen möchten.

1. Klicken Sie auf **[!UICONTROL Anwenden]**.
1. (Optional) Aktivieren oder deaktivieren Sie die Option **[!UICONTROL Min-Max-Bereich anzeigen]** , um zu bestimmen, ob Mindest- und Höchstwerte im Diagramm angezeigt werden.\
   Wenn diese Option aktiviert ist, wird zwischen den minimalen und maximalen aufgezeichneten Werten eine blaue Schattierung angezeigt.

## Berichte drucken

1. Rufen Sie die Seite **[!UICONTROL Dashboards]** auf.
1. Klicken Sie auf die Registerkarte **[!UICONTROL Berichte]** und dann auf **[!UICONTROL Drucken]**.\
   ![proof_reports_print.png](assets/proof-reports-print-350x191.png)

1. Wählen Sie aus den verschiedenen verfügbaren Druckoptionen aus.\
   Die Druckoptionen variieren je nach verwendetem Browser und Browser.
