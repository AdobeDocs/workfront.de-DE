---
product-area: workfront-integrations;projects
keywords: google,doc,document,sheet,slide
navigation-topic: workfront-for-g-suite
title: Aktualisieren eines [!DNL Adobe Workfront] Elements aus Google Workspace mithilfe von E-Mail-Inhalten
description: Sie können ein vorhandenes Projekt, eine Aufgabe oder ein Problem mit Informationen aus einer Nicht-Adobe Workfront-E-Mail aktualisieren.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 2ac392f5-98a3-4ab6-a0e3-cda378f0f68b
source-git-commit: 84444753db0e5c496f013e0245988e62fddad585
workflow-type: tm+mt
source-wordcount: '645'
ht-degree: 0%

---

# Aktualisieren eines [!DNL Adobe Workfront] -Elements von [!DNL Google Workspace] mit E-Mail-Inhalt

>[!NOTE]
>
>Die neueste Version des Adobe Workfront-Plug-ins für Google wurde am 26. Juni 2023 veröffentlicht.

Sie können ein vorhandenes Projekt, eine Aufgabe oder ein Problem mit Informationen aus einer Nicht-[!DNL Adobe Workfront]-E-Mail aktualisieren.

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td> <p>[!UICONTROL Work], [!UICONTROL Plan]</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren [!DNL Workfront] -Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Voraussetzungen

Bevor Sie ein [!DNL Workfront] -Element mit E-Mail-Inhalt von [!DNL Google Workspace] aktualisieren können, müssen Sie

* Installieren Sie [!DNL Workfront for Google Workspace]\
   Anweisungen finden Sie unter [Installieren [!DNL Adobe Workfront for Google Workspace]](../../workfront-integrations-and-apps/workfront-for-g-suite/install-workfront-for-gsuite.md).

## Aktualisieren eines [!DNL Workfront] -Elements mit E-Mail-Inhalt von [!DNL Google Workspace]

1. Wenn das Bedienfeld [!UICONTROL Workfront für Google Workspace] nicht angezeigt wird, klicken Sie in der Seitenleiste der Add-ons [!DNL Google Workspace] ganz rechts auf der Seite auf das Workfront-Symbol ![](assets/wf-lion-icon.png) .
1. Wenn die E-Mail-Nachricht in [!DNL Google Workspace] geöffnet ist, klicken Sie im Bedienfeld [!DNL Google Workspace] auf **[!UICONTROL Post als neues Update]** .
1. Klicken Sie unter &quot;**[!UICONTROL Typ]**&quot;auf den Dropdown-Pfeil und dann auf den Objekttyp, dem Sie die Aktualisierung hinzufügen möchten.
1. Klicken Sie auf die Option **[!UICONTROL Suchen nach]** , geben Sie den Namen des Objekts ein, dem Sie die Aktualisierung hinzufügen möchten, und wählen Sie dann das Element aus, wenn es in der folgenden Liste angezeigt wird.

   Diese Option variiert je nach Auswahl in Schritt 3. Es kann **[!UICONTROL Nach einem Projekt suchen]**, **[!UICONTROL Nach einer Aufgabe suchen]** oder **[!UICONTROL Nach einem Problem suchen]** sein.

   >[!NOTE]
   >
   >Wenn Sie den Namen einer Aufgabe eingeben, werden persönliche Ad-hoc-Aufgaben aus der unten angezeigten Namensliste ausgeschlossen.

1. Nehmen Sie eine der folgenden optionalen Änderungen vor:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Update]</td> 
      <td>Bearbeiten Sie einen beliebigen Teil dieses Textes, der aus der Betreffzeile und dem Text der E-Mail übernommen wird.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL E-Mail-Anhänge einschließen]</td> 
      <td><p>(Nur verfügbar, wenn die E-Mail mindestens einen Anhang enthält.) Klicken Sie auf diese Option, um Anlagen auf der Registerkarte [!UICONTROL Dokumente] für die Aufgabe oder das Problem zu speichern. </p><p>Wenn Sie keine Anlage speichern möchten, klicken Sie auf das X rechts neben ihrem Namen. </p><p>Wenn die E-Mail Links zu Dokumenten in [!DNL Google Drive] enthält, werden die Links im Tab [!UICONTROL Übersicht] der Aufgabe oder des Problems gespeichert, die bzw. das Sie erstellen. </p><p>Wichtig: <span style="color: #ff1493;"><span style="color: #000000;"> Damit dies funktioniert, muss Ihr </span></span>[!DNL Workfront] Administrator<span style="color: #ff1493;"><span style="color: #000000;"> [!DNL Google Drive] autorisieren, mit [!DNL Workfront]</span></span> zu arbeiten.</p>
      <p>Wenn Sie diese Option aktivieren, bleibt sie für andere E-Mails aktiviert, die Sie in Aufgaben, Probleme und Updates konvertieren.</p></td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Benachrichtigen</td> 
      <td>Klicken Sie auf die Option <strong>[!UICONTROL Benachrichtigen]</strong>, klicken Sie auf die Option <strong>[!UICONTROL Suchen nach einem Benutzer oder Team]</strong> , geben Sie dann den Namen der Person oder des Teams ein und klicken Sie darauf, sobald diese in der unten stehenden Liste angezeigt wird. Wiederholen Sie diesen Vorgang für jede Person und jedes Team, die Sie hinzufügen möchten, und klicken Sie dann auf <strong>[!UICONTROL Speichern]</strong>.</td> 
     </tr> 
    </tbody> 
   </table>

1. Klicken Sie auf **[!UICONTROL Aktualisieren]**.

   Wenn Sie Ihren Browser aktualisieren, wird durch eine Meldung mit einem Link am unteren Rand des Bereichs [!DNL Workfront for Google Workspace] bestätigt, dass Sie die E-Mail in eine Aktualisierung konvertiert haben:

   Sie können auf den Link klicken, um die Registerkarte [!UICONTROL Aktualisierungen] in [!DNL Workfront] für das Objekt aufzurufen, das Sie in Schritt 4 angegeben haben.

   Sie können diese Schritte wiederholen, um dieselbe E-Mail in Aktualisierungen, Aufgaben und Probleme zu konvertieren (siehe [Erstellen eines Adobe Workfront-Problems in  [!DNL Google Workspace] mit E-Mail-Inhalt](../../workfront-integrations-and-apps/workfront-for-g-suite/create-wf-issue-in-g-suite-using-email-content.md)). Wenn Sie Ihren Browser aktualisieren oder zu einem anderen Zeitpunkt zur E-Mail zurückkehren, werden alle Links, die Sie für die E-Mail erstellt haben, unten im Bedienfeld &quot;[!UICONTROL Workfront für Google Workspace]&quot;aufgelistet.

1. (Optional) Fahren Sie mit der Aktualisierung im Add-On-Bedienfeld [!DNL Workfront] fort, indem Sie einen der folgenden Schritte ausführen:

   * Um auf der Registerkarte **[!UICONTROL Aktualisierungen]** ein weiteres Update hinzuzufügen, klicken Sie auf **[!UICONTROL Neues Update starten]** und geben Sie die Informationen ein.

   * Um auf ein Update auf der Registerkarte **[!UICONTROL Aktualisierungen]** zu antworten, klicken Sie auf **[!UICONTROL Antworten]** und geben Sie Ihre Antwort ein.

     Für beide oben genannten Optionen können Sie auf **[!UICONTROL Benachrichtigen]** klicken, um wie in Schritt 5 Empfänger für die Antwort anzugeben. Wenn Sie bereit sind, klicken Sie auf **[!UICONTROL Post]** , um die Aktualisierung oder Antwort hinzuzufügen.

   * Klicken Sie auf die Registerkarte **[!UICONTROL Details]** , um die Details für das neue Projekt, die Aufgabe oder das Problem anzuzeigen.
