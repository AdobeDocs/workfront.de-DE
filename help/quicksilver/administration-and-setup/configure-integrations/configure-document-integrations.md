---
title: Document Integrations konfigurieren
user-type: administrator
product-area: system-administration;workfront-integrations;setup
navigation-topic: administrator-integrations
description: Als Adobe Workfront-Administrator können Sie Dokumentintegrationen konfigurieren, um Dokumente in Workfront zu verwalten.
author: Courtney, Becky
feature: System Setup and Administration, Workfront Integrations and Apps, Digital Content and Documents
role: Admin
exl-id: cf5c4e3d-b45f-46cd-a938-22e412d1c491
source-git-commit: 04bdfbdf1fa05082fe12c2ab239e861a6db4ee6e
workflow-type: tm+mt
source-wordcount: '1088'
ht-degree: 1%

---

# Dokumentintegrationen konfigurieren

<!-- Audited: 12/2023 -->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">***DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

Als [!DNL Adobe Workfront] -Administrator können Sie Dokumentintegrationen konfigurieren, um Dokumente in [!UICONTROL Workfront] zu verwalten. Sie können auch [!UICONTROL Workfront] so konfigurieren, dass Dokumente nur in Document Services-Anwendungen und nicht in [!UICONTROL Workfront] selbst gespeichert werden. Weitere Informationen finden Sie unter [Aktualisieren und Verknüpfen eines Dokuments von [!UICONTROL Workfront] mit einem externen Cloud-Anbieter](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md#update-and-link-a-document-from-workfront-to-an-external-cloud-provider) in [Verknüpfen von Dokumenten aus externen Anwendungen](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

>[!NOTE]
>
>Um eine offene Kommunikation zwischen [!DNL Workfront Proof] und den [!DNL Workfront] -Servern zu ermöglichen, müssen Sie möglicherweise bestimmte IP-Adressen zu Ihrer Zulassungsliste hinzufügen. Weitere Informationen finden Sie unter [Konfigurieren der Zulassungsliste Ihrer Firewall-](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

Sie müssen über Folgendes verfügen, um die Schritte in diesem Artikel durchzuführen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Plan</td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Lizenz</td> 
   <td><p>Neu: [!UICONTROL Standard]</p>
       <p>oder</p>
       <p>Aktuell: [!UICONTROL Plan]</p></td>
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Sie müssen ein [!DNL Workfront] -Administrator sein.</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Unterstützte Integrationen

<!--DON'T DELETE, DRAFT OR HIDE THIS SECTION IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

Sie können die folgenden Integrationen zum Verwalten von Dokumenten konfigurieren:

<!--
  Experience Manager Assets Essentials </p>
  -->

* [!DNL Workfront DAM]

* [!DNL Workfront Proof]

  Durch die Verknüpfung von Testsendungen von [!DNL Workfront Proof] können Sie Testsendungen, die ursprünglich innerhalb von [!DNL Workfront Proof] erstellt wurden, innerhalb von [!DNL Workfront] verfügbar machen. Für die aktuellen Pläne ist ein [!UICONTROL Pro] [!DNL Workfront] Plan oder höher erforderlich, um diese Funktion zu verwenden. Für die neuen Pläne ist diese Funktion mit allen Plänen verfügbar. Weitere Informationen zu den verschiedenen verfügbaren Plänen finden Sie unter [Workfront-Pläne](https://www.workfront.com/plans).

* [!DNL Microsoft SharePoint]

  Informationen zur Integration mit [!DNL SharePoint] finden Sie unter [Konfigurieren der [!DNL SharePoint] Integration](../../administration-and-setup/configure-integrations/configure-sharepoint-integration.md).

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
  >Sie können Dokumente, die von einem externen Cloud-Anbieter verknüpft sind, auf die gleiche Weise wie Dokumente, die direkt in [!DNL Workfront] hochgeladen wurden, testen und genehmigen.

* Andere Dokumentenanbieter (über benutzerdefinierte Dokumentenintegrationen).

  Für die aktuellen Pläne ist ein [!UICONTROL Pro] [!DNL Workfront] Plan oder höher erforderlich, um diese Funktion zu verwenden. Für die neuen Pläne ist diese Funktion mit allen Plänen verfügbar. Weitere Informationen zu den verschiedenen verfügbaren Plänen finden Sie unter [Workfront-Pläne](https://www.workfront.com/plans).

Darüber hinaus können Sie Ihr [!DNL Workfront] -Dokumenterlebnis mit DAM-Integrationen von Drittanbietern verbessern. Administratoren müssen diese Funktionen aktivieren, damit Benutzer den Dienst mit ihrem [!DNL Workfront] -Konto verknüpfen können.

## Integrationen zum Verwalten von Dokumenten konfigurieren

{{step-1-to-setup}}

1. Klicken Sie im linken Bereich auf **[!UICONTROL Dokumente]** > **[!UICONTROL Cloud-Anbieter].**

1. (Optional) Um Dokumente in einer Document Services-Anwendung und nicht in [!DNL Workfront] zu speichern, wählen Sie **[!UICONTROL Benutzer daran hindern, Dokumente in [!DNL Workfront]] zu speichern.**

1. Wählen Sie die Integrationen aus, die aktiviert werden sollen.
1. Klicken Sie auf **[!UICONTROL Speichern]**.

Wenn Sie Integrationen mit [!DNL Workfront DAM] einrichten, können Sie [!DNL Workfront] aktivieren, um Metadaten in Dokumente einzuschließen. Informationen zum Zuordnen von Metadaten finden Sie unter [Einrichten der Metadaten-Zuordnung](../../administration-and-setup/configure-integrations/set-up-metadata-mapping.md).

## Benutzerdefinierte Dokumentintegrationen konfigurieren

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ***DON'T DELETE, DRAFT OR HIDE THIS SECTION IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **)</p>
-->

Durch eine benutzerdefinierte Dokumentenintegration können [!DNL Workfront] Benutzer Dateien von praktisch jedem System aus mit [!DNL Workfront] verknüpfen, vorausgesetzt, das System funktioniert mit [!DNL Workfront].

Um die benutzerdefinierte Integration für Benutzer verfügbar zu machen, müssen Sie zunächst die Integration erstellen. Informationen zum Erstellen von Integrationen für die Verwendung mit [!DNL Workfront] finden Sie unter [Document Webhooks API](../../wf-api/doc-wbhks-api/docu-webhook-api.md).

Nachdem die benutzerdefinierte Dokumentintegration erstellt wurde, können Sie sie für Benutzer auf Ihrer Site verfügbar machen.

{{step-1-to-setup}}

1. Klicken Sie im linken Bereich auf **[!UICONTROL Dokumente]** > **[!UICONTROL Benutzerdefinierte Integration]**.

1. Klicken Sie auf **[!UICONTROL Benutzerdefinierte Integration hinzufügen]**.
1. Geben Sie die folgenden Informationen ein, um die Integration zu konfigurieren:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Name]</td> 
      <td>Der Name der benutzerdefinierten Integration. Dies ist der Name, den Benutzer bei Verwendung der Integration in Workfront sehen.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Basis-API-URL] </td> 
      <td>Die Basis-HTTP oder sichere HTTP-URL für API-Aufrufe. Beispiel: <code>https://&lt;documentprovider&gt;.com/api/v2</code></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Authentifizierungstyp]</td> 
      <td> <p>Die Authentifizierungsmethode, die beim Ausführen autorisierter API-Aufrufe für die benutzerdefinierte Integration verwendet wird.</p> 
       <ul> 
        <li>Wenn Sie <strong>[!UICONTROL OAuth]</strong> auswählen, fahren Sie mit Schritt 5 fort.</li> 
        <li>Wenn Sie <strong>[!UICONTROL APIKey]</strong> auswählen, fahren Sie mit Schritt 6 fort.</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Bedingt) Wenn Sie die **[!UICONTROL OAuth]**-Authentifizierung für den **[!UICONTROL Authentifizierungstyp]** ausgewählt haben, geben Sie die folgenden Informationen ein:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Authentifizierungs-URL]</td> 
      <td>Die vollständige URL für die Benutzerauthentifizierung. [!DNL Workfront] navigiert Benutzer im Rahmen des OAuth-Bereitstellungsprozesses zu dieser Adresse.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Token Endpoint-URL]</td> 
      <td>Die zum Abruf von OAuth-Token verwendete vollständige API-URL.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Client-ID]</td> 
      <td>Die OAut-Client-ID für diese Integration.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Client Secret]</td> 
      <td>Das OAut-Client-Geheimnis für diese Integration.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Anforderungsparameter]</td> 
      <td> <p>Geben Sie optionale Werte ein, die an die Abfragezeichenfolge jedes API-Aufrufs angehängt werden sollen. Beispielsweise access_type=offline.</p> <p>Um mehrere Anforderungsparameter hinzuzufügen, klicken Sie auf <strong>+Anforderungsparameter hinzufügen</strong>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >Der Umleitungs-URI [!DNL Workfront] , der unten auf der Seite [!UICONTROL Benutzerspezifische Integration] angezeigt wird, listet den URI auf, der zum Registrieren dieser Integration beim externen Dokumentanbieter verwendet wird.

1. (Bedingt) Wenn Sie die Authentifizierung für den **[!UICONTROL Authentifizierungstyp]** mit **[!UICONTROL APIKey]** ausgewählt haben, geben Sie den API-Schlüssel ein, der vom benutzerdefinierten Dokumentenanbieter ausgegeben wurde.

   [!DNL Workfront] verwendet diesen API-Schlüssel, um autorisierte API-Aufrufe an den Dokumentenanbieter durchzuführen.

1. Klicken Sie auf **[!UICONTROL Speichern]** , um die Integration zu erstellen.

## Dokumentintegrationen verwenden

Weitere Informationen dazu, wie Benutzer Testsendungen verwenden können, finden Sie unter [Erstellen von Testsendungen](../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-proofs-in-wf.md).

Informationen dazu, wie Benutzer Dokumentintegrationen von Drittanbietern verwenden können, nachdem Sie sie konfiguriert haben, finden Sie unter [Verknüpfen von Dokumenten aus externen Anwendungen](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

### Konfigurieren von [!DNL Workfront] zum Senden von Metadaten an [!UICONTROL [!DNL Workfront] DAM] {#configure-workfront-to-send-metadata-to-workfront-dam}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ***DON'T DELETE, DRAFT OR HIDE THIS SECTION IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **) </p>
-->

Wenn Sie ein Dokument von [!DNL Workfront] an [!DNL Workfront DAM] senden, können Sie auch Informationen senden, die mit diesem Dokument verknüpft sind. Informationen zum Dokument werden [!DNL Workfront DAM] als Metadaten zugeordnet.

Informationen werden nur einseitig zugeordnet, von [!DNL Workfront] zu [!DNL Workfront DAM] und nur übertragen, wenn das Dokument in [!DNL Workfront DAM] hochgeladen wird. Künftige Änderungen an den Workfront-Feldern aktualisieren die Metadatenfelder nicht mehr in [!DNL Workfront DAM], nachdem das Dokument bereits hochgeladen wurde.\
Sie können dasselbe [!DNL Workfront] -Feld verschiedenen [!DNL Workfront DAM] -Feldern zuordnen, Sie können jedoch nicht dasselbe [!DNL Workfront DAM] -Feld für mehrere [!DNL Workfront] -Felder verwenden.

Wenn Sie mehrere [!DNL Workfront] -Felder konfigurieren müssen, um in ein [!DNL Workfront DAM] -Feld zu exportieren, erstellen Sie zunächst ein berechnetes benutzerdefiniertes Feld in [!DNL Workfront], um alle individuellen benutzerdefinierten Felder eines Objekts anzuzeigen. Ordnen Sie dann das berechnete [!DNL Workfront] -Feld einem [!DNL Workfront DAM] -Feld zu.\
Weitere Informationen zu berechneten benutzerdefinierten Feldern finden Sie unter [Berechnete Felder zu einem Formular hinzufügen](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md).

Die Zuordnung wirkt sich auf alle Dokumente aus, die von einem Benutzer von [!DNL Workfront] in [!UICONTROL Workfront] DAM hochgeladen wurden.

Als [!DNL Workfront] -Administrator müssen Sie [!DNL Workfront DAM] in Workfront aktivieren, bevor Sie die Felder für den Metadatenzuordnungsprozess zuordnen können.

So konfigurieren Sie [!DNL Workfront] für das Senden von Metadaten an [!DNL Workfront DAM]:

{{step-1-to-setup}}

1. Klicken Sie auf **[!UICONTROL Dokumente]** > **[!UICONTROL Metadatenzuordnung]**.

1. Geben Sie im Feld **[!UICONTROL Source-Feld für Zuordnung auswählen]** den Namen des Workfront-Felds ein, das Sie [!DNL Workfront DAM] zuordnen möchten, und wählen Sie es dann aus, wenn es in der Liste angezeigt wird.
1. Wählen Sie im Feld **[!UICONTROL Zielfeld für Zuordnung auswählen]** das Feld [!DNL Workfront DAM] aus, das mit den Informationen im ausgewählten Feld [!DNL Workfront] gefüllt werden soll.

   >[!NOTE]
   >
   > Alle Dokumente, die von Benutzern mit entsprechenden Berechtigungen an [!DNL Workfront DAM] gesendet werden, werden beim Hochladen in [!DNL Workfront DAM] mit den hier zugeordneten [!DNL Workfront] -Feldern aktualisiert.

1. Klicken Sie auf **[!UICONTROL Zuordnung hinzufügen]**.

1. Fügen Sie weitere [!UICONTROL Workfront] -Felder und die entsprechenden [!DNL Workfront DAM] -Felder hinzu.

### Zugeordnete Felder löschen

{{step-1-to-setup}}

1. Erweitern Sie **[!UICONTROL Dokumente]** und klicken Sie dann auf **[!UICONTROL Metadatenzuordnung]**.

1. Wählen Sie in der Feldliste eines der Felder aus, die Sie aus der Metadaten-Zuordnung entfernen möchten.
1. Klicken Sie auf **[!UICONTROL Löschen]**.

   Die Felder werden aus der Metadaten-Zuordnung entfernt und die darin enthaltenen Informationen werden nicht mit den hochgeladenen Dokumenten an [!DNL Workfront DAM] übertragen.
