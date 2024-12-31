---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Migrieren von verknüpften Ordnern und Dokumenten
description: Sie können die -API verwenden, um verknüpfte Ordner und Dokumente nach Adobe Experience Manager Assets zu migrieren.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: 586ab0a8-52ee-4aba-9298-af5a304acb02
source-git-commit: aad8f4648a57c93047a1a691d5e608c327d78c1b
workflow-type: tm+mt
source-wordcount: '918'
ht-degree: 0%

---

# Migrieren von verknüpften Ordnern und Dokumenten

Sie können die -API verwenden, um verknüpfte Ordner und Dokumente nach Adobe Experience Manager Assets zu migrieren.

## Verfahren

1. Identifizieren Sie alle Dokumente und Ordner, die mit dem vorherigen externen Dokumentenspeicheranbieter verknüpft sind, und notieren Sie ihre internen Dokument- oder Ordnerkennungen in Workfront sowie die Ordner-ID aller enthaltenen Ordner.

   >[!NOTE]
   >
   > Sie sollten nach allen gefundenen Ordnern oder Dokumenten suchen, um sicherzustellen, dass noch kein Link für sie mit dem neuen Anbieter erstellt wurde.

1. Suchen Sie die Dokumente und Ordner im neuen Repository nach dem Pfad und suchen Sie dann im externen System nach ihrer Identität.

1. Erstellen Sie eine Zuordnung der internen Workfront-ID zur ID im neuen externen Store. Sie benötigen dies, um im folgenden Schritt einen neuen Link zu erstellen.

1. Erstellen Sie einen neuen Link für ein Dokument oder einen Dokumentordner in Workfront, der über die neue externe ID auf die Ressource an deren neuem Speicherort verweist.

   1. **Dokumente**: Eine neue Version des vorhandenen Dokuments mit dem neuen externen Dokumentanbieter hinzufügen.
   1. **Ordner**: Erstellen Sie einen neuen Ordner an derselben Stelle mit demselben Namen.

>[!CAUTION]
>
>   Löschen Sie nicht die vorhandenen verknüpften Ordner. Dies kann zu Datenverlust führen. Um alte Ordnerlinks aus dem Workfront-Programm zu entfernen, deaktivieren Sie die benutzerdefinierte Dokumentintegration im Bereich Setup .


## Beispielprozess zum Migrieren von Links

![vereinfachter Link-Fluss](assets/links-flow-simplified.png)

## API-Informationen

Weitere Informationen zu den Workfront-APIs finden Sie in diesem Abschnitt unter [Entwicklerdokumentation:Dokumente](https://developer.workfront.com/documents.html).

### Alle Dokumente suchen

Alle **Dokumente (DOCU)** verknüpft mit **Dokumentanbieter** von **providerType** mit **documentProviderID**.

```
Http Method: GET
 
Http Endpoint: {host}/attask/api/v14.0/document/search?fields=currentVersion:*&currentVersion:externalIntegrationType={providerType}
```

[API-DOKUMENTE-Referenz](https://developer.workfront.com/documents.html#get-/docu/search)

### Alle Ordner suchen

Alle **Dokumentenordner (DOCFDR),** mit dem Dokumentanbieter (**) verknüpft**, **documentProviderID**.

```
Http Method: GET
 
Http Endpoint: {host}/attask/api/v14.0/documentFolder/search?fields=*,linkedFolder:*&linkedFolder:externalIntegrationType={providerType}
```

API-Dokumente: (Endpunkte für Dokumentenordner werden derzeit nicht unter developer.workfront.com behandelt)

### Dokumente verknüpfen

Verknüpfung **Dokumente (DOCU)** von **Externer Dokumentanbieter** von **providerType** mit **documentProviderID**.

>[!IMPORTANT]
>
>Dokumente werden vorübergehend gespeichert. Das heißt, Sie haben Zugriff auf alle Versionen des Dokuments. Wenn Sie den Link erstellen, können Sie die vorhandene Dokument-ID angeben, sodass Sie einfach eine neue Version in dieses Dokument schreiben, wobei die Daten extern im neuen Anbieter gehostet werden. Diese Dokument-ID ist mit der Dokument-ID identisch, die in dem Dokument-Link gefunden wurde, den Sie ersetzen. Es ist dasselbe konzeptionelle Dokument. Sie geben einfach an, dass die Bytes für diese neue Version bei einem anderen Anbieter gespeichert werden.

```
Http Method: POST
 
Endpoint: {host}/internal/documents/linkExternalObjects
 
Http Body:
refObjCode=DOCU&refObjID={documentId}&providerType={providerType}&documentProviderID={documentProviderID}
```

API-Dokumente: (Endpunkte für interne Links werden derzeit nicht unter developer.workfront.com behandelt)

### Ordner verknüpfen

Verknüpfung **Dokumentordner (DOCFDR** von **Externer Dokumentanbieter** von **providerType** mit **documentProviderID**.

>[!IMPORTANT]
>
>Bei Ordnerlinks benötigen Sie anders als bei Dokumentlinks die „documentFolderId“ des Ordners in Workfront, in dem Sie Ihren neuen Link platzieren möchten. Dies ist höchstwahrscheinlich derselbe übergeordnete Ordner wie der verknüpfte Ordner, den wir kopieren.

>[!CAUTION]
>
>Ordner werden nicht temporär gespeichert. Löschen Sie nicht die alten Ordner. Deaktivieren Sie die Integration benutzerdefinierter Dokumente im Bereich Setup , um alte Ordner zu entfernen.


```
Http Method: POST
 
Endpoint: {host}/internal/document/version/linkExternal
 
Http Body:
providerType={providerType}&documentProviderID={documentProviderID}&breadcrumb=[]&linkAction=LINKEXTERNAL&refObjCode={USER|PROJECT_TASK|TEMPLATE_TASK|securityRootObjectCode}&refObjID={userID|taskID|templateTaskID|securityRootId}&destFolderID={parentFolderId}
```

API-Dokumente: (Endpunkte für interne Links werden derzeit nicht unter developer.workfront.com behandelt)

## Wichtige Begriffe

* **Dokument**: Ein digitales Asset in Workfront

* **Dokumentenordner**: Ein Container für digitale Assets in Workfront

* **Dokument-ID**: Interne Workfront-ID für ein digitales Asset

* **Dokumentordner-ID**: Interne Workfront-ID für einen Ordner für digitale Assets

* **Dokumentanbieter-ID**: ID, die bestimmten Dokumentanbietern zugeordnet ist

>[!IMPORTANT]
>
> Für jeden Dokumentanbietertyp kann ein Kunde über mehrere verbundene Instanzen verfügen. Sie können beispielsweise mehrere AEM-Repositorys verknüpft haben. Oder mehrere Google Drive-Instanzen verknüpft. Die Dokumentanbieter-ID gibt die spezifische Instanz des Verbindungstyps an, den wir ersetzen oder zu dem wir wechseln möchten.

* **Document Storage Provider Type (auch „External Integration Type„)**: Der Integrationstyp des Document Storage Providers, den Workfront unterstützt. Entweder über eine dedizierte Integration oder eine „benutzerdefinierte Integration“.

* **Aktuelle Typen von Dokumentspeicheranbietern ( providerType)**:

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

* **Verknüpftes Dokument**: Ein digitales Asset, das in einem externen Dokumentspeicheranbieter gehostet wird. Workfront verfügt über eine eigene interne „Dokument-ID“ für das Asset, die Bytes werden jedoch extern gespeichert. Um dies zu erleichtern, speichert Workfront auch eine „externe Dokument-ID“, um die Suche nach der extern referenzierten Ressource innerhalb des Remote-Repositorys oder -Speichers zu erleichtern.

* **Verknüpfter Dokumentordner**: Ein Container für digitale Assets, der in einem externen Dokumentspeicheranbieter gehostet wird. Workfront verfügt für das Asset über eine eigene interne „Dokumentenordner-ID“, die Bytes werden jedoch extern gespeichert. Um dies zu erleichtern, speichert Workfront auch eine „externe Dokument-ID“, um die Suche nach der extern referenzierten Ressource innerhalb des Remote-Repositorys oder -Speichers zu erleichtern.

* **ID des externen**: ID, die zugewiesen wird, wenn Assets außerhalb von Workfront gespeichert werden. Workfront ordnet seine interne Kennung der Kennung zu, die zum Auffinden des Assets im externen System verwendet wird, und zwar über dieses Feld „Kennung des externen Dokuments“. Daher muss beim Verknüpfen des Dokuments oder Ordners aus einem neuen externen Speicher eine neue externe Dokumentkennung in dem entsprechenden Format erstellt werden, damit der externe Dokumentanbieter das Dokument in dem neuen Repository oder Speicher identifizieren kann.

  >[!NOTE]
  >
  > Workfront verfügt noch nicht über einen Standard für externe Dokumentkennungen. Für AEM-IDs wird eine neue Spezifikation verwendet. Für andere IDs kann die ID des externen Dokuments jedoch je nach Anbietertyp unterschiedliche Formen annehmen.


* **Objekttyp**: Dies ist ein API-Begriff für die Zwecke dieses Dokuments. Es handelt sich um ein generisches Objekt in Workfront, mit dem Sie interagieren möchten. In diesem Fall interagieren Sie mit Dokumenten und Ordnern, die die Typen „DOCU“ bzw. „DOCDR“ aufweisen.

* **Objekt-ID**: Die interne Workfront-Kennung für das generische Objekt, mit dem Sie interagieren möchten. Sie interagieren mit Dokumenten und Ordnern, sodass dies entweder die Dokument-ID oder die Dokument-Ordner-ID ist.
