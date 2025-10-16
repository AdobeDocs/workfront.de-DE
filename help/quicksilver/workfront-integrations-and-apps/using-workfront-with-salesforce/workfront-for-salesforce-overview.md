---
content-type: overview
product-area: workfront-integrations
navigation-topic: workfront-for-salesforce
title: Übersicht über Adobe Workfront für Salesforce
description: Salesforce Sie können für  [!DNL Adobe Workfront]  installieren, damit Ihre Salesforce-Benutzenden Anfragen senden  [!DNL Workfront]  automatisch Projekte erstellen können, ohne Salesforce verlassen zu müssen.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 65d4cdae-1d34-4a8a-a1c0-706cd41fc75e
source-git-commit: 85ccee879fd4ba5a80b6e885458839901f83d26e
workflow-type: tm+mt
source-wordcount: '495'
ht-degree: 1%

---

# Übersicht über [!DNL Adobe Workfront for Salesforce]

<!-- Audited: 5/2025 -->

>[!IMPORTANT]
>
>Um stabilere und skalierbarere Integrationen bereitzustellen, wechseln wir mithilfe von Workfront Automation and Integration (Fusion) zu einem modernen, flexiblen Integrationsansatz. Im Rahmen dieses Übergangsprozesses wird die Integration von Workfront mit Salesforce nach dem 28. **2026 nicht mehr**.
>
>Es wird empfohlen, Workfront-Automatisierung und -Integration für die Integrationsanforderungen Ihres Unternehmens mit Salesforce zu verwenden.
>
>Einen Überblick über die Automatisierung und Integration von Workfront finden Sie unter [Übersicht über Adobe Workfront Fusion](https://experienceleague.adobe.com/de/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview).
>
>Informationen zu den spezifischen Funktionen der Workfront-Automatisierungs- und Integrationsmodule für Salesforce finden Sie unter [Salesforce-Module](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/salesforce-modules).

Sie können [!DNL Adobe Workfront for Salesforce] installieren, damit Ihre [!DNL Salesforce]-Benutzer [!DNL Workfront]-Anfragen senden und automatisch Projekte erstellen können, ohne [!DNL Salesforce] verlassen zu müssen.

Als [!DNL Workfront] können Sie [!DNL Workfront for Salesforce] herunterladen und konfigurieren. Anschließend können Sie es für alle anderen [!DNL Salesforce] Benutzer freigeben.

Weitere Informationen zum Installieren von [!DNL Workfront for Salesforce] finden Sie unter [Installieren [!DNL Adobe Workfront for Salesforce]](../../workfront-integrations-and-apps/using-workfront-with-salesforce/install-workfront-for-salesforce.md).

Weitere Informationen zum Konfigurieren des [!DNL Workfront] in [!DNL Salesforce] für alle Benutzer finden Sie unter [Konfigurieren des  [!DNL Adobe Workfront]  für  [!DNL Salesforce] Benutzer](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Paket</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td> <p>Standard</p>
   <p>Plan</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## [!DNL Workfront for Salesforce]

Bei Verwendung von [!DNL Workfront for Salesforce] können Sie Folgendes tun:

* Manuelles Erstellen neuer [!DNL Workfront] aus [!DNL Salesforce] innerhalb einer Opportunity oder eines Kontos.

  Weitere Informationen finden Sie unter [submit [!DNL Adobe Workfront] requests from [!DNL Salesforce] objects](../../workfront-integrations-and-apps/using-workfront-with-salesforce/submit-workfront-requests-from-salesforce-objects.md).

* Die Erstellung von Projekten in [!DNL Workfront] wird automatisch Trigger, wenn bestimmte Kriterien in [!DNL Salesforce] erfüllt sind. Ihr [!DNL Salesforce] muss Trigger konfigurieren, um Projekte aus [!DNL Salesforce] zu erstellen.

  Weitere Informationen zum Erstellen [!DNL Workfront] Projekte aus [!DNL Salesforce] finden Sie unter [Erstellen [!DNL Adobe Workfront] Projekte aus [!DNL Salesforce] Objekten](../../workfront-integrations-and-apps/using-workfront-with-salesforce/create-wf-projects-from-salesforce-objects.md).

Beachten Sie beim Arbeiten mit [!DNL Workfront] für [!DNL Salesforce] Folgendes:

* Wir unterstützen sowohl den [!DNL Salesforce Classic]- als auch den [!DNL Lightning Experience].
* Elemente können nur von [!DNL Salesforce] bis [!DNL Workfront] erstellt werden.
* Sie können einige Informationen zu den [!DNL Workfront] Elementen in [!DNL Salesforce] anzeigen. Diese Informationen können nicht angepasst werden.

  Eine Liste der [!DNL Workfront] Felder, die Sie in [!DNL Salesforce] anzeigen können, finden Sie unter [Senden [!DNL Adobe Workfront] Anfragen von [!DNL Salesforce] Objekten](../../workfront-integrations-and-apps/using-workfront-with-salesforce/submit-workfront-requests-from-salesforce-objects.md) und [Erstellen [!DNL Adobe Workfront] Projekte aus [!DNL Salesforce] Objekten](../../workfront-integrations-and-apps/using-workfront-with-salesforce/create-wf-projects-from-salesforce-objects.md).

* Sie können direkt auf Elemente zugreifen, die mit [!DNL Salesforce] verknüpft sind, indem Sie in Workfront auf [!UICONTROL &#x200B; Link &#x200B;]Zu Salesforce gehen“ klicken.

  Sie können keine Informationen zu den [!DNL Salesforce] Elementen in [!DNL Workfront] anzeigen. Über einen Link in Workfront gelangen Sie jedoch zu dem Element in Salesforce, damit Sie es dort überprüfen können.

  [!UICONTROL Der Link Wechseln zu Salesforce] wird in den folgenden Bereichen angezeigt:

   * Der [!UICONTROL Details] eines Projekts oder einer Anfrage.
   * Die Kopfzeile eines Projekts oder eines Problems.

     Ihr System- oder Gruppenadministrator muss das Feld [!UICONTROL Integrationen] zu Ihrer Layout-Vorlage hinzufügen, um den Link [!UICONTROL Zu Salesforce wechseln] in der Kopfzeile des Projekts oder Problems anzuzeigen.
   * Das [!DNL Summary] Bedienfeld eines Problems, wenn Sie das Problem in einer Liste auswählen, nachdem Sie auf [!UICONTROL Zusammenfassung öffnen] ![Symbol des Zusammenfassungsbereichs](assets/summary-panel-icon.png) in der Symbolleiste der Liste geklickt haben.

     >[!NOTE]
     >
     >Der [!UICONTROL Zu Salesforce wechseln]-Link ist für alle [!DNL Workfront] Benutzer sichtbar, die das Projekt oder das Problem anzeigen können. Sie müssen über ein [!DNL Salesforce]-Konto verfügen, um zu dem Opportunity-Konto oder [!DNL Salesforce]-Konto gehen zu können, in dem das Problem protokolliert wurde.

* Beim Aktualisieren von Feldern eines Elements in einem Programm werden keine Informationen zu verknüpften Elementen in dem anderen Programm aktualisiert.
