---
filename: aem-assets-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: Connector
navigation-topic: apps-and-their-modules
title: Adobe Experience Manager Forms-Module
description: Mit dem [!DNL Adobe Experience Manager Forms] Connector für das [!DNL Adobe Workfront Fusion], you can start a scenario based on events in your [!DNL Adobe Experience Manager Forms] -Konto können Sie Assets erstellen, hochladen und aktualisieren sowie Ordner und Assets kopieren oder verschieben.
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: 107d81f7-ca41-4d76-a6dd-e579886dc2ad
source-git-commit: 27fb07b7b19bab25bb7ee925e722ccace3bea628
workflow-type: tm+mt
source-wordcount: '573'
ht-degree: 1%

---

# [!DNL Adobe Experience Manager Forms] Module

Mit dem [!DNL Adobe Experience Manager Forms] -Connector für [!DNL Adobe Workfront Fusion] können Sie ein Szenario starten, das auf Ereignissen in Ihrem [!DNL Adobe Experience Manager Forms] -Konto basiert, indem Sie einen Webhook erstellen.

Sie können ein Formular innerhalb von [!DNL Adobe Experience Manager Forms] konfigurieren, um Formulareinsendungen an diesen Webhook zu senden.

## Zugriffsanforderungen

Sie müssen über den folgenden Zugriff verfügen, um die Funktionalität in diesem Artikel verwenden zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td>
  <td> <p>[!UICONTROL Pro] oder höher</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td>
   <td> <p>[!UICONTROL Plan], [!UICONTROL Arbeit]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] license**</td> 
   <td>
   <p>Aktuelle Lizenzanforderungen: Keine [!DNL Workfront Fusion] Lizenzanforderungen.</p>
   <p>Oder</p>
   <p>Alte Lizenzanforderung: [!UICONTROL [!DNL Workfront Fusion] für die Arbeitsautomatisierung und -integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>
   <p>Aktuelle Produktanforderung: Wenn Sie über den [!UICONTROL Select]- oder [!UICONTROL Prime] [!DNL Adobe Workfront]-Plan verfügen, muss Ihr Unternehmen [!DNL Adobe Workfront Fusion] sowie [!DNL Adobe Workfront] erwerben, um die in diesem Artikel beschriebenen Funktionen nutzen zu können. [!DNL Workfront Fusion] ist im [!UICONTROL Ultimate] [!DNL Workfront]-Plan enthalten.</p>
   <p>Oder</p>
   <p>Alte Produktanforderung: Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] sowie [!DNL Adobe Workfront] erwerben, um die in diesem Artikel beschriebenen Funktionen nutzen zu können.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Wenden Sie sich an Ihren [!DNL Workfront] -Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

Informationen zu [!DNL Adobe Workfront Fusion] -Lizenzen finden Sie unter [[!DNL Adobe Workfront Fusion] Lizenzen](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Voraussetzungen

* Sie müssen über ein [!DNL Adobe Experience Manager Forms] -Konto verfügen, um dieses Modul verwenden zu können.

## Adobe Experience Manager Assets-API-Informationen

Der Adobe Experience Manager Assets-Connector verwendet Folgendes:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">API-Tag</td> 
   <td>v1.2.27</td> 
  </tr>
 </tbody> 
 </table>

## Herstellen einer Verbindung zu Adobe Experience Manager Forms

So erstellen Sie eine Verbindung für Ihre [!DNL Adobe Experience Manager Forms] -Module:

1. Klicken Sie neben dem Feld Verbindung auf **[!UICONTROL Hinzufügen]** .

1. Füllen Sie die folgenden Felder aus:

   <table style="table-layout:auto"> 
    <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1">
    </col>
    <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2">
    </col>
    <tbody>
      <tr>
        <td role="rowheader">[!UICONTROL Verbindungsname]</td>
        <td>
          <p>Geben Sie einen Namen für diese Verbindung ein.</p>
        </td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Umgebung]</td>
        <td>
          <p>Wählen Sie aus, ob diese Verbindung eine Verbindung zu einer Produktions- oder Nicht-Produktionsumgebung herstellt.</p>
        </td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Typ]</td>
        <td>
          <p>Wählen Sie aus, ob es sich bei diesem Konto um ein Dienstkonto oder ein persönliches Konto handelt.</p>
        </td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Instanz-URL ohne Schrägstrich]</td>
        <td>
          <p>Geben Sie die URL ein, die Sie für den Zugriff auf das Konto verwenden, ohne den endgültigen Schrägstrich einzufügen.</p>
        </td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL IMS-Endpunkt]</td>
        <td>
          <p><code>https://ims-na1.adobelogin.com</code></p>
        </td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Client-ID]</td>
        <td>Geben Sie Ihre [!DNL Adobe] Client-ID ein. Dies finden Sie im Abschnitt [!UICONTROL Anmeldeinformationen] des Abschnitts [!DNL Adobe Developer Console].
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Client Secret]</td>
        <td>Geben Sie Ihr [!DNL Adobe] Client-Geheimnis ein. Dies finden Sie im Abschnitt [!UICONTROL Anmeldeinformationen] des Abschnitts [!DNL Adobe Developer Console].
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Organisations-ID]</td>
        <td>Geben Sie Ihre [!DNL Adobe] Organisations-ID ein. Dies finden Sie im Abschnitt [!UICONTROL Anmeldeinformationen] des Abschnitts [!DNL Adobe Developer Console].
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL ID des technischen Kontos]</td>
        <td>Geben Sie Ihre [!DNL Adobe] ID des technischen Kontos ein. Dies finden Sie im Abschnitt [!UICONTROL Anmeldeinformationen] des Abschnitts [!DNL Adobe Developer Console].
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Meta Scopes]</td>
        <td>Eingeben der entsprechenden Meta-Bereiche       </td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Privater Schlüssel]</td>
        <td>
          <p>Geben Sie den privaten Schlüssel ein, der beim Erstellen Ihrer Anmeldedaten in der [!DNL Adobe Developer Console] generiert wurde. </p>
          <p>So extrahieren Sie Ihren privaten Schlüssel oder Ihr Zertifikat:</p>
          <ol>
            <li value="1">
              <p>Klicken Sie auf <b>[!UICONTROL Extract]</b>.</p>
            </li>
            <li value="2">
              <p>Wählen Sie den Dateityp aus, den Sie extrahieren.</p>
            </li>
            <li value="3">
              <p>Wählen Sie die Datei aus, die den privaten Schlüssel oder das Zertifikat enthält.</p>
            </li>
            <li value="4">
              <p>Geben Sie das Kennwort für die Datei ein.</p>
            </li>
            <li value="5">
              <p>Klicken Sie auf <b>[!UICONTROL Save]</b> , um die Datei zu extrahieren und zur Verbindungseinrichtung zurückzukehren.</p>
            </li>
          </ol>
        </td>
      </tr>
    </tbody>
    </table>

1. Klicken Sie auf **[!UICONTROL Weiter]** , um die Verbindung zu speichern und zum Modul zurückzukehren.

## Adobe Experience Manager Forms-Modul und seine Felder

Derzeit befindet sich nur ein Modul im Adobe Experience Manager Forms-Connector.

### Formularereignisse beobachten

Mit diesem Instant Trigger (Webhook) können Sie ein Szenario starten, wenn eine Sendeaktion in einem Adobe Experience Manager-Formular auftritt.

>[!IMPORTANT]
>
>Dieses Modul muss auch in Adobe Experience Manager konfiguriert werden. Nachdem Sie diesen Webhook eingerichtet haben, müssen Sie Adobe Experience Manager öffnen und Ihr Formular so konfigurieren, dass Übermittlungen an den Webhook gesendet werden.
>
><!--For instructions on the required form configuration, see insert url here-->

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Webhook name]</td> 
   <td> <p>Geben Sie einen Namen für den Webhook ein</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Adobe Experience Manager]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/apps-and-their-modules/aem-forms-modules.md#create-a-connection-to-adobe-experience-manager-forms" class="MCXref xref">Erstellen einer Verbindung zu [!DNL Adobe Experience Manager Forms]</a> .</p> </td> 
  </tr>

Das Modul erstellt einen Webhook und gibt Ihnen die Webhook-Adresse, die Sie in das Formularübermittlungsdialogfeld in [!DNL Adobe Experience Manager Forms] eingeben können.
