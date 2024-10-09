---
content-type: overview;reference
product-area: reports and dashboards
navigation-topic: data connect
title: Anzeigen der Workfront Data Connect-Nutzungsmetriken
description: Auf der Registerkarte Workfront-Datenverbindungs-Metriken können Sie die Nutzungsmetriken Ihres Unternehmens sowohl nach den monatlichen Berechnungsstunden als auch nach der Anzahl der durchgeführten Abfragen anzeigen.
author: Nolan
feature: Reports and Dashboards
source-git-commit: 4c8b7e7f33ec593b2942725eb9160f7fbe2962e3
workflow-type: tm+mt
source-wordcount: '346'
ht-degree: 1%

---

# Anzeigen der [!DNL Workfront Data Connect]-Nutzungsmetriken

Auf der Registerkarte [!DNL Workfront Data Connect] [!UICONTROL Metriken] können Sie die Nutzungsmetriken Ihres Unternehmens sowohl in Bezug auf die verwendeten Berechnungsstunden als auch auf die Anzahl der durchgeführten Abfragen anzeigen. Unternehmen haben eine begrenzte Anzahl monatlicher Berechnungsstunden, die auf der Grundlage ihres Lizenztyps und der Data Connect-Add-on-Käufe verfügbar sind. Auf der Registerkarte [!UICONTROL Metriken] werden Informationen zu den verfügbaren monatlichen Berechnungsstunden in Bezug auf den verwendeten Wert angezeigt.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Abo</td> 
   <td><p>In den folgenden Plänen enthalten:</p>
    <ul>
        <li>Ultimativ</li> 
    </ul>    
   <p>Kann als Zusatzprodukt zu den folgenden Plänen erworben werden:</p> 
    <ul>
        <li>Auswählen</li> 
        <li>Erstklassig</li>
    </ul> 
    <p>Workfront Data Connect ist nicht für ältere Workfront-Pläne verfügbar.</p> 
   </td> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Sie müssen Workfront-Administrator sein.</p></td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Nutzungsmetriken und verfügbare Berechnungsstunden anzeigen

1. Klicken Sie auf das Symbol **[!UICONTROL Hauptmenü]** ![Hauptmenü](/help/_includes/assets/main-menu-icon.png) oben rechts in Adobe Workfront oder (falls verfügbar) auf das Symbol **[!UICONTROL Hauptmenü]**, das Symbol ![Hauptmenü](/help/_includes/assets/main-menu-icon-left-nav.png) oben links und klicken Sie dann auf [!UICONTROL **Setup**].

1. Klicken Sie im linken Bereich auf [!UICONTROL **System**] > [!UICONTROL **Datenzugriff**].

1. Klicken Sie auf die Registerkarte [!UICONTROL **Metriken**]. Ihre Nutzungsmetriken werden im Diagramm **Nutzung berechnen** angezeigt, während die Anzahl der durchgeführten Abfragen im Diagramm **Abfrageanzahl** angezeigt wird.

   ![Nutzungsmetriken zur Datenverbindung](/help/quicksilver/reports-and-dashboards/data-lake/assets/data-connect-usage-metrics.png)

1. (Optional) Sie können das Dropdown-Menü [!UICONTROL **Ansicht auswählen**] verwenden, um den Zeitraum für die in beiden Diagrammen enthaltenen Informationen zu ändern.

1. (Optional) Sie können die Kontrollkästchen über dem Diagramm **Nutzung berechnen** verwenden, um Folgendes ein- oder auszublenden:
   * [!UICONTROL **Tägliche Berechnungsstunden**] - Die Anzahl der Berechnungsstunden, die Ihr Unternehmen täglich verwendet.
   * [!UICONTROL **Monatliche kumulative Berechnungsstunden**] - Die Gesamtzahl der Berechnungsstunden, die Ihr Unternehmen in einem Monat verwendet hat. Setzt jeden Monat auf null zurück.
   * [!UICONTROL **Monatlicher Compute Hour Allowance**] - Die Anzahl der Berechnungsstunden, die Ihrem Unternehmen aufgrund von Lizenz- und/oder Add-On-Käufen zur Verfügung stehen.
