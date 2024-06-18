---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Verknüpfte Ordner und Dokumente migrieren
description: Sie können die API verwenden, um verknüpfte Ordner und Dokumente nach Adobe Experience Manager Assets zu migrieren.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: 586ab0a8-52ee-4aba-9298-af5a304acb02
source-git-commit: aad8f4648a57c93047a1a691d5e608c327d78c1b
workflow-type: tm+mt
source-wordcount: '918'
ht-degree: 0%

---

# Verknüpfte Ordner und Dokumente migrieren

Sie können die API verwenden, um verknüpfte Ordner und Dokumente nach Adobe Experience Manager Assets zu migrieren.

## Verfahren

1. Identifizieren Sie alle Dokumente und Ordner, die mit dem vorherigen externen Dokumentenspeicher verknüpft sind, unter Angabe der internen Workfront-Dokument- oder -Ordnerkennungen sowie der Ordner-ID aller Ordner, die diesen Ordner enthalten.

   >[!NOTE]
   >
   > Sie sollten nach allen gefundenen Ordnern oder Dokumenten suchen, um sicherzustellen, dass sie noch keinen Link mit dem neuen Anbieter erstellt haben.

1. Suchen Sie die Dokumente und Ordner im neuen Repository nach Pfad und suchen Sie dann ihre Identität im externen System.

1. Erstellen Sie eine Zuordnung der internen Workfront ID zur ID im neuen externen Speicher. Sie benötigen dies, um im folgenden Schritt einen neuen Link zu erstellen.

1. Erstellen Sie in Workfront einen neuen Dokument- oder Dokumentordnerlink, der über die neue externe ID auf die Ressource am neuen Speicherort verweist.

   1. **Dokumente**: Fügen Sie mit dem neuen externen Dokumentenanbieter eine neue Version des vorhandenen Dokuments hinzu.
   1. **Ordner**: Erstellen Sie einen neuen Ordner an derselben Stelle mit demselben Namen.

>[!CAUTION]
>
>   Löschen Sie nicht die vorhandenen verknüpften Ordner. Dies kann zu Datenverlust führen. Um alte Ordnerlinks aus der Workfront-Anwendung zu entfernen, deaktivieren Sie die benutzerdefinierte Dokumentenintegration im Bereich Einrichtung .


## Beispielprozess für die Migration von Links

![simple-link-flow](assets/links-flow-simplified.png)

## API-Informationen

Weitere Informationen zu den Workfront-APIs finden Sie in diesem Abschnitt [Entwicklerdokumentation:Dokumente](https://developer.workfront.com/documents.html).

### Alle Dokumente suchen

Alle suchen **Dokumente (DOCU)** Verknüpfung zu **Document Provider** von **providerType** mit **documentProviderID**.

```
Http Method: GET
 
Http Endpoint: {host}/attask/api/v14.0/document/search?fields=currentVersion:*&currentVersion:externalIntegrationType={providerType}
```

[API-DOCS-Referenz](https://developer.workfront.com/documents.html#get-/docu/search)

### Suchen aller Ordner

Alle suchen **Dokumentenordner (DOCFDR)** Verknüpfung mit Document Provider von **providerType** mit **documentProviderID**.

```
Http Method: GET
 
Http Endpoint: {host}/attask/api/v14.0/documentFolder/search?fields=*,linkedFolder:*&linkedFolder:externalIntegrationType={providerType}
```

API-DOCS: (Document Folder Endpoints, die derzeit nicht unter developer.workfront.com abgedeckt sind)

### Verknüpfen von Dokumenten

Link **Dokumente (DOCU)** von **Externer Dokumentanbieter** von **providerType** mit **documentProviderID**.

>[!IMPORTANT]
>
>Dokumente werden vorübergehend gespeichert. Das bedeutet, Sie haben Zugriff auf alle Versionen des Dokuments. Beim Erstellen des Links können Sie die vorhandene Dokument-ID angeben, sodass Sie einfach eine neue Version in dieses Dokument schreiben, wobei die Daten extern im neuen Anbieter gehostet werden. Diese Dokument-ID entspricht der Dokument-ID, die auf dem Dokumentlink gefunden wird, den Sie ersetzen. Es ist dasselbe konzeptionelle Dokument. Sie geben einfach an, dass die Bytes für diese neue Version bei einem anderen Anbieter gespeichert werden.

```
Http Method: POST
 
Endpoint: {host}/internal/documents/linkExternalObjects
 
Http Body:
refObjCode=DOCU&refObjID={documentId}&providerType={providerType}&documentProviderID={documentProviderID}
```

API-DOCS: (Interne Link-Endpunkte, die derzeit nicht unter developer.workfront.com abgedeckt sind)

### Verknüpfungsordner

Link **Dokumentenordner (DOCFDR)** von **Externer Dokumentanbieter** von **providerType** mit **documentProviderID**.

>[!IMPORTANT]
>
>Für Ordnerlinks benötigen Sie im Gegensatz zu Document-Links die &#39;documentFolderId&#39; des Ordners in Workfront, in den Sie den neuen Link platzieren möchten. Dies ist wahrscheinlich derselbe übergeordnete Ordner wie der verknüpfte Ordner, den wir kopieren.

>[!CAUTION]
>
>Ordner werden nicht temporär gespeichert. Löschen Sie nicht die alten Ordner. Deaktivieren Sie die benutzerdefinierte Dokumentintegration im Setup-Bereich, um alte Ordner zu entfernen.


```
Http Method: POST
 
Endpoint: {host}/internal/document/version/linkExternal
 
Http Body:
providerType={providerType}&documentProviderID={documentProviderID}&breadcrumb=[]&linkAction=LINKEXTERNAL&refObjCode={USER|PROJECT_TASK|TEMPLATE_TASK|securityRootObjectCode}&refObjID={userID|taskID|templateTaskID|securityRootId}&destFolderID={parentFolderId}
```

API-DOCS: (Interne Link-Endpunkte, die derzeit nicht unter developer.workfront.com abgedeckt sind)

## Wichtige Begriffe

* **Dokument**: Ein digitales Asset in Workfront

* **Dokumentordner**: Ein Container für digitale Assets in Workfront

* **Dokument-ID**: Interne Workfront-ID für ein digitales Asset

* **Document Folder ID**: Interne Workfront-ID für einen digitalen Asset-Ordner

* **Dokumentanbieter-ID**: Kennung, die bestimmten Dokumentenanbietern zugeordnet ist

>[!IMPORTANT]
>
> Für jeden Dokumentanbietertyp kann ein Kunde über mehrere verbundene Instanzen verfügen. Sie können beispielsweise mehrere AEM Repositorys verknüpfen. Oder mehrere verknüpfte Google Drive-Instanzen. Die Document Provider-ID gibt die spezifische Instanz des Verbindungstyps an, den wir ersetzen oder zu der wir wechseln möchten.

* **Document Storage Provider-Typ (auch &quot;External Integration Type&quot;)**: Der Typ der von Workfront unterstützten Document Storage Provider-Integration. Entweder über eine dedizierte Integration oder eine &quot;benutzerdefinierte Integration&quot;.

* **Aktuelle Document Storage Provider-Typen ( providerType)**:

  ```
  ATTASK
  BOX
  GOOGLE
  SHAREPOINT
  WEBDAM
  WORKFRONTDAM
  INFERNO
  WIDEN
  DROPBOX
  DROPBOX_BUSINESS
  ONEDRIVE
  QUIP
  WEBHOOKS
  AEM
  MOCK
  ```

* **Verknüpftes Dokument**: Ein digitales Asset, das in einem externen Dokumentenspeicheranbieter gehostet wird. Workfront verfügt über eine eigene interne &quot;Dokument-ID&quot;für das Asset, die Bytes werden jedoch extern gespeichert. Um dies zu erleichtern, speichert Workfront auch eine &quot;externe Dokument-ID&quot;, die bei der Suche nach der extern referenzierten Ressource im Remote-Repository oder -Speicher hilft.

* **Verknüpfter Dokumentordner**: Ein Container für digitale Assets, der in einem externen Dokumentenspeicheranbieter gehostet wird. Workfront verfügt über eine eigene interne &quot;Dokumentordner-ID&quot;für das Asset, die Bytes werden jedoch extern gespeichert. Um dies zu erleichtern, speichert Workfront auch eine &quot;externe Dokument-ID&quot;, die bei der Suche nach der extern referenzierten Ressource im Remote-Repository oder -Speicher hilft.

* **Externe Dokument-ID**: ID, die zugewiesen wird, wenn Assets außerhalb von Workfront gespeichert werden. Workfront ordnet seine interne Kennung über dieses Feld &quot;Externe Dokumentkennung&quot;der Kennung zu, die zum Suchen des Assets im externen System verwendet wird. Daher muss beim Verknüpfen des Dokuments oder Ordners aus einem neuen externen Speicher eine neue externe Dokumentkennung im entsprechenden Format erstellt werden, damit der externe Dokumentanbieter das Dokument im neuen Repository oder Store identifizieren kann.

  >[!NOTE]
  >
  > Workfront verfügt noch nicht über einen Standard für externe Dokument-IDs. Für AEM IDs wird eine neue Spezifikation verwendet. Für andere IDs kann die externe Dokument-ID jedoch je nach Anbietertyp in verschiedenen Formularen verwendet werden.


* **Objekttyp**: Dies ist ein API-lediglich-Begriff für die Zwecke dieses Dokuments. Es handelt sich um eine Art generisches Objekt in Workfront, mit dem Sie interagieren möchten. In diesem Fall interagieren Sie mit Dokumenten und Ordnern mit den Typen &quot;DOCU&quot;bzw. &quot;DOCFDR&quot;.

* **Objekt-ID**: Die interne Workfront-Kennung für das generische Objekt, mit dem Sie interagieren möchten. Sie interagieren mit Dokumenten und Ordnern, sodass es sich entweder um die Dokument-ID oder um die Dokumentordner-ID handelt.
