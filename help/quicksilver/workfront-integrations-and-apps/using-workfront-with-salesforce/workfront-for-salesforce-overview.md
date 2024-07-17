---
content-type: overview
product-area: workfront-integrations
navigation-topic: workfront-for-salesforce
title: Übersicht über Adobe Workfront für Salesforce
description: Sie können [!DNL Adobe Workfront] für Salesforce installieren, damit Ihre Salesforce-Benutzer  [!DNL Workfront] Anforderungen senden und automatisch Projekte erstellen können, ohne Salesforce verlassen zu müssen.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 65d4cdae-1d34-4a8a-a1c0-706cd41fc75e
source-git-commit: 5b889633a96d634a359181bfd53ec106b0f3705c
workflow-type: tm+mt
source-wordcount: '434'
ht-degree: 0%

---

# [!DNL Adobe Workfront for Salesforce] Übersicht

Für die Verwendung dieser Funktion ist ein [!UICONTROL Pro] [!DNL Workfront] Plan erforderlich. Weitere Informationen zu den verschiedenen verfügbaren Plänen finden Sie unter [[!DNL Workfront] Pläne.](https://www.workfront.com/plans)

Sie können [!DNL Adobe Workfront for Salesforce] installieren, damit Ihre [!DNL Salesforce] -Benutzer [!DNL Workfront] -Anforderungen senden und automatisch Projekte erstellen können, ohne je [!DNL Salesforce] verlassen zu müssen.

Als [!DNL Workfront] -Administrator können Sie [!DNL Workfront for Salesforce] herunterladen und konfigurieren. Anschließend können Sie es für alle anderen [!DNL Salesforce] -Benutzer freigeben.

Weitere Informationen zum Installieren von [!DNL Workfront for Salesforce] finden Sie unter [Installieren [!DNL Adobe Workfront for Salesforce]](../../workfront-integrations-and-apps/using-workfront-with-salesforce/install-workfront-for-salesforce.md).\
Weitere Informationen zum Konfigurieren des Bereichs [!DNL Workfront] in [!DNL Salesforce] für alle Benutzer finden Sie unter [Konfigurieren des Abschnitts  [!DNL Adobe Workfront] für  [!DNL Salesforce] Benutzer](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md).

## Zugriffsanforderungen

Sie müssen über den folgenden Zugriff verfügen, um die in diesem Artikel beschriebene Funktion verwenden zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!UICONTROL Pro] oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td> <p>[!UICONTROL Plan]</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren [!DNL Workfront] -Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## [!DNL Workfront for Salesforce]

Bei Verwendung von [!DNL Workfront for Salesforce] können Sie Folgendes tun:

* Erstellen Sie manuell neue [!DNL Workfront] -Anforderungen von [!DNL Salesforce] innerhalb einer Chance oder eines Kontos.

  Weitere Informationen zum Erstellen von [!DNL Workfront] -Anforderungen aus [!DNL Salesforce] finden Sie unter [Senden [!DNL Adobe Workfront] von Anforderungen von  [!DNL Salesforce] Objekten](../../workfront-integrations-and-apps/using-workfront-with-salesforce/submit-workfront-requests-from-salesforce-objects.md).

* Trigger der Projekterstellung in [!DNL Workfront] automatisch, wenn bestimmte Kriterien in [!DNL Salesforce] erfüllt sind. Ihr [!DNL Salesforce] -Systemadministrator muss Trigger zum Erstellen von Projekten aus [!DNL Salesforce] konfigurieren.

  Weitere Informationen zum Erstellen von [!DNL Workfront] Projekten aus [!DNL Salesforce] finden Sie unter [Erstellen [!DNL Adobe Workfront] von Projekten aus  [!DNL Salesforce] Objekten](../../workfront-integrations-and-apps/using-workfront-with-salesforce/create-wf-projects-from-salesforce-objects.md).

Beachten Sie Folgendes beim Arbeiten mit [!DNL Workfront] für [!DNL Salesforce]:

* Wir unterstützen sowohl die Frameworks [!DNL Salesforce Classic] als auch [!DNL Lightning Experience].
* Elemente können nur von [!DNL Salesforce] in bis [!DNL Workfront] erstellt werden.
* Sie können einige Informationen über die [!DNL Workfront] Elemente in [!DNL Salesforce] anzeigen.

  Diese Informationen können nicht angepasst werden.

  Eine Liste der [!DNL Workfront]-Felder, die Sie in [!DNL Salesforce] anzeigen können, finden Sie unter [Senden [!DNL Adobe Workfront] von Anforderungen von  [!DNL Salesforce] Objekten](../../workfront-integrations-and-apps/using-workfront-with-salesforce/submit-workfront-requests-from-salesforce-objects.md) und [Erstellen [!DNL Adobe Workfront] von Projekten aus [!DNL Salesforce] Objekten](../../workfront-integrations-and-apps/using-workfront-with-salesforce/create-wf-projects-from-salesforce-objects.md).

* Sie können direkt auf mit [!DNL Salesforce] verknüpfte Elemente zugreifen, indem Sie in Workfront auf den Link **[!UICONTROL Gehe zu Salesforce]** klicken.

  Sie können keine Informationen über die [!DNL Salesforce] Elemente in [!DNL Workfront] anzeigen, aber Sie haben einen Link zum Element [!UICONTROL Salesforce] von [!DNL Workfront], um es in [!DNL Salesforce] zu überprüfen.

  [!UICONTROL Der Link **Gehe zu Salesforce**] wird in den folgenden Bereichen angezeigt:

   * Der Abschnitt [!UICONTROL Details] eines Projekts oder eines Problems
   * Die Kopfzeile eines Projekts oder eines Problems.

     Ihr System- oder Gruppenadministrator muss das Feld [!UICONTROL Integrationen] zu Ihrer Layout-Vorlage hinzufügen, um den Link [!UICONTROL Gehe zu Salesforce] im Projekt- oder Problemkopf anzuzeigen.
   * Das Bedienfeld [!DNL Summary] eines Problems bei der Auswahl des Problems in einer Liste, nachdem in der Symbolleiste der Liste auf [!UICONTROL Zusammenfassung öffnen] ![](assets/summary-panel-icon.png) geklickt wurde.

     >[!NOTE]
     >
     >Der Link [!UICONTROL Gehe zu Salesforce] ist für alle [!DNL Workfront] Benutzer sichtbar, die das Projekt oder das Problem anzeigen können. Sie müssen über ein [!DNL Salesforce] -Konto verfügen, um zur [!DNL Salesforce] Gelegenheit oder zum Konto wechseln zu können, bei der das Problem protokolliert wurde.

* Durch die Aktualisierung von Feldern auf einem Element in einer Anwendung werden Informationen zu verknüpften Elementen in der anderen Anwendung nicht aktualisiert.
