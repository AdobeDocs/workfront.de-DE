---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: connections-annd-webhooks
title: Verbindungen - Übersicht
description: Für die meisten Apps ist es erforderlich, eine Verbindung zu erstellen, über  [!DNL Adobe Workfront Fusion]  mit dem angegebenen Drittanbieterdienst entsprechend den Einstellungen des spezifischen Szenarios kommunizieren kann.
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

Für die meisten Apps ist [!DNL Workfront Fusion] eine Verbindung erforderlich, über die es mit dem angegebenen Drittanbieterdienst entsprechend den Einstellungen des jeweiligen Szenarios kommunizieren kann.

Wenn Sie beispielsweise ein Szenario erstellen möchten, das Informationen aus [!DNL Workfront] abruft, müssen Sie [!DNL Workfront Fusion] Zugriffsberechtigungen erteilen, damit sie auf Ihr [!DNL Workfront]-Konto zugreifen können.

Eine Verbindung stellt die Autorisierung und Berechtigungen dar, die Fusion für den Zugriff auf das Programm verwendet. Sie können für jede Anwendung eine oder mehrere Verbindungen erstellen und dieselbe Verbindung in mehreren Modulen oder Szenarien verwenden.

Die meisten Verbindungen werden nur für eine einzige Anwendung verwendet. Beispielsweise kann eine [!DNL Workfront] nicht in einem [!UICONTROL Salesforce]-Modul verwendet werden. Einige [!DNL Adobe] Anwendungen können Verbindungen gemeinsam nutzen. Weitere Informationen finden Sie in den Artikeln für diese Programme, die unter &quot;[ und ihre Module“ aufgeführt ](/help/quicksilver/workfront-fusion/apps-and-their-modules/apps-and-their-modules.md).

Verbindungen werden auf Team-Ebene verwaltet. Alle Mitglieder eines Teams haben Zugriff auf die Verbindungen des Teams, und Benutzer außerhalb eines Teams haben keinen Zugriff auf die Verbindungen des Teams.

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Funktion in diesem Artikel verwenden zu können:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Plan</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] Lizenz</td> 
   <td> <p>Neu: [!UICONTROL Standard]</p><p>Oder</p><p>Aktuell: [!UICONTROL Work] oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] Lizenz **</td> 
   <td>
   <p>Aktuell: Keine [!DNL Workfront Fusion].</p>
   <p>Oder</p>
   <p>Legacy: Beliebig </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>
   <p>Neu:</p> <ul><li>[!UICONTROL Select] oder [!UICONTROL Prime] [!DNL Workfront] Plan: Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] kaufen.</li><li>[!UICONTROL Ultimate] [!DNL Workfront]: [!DNL Workfront Fusion] ist enthalten.</li></ul>
   <p>Oder</p>
   <p>Aktuell: Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] erwerben.</p>
   </td> 
  </tr>
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

Informationen zu [!DNL Adobe Workfront Fusion] finden Sie unter [[!DNL Adobe Workfront Fusion] Lizenzen](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Zugriffsberechtigungen

Für jede Verbindung benötigt [!DNL Workfront Fusion] nur die Zugriffsrechte, die für den erfolgreichen Abschluss eines bestimmten Szenarios erforderlich sind. Wenn Sie beispielsweise ein Szenario erstellen, um Dokumente aus [!DNL Google Docs] aufzulisten, fordert [!DNL Workfront Fusion] keine Berechtigung zum Abrufen des Inhalts der Dokumente an. Wenn Sie später feststellen, dass Sie auf den Inhalt der Dokumente zugreifen müssen, können Sie die Verbindung aktualisieren oder eine neue erstellen, die auf diesen Inhalt zugreifen kann.

Nicht alle Services ermöglichen es Ihnen, den Zugriff auf bestimmte Aufgaben zu beschränken. In diesen Fällen müssen [!DNL Workfront Fusion] vollständige Zugriffsrechte benötigen. Weitere Informationen dazu, wie Sie [!DNL Workfront Fusion] Zugriff auf Ihr registriertes -Konto auf diese Services beschränken können, finden Sie in der programmspezifischen Dokumentation unter [Apps und ihre Module](/help/quicksilver/workfront-fusion/apps-and-their-modules/apps-and-their-modules.md).

## Verbindungen verwalten

Sie können alle Verbindungen über den Bereich [!UICONTROL Verbindungen] verwalten.

>[!NOTE]
>
>Verbindungen gehören Teams. Wenn Sie die gesuchte Verbindung nicht finden können, überprüfen Sie, ob Sie das richtige Team anzeigen.
>
>So wählen Sie ein neues Team:
>
>* Klicken Sie im linken Navigationsbereich auf den Namen des Teams und wählen Sie ein neues Team aus.
>
>    Oder
>
>* Klicken Sie in der linken Navigationsleiste auf Team-Übersicht und dann auf den Dropdown-Pfeil neben dem Team-Namen oben auf der Seite. Wählen Sie ein neues Team aus.

1. Um den Bereich [!UICONTROL Verbindungen] zu öffnen, klicken <b>[!UICONTROL  im linken Navigationsbereich ]</b>Verbindungen“.
1. (Optional) Geben Sie die Umgebung und den Verbindungstyp an, indem Sie auf die Dropdown-Liste Umgebung und Typ klicken und eine Option auswählen.
1. (Optional) Um anzuzeigen, welche Berechtigungen [!DNL Workfront Fusion] für eine Verbindung erteilt wurden, klicken Sie auf das Symbol Anzeigen ![Verbindungsberechtigungen anzeigen](assets/view-connection-permissions.png) für diese Verbindung.
1. (Optional) Um eine Verbindung umzubenennen, markieren Sie den Verbindungsnamen und geben Sie den neuen Namen ein.
1. (Optional) Um eine Verbindung erneut zu autorisieren, klicken Sie auf **Erneut autorisieren** für diese Verbindung.
1. (Optional) Um eine Verbindung zu löschen, klicken Sie auf **Löschen** für diese Verbindung.
1. (Optional) Um sicherzustellen, dass die Verbindung zum Service erfolgreich hergestellt wurde, klicken Sie auf **Überprüfen** für die Verbindung.



## Erneuern einer Verbindung

[!DNL Workfront Fusion] erhält in der Regel für unbegrenzte Zeit Zugriffsrechte für einen bestimmten Dienst. Bei einigen Anwendungen muss die Zugriffsberechtigung nach einer bestimmten Zeit erneuert werden. In diesen Fällen benachrichtigt [!DNL Workfront Fusion] Sie per E-Mail, kurz bevor die Zugriffsrechte ablaufen.

So erneuern Sie eine Verbindung:

1. Klicken Sie auf **[!UICONTROL Erneut genehmigen]** im Bereich **[!UICONTROL Verbindungen]**.
