---
content-type: overview
product-area: workfront-integrations
navigation-topic: workfront-for-salesforce
title: Übersicht über Adobe Workfront für Salesforce
description: Sie können [!DNL Adobe Workfront] für Salesforce, damit Ihre Salesforce-Benutzer die [!DNL Workfront] -Anfragen und automatisch Projekte erstellen, ohne Salesforce verlassen zu müssen.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 65d4cdae-1d34-4a8a-a1c0-706cd41fc75e
source-git-commit: 5b889633a96d634a359181bfd53ec106b0f3705c
workflow-type: tm+mt
source-wordcount: '436'
ht-degree: 0%

---

# [!DNL Adobe Workfront for Salesforce] Übersicht

A [!UICONTROL Pro] [!DNL Workfront] Für die Verwendung dieser Funktion ist ein Plan erforderlich. Weitere Informationen zu den verschiedenen verfügbaren Plänen finden Sie unter [[!DNL Workfront] Pläne.](https://www.workfront.com/plans)

Sie können [!DNL Adobe Workfront for Salesforce] , um [!DNL Salesforce] Benutzer zum Senden [!DNL Workfront] Anforderungen und automatisches Erstellen von Projekten ohne Hinterlassen [!DNL Salesforce].

Als [!DNL Workfront] Administrator, können Sie [!DNL Workfront for Salesforce]. Dann können Sie sie für alle anderen freigeben [!DNL Salesforce] Benutzer.

Weitere Informationen zur Installation [!DNL Workfront for Salesforce], siehe [Installieren [!DNL Adobe Workfront for Salesforce]](../../workfront-integrations-and-apps/using-workfront-with-salesforce/install-workfront-for-salesforce.md).\
Weitere Informationen zur Konfiguration der [!DNL Workfront] Abschnitt in [!DNL Salesforce] Für alle Benutzer finden Sie unter [Konfigurieren Sie die [!DNL Adobe Workfront] Abschnitt für [!DNL Salesforce] Benutzer](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md).

## Zugriffsanforderungen

Sie müssen über den folgenden Zugriff verfügen, um die in diesem Artikel beschriebene Funktion verwenden zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Plan*</td> 
   <td> <p>[!UICONTROL Pro] oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td> <p>[!UICONTROL Plan]</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren [!DNL Workfront] Administrator.

## [!DNL Workfront for Salesforce]

Wenn Sie [!DNL Workfront for Salesforce]:

* Manuelles Erstellen neuer [!DNL Workfront] Anforderungen von [!DNL Salesforce] innerhalb einer Gelegenheit oder eines Kontos.

   Weitere Informationen zur Erstellung von [!DNL Workfront] Anforderungen von [!DNL Salesforce], siehe [Einsenden [!DNL Adobe Workfront] Anforderungen von [!DNL Salesforce] Objekte](../../workfront-integrations-and-apps/using-workfront-with-salesforce/submit-workfront-requests-from-salesforce-objects.md).

* Automatische Trigger der Projekterstellung in [!DNL Workfront] wenn bestimmte Kriterien in [!DNL Salesforce]. Ihre [!DNL Salesforce] Der Systemadministrator muss Trigger zum Erstellen von Projekten aus konfigurieren [!DNL Salesforce].

   Weitere Informationen zur Erstellung von [!DNL Workfront] Projekte aus [!DNL Salesforce], siehe [Erstellen [!DNL Adobe Workfront] Projekte aus [!DNL Salesforce] Objekte](../../workfront-integrations-and-apps/using-workfront-with-salesforce/create-wf-projects-from-salesforce-objects.md).

Beachten Sie beim Arbeiten mit [!DNL Workfront] für [!DNL Salesforce]:

* Wir unterstützen beide [!DNL Salesforce Classic] und [!DNL Lightning Experience] Frameworks.
* Elemente können nur aus [!DNL Salesforce] in [!DNL Workfront].
* Sie können einige Informationen zu den [!DNL Workfront] Elemente in [!DNL Salesforce].

   Diese Informationen können nicht angepasst werden.

   Für eine Liste von [!DNL Workfront] Felder, die angezeigt werden können [!DNL Salesforce], siehe  [Einsenden [!DNL Adobe Workfront] Anforderungen von [!DNL Salesforce] Objekte](../../workfront-integrations-and-apps/using-workfront-with-salesforce/submit-workfront-requests-from-salesforce-objects.md)  und [Erstellen [!DNL Adobe Workfront] Projekte aus [!DNL Salesforce] Objekte](../../workfront-integrations-and-apps/using-workfront-with-salesforce/create-wf-projects-from-salesforce-objects.md).

* Sie können direkt auf Elemente zugreifen, die mit [!DNL Salesforce] durch Klicken auf **[!UICONTROL Gehe zu Salesforce]** von Workfront aus.

   Sie können keine Informationen zu den [!DNL Salesforce] Elemente in [!DNL Workfront], aber Sie haben einen Link zum [!UICONTROL Salesforce] Element aus [!DNL Workfront] , um sie in [!DNL Salesforce].

   [!UICONTROL Die **Gehe zu Salesforce**] -Link wird in den folgenden Bereichen angezeigt:

   * Die [!UICONTROL Details] Abschnitt eines Projekts oder eines Problems
   * Die Kopfzeile eines Projekts oder eines Problems.

      Ihr System- oder Gruppenadministrator muss [!UICONTROL Integrationen] -Feld zu Ihrer Layout-Vorlage hinzufügen, um [!UICONTROL Gehe zu Salesforce] -Link in der Projekt- oder Problemüberschrift.
   * Die [!DNL Summary] ein Problem bei der Auswahl des Problems in einer Liste durch Klicken auf [!UICONTROL Zusammenfassung öffnen] ![](assets/summary-panel-icon.png) in der Symbolleiste der Liste.

      >[!NOTE]
      >
      >Die [!UICONTROL Gehe zu Salesforce] Link für alle sichtbar [!DNL Workfront] Benutzer, die das Projekt oder das Problem anzeigen können. Sie müssen über eine [!DNL Salesforce] -Konto, um zur [!DNL Salesforce] Gelegenheit oder Konto, bei dem das Problem protokolliert wurde.

* Durch die Aktualisierung von Feldern auf einem Element in einer Anwendung werden Informationen zu verknüpften Elementen in der anderen Anwendung nicht aktualisiert.
