---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: connections-annd-webhooks
title: Verbindungen - Übersicht
description: Für die meisten Apps ist es erforderlich, eine Verbindung zu erstellen, über die [!DNL Adobe Workfront Fusion] gemäß den Einstellungen des jeweiligen Szenarios mit dem angegebenen Drittanbieterdienst kommunizieren kann.
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

Für die meisten Apps erfordert [!DNL Workfront Fusion] eine Verbindung, über die es mit dem angegebenen Drittanbieterdienst gemäß den Einstellungen des jeweiligen Szenarios kommunizieren kann.

Wenn Sie beispielsweise ein Szenario erstellen möchten, das Informationen aus [!DNL Workfront] abruft, müssen Sie [!DNL Workfront Fusion] Zugriffsberechtigungen erteilen, um auf Ihr [!DNL Workfront] -Konto zuzugreifen.

Eine Verbindung stellt die Autorisierung und Berechtigungen dar, die Fusion für den Zugriff auf die Anwendung verwendet. Sie können für jede Anwendung eine oder mehrere Verbindungen erstellen und dieselbe Verbindung in mehreren Modulen oder Szenarien verwenden.

Die meisten Verbindungen werden nur für eine einzelne Anwendung verwendet. Beispielsweise kann eine [!DNL Workfront] -Verbindung nicht in einem [!UICONTROL Salesforce] -Modul verwendet werden. Einige [!DNL Adobe] -Anwendungen können Verbindungen freigeben. Weitere Informationen finden Sie in den Artikeln für diese Anwendungen, aufgeführt in [Apps und deren Modulen](/help/quicksilver/workfront-fusion/apps-and-their-modules/apps-and-their-modules.md).

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
   <p>Aktuell: Keine [!DNL Workfront Fusion] Lizenzanforderung.</p>
   <p>Oder</p>
   <p>Veraltet: Beliebig </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>
   <p>Neu:</p> <ul><li>[!UICONTROL Select] oder [!UICONTROL Prime] [!DNL Workfront] Plan: Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] erwerben.</li><li>[!UICONTROL Ultimate] [!DNL Workfront] Plan: [!DNL Workfront Fusion] ist enthalten.</li></ul>
   <p>Oder</p>
   <p>Aktuell: Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] kaufen.</p>
   </td> 
  </tr>
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

Informationen zu [!DNL Adobe Workfront Fusion] -Lizenzen finden Sie unter [[!DNL Adobe Workfront Fusion] Lizenzen](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Zugriffsberechtigungen

Für jede Verbindung erfordert [!DNL Workfront Fusion] nur die Zugriffsberechtigungen, die erforderlich sind, um ein bestimmtes Szenario erfolgreich abzuschließen. Wenn Sie beispielsweise ein Szenario zum Auflisten von Dokumenten aus [!DNL Google Docs] erstellen, fordert [!DNL Workfront Fusion] keine Berechtigung zum Abrufen des Inhalts der Dokumente an. Wenn Sie später feststellen, dass Sie auf den Inhalt der Dokumente zugreifen müssen, können Sie die Verbindung aktualisieren oder eine neue Verbindung erstellen, die auf diesen Inhalt zugreifen kann.

Nicht alle Dienste ermöglichen es Ihnen, den Zugriff auf bestimmte Aufgaben zu beschränken. In diesen Fällen muss [!DNL Workfront Fusion] vollständige Zugriffsberechtigungen erfordern. Weitere Informationen dazu, wie Sie den [!DNL Workfront Fusion]-Zugriff auf Ihr Konto beschränken, das für diese Dienste registriert ist, finden Sie in der anwendungsspezifischen Dokumentation unter [Apps und deren Module](/help/quicksilver/workfront-fusion/apps-and-their-modules/apps-and-their-modules.md).

## Verbindungen verwalten

Sie können alle Verbindungen über den Bereich [!UICONTROL Verbindungen] verwalten.

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

1. Um den Bereich [!UICONTROL Verbindungen] zu öffnen, klicken Sie im linken Navigationsbereich auf <b>[!UICONTROL Verbindungen]</b> .
1. (Optional) Geben Sie die Umgebung und den Verbindungstyp an, indem Sie auf das Dropdown-Menü Umgebung und Typ klicken und eine Option auswählen.
1. (Optional) Um anzuzeigen, welche Berechtigungen [!DNL Workfront Fusion] für eine Verbindung zugewiesen wurden, klicken Sie auf das Ansichtssymbol ![Verbindungsberechtigungen anzeigen](assets/view-connection-permissions.png) für diese Verbindung.
1. (Optional) Um eine Verbindung umzubenennen, markieren Sie den Verbindungsnamen und geben Sie den neuen Namen ein.
1. (Optional) Klicken Sie zum erneuten Autorisieren einer Verbindung auf **Neu autorisieren** für diese Verbindung.
1. (Optional) Klicken Sie zum Löschen einer Verbindung auf **Löschen** für diese Verbindung.
1. (Optional) Um sicherzustellen, dass die Verbindung zum Dienst erfolgreich hergestellt wurde, klicken Sie auf **Überprüfen** für die Verbindung.



## Verbindung erneuern

[!DNL Workfront Fusion] erhält für gewöhnlich unbegrenzte Zeit Zugriffsrechte auf einen bestimmten Dienst. Einige Anwendungen erfordern, dass die Zugriffsberechtigung nach einem bestimmten Zeitraum erneuert wird. In diesen Fällen benachrichtigt Sie [!DNL Workfront Fusion] per E-Mail kurz vor Ablauf der Zugriffsberechtigungen.

So erneuern Sie eine Verbindung:

1. Klicken Sie im Bereich **[!UICONTROL Verbindungen]** auf die Schaltfläche **[!UICONTROL Neu autorisieren]** .
