---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: connections-annd-webhooks
title: Verbindungen - Übersicht
description: Für die meisten Apps ist es erforderlich, eine Verbindung zu erstellen, durch die [!DNL Adobe Workfront Fusion] kann mit dem angegebenen Drittanbieterdienst gemäß den Einstellungen des jeweiligen Szenarios kommunizieren.
author: Becky
feature: Workfront Fusion
exl-id: 2d5cf083-9893-45e8-8f7d-0f8f5a74eef3
source-git-commit: b90343eab40e91c6f5cddeaa960ce9c9c97b1d29
workflow-type: tm+mt
source-wordcount: '616'
ht-degree: 0%

---

# Verbindungen - Übersicht

<!-- Audited: 3/2024-->

Für die meisten Apps gilt Folgendes: [!DNL Workfront Fusion] erfordert eine Verbindung, über die es mit dem angegebenen Drittanbieterdienst gemäß den Einstellungen des jeweiligen Szenarios kommunizieren kann.

Beispiel: Wenn Sie ein Szenario erstellen möchten, das Informationen aus [!DNL Workfront]müssen Sie Zugriffsberechtigungen für [!DNL Workfront Fusion] , um auf [!DNL Workfront] -Konto.

Eine Verbindung stellt die Autorisierung und Berechtigungen dar, die Fusion für den Zugriff auf die Anwendung verwendet. Sie können für jede Anwendung eine oder mehrere Verbindungen erstellen und dieselbe Verbindung in mehreren Modulen oder Szenarien verwenden.

Die meisten Verbindungen werden nur für eine einzelne Anwendung verwendet. Beispiel: eine [!DNL Workfront] Verbindung kann nicht in einer [!UICONTROL Salesforce] -Modul. Einige [!DNL Adobe] Anwendungen können Verbindungen freigeben. Weitere Informationen finden Sie in den Artikeln für diese Anwendungen, aufgeführt in [Apps und ihre Module](/help/quicksilver/workfront-fusion/apps-and-their-modules/apps-and-their-modules.md).

Verbindungen werden auf Teamebene verwaltet. Alle Mitglieder eines Teams haben Zugriff auf die Verbindungen des Teams und Benutzer außerhalb eines Teams haben keinen Zugriff auf die Verbindungen des Teams.

## Zugriffsanforderungen

Sie müssen über den folgenden Zugriff verfügen, um die Funktionalität in diesem Artikel verwenden zu können:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Plan</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] Lizenz</td> 
   <td> <p>Neu: [!UICONTROL Standard]</p><p>Oder</p><p>Aktuell: [!UICONTROL Arbeit] oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] license**</td> 
   <td>
   <p>Aktuell: Nein [!DNL Workfront Fusion] Lizenzanforderungen.</p>
   <p>Oder</p>
   <p>Veraltet: Beliebig </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>
   <p>Neu:</p> <ul><li>[!UICONTROL Select] oder [!UICONTROL Prime] [!DNL Workfront] Plan: Ihr Unternehmen muss [!DNL Adobe Workfront Fusion].</li><li>[!UICONTROL Ultimate] [!DNL Workfront] Plan: [!DNL Workfront Fusion] ist enthalten.</li></ul>
   <p>Oder</p>
   <p>Aktuell: Ihr Unternehmen muss Einkäufe tätigen [!DNL Adobe Workfront Fusion].</p>
   </td> 
  </tr>
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

Informationen über [!DNL Adobe Workfront Fusion] Lizenzen, siehe [[!DNL Adobe Workfront Fusion] Lizenzen](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Zugriffsberechtigungen

Für jede Verbindung [!DNL Workfront Fusion] erfordert nur die Zugriffsrechte, die für den erfolgreichen Abschluss eines bestimmten Szenarios erforderlich sind. Wenn Sie beispielsweise ein Szenario erstellen, um Dokumente aus [!DNL Google Docs], [!DNL Workfront Fusion] fordert keine Berechtigung zum Abrufen des Inhalts der Dokumente an. Wenn Sie später feststellen, dass Sie auf den Inhalt der Dokumente zugreifen müssen, können Sie die Verbindung aktualisieren oder eine neue Verbindung erstellen, die auf diesen Inhalt zugreifen kann.

Nicht alle Dienste ermöglichen es Ihnen, den Zugriff auf bestimmte Aufgaben zu beschränken. In diesen Fällen [!DNL Workfront Fusion] muss vollständige Zugriffsberechtigungen erfordern. Weitere Informationen zur Beschränkung von [!DNL Workfront Fusion] Zugriff auf Ihr Konto, das für diese Dienste registriert ist, finden Sie in der anwendungsspezifischen Dokumentation unter [Apps und ihre Module](/help/quicksilver/workfront-fusion/apps-and-their-modules/apps-and-their-modules.md).

## Verbindungen verwalten

Sie können alle Verbindungen über die [!UICONTROL Verbindungen] Bereich.

>[!NOTE]
>
>Verbindungen gehören Teams. Wenn Sie die gewünschte Verbindung nicht finden können, überprüfen Sie, ob Sie das richtige Team anzeigen.
>
>So wählen Sie ein neues Team aus:
>
>* Klicken Sie im linken Navigationsbereich auf den Teamnamen und wählen Sie ein neues Team aus.
>
>    Oder
>
>* Klicken Sie in der linken Navigation auf Team overview und dann oben auf der Seite auf den Dropdown-Pfeil neben dem Teamnamen. Wählen Sie ein neues Team aus.

1. So öffnen Sie die [!UICONTROL Verbindungen] Bereich, klicken Sie <b>[!UICONTROL Verbindungen]</b> in der linken Navigation.
1. (Optional) Geben Sie die Umgebung und den Verbindungstyp an, indem Sie auf das Dropdown-Menü Umgebung und Typ klicken und eine Option auswählen.
1. (Optional) Um anzuzeigen, welche Berechtigungen gewährt wurden [!DNL Workfront Fusion] für eine Verbindung auf das Symbol Ansicht ![Verbindungsberechtigungen anzeigen](assets/view-connection-permissions.png) für diese Verbindung.
1. (Optional) Um eine Verbindung umzubenennen, markieren Sie den Verbindungsnamen und geben Sie den neuen Namen ein.
1. (Optional) Um eine Verbindung neu zu autorisieren, klicken Sie auf **Neu autorisieren** für diese Verbindung.
1. (Optional) Klicken Sie zum Löschen einer Verbindung auf **Löschen** für diese Verbindung.
1. (Optional) Um sicherzustellen, dass die Verbindung zum Dienst erfolgreich hergestellt wurde, klicken Sie auf **Überprüfen** für die Verbindung.



## Verbindung erneuern

[!DNL Workfront Fusion] erhält normalerweise für unbegrenzte Zeit Zugriffsrechte auf einen bestimmten Dienst. Einige Anwendungen erfordern, dass die Zugriffsberechtigung nach einem bestimmten Zeitraum erneuert wird. In diesen Fällen [!DNL Workfront Fusion] werden Sie kurz vor Ablauf der Zugriffsberechtigungen per E-Mail benachrichtigt.

So erneuern Sie eine Verbindung:

1. Klicken Sie auf **[!UICONTROL Neu autorisieren]** im **[!UICONTROL Verbindungen]** Bereich.
