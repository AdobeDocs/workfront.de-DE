---
product-area: workfront-integrations;projects
keywords: Google,DOC,Dokument,Blatt,Folie
navigation-topic: workfront-for-g-suite
title: Aktualisieren eines  [!DNL Adobe Workfront]  aus Google Workspace mithilfe von E-Mail-Inhalten
description: Sie können ein vorhandenes Projekt, eine Aufgabe oder ein Problem mit Informationen aus einer Nicht-Adobe Workfront-E-Mail aktualisieren.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 2ac392f5-98a3-4ab6-a0e3-cda378f0f68b
source-git-commit: 1e5b3c7d087c34870ccb0f4e65021358f08b81bf
workflow-type: tm+mt
source-wordcount: '742'
ht-degree: 0%

---

# Aktualisieren eines [!DNL Adobe Workfront] aus [!DNL Google Workspace] mithilfe von E-Mail-Inhalten

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
>Informationen zu den spezifischen Funktionen der Workfront-Automatisierungs- und Integrationsmodule für Google Workspace finden Sie unter [Gmail-](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/gmail-modules) und [Google-](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/google-calendar-modules).

Sie können ein vorhandenes Projekt, eine Aufgabe oder ein Problem mit Informationen aus einer nicht [!DNL Adobe Workfront] E-Mail aktualisieren.

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

Bevor Sie ein [!DNL Workfront] mit E-Mail-Inhalt aus [!DNL Google Workspace] aktualisieren können, müssen Sie Folgendes tun

* Installieren von [!DNL Workfront for Google Workspace]\
   Anweisungen finden Sie unter [Installieren [!DNL Adobe Workfront for Google Workspace]](../../workfront-integrations-and-apps/workfront-for-g-suite/install-workfront-for-gsuite.md).

## Aktualisieren eines [!DNL Workfront] mithilfe von E-Mail-Inhalten aus [!DNL Google Workspace]

1. Wenn das Bedienfeld [!UICONTROL Workfront für Google Workspace] nicht angezeigt wird, klicken Sie auf das Workfront-Symbol ![Workfront](assets/wf-lion-icon.png)Symbol in der Seitenleiste [!DNL Google Workspace] Add-ons ganz rechts auf der Seite.
1. Wenn die E-Mail-Nachricht in [!DNL Google Workspace] geöffnet ist **[!UICONTROL klicken Sie im]**-Bedienfeld auf [!DNL Google Workspace]Als neues Update posten.
1. Klicken **[!UICONTROL unter &quot;]**&quot; auf den Dropdown-Pfeil und dann auf den Objekttyp, zu dem Sie die Aktualisierung hinzufügen möchten.
1. Klicken Sie auf die **[!UICONTROL Suchen nach]**, geben Sie den Namen des Objekts ein, zu dem Sie die Aktualisierung hinzufügen möchten, und wählen Sie dann das Element aus, wenn es in der Liste unten angezeigt wird.

   Diese Option variiert je nachdem, was Sie in Schritt 3 ausgewählt haben. Dies kann **[!UICONTROL Nach einem Projekt suchen]**, **[!UICONTROL Nach einer Aufgabe suchen]** oder **[!UICONTROL Nach einem Problem suchen]** sein.

   >[!NOTE]
   >
   >Wenn Sie den Namen einer Aufgabe eingeben, werden persönliche Ad-hoc-Aufgaben aus der Liste mit dem Namen ausgeschlossen, die unten angezeigt wird.

1. Nehmen Sie eine dieser optionalen Änderungen vor:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL aktualisieren]</td> 
      <td>Bearbeiten Sie einen beliebigen Teil dieses Textes, der aus der Betreffzeile und dem Textkörper der E-Mail übernommen wird.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL E-Mail-Anhänge einschließen]</td> 
      <td><p>(Nur verfügbar, wenn die E-Mail mindestens einen Anhang enthält.) Klicken Sie auf diese Option, um Anhänge für die Aufgabe oder das Problem auf der Registerkarte [!UICONTROL Documents] zu speichern. </p><p>Wenn Sie einen Anhang nicht speichern möchten, klicken Sie auf das X rechts neben seinem Namen. </p><p>Wenn die E-Mail in [!DNL Google Drive] Links zu Dokumenten enthält, werden die Links auf der Registerkarte [!UICONTROL Übersicht] der Aufgabe oder des Problems gespeichert, die bzw. das Sie erstellen. </p><p>Wichtig: <span style="color: #ff1493;"><span style="color: #000000;">Damit dies funktioniert, muss Ihr </span></span>[!DNL Workfront]-<span style="color: #ff1493;"><span style="color: #000000;"> [!DNL Google Drive] autorisieren, mit [!DNL Workfront]</span></span> zu arbeiten</p>
      <p>Wenn Sie diese Option aktivieren, bleibt sie für andere E-Mails aktiviert, die Sie in Aufgaben, Probleme und Aktualisierungen konvertieren.</p></td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Benachrichtigen</td> 
      <td>Klicken Sie auf <strong>[!UICONTROL Benachrichtigen]</strong>, klicken Sie auf die <strong>[!UICONTROL Nach einem Benutzer oder Team suchen]</strong> Option, die angezeigt wird, geben Sie dann den Namen der Person oder des Teams ein und klicken Sie auf ihn, wenn er in der folgenden Liste angezeigt wird. Wiederholen Sie diesen Vorgang für jede Person und jedes Team, die Sie hinzufügen möchten, und klicken Sie dann auf <strong>[!UICONTROL Speichern]</strong>.</td> 
     </tr> 
    </tbody> 
   </table>

1. Klicken Sie auf **[!UICONTROL Aktualisieren]**.

   Wenn Sie Ihren Browser aktualisieren, wird in einer Meldung mit einem Link am unteren Rand des [!DNL Workfront for Google Workspace] bestätigt, dass Sie die E-Mail in ein Update konvertiert haben:

   Sie können auf den Link klicken, um zur Registerkarte [!UICONTROL Aktualisierungen] in [!DNL Workfront] für das Objekt zu wechseln, das Sie in Schritt 4 angegeben haben.

   Sie können diese Schritte wiederholen, um dieselbe E-Mail in Aktualisierungen, Aufgaben und Probleme zu konvertieren (siehe [Erstellen eines Adobe Workfront-Problems in [!DNL Google Workspace] Verwenden von E-Mail-Inhalten](../../workfront-integrations-and-apps/workfront-for-g-suite/create-wf-issue-in-g-suite-using-email-content.md)). Wenn Sie Ihren Browser aktualisieren oder zu einem anderen Zeitpunkt zur E-Mail zurückkehren, werden alle Links, die Sie für die E-Mail erstellt haben, unten im Bedienfeld [!UICONTROL Workfront für Google Workspace] aufgeführt.

1. (Optional) Fahren Sie mit der Aktualisierung im Add-on-Bedienfeld &quot;[!DNL Workfront]&quot; fort, indem Sie einen der folgenden Schritte ausführen:

   * Um ein weiteres Update zur Registerkarte **[!UICONTROL Updates]** hinzuzufügen, klicken Sie auf **[!UICONTROL Neues Update starten]** und geben Sie die Informationen ein.

   * Um auf eine Aktualisierung auf der Registerkarte **[!UICONTROL Aktualisierungen]** zu antworten, klicken Sie auf **[!UICONTROL Antworten]** und geben Sie Ihre Antwort ein.

     Bei beiden oben genannten Optionen können Sie auf &quot;**[!UICONTROL &quot; klicken]** um Empfänger für die Antwort anzugeben, wie in Schritt 5 beschrieben. Wenn Sie fertig sind, klicken Sie auf **[!UICONTROL Posten]**, um die Aktualisierung oder Antwort hinzuzufügen.

   * Klicken Sie auf **[!UICONTROL Details]**, um die Details für das neue Projekt, die neue Aufgabe oder das neue Problem anzuzeigen.
