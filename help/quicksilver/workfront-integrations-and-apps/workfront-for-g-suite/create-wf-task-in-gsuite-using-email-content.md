---
product-area: workfront-integrations;projects
keywords: Google,DOC,Dokument,Blatt,Folie
navigation-topic: workfront-for-g-suite
title: Erstellen einer  [!DNL Adobe Workfront]  in Google Workspace mithilfe von E-Mail-Inhalten
description: Sie können eine externe E-Mail (die nicht von Adobe generiert wurde [!DNL Workfront] in eine Workfront-Aufgabe konvertieren.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 6bbb4301-2791-4d72-bad8-fef63d6e892a
source-git-commit: 1e5b3c7d087c34870ccb0f4e65021358f08b81bf
workflow-type: tm+mt
source-wordcount: '1017'
ht-degree: 0%

---

# Erstellen einer [!DNL Adobe Workfront] Aufgabe in [!DNL Google Workspace] mit E-Mail-Inhalt

>[!IMPORTANT]
>
>Um stabilere und skalierbarere Integrationen bereitzustellen, wechseln wir mithilfe von Workfront Automation and Integration (Fusion) zu einem modernen, flexiblen Integrationsansatz. Im Rahmen dieser Umstellung werden die folgenden Funktionen von Workfront für Google Workspace nach dem 28. **2026 nicht mehr verfügbar**:
>
>* Zugriff auf Google Workspace-Funktionen in Workfront
>
>* Anzeigen und Verwalten von Workfront-Aufgaben über Gmail oder das Site-Panel des Google-Kalenders
>
>Es wird empfohlen, Workfront-Automatisierung und -Integration für die Integrationsanforderungen Ihres Unternehmens mit Google Workspace zu verwenden.
>
>Einen Überblick über die Automatisierung und Integration von Workfront finden Sie unter [Übersicht über Adobe Workfront Fusion](https://experienceleague.adobe.com/de/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview).
>
>Informationen zu den spezifischen Funktionen der Workfront-Automatisierungs- und Integrationsmodule für Google Workspace finden Sie unter [Gmail-](https://experienceleague.adobe.com/de/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/gmail-modules) und [Google-](https://experienceleague.adobe.com/de/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/google-calendar-modules).

Sie können eine externe E-Mail (nicht von [!DNL Adobe Workfront] generiert) in eine [!DNL Workfront] Aufgabe konvertieren.

Sie können auch eine externe E-Mail in eine Aktualisierung einer vorhandenen Aufgabe konvertieren. Weitere Informationen finden Sie unter [Aktualisieren eines  [!DNL Adobe Workfront] -Elements  [!DNL Google Workspace] Verwenden von E-Mail-Inhalten](../../workfront-integrations-and-apps/workfront-for-g-suite/update-wf-item-using-email-content.md).

Weitere Informationen zur Verwendung von [!DNL Google Workspace] für die Arbeit mit von [!DNL Workfront] gesendeten Benachrichtigungs-E-Mails finden [&#x200B; unter Verwalten [!DNL Adobe Workfront] Benachrichtigungsdetails von [!DNL Google Workspace]](../../workfront-integrations-and-apps/workfront-for-g-suite/manage-wf-email-notification-details-in-gsuite.md).

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
   <td> <p>Standard</p><p>Arbeit oder höher</p>
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Voraussetzungen

Bevor Sie eine [!DNL Workfront] Aufgabe in [!DNL Google Workspace] erstellen können, müssen Sie

* Installieren von [!DNL Workfront for Google Workspace]\
   Anweisungen finden Sie unter [Installieren [!DNL Adobe Workfront for Google Workspace]](../../workfront-integrations-and-apps/workfront-for-g-suite/install-workfront-for-gsuite.md).

## Erstellen einer [!DNL Adobe Workfront] Aufgabe in [!DNL Google Workspace] mit E-Mail-Inhalt

1. Wenn das Bedienfeld [!UICONTROL Workfront für Google Workspace] nicht angezeigt wird, klicken Sie auf das [!DNL Workfront]-Symbol ![Workfront](assets/wf-lion-icon.png) in der Seitenleiste [!DNL Google Workspace] Add-ons ganz rechts auf der Seite.
1. Wenn die E-Mail-Nachricht in [!DNL Google Workspace] geöffnet ist, klicken Sie auf eine Option in [!DNL Workfront for Google Workspace], um die E-Mail in eine neue [!DNL Workfront]-Aufgabe zu konvertieren.

1. Wählen Sie eine **[!UICONTROL Neu erstellen]**, um anzugeben, ob die Aufgabe Teil eines Projekts oder einer persönlichen Aufgabe sein soll, die unabhängig von einem Projekt ist.
1. Wenn Sie die Aufgabe an ein übergeordnetes Projekt anhängen möchten, klicken Sie auf **[!UICONTROL Projektname]**, geben Sie den Namen des Projekts ein, in dem die Aufgabe angezeigt werden soll, und klicken Sie dann auf den Projektnamen, wenn er in der Liste unten angezeigt wird.
1. Nehmen Sie eine dieser Änderungen vor:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Aufgabenname]</td> 
      <td>Bearbeiten Sie einen beliebigen Teil dieses Textes, der aus der Betreffzeile der E-Mail stammt.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Beschreibung]</td> 
      <td>Bearbeiten Sie einen beliebigen Teil dieses Textes, der aus dem Textkörper der E-Mail übernommen wird.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Zuweisen zu]</td> 
      <td>Klicken Sie auf <strong>[!UICONTROL Zuweisen zu]</strong>, klicken Sie auf die <strong>[!UICONTROL Zuweisen zu]</strong> Option, die angezeigt wird, und tippen Sie dann den Namen der Person ein und klicken Sie darauf, wenn er in der folgenden Liste angezeigt wird. Wiederholen Sie diesen Vorgang für jede Person, die Sie hinzufügen möchten, und klicken Sie dann auf <strong>[!UICONTROL Speichern]</strong>.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Geplante Dauer]</td> 
      <td> <p>Klicken Sie auf <strong>[!UICONTROL Geplante Dauer]</strong> und geben Sie die Anzahl der Tage ein, die die Aufgabe dauern soll. </p> <p>Hinweis: Diese Option kann für Ihr Unternehmen auf unterschiedliche Weise konfiguriert werden. Für Ihr Unternehmen müssen Sie beispielsweise möglicherweise die Anzahl der Stunden anstatt der Tage eingeben. Weitere Informationen erhalten Sie von Ihrem [!DNL Workfront]. Wenn Sie einen anderen Zeitraum als den konfigurierten Standardwert angeben möchten, geben Sie <strong>m</strong>, <strong>h</strong>, <strong>d</strong>, <strong>w</strong> oder <strong>mo</strong> nach der Zahl ein, die Minuten, Stunden, Tage, Wochen oder Monate angibt.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL -Priorität]</td> 
      <td>Klicken Sie auf den Dropdown-Pfeil und dann auf die Priorität, die Sie für die Aufgabe haben möchten.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL E-Mail-Anhänge einschließen]</td> 
      <td> <p>(Nur verfügbar, wenn die E-Mail mindestens einen Anhang enthält.) Klicken Sie auf diese Option, um Anhänge in der E-Mail im Bereich [!UICONTROL -Dokumente] der Aufgabe zu speichern. </p> <p>Wenn Sie einen Anhang nicht speichern möchten, klicken Sie auf das X rechts neben seinem Namen. </p> <p>Wenn die E-Mail Links zu Dokumenten in [!DNL Google Drive] enthält, werden diese auf der Registerkarte [!UICONTROL Übersicht] der Aufgabe gespeichert, die Sie gerade erstellen. </p> <p>Wichtig: Damit dies funktioniert, muss Ihr [!DNL Workfront]-Administrator [!DNL Google Drive] autorisieren, mit Dokumenten in [!DNL Workfront] zu arbeiten, wie im Abschnitt <a href="../../administration-and-setup/configure-integrations/configure-document-integrations.md#configur" class="MCXref xref">Konfigurieren von Integrationen zur Verwaltung von Dokumenten</a> im Artikel <a href="../../administration-and-setup/configure-integrations/configure-document-integrations.md" class="MCXref xref">Konfigurieren von Dokumentenintegrationen</a>.</p> <p>Wenn Sie diese Option aktivieren, bleibt sie für andere E-Mails aktiviert, die Sie in Aufgaben, Probleme und Aktualisierungen konvertieren.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL E-Mail-Datei einschließen]</td> 
      <td> <p>Klicken Sie auf diese Option, um die ursprüngliche E-Mail als E-Mail-Datei (EML<span> im Bereich [!UICONTROL Dokumente] </span> Aufgabe zu speichern. Von dort aus können Sie auf die Datei doppelklicken, um die E-Mail in Ihrer E-Mail-Anwendung zu öffnen.</p> <p>Wenn Sie diese Option aktivieren, bleibt sie für andere E-Mails aktiviert, die Sie in Aufgaben, Probleme und Aktualisierungen konvertieren.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Klicken Sie **[!UICONTROL Aufgabe erstellen]**.

   Die **[!UICONTROL Details]** für die neue Aufgabe wird im [!DNL Workfront for Google Workspace] angezeigt. Sie können auf **[!UICONTROL Updates]** klicken und sofort mit Ihren Mitarbeitern kommunizieren, ohne Ihren Posteingang verlassen zu müssen.

   Unten auf der Registerkarte **[!UICONTROL Details]** können Sie auch auf **[!UICONTROL In anzeigen[!DNL Workfront]]** klicken, um zur neuen Aufgabe in Workfront zu wechseln.

   Wenn Sie Ihren Browser aktualisieren, wird in einer Nachricht mit einem Link am unteren Rand des [!DNL Workfront for Google Workspace] bestätigt, dass Sie die E-Mail in eine Aufgabe konvertiert haben:

   Sie können auf den Link klicken, um zur Detailansicht im [!DNL Workfront for Google Workspace] für die Aufgabe zu wechseln, die Sie erstellt haben.

   Sie können diese Schritte wiederholen, um dieselbe E-Mail in mehrere Aufgaben zu konvertieren. Wenn Sie Ihren Browser aktualisieren oder zu einem anderen Zeitpunkt zur E-Mail zurückkehren, werden alle Links, die Sie für die E-Mail erstellt haben, unten im Bedienfeld [!UICONTROL Workfront für Google Workspace] aufgeführt.

1. (Optional) Fahren Sie mit der Aufgabe im [!DNL Workfront for Google Workspace] fort, indem Sie einen der folgenden Schritte ausführen:

   * Um ein Update auf der Registerkarte **[!UICONTROL Updates]** hinzuzufügen, klicken Sie auf **[!UICONTROL Neues Update starten]** und geben Sie das Update ein.

   * Um auf eine Aktualisierung auf der Registerkarte **[!UICONTROL Aktualisierungen]** zu antworten, klicken Sie auf **[!UICONTROL Antworten]** und geben Sie Ihre Antwort ein.

     Bei beiden oben genannten Aktionen können Sie bestimmte Benutzer über Ihren Kommentar benachrichtigen. Klicken Sie auf **[!UICONTROL Benachrichtigen]**, beginnen Sie mit der Eingabe des Benutzernamens, und klicken Sie dann auf den Namen, wenn er in der Dropdown-Liste angezeigt wird. Wiederholen Sie diesen Vorgang für andere Benutzer, die Sie benachrichtigen möchten, und klicken Sie dann auf **[!UICONTROL Veröffentlichen]**.

   * Klicken Sie auf **[!UICONTROL Dokumente]**, um alle mit der Aufgabe gespeicherten Dokumente anzuzeigen.

Sie können diese Schritte wiederholen, um dieselbe E-Mail in mehrere Aufgaben zu konvertieren. Wenn Sie Ihren Browser aktualisieren oder zu einem anderen Zeitpunkt zur E-Mail zurückkehren, werden alle Links, die Sie für die E-Mail erstellt haben, unten im Bedienfeld [!DNL Workfront for Google Workspace] aufgeführt.
