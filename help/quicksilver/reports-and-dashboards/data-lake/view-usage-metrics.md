---
content-type: overview;reference
product-area: reports and dashboards
navigation-topic: data connect
title: Anzeigen von Workfront Data Connect-Nutzungsmetriken
description: Auf der Registerkarte Workfront Data Connect-Metriken können Sie die Nutzungsmetriken Ihres Unternehmens sowohl nach den monatlichen Rechenstunden als auch nach der Anzahl der durchgeführten Abfragen anzeigen.
author: Nolan
feature: Reports and Dashboards
exl-id: 29185bd1-e058-4b42-a508-53406fb9ddd2
source-git-commit: ea9c674b798c48927c7a0a542d36d5ded15ea3f1
workflow-type: tm+mt
source-wordcount: '334'
ht-degree: 0%

---

# Anzeigen [!DNL Workfront Data Connect] Nutzungsmetriken

Auf der Registerkarte [!DNL Workfront Data Connect] [!UICONTROL Metriken] können Sie die Nutzungsmetriken Ihres Unternehmens sowohl nach verwendeten Rechenstunden als auch nach der Anzahl der durchgeführten Abfragen anzeigen. Unternehmen verfügen je nach Lizenztyp und Add-on-Käufen für Data Connect über eine begrenzte Anzahl monatlicher Rechenstunden. Auf [!UICONTROL  Registerkarte ]Metriken“ werden Informationen zu den verfügbaren monatlichen Berechnungsstunden im Verhältnis zu den verwendeten Werten angezeigt.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan</td> 
   <td><p>In den folgenden Plänen enthalten:</p>
    <ul>
        <li>Ultimativ</li> 
    </ul>    
   <!--<p>Can be purchased as an add-on to the following plans:</p> 
    <ul>
        <li>Select</li> 
        <li>Prime</li>
    </ul>--> 
    <p>Workfront Data Connect ist nicht für veraltete Workfront-Pläne verfügbar.</p> 
   </td> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td><p>Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Sie müssen ein Workfront-Administrator sein.</p></td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Anzeigen von Nutzungsmetriken und verfügbaren Berechnungsstunden

1. Klicken Sie auf das **[!UICONTROL Hauptmenü]**-Symbol ![Hauptmenü](/help/_includes/assets/main-menu-icon.png) in der oberen rechten Ecke von Adobe Workfront oder (falls verfügbar) klicken Sie auf das **[!UICONTROL Hauptmenü]**-Symbol ![Hauptmenü](/help/_includes/assets/main-menu-icon-left-nav.png) in der oberen linken Ecke und klicken Sie dann auf [!UICONTROL **Setup**].

1. Klicken Sie im linken Bedienfeld auf [!UICONTROL **System**] > [!UICONTROL **Datenzugriff**].

1. Klicken Sie auf die Registerkarte [!UICONTROL **Metriken**]. Ihre Nutzungsmetriken werden im Diagramm **Nutzung berechnen** angezeigt, während die Anzahl der durchgeführten Abfragen im Diagramm **Abfragenanzahl** angezeigt wird.

   ![Metriken zur Datennutzung](/help/quicksilver/reports-and-dashboards/data-lake/assets/data-connect-usage-metrics.png)

1. (Optional) Sie können das Dropdown-Menü [!UICONTROL **Ansicht auswählen**] verwenden, um den Zeitbereich für die in beiden Diagrammen enthaltenen Informationen zu ändern.

1. (Optional) Sie können die Kontrollkästchen über dem Diagramm **Nutzung berechnen** zum Ein- oder Ausblenden verwenden:
   * [!UICONTROL **Tägliche Berechnungsstunden**] - Die Anzahl der von Ihrem Unternehmen täglich verwendeten Berechnungsstunden.
   * [!UICONTROL **Kumulative monatliche**]: Die Gesamtzahl der von Ihrer Organisation in einem Monat verwendeten Berechnungsstunden. Setzt jeden Monat auf null zurück.
   * [!UICONTROL **Monatliches Compute-Stundenkontingent**] - Die Anzahl der Compute-Stunden, die Ihrem Unternehmen auf der Grundlage von Lizenz- und/oder Add-on-Käufen zur Verfügung stehen.
