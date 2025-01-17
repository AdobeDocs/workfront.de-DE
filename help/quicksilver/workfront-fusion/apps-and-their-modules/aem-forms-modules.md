---
filename: aem-assets-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: Steckverbinder
navigation-topic: apps-and-their-modules
title: Adobe Experience Manager Forms-Module
description: Die Dokumentation zu Adobe Workfront Fusion wurde an einen neuen Speicherort verschoben. Dieser Artikel ist veraltet, enthält jedoch einen Link zum neuen Artikel, der diese Funktion behandelt.
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: 107d81f7-ca41-4d76-a6dd-e579886dc2ad
source-git-commit: efbe888d370e20c895dc40f18f999f2d01ec6337
workflow-type: tm+mt
source-wordcount: '632'
ht-degree: 1%

---

# [!DNL Adobe Experience Manager Forms]

>[!IMPORTANT]
>
>Die Dokumentation zu Adobe Workfront Fusion wurde an einen neuen Speicherort verschoben.
>
>Die Informationen in diesem Artikel finden Sie jetzt im Artikel:
>
>* [Adobe Experience Manager Forms-Module](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/apps-and-their-modules/adobe-connectors/aem-forms-modules.html)
>
>Bitte aktualisieren Sie alle Lesezeichen.
>
>Dieser Artikel wird nicht mehr aktualisiert und in naher Zukunft entfernt.

Mit dem [!DNL Adobe Experience Manager Forms]-Connector für [!DNL Adobe Workfront Fusion] können Sie ein Szenario starten, das auf Ereignissen in Ihrem [!DNL Adobe Experience Manager Forms]-Konto basiert, indem Sie einen Webhook erstellen.

Sie können ein Formular in [!DNL Adobe Experience Manager Forms] so konfigurieren, dass Formularübermittlungen an diesen Webhook gesendet werden.

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Funktion in diesem Artikel verwenden zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Plan*</td>
  <td> <p>[!UICONTROL Pro] oder höher</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] Lizenz*</td>
   <td> <p>[!UICONTROL-Plan], [!UICONTROL-Arbeit]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] Lizenz **</td> 
   <td>
   <p>Aktuelle Lizenzanforderung: Keine [!DNL Workfront Fusion].</p>
   <p>Oder</p>
   <p>Legacy-Lizenzanforderung: [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>
   <p>Aktuelle Produktanforderung: Wenn Sie über den [!DNL Adobe Workfront] [!UICONTROL Select] oder [!UICONTROL Prime] verfügen, muss Ihr Unternehmen [!DNL Adobe Workfront Fusion] erwerben und [!DNL Adobe Workfront], die in diesem Artikel beschriebenen Funktionen zu nutzen. [!DNL Workfront Fusion] ist im [!DNL Workfront] [!UICONTROL Ultimate] enthalten.</p>
   <p>Oder</p>
   <p>Legacy-Produktanforderung: Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] erwerben und [!DNL Adobe Workfront], die in diesem Artikel beschriebenen Funktionen zu verwenden.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Wenden Sie sich an Ihren [!DNL Workfront], um herauszufinden, über welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie verfügen.

Informationen zu [!DNL Adobe Workfront Fusion] finden Sie unter [[!DNL Adobe Workfront Fusion] Lizenzen](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Voraussetzungen

* Sie müssen über ein [!DNL Adobe Experience Manager Forms]-Konto verfügen, um dieses Modul verwenden zu können.

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

## Erstellen einer Verbindung mit Adobe Experience Manager Forms

So erstellen Sie eine Verbindung für Ihre [!DNL Adobe Experience Manager Forms]:

1. Klicken Sie **[!UICONTROL Hinzufügen]** neben dem Feld Verbindung auf.

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
          <p>Wählen Sie aus, ob diese Verbindung mit einer Produktions- oder Nicht-Produktionsumgebung verbunden werden soll.</p>
        </td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Typ]</td>
        <td>
          <p>Wählen Sie aus, ob dieses Konto ein Service-Konto oder ein persönliches Konto ist.</p>
        </td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL-Instanz-URL ohne Schrägstrich]</td>
        <td>
          <p>Geben Sie die URL ein, über die Sie auf das Konto zugreifen möchten, ohne den abschließenden Schrägstrich.</p>
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
        <td>Geben Sie Ihre [!DNL Adobe]-Client-ID ein. Dies finden Sie im Abschnitt [!UICONTROL Anmeldeinformationen] des [!DNL Adobe Developer Console].
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Client-Geheimnis]</td>
        <td>Geben Sie Ihr [!DNL Adobe]-Client-Geheimnis ein. Dies finden Sie im Abschnitt [!UICONTROL Anmeldeinformationen] des [!DNL Adobe Developer Console].
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Org ID]</td>
        <td>Geben Sie Ihre [!DNL Adobe] Organisations-ID ein. Dies finden Sie im Abschnitt [!UICONTROL Anmeldeinformationen] des [!DNL Adobe Developer Console].
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL ID des technischen Kontos]</td>
        <td>Geben Sie die ID Ihres [!DNL Adobe] technischen Kontos ein. Dies finden Sie im Abschnitt [!UICONTROL Anmeldeinformationen] des [!DNL Adobe Developer Console].
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Meta Scopes]</td>
        <td>Geben Sie alle passenden Metabereiche ein       </td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Privater Schlüssel]</td>
        <td>
          <p>Geben Sie den privaten Schlüssel ein, der bei der Erstellung Ihrer Anmeldeinformationen im [!DNL Adobe Developer Console] generiert wurde. </p>
          <p>So extrahieren Sie Ihren privaten Schlüssel oder Ihr Zertifikat:</p>
          <ol>
            <li value="1">
              <p>Klicken Sie auf <b>[!UICONTROL Extract]</b>.</p>
            </li>
            <li value="2">
              <p>Wählen Sie den zu extrahierenden Dateityp aus.</p>
            </li>
            <li value="3">
              <p>Wählen Sie die Datei aus, die den privaten Schlüssel oder das Zertifikat enthält.</p>
            </li>
            <li value="4">
              <p>Geben Sie das Kennwort für die Datei ein.</p>
            </li>
            <li value="5">
              <p>Klicken Sie auf <b>[!UICONTROL Speichern]</b>, um die Datei zu extrahieren und zur Verbindungseinrichtung zurückzukehren.</p>
            </li>
          </ol>
        </td>
      </tr>
    </tbody>
    </table>

1. Klicken Sie **[!UICONTROL Fortfahren]**, um die Verbindung zu speichern und zum Modul zurückzukehren.

## Adobe Experience Manager Forms-Modul und seine Felder

Derzeit gibt es nur ein Modul im Adobe Experience Manager Forms-Connector.

### Nach Formularereignissen suchen

Mit diesem Trigger (Webhook) können Sie ein Szenario starten, wenn eine Übermittlungsaktion in einem Adobe Experience Manager-Formular stattfindet.

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
   <td role="rowheader">[!UICONTROL Webhook-Name]</td> 
   <td> <p>Einen Namen für den Webhook eingeben</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Adobe Experience Manager]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/apps-and-their-modules/aem-forms-modules.md#create-a-connection-to-adobe-experience-manager-forms" class="MCXref xref">Erstellen einer Verbindung zu [!DNL Adobe Experience Manager Forms]</a></p> </td> 
  </tr>

Das Modul erstellt einen Webhook und gibt die Webhook-Adresse an, die Sie in [!DNL Adobe Experience Manager Forms] in das Dialogfeld für die Formularübermittlung eingeben können.
