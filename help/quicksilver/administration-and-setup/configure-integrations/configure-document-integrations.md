---
title: Dokumentintegrationen konfigurieren
user-type: administrator
product-area: system-administration;workfront-integrations;setup
navigation-topic: administrator-integrations
description: Dokumentintegrationen konfigurieren
author: Courtney, Caroline
feature: System Setup and Administration, Workfront Integrations and Apps, Digital Content and Documents
role: Admin
exl-id: cf5c4e3d-b45f-46cd-a938-22e412d1c491
source-git-commit: ceda437684f565b91dbb8b02f6b03cbe8d27a70a
workflow-type: tm+mt
source-wordcount: '1161'
ht-degree: 1%

---

# Dokumentintegrationen konfigurieren

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">***DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

Als [!DNL Adobe Workfront] Administrator können Sie Dokumentintegrationen konfigurieren, um Dokumente in zu verwalten [!UICONTROL Workfront]. Sie können auch [!UICONTROL Workfront] sodass Dokumente nur in Document Services-Anwendungen und nicht in gespeichert werden [!UICONTROL Workfront] selbst. Weitere Informationen finden Sie unter [Aktualisieren und Verknüpfen eines Dokuments aus [!UICONTROL Workfront] zu einem externen Cloud-Anbieter](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md#sending-documents) in [Verknüpfen von Dokumenten mit externen Anwendungen](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

>[!NOTE]
>
>Offene Kommunikation zwischen [!DNL Workfront Proof] und [!DNL Workfront] -Servern verwenden, müssen Sie möglicherweise bestimmte IP-Adressen zu Ihrer Zulassungsliste hinzufügen. Weitere Informationen finden Sie unter [Konfigurieren der Zulassungsliste Ihrer Firewall](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

## Zugriffsanforderungen

Sie müssen über Folgendes verfügen, um die Schritte in diesem Artikel durchzuführen:

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
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Sie müssen [!DNL Workfront] Administrator. Informationen über [!DNL Workfront] Administratoren, siehe <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Gewähren eines vollen Administratorzugriffs</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren [!DNL Workfront] Administrator.

## Unterstützte Integrationen

<!--DON'T DELETE, DRAFT OR HIDE THIS SECTION IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

Sie können die folgenden Integrationen zum Verwalten von Dokumenten konfigurieren:

<!--
  Experience Manager Assets Essentials </p>
  -->

* [!DNL Workfront DAM]

* [!DNL Workfront Proof]

   Verknüpfen von Testsendungen aus [!DNL Workfront Proof] ermöglicht Ihnen die Durchführung von Testsendungen, die ursprünglich in [!DNL Workfront Proof] verfügbar innerhalb [!DNL Workfront]. A [!UICONTROL Pro] [!DNL Workfront] Für die Verwendung dieser Funktion ist ein Plan oder höher erforderlich. Weitere Informationen zu den verschiedenen verfügbaren Plänen finden Sie unter [Workfront-Pläne.](https://www.workfront.com/plans)

* [!DNL Microsoft SharePoint]

   Informationen zur Integration mit [!DNL SharePoint], siehe [Konfigurieren Sie die [!DNL SharePoint] Integration](../../administration-and-setup/configure-integrations/configure-sharepoint-integration.md).

* Drittanbieter von Cloud-Dokumenten:

   * [!DNL Box]
   * [!DNL Dropbox]
   * [!DNL Dropbox Business]
   * [!DNL WebDAM]
   * [!DNL Microsoft OneDrive]
   * [!UICONTROL Google Drive]

      <!--Quip-->
   >[!TIP]
   >
   >Sie können Dokumente, die von einem externen Cloud-Anbieter verknüpft sind, auf dieselbe Weise prüfen und genehmigen wie Dokumente, die direkt in hochgeladen wurden [!DNL Workfront].

* Andere Dokumentenanbieter (über benutzerdefinierte Dokumentenintegrationen).

   A [!UICONTROL Pro] [!DNL Workfront] Für die Verwendung dieser Funktion ist ein Plan oder höher erforderlich. Weitere Informationen zu den verschiedenen verfügbaren Plänen finden Sie unter [[!DNL Workfront] Pläne.](https://www.workfront.com/plans)

Darüber hinaus können Sie Ihre [!DNL Workfront] Dokumenterfahrung mit einem nativen DAM-System (Digital Asset Management) oder mit DAM-Integrationen von Drittanbietern. Administratoren müssen diese Funktionen aktivieren, damit Benutzer den Dienst mit ihrer [!DNL Workfront] -Konto. Weitere Informationen zu Workfront DAM finden Sie unter [Verwalten von Dokumenten mit [!DNL Adobe Workfront DAM]](../../documents/workfront-dam-within-workfront/manage-docs-with-wf-dam.md).

## Integrationen zum Verwalten von Dokumenten konfigurieren

1. Anmelden bei [!DNL Workfront] als Administrator.
1. Klicken Sie auf **[!UICONTROL Hauptmenü]** icon ![](assets/main-menu-icon.png) in der oberen rechten Ecke von [!DNL Adobe Workfront]Klicken Sie auf **[!UICONTROL Einrichtung]** ![](assets/gear-icon-settings.png).

1. Klicken Sie im linken Bereich auf **[!UICONTROL Dokumente]** > **[!UICONTROL Cloud-Anbieter].**

1. (Optional) So speichern Sie Dokumente in einer Document Services-Anwendung und nicht in [!DNL Workfront]auswählen **[!UICONTROL Benutzer daran hindern, Dokumente in zu speichern [!DNL Workfront]].**

1. Wählen Sie die Integrationen aus, die aktiviert werden sollen.
1. Klicken Sie auf **[!UICONTROL Speichern]**.

Wenn Sie Integrationen mit [!DNL Workfront DAM]können Sie [!DNL Workfront] , um Metadaten in Dokumente einzuschließen. Informationen zum Zuordnen von Metadaten finden Sie unter [Einrichten der Metadaten-Zuordnung](../../administration-and-setup/configure-integrations/set-up-metadata-mapping.md).

## Benutzerdefinierte Dokumentintegrationen konfigurieren

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ***DON'T DELETE, DRAFT OR HIDE THIS SECTION IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **)</p>
-->

Eine benutzerdefinierte Dokumentintegration ermöglicht Folgendes [!DNL Workfront] Benutzer, die Dateien verknüpfen [!DNL Workfront] von praktisch jedem System aus, sofern das System für die Arbeit mit [!DNL Workfront].

Um die benutzerdefinierte Integration für Benutzer verfügbar zu machen, müssen Sie zunächst die Integration erstellen. Informationen zum Erstellen von Integrationen, die mit [!DNL Workfront], siehe [Document Webhooks-API](../../wf-api/doc-wbhks-api/docu-webhook-api.md).

Nachdem die benutzerdefinierte Dokumentintegration erstellt wurde, können Sie sie für Benutzer auf Ihrer Site verfügbar machen.

1. Anmelden bei [!DNL Workfront] als Administrator.
1. Klicken Sie auf **[!UICONTROL Hauptmenü]** icon ![](assets/main-menu-icon.png) in der oberen rechten Ecke von [!DNL Adobe Workfront]Klicken Sie auf **[!UICONTROL Einrichtung]** ![](assets/gear-icon-settings.png).

1. Klicken Sie im linken Bereich auf **[!UICONTROL Dokumente]** > **[!UICONTROL Benutzerdefinierte Integration].**

1. Klicken **[!UICONTROL Benutzerdefinierte Integration hinzufügen]**.
1. Geben Sie die folgenden Informationen zum Konfigurieren der Integration an:

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
      <td>Die Basis-HTTP oder sichere HTTP-URL für API-Aufrufe. Beispiel: <a class="link-https" title="https://documentprovider.com/api/v2" href="https://documentprovider.com/api/v2">https://documentprovider.com/api/v2</a></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Authentifizierungstyp]</td> 
      <td> <p>Die Authentifizierungsmethode, die beim Ausführen autorisierter API-Aufrufe für die benutzerdefinierte Integration verwendet wird.</p> 
       <ul> 
        <li>Wenn Sie <strong>[!UICONTROL OAuth]</strong>, fahren Sie mit Schritt 6 fort.</li> 
        <li>Wenn Sie <strong>[!UICONTROL APIKey]</strong>, fahren Sie mit Schritt 7 fort.</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Bedingt) Wenn Sie ausgewählt haben **[!UICONTROL OAuth]** Authentifizierung für **[!UICONTROL Authentifizierungstyp]** Geben Sie die folgenden Informationen an:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Authentifizierungs-URL]</td> 
      <td>Die vollständige URL, die für die Benutzerauthentifizierung verwendet wird. [!DNL Workfront] navigiert Benutzer im Rahmen des OAuth-Bereitstellungsprozesses zu dieser Adresse.</td> 
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
      <td> <p>Geben Sie optionale Werte an, die an die Abfragezeichenfolge jedes API-Aufrufs angehängt werden sollen. Beispielsweise access_type=offline.</p> <p>Um mehrere Anforderungsparameter hinzuzufügen, klicken Sie auf <strong>+Anforderungsparameter hinzufügen</strong>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >Die [!DNL Workfront] Umleitungs-URI, der unten im [!UICONTROL Benutzerdefinierte Integration] auf der Seite wird der URI aufgelistet, der zum Registrieren dieser Integration beim externen Dokumentanbieter verwendet wird.

1. (Bedingt) Wenn Sie ausgewählt haben **[!UICONTROL ApiKey]** Authentifizierung für **[!UICONTROL Authentifizierungstyp]** Geben Sie den API-Schlüssel an, der vom benutzerdefinierten Dokumentenanbieter ausgegeben wurde.

   [!DNL Workfront] verwendet diesen API-Schlüssel, um autorisierte API-Aufrufe an den Dokumentenanbieter durchzuführen.

1. Klicken **[!UICONTROL Speichern]** , um die Integration zu erstellen.

## Dokumentintegrationen verwenden

Informationen darüber, wie Benutzer [!DNL Workfront DAM], siehe [Verwalten von Dokumenten mit [!DNL Adobe Workfront DAM]](../../documents/workfront-dam-within-workfront/manage-docs-with-wf-dam.md).

Informationen dazu, wie Benutzer die Prüfung verwenden können, finden Sie unter [Testsendungen erstellen](../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-proofs--in-wf.md).

Informationen dazu, wie Benutzer Dokumentintegrationen von Drittanbietern verwenden können, nachdem Sie sie konfiguriert haben, finden Sie unter [Verknüpfen von Dokumenten mit externen Anwendungen](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

### Konfigurieren [!DNL Workfront] Senden von Metadaten an [!UICONTROL [!DNL Workfront] DAM] {#configure-workfront-to-send-metadata-to-workfront-dam}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ***DON'T DELETE, DRAFT OR HIDE THIS SECTION IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **) </p>
-->

Beim Senden eines Dokuments aus [!DNL Workfront] nach [!DNL Workfront DAM]können Sie auch Informationen senden, die mit diesem Dokument verknüpft sind. Informationen zum Dokument werden [!DNL Workfront DAM] als Metadaten.

Informationen werden nur einseitig zugeordnet, von [!DNL Workfront] nach [!DNL Workfront DAM] und wird nur übertragen, wenn das Dokument hochgeladen wird [!DNL Workfront DAM]. Zukünftige Änderungen an den Workfront-Feldern aktualisieren keine Metadatenfelder in [!DNL Workfront DAM] nachdem das Dokument bereits hochgeladen wurde.\
Sie können die gleiche [!DNL Workfront] -Feld zu verschiedenen [!DNL Workfront DAM] nicht verwenden. [!DNL Workfront DAM] Feld für mehrere [!DNL Workfront] -Felder.

Wenn mehrere [!DNL Workfront] Felder, die in eine Datei exportiert werden sollen [!DNL Workfront DAM] erstellen Sie zunächst ein berechnetes benutzerdefiniertes Feld in [!DNL Workfront] , um alle einzelnen benutzerdefinierten Felder eines Objekts anzuzeigen. Ordnen Sie dann die berechnete [!DNL Workfront] -Feld zu einem [!DNL Workfront DAM] -Feld.\
Weitere Informationen zu berechneten benutzerdefinierten Feldern finden Sie unter [Hinzufügen errechneter Daten zu einem benutzerdefinierten Formular](../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

Die Zuordnung wirkt sich auf alle Dokumente aus, die von einem beliebigen Benutzer hochgeladen wurden. [!DNL Workfront] nach [!UICONTROL Workfront] DAM.

Als [!DNL Workfront] Administrator, müssen Sie [!DNL Workfront DAM] in Workfront, bevor Sie die Felder für den Metadaten-Zuordnungsprozess zuordnen können. Weitere Informationen zum Aktivieren von [!DNL Workfront DAM], siehe [Konfigurieren von Workfront zum Senden von Metadaten an [!DNL Workfront DAM]](#configure-workfront-to-send-metadata-to-workfront-dam).

So konfigurieren Sie [!DNL Workfront] Senden von Metadaten an [!DNL Workfront DAM]:

1. Klicken Sie auf **[!UICONTROL Hauptmenü]** icon ![](assets/main-menu-icon.png) in der oberen rechten Ecke von [!DNL Adobe Workfront]Klicken Sie auf **[!UICONTROL Einrichtung]** ![](assets/gear-icon-settings.png).

1. Klicken **[!UICONTROL Dokumente]** > **[!UICONTROL Metadatenzuordnung]**.

1. Im **[!UICONTROL Quellfeld für Zuordnung auswählen]** eingeben, beginnen Sie mit der Eingabe des Namens des Workfront-Felds, das Sie zuordnen möchten. [!DNL Workfront DAM], und wählen Sie es aus, wenn Sie es in der Liste sehen.
1. Im **[!UICONTROL Zielfeld für Zuordnung auswählen]**, wählen Sie die [!DNL Workfront DAM] -Feld, das mit den Informationen in der ausgewählten [!DNL Workfront] -Feld.

   >[!NOTE]
   >
   > Alle Dokumente an [!DNL Workfront DAM] von Benutzern, die über entsprechende Berechtigungen verfügen, deren Metadaten mit der [!DNL Workfront] Felder, die hier zugeordnet sind, wenn sie [!DNL Workfront DAM].

1. Klicken **[!UICONTROL Zuordnung hinzufügen]**.

1. Weitere Informationen hinzufügen [!UICONTROL Workfront] Felder und entsprechende [!DNL Workfront DAM] -Felder.

### Zugeordnete Felder löschen

1. Klicken Sie auf **[!UICONTROL Hauptmenü]** icon ![](assets/main-menu-icon.png) in der oberen rechten Ecke von [!DNL Adobe Workfront]Klicken Sie auf **[!UICONTROL Einrichtung]** ![](assets/gear-icon-settings.png).

1. Erweitern **[!UICONTROL Dokumente]** Klicken Sie auf **[!UICONTROL Metadatenzuordnung]**.

1. Wählen Sie in der Feldliste eines der Felder aus, die Sie aus der Metadaten-Zuordnung entfernen möchten.
1. Klicken **[!UICONTROL Löschen]**.

   Die Felder werden aus der Metadatenzuordnung entfernt und die darin enthaltenen Informationen werden nicht an [!DNL Workfront DAM] mit den hochgeladenen Dokumenten.
