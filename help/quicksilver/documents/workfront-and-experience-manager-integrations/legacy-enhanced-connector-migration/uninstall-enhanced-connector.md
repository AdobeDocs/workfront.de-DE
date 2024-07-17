---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Deinstallieren des erweiterten Workfront for Adobe Experience Manager-Connectors
description: Sie müssen den erweiterten Connector Workfront mit Adobe Experience Manager deinstallieren, um die neueste native Integration zu nutzen, die Workfront und Adobe Experience Manager Assets as a Cloud Service verbindet.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: c6203c71-a4c4-41ee-ac4e-57137661e5b3
source-git-commit: 9673009f12509b5e7051ee91e142d311f333f215
workflow-type: tm+mt
source-wordcount: '261'
ht-degree: 0%

---

# Deinstallieren des erweiterten Connectors von Workfront mit Adobe Experience Manager

Sie müssen den erweiterten Connector Workfront mit Adobe Experience Manager deinstallieren, um die neueste native Integration zu nutzen, die Workfront und Adobe Experience Manager Assets as a Cloud Service verbindet.

## Voraussetzungen

* (Optional) Wiederholen Sie bei Bedarf alle Änderungen, die an der Workfront-Firewall-Konfiguration und AEM Dispatcher-Einstellungen vorgenommen wurden.

## Deinstallieren des erweiterten Connectors

1. Greifen Sie über Cloud Manager auf Ihr AEM as a Cloud Service-Repository zu und klonen Sie es.

1. Öffnen Sie Ihr geklontes Git-Repository in der IDE Ihrer Wahl.

1. Checken Sie die Verzweigung aus, in der der erweiterte Connector installiert ist.

1. Navigieren Sie zum folgenden Pfad und entfernen Sie die verbesserte ZIP-Datei des Connectors:

   `Path: /ui.apps/src/main/resources/<zip file will be here>`

1. Entfernen Sie die folgende Abhängigkeit aus der Datei &quot;pom.xml&quot;im Stammverzeichnis des Projekts.

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
   >Stellen Sie sicher, dass die im obigen Codeblock referenzierte Version, d. h. 1.8.0, die Version widerspiegelt, die aus dem Code deinstalliert wird.

1. Entfernen Sie die folgende Abhängigkeit aus der Datei &quot;pom.xml&quot;des Untermoduls des Projekts mit dem Namen **all**.

   ```
   <!-- Workfront Tools -->
   <embedded>
       <groupId>digital.hoodoo</groupId>
       <artifactId>workfront-tools.ui.apps</artifactId>
       <type>zip</type>
       <target>/apps/<path-to-project-install-folder>/install</target>
   </embedded>
   ```

1. Entfernen Sie Folgendes aus der Datei &quot;pom.xml&quot;des Untermoduls &quot;all&quot;des Projekts.

   ```
   <!-- Workfront Tools -->
   <embedded>
       <groupId>digital.hoodoo</groupId>
       <artifactId>workfront-tools.ui.apps</artifactId>
       <type>zip</type>
       <target>/apps/<path-to-project-install-folder>/install</target>
   </embedded>
   ```

1. (Bedingt) Entfernen Sie die Repository-Konfiguration aus der Datei &quot;pom.xml&quot;im Stammverzeichnis des Projekts.


   ```
   <repository>
       <id>hoodoo-maven</id>
       <name>Hoodoo Repository</name>
       <url>https://gitlab.com/api/v4/projects/12715200/packages/maven</url>
   </repository>
   ```

1. (Bedingt) Entfernen Sie die Serverkonfiguration aus der Datei settings.xml, die im folgenden Pfad vorhanden ist:/cloudmanager/maven/settings.xml im Projektstamm.&quot;

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

1. Übertragen Sie die Änderungen und den Code in das Cloud Manager-Repository.

1. Führen Sie die Cloud Manager-Pipeline aus, um die Änderungen auf Ihrer Cloud Service-Instanz bereitzustellen.
