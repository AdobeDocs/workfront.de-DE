---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Legacy-Connector deinstallieren
description: text
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: 4b3834bf-2e6d-4588-8d77-671e14390115
source-git-commit: 3a1bc4a56cba2fe224a1f0a21c8882c2d9d030de
workflow-type: tm+mt
source-wordcount: '425'
ht-degree: 0%

---

# Deinstallieren des Legacy-Connectors von Workfront mit Adobe Experience Manager

Sie müssen den alten Connector Workfront mit Adobe Experience Manager deinstallieren und die neueste native Integration nutzen, die Workfront und Adobe Experience Manager Assets as a Cloud Service verbindet.

## Abmeldung von Workfront

1. Öffnen Sie Adobe Experience Manager.
1. Navigieren Sie in Experience Manager zu &quot;**Tools**&quot;> &quot;**Cloud Service**&quot;> &quot;**Workfront-Integrationskonfiguration**&quot;.
1. Wählen Sie Ihre Konfiguration aus (standardmäßig global-workfront) und klicken Sie auf **Eigenschaften**.
   ![Abmeldung von der Arbeitsfläche](assets/unsubscribe-from-workfront.png)
1. Deaktivieren Sie die Synchronisierung von Dokumenten, Kommentaren und Metadaten. Der Titel sollte Tag Deaktiviert sein.
Dadurch werden die Abonnements in Workfront entfernt und der Benutzer kann ein neues Abonnement mit derselben URL erstellen, die in Day CQ Link Externalizer definiert ist.

## Löschen der Workfront-Integrationskonfiguration

Nach dem Entfernen des Abonnements ist es jetzt sicher, die Workfront-Integrationskonfiguration zu löschen.

1. Öffnen Sie die Konfiguration und wählen Sie **Löschen** aus.
   ![Konfiguration löschen](assets/delete-wf-configuration.png)

## Zuordnung löschen

Als Nächstes müssen Sie die Workfront-Eigenschaftenzuordnung löschen.

1. Navigieren Sie im Experience Manager zu **Tools** > **Assets** > **Workfront-Eigenschaftenzuordnung**.

1. Wählen Sie alle Zuordnungen aus und klicken Sie auf **Löschen**.

## Benutzerberechtigungen

Alle Benutzer, die über Workfront auf AEM DAM zugreifen, erhielten Leseberechtigungen für `/content/dam`. Wenn ein Benutzer das nicht mehr benötigt, können Sie die diesen Benutzern erteilten Berechtigungen entfernen.

Der Connector funktioniert mit dem Workfront-Service des Systembenutzers. Diese wird bei der Deinstallation des Connectors deinstalliert.

>[!NOTE]
>
>Wenn Sie die Connector-Version 2.0.3 verwenden und die Gruppe `workfront-aem-connector-group` hinzugefügt haben, muss dies ebenfalls entfernt werden, indem Sie zu **Tools** > **Sicherheit** > **Gruppen** navigieren.

## Day CQ Link Externalizer

Wenn Sie den Day CQ Link Externalizer nicht benötigen, können Sie diesen auf &quot;`localhost:4502`&quot;zurücksetzen, indem Sie zu &quot;`/system/console/configMgr`&quot;gehen und nach &quot;Day CQ Link Externalizer&quot;suchen.

>[!NOTE]
>
>Wenn Sie Adobe Experience Manager as a Cloud Service verwenden, können Sie dies ändern, indem Sie sich Ihr Projekt ansehen und die Datei &quot;_com.day.cq.commons.impl.ExternalizerImpl.xml_&quot;in &quot;_ui.apps/src/main/content/jcr_root/apps/mysite/config_&quot;suchen.

![Day CQ Link Externalizer](assets/Day-CQ-Link-Externalizer.png)

## Connector-Paket deinstallieren

Die zum Deinstallieren des Connector-Pakets erforderlichen Schritte unterscheiden sich je nach verwendeter Adobe Experience Manager-Version.

### Adobe Experience Manager On-Premise

Wenn Sie Adobe Experience Manager On-Premise verwenden, gehen Sie zu &quot;_crx/packmgr/index.jsp_&quot;und suchen Sie nach &quot;`workfront-aem-connector.all-<version>.zip`&quot;, klicken Sie auf &quot;**Mehr**&quot;und dann auf &quot;**Deinstallieren**&quot;.

Überprüfen Sie unter &quot;`/conf`&quot;, ob alle von Workfront erstellten Dateien entfernt wurden.

### Adobe Experience Manager as a Cloud Service

Bei Adobe Experience Manager as a Cloud Service können Sie die Abhängigkeiten für den Connector aus den pom.files des Projekts entfernen.

## Firewall und Dispatcher

Vergessen Sie nicht, Ihre auf der Whitelist befindlichen Workfront-URLs zu entfernen, wenn keine Kommunikation mehr erforderlich ist. Außerdem verwendet der Connector die Header apiKey und den Benutzernamen, die auf den Dispatcher festgelegt wurden. Diese können ebenfalls entfernt werden.
