---
title: Konfigurieren von [!DNL Workfront] mit [!DNL Adobe Experience Manager] Legacy-Connector
user-type: administrator
product-area: system-administration;workfront-integrations;setup
navigation-topic: administrator-integrations
description: Als [!DNL Adobe Workfront] Administrator können Sie [!DNL Workfront] in Adobe Experience Manager (AEM) Assets integrieren und Ihrem Unternehmen eine umfassende Inhaltsverwaltungslösung für die Erstellung, Freigabe und Wartung von Assets innerhalb Ihres Workflows bereitstellen.
author: Courtney
feature: System Setup and Administration, Workfront Integrations and Apps
role: Admin
exl-id: 024b8606-a9b7-413a-b393-8e5cdff37dd4
source-git-commit: 55c8a3e5d0041a0e975bfd979a2d2e38930fea8d
workflow-type: tm+mt
source-wordcount: '1875'
ht-degree: 0%

---

# Konfigurieren von [!DNL Workfront] mit dem älteren Connector [!DNL Adobe Experience Manager]

Als [!DNL Adobe Workfront] -Administrator können Sie [!DNL Workfront] in [!UICONTROL Adobe Experience Manager (AEM) Assets] integrieren und Ihrem Unternehmen eine umfassende Inhaltsverwaltungslösung für die Erstellung, Freigabe und Wartung von Assets innerhalb Ihres Workflows bereitstellen.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Sie müssen ein [!DNL Workfront] -Administrator sein. Weitere Informationen zu [!DNL Workfront] -Administratoren finden Sie unter <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Gewähren eines vollen Administratorzugriffs für einen Benutzer</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren [!DNL Workfront] -Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

+++

## [!DNL Workfront for AEM Assets]

Mit dem [!DNL Workfront for AEM Assets connector] kann Ihr Unternehmen Folgendes tun:

* Zusammenarbeit und Verwaltung von kreativen Inhalten durch Verknüpfen AEM Assets und Ordner mit Projekten, Aufgaben, Problemen und Anforderungen in [!DNL Workfront].

  Weitere Informationen zum Konfigurieren von Dokumentationsintegrationen mit Drittanbieteranwendungen finden Sie unter [Dokumentintegrationen konfigurieren](../../administration-and-setup/configure-integrations/configure-document-integrations.md).

* Integrieren Sie in das Repository [!DNL AEM Digital Asset Managemen]t (DAM), sodass Sie mit [!DNL Workfront] digitale Assets verwalten und freigeben können, die in DAM gespeichert sind.

  Weitere Informationen zum Verknüpfen von Dokumenten und Asset-Ordnern finden Sie unter   [Verknüpfen von Dokumenten aus externen Anwendungen](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

* Kombinieren und Anwenden von Metadaten aus beiden Anwendungen auf ein Asset.
* Anzeigen eines umfassenden Kommunikationsstreams für ein Asset. Aktualisierungen und Kommentare, die an einem Asset entweder in [!DNL Workfront] oder in [!UICONTROL AEM Assets] vorgenommen wurden, werden mit der anderen Anwendung synchronisiert, wodurch ein umfassender Verlauf der mit dem Asset gesendeten Nachrichten erstellt wird.

  Weitere Informationen zum Hinzufügen von Kommentaren in [!DNL Workfront] finden Sie unter [Hinzufügen einer Aktualisierung zu einem Dokument](../../documents/managing-documents/add-update-documents.md).

## Voraussetzungen für die Installation des [!DNL AEM Assets]-Connectors

Bevor Sie den [!DNL Workfront] -Connector für [!UICONTROL AEM Assets] installieren können, stellen Sie sicher, dass die folgenden Voraussetzungen erfüllt sind:

* [!UICONTROL AEM Assets] installiert und konfiguriert, Version 6.5 oder neuer. Informationen zur Installation von [!UICONTROL AEM Assets] finden Sie in der [[!DNL Adobe Experience Manager] Dokumentation](https://experienceleague.adobe.com/docs/experience-manager.html).
* (Bedingt) Wenn Ihre Firewall-Regeln Traffic nicht erwartungsgemäß zulassen, fügen Sie die IP-Adresse und/oder Domäne Ihres Clusters zu Ihrer Zulassungsliste hinzu. Weitere Informationen finden Sie unter [Konfigurieren der Zulassungsliste Ihrer Firewall-](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

## Installieren Sie das Connector-Paket [!DNL Workfront for AEM Assets] . {#install-the-workfront-for-aem-assets-connector-package}

>[!IMPORTANT]
>
>Die folgenden Anweisungen gelten für einen älteren Connector vom Typ [!DNL Workfront with AEM Assets] , der durch den erweiterten Connector [[!DNL Workfront for Experience Manager]  ersetzt wurde. ](../../documents/workfront-and-experience-manager-integrations/workfront-for-experience-manager-enhanced-connector/workfront-for-aem-enhanced-connector.md) Wenden Sie sich für weitere Informationen an Ihren Kundenbetreuer.

Um den Connector [!DNL Workfront for AEM Assets] zu installieren, müssen Sie den Connector mit dem [!UICONTROL CRX Package Manager] als Paket in AEM importieren.

1. Laden Sie auf einer Workstation, auf der Sie bereits AEM installiert haben, die Installationsdatei [!DNL Workfront for AEM Assets] Connector herunter.

   Sie können den [!DNL Workfront for AEM Assets]-Connector von Ihrem [!DNL Workfront]-Support-Mitarbeiter erhalten.

1. Melden Sie sich mit einem Administratorkonto bei AEM an.
1. Klicken Sie auf **[!UICONTROL Tools]** > **[!UICONTROL Bereitstellung]** > **[!UICONTROL Pakete]**.

   Der [!UICONTROL CRX Package Manager] wird geöffnet.

1. Klicken Sie auf **[!UICONTROL Paket hochladen].**

1. Suchen Sie im Dialogfeld [!UICONTROL Paket hochladen] nach dem Paket [!UICONTROL Workfront Connector] und wählen Sie es aus. Klicken Sie dann auf **[!UICONTROL OK]**.\
   Das Paket wird im [!UICONTROL CRX Package Manager] angezeigt.

1. Klicken Sie auf **[!UICONTROL Installieren].**

1. Ignorieren Sie im Dialogfeld [!UICONTROL Package] die erweiterten Einstellungen und klicken Sie auf **[!UICONTROL Installieren]**.
1. (Optional) Um zu bestätigen, dass der Connector erfolgreich installiert wurde, stellen Sie sicher, dass die folgende Anweisung im [!UICONTROL Aktivitätsprotokoll] angezeigt wird:

   ```
   Package installed in <time>
   ```

1. Schließen Sie den [!UICONTROL CRX Package Manager].

   Der Connector ist installiert und Sie können jetzt [!DNL AEM Assets] für die Integration mit [!DNL Workfront] konfigurieren.

1. Fahren Sie mit [Konfigurieren [!DNL AEM Assets] für die Integration mit [!DNL Workfront]](#configure-aem-assets-to-integrate-with-workfront) fort.

## Konfigurieren von [!DNL AEM Assets] für die Integration mit [!DNL Workfront] {#configure-aem-assets-to-integrate-with-workfront}

Importieren Sie nach der Installation des Connectors das Connector-Paket in AEM und konfigurieren Sie AEM so, dass eine Verknüpfung mit Dokumenten in [!DNL Workfront] hergestellt wird.

Informationen zum Installieren des Connectors finden Sie unter [Installieren des [!DNL Workfront for AEM Assets] Connector-Pakets](#install-the-workfront-for-aem-assets-connector-package).

* [Voraussetzungen](#prerequisites)
* [AEM mit [!DNL Workfront] integrieren](#integrate-aem-with-workfront)
* [Konfigurieren des [!UICONTROL AEM Externalizer]](#configure-the-aem-externalizer)

### Voraussetzungen {#prerequisites}

Bevor Sie beginnen, müssen Sie Berechtigungen für den Workfront-Service aktivieren:

1. Gehen Sie AEM zu **[!UICONTROL Tools]**> **[!UICONTROL Sicherheit]**> **[!UICONTROL Berechtigungen]**.
1. Wählen Sie in der oberen linken Ecke die &#x200B; **[!UICONTROL Benutzer]** aus dem Dropdown-Menü und geben Sie im &#x200B; Feld **[!UICONTROL Suche]** den Wert *[!UICONTROL workfront-service]* ein. Wählen Sie den Benutzer [!UICONTROL workfront-service] aus.
1. Wählen Sie rechts im Bildschirm **[!UICONTROL ACE hinzufügen]** aus, um neue Einträge zu erstellen.
1. Wählen Sie im &#x200B; Fenster &#x200B;**[!UICONTROL Neuen Eintrag hinzufügen]** das Kontrollkästchen im &#x200B; Feld **[!UICONTROL Pfad]** aus und wählen Sie den Ordner: */conf*
1. Geben Sie im Feld Berechtigungen Folgendes ein: *jcr:read*
1. Wählen Sie oben rechts die &#x200B; **[!UICONTROL Hinzufügen]** aus.
1. (Optional) Wiederholen Sie die Schritte, um weitere Einträge zu erstellen.

### AEM mit [!DNL Workfront] integrieren {#integrate-aem-with-workfront}

1. Melden Sie sich bei AEM Assets als Administrator an.
1. Klicken Sie auf **[!UICONTROL Tools]** >**[!UICONTROL Cloud Service]**>**[!UICONTROL Workfront-Integrationskonfiguration]** >**[!UICONTROL Global-Workfront].** &#x200B;**&#x200B;**

1. (Bedingt) Wenn Sie dies noch nicht getan haben, erstellen Sie eine [!DNL Workfront] Cloud-Konfigurationsdatei.

   1. Klicken Sie oben rechts auf der Seite [!DNL Global-Workfront] auf **[!UICONTROL Erstellen]** .
   1. Geben Sie im Feld **[!UICONTROL Workfront URL]** die URL für Ihre [!DNL Workfront] -Instanz an.

      Beispiel: [!DNL https]://`<account>`.my.workfront.com, wobei `<account>` das Konto ist, das Sie für Integrationen mit AEM verwenden.

   1. Aktivieren Sie im Feld &#x200B;**[!UICONTROL Basisordner]** das Kontrollkästchen und wählen Sie dann im Dropdown-Menü den Pfad aus, in dem Dokumente gespeichert werden, die mit [!DNL Workfront] -Objekten verknüpft sind.
   1. Im angezeigten AEM-Modal folgen Sie dem Pfad zum Ordner mit den Dokumenten, die mit [!DNL Workfront] -Objekten verbunden sind. Wählen Sie den Ordner aus und drücken Sie die &#x200B; **[!UICONTROL Auswählen]** oben rechts.

      Sie können einen beliebigen Ordner unter dem Stammordner /content/dam/ verknüpfen.

   1. Geben Sie im Feld **[!UICONTROL Workfront-API-Schlüssel]** Ihren [!UICONTROL Workfront]-API-Schlüssel an.

      So rufen Sie Ihren [!DNL Workfront] -API-Schlüssel ab:

      1. Öffnen Sie eine Browser-Registerkarte und melden Sie sich als [!DNL Workfront] -Administrator bei Ihrem [!DNL Workfront] -Konto an.

      {{step-1-to-setup}}

      1. Klicken Sie auf **[!UICONTROL System]** >**[!UICONTROL Customer Info]**.

         Wenn Sie bereits einen API-Schlüssel generiert haben, wird Ihr [!DNL Workfront] API-Schlüssel unter der Bezeichnung API-Schlüssel Ihres Benutzers angezeigt.

      1. (Bedingt) Wenn Sie noch keinen API-Schlüssel generiert haben, müssen Sie einen generieren:

         1. Stellen Sie im Abschnitt **[!UICONTROL API-Schlüsseleinstellungen]** sicher, dass die Option **[!UICONTROL Nach der Erstellung laufen API-Schlüssel in]** auf &quot;Keine&quot;eingestellt ist.

            Wenn Sie einen Ablaufzeitraum auswählen, funktioniert der Connector nach Ablauf des API-Schlüssels nicht mehr. Anschließend müssen Sie einen API-Schlüssel neu generieren und Ihre [!DNL Workfront] -Konfiguration aktualisieren.

         1. Klicken Sie unter der Beschriftung **[!UICONTROL API-Schlüssel Ihres Benutzers]** auf **[!UICONTROL API-Schlüssel generieren]** .

            Ein API-Schlüssel für [!DNL Workfront] wird generiert und angezeigt.
      1. Kopieren Sie den API-Schlüssel in die Zwischenablage.
      1. Öffnen Sie die Browser-Registerkarte für AEM Connector und fügen Sie im Feld **[!DNL Workfront API Key]** den kopierten API-Schlüssel ein.
   1. (Bedingt) Klicken Sie auf die Registerkarte **[!UICONTROL Erweitert]** in der oberen linken Ecke der Seite [!UICONTROL [!DNL Workfront] Integrationskonfiguration] und wählen Sie die folgenden Optionen aus, sofern zutreffend:

      **[!UICONTROL Durchsuchen von Sammlungen zulassen]:** &#x200B; Wählen Sie diese Option, wenn Ihr Unternehmen es [!DNL Workfront] Benutzern ermöglicht, AEM Assets-Sammlungen mit [!DNL Workfront] -Objekten zu verknüpfen.

      **[!UICONTROL Benutzer-Federated ID]:** Wählen Sie diese Option aus, wenn Ihr Unternehmen bei der Anmeldung bei Workfront Federated IDs oder Single Sign-On (SSO) verwendet.

      **[!UICONTROL E-Mail-Domäne ignorieren]:** Wählen Sie diese Option, wenn Ihre AEM-Benutzer den Domänennamen nicht in ihrer Benutzer-ID verwenden.

      **[!UICONTROL Zugriff beschränken]:** Wählen Sie diese Option, um die entsprechenden [!DNL Workfront] IP-Adressen anzugeben, die der Zulassungsliste hinzugefügt werden müssen. Weitere Informationen zur Zulassungsliste finden Sie unter [Konfigurieren der Zulassungsliste Ihrer Firewall](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

   1. Klicken Sie auf die Registerkarte **[!UICONTROL Einfach]** oben links auf der Seite &quot;Workfront-Integrationskonfiguration&quot;und klicken Sie dann auf **[!UICONTROL Verbinden]**.

      >[!NOTE]
      >
      >Änderungen können einige Zeit in Anspruch nehmen. Das Neustart des Bundles kann den Prozess beschleunigen.



1. (Bedingt) Wenn Sie bereits eine [!DNL Workfront] -Cloud-Konfigurationsdatei erstellt haben, wählen Sie **[!UICONTROL Global-[!DNL Workfront]]** und klicken Sie dann oben links auf **[!UICONTROL Eigenschaften]**.

1. Generieren Sie den AEM API-Schlüssel, indem Sie auf **[!UICONTROL Schlüssel generieren],** klicken und dann den AEM API-Schlüssel in die Zwischenablage kopieren.

   Sie benötigen den AEM API-Schlüssel später, wenn Sie [!UICONTROL Workfront] für die Integration mit [!UICONTROL AEM Assets] konfigurieren. Weitere Informationen finden Sie unter [Konfigurieren von Workfront für die Integration mit AEM Assets](#configure-workfront-to-integrate-with-aem-assets).

1. Klicken Sie oben rechts auf **[!UICONTROL Speichern]**.

   Das Fenster [!UICONTROL Global-[!DNL Workfront]] wird angezeigt.

   ![properties.png](assets/properties-350x117.png)

1. (Optional) Synchronisieren Sie die bidirektionale Kommunikation zwischen AEM und [!DNL Workfront].

   1. Klicken Sie auf **[!UICONTROL Global-[!DNL Workfront]].**
   1. Klicken Sie in der linken oberen Ecke des Fensters auf **[!UICONTROL Eigenschaften]**.

      Die Seite [!UICONTROL [!DNL Workfront] Integrationskonfiguration] wird angezeigt.

      ![properties2.png](assets/properties2-350x444.png)

   1. (Optional) Um die Synchronisierung von Kommentaren zwischen [!UICONTROL AEM Assets] und [!DNL Workfront] zu aktivieren, klicken Sie auf **[!UICONTROL Kommentarsynchronisierung aktivieren]**.

      >[!IMPORTANT]
      >
      >Sie müssen die [!UICONTROL Dokumentsynchronisierung] aktivieren, um die Assets zu synchronisieren.

   1. (Optional) Klicken Sie zum Deaktivieren der Kommentarsynchronisierung auf **[!UICONTROL Kommentarsynchronisierung deaktivieren].**

      Oder

      Löschen Sie das für Ihre AEM-Instanz registrierte Ereignisabonnement [!UICONTROL NOTE CREATE] .

      Informationen zu Ereignisabonnements finden Sie unter [Ereignisabonnement-API](../../wf-api/general/event-subs-api.md).

1. Fahren Sie mit [Konfigurieren Sie den [!UICONTROL AEM Externalizer]](#configure-the-aem-externalizer) fort.

### Konfigurieren des [!UICONTROL AEM Externalizer] {#configure-the-aem-externalizer}

Mit dem [!UICONTROL AEM Externalizer] können AEM URLs in einem Format übergeben, das in [!DNL Workfront] verwendet werden kann. Wenn die URL nicht ordnungsgemäß konfiguriert ist, kann [!DNL Workfront] keine Aufrufe an die AEM-API tätigen und die URLs, die AEM Dokumente in Workfront verknüpfen, funktionieren nicht.

1. Klicken Sie in AEM auf **[!UICONTROL Tools]** > **[!UICONTROL Vorgänge]** >**[!UICONTROL Web-Konsole]**.

1. Klicken Sie auf **[!UICONTROL OSGI]** und dann im Dropdown-Menü auf **[!UICONTROL Konfiguration]** .

1. Wählen Sie in der Konfigurationsliste &#x200B;**[!UICONTROL Day CQ Link Externalizer].**

   Die Seite [!UICONTROL Externalizer] wird angezeigt.

1. Stellen Sie im Abschnitt **[!UICONTROL Domänen]** sicher, dass die im Feld [!UICONTROL Autor] aufgelistete Domäne der Domänenname ist, auf den AEM Benutzer extern zugreifen können.

   Der Domänenname im Feld [!UICONTROL author] sollte mit der Domäne übereinstimmen, die in der URL-Zeile Ihrer AEM-Instanz aufgeführt ist.

   ![[!DNL Extenalizer].png](assets/extenalizer-350x128.png)

1. (Bedingt) Aktualisieren Sie bei Bedarf die Domäne im Feld [!UICONTROL Autor] .
1. Klicken Sie auf **[!UICONTROL Speichern]**.

   [!UICONTROL AEM Assets] ist jetzt so konfiguriert, dass Dokumente mit [!DNL Workfront] verknüpft werden

1. Fahren Sie mit [Konfigurieren [!DNL Workfront] für die Integration mit [!DNL AEM assets]](#configure-workfront-to-integrate-with-aem-assets) fort.

## Konfigurieren von [!DNL Workfront] für die Integration mit [!DNL AEM assets] {#configure-workfront-to-integrate-with-aem-assets}

Nachdem Sie den Connector [!UICONTROL Workfront für AEM Assets] installiert haben (wie unter [Installieren des Connector-Pakets [!UICONTROL Workfront für AEM Assets]](#install-the-workfront-for-aem-assets-connector-package) beschrieben) und [!UICONTROL AEM Assets] konfiguriert haben (wie unter Konfigurieren von [!UICONTROL  AEM Assets] für die Integration mit  [!DNL Workfront]](#configure-aem-assets-to-integrate-with-workfront) beschrieben), müssen Sie [!DNL Workfront] so konfigurieren, dass Dokumente zwischen [!DNL Workfront] und [!DNL AEM Assets] verknüpft werden.[

1. Melden Sie sich bei [!DNL Workfront] als [!UICONTROL Workfront] -Administrator an.

   >[!TIP]
   >
   >[!UICONTROL Workfront] empfiehlt die Erstellung eines [!UICONTROL Workfront] -Administrators, der ausschließlich Ihrer AEM dient. Weitere Informationen zum Zuweisen der Zugriffsstufe des Administrators für [!UICONTROL Workfront] zu einem Benutzer finden Sie unter [Gewähren von Benutzern administrativen Zugriff auf bestimmte Bereiche](../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

{{step-1-to-setup}}

1. Klicken Sie auf **[!UICONTROL Dokumente]**> **[!UICONTROL Benutzerspezifische Integration].**

1. Klicken Sie auf **[!UICONTROL Benutzerdefinierte Integration hinzufügen]**.
1. Geben Sie im Feld **[!UICONTROL Name]** den Namen der benutzerdefinierten Integration an.

   Dies ist der Name, den Benutzer sehen, wenn sie die Integration in [!UICONTROL Workfront] verwenden. Sie können beispielsweise *&quot;[!DNL AEM Assets]&quot;* für den Namen eingeben.

1. Geben Sie im Feld **[!UICONTROL Basis-API-URL]** die URL für Ihre AEM-Instanz an.

   Die Basis-API-URL besteht aus der URL für Ihre AEM Instanz gefolgt vom Pfad: /bin/webhooks/api/

   ![mceclip3.png](assets/mceclip3-350x130.png)

1. Wählen Sie im Dropdown-Menü **[!UICONTROL Authentifizierungstyp]** die Option **[!UICONTROL APIKey].**

1. Fügen Sie in das Feld &#x200B;**[!UICONTROL API-Schlüssel]** den AEM API-Schlüssel ein, den Sie beim Konfigurieren von [!UICONTROL AEM Assets] kopiert haben.
1. Klicken Sie auf **[!UICONTROL Speichern]**.
1. (Optional) Stellen Sie sicher, dass die Integration als [!UICONTROL aktiv] gekennzeichnet ist.\
   ![aem_custom_integration_active.png](assets/aem-custom-integration-active-350x81.png)

   [!DNL Workfront] ist jetzt so konfiguriert, dass es mit [!DNL AEM Assets] funktioniert.

   Um auf Assets in AEM zugreifen zu können, muss jeder [!DNL Workfront]-Benutzer, der den Connector verwenden muss, als Benutzer in AEM eingerichtet sein. Informationen zum Erstellen von Benutzern finden Sie unter [Einrichten von Benutzern für die Verwendung des Connectors](#set-up-users-to-use-the-connector).

## Benutzer für die Verwendung des Connectors einrichten {#set-up-users-to-use-the-connector}

Damit Benutzer auf den Connector zugreifen können, müssen sie über ein Benutzerprofil in AEM verfügen und einer [!DNL Workfront] -Gruppe angehören, deren Zugriffsebene die Berechtigungen [!UICONTROL Erstellen] und [!UICONTROL Löschen] enthält.

Weitere Informationen zu [!DNL Workfront] -Berechtigungen finden Sie unter [Benutzerdefinierte Zugriffsebenen erstellen oder ändern](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

* [Benutzer in [!DNL AEM assets] einrichten](#set-up-users-in-aem-assets)

### Einrichten von Benutzern in [!DNL AEM assets] {#set-up-users-in-aem-assets}

1. Melden Sie sich bei [!DNL AEM Assets] als [!DNL Workfront] -Administrator an.
1. Klicken Sie auf **[!UICONTROL Tools]** >**&#x200B;** &#x200B;**[!UICONTROL Sicherheit]** >**[!UICONTROL Benutzer]**.

1. (Bedingt) Wenn der Benutzer kein Benutzerprofil in AEM hat, erstellen Sie ein AEM Benutzerprofil.

   1. Klicken Sie auf **[!UICONTROL Benutzer erstellen].**
   1. Geben Sie die persönlichen Daten des Benutzers ein.

      ![64NewUser.png](assets/64newuser-350x524.png)

      Das einzige erforderliche Feld ist das ID-Feld. Die AEM-ID des Benutzers muss mit der [!DNL Workfront]-ID übereinstimmen, der [!DNL Workfront]-E-Mail-Adresse des Benutzers.

      Wenn Sie die Option [!UICONTROL E-Mail-Domäne ignorieren] bei der Konfiguration der AEM für die Integration mit [!DNL Workfront] ausgewählt haben, stimmt die AEM-ID nicht mit der [!DNL Workfront] E-Mail-Adresse überein.

1. (Bedingt) Wenn der Benutzer über ein AEM Profil verfügt, öffnen Sie das AEM des Benutzers.

   1. Klicken Sie auf &#x200B;**[!UICONTROL Benutzer].**

      Die Seite [!UICONTROL Benutzerverwaltung] wird angezeigt.

   1. Klicken Sie auf den Benutzer, den Sie hinzufügen möchten, und klicken Sie dann auf **[!UICONTROL Eigenschaften]**.

      Die Einstellungsseite des Benutzers wird angezeigt.

1. Klicken Sie auf die Registerkarte **[!UICONTROL Gruppen]**.

   ![](assets/groupstab.png)

1. Stellen Sie sicher, dass der Benutzer zu mindestens einer [!DNL Workfront] Gruppe gehört, die über Zugriffsebenen verfügt, die die Berechtigungen [!UICONTROL Erstellen] und [!UICONTROL Löschen] enthalten.

   1. Um den Benutzer einer vorhandenen Gruppe hinzuzufügen, geben Sie zunächst den Gruppennamen in das Feld **[!UICONTROL Gruppenname]** ein und wählen Sie dann die Gruppe aus, wenn sie im Dropdown-Menü angezeigt wird.

      Oder

      Um eine Gruppe auszuwählen, der der Benutzer angehört, wählen Sie eine Gruppe im Abschnitt **[!UICONTROL Gruppen aus, der dieser Benutzer angehört]**.

1. Klicken Sie auf **[!UICONTROL Speichern].**
