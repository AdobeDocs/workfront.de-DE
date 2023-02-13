---
title: Konfigurieren [!DNL Workfront] mit [!DNL Adobe Experience Manager] Legacy-Connector
user-type: administrator
product-area: system-administration;workfront-integrations;setup
navigation-topic: administrator-integrations
description: Als [!DNL Adobe Workfront] Administrator, können Sie [!DNL Workfront] mit Adobe Experience Manager-Assets (AEM) arbeiten und Ihrem Unternehmen eine umfassende Content-Management-Lösung für die Erstellung, Freigabe und Wartung von Assets innerhalb Ihres Workflows bieten.
author: Courtney
feature: System Setup and Administration, Workfront Integrations and Apps
role: Admin
exl-id: 024b8606-a9b7-413a-b393-8e5cdff37dd4
source-git-commit: 2f840ea68c9efb78acb4c24346c6775671ed0334
workflow-type: tm+mt
source-wordcount: '1893'
ht-degree: 0%

---

# Konfigurieren [!DNL Workfront] mit [!DNL Adobe Experience Manager] Legacy-Connector

Als [!DNL Adobe Workfront] Administrator, können Sie [!DNL Workfront] mit [!UICONTROL Adobe Experience Manager (AEM) Assets] und stellen Ihrer Organisation eine umfassende Content-Management-Lösung für die Erstellung, Freigabe und Wartung von Assets innerhalb Ihres Workflows zur Verfügung.

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Plan*</td> 
   <td>Beliebig</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Sie müssen [!DNL Workfront] Administrator. Informationen über [!DNL Workfront] Administratoren, siehe <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Gewähren eines vollen Administratorzugriffs</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren [!DNL Workfront] Administrator.

## [!DNL Workfront for AEM Assets]

Die [!DNL Workfront for AEM Assets connector] ermöglicht Ihrem Unternehmen Folgendes:

* Zusammenarbeiten und Verwalten von kreativen Inhalten durch Verknüpfen AEM Assets und Ordner mit Projekten, Aufgaben, Problemen und Anforderungen in [!DNL Workfront].

   Weitere Informationen zum Konfigurieren von Dokumentationsintegrationen mit Drittanbieteranwendungen finden Sie unter  [Dokumentintegrationen konfigurieren](../../administration-and-setup/configure-integrations/configure-document-integrations.md).

* Integrieren mit der [!DNL AEM Digital Asset Managemen]t-Repository (DAM), in dem Sie [!DNL Workfront] , um im DAM gespeicherte digitale Assets zu verwalten und freizugeben.

   Weitere Informationen zum Verknüpfen von Dokumenten und Asset-Ordnern finden Sie unter   [Verknüpfen von Dokumenten mit externen Anwendungen](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

* Kombinieren und Anwenden von Metadaten aus beiden Anwendungen auf ein Asset.
* Anzeigen eines umfassenden Kommunikationsstreams für ein Asset. Aktualisierungen und Kommentare zu einem Asset in [!DNL Workfront] oder [!UICONTROL AEM Assets] mit der anderen Anwendung synchronisiert werden, wodurch ein umfassender Verlauf der mit dem Asset gesendeten Nachrichten erstellt wird.

   Weitere Informationen zu Kommentaren finden Sie unter [!DNL Workfront], siehe [Hinzufügen von Dokumentaktualisierungen](../../documents/managing-documents/add-update-documents.md).

## Voraussetzungen für die Installation der [!DNL AEM Assets] Connector

Bevor Sie die [!DNL Workfront] Connector für [!UICONTROL AEM Assets]müssen Sie sicherstellen, dass die folgenden Voraussetzungen erfüllt sind:

* [!UICONTROL AEM Assets] installiert und konfiguriert, Version 6.5 oder neuer. Informationen zur Installation [!UICONTROL AEM Assets], siehe [[!DNL Adobe Experience Manager] Dokumentation](https://experienceleague.adobe.com/docs/experience-manager.html).
* (Bedingt) Wenn Ihre Firewall-Regeln Traffic nicht erwartungsgemäß zulassen, fügen Sie die IP-Adresse und/oder Domäne Ihres Clusters zu Ihrer Zulassungsliste hinzu. Weitere Informationen finden Sie unter [Konfigurieren der Zulassungsliste Ihrer Firewall](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

## Installieren Sie die [!DNL Workfront for AEM Assets] Connector-Paket {#install-the-workfront-for-aem-assets-connector-package}

>[!IMPORTANT]
>
>Die folgenden Anweisungen gelten für einen [!DNL Workfront with AEM Assets] Legacy-Connector, der durch die [[!DNL Workfront for Experience Manager] verbesserter Connector](../../documents/workfront-and-experience-manager-integrations/workfront-for-experience-manager-enhanced-connector/workfront-for-aem-enhanced-connector.md). Wenden Sie sich für weitere Informationen an Ihren Kundenbetreuer.

So installieren Sie die [!DNL Workfront for AEM Assets] Connector verwenden, müssen Sie den Connector als Package in AEM importieren. [!UICONTROL CRX Package Manager].

1. Laden Sie auf einer Workstation, auf der Sie bereits AEM installiert haben, die [!DNL Workfront for AEM Assets] Installationsdatei des Connectors.

   Sie können die [!DNL Workfront for AEM Assets] Connector aus Ihrem [!DNL Workfront] Vertreter.

1. Melden Sie sich mit einem Administratorkonto bei AEM an.
1. Klicken **[!UICONTROL Instrumente]** > **[!UICONTROL Implementierung]** > **[!UICONTROL Pakete]**.

   Die [!UICONTROL CRX Package Manager] geöffnet.

1. Klicken **[!UICONTROL Paket hochladen].**

1. Im [!UICONTROL Paket hochladen] -Dialogfeld, suchen Sie nach und wählen Sie die [!UICONTROL Workfront Connector] Paket, und klicken Sie dann auf **[!UICONTROL OK]**.\
   Das Paket wird im [!UICONTROL CRX Package Manager].

1. Klicken **[!UICONTROL Installieren].**

1. Im [!UICONTROL Paket] werden, ignorieren Sie die erweiterten Einstellungen und klicken Sie auf **[!UICONTROL Installieren]**.
1. (Optional) Um zu bestätigen, dass der Connector erfolgreich installiert wurde, stellen Sie sicher, dass die folgende Anweisung in der [!UICONTROL Aktivitätsprotokoll]:

   ```
   Package installed in <time>
   ```

1. Schließen Sie die [!UICONTROL CRX Package Manager].

   Der Connector ist installiert und Sie können jetzt konfigurieren [!DNL AEM Assets] zur Integration mit [!DNL Workfront].

1. Fahren Sie mit [Konfigurieren [!DNL AEM Assets] zur Integration mit [!DNL Workfront]](#configure-aem-assets-to-integrate-with-workfront).

## Konfigurieren [!DNL AEM Assets] zur Integration mit [!DNL Workfront] {#configure-aem-assets-to-integrate-with-workfront}

Importieren Sie nach der Installation des Connectors das Connector-Paket in AEM und konfigurieren Sie AEM so, dass eine Verknüpfung mit Dokumenten hergestellt wird in [!DNL Workfront].

Informationen zum Installieren des Connectors finden Sie unter  [Installieren Sie die [!DNL Workfront for AEM Assets] Connector-Paket](#install-the-workfront-for-aem-assets-connector-package).

* [Voraussetzungen](#prerequisites)
* [AEM integrieren mit [!DNL Workfront]](#integrate-aem-with-workfront)
* [Konfigurieren Sie die [!UICONTROL AEM Externalizer]](#configure-the-aem-externalizer)

### Voraussetzungen {#prerequisites}

Bevor Sie beginnen, müssen Sie Berechtigungen für den Workfront-Service aktivieren:

1. Gehen Sie AEM zu **[!UICONTROL Instrumente]**> **[!UICONTROL Sicherheit]**> **[!UICONTROL Berechtigungen]**.
1. Wählen Sie in der oberen linken Ecke **[!UICONTROL Benutzer]**&#x200B; im Dropdown-Menü und geben Sie *[!UICONTROL workfront-service]* im **[!UICONTROL Suche]**&#x200B; Feld. Wählen Sie die [!UICONTROL workfront-service] Benutzer.
1. Wählen Sie rechts im Bildschirm die Option **[!UICONTROL ACE hinzufügen]** um neue Einträge zu erstellen.
1. Im &#x200B;**[!UICONTROL Neuen Eintrag hinzufügen]**&#x200B; Fenster aktivieren Sie das Kontrollkästchen im **[!UICONTROL Pfad]**&#x200B; und wählen Sie den Ordner aus: */conf*
1. Geben Sie im Feld Berechtigungen Folgendes ein: *jcr:read*
1. Auswählen **[!UICONTROL Hinzufügen]**&#x200B; oben rechts
1. (Optional) Wiederholen Sie die Schritte, um weitere Einträge zu erstellen.

### AEM integrieren mit [!DNL Workfront] {#integrate-aem-with-workfront}

1. Melden Sie sich bei AEM Assets als Administrator an.
1. Klicken **[!UICONTROL Instrumente]** >**[!UICONTROL Cloud Services]**>**[!UICONTROL Konfiguration der Workfront-Integration]** >**[!UICONTROL Global-Workfront].**&#x200B;**&#x200B;**

1. (Bedingt) Erstellen Sie eine [!DNL Workfront] Cloud-Konfigurationsdatei.

   1. Klicken  **[!UICONTROL Erstellen]** in der oberen rechten Ecke des [!DNL Global-Workfront] Seite.
   1. Im **[!UICONTROL Workfront-URL]** -Feld die URL für Ihre [!DNL Workfront] -Instanz.

      Beispiel: [!DNL https]://`<account>`.my.workfront.com, wobei `<account>` ist das Konto, das Sie für Integrationen mit AEM verwenden.

   1. Im &#x200B;**[!UICONTROL Basisordner]** ein Feld, aktivieren Sie das Kontrollkästchen und wählen Sie dann im Dropdown-Menü den Pfad aus, zu dem die Dokumente gehören [!DNL Workfront] -Objekte gespeichert werden.
   1. Führen Sie im angezeigten AEM-Modal den Pfad zum Ordner mit den Dokumenten aus, mit denen eine Verbindung besteht. [!DNL Workfront] Objekte. Wählen Sie den Ordner aus und drücken Sie die Eingabetaste **[!UICONTROL Auswählen]**&#x200B; oben rechts.

      Sie können einen beliebigen Ordner unter dem Stammordner /content/dam/ verknüpfen.

   1. Im **[!UICONTROL Workfront API-Schlüssel]** und geben Sie Ihre [!UICONTROL Workfront] API-Schlüssel.

      So rufen Sie Ihre [!DNL Workfront] API-Schlüssel:

      1. Öffnen Sie eine Browser-Registerkarte und melden Sie sich bei Ihrem [!DNL Workfront] als [!DNL Workfront] Administrator.
      1. Klicken Sie auf **[!UICONTROL Hauptmenü]** icon ![](assets/main-menu-icon.png) in der oberen rechten Ecke von [!DNL Adobe Workfront]Klicken Sie auf **[!UICONTROL Einrichtung]** ![](assets/gear-icon-settings.png).

      1. Klicken **[!UICONTROL System]** >**[!UICONTROL Kundeninformationen]**.

         Wenn Sie bereits einen API-Schlüssel generiert haben, [!DNL Workfront] Der API-Schlüssel wird unter der Bezeichnung API-Schlüssel Ihres Benutzers angezeigt.

      1. (Bedingt) Wenn Sie noch keinen API-Schlüssel generiert haben, müssen Sie einen generieren:

         1. Im **[!UICONTROL API-Schlüsseleinstellungen]** sicherstellen, dass die **[!UICONTROL Nach der Erstellung laufen API-Schlüssel ab in]** auf &quot;Ohne&quot;eingestellt ist.

            Wenn Sie einen Ablaufzeitraum auswählen, funktioniert der Connector nach Ablauf des API-Schlüssels nicht mehr. Anschließend müssen Sie einen API-Schlüssel neu generieren und Ihre [!DNL Workfront] Konfiguration.

         1. Unter dem **[!UICONTROL API-Schlüssel Ihres Benutzers]** label, klicken Sie auf **[!UICONTROL API-Schlüssel generieren]**.

            Ein API-Schlüssel für [!DNL Workfront] generiert und zeigt an.
      1. Kopieren Sie den API-Schlüssel in die Zwischenablage.
      1. Öffnen Sie die Browserregisterkarte für AEM Connector und im **[!DNL Workfront API Key]** den kopierten API-Schlüssel einfügen.
   1. (Bedingt) Klicken Sie auf die **[!UICONTROL Erweitert]** in der linken oberen Ecke des [!UICONTROL [!DNL Workfront] Integrationskonfiguration] und wählen Sie gegebenenfalls die folgenden Optionen aus:

      **[!UICONTROL Durchsuchen von Sammlungen zulassen]:**&#x200B; Wählen Sie diese Option aus, wenn Ihr Unternehmen [!DNL Workfront] Benutzer, die AEM Assets-Sammlungen mit [!DNL Workfront] Objekte.

      **[!UICONTROL User Federated ID]:** Wählen Sie diese Option aus, wenn Ihr Unternehmen bei der Anmeldung bei Workfront Federated IDs oder Single Sign-On (SSO) verwendet.

      **[!UICONTROL E-Mail-Domäne ignorieren]:** Wählen Sie diese Option aus, wenn Ihre AEM-Benutzer den Domänennamen in ihrer Benutzer-ID nicht verwenden.

      **[!UICONTROL Zugriff beschränken]:** Wählen Sie diese Option aus, um die entsprechende [!DNL Workfront] IP-Adressen, die der Zulassungsliste hinzugefügt werden müssen. Weitere Informationen zur Zulassungsliste finden Sie unter [Konfigurieren der Zulassungsliste Ihrer Firewall](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

   1. Klicken Sie auf **[!UICONTROL Allgemein]** Registerkarte oben links auf der Seite &quot;Workfront-Integrationskonfiguration&quot;und klicken Sie auf **[!UICONTROL Verbinden]**.

      >[!NOTE]
      >
      >Änderungen können einige Zeit in Anspruch nehmen. Das Neustart des Bundles kann den Prozess beschleunigen.



1. (Bedingt) Wenn Sie bereits eine [!DNL Workfront] Cloud-Konfigurationsdatei, wählen Sie **[!UICONTROL Global-[!DNL Workfront]]** und klicken Sie dann oben links auf **[!UICONTROL Eigenschaften]**.

1. Generieren Sie den AEM API-Schlüssel durch Klicken auf **[!UICONTROL Generate Key],** Kopieren Sie dann den AEM-API-Schlüssel in die Zwischenablage.

   Sie benötigen den AEM API-Schlüssel später bei der Konfiguration [!UICONTROL Workfront] zur Integration mit [!UICONTROL AEM Assets]. Weitere Informationen finden Sie unter [Konfigurieren von Workfront zur Integration mit AEM Assets](#configure-workfront-to-integrate-with-aem-assets).

1. Klicken Sie oben rechts auf **[!UICONTROL Speichern]**.

   Die [!UICONTROL Global-[!DNL Workfront]] angezeigt.

   ![properties.png](assets/properties-350x117.png)

1. (Optional) Synchronisieren der bidirektionalen Kommunikation zwischen AEM und [!DNL Workfront].

   1. Klicken **[!UICONTROL Global-[!DNL Workfront]].**
   1. Klicken Sie in der linken oberen Ecke des Fensters auf **[!UICONTROL Eigenschaften]**.

      Die [!UICONTROL [!DNL Workfront] Integrationskonfiguration] angezeigt.

      ![properties2.png](assets/properties2-350x444.png)

   1. (Optional) Um die Synchronisierung von Kommentaren zwischen [!UICONTROL AEM Assets] und [!DNL Workfront]klicken **[!UICONTROL Kommentarsynchronisierung aktivieren]**.

      >[!IMPORTANT]
      >
      >Sie müssen [!UICONTROL Dokumentensynchronisierung] , um die Assets zu synchronisieren.

   1. (Optional) Um die Kommentarsynchronisierung zu deaktivieren, klicken Sie auf **[!UICONTROL Kommentarsynchronisierung deaktivieren].**

      Oder

      Löschen Sie die [!UICONTROL NOTE CREATE] Ereignisabonnement, das bei Ihrer AEM-Instanz registriert ist.

      Informationen zu Ereignisanmeldungen finden Sie unter [Ereignisabonnement-API](../../wf-api/general/event-subs-api.md).

1. Fahren Sie mit [Konfigurieren Sie die [!UICONTROL AEM Externalizer]](#configure-the-aem-externalizer).

### Konfigurieren Sie die [!UICONTROL AEM Externalizer] {#configure-the-aem-externalizer}

Die [!UICONTROL AEM Externalizer] ermöglicht es AEM, URLs in einem Format zu übergeben, das in [!DNL Workfront]. Wenn sie nicht ordnungsgemäß konfiguriert sind, [!DNL Workfront] kann die AEM-API nicht aufrufen, und die URLs, die AEM Dokumente in Workfront verknüpfen, funktionieren nicht.

1. Klicken Sie AEM auf **[!UICONTROL Instrumente]** > **[!UICONTROL Aktivitäten]** >**[!UICONTROL Web-Konsole]**.

1. Klicken **[!UICONTROL OSGi]** Klicken Sie auf **[!UICONTROL Konfiguration]** im Dropdown-Menü.

1. Wählen Sie in der Konfigurationsliste &#x200B; aus.**[!UICONTROL Day CQ Link Externalizer].**

   Die [!UICONTROL Externalizer] angezeigt.

1. Im **[!UICONTROL Domänen]** Stellen Sie sicher, dass die in der [!UICONTROL Autor] -Feld ist der Domänenname, auf den AEM Benutzer extern zugreifen können.

   Der Domänenname im [!UICONTROL author] sollte mit der Domäne übereinstimmen, die in der URL-Zeile Ihrer AEM-Instanz aufgeführt ist.

   ![[!DNL Extenalizer].png](assets/extenalizer-350x128.png)

1. (Bedingt) Aktualisieren Sie bei Bedarf die Domäne im [!UICONTROL Autor] -Feld.
1. Klicken Sie auf **[!UICONTROL Speichern]**.

   [!UICONTROL AEM Assets] ist jetzt so konfiguriert, dass Dokumente mit [!DNL Workfront]

1. Fahren Sie mit [Konfigurieren [!DNL Workfront] zur Integration mit [!DNL AEM assets]](#configure-workfront-to-integrate-with-aem-assets).

## Konfigurieren [!DNL Workfront] zur Integration mit [!DNL AEM assets] {#configure-workfront-to-integrate-with-aem-assets}

Nach der Installation [!UICONTROL Workfront für AEM Assets] Connector (wie beschrieben in [Installieren Sie die [!UICONTROL Workfront für AEM Assets] Connector-Paket](#install-the-workfront-for-aem-assets-connector-package)) und konfigurieren [!UICONTROL AEM Assets] (gemäß [Konfigurieren[!UICONTROL  AEM Assets] zur Integration mit [!DNL Workfront]](#configure-aem-assets-to-integrate-with-workfront)), müssen Sie [!DNL Workfront] Verknüpfen von Dokumenten zwischen [!DNL Workfront] und [!DNL AEM Assets].

1. Anmelden bei [!DNL Workfront] as a [!UICONTROL Workfront] Administrator.

   >[!TIP]
   >
   >[!UICONTROL Workfront] empfiehlt, eine [!UICONTROL Workfront] Administrator, der ausschließlich Ihrer AEM-Integration gewidmet ist. Weitere Informationen zur Zuweisung der [!UICONTROL Workfront] Administrator-Zugriffsstufe für einen Benutzer, siehe [Benutzern administrativen Zugriff auf bestimmte Bereiche gewähren](../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

1. Klicken Sie auf **[!UICONTROL Hauptmenü]** icon ![](assets/main-menu-icon.png) in der oberen rechten Ecke von [!DNL Adobe Workfront]Klicken Sie auf **[!UICONTROL Einrichtung]** ![](assets/gear-icon-settings.png).

1. Klicken **[!UICONTROL Dokumente]**> **[!UICONTROL Benutzerdefinierte Integration].**

1. Klicken **[!UICONTROL Benutzerspezifische Integration hinzufügen]**.
1. Im **[!UICONTROL Name]** Geben Sie den Namen der benutzerdefinierten Integration an.

   Dies ist der Name, den Benutzer bei Verwendung der Integration in [!UICONTROL Workfront]; Sie können beispielsweise *&quot;[!DNL AEM Assets]&quot;* für den Namen.

1. Im **[!UICONTROL Basis-API-URL]** Geben Sie die URL für Ihre AEM-Instanz an.

   Die Basis-API-URL besteht aus der URL für Ihre AEM Instanz gefolgt vom Pfad: /bin/webhooks/api/

   ![mceclip3.png](assets/mceclip3-350x130.png)

1. Im **[!UICONTROL Authentifizierungstyp]** Dropdown-Menü auswählen **[!UICONTROL ApiKey].**

1. Im &#x200B;**[!UICONTROL API-Schlüssel]** den AEM API-Schlüssel, den Sie bei der Konfiguration kopiert haben, einfügen [!UICONTROL AEM Assets].
1. Klicken Sie auf **[!UICONTROL Speichern]**.
1. (Optional) Stellen Sie sicher, dass die Integration markiert ist. [!UICONTROL Aktiv].\
   ![aem_custom_integration_active.png](assets/aem-custom-integration-active-350x81.png)

   [!DNL Workfront] ist jetzt so konfiguriert, dass [!DNL AEM Assets].

   Um auf Assets in AEM zuzugreifen, muss jeder [!DNL Workfront] Benutzer, die den Connector verwenden müssen, müssen in AEM als Benutzer eingerichtet werden. Informationen zum Erstellen von Benutzern finden Sie unter  [Benutzer für die Verwendung des Connectors einrichten](#set-up-users-to-use-the-connector).

## Benutzer für die Verwendung des Connectors einrichten {#set-up-users-to-use-the-connector}

Damit Benutzer auf den Connector zugreifen können, müssen sie über ein Benutzerprofil in AEM verfügen und zu einer [!DNL Workfront] -Gruppe mit Zugriffsebenen, die Folgendes enthalten: [!UICONTROL Erstellen] und [!UICONTROL Löschen] Berechtigungen.

Weitere Informationen finden Sie unter [!DNL Workfront] Berechtigungen, siehe [Benutzerdefinierte Zugriffsebenen erstellen oder ändern](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

* [Einrichten von Benutzern in [!DNL AEM assets]](#set-up-users-in-aem-assets)

### Einrichten von Benutzern in [!DNL AEM assets] {#set-up-users-in-aem-assets}

1. Anmelden bei [!DNL AEM Assets] as a [!DNL Workfront] Administrator.
1. Klicken **[!UICONTROL Instrumente]** >**&#x200B;**&#x200B;**[!UICONTROL Sicherheit]** >**[!UICONTROL Benutzer]**.

1. (Bedingt) Wenn der Benutzer kein Benutzerprofil in AEM hat, erstellen Sie ein AEM Benutzerprofil.

   1. Klicken **[!UICONTROL Benutzer erstellen].**
   1. Geben Sie die persönlichen Daten des Benutzers ein.

      ![64NewUser.png](assets/64newuser-350x524.png)

      Das einzige erforderliche Feld ist das ID-Feld. Die AEM-ID des Benutzers muss mit der [!DNL Workfront] ID, die der [!DNL Workfront] E-Mail-Adresse.

      Wenn Sie die Option [!UICONTROL E-Mail-Domäne ignorieren] Option bei der Konfiguration der AEM zur Integration mit [!DNL Workfront], stimmt die AEM ID nicht mit der [!DNL Workfront] E-Mail-Adresse.

1. (Bedingt) Wenn der Benutzer über ein AEM Profil verfügt, öffnen Sie das AEM des Benutzers.

   1. Klicken Sie auf &#x200B;**[!UICONTROL Benutzer].**

      Die [!UICONTROL Benutzerverwaltung] angezeigt.

   1. Klicken Sie auf den Benutzer, den Sie hinzufügen möchten, und klicken Sie dann auf **[!UICONTROL Eigenschaften]**.

      Die Einstellungsseite des Benutzers wird angezeigt.

1. Klicken Sie auf **[!UICONTROL Gruppen]** Registerkarte.

   ![](assets/groupstab.png)

1. Stellen Sie sicher, dass der Benutzer zu mindestens einem [!DNL Workfront] -Gruppe mit Zugriffsebenen, die Folgendes enthalten: [!UICONTROL Erstellen] und [!UICONTROL Löschen] Berechtigungen.

   1. Um den Benutzer einer vorhandenen Gruppe hinzuzufügen, geben Sie den Gruppennamen in die **[!UICONTROL Gruppenname eingeben]** und wählen Sie dann die Gruppe aus, wenn sie im Dropdown-Menü angezeigt wird.

      Oder

      Um eine Gruppe auszuwählen, der der Benutzer angehört, wählen Sie eine Gruppe in der **[!UICONTROL Gruppen, denen dieser Benutzer angehört]** Abschnitt.

1. Klicken Sie auf **[!UICONTROL Speichern].**
