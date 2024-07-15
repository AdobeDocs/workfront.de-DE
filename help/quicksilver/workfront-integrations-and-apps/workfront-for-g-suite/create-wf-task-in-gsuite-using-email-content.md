---
product-area: workfront-integrations;projects
keywords: google,doc,document,sheet,slide
navigation-topic: workfront-for-g-suite
title: Erstellen einer [!DNL Adobe Workfront] Aufgabe in Google Workspace mit E-Mail-Inhalt
description: Sie können eine (nicht von Adobe [!DNL Workfront] generierte) externe E-Mail in eine Workfront-Aufgabe konvertieren.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 6bbb4301-2791-4d72-bad8-fef63d6e892a
source-git-commit: 84444753db0e5c496f013e0245988e62fddad585
workflow-type: tm+mt
source-wordcount: '920'
ht-degree: 0%

---

# Erstellen einer [!DNL Adobe Workfront]-Aufgabe in [!DNL Google Workspace] mithilfe des E-Mail-Inhalts

>[!NOTE]
>
>Die neueste Version des Adobe Workfront-Plug-ins für Google wurde am 26. Juni 2023 veröffentlicht.

Sie können eine externe E-Mail (nicht von [!DNL Adobe Workfront] generiert) in eine [!DNL Workfront] -Aufgabe konvertieren.

Sie können auch eine externe E-Mail in eine Aktualisierung einer vorhandenen Aufgabe konvertieren. Weitere Informationen finden Sie unter [Aktualisieren eines  [!DNL Adobe Workfront] Elements von  [!DNL Google Workspace] mit E-Mail-Inhalt](../../workfront-integrations-and-apps/workfront-for-g-suite/update-wf-item-using-email-content.md).

Informationen zur Verwendung von [!DNL Google Workspace] für die Verwendung mit Benachrichtigungs-E-Mails, die von [!DNL Workfront] gesendet werden, finden Sie unter [Verwalten von [!DNL Adobe Workfront] Benachrichtigungsdetails von  [!DNL Google Workspace]](../../workfront-integrations-and-apps/workfront-for-g-suite/manage-wf-email-notification-details-in-gsuite.md).

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

Bevor Sie eine [!DNL Workfront] -Aufgabe in [!DNL Google Workspace] erstellen können, müssen Sie

* Installieren Sie [!DNL Workfront for Google Workspace]\
   Anweisungen finden Sie unter [Installieren [!DNL Adobe Workfront for Google Workspace]](../../workfront-integrations-and-apps/workfront-for-g-suite/install-workfront-for-gsuite.md).

## Erstellen einer [!DNL Adobe Workfront]-Aufgabe in [!DNL Google Workspace] mithilfe des E-Mail-Inhalts

1. Wenn das Bedienfeld [!UICONTROL Workfront für Google Workspace] nicht angezeigt wird, klicken Sie in der Seitenleiste [!DNL Google Workspace] der Add-ons ganz rechts auf das Symbol [!DNL Workfront] ![](assets/wf-lion-icon.png) .
1. Wenn die E-Mail-Nachricht in [!DNL Google Workspace] geöffnet ist, klicken Sie auf eine Option in [!DNL Workfront for Google Workspace], um die E-Mail in eine neue [!DNL Workfront] -Aufgabe zu konvertieren.

1. Wählen Sie die Option **[!UICONTROL Neu erstellen]** aus, um anzugeben, ob die Aufgabe Teil eines Projekts oder einer persönlichen Aufgabe sein wird, die von einem Projekt unabhängig ist.
1. Wenn Sie die Aufgabe an ein übergeordnetes Projekt anhängen möchten, klicken Sie auf &quot;**[!UICONTROL Projektname]**&quot;, geben Sie den Namen des Projekts ein, in dem die Aufgabe ausgeführt werden soll, und klicken Sie dann auf den Projektnamen, wenn er in der folgenden Liste angezeigt wird.
1. Nehmen Sie eine der folgenden Änderungen vor:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Task Name]</td> 
      <td>Bearbeiten Sie einen beliebigen Teil dieses Textes, der sich aus der Betreffzeile der E-Mail ergibt.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Beschreibung]</td> 
      <td>Bearbeiten Sie einen beliebigen Teil dieses Textes, der aus dem Text der E-Mail stammt.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Zuweisen zu]</td> 
      <td>Klicken Sie auf <strong>[!UICONTROL Zuweisen zu]</strong>, klicken Sie auf die angezeigte Option <strong>[!UICONTROL Zuweisen zu]</strong>, geben Sie dann den Namen der Person ein und klicken Sie auf diese Option, wenn sie in der unten stehenden Liste angezeigt wird. Wiederholen Sie diesen Vorgang für jede Person, die Sie hinzufügen möchten, und klicken Sie dann auf <strong>[!UICONTROL Speichern]</strong>.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Geplante Dauer]</td> 
      <td> <p>Klicken Sie auf <strong>[!UICONTROL Plante Dauer]</strong> und geben Sie dann die Anzahl der Tage ein, für die die Aufgabe ausgeführt werden soll. </p> <p>Hinweis: Diese Option kann für Ihr Unternehmen auf unterschiedliche Weise konfiguriert werden. Beispielsweise müssen Sie für Ihre Organisation möglicherweise eine Anzahl von Stunden anstelle von Tagen eingeben. Wenn Sie weitere Informationen benötigen, wenden Sie sich an Ihren [!DNL Workfront] -Administrator. Wenn Sie einen anderen Zeitraum als den konfigurierten Standardwert angeben möchten, geben Sie <strong>m</strong>, <strong>h</strong>, <strong>d</strong>, <strong>w</strong> oder <strong>mo</strong> nach der Zahl ein, um Minuten, Stunden, Tage, Wochen oder Monate anzugeben.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Priority]</td> 
      <td>Klicken Sie auf den Dropdown-Pfeil und dann auf die gewünschte Priorität für die Aufgabe.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL E-Mail-Anhänge einschließen]</td> 
      <td> <p>(Nur verfügbar, wenn die E-Mail mindestens einen Anhang enthält.) Klicken Sie auf diese Option, um Anlagen in der E-Mail im Bereich [!UICONTROL Dokumente] der Aufgabe zu speichern. </p> <p>Wenn Sie keine Anlage speichern möchten, klicken Sie auf das X rechts neben ihrem Namen. </p> <p>Wenn die E-Mail Links zu Dokumenten in [!DNL Google Drive] enthält, werden diese im Tab [!UICONTROL Übersicht] der Aufgabe gespeichert, die Sie erstellen. </p> <p>Wichtig: Damit dies funktioniert, muss Ihr [!DNL Workfront] -Administrator [!DNL Google Drive] autorisieren, mit Dokumenten in [!DNL Workfront] zu arbeiten, wie im Abschnitt <a href="../../administration-and-setup/configure-integrations/configure-document-integrations.md#configur" class="MCXref xref">Integrationen für die Verwaltung von Dokumenten konfigurieren</a> im Artikel <a href="../../administration-and-setup/configure-integrations/configure-document-integrations.md" class="MCXref xref">Dokumentintegrationen konfigurieren</a> beschrieben.</p> <p>Wenn Sie diese Option aktivieren, bleibt sie für andere E-Mails aktiviert, die Sie in Aufgaben, Probleme und Updates konvertieren.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL E-Mail-Datei einschließen]</td> 
      <td> <p>Klicken Sie auf diese Option, um die ursprüngliche E-Mail als E-Mail-Datei (EML) <span>im Bereich [!UICONTROL Dokumente]</span> der Aufgabe zu speichern. Dort können Sie auf die Datei doppelklicken, um die E-Mail in Ihrer E-Mail-Anwendung zu öffnen.</p> <p>Wenn Sie diese Option aktivieren, bleibt sie für andere E-Mails aktiviert, die Sie in Aufgaben, Probleme und Updates konvertieren.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Klicken Sie auf **[!UICONTROL Aufgabe erstellen]**.

   Die Registerkarte **[!UICONTROL Details]** für die neue Aufgabe wird im Bedienfeld [!DNL Workfront for Google Workspace] angezeigt. Sie können auf **[!UICONTROL Aktualisierungen]** klicken und sofort mit den Mitwirkenden kommunizieren, ohne das Feld verlassen zu müssen.

   Am unteren Rand der Registerkarte **[!UICONTROL Details]** können Sie auch auf **[!UICONTROL In[!DNL Workfront]]** anzeigen klicken, um zur neuen Aufgabe in Workfront zu wechseln.

   Wenn Sie Ihren Browser aktualisieren, wird durch eine Meldung mit einem Link am unteren Rand des Bereichs [!DNL Workfront for Google Workspace] bestätigt, dass Sie die E-Mail in eine Aufgabe konvertiert haben:

   Sie können auf den Link klicken, um zur Detailansicht im Bereich [!DNL Workfront for Google Workspace] für die Aufgabe zu wechseln, die Sie erstellt haben.

   Sie können diese Schritte wiederholen, um dieselbe E-Mail in mehrere Aufgaben zu konvertieren. Wenn Sie Ihren Browser aktualisieren oder zu einem anderen Zeitpunkt zur E-Mail zurückkehren, werden alle Links, die Sie für die E-Mail erstellt haben, unten im Bedienfeld &quot;[!UICONTROL Workfront für Google Workspace]&quot;aufgelistet.

1. (Optional) Fahren Sie mit der Aufgabe im Bedienfeld [!DNL Workfront for Google Workspace] fort, indem Sie einen der folgenden Schritte ausführen:

   * Um ein Update auf der Registerkarte **[!UICONTROL Aktualisierungen]** hinzuzufügen, klicken Sie auf **[!UICONTROL Neues Update starten]** und geben Sie das Update ein.

   * Um auf ein Update auf der Registerkarte **[!UICONTROL Aktualisierungen]** zu antworten, klicken Sie auf **[!UICONTROL Antworten]** und geben Sie Ihre Antwort ein.

     Bei beiden der oben genannten Aktionen können Sie bestimmte Benutzer über Ihren Kommentar benachrichtigen. Klicken Sie auf **[!UICONTROL Benachrichtigen]**, beginnen Sie mit der Eingabe des Benutzernamens und klicken Sie dann auf den Namen, wenn er in der Dropdown-Liste angezeigt wird. Wiederholen Sie diesen Vorgang für andere Benutzer, die Sie benachrichtigen möchten, und klicken Sie dann auf **[!UICONTROL Post]**.

   * Klicken Sie auf die Registerkarte **[!UICONTROL Dokumente]** , um alle mit der Aufgabe gespeicherten Dokumente anzuzeigen.

Sie können diese Schritte wiederholen, um dieselbe E-Mail in mehrere Aufgaben zu konvertieren. Wenn Sie Ihren Browser aktualisieren oder zu einem anderen Zeitpunkt zur E-Mail zurückkehren, werden alle Links, die Sie für die E-Mail erstellt haben, unten im Bedienfeld &quot;[!DNL Workfront for Google Workspace]&quot;aufgelistet.
