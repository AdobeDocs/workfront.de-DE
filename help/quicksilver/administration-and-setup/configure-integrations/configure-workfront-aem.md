---
title: Konfigurieren  [!DNL Workfront]  Connectors  [!DNL Adobe Experience Manager] .veraltet
user-type: administrator
product-area: system-administration;workfront-integrations;setup
navigation-topic: administrator-integrations
description: Als  [!DNL Adobe Workfront]  können Sie eine Integration  [!DNL Workfront]  Adobe Experience Manager (AEM) Assets vornehmen und Ihrem Unternehmen eine umfassende Content-Management-Lösung für die Erstellung, Freigabe und Wartung von Assets innerhalb Ihres Workflows bieten.
author: Courtney
feature: System Setup and Administration, Workfront Integrations and Apps
role: Admin
exl-id: 024b8606-a9b7-413a-b393-8e5cdff37dd4
source-git-commit: 5d818b2e3c3314c6af076df46f7f806214f97bab
workflow-type: tm+mt
source-wordcount: '1869'
ht-degree: 0%

---

# Konfigurieren von [!DNL Workfront] mit [!DNL Adobe Experience Manager] Legacy-Connector

Als [!DNL Adobe Workfront] können Sie [!DNL Workfront] mit [!UICONTROL Adobe Experience Manager (AEM) Assets] integrieren und Ihrem Unternehmen eine umfassende Content-Management-Lösung für die Erstellung, Freigabe und Wartung von Assets in Ihrem Workflow bereitstellen.

## Zugriffsanforderungen

<!-- Audited: 4/2025 -->

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

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
   <td><p>Neu: Standard</p>
   <p>Oder</p>
   <p>Aktuell: Plan</p>
 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td>Systemadministrator </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## [!DNL Workfront for AEM Assets]

Die [!DNL Workfront for AEM Assets connector] ermöglicht Ihrem Unternehmen Folgendes:

* Zusammenarbeit und Verwaltung kreativer Inhalte durch Verknüpfen von AEM-Assets und -Ordnern mit Projekten, Aufgaben, Problemen und Anfragen in [!DNL Workfront].

  Weitere Informationen zum Konfigurieren von Dokumentationsintegrationen mit Anwendungen von Drittanbietern finden Sie unter [Konfigurieren von Dokumentintegrationen](../../administration-and-setup/configure-integrations/configure-document-integrations.md).

* Integration mit dem [!DNL AEM Digital Asset Managemen]t (DAM)-Repository, sodass Sie [!DNL Workfront] verwenden können, um im DAM gespeicherte digitale Assets zu verwalten und freizugeben.

  Weitere Informationen zum Verknüpfen von Dokumenten und Asset-Ordnern finden Sie unter   [Verknüpfen von Dokumenten aus externen Anwendungen](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

* Kombinieren und Anwenden von Metadaten aus beiden Programmen auf ein Asset.
* Anzeigen eines umfassenden Kommunikations-Streams für ein Asset Aktualisierungen und Kommentare, die in [!DNL Workfront] oder [!UICONTROL AEM Assets] an einem Asset vorgenommen wurden, werden mit dem anderen Programm synchronisiert, wodurch ein umfassender Verlauf der an dem Asset vorgenommenen Kommunikationen erstellt wird.

  Weitere Informationen zum Erstellen von Kommentaren in [!DNL Workfront] finden Sie unter [Hinzufügen einer Aktualisierung zu einem Dokument](../../documents/managing-documents/add-update-documents.md).

## Voraussetzungen für die Installation des [!DNL AEM Assets] Connectors

Stellen Sie vor der Installation des [!DNL Workfront]-Connectors für [!UICONTROL AEM Assets] sicher, dass die folgenden Voraussetzungen erfüllt sind:

* [!UICONTROL AEM Assets] ist installiert und konfiguriert, Version 6.5 oder höher. Informationen zur Installation von [!UICONTROL AEM Assets] finden Sie unter [[!DNL Adobe Experience Manager] Dokumentation](https://experienceleague.adobe.com/docs/experience-manager.html).
* (Bedingt) Wenn Ihre Firewall-Regeln Traffic nicht wie erwartet zulassen, fügen Sie die IP-Adresse und/oder Domain Ihres Clusters zu Ihrer Zulassungsliste hinzu. Weitere Informationen finden Sie [Zulassungsliste zum Konfigurieren der Firewall](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

## Installieren des [!DNL Workfront for AEM Assets] Connector-Pakets {#install-the-workfront-for-aem-assets-connector-package}

>[!IMPORTANT]
>
>Die folgenden Anweisungen gelten für einen [!DNL Workfront with AEM Assets] Legacy-Connector, der durch den [[!DNL Workfront for Experience Manager] erweiterten Connector“ ersetzt ](../../documents/workfront-and-experience-manager-integrations/workfront-for-experience-manager-enhanced-connector/workfront-for-aem-enhanced-connector.md). Weitere Informationen erhalten Sie von Ihrem Kontovertreter.

Um den [!DNL Workfront for AEM Assets]-Connector zu installieren, müssen Sie den Connector mit dem [!UICONTROL CRX Package Manager} als Paket in AEM ].

1. Laden Sie auf einer Workstation, auf der Sie AEM bereits installiert haben, die Installationsdatei für den [!DNL Workfront for AEM Assets] Connector herunter.

   Sie können den [!DNL Workfront for AEM Assets]-Connector von Ihrem [!DNL Workfront] abrufen.

1. Melden Sie sich mit einem Administratorkonto bei AEM an.
1. Klicken Sie **[!UICONTROL Tools]** > **[!UICONTROL Bereitstellung]** > **[!UICONTROL Pakete]**. Der [!UICONTROL CRX Package Manager] wird geöffnet.

1. Klicken Sie **[!UICONTROL Paket hochladen].**

1. Suchen Sie im Dialogfeld **[!UICONTROL Paket hochladen]** nach dem Paket **[!UICONTROL Workfront Connector]** und wählen Sie es aus. Klicken Sie dann auf **[!UICONTROL OK]**. Das Paket wird im [!UICONTROL CRX Package Manager] angezeigt.

1. Klicken Sie auf **[!UICONTROL Installieren].**

1. Ignorieren Sie im Dialogfeld **[!UICONTROL Paket]** die erweiterten Einstellungen und klicken Sie auf **[!UICONTROL Installieren]**.
1. (Optional) Um zu bestätigen, dass der Connector erfolgreich installiert wurde, stellen Sie sicher, dass im [!UICONTROL Aktivitätsprotokoll“ die folgende Anweisung angezeigt ]:

   ```
   Package installed in <time>
   ```

1. Schließen Sie den [!UICONTROL CRX Package Manager]. Der Connector ist installiert, und Sie können [!DNL AEM Assets] jetzt für die Integration mit [!DNL Workfront] konfigurieren.

1. Fahren Sie mit [Konfigurieren [!DNL AEM Assets]  fort, um mit zu  [!DNL Workfront]](#configure-aem-assets-to-integrate-with-workfront).

## Konfigurieren von [!DNL AEM Assets] für die Integration mit [!DNL Workfront] {#configure-aem-assets-to-integrate-with-workfront}

Importieren Sie nach der Installation des Connectors das Connector-Paket in AEM und konfigurieren Sie AEM so, dass es eine Verknüpfung mit Dokumenten in [!DNL Workfront] herstellt.

Informationen zur Installation des Connectors finden Sie unter [Installieren des  [!DNL Workfront for AEM Assets] -Connector-Pakets](#install-the-workfront-for-aem-assets-connector-package).

* [Voraussetzungen](#prerequisites)
* [Integrieren von AEM mit [!DNL Workfront]](#integrate-aem-with-workfront)
* [Konfigurieren Sie den [!UICONTROL AEM Externalizer]](#configure-the-aem-externalizer)

### Voraussetzungen {#prerequisites}

Bevor Sie beginnen, müssen Sie Berechtigungen für den Workfront-Service aktivieren:

1. Navigieren Sie in AEM zu **[!UICONTROL Tools]** > **[!UICONTROL Sicherheit]** > **[!UICONTROL Berechtigungen]**.
1. Wählen Sie oben links im Dropdown-Menü **[!UICONTROL Benutzer]**&#x200B; aus und geben Sie *[!UICONTROL Workfront-Service]* in das Feld **[!UICONTROL Suche]** &#x200B;. Wählen Sie den [!UICONTROL Workfront-Service]-Benutzer aus.
1. Klicken Sie auf der rechten Seite des Bildschirms auf **[!UICONTROL ACE hinzufügen]**, um neue Einträge zu erstellen.
1. Aktivieren Sie im Fenster &#x200B;**[!UICONTROL Neuen Eintrag hinzufügen]**&#x200B; das Kontrollkästchen-Symbol im Feld **[!UICONTROL Pfad]**&#x200B; und wählen Sie den Ordner aus: */conf*
1. Geben Sie **Feld** Folgendes ein: *jcr:read*
1. Klicken Sie oben rechts auf **[!UICONTROL Hinzufügen]**&#x200B;.
1. (Optional) Wiederholen Sie die obigen Schritte, um weitere Einträge zu erstellen.

### Integrieren von AEM mit [!DNL Workfront] {#integrate-aem-with-workfront}

1. Melden Sie sich bei AEM Assets als Administrator an.
1. Klicken Sie auf **[!UICONTROL Tools]** > **[!UICONTROL Cloud Services]** > **[!UICONTROL Workfront-Integrationskonfiguration]** > **[!UICONTROL Global-Workfront].**&#x200B;**&#x200B;**

1. (Bedingt) Wenn Sie dies noch nicht getan haben, erstellen Sie eine [!DNL Workfront] Cloud-Konfigurationsdatei:

   1. Klicken Sie oben rechts auf der [!DNL Global-Workfront] auf **[!UICONTROL Erstellen]**.
   1. Geben Sie im Feld **[!UICONTROL Workfront]** URL die URL für Ihre [!DNL Workfront] an.

      Beispiel: [!DNL https]://`<account>`.my.workfront.com, wobei `<account>` das Konto ist, das Sie für Integrationen mit AEM verwenden.

   1. Aktivieren Sie &#x200B; Feld **[!UICONTROL Basisordner]** das Kontrollkästchen-Symbol.
   1. Wählen Sie im Dropdown-Menü den Pfad aus, unter dem mit [!DNL Workfront] Objekten verknüpfte Dokumente gespeichert werden.
   1. Folgen Sie im angezeigten AEM-Modal dem Pfad zum Ordner mit den Dokumenten, die mit [!DNL Workfront] Objekten verbunden sind. Wählen Sie den Ordner aus und drücken **[!UICONTROL Auswählen]**&#x200B;in der oberen rechten Ecke.

      Sie können eine Verknüpfung zu einem beliebigen Ordner unter dem Stammverzeichnis /content/dam/ herstellen.

   1. Geben Sie im Feld **[!UICONTROL Workfront]** API-Schlüssel Ihren [!UICONTROL Workfront]-API-Schlüssel an.

      So rufen Sie Ihren [!DNL Workfront]-API-Schlüssel ab:

      1. Öffnen Sie eine Browser-Registerkarte und melden Sie sich als [!DNL Workfront] bei Ihrem [!DNL Workfront] an.

      {{step-1-to-setup}}

      1. Klicken Sie **[!UICONTROL System]** > **[!UICONTROL Kundeninformationen]**.

         Wenn Sie bereits einen API-Schlüssel generiert haben, wird Ihr [!DNL Workfront]-API-Schlüssel unter der Bezeichnung **Der API-Schlüssel** Benutzers“ angezeigt.

      1. (Bedingt) Wenn Sie noch keinen API-Schlüssel generiert haben, müssen Sie einen generieren:

         1. Stellen Sie im Abschnitt **[!UICONTROL API]** Schlüsseleinstellungen“ sicher, dass die Option **[!UICONTROL Nach der Erstellung laufen die API-Schlüssel in ab]** auf **Keine** gesetzt ist.

            Wenn Sie einen Gültigkeitszeitraum auswählen, funktioniert der Connector nach Ablauf des API-Schlüssels nicht mehr. Sie müssen dann einen API-Schlüssel neu generieren und Ihre [!DNL Workfront]-Konfiguration aktualisieren.

         1. Klicken **[!UICONTROL unter der Beschriftung „API-Schlüssel Ihres Benutzers]** auf **[!UICONTROL API-Schlüssel generieren]**. Ein API-Schlüssel für [!DNL Workfront] generiert und zeigt ihn an.
      1. Kopieren Sie den API-Schlüssel in die Zwischenablage.
      1. Öffnen Sie die Browser-Registerkarte für AEM Connector und fügen Sie den kopierten API-Schlüssel in das **[!DNL Workfront API Key]** ein.
   1. (Bedingt) Klicken Sie auf die **[!UICONTROL Erweitert]** in der oberen linken Ecke der Seite [!UICONTROL [!DNL Workfront]-Integrationskonfiguration] und wählen Sie die folgenden Optionen aus, falls zutreffend:

      **[!UICONTROL Durchsuchen von Sammlungen zulassen]:** Wählen Sie &#x200B; Option aus, wenn Ihr Unternehmen [!DNL Workfront] Benutzern erlaubt, AEM Assets-Sammlungen mit [!DNL Workfront] Objekten zu verknüpfen.

      **[!UICONTROL Benutzer Federated ID]:** Wählen Sie diese Option aus, wenn Ihr Unternehmen Federated IDs oder Single Sign-On (SSO) bei der Anmeldung bei Workfront verwendet.

      **[!UICONTROL E-Mail-Domain ignorieren]:** Wählen Sie diese Option, wenn AEM-Benutzer den Domain-Namen nicht in ihrer Benutzer-ID verwenden.

      **[!UICONTROL Zugriff beschränken]:** Wählen Sie diese Option, um die entsprechenden [!DNL Workfront] IP-Adressen anzugeben, die der Zulassungsliste hinzugefügt werden müssen. Weitere Informationen über die Zulassungsliste finden Sie [Zulassungsliste zur Firewall konfigurieren](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

   1. Klicken Sie oben links auf der Seite Workfront-Integrationskonfiguration auf die Registerkarte **[!UICONTROL Standard]** und dann auf **[!UICONTROL Verbinden]**.

      >[!NOTE]
      >
      >Es kann einige Zeit dauern, bis die Änderungen angewendet werden. Ein Neustart des Bundles kann den Prozess beschleunigen.



1. (Bedingt) Wenn Sie bereits eine [!DNL Workfront] Cloud-Konfigurationsdatei erstellt haben, wählen Sie **[!UICONTROL global-[!DNL Workfront]]** aus und klicken Sie dann links oben auf **[!UICONTROL Eigenschaften]**.

1. Generieren Sie den AEM-API-Schlüssel, indem **[!UICONTROL Generate Key] klicken** den AEM-API-Schlüssel in die Zwischenablage kopieren.

   Sie benötigen den AEM-API-Schlüssel später, wenn Sie [!UICONTROL Workfront] für die Integration mit [!UICONTROL AEM Assets] konfigurieren. Weitere Informationen finden Sie unter [Konfigurieren von Workfront für die Integration mit AEM Assets](#configure-workfront-to-integrate-with-aem-assets).

1. Klicken Sie oben rechts auf **[!UICONTROL Speichern]**. Das Fenster [!UICONTROL Global-[!DNL Workfront]]&quot; wird angezeigt.

   ![properties.png](assets/properties-350x117.png)

1. (Optional) Synchronisieren Sie die bidirektionale Kommunikation zwischen AEM und [!DNL Workfront]:

   1. Klicken Sie auf **[!UICONTROL global-[!DNL Workfront]].**
   1. Klicken Sie oben links im Fenster auf **[!UICONTROL Eigenschaften]**. Die Seite **[!UICONTROL [!DNL Workfront]-Integrationskonfiguration]** wird angezeigt.

      ![properties2.png](assets/properties2-350x444.png)

   1. (Optional) Um die Synchronisierung von Kommentaren zwischen [!UICONTROL AEM Assets] und [!DNL Workfront] zu aktivieren, klicken Sie auf **[!UICONTROL Kommentarsynchronisierung aktivieren]**.

      >[!IMPORTANT]
      >
      >Sie müssen &quot;[!UICONTROL &quot; aktivieren] um die Assets zu synchronisieren.

   1. (Optional) Um die Kommentarsynchronisierung zu deaktivieren, klicken Sie auf **[!UICONTROL Kommentarsynchronisierung deaktivieren].**

      Oder

      Löschen Sie das [!UICONTROL NOTE CREATE]-Ereignisabonnement, das bei Ihrer AEM-Instanz registriert ist.

      Informationen zu Ereignisabonnements finden Sie unter [Ereignisabonnement-API](../../wf-api/general/event-subs-api.md).

1. Fahren Sie fort mit [Konfigurieren des [!UICONTROL AEM Externalizer]](#configure-the-aem-externalizer).

### Konfigurieren Sie den [!UICONTROL AEM Externalizer] {#configure-the-aem-externalizer}

Mit dem [!UICONTROL AEM Externalizer] kann AEM URLs in einem Format übergeben, das in [!DNL Workfront] verwendet werden kann. Wenn [!DNL Workfront] nicht richtig konfiguriert sind, können Sie die AEM-API nicht aufrufen, und die URLs, die AEM-Dokumente in Workfront verknüpfen, funktionieren nicht.

1. Klicken Sie in AEM auf **[!UICONTROL Tools]** > **[!UICONTROL Vorgänge]** > **[!UICONTROL Web-Konsole]**.

1. Klicken Sie **[!UICONTROL OSGI]** und dann ]**Dropdown-Menü auf**[!UICONTROL  Konfiguration“.

1. Wählen Sie in der Konfigurationsliste &#x200B;/**[!UICONTROL CQ Link Externalizer ].** Die Seite **[!UICONTROL Externalizer]** wird angezeigt.

1. Stellen Sie im Abschnitt **[!UICONTROL Domains]** sicher, dass die im Feld **[!UICONTROL author]** aufgeführte Domain der Domain-Name ist, auf den AEM-Benutzer extern zugreifen können.

   Der Domain-Name im Feld [!UICONTROL author] sollte mit der Domain übereinstimmen, die in der URL-Zeile Ihrer AEM-Instanz aufgeführt ist.

   ![[!DNL Extenalizer].png](assets/extenalizer-350x128.png)

1. (Bedingt) Aktualisieren Sie bei Bedarf die Domain im Feld **[!UICONTROL Autor]**.
1. Klicken Sie auf **[!UICONTROL Speichern]**. [!UICONTROL AEM Assets] ist jetzt so konfiguriert, dass Dokumente mit [!DNL Workfront] verknüpft werden.

1. Fahren Sie mit [Konfigurieren [!DNL Workfront]  fort, um mit zu  [!DNL AEM assets]](#configure-workfront-to-integrate-with-aem-assets).

## Konfigurieren von [!DNL Workfront] für die Integration mit [!DNL AEM assets] {#configure-workfront-to-integrate-with-aem-assets}

Nach der Installation des [!UICONTROL Connectors für WorkfrontAEM Assets ] (wie unter [Installieren des [!UICONTROL Connector-Pakets für Workfront für AEM Assets] beschrieben](#install-the-workfront-for-aem-assets-connector-package)) und der Konfiguration von [!UICONTROL AEM Assets] (wie unter [Konfigurieren[!UICONTROL  AEM Assets] für die Integration mit [!DNL Workfront]](#configure-aem-assets-to-integrate-with-workfront) beschrieben) müssen Sie [!DNL Workfront] konfigurieren, um Dokumente zwischen [!DNL Workfront] und [!DNL AEM Assets] zu verknüpfen.

1. Melden Sie sich bei Workfront als Administrator an.

   >[!TIP]
   >
   >[!UICONTROL Workfront] empfiehlt, einen [!UICONTROL Workfront]-Administrator zu erstellen, der ausschließlich Ihrer AEM-Integration dient. Weitere Informationen zum Zuweisen der Admin-Zugriffsebene [!UICONTROL Workfront] zu einem Benutzer finden Sie unter [Gewähren von administrativem Zugriff für Benutzer auf bestimmte Bereiche](../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

{{step-1-to-setup}}

1. Klicken Sie auf **[!UICONTROL Dokumente]** > **[!UICONTROL Benutzerdefinierte Integration].**

1. Klicken Sie **[!UICONTROL Benutzerdefinierte Integration hinzufügen]**.
1. Geben **[!UICONTROL in das Feld]** den Namen der benutzerdefinierten Integration ein.

   Dies ist der Name, den Benutzer sehen, wenn sie die Integration in [!UICONTROL Workfront] verwenden.

1. Geben Sie in das Feld **[!UICONTROL Basis]** API-URL die URL für Ihre AEM-Instanz ein.

   Die Basis-API-URL besteht aus der URL für Ihre AEM-Instanz, gefolgt vom Pfad: /bin/webhooks/api/

   ![mceclip3.png](assets/mceclip3-350x130.png)

1. Wählen Sie im Dropdown **[!UICONTROL Menü]** Authentifizierungstyp“ die Option **[!UICONTROL APIkey].**

1. Fügen Sie im Feld &#x200B;**[!UICONTROL API-]** den AEM-API-Schlüssel ein, den Sie bei der Konfiguration von [!UICONTROL AEM Assets kopiert ].
1. Klicken Sie auf **[!UICONTROL Speichern]**.
1. (Optional) Stellen Sie sicher, dass die Integration mit [!UICONTROL Aktiv] markiert ist.\
   ![aem_custom_integration_active.png](assets/aem-custom-integration-active-350x81.png)

   [!DNL Workfront] ist jetzt für die Verwendung mit [!DNL AEM Assets] konfiguriert.

   Um auf Assets in AEM zugreifen zu können, muss jeder [!DNL Workfront], der den Connector verwenden muss, in AEM als Benutzer eingerichtet sein. Informationen zum Erstellen von Benutzern finden Sie unter [Einrichten von Benutzern für die Verwendung des Connectors](#set-up-users-to-use-the-connector).

## Einrichten von Benutzern für die Verwendung des Connectors {#set-up-users-to-use-the-connector}

Damit Benutzer auf den Connector zugreifen können, müssen sie über ein Benutzerprofil in AEM verfügen und zu einer [!DNL Workfront] gehören, die über Zugriffsebenen mit den Berechtigungen [!UICONTROL Erstellen] und [!UICONTROL Löschen] verfügt.

Weitere Informationen zu [!DNL Workfront] finden Sie unter [Erstellen oder Ändern benutzerdefinierter Zugriffsebenen](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

* [Einrichten von Benutzern in [!DNL AEM assets]](#set-up-users-in-aem-assets)

### Einrichten von Benutzern in [!DNL AEM assets] {#set-up-users-in-aem-assets}

1. Melden Sie sich bei [!DNL AEM Assets] als Workfront-Administrator an.
1. Klicken Sie **[!UICONTROL Tools]** > **&#x200B;**&#x200B;**[!UICONTROL security]** > **[!UICONTROL users]**.

1. (Bedingt) Wenn der/die Benutzende in AEM kein Benutzerprofil hat, erstellen Sie ein AEM-Benutzerprofil.

   1. Klicken Sie **[!UICONTROL Benutzer erstellen].**
   1. Geben Sie die persönlichen Informationen des Benutzers ein.

      ![64NewUser.png](assets/64newuser-350x524.png)

      Das einzige erforderliche Feld ist das **ID**-Feld. Die AEM-ID des Benutzers muss mit seiner [!DNL Workfront]-ID übereinstimmen, d. h. mit seiner [!DNL Workfront]-E-Mail-Adresse.

      Wenn Sie die Option **[!UICONTROL E-Mail-Domain ignorieren]** ausgewählt haben, als Sie AEM für die Integration mit [!DNL Workfront] konfiguriert haben, stimmt die AEM-ID nicht mit der [!DNL Workfront] E-Mail-Adresse überein.

1. (Bedingt) Wenn der/die Benutzende über ein AEM-Profil verfügt, öffnen Sie das AEM-Profil des/r Benutzenden:

   1. click&#x200B;**[!UICONTROL user]**. Die **[!UICONTROL Benutzerverwaltung]** wird angezeigt.

   1. Klicken Sie auf den Benutzer, den Sie hinzufügen möchten, und dann auf **[!UICONTROL Eigenschaften]**. Die Seite mit den Benutzereinstellungen wird angezeigt.

1. Klicken Sie auf **[!UICONTROL Registerkarte]** Gruppen“.

   ![Registerkarte „Gruppen“](assets/groupstab.png)

1. Stellen Sie sicher, dass der Benutzer zu mindestens einer [!DNL Workfront] gehört, die über Zugriffsebenen verfügt, die die Berechtigungen **[!UICONTROL Erstellen]** und **[!UICONTROL Löschen]** beinhalten.

   1. Um den Benutzer einer vorhandenen Gruppe hinzuzufügen, geben Sie den Gruppennamen in das Feld **[!UICONTROL Gruppennamen eingeben]** und wählen Sie dann die Gruppe aus, wenn sie im Dropdown-Menü angezeigt wird.

      Oder

      Um eine Gruppe auszuwählen, der der Benutzer angehört, wählen Sie eine Gruppe im Abschnitt **[!UICONTROL Gruppen, denen dieser Benutzer angehört]** aus.

1. Klicken Sie **[!UICONTROL Speichern].**
