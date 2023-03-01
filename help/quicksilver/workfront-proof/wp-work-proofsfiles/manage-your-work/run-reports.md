---
product-previous: workfront-proof
product-area: documents
navigation-topic: manage-your-work-workfront-proof
title: Ausführen von Berichten in [!DNL Workfront Proof]
description: Workfront-Testversand ermöglicht es Ihnen, Berichte anzuzeigen, damit Sie den Arbeitsfortschritt und die Effizienz Ihrer Teams verfolgen können.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 342f9282-b6f5-425e-a7ef-e23bd011d284
source-git-commit: a0d76692f9e9d12ed0d538c1344638dbc208d625
workflow-type: tm+mt
source-wordcount: '691'
ht-degree: 0%

---

# Ausführen von Berichten in [!DNL Workfront Proof]


>[!IMPORTANT]
>
>* <span class="previe">Die Berichtsfunktion ist in nicht mehr verfügbar [!DNL Workfront Proof]. Der Tab Berichterstellung wird weiterhin angezeigt, die Daten sind jedoch nicht präzise.</span>
> 
>* Dieser Artikel bezieht sich auf die Funktionalität im eigenständigen Produkt [!DNL Workfront Proof]. Informationen zum Testen in [!DNL Adobe Workfront], siehe [Testversand](../../../review-and-approve-work/proofing/proofing.md).


Workfront-Testversand ermöglicht es Ihnen, Berichte anzuzeigen, damit Sie den Arbeitsfortschritt und die Effizienz Ihrer Teams verfolgen können.

Sie können die Anzahl der in Ihren [!DNL Workfront Proof] -Konto, wie viele Versionen mit jedem Testversand verknüpft sind, die Bearbeitungszeit und mehr.

## Voraussetzungen

Ob Berichte verfügbar sind, hängt von Ihrem Typ ab [!DNL Workfront Proof] -Konto und Benutzerberechtigungsebenen.

* [Kontovoraussetzungen](#account-prerequisites)
* [Benutzervoraussetzungen](#user-prerequisites)

### Kontovoraussetzungen {#account-prerequisites}

Berichtinformationen sind nur bei Premium-Plänen verfügbar.

### Benutzervoraussetzungen {#user-prerequisites}

Die Berichtinformationen stehen nur Benutzern mit uneingeschränktem Zugriff auf alle Testsendungen in Ihrem Konto zur Verfügung (d. h. Benutzern mit mindestens [Profile für Testberechtigungen in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md)).

In diesem Bereich können Sie

* Zeitspanne der angezeigten Daten steuern
* Änderungen an Metriken im Zeitverlauf analysieren
* Überprüfen Sie die Details eines ausgewählten Zeitpunkts, indem Sie den Mauszeiger darüber bewegen.
* Überprüfen Sie die Gesamtzahl der in Ihrem ausgewählten Zeitraum erstellten Testsendungen.
* Überprüfen Sie die durchschnittliche Anzahl der Versionen, die in den abgeschlossenen Testsendungen enthalten sind.

## Anzeigen von Berichten {#viewing-reports}

1. Navigieren Sie zu **[!UICONTROL Dashboards]** Seite.
1. Klicken Sie auf **[!UICONTROL Berichte]** Registerkarte.\
   ![proof_reports.png](assets/proof-reports-350x193.png)

1. Im **[!UICONTROL Zeitrahmen]** Wählen Sie aus dem Dropdown-Menü aus, ob Sie Informationen zu den in den letzten 24 Stunden, 7 Tagen, 30 Tagen, 90 Tagen oder einem benutzerdefinierten Zeitraum erstellten Testsendungen anzeigen möchten.\
   Wenn Sie einen benutzerdefinierten Zeitraum auswählen, wählen Sie das Start- und Enddatum aus und klicken Sie auf **[!UICONTROL Anwenden]**.\
   Die folgenden Informationen werden für den ausgewählten Zeitraum angezeigt:\
   **Testversand erstellt:** Anzahl der innerhalb des ausgewählten Zeitraums erstellten Testsendungen.\
   **Versionen pro Testversand:** Durchschnittliche Anzahl der Versionen pro Testversand für alle abgeschlossenen Testsendungen (Genehmigt oder Genehmigt mit Änderungen) innerhalb des ausgewählten Zeitraums.\
   **Um Zeit drehen:** Durchschnittliche Zeit ab der Erstellung der ersten Version bis zum Zeitpunkt der Entscheidungsfindung für die endgültige Version.\
   **Erstmalige Aktivität:** Durchschnittliche Zeit ab der Erstellung des Testversands bis zur ersten Aktivität des Testversands.\
   **Testsendungen verspätet:** Durchschnittlicher Prozentsatz abgeschlossener Testsendungen (Genehmigt oder Genehmigt mit Änderungen) mit mindestens einer Version, die im ausgewählten Zeitraum zu spät war.\
   **Kommentare und Antworten:** Durchschnittliche Anzahl der Kommentare und Antworten, die zu allen Testsendungen innerhalb des ausgewählten Zeitraums abgegeben wurden.

1. (Optional) Aktivieren oder deaktivieren Sie die **[!UICONTROL Min.-Max-Bereich anzeigen]** -Option, um zu bestimmen, ob Mindest- und Höchstwerte im Diagramm angezeigt werden.\
   Wenn diese Option aktiviert ist, wird zwischen den minimalen und maximalen aufgezeichneten Werten eine blaue Schattierung angezeigt.

1. (Optional) Sie können die angezeigten Daten filtern, wie unter [Filtern von Berichten](#filtering-reports).

## Filtern von Berichten {#filtering-reports}

Standardmäßig enthalten in Berichten angezeigte Daten alle Informationen aus Ihrer [!DNL Workfront Proof] System. Sie können Filter verwenden, um nur Informationen anzuzeigen, die für Ihre Anforderungen relevant sind.

So filtern Sie Berichtsinformationen:

1. Navigieren Sie zu **[!UICONTROL Dashboards]** Seite.
1. Klicken Sie auf **[!UICONTROL Berichte]** Registerkarte.\
   ![proof_reports.png](assets/proof-reports-350x193.png)

1. Führen Sie einen Bericht aus, wie unter [Anzeigen von Berichten](#viewing-reports).
1. Klicken **[!UICONTROL Filter]**.

1. Wählen Sie auf der linken Seite der Seite aus den folgenden Filteroptionen:\
   **[!UICONTROL Testversand-Typ]:** Wählen Sie den Testversand-Typ aus, der in den Bericht aufgenommen werden soll.\
   **[!UICONTROL Entscheidungen]:** Wählen Sie Optionen aus, um festzulegen, ob nur Testsendungen durchgeführt wurden, die bestimmte Entscheidungen enthalten.\
   **[!UICONTROL Empfänger]:** Wählen Sie einzelne Benutzer aus, um Informationen zu Testsendungen anzuzeigen, die für die ausgewählten Benutzer freigegeben wurden.\
   **[!UICONTROL Testversand-Eigentümer]:** Wählen Sie einzelne Benutzer aus, um Informationen zu Testsendungen der ausgewählten Benutzer anzuzeigen.\
   **[!UICONTROL Ersteller von Testsendungen]:** Wählen Sie einzelne Benutzer aus, um Informationen zu Testsendungen anzuzeigen, die von den ausgewählten Benutzern erstellt wurden.\
   **[!UICONTROL Konten]:** Wählen Sie aus, welche Konten Sie in den Bericht aufnehmen möchten.

1. Klicken **[!UICONTROL Anwenden]**.
1. (Optional) Aktivieren oder deaktivieren Sie die **[!UICONTROL Min.-Max-Bereich anzeigen]** -Option, um zu bestimmen, ob Mindest- und Höchstwerte im Diagramm angezeigt werden.\
   Wenn diese Option aktiviert ist, wird zwischen den minimalen und maximalen aufgezeichneten Werten eine blaue Schattierung angezeigt.

## Berichte drucken

1. Navigieren Sie zu **[!UICONTROL Dashboards]** Seite.
1. Klicken Sie auf **[!UICONTROL Berichte]** Registerkarte und klicken Sie dann auf **[!UICONTROL Drucken]**.\
   ![proof_reports_print.png](assets/proof-reports-print-350x191.png)

1. Wählen Sie aus den verschiedenen verfügbaren Druckoptionen aus.\
   Die Druckoptionen variieren je nach verwendetem Browser und Browser.
