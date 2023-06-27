---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: connections-annd-webhooks
title: Über die Verbindung [!DNL Adobe Workfront Fusion] an eine App oder einen Dienst
description: Für die meisten Apps ist es erforderlich, eine Verbindung zu erstellen, durch die [!DNL Adobe Workfront Fusion] kann mit dem angegebenen Drittanbieterdienst gemäß den Einstellungen des jeweiligen Szenarios kommunizieren.
author: Becky
feature: Workfront Fusion
exl-id: 2d5cf083-9893-45e8-8f7d-0f8f5a74eef3
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '402'
ht-degree: 0%

---

# Über die Verbindung [!DNL Adobe Workfront Fusion] an eine App oder einen Dienst

Für die meisten Apps ist es erforderlich, eine Verbindung zu erstellen, durch die [!DNL Adobe Workfront Fusion] kann mit dem angegebenen Drittanbieterdienst gemäß den Einstellungen des jeweiligen Szenarios kommunizieren.

Beispiel: Wenn Sie ein Szenario erstellen möchten, das Informationen aus [!DNL Workfront]müssen Sie Zugriffsberechtigungen für [!DNL Workfront Fusion] , um auf [!DNL Workfront] -Konto.

## Zugriffsanforderungen

Sie müssen über den folgenden Zugriff verfügen, um die in diesem Artikel enthaltene Funktionalität nutzen zu können:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Plan*</td> 
   <td> <p>[!UICONTROL Pro] oder höher</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Arbeit]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] license**</td> 
   <td>
   <p>Aktuelle Lizenzanforderungen: Nein [!DNL Workfront Fusion] Lizenzanforderungen.</p>
   <p>Oder</p>
   <p>Ältere Lizenzanforderungen: [!UICONTROL [!DNL Workfront Fusion] für Arbeitsautomatisierung und Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>
   <p>Aktuelle Produktanforderungen: Wenn Sie über [!UICONTROL Select] oder [!UICONTROL Prime] verfügen [!DNL Adobe Workfront] Planung, Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] sowie [!DNL Adobe Workfront] , um die in diesem Artikel beschriebenen Funktionen zu verwenden. [!DNL Workfront Fusion] ist in [!UICONTROL Ultimate] enthalten. [!DNL Workfront] Plan.</p>
   <p>Oder</p>
   <p>Ältere Produktanforderungen: Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] sowie [!DNL Adobe Workfront] , um die in diesem Artikel beschriebenen Funktionen zu verwenden.</p>
   </td> 
  </tr>
 </tbody> 
</table>

Wenden Sie sich an Ihren [!DNL Workfront] Administrator.

Informationen über [!DNL Adobe Workfront Fusion] Lizenzen, siehe [[!DNL Adobe Workfront Fusion] Lizenzen](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Zugriffsberechtigungen

Für jede Verbindung [!DNL Workfront Fusion] erfordert nur die Zugriffsrechte, die für den erfolgreichen Abschluss eines bestimmten Szenarios erforderlich sind. Wenn Sie beispielsweise ein Szenario zum Auflisten von Dokumenten aus erstellen [!DNL Google Docs], [!DNL Workfront Fusion] fordert keine Berechtigung zum Abrufen des Inhalts der Dokumente an.

Leider können Sie nicht alle Dienste den Zugriff auf bestimmte Aufgaben beschränken. Daher [!DNL Workfront Fusion] muss vollständige Zugriffsberechtigungen erfordern. Weitere Informationen zur Beschränkung von [!DNL Workfront Fusion] Zugriff auf Ihr Konto, das für diese Dienste registriert ist, finden Sie in der anwendungsspezifischen Dokumentation.

## Über die Verwaltung von Verbindungen

Sie können alle Verbindungen über die [!UICONTROL Verbindungen] Bereich. Hier haben Sie folgende Möglichkeiten:

* Ermitteln, welche Berechtigungen erteilt wurden [!DNL Workfront Fusion] für jede Verbindung
* Umbenennen von Verbindungen
* Vorhandene Verbindungen erneut autorisieren
* Vorhandene Verbindungen löschen
* Überprüfen, ob die Verbindung zum Dienst erfolgreich hergestellt wurde

So öffnen Sie die [!UICONTROL Verbindungen] Bereich, klicken Sie <b>[!UICONTROL Verbindungen]</b> in der linken Navigation.

## Verbindung erneuern

[!DNL Workfront Fusion] erhält normalerweise unbegrenzte Zugriffsrechte auf einen bestimmten Dienst. Dies ist jedoch nicht immer der Fall. Bei einigen Diensten muss die Zugriffsberechtigung nach einem bestimmten Zeitraum verlängert werden. In diesen Fällen [!DNL Workfront Fusion] werden Sie kurz vor Ablauf der Zugriffsberechtigungen per E-Mail benachrichtigt.

So erneuern Sie eine Verbindung:

1. Klicken Sie auf **[!UICONTROL Neu autorisieren]** im **[!UICONTROL Verbindungen]** Bereich.
