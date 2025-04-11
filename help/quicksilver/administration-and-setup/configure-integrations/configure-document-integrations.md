---
title: Dokumentintegrationen konfigurieren
user-type: administrator
product-area: system-administration;workfront-integrations;setup
navigation-topic: administrator-integrations
description: Als Adobe Workfront-Administrator können Sie Dokumentintegrationen konfigurieren, um Dokumente in Workfront zu verwalten.
author: Courtney, Becky
feature: System Setup and Administration, Workfront Integrations and Apps, Digital Content and Documents
role: Admin
exl-id: cf5c4e3d-b45f-46cd-a938-22e412d1c491
source-git-commit: 5ff071a6e0af93f5280225355edad1d0dde42b3f
workflow-type: tm+mt
source-wordcount: '1125'
ht-degree: 1%

---

# Dokumentintegrationen konfigurieren

<!-- Audited: 12/2023 -->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">***DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

[!DNL Adobe Workfront] Als Administrator können Sie Dokument Integrationen konfigurieren, um Dokumente in [!UICONTROL Workfront] zu managen. Sie können Workfront] auch so konfigurieren[!UICONTROL , dass Dokumente nur in Dokument Dienstanwendungen und nicht in [!UICONTROL Workfront] selbst gespeichert werden. Weitere Informationen finden Sie unter [Aktualisieren und verknüpfen einer Dokument von [!UICONTROL Workfront] zu einem externen Cloud](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md#update-and-link-a-document-from-workfront-to-an-external-cloud-provider) Anbieter in [Link Dokumente von externen Anwendungen](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

>[!NOTE]
>
>Um eine offene Kommunikation zwischen [!DNL Workfront Proof] den Servern und den [!DNL Workfront] Servern zu ermöglichen, müssen Sie möglicherweise bestimmte IP-Adressen zu Ihrer Zulassungsliste hinzufügen. Weitere Informationen finden Sie unter [Konfigurieren der Zulassungsliste](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md) Ihrer Firewall.

## Voraussetzungen für den Zugriff

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über Folgendes verfügen, um die Schritte in diesem Artikel auszuführen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Plan</td> 
   <td>Beliebig</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Lizenz</td> 
   <td><p>Neu: [!UICONTROL Standard]</p>
       <p>oder</p>
       <p>Aktuell: [!UICONTROL Plan]</p></td>
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Sie müssen [!DNL Workfront] sein.</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Unterstützte Integrationen

<!--DON'T DELETE, DRAFT OR HIDE THIS SECTION IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

Sie können die folgenden Integrationen zum Verwalten von Dokumenten konfigurieren:

<!--
  Experience Manager Assets Essentials </p>
  -->

* [!DNL Workfront DAM]

* [!DNL Workfront Proof]

  Durch das Verknüpfen von Korrekturabzügen aus [!DNL Workfront Proof] können Sie Korrekturabzüge, die ursprünglich in [!DNL Workfront Proof] erstellt wurden, in [!DNL Workfront] verfügbar machen. Für die aktuellen Pläne ist ein [!UICONTROL Pro]-[!DNL Workfront] oder höher erforderlich, um diese Funktion verwenden zu können. Für die neuen Pläne ist diese Funktion in allen Plänen verfügbar. Weitere Informationen zu den verschiedenen verfügbaren Plänen finden Sie unter [Workfront-Pläne](https://www.workfront.com/plans).

* [!DNL Microsoft SharePoint]

  For information about integrating with [!DNL SharePoint], see [Configure the [!DNL SharePoint] integration](../../administration-and-setup/configure-integrations/configure-sharepoint-integration.md).

* Drittanbieter von Cloud-Dokumenten:

   * [!DNL Box]
   * [!DNL Dropbox]
   * [!DNL Dropbox Business]
   * [!DNL WebDAM]
   * [!DNL Microsoft OneDrive]
   * [!DNL Microsoft SharePoint]
   * [!UICONTROL Google-Laufwerk]
   * Quip

  >[!TIP]
  >
  >Sie können von einem externen Cloud-Anbieter verknüpfte Dokumente auf die gleiche Weise prüfen und genehmigen wie Dokumente, die direkt in [!DNL Workfront] hochgeladen wurden.

* Andere Dokumentanbieter (über benutzerdefinierte Dokumentintegrationen).

  Für die aktuellen Pläne ist ein [!UICONTROL Pro]-[!DNL Workfront] oder höher erforderlich, um diese Funktion verwenden zu können. Für die neuen Pläne ist diese Funktion in allen Plänen verfügbar. Weitere Informationen zu den verschiedenen verfügbaren Plänen finden Sie unter [Workfront-Pläne](https://www.workfront.com/plans).

In addition, you can enhance your [!DNL Workfront] document experience with a third-party DAM integrations. Administratoren müssen diese Funktionen aktivieren bestellen Benutzer den Dienst auf ihrer Konto verknüpfen können [!DNL Workfront] .

## Konfigurieren von Integrationen für managen Dokumente

{{step-1-to-setup}}

1. Klicken Sie im linken Bedienfeld auf Dokumente **** > **[!UICONTROL Cloud-Anbieter].**

1. (Optional) To stored documents in a document services application and not in [!DNL Workfront], select **[!UICONTROL Prevent Users From Storing Documents in [!DNL Workfront]].**

1. Select the integrations you want enabled.
1. Klicken Sie auf **[!UICONTROL Speichern]**.

If you are setting up integrations with [!DNL Workfront DAM], you can enable [!DNL Workfront] to include metadata with documents. For information about mapping metadata, see [Set up metadata mapping](../../administration-and-setup/configure-integrations/set-up-metadata-mapping.md).

## Configure custom document integrations

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ***DON'T DELETE, DRAFT OR HIDE THIS SECTION IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **)</p>
-->

Eine benutzerdefinierte Dokument-Integration ermöglicht es [!DNL Workfront] Benutzern, Dateien von praktisch jedem System aus zu [!DNL Workfront] verknüpfen, vorausgesetzt, das System ist für die Arbeit mit [!DNL Workfront].

Um die benutzerdefinierte Integration für -Benutzer verfügbar zu machen, müssen Sie zunächst die Integration erstellen. Informationen zum Erstellen von Integrationen für die Verwendung mit [!DNL Workfront] finden Sie unter [Document Webhooks API](../../wf-api/doc-wbhks-api/docu-webhook-api.md).

Nachdem die benutzerdefinierte Dokumentenintegration erstellt wurde, können Sie sie für Benutzer auf Ihrer Site verfügbar machen.

{{step-1-to-setup}}

1. Klicken Sie im linken Bedienfeld auf **[!UICONTROL Dokumente]** > **[!UICONTROL Benutzerdefinierte Integration]**.

1. Klicken Sie **[!UICONTROL Benutzerdefinierte Integration hinzufügen]**.
1. Geben Sie die folgenden Informationen ein, um die Integration zu konfigurieren:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Name]</td> 
      <td>The name of the custom integration. This is the name users see when using the integration within Workfront.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Base API URL] </td> 
      <td>The base HTTP or secure HTTP URL for API calls. Beispiel: <code>https://&lt;documentprovider&gt;.com/api/v2</code></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Authentication Type]</td> 
      <td> <p>The authentication method to use when making authorized API calls to the custom integration.</p> 
       <ul> 
        <li>If you choose <strong>[!UICONTROL OAuth]</strong>, continue with Step 5.</li> 
        <li>If you choose <strong>[!UICONTROL ApiKey]</strong>, continue with Step 6.</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Conditional) If you selected **[!UICONTROL OAuth]** authentication for the **[!UICONTROL Authentication Type]**, enter the following information:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[! UICONTROL Authentication URL]</td> 
      <td>Der vollständige URL für die User-Authentifizierung verwendet. [!DNL Workfront] navigiert Benutzer im Rahmen des OAuth Bereitstellung-Prozesses zu dieser Adresse.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[! UICONTROL Token Endpoint URL]</td> 
      <td>Die zum Abruf von OAuth-Token verwendete vollständige API-URL.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Client-ID]</td> 
      <td>Die OAut Client ID für diese Integration.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[! UICONTROL-Client Geheimnis]</td> 
      <td>Das OAut Client Geheimnis für diese Integration.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[! UICONTROL-Anfrage Parameter]</td> 
      <td> <p>Geben Sie optionale Werte ein, die an die Abfragezeichenfolge jedes API-Aufrufs angehängt werden. Beispiel: access_type=offline.</p> <p>Um mehrere Anfrageparameter hinzuzufügen, klicken Sie auf <strong>+Anfrageparameter hinzufügen</strong>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >Der [!DNL Workfront] Umleitungs-URI, der unten auf der Seite &quot;[!UICONTROL  Integration“ angezeigt wird] listet den URI auf, mit dem diese Integration beim externen Dokumentanbieter registriert wurde.

1. (Bedingt) Wenn Sie **[!UICONTROL ApiKey]**-Authentifizierung für den **[!UICONTROL Authentifizierungstyp]** ausgewählt haben, geben Sie den API-Schlüssel ein, der vom benutzerdefinierten Dokumentanbieter ausgestellt wurde.

   [!DNL Workfront] verwendet diesen API-Schlüssel für autorisierte API-Aufrufe an den Dokumentanbieter.

1. Klicken Sie **[!UICONTROL Speichern]**, um die Integration zu erstellen.

## Verwenden von Dokumentintegrationen

Informationen dazu, wie Benutzer Proofing verwenden können, finden Sie unter [Erstellen von Korrekturabzügen](../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-proofs-in-wf.md).

Informationen dazu, wie Benutzer nach der Konfiguration Dokumentintegrationen von Drittanbietern verwenden können, finden Sie unter [Verknüpfen von Dokumenten aus externen Programmen](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

### Konfigurieren von [!DNL Workfront] zum Senden von Metadaten an [!UICONTROL [!DNL Workfront] DAM] {#configure-workfront-to-send-metadata-to-workfront-dam}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ***DON'T DELETE, DRAFT OR HIDE THIS SECTION IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **) </p>
-->

Beim Senden eines Dokuments von [!DNL Workfront] an [!DNL Workfront DAM] können Sie auch mit diesem Dokument verknüpfte Informationen senden. Informationen zum Dokument werden [!DNL Workfront DAM] als Metadaten zugeordnet.

Informationen werden nur in eine Richtung zugeordnet, von [!DNL Workfront] zu [!DNL Workfront DAM], und sie werden nur übertragen, wenn das Dokument in [!DNL Workfront DAM] hochgeladen wird. Zukünftige Änderungen in den Workfront-Feldern werden die Metadatenfelder in [!DNL Workfront DAM] nicht aktualisieren, nachdem das Dokument bereits hochgeladen wurde.\
Sie können dasselbe [!DNL Workfront] verschiedenen [!DNL Workfront DAM] zuordnen, aber Sie können dasselbe [!DNL Workfront DAM] nicht für mehrere [!DNL Workfront] verwenden.

Wenn Sie mehrere [!DNL Workfront] für den Export in ein [!DNL Workfront DAM] konfigurieren müssen, erstellen Sie zunächst ein berechnetes benutzerdefiniertes Feld, [!DNL Workfront] alle individuellen Felder eines Objekts anzuzeigen. Ordnen Sie dann das berechnete [!DNL Workfront] einem [!DNL Workfront DAM] zu.\
For more information about calculated custom fields, see [Add calculated fields to a form](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md).

The mapping affects all the documents uploaded by any user from [!DNL Workfront] to [!UICONTROL Workfront] DAM.

Als [!DNL Workfront] müssen Sie [!DNL Workfront DAM] in Workfront aktivieren, bevor Sie die Felder für den Metadatenzuordnungsprozess zuordnen können.

So konfigurieren Sie [!DNL Workfront] zum Senden von Metadaten an [!DNL Workfront DAM]:

{{step-1-to-setup}}

1. Klicken Sie **[!UICONTROL Dokumente]** > **[!UICONTROL Metadatenzuordnung]**.

1. Beginnen Sie im Feld **[!UICONTROL Source-Feld für Zuordnung auswählen]** mit der Eingabe des Namens des Workfront-Felds, dem Sie [!DNL Workfront DAM] zuordnen möchten, und wählen Sie es aus, wenn Sie es in der Liste sehen.
1. Wählen **[!UICONTROL im Feld Zielfeld für Zuordnung auswählen]** das [!DNL Workfront DAM] Feld aus, das Sie mit den Informationen im ausgewählten [!DNL Workfront] füllen möchten.

   >[!NOTE]
   >
   > Bei allen Dokumenten, die von dazu berechtigten Benutzenden an [!DNL Workfront DAM] gesendet werden, werden die Metadaten dieser Dokumente mit den [!DNL Workfront] hier zugeordneten Feldern aktualisiert, wenn sie in [!DNL Workfront DAM] hochgeladen werden.

1. Click **[!UICONTROL Add Mapping]**.

1. Continue adding more [!UICONTROL Workfront] fields and corresponding [!DNL Workfront DAM] fields.

### Löschen gemappte Felder

{{step-1-to-setup}}

1. **[!UICONTROL Erweitern Dokumente]** und klicken Sie auf &quot;**[!UICONTROL Metadatenzuordnung]**&quot;.

1. Wählen Sie in der Liste der Felder eines der Felder aus, die Sie aus Metadaten Mapping entfernen möchten.
1. Click **[!UICONTROL Delete]**.

   Die Felder werden aus der Metadatenzuordnung entfernt und die darin enthaltenen Informationen werden nicht an [!DNL Workfront DAM] mit den hochgeladenen Dokumenten übertragen.


## Einschränkungen

* Die Google Drive-Dokumentintegration unterstützt das Hinzufügen von Ordnern und Bildern aus dem Bereich „Mein Laufwerk“ auf dem Google-Laufwerk. Sie können keine Ordner oder Bilder von einem freigegebenen Laufwerk hinzufügen. Weitere Informationen zu [Google Shared Drives](https://support.google.com/a/users/answer/7212025?hl=en).