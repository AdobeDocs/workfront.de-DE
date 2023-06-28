---
product-area: workfront-integrations;projects
keywords: google,doc,document,sheet,slide
navigation-topic: workfront-for-g-suite
title: Aktualisieren von [!DNL Adobe Workfront] Element von G Suite mit E-Mail-Inhalt
description: Sie können ein vorhandenes Projekt, eine Aufgabe oder ein Problem mit Informationen aus einer Nicht-Adobe Workfront-E-Mail aktualisieren.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 2ac392f5-98a3-4ab6-a0e3-cda378f0f68b
source-git-commit: 4b95828dc3e6a67c4dbefb46f173303c519643a9
workflow-type: tm+mt
source-wordcount: '649'
ht-degree: 0%

---

# Aktualisieren von [!DNL Adobe Workfront] Element aus [!DNL G Suite] Verwenden von E-Mail-Inhalten

>[!NOTE]
>
>Die neueste Version des Adobe Workfront-Plug-ins für Google wurde am 26. Juni 2023 veröffentlicht.

Sie können ein vorhandenes Projekt, eine Aufgabe oder ein Problem mit Informationen aus einem Nicht-Netzwerk aktualisieren[!DNL Adobe Workfront] E-Mail.

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Plan*</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td> <p>[!UICONTROL Work], [!UICONTROL Plan]</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren [!DNL Workfront] Administrator.

## Voraussetzungen

Bevor Sie eine [!DNL Workfront] Element mit E-Mail-Inhalt aus [!DNL G Suite], müssen Sie

* Installieren [!DNL Workfront for G suite]\
   Anweisungen finden Sie unter [Installieren [!DNL Adobe Workfront for G Suite]](../../workfront-integrations-and-apps/workfront-for-g-suite/install-workfront-for-gsuite.md).

## Aktualisieren Sie eine [!DNL Workfront] Element mit E-Mail-Inhalt aus [!DNL G Suite]

1. Wenn die Variable [!UICONTROL Workfront für G Suite] nicht angezeigt wird, klicken Sie auf das Workfront-Symbol ![](assets/wf-lion-icon.png) im [!DNL G Suite] Seitenleiste für Add-ons ganz rechts auf der Seite.
1. Öffnen Sie die E-Mail-Nachricht in [!DNL G Suite]klicken **[!UICONTROL Als neues Update posten]** im [!DNL G Suite] Bereich.
1. under **[!UICONTROL Typ]** klicken Sie auf den Dropdown-Pfeil und dann auf den Objekttyp, dem Sie die Aktualisierung hinzufügen möchten.
1. Klicken Sie auf **[!UICONTROL Suchen Sie nach]** Geben Sie den Namen des Objekts ein, für das Sie die Aktualisierung hinzufügen möchten, und wählen Sie dann das Element aus, wenn es in der folgenden Liste angezeigt wird.

   Diese Option variiert je nach Auswahl in Schritt 3. Es könnte **[!UICONTROL Suchen nach einem Projekt]**, **[!UICONTROL Nach Aufgaben suchen]** oder **[!UICONTROL Suchen nach einem Problem]**.

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
      <td><p>(Nur verfügbar, wenn die E-Mail mindestens einen Anhang enthält.) Klicken Sie auf diese Option, um Anlagen auf der Registerkarte [!UICONTROL Dokumente] für die Aufgabe oder das Problem zu speichern. </p><p>Wenn Sie keine Anlage speichern möchten, klicken Sie auf das X rechts neben ihrem Namen. </p><p>Wenn die E-Mail Links zu Dokumenten in [!DNL Google Drive], werden die Links auf der Registerkarte [!UICONTROL Übersicht] der Aufgabe oder des Problems gespeichert, die bzw. das Sie erstellen. </p><p>Wichtig: <span style="color: #ff1493;"><span style="color: #000000;">Damit dies funktioniert, muss Ihr</span></span>[!DNL Workfront] administrator<span style="color: #ff1493;"><span style="color: #000000;"> muss autorisieren [!DNL Google Drive] , um [!DNL Workfront]</span></span></p>
      <p>Wenn Sie diese Option aktivieren, bleibt sie für andere E-Mails aktiviert, die Sie in Aufgaben, Probleme und Updates konvertieren.</p></td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Benachrichtigen</td> 
      <td>Klicken <strong>[!UICONTROL Benachrichtigen]</strong>, klicken Sie auf die <strong>[!UICONTROL Suche nach einem Benutzer oder Team]</strong> -Option, geben Sie den Namen der Person oder des Teams ein und klicken Sie darauf, wenn er in der unten stehenden Liste angezeigt wird. Wiederholen Sie diesen Vorgang für jede Person und jedes Team, die Sie hinzufügen möchten, und klicken Sie dann auf <strong>[!UICONTROL Save]</strong>.</td> 
     </tr> 
    </tbody> 
   </table>

1. Klicken **[!UICONTROL Aktualisieren]**.

   Wenn Sie den Browser aktualisieren, wird eine Meldung mit einem Link am unteren Rand des [!DNL Workfront for G Suite] bestätigt, dass Sie die E-Mail in eine Aktualisierung konvertiert haben:

   Sie können auf den Link klicken, um zum [!UICONTROL Updates] Registerkarte in [!DNL Workfront] für das Objekt, das Sie in Schritt 4 angegeben haben.

   Sie können diese Schritte wiederholen, um dieselbe E-Mail in Aktualisierungen, Aufgaben und Probleme zu konvertieren (siehe [Erstellen eines Adobe Workfront-Problems in [!DNL G Suite] mithilfe von E-Mail-Inhalten](../../workfront-integrations-and-apps/workfront-for-g-suite/create-wf-issue-in-g-suite-using-email-content.md)). Wenn Sie Ihren Browser aktualisieren oder zu einem anderen Zeitpunkt zur E-Mail zurückkehren, werden alle Links, die Sie für die E-Mail erstellt haben, unten im [!UICONTROL Workfront für G Suite] Bereich.

1. (Optional) Arbeiten Sie mit der Aktualisierung im [!DNL Workfront] Add-On-Bedienfeld verwenden, indem Sie einen der folgenden Schritte ausführen:

   * So fügen Sie eine weitere Aktualisierung zu **[!UICONTROL Updates]** Registerkarte, klicken Sie auf **[!UICONTROL Neue Aktualisierung starten]** und geben Sie die Informationen ein.

   * So antworten Sie auf eine Aktualisierung der **[!UICONTROL Updates]** Registerkarte, klicken Sie auf **[!UICONTROL Antwort]** und geben Sie Ihre Antwort ein.

     Für beide oben genannten Optionen können Sie auf **[!UICONTROL Benachrichtigen]** um die Empfänger für die Antwort anzugeben, wie in Schritt 5 beschrieben. Wenn Sie bereit sind, klicken Sie auf **[!UICONTROL Post]** , um die Aktualisierung oder Antwort hinzuzufügen.

   * Klicken Sie auf **[!UICONTROL Details]** -Registerkarte, um die Details für das neue Projekt, die Aufgabe oder das Problem anzuzeigen.
