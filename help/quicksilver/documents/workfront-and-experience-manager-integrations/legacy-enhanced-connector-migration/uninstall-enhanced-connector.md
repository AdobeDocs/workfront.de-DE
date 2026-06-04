---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Deinstallieren des erweiterten Connectors von Workfront for Adobe Experience Manager
description: Sie müssen den erweiterten Connector von Workfront mit Adobe Experience Manager deinstallieren, um die neueste native Integration zu erhalten, die Workfront und Adobe Experience Manager Assets as a Cloud Service verbindet.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: c6203c71-a4c4-41ee-ac4e-57137661e5b3
TQID: https://experienceleague.adobe.com/CeCyF8zbwp4tVcxQebq0EdaJqagDyppVuCL6ilqEvJA
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 260
ht-degree: 3%

---

# Deinstallieren des erweiterten Connectors von Workfront mit Adobe Experience Manager

Sie müssen den erweiterten Connector von Workfront mit Adobe Experience Manager deinstallieren, um die neueste native Integration zu erhalten, die Workfront und Adobe Experience Manager Assets as a Cloud Service verbindet.

## Voraussetzungen

* (Optional) Setzen Sie bei Bedarf alle Änderungen zurück, die an der Workfront-Firewallkonfiguration und den AEM-Dispatcher-Einstellungen vorgenommen wurden.

## Deinstallieren des erweiterten Connectors

1. Greifen Sie auf Ihr AEM as a Cloud Service-Repository zu und klonen Sie es von Cloud Manager aus.

1. Öffnen Sie das geklonte Git-Repository in der IDE Ihrer Wahl.

1. Checken Sie die Verzweigung aus, in der der erweiterte Connector installiert ist.

1. Navigieren Sie zum folgenden Pfad und entfernen Sie die ZIP-Datei des erweiterten Connectors:

   `Path: /ui.apps/src/main/resources/<zip file will be here>`

1. Entfernen Sie die folgende Abhängigkeit aus der Datei „pom.xml“ des Stammordners des Projekts.

   ```
   <!-- Workfront Tools -->
    <dependency>
        <groupId>digital.hoodoo</groupId>
        <artifactId>workfront-tools.ui.apps</artifactId>
        <type>zip</type>
        <version>1.8.0</version>
        <scope>system</scope>
        <systemPath>${project.basedir}/ui.apps/src/main/resources/workfront-tools.ui.apps.zip</systemPath>
    </dependency>
   ```

   >[!NOTE]
   >
   >Stellen Sie sicher, dass die im obigen Code-Block referenzierte Version (d. h. 1.8.0) die Version widerspiegelt, die aus dem Code deinstalliert wird.

1. Entfernen Sie die folgende Abhängigkeit aus der Datei „pom.xml“ des Untermoduls des Projekts mit dem Namen **all**.

   ```
   <!-- Workfront Tools -->
   <embedded>
       <groupId>digital.hoodoo</groupId>
       <artifactId>workfront-tools.ui.apps</artifactId>
       <type>zip</type>
       <target>/apps/<path-to-project-install-folder>/install</target>
   </embedded>
   ```

1. Entfernen Sie das folgende eingebettete aus der Datei „pom.xml“ des Untermoduls „all“ des Projekts.

   ```
   <!-- Workfront Tools -->
   <embedded>
       <groupId>digital.hoodoo</groupId>
       <artifactId>workfront-tools.ui.apps</artifactId>
       <type>zip</type>
       <target>/apps/<path-to-project-install-folder>/install</target>
   </embedded>
   ```

1. (Bedingt) Entfernen Sie die Repository-Konfiguration aus der Datei „pom.xml“ des Stammordners des Projekts.


   ```
   <repository>
       <id>hoodoo-maven</id>
       <name>Hoodoo Repository</name>
       <url>https://gitlab.com/api/v4/projects/12715200/packages/maven</url>
   </repository>
   ```

1. (Bedingt) Entfernen Sie die Server-Konfiguration aus der settings.xml, die im folgenden Pfad ./cloudmanager/maven/settings.xml im Projektstamm vorhanden ist.“

   ```
           <server>
           <id>hoodoo-maven</id>
           <configuration>
               <httpHeaders>
                   <property>
                       <name>Deploy-Token</name>
                       <value>*********************</value>
                   </property>
               </httpHeaders>
           </configuration>
       </server>
   ```

1. Übertragen Sie die Änderungen und übertragen Sie den Code in das Cloud Manager-Repository

1. Führen Sie die Cloud Manager-Pipeline aus, um die Änderungen auf Ihrer Cloud Services-Instanz bereitzustellen
