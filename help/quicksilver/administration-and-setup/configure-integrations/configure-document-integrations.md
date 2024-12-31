---
title: Konfigurieren von Dokumentenintegrationen
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

Als [!DNL Adobe Workfront] können Sie Dokumentintegrationen konfigurieren, um Dokumente in [!UICONTROL Workfront zu verwalten]. Sie können [!UICONTROL Workfront] auch so konfigurieren, dass Dokumente nur in Document Services-Programmen und nicht in [!UICONTROL Workfront] gespeichert werden. Weitere Informationen finden Sie unter [Aktualisieren und Verknüpfen eines Dokuments von [!UICONTROL Workfront] mit einem externen Cloud-Anbieter](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md#update-and-link-a-document-from-workfront-to-an-external-cloud-provider) in [Verknüpfen von Dokumenten aus externen Programmen](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

>[!NOTE]
>
>Um eine offene Kommunikation zwischen [!DNL Workfront Proof] und den [!DNL Workfront]-Servern zu ermöglichen, müssen Sie möglicherweise bestimmte IP-Adressen zu Ihrer Zulassungsliste hinzufügen. Weitere Informationen finden Sie [Zulassungsliste zum Konfigurieren der Firewall](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

## Zugriffsanforderungen

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

  Informationen zur Integration von mit [!DNL SharePoint] finden Sie [Konfigurieren der  [!DNL SharePoint] -Integration](../../administration-and-setup/configure-integrations/configure-sharepoint-integration.md).

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

Darüber hinaus können Sie Ihr [!DNL Workfront]-Dokumenterlebnis mit DAM-Integrationen von Drittanbietern verbessern. Administratoren müssen diese Funktionen aktivieren, damit Benutzer den Dienst mit ihrem [!DNL Workfront] verknüpfen können.

## Konfigurieren von Integrationen zum Verwalten von Dokumenten

{{step-1-to-setup}}

1. Klicken Sie im linken Bedienfeld auf **[!UICONTROL Dokumente]** > **[!UICONTROL Cloud-Anbieter].**

1. (Optional) Um Dokumente in einer Document Services-Anwendung und nicht in [!DNL Workfront] zu speichern, wählen Sie **[!UICONTROL Benutzer daran hindern, Dokumente in [!DNL Workfront]] zu speichern.**

1. Wählen Sie die Integrationen aus, die Sie aktivieren möchten.
1. Klicken Sie auf **[!UICONTROL Speichern]**.

Wenn Sie Integrationen mit [!DNL Workfront DAM] einrichten, können Sie [!DNL Workfront] aktivieren, um Metadaten in Dokumente einzuschließen. Weitere Informationen zum Zuordnen von Metadaten finden Sie unter [Einrichten der Metadatenzuordnung](../../administration-and-setup/configure-integrations/set-up-metadata-mapping.md).

## Konfigurieren von benutzerdefinierten Dokumentintegrationen

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ***DON'T DELETE, DRAFT OR HIDE THIS SECTION IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **)</p>
-->

Eine benutzerdefinierte Dokumentenintegration ermöglicht es [!DNL Workfront] Benutzern, Dateien aus praktisch jedem System in [!DNL Workfront] zu verknüpfen, vorausgesetzt, das System ist für die Zusammenarbeit mit [!DNL Workfront] ausgelegt.

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
      <td>Der Name der benutzerdefinierten Integration. Dies ist der Name, den Benutzer sehen, wenn sie die Integration in Workfront verwenden.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Basis-API-URL] </td> 
      <td>Die HTTP-Basis- oder sichere HTTP-URL für API-Aufrufe. Beispiel: <code>https://&lt;documentprovider&gt;.com/api/v2</code></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Authentifizierungstyp]</td> 
      <td> <p>Die Authentifizierungsmethode, die bei der Durchführung autorisierter API-Aufrufe an die benutzerdefinierte Integration verwendet werden muss.</p> 
       <ul> 
        <li>Wenn Sie <strong>[!UICONTROL OAuth]</strong> auswählen, fahren Sie mit Schritt 5 fort.</li> 
        <li>Wenn Sie <strong>[!UICONTROL APIkey]</strong> auswählen, fahren Sie mit Schritt 6 fort.</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Bedingt) Wenn Sie **[!UICONTROL OAuth]**-Authentifizierung für **[!UICONTROL Authentifizierungstyp]** ausgewählt haben, geben Sie die folgenden Informationen ein:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL-Authentifizierungs-URL]</td> 
      <td>Die für die Benutzerauthentifizierung verwendete vollständige URL. [!DNL Workfront] navigiert Benutzer im Rahmen des OAuth-Bereitstellungsprozesses zu dieser Adresse.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Token-Endpunkt-URL]</td> 
      <td>Die zum Abruf von OAuth-Token verwendete vollständige API-URL.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Client-ID]</td> 
      <td>Die OAuth-Client-ID für diese Integration.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Client-Geheimnis]</td> 
      <td>Das OAuth-Client-Geheimnis für diese Integration.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Anforderungsparameter]</td> 
      <td> <p>Geben Sie optionale Werte ein, die an die Abfragezeichenfolge jedes API-Aufrufs angehängt werden sollen. Beispiel: access_type=offline.</p> <p>Um mehrere Anfrageparameter hinzuzufügen, klicken Sie auf <strong>+Anfrageparameter hinzufügen</strong>.</p> </td> 
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
Weitere Informationen zu berechneten benutzerdefinierten Feldern finden Sie unter [Hinzufügen berechneter Felder zu einem Formular](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md).

Die Zuordnung wirkt sich auf alle Dokumente aus, die von einem Benutzer von [!DNL Workfront] in das [!UICONTROL Workfront] DAM hochgeladen werden.

Als [!DNL Workfront] müssen Sie [!DNL Workfront DAM] in Workfront aktivieren, bevor Sie die Felder für den Metadatenzuordnungsprozess zuordnen können.

So konfigurieren Sie [!DNL Workfront] zum Senden von Metadaten an [!DNL Workfront DAM]:

{{step-1-to-setup}}

1. Klicken Sie **[!UICONTROL Dokumente]** > **[!UICONTROL Metadatenzuordnung]**.

1. Beginnen Sie im Feld **[!UICONTROL Source-Feld für Zuordnung auswählen]** mit der Eingabe des Namens des Workfront-Felds, dem Sie [!DNL Workfront DAM] zuordnen möchten, und wählen Sie es aus, wenn Sie es in der Liste sehen.
1. Wählen **[!UICONTROL im Feld Zielfeld für Zuordnung auswählen]** das [!DNL Workfront DAM] Feld aus, das Sie mit den Informationen im ausgewählten [!DNL Workfront] füllen möchten.

   >[!NOTE]
   >
   > Bei allen Dokumenten, die von dazu berechtigten Benutzenden an [!DNL Workfront DAM] gesendet werden, werden die Metadaten dieser Dokumente mit den [!DNL Workfront] hier zugeordneten Feldern aktualisiert, wenn sie in [!DNL Workfront DAM] hochgeladen werden.

1. Klicken Sie **[!UICONTROL Zuordnung hinzufügen]**.

1. Fügen Sie weitere [!UICONTROL Workfront]-Felder und entsprechende [!DNL Workfront DAM] hinzu.

### Zugeordnete Felder löschen

{{step-1-to-setup}}

1. Erweitern Sie **[!UICONTROL Dokumente]** und klicken Sie dann auf **[!UICONTROL Metadatenzuordnung]**.

1. Wählen Sie in der Liste der Felder eines der Felder aus, die Sie aus der Metadatenzuordnung entfernen möchten.
1. Klicken Sie **[!UICONTROL Löschen]**.

   Die Felder werden aus der Metadatenzuordnung entfernt und die darin enthaltenen Informationen werden nicht an [!DNL Workfront DAM] mit den hochgeladenen Dokumenten übertragen.
