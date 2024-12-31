---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Legacy-Connector deinstallieren
description: Text
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: 4b3834bf-2e6d-4588-8d77-671e14390115
source-git-commit: 3a1bc4a56cba2fe224a1f0a21c8882c2d9d030de
workflow-type: tm+mt
source-wordcount: '425'
ht-degree: 0%

---

# Deinstallieren des alten Connectors von Workfront mit Adobe Experience Manager

Sie müssen den Legacy-Connector von Workfront mit Adobe Experience Manager deinstallieren, um die neueste native Integration zu erhalten, die Workfront und Adobe Experience Manager Assets as a Cloud Service verbindet.

## Abo von Workfront stornieren

1. Öffnen Sie Adobe Experience Manager.
1. Wechseln Sie im Experience Manager zu **Tools** > **Cloud Service** > **Workfront-Integrationskonfiguration**.
1. Wählen Sie Ihre Konfiguration aus (standardmäßig global-workfront) und klicken Sie auf **Eigenschaften**.
   ![Abo von Workfront beenden](assets/unsubscribe-from-workfront.png)
1. Deaktivieren Sie die Synchronisierung von Dokumenten, Kommentaren und Metadaten. Der Tag der Kennzeichnung sollte deaktiviert sein.
Dadurch werden die Abonnements in Workfront entfernt und die Benutzenden können mit derselben URL, die im Day CQ Link Externalizer definiert ist, ein neues Abonnement erstellen.

## Löschen der Workfront-Integrationskonfiguration

Nachdem Sie das Abonnement entfernt haben, können Sie die Workfront-Integrationskonfiguration jetzt löschen.

1. Öffnen Sie die Konfiguration und wählen Sie **Löschen** aus.
   ![Konfiguration löschen](assets/delete-wf-configuration.png)

## Zuordnung entfernen

Als Nächstes müssen Sie die Workfront-Eigenschaftszuordnung löschen.

1. Wechseln Sie im Experience Manager zu **Tools** > **Assets** > **Workfront-Eigenschaftenzuordnung**.

1. Wählen Sie alle Zuordnungen aus und klicken Sie auf **Löschen**.

## Benutzerberechtigungen

Alle Benutzenden, die über Workfront auf AEM DAM zugreifen, erhielten Leseberechtigungen für `/content/dam`. Wenn ein Benutzer dies nicht mehr benötigt, können Sie die Berechtigungen entfernen, die diesen Benutzern erteilt wurden.

Der Connector wird mit dem Workfront-Service des Systembenutzers verwendet. Dies wird bei der Deinstallation des Connectors deinstalliert.

>[!NOTE]
>
>Wenn Sie die Connector-Version 2.0.3 verwenden und die Gruppe `workfront-aem-connector-group` hinzugefügt haben, muss dies ebenfalls entfernt werden, indem Sie zu **Tools** > **Sicherheit** > **Gruppen**.

## Day CQ Link Externalizer

Wenn Sie den Day CQ Link Externalizer nicht benötigen, können Sie diesen wieder auf `localhost:4502` zurücksetzen, indem Sie zu `/system/console/configMgr` wechseln und nach „Day CQ Link Externalizer“ suchen.

>[!NOTE]
>
>Wenn Sie Adobe Experience Manager as a Cloud Service verwenden, können Sie dies ändern, indem Sie Ihr Projekt überprüfen und die Datei _com.day.cq.commons.impl.ExternalizerImpl.xml_ in _ui.apps/src/main/content/jcr_root/apps/mysite/config_ suchen.

![Day CQ Link Externalizer](assets/Day-CQ-Link-Externalizer.png)

## Connector-Paket deinstallieren

Die zum Deinstallieren des Connector-Pakets erforderlichen Schritte hängen davon ab, welche Adobe Experience Manager-Version Sie haben.

### Adobe Experience Manager On-Premise

Wenn Sie Adobe Experience Manager On-Premise verwenden, navigieren Sie zu _crx/packmgr/index.jsp_, suchen Sie nach dem `workfront-aem-connector.all-<version>.zip`, klicken Sie auf **Mehr** und dann auf **Deinstallieren**.

Überprüfen Sie unter `/conf` , ob alle von Workfront erstellten Dateien entfernt wurden.

### Adobe Experience Manager as a Cloud Service

Für Adobe Experience Manager as a Cloud Service können Sie die Abhängigkeiten für den Connector aus den pom.files des Projekts entfernen.

## Firewall und Dispatcher

Vergessen Sie nicht, Ihre Workfront-URLs auf der Zulassungsliste zu entfernen, wenn keine Kommunikation mehr erforderlich ist. Außerdem verwendet der Connector den Kopfzeilen-API-Schlüssel und den Benutzernamen, der für den Dispatcher festgelegt wurde. Diese können ebenfalls entfernt werden.
