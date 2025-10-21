---
product-area: documents
navigation-topic: approvals
title: AppBuilder in Workfront Document Details
description: Sie können AppBuilder in Dokumentdetails installieren
author: Courtney
feature: Work Management, Digital Content and Documents
hide: true
hidefromtoc: true
recommendations: noDisplay, noCatalog
exl-id: 74e0a85b-a8aa-4e39-9c2e-0f09957ebafa
source-git-commit: cd0214917620e0b147d0da3402ea2d34e28bc9c3
workflow-type: tm+mt
source-wordcount: '1357'
ht-degree: 0%

---

# AppBuilder in Workfront Document Details

Sie können AppBuilder in Dokumentdetails installieren.

## Voraussetzungen

Sie müssen über Folgendes verfügen:

* Ein IMS-aktiviertes Workfront-Konto
* Ein Entwicklungsrechner mit Knoten v18 und npm

## Hinzufügen von Entwicklern zur Admin Console

>[!IMPORTANT]
>
>Stellen Sie sicher, dass Sie für alle folgenden Schritte die richtige IMS-Organisation ausgewählt haben. Wenn Sie mehreren Organisationen angehören, können Sie die falsche auswählen. Stellen Sie sicher, dass Sie unter der rechten Organisation handeln, die normalerweise oben rechts aufgeführt ist.


1. Navigieren Sie zu einem der folgenden:

* Schritt: [https://stage.adminconsole.adobe.com/](https://stage.adminconsole.adobe.com/)
* PROD: [https://adminconsole.adobe.com/](https://adminconsole.adobe.com/)

1. Klicken Sie im Abschnitt Benutzer auf **Entwickler** > **Entwickler hinzufügen**.

   ![Verwalten von Entwicklern in Admin Console](assets/manage-users-admin-console.png)

   >[!NOTE]
   >
   >Wenn keine Option zum Verwalten von Entwicklern angezeigt wird, verfügen Sie über kein Produkt, das den Entwicklerzugriff ermöglicht. Workfront bietet im Gegensatz zu AEM keinen Entwicklerzugriff. Wenn Sie dies nicht sehen, müssen wir herausfinden, wie wir Workfront in die Liste der Apps aufnehmen können, die Entwickler unterstützen.

1. Fügen Sie die E-Mail des Benutzers hinzu. Sie sollte nach vorhandenen Benutzern suchen, die bereits in der Admin Console hinzugefügt wurden.

1. Fügen Sie die erforderlichen Produkte zum Entwicklerprofil hinzu und klicken Sie auf **Speichern**.

![Entwickler hinzufügen](assets/add-developer.png)

## Zugriff auf AppBuilder erhalten

Unternehmen müssen mit ihren Account Managern zusammenarbeiten, um AppBuilder zu erwerben. Der genaue Prozess dafür ist nicht verstanden, da wir dies für den POC nicht tun mussten.

Wenn Sie die AppBuilder-Integration testen möchten, können Sie hier eine kostenlose Testversion für Ihre IMS-Organisation anfordern:
[https://developer.adobe.com/app-builder/docs/overview/getting_access/#](https://developer.adobe.com/app-builder/docs/get_started/app_builder_get_started/set-up#access-and-credentials)

Ich habe den Eindruck, dass sie die Testversion, auch wenn es eine kostenlose 30-Tage-Testversion ist, danach nicht mehr deaktivieren werden.

Wenn AppBuilder ordnungsgemäß konfiguriert ist, sollte beim Erstellen eines neuen Projekts „Projekt aus Vorlage erstellen“ angezeigt werden (was im nächsten Abschnitt behandelt wird).

## Erstellen eines neuen Projekts in der Developer Console

1. Klicken Sie **Projekt aus Vorlage erstellen**.

   >[!IMPORTANT]
   >
   >Wenn diese Option nicht angezeigt wird, sind Sie in der Admin Console falsch konfiguriert und haben keinen Zugriff auf den App Builder-Katalog. Diese Option wird nur angezeigt, wenn Sie Zugriff auf AppBuilder haben.

   ![Erstellen eines Projekts aus einer Vorlage](assets/create-from-template.png)

1. **App Builder**.

1. Geben Sie einen **Projekttitel** und **App-Namen** ein. Beide verfügen über Standardwerte, aber es ist später einfacher, das gewünschte Projekt zu identifizieren, wenn Sie den Wert anpassen.

   >[!NOTE]
   >
   >In diesem Schritt gibt es eine Option zum Hinzufügen zusätzlicher Arbeitsbereiche. Uns wurde vorgeschlagen, für jeden Entwickler einen Arbeitsbereich zu erstellen. Dadurch werden Geheimnisse und Bereitstellungen bei der Entwicklungsarbeit voneinander getrennt. Sie sollten den Arbeitsbereich mit dem Namen des Entwicklers benennen, der ihn verwendet. Die AIO-CLI bietet Optionen zum Wechseln des Arbeitsbereichs, die wir später behandeln werden.


1. Lassen Sie **Laufzeit**.

1. Klicken Sie auf **Speichern**.

## Adobe IO (AIO) CLI

Adobe bietet eine Open-Source-CLI, die zum Erstellen der App Builder-Programme verwendet werden kann. Die Dokumentation finden Sie hier: [https://github.com/adobe/aio-cli](https://github.com/adobe/aio-cli) sowie Adobe App Builder-Anweisungen [https://developer.adobe.com/app-builder/docs/getting_started/first_app/](https://developer.adobe.com/app-builder/docs/get_started/app_builder_get_started/first-app).

1. Installation

   1. Um das Tool zu installieren (stellen Sie sicher, dass Sie sich zuerst auf dem Knoten 18 befinden), führen Sie `npm install -g @adobe/aio-cli` aus.

1. Im Terminal authentifizieren

   1. Starten Sie Ihr Terminal und melden Sie sich mit dem Befehl `aio login` bei der Organisation an.

1. Initialisieren der Anwendung

   1. Beginnen Sie mit der Einrichtung Ihrer App, indem Sie Folgendes ausführen: `aio app init example-app`.

1. Konfigurationsauswahl

   1. Wählen Sie anschließend Organisation und Projekt aus den bereitgestellten Optionen aus.

      ![Organisation auswählen](assets/select-org.png)

      ![Projekt auswählen](assets/select-project.png)

1. Vorlagenauswahl und Einrichtung

   1. Durchsuchen Sie alle verfügbaren Vorlagen und wählen Sie die Vorlage **@adobe/aem-cf-editor-ui-ext-tpl** für Ihr Projekt aus.

      ![Suchvorlage](assets/search-template.png)

      ![Vorlage auswählen](assets/select-template.png)

1. Definieren der Erweiterung

   1. Benennen Sie Ihre Erweiterung.
   1. Geben Sie eine beschreibende Zusammenfassung der Funktionalität Ihrer Erweiterung an.
   1. Wählen Sie eine anfängliche Versionsnummer aus, mit der Sie beginnen möchten.
   1. Bestätigen Sie den Abschluss, indem **Ich bin fertig** auswählen.

   ![Erweiterung definieren](assets/define-extension.png)

1. Navigieren Sie zu Ihrem Projektordner

   1. Zugriff auf den src-Ordner

   1. Benennen Sie den Ordner `aem-cf-editor-1` in `workfront-doc-details-1` um.

1. Konfigurationsdateien ändern

   1. Öffnen Sie app.config.yaml
   1. Aktualisieren Sie die Zeile von `aem/cf-editor/1` in `workfront/doc-details/1`.
   1. Passen Sie den Einschlusspfad von `src/aem-cf-editor-1/ext.config.yaml` nach `src/workfront-doc-details-1/ext.config.yaml` an.

1. Bearbeiten der Erweiterungsregistrierungs-Komponente

   1. Öffnen Sie `src/workfront-doc-details-1/web-src/src/components/ExtensionRegistration.js`.
   1. Fügen Sie im Methodenabschnitt eine `secondaryNav` hinzu, die eine asynchrone `getButtons` enthält.
   1. `getButtons` sollte ein -Objekt mit der folgenden Struktur erhalten:

      ```
          {
          docId: "String",  // Document ID
          docvId: "String", // Document version ID
          sharedContext: {
              hostname: "String",
              protocol: "String",
              auth: {
              imsOrgID: "String",    // Customer's IMS Org ID
              imsToken: "String",    // User's IMS token
              imsClientId: "String"
              }
          }
          }
      ```

1. Diese Funktion gibt ein Array von Schaltflächen-Objekten zurück, die in der Navigation angezeigt werden:

   ```
       methods: {
       secondaryNav: {
           async getButtons({docId, docvId, sharedContext}) {
           return [
               { label: 'Registration', url: '/index.html' },
               { label: 'Review', url: '/index.html#review' }
           ];
           }
       }
       }
   ```

1. Konfigurieren von Anwendungs-Routing
   1. Öffnen Sie Ihre App.js-Datei und konfigurieren Sie die Routen, um die neu entwickelten Funktionen einzuschließen. Sie müssen Routen für die Standardansicht und alle zusätzlichen Ansichten wie die Überprüfungsseite einrichten. So können Sie diese Routen definieren:

      ```
          <Route index element={<ExtensionRegistration />} />
          <Route exact path="index.html" element={<ExtensionRegistration />} />
          <Route exact path="review" element={<Review />} />
      ```

1. Dokumentdetails aufrufen
   1. Implementieren Sie die bereitgestellten `document.getDocumentDetails` in Ihrer Anwendung, um wichtige Dokumentspezifikationen abzurufen. Diese Funktion ruft ein -Objekt ab, das `docId` und `docvId` sowie ein `sharedContext` mit `hostname`-, `protocol`- und Authentifizierungsdetails enthält. Stellen Sie sicher, dass Ihre Anwendung diese Daten ordnungsgemäß verarbeitet.

1. Integrieren des Datenabrufs in Ihre Komponenten
   1. Fügen Sie eine neue Komponente zum Komponentenordner Ihres Programms hinzu. Stellen Sie innerhalb dieser Komponente eine Verbindung zu Workfront her, um Dokumentinformationen und Authentifizierungsdaten mithilfe der Verbindung abzurufen, die mit der Hostanwendung hergestellt wurde. Im Folgenden finden Sie ein Beispiel dafür, wie Sie Ihre Komponente strukturieren können, um dies zu handhaben:

      ```
          import { useEffect, useState } from 'react';
          import { attach } from "@adobe/uix-guest";
          import { extensionId } from "./Constants";
      
          function Review() {
              const [conn, setConn] = useState();
      
              useEffect(() => {
              const iife = async () => {
                  // "attach" the guest application to the host. This creates a "tunnel" from the host app that allows data to be passed to the iframe running this app.
                  const connection = await attach({
                  id: extensionId,
                  });
                  setConn(connection);
              };
      
              iife();
              }, []);
      
              useEffect(() => {
                  if (conn) {
                      // Using the connection created above, grab the document details from the host tunnel.
                      conn?.host?.document?.getDocumentDetails().then(setDocDetails);
                      // Pull the auth tokens from the sharedContext (see host app for details)
                      setAuth(conn?.sharedContext?.get("auth"));
                      setHostname(conn?.sharedContext?.get("hostname"));
                      setProtocol(conn?.sharedContext?.get("protocol"));
                  }
              }, [conn]);
      
          return (<>Text</>);
          }
      
          export default Review;
      ```

## Konfiguration für bestehende AIO-Projekte

1. Aktualisieren von Konfigurationsdateien
   1. Öffnen Sie `app.config.yaml`.
   1. Ändern Sie die Konfiguration, indem Sie die Referenz von `aem/cf-editor/1` auf `workfront/doc-details/1` aktualisieren. Durch diese Anpassung werden die Dateipfade an Ihrer aktuellen Projektstruktur ausgerichtet.

1. Überarbeiten der Registrierungskomponente für Erweiterungen
   1. Suchen und öffnen Sie die Datei mit dem Namen `ExtensionRegistration.js`.
   1. Fügen Sie im Methodenabschnitt eine `secondaryNav` hinzu, die eine asynchrone `getButtons` enthält.
   1. `getButtons` sollte ein -Objekt mit der folgenden Struktur erhalten:

      ```
          {
          docId: "String",  // Document ID
          docvId: "String", // Document version ID
          sharedContext: {
              hostname: "String",
              protocol: "String",
              auth: {
              imsOrgID: "String",    // Customer's IMS Org ID
              imsToken: "String",    // User's IMS token
              imsClientId: "String"
              }
          }
          }
      ```

1. Diese Funktion gibt ein Array von Schaltflächen-Objekten zurück, die in der Navigation angezeigt werden:

   ```
       methods: {
       secondaryNav: {
           async getButtons({docId, docvId, sharedContext}) {
           return [
               { label: 'Registration', url: '/index.html' },
               { label: 'Review', url: '/index.html#review' }
           ];
           }
       }
       }
   ```

1. Konfigurieren von Anwendungs-Routing
   1. Öffnen Sie Ihre `App.js`Datei“ und konfigurieren Sie die Routen, um die neu entwickelten Funktionen einzuschließen. Sie müssen Routen für die Standardansicht und alle zusätzlichen Ansichten wie die Überprüfungsseite einrichten. So können Sie diese Routen definieren:

      ```
          <Route index element={<ExtensionRegistration />} />
          <Route exact path="index.html" element={<ExtensionRegistration />} />
          <Route exact path="review" element={<Review />} />
      ```

1. Dokumentdetails aufrufen
   1. Implementieren Sie die bereitgestellten `document.getDocumentDetails` in Ihrer Anwendung, um wichtige Dokumentspezifikationen abzurufen. Diese Funktion ruft ein -Objekt ab, das `docId` und `docvId` sowie ein `sharedContext` mit `hostname`-, `protocol`- und Authentifizierungsdetails enthält. Stellen Sie sicher, dass Ihre Anwendung diese Daten ordnungsgemäß verarbeitet.

1. Integrieren des Datenabrufs in Ihre Komponenten
   1. Fügen Sie eine neue Komponente zum Komponentenordner Ihres Programms hinzu. Stellen Sie innerhalb dieser Komponente eine Verbindung zu Workfront her, um Dokumentinformationen und Authentifizierungsdaten mithilfe der Verbindung abzurufen, die mit der Hostanwendung hergestellt wurde. Im Folgenden finden Sie ein Beispiel dafür, wie Sie Ihre Komponente strukturieren können, um dies zu handhaben:

      ```
          import { useEffect, useState } from 'react';
          import { attach } from "@adobe/uix-guest";
          import { extensionId } from "./Constants";
      
          function Review() {
              const [conn, setConn] = useState();
      
              useEffect(() => {
              const iife = async () => {
                  // "attach" the guest application to the host. This creates a "tunnel" from the host app that allows data to be passed to the iframe running this app.
                  const connection = await attach({
                  id: extensionId,
                  });
                  setConn(connection);
              };
      
              iife();
              }, []);
      
              useEffect(() => {
                  if (conn) {
                      // Using the connection created above, grab the document details from the host tunnel.
                      conn?.host?.document?.getDocumentDetails().then(setDocDetails);
                      // Pull the auth tokens from the sharedContext (see host app for details)
                      setAuth(conn?.sharedContext?.get("auth"));
                      setHostname(conn?.sharedContext?.get("hostname"));
                      setProtocol(conn?.sharedContext?.get("protocol"));
                  }
              }, [conn]);
      
          return (<>Text</>);
          }
      
          export default Review;
      ```

## Programme veröffentlichen

>[!IMPORTANT]
>
>Stellen Sie sicher, dass Sie für jeden der folgenden Schritte die richtige IMS-Organisation ausgewählt haben.

Damit ein Gastantrag in Workfront geladen werden kann, muss der Antrag an den Produktionsarbeitsbereich gesendet und zur Genehmigung eingereicht werden.

1. Anwendung im Produktionsarbeitsbereich bereitstellen

   1. `aio app use -w Production`
   1. `aio app deploy`

1. Navigieren Sie zu [https://developer-stage.adobe.com/](https://developer-stage.adobe.com/) oder [https://developer.adobe.com/](https://developer.adobe.com/).

   1. Klicken **oben** auf „Konsole“.

1. Suchen Sie das Projekt, das Sie zum Erstellen des AppBuilder-Programms verwendet haben.
1. Wählen Sie die Produktions-Workspace aus.

   ![Produktions-Arbeitsbereich auswählen](assets/find-application.png)

1. Senden Sie den Antrag zur privaten Überprüfung (Sie erhalten Warnungen, dass wir nicht auf dem App Exchange-Marktplatz veröffentlichen, was in Ordnung ist).
1. Füllen Sie das Formular aus (Titel, Beschreibung, Symbol und Hinweis für den Prüfer).

   ![Formular zur privaten Überprüfung ausfüllen](assets/submission-details.png)

>[!IMPORTANT]
>
>Nach der Übermittlung muss ein Systemadministrator für die Organisation die Übermittlung genehmigen.

## Übermittlung genehmigen

1. Navigieren Sie als Systemadministrator zu [https://stage.exchange.adobe.com/](https://stage.exchange.adobe.com/) oder [https://exchange.adobe.com/](https://exchange.adobe.com/).

1. Klicken Sie **Verwalten** > **Experience Cloud Applications**. Die eingereichten Apps sollten mit Optionen zum Genehmigen/Ablehnen angezeigt werden.
Nach der Genehmigung sollten die veröffentlichten Anwendungserweiterungen automatisch in Ihrer Workfront-Umgebung geladen werden.

   ![Genehmigte Übermittlung](assets/approve-submission.png)

## Zusätzliche Hilfe

Adobe bietet eine hervorragende Dokumentation zu den ersten Schritten beim Erstellen von Apps für AppBuilder und deren Bereitstellung.

Im Folgenden finden Sie einige hilfreiche Links:

* [https://developer.adobe.com/app-builder/docs/getting_started/first_app/#4-bootstrapping-new-app-using-the-cli](https://developer.adobe.com/app-builder/docs/get_started/app_builder_get_started/first-app#bootstrap-the-new-app-using-the-cli)

* [https://developer.adobe.com/uix/docs/guides/publication/](https://developer.adobe.com/uix/docs/guides/publication/)

* [https://developer.adobe.com/uix/docs/services/aem-cf-console-admin/extension-development/](https://developer.adobe.com/uix/docs/services/aem-cf-console-admin/extension-development/)

## Lokale Entwicklung

Beim Entwickeln Ihres App Builder-Programms für Workfront müssen Sie Ihr Programm möglicherweise in Workfront testen, ohne es zu veröffentlichen. Glücklicherweise haben wir dafür eine Lösung.

Innerhalb Ihrer App Builder-App können Sie `aio app run` für die lokale Entwicklung initiieren. Dadurch erhalten Sie eine URL, normalerweise `https://localhost:9080`. Alternativ können Sie `aio app deploy` ausführen, um eine statische Adobe-Domain abzurufen. Notieren Sie sich diese URLs für die zukünftige Verwendung.

Navigieren Sie dann in Ihrem Browser zur Dokumentdetailseite, für die Sie eine Entwicklung durchführen möchten. Öffnen Sie die Entwickler-Tools und greifen Sie auf den lokalen Speicher für workfront.com oder workfront.adobe.com zu. Hier müssen Sie einen Eintrag hinzufügen. Verwenden Sie `appBuilderDocDetailsOverride` als Schlüssel und die zuvor erwähnte App Builder-URL als Wert.

Nach dem Neuladen der Seite werden die Schaltflächen in Ihrer App Builder-Anwendung angezeigt. Durch Klicken auf diese Schaltflächen können Sie Ihre App in Aktion anzeigen.
