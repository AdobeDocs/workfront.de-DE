---
title: Erstellen benutzerdefinierter Programme für Workfront mit Adobe App Builder
description: Benutzeroberflächenerweiterungen für Workfront auf Basis von Adobe App Builder ermöglichen es Kunden und Partnern, benutzerdefinierte Benutzererlebnisse zu erstellen.
author: Courtney
feature: Digital Content and Documents
exl-id: 2ed75053-8199-474c-afb4-fa9bbd3750f8
source-git-commit: a4e715d5212c3c166ce6ed995b327eb2b7198123
workflow-type: tm+mt
source-wordcount: '1693'
ht-degree: 0%

---

# Erstellen benutzerdefinierter Programme für Workfront mit Adobe App Builder

Benutzeroberflächenerweiterungen für Workfront auf Basis von Adobe App Builder ermöglichen es Kunden und Partnern, benutzerdefinierte Benutzererlebnisse zu erstellen. Diese Tools steigern die Effizienz, bieten nahtlose, vernetzte Erlebnisse und verbessern die Benutzerzufriedenheit erheblich und helfen Unternehmen, ihre einzigartige Vision zu verwirklichen.

Ohne Workfront UI-Erweiterungen muss ein Projektmanager beispielsweise möglicherweise zwischen Workfront und einem separaten Zeitverfolgungssystem wechseln, um Stunden zu protokollieren. Mit Benutzeroberflächenerweiterungen kann die Zeitverfolgung direkt in das Workfront-Erlebnis integriert werden, was den Workflow optimiert und Zeit spart. Darüber hinaus können Sie benutzerdefinierte Komponenten hinzufügen, um die Benutzerfreundlichkeit zu verbessern, sich wiederholende Aufgaben zu automatisieren und das Content-Management mit Funktionen wie Metadaten-Tagging und Inhaltsvorschauen zu verbessern. Adobe App Builder bietet außerdem Skalierbarkeit und robustes Identity Management (IMS), sodass eine sichere und effiziente Anpassung in jedem Maßstab gewährleistet ist.

Erweiterungen der Workfront-Benutzeroberfläche bieten mehrere wichtige Vorteile:

* Präzise Anpassung: Standardmäßige Software-Schnittstellen erfüllen häufig nicht alle Geschäftsanforderungen. Benutzeroberflächenerweiterungen ermöglichen es Entwicklerinnen und Entwicklern, die Standardbenutzeroberfläche zu ändern und zu erweitern, um bestimmte Geschäftsanforderungen zu erfüllen.
* Systemintegration: Benutzeroberflächenerweiterungen erleichtern die Integration anderer Systeme und gewährleisten so nahtlose Workflows und Datenkonsistenz.
* Skalierbarkeit: Wenn Unternehmen wachsen, können Benutzeroberflächenerweiterungen entwickelt werden, um neue Funktionen hinzuzufügen, ohne dass das System komplett überholt werden muss.
* Verkürzte Entwicklungszeit: Vorkonfigurierte Erweiterungspunkte und Tools reduzieren den Zeit- und Arbeitsaufwand für die Implementierung benutzerdefinierter Funktionen erheblich.
* Verbesserte Benutzerakzeptanz: Ein optimiertes Benutzererlebnis kann die Softwareakzeptanz erheblich steigern. Benutzerdefinierte Benutzeroberflächenelemente, die auf die Benutzerpräferenzen abgestimmt sind, können die Akzeptanzraten und die allgemeine Zufriedenheit verbessern.
* Mithilfe von Workfront UI-Erweiterungen können Unternehmen maßgeschneiderte Benutzererlebnisse erstellen, die die Effizienz, Integration und Benutzerzufriedenheit steigern.

Nachdem eine Anwendung in der Adobe App Builder erstellt wurde, kann sie ein Workfront-Administrator mithilfe von Layout-Vorlagen dem Workfront-Hauptmenü und dem linken Navigationsbereich hinzufügen. Wenn ein(e) Benutzende(r) mit der Layout-Vorlage auf das Programm klickt, wird das Programm in Workfront eingebettet, anstatt es separat öffnen zu müssen.

In diesem Artikel wird beschrieben, wie Sie auf die App Builder zugreifen und eine Vorlage verwenden können, um eine Anwendung zu erstellen.

Informationen zum Hinzufügen einer benutzerdefinierten Anwendung zu Layout-Vorlagen finden Sie unter [Anpassen des Hauptmenüs mithilfe einer Layout-Vorlage](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md) und [Anpassen des linken Bereichs mithilfe einer Layout-Vorlage](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-left-panel.md).

## Voraussetzungen

Sie müssen über Folgendes verfügen:

* Ein IMS-aktiviertes Workfront-Konto
* Ein Entwicklungsrechner mit Knoten v18 und npm
* App Builder-Lizenz

## Zugriff auf Adobe App Builder

Um Benutzeroberflächenerweiterungen zu erstellen, benötigen Sie Zugriff auf Adobe App Builder in der Adobe Developer Console.

Weitere Anweisungen finden Sie auf der [Adobe Developer-Site](https://developer.adobe.com/uix/docs/guides/get-access/).

### Hinzufügen von Entwicklern zur Adobe Admin Console

>[!IMPORTANT]
>
>Stellen Sie sicher, dass Sie für alle folgenden Schritte die richtige IMS-Organisation ausgewählt haben. Wenn Sie mehreren Organisationen angehören, können Sie die falsche auswählen. Stellen Sie sicher, dass Sie unter der rechten Organisation handeln, die normalerweise oben rechts aufgeführt ist.

1. Navigieren Sie zur Produktion: https://adminconsole.adobe.com/

1. Klicken **Abschnitt „Benutzer** auf **Entwickler** > **Entwickler hinzufügen**.

   ![Benutzer in der Admin Console hinzufügen](assets/manage-users-admin-console.png)

   >[!NOTE]
   >
   >Wenn keine Option zum Verwalten von Entwicklern angezeigt wird, verfügen Sie über kein Produkt, das Entwicklerzugriff ermöglicht.

1. Fügen Sie die E-Mail des Benutzers hinzu. Sie sollte nach vorhandenen Benutzern suchen, die bereits in der Admin Console hinzugefügt wurden.

1. Fügen Sie die erforderlichen Produkte zum Entwicklerprofil hinzu und klicken Sie auf **Speichern**.\
   ![Entwickler hinzufügen](assets/add-developer.png)

### Zugriff auf App Builder erhalten

Unternehmen müssen beim Kauf von App Builder mit ihren Account Managern zusammenarbeiten.

Wenn AppBuilder ordnungsgemäß konfiguriert ist, sollte beim Erstellen eines neuen Projekts „Projekt aus Vorlage erstellen“ angezeigt werden.

## Erstellen eines neuen Projekts in der Adobe Developer Console

Sie müssen die Adobe Developer Console verwenden, um Ihre Benutzeroberflächenerweiterung zu erstellen.

Weitere Anweisungen finden Sie auf der [Adobe Developer-Site](https://developer.adobe.com/uix/docs/guides/creating-project-in-dev-console/).

1. Melden Sie sich mit Ihrer Adobe ID bei der Adobe Developer Console an.

1. Wählen Sie Ihr -Konto und Ihr Profil oder Ihre Organisation aus.

1. Klicken Sie **Schnellstartbereich auf** Projekt aus Vorlage erstellen“ oder klicken Sie auf **Neues Projekt erstellen > Projekt aus Vorlage**.

   >[!IMPORTANT]
   >
   >Wenn Sie die Option zum Erstellen eines Projekts über eine Vorlage nicht sehen, sind Sie in der Admin Console falsch konfiguriert und haben keinen Zugriff auf den App Builder-Katalog. Diese Option wird nur angezeigt, wenn Sie Zugriff auf AppBuilder haben.

   ![Aus Vorlage erstellen](assets/create-from-template.png)

1. **App Builder**.

1. Geben Sie einen **Projekttitel** und **App-Namen** ein. Beide verfügen über Standardwerte, aber es ist später einfacher, das gewünschte Projekt zu identifizieren, wenn Sie den Wert anpassen.

1. Lassen Sie **Laufzeit**.

1. Klicken Sie auf **Speichern**.

## Verwenden der Adobe IO (AIO)-CLI

Adobe bietet eine Open-Source-CLI, mit der Sie das App Builder-Programm erstellen können.

Weitere Anweisungen finden Sie auf GitHub und der Adobe Developer-Site:

* https://github.com/adobe/aio-cli
* https://developer.adobe.com/app-builder/docs/getting_started/first_app/

1. Um das Tool zu installieren (stellen Sie sicher, dass Sie sich zuerst auf dem Knoten 18 befinden), führen Sie `npm install -g @adobe/aio-cli` aus.
1. Starten Sie Ihr Terminal und melden Sie sich mit dem Befehl `aio login` bei der Organisation an. Wenn Sie Probleme haben, sich bei der richtigen IMS-Organisation anzumelden, versuchen Sie `aio login -f`, eine Eingabeaufforderung zu erzwingen. Verwenden Sie `aio where`, um anzuzeigen, welche Organisation Sie bei der richtigen IMS-Organisation angemeldet sind. Weitere Informationen finden Sie unter `aio config`.
1. Beginnen Sie mit der Einrichtung Ihrer App, indem Sie ausführen: `aio app init example-app` Sie sicher, dass Sie „example-app“ durch Ihren App-Namen ersetzen. Wenn Sie sich nicht sicher sind, wie die App-Namen lauten, wird eine Liste der App-Namen mit dem `aio console project list` angezeigt.
1. Wählen Sie Ihre Organisation und Ihr Projekt aus den bereitgestellten Optionen aus.
   ![Befehlsergebnis](assets/1-command-result.png)
   ![Projekt auswählen](assets/2-select-a-project.png)

1. Durchsuchen Sie alle verfügbaren Vorlagen und wählen Sie die **@adobe/workfront-ui-ext-tpl** für Ihr Projekt aus.
   ![Wählen Sie eine Vorlage](assets/3-choose-template.png)
1. Wählen Sie den Projektnamen aus, den Sie in der Adobe Developer Console erstellt haben, und geben Sie ihn ein.
   ![Projektname auswählen und eingeben](assets/4-select-and-enter-project-name.png)

1. Beantworten Sie die Eingabeaufforderungen für die Anwendung:

   * Benennen Sie die Erweiterung.
   * Geben Sie eine beschreibende Zusammenfassung der Funktionalität der Erweiterung an.
   * Wählen Sie eine anfängliche Versionsnummer aus, mit der Sie beginnen möchten.
   * Die Vorlage erstellt den Code für eine primäre Navigationsschaltfläche, wenn Sie die Option „Benutzerdefinierte Schaltfläche zum Hauptmenüelement hinzufügen“ auswählen, wenn Sie nach der Frage „Was möchten Sie als Nächstes tun?“ gefragt werden.

   ![Wählen Sie „Fertig“](assets/5-select-done.png)

1. Bestätigen Sie den Abschluss, indem Sie Ich bin fertig wählen. Die Code-Generierung aus der Vorlage ist in Bearbeitung.
   ![Generierung läuft](assets/6-generation-in-process.png)
1. Warten Sie, bis eine Meldung angezeigt wird, dass die App-Initialisierung abgeschlossen ist. Anschließend können Sie das Projekt in einer IDE öffnen (Visual Studio Code wird empfohlen) und auf den src-Ordner zugreifen.

   Weitere Informationen zu den Ordnern und Dateien in Ihrem Projekt finden Sie auf der [Adobe Developer Site](https://developer.adobe.com/app-builder/docs/getting_started/first_app/#5-anatomy-of-an-appbuilder-application).

## Erstellen der Erweiterungen in VSCode

Die Dateikonfiguration App.js ist erforderlich, um die Navigation über das Workfront-Hauptmenü oder die sekundäre Navigation (linker Bereich) zu aktivieren.

Die Dateikonfiguration extensionRegistration.js ist erforderlich, um die Erweiterungen in Workfront-Layout-Vorlagen anzuzeigen.

Die folgenden Beispiele zeigen, wie Sie dem Workfront-Hauptmenü und dem linken Bedienfeld eines Objekts mithilfe der Benutzeroberflächenerweiterungen benutzerdefinierte Programme hinzufügen.

### Konfigurieren von ExtensionRegistration.js

So lassen Sie benutzerdefinierte Anwendungen im Hauptmenü von Workfront zu:

1. Gehen Sie zu ExtensionRegistration.js.

In der Funktion ExtensionRegistration sollte der folgende Code angezeigt werden. Dieser Code wurde von der Vorlage für Sie erstellt. Dieser Code kann hinzugefügt werden, um zusätzliche Menüelemente zu erstellen. Ersetzen Sie unbedingt die IDs und URLs.

    &quot;
    mainMenu: &lbrace;
    
    getItems() &lbrace;
    
    return &lbrack;
    
    &lbrace;
    
    id: &#39;main-menu-label&#39;,
    
    url: &#39;/index.html#/main-menu-label&#39;,
    
    label: &#39;main menu label&#39;,
    
    icon: icon1,
    
    &rbrace;,
    
    &rbrack;;
    
    &rbrace;,
    
    &rbrace;
    &quot;

1. Fügen Sie das folgende Codefragment hinzu:
   ![Code-](assets/7-extension-registration-step1-from-sam.png)
Dieses Beispiel zeigt ein Hauptmenüelement. Sie müssen die ID, die Bezeichnung, das Symbol und die URL auf die richtigen Namen für Ihr Programm aktualisieren. Stellen Sie beim Hinzufügen mehrerer Elemente sicher, dass die ID eindeutig ist.

1. Speichern Sie Ihre Arbeit.

### Zulassen von benutzerdefinierten Programmen in der Navigation im linken Bereich von Workfront

So lassen Sie benutzerdefinierte Programme im Navigationsbereich des linken Workfront-Bereichs zu:

1. Gehen Sie zu ExtensionRegistration.js.
1. Fügen Sie in der Funktion ExtensionRegistration das folgende Codefragment hinzu:

   ```
   secondaryNav: {  
   
   TASK: {  
   
       getItems() {       return [         {           id: "TASK", 
   
   label: "My TASK",           icon: metricsIcon,           url: "/myTask",  
   
           },  
   
       ];  
   
       },  
   
   },  
   
   },  
   ```

   ![Registrierung der Erweiterung](assets/8-extension-registration-file-step2.png)

   * Dieses Beispiel zeigt ein Navigationselement des linken Bedienfelds namens „Meine Aufgabe“. Sie müssen die ID, die Bezeichnung, das Symbol und die URL auf die richtigen Namen für Ihr Programm aktualisieren.

   * Dieses Beispiel zeigt ein Navigationselement des linken Bedienfelds für den Projektobjekttyp. Sie müssen diese Elemente für jedes Objekt, in dem sie in Workfront unterstützt werden, separat erstellen. Die folgenden Objekte sind verfügbar: Projekt, Aufgabe, Problem, Portfolio und Programm.

1. Speichern Sie Ihre Arbeit.

### Konfigurieren von App.js

1. Wechseln Sie zu App.js.

1. Die Vorlage zeigt eine Route für eine Hauptmenüoption an. Eine Route definiert die Zuordnung zwischen URL-Pfaden und den für diese Pfade gerenderten Komponenten. Um eine Route hinzuzufügen, verwenden Sie das folgende Codefragment. Ersetzen Sie unbedingt den genauen Pfad und das Element durch Ihres.

   ```
       <Route 
   
               exact path="custom-application" 
   
               element={<Customapplication />} 
   
           /> 
   ```

   ![Code-Beispiel](assets/9-app-file-step-1-from-sam.png)
1. Speichern Sie Ihre Arbeit.

Weitere Informationen zum Entwickeln und Ausführen der Anwendung finden Sie auf der [Adobe Developer Site](https://developer.adobe.com/app-builder/docs/getting_started/first_app/#6developing-the-application).

## Freigegebener Kontext

Freigegebener Kontext wird verwendet, um Daten aus Workfront für eine Benutzeroberflächenerweiterung freizugeben. Zu den über Shared Context verfügbaren Daten gehören Benutzerdaten und der Anwendungskontext.


### Benutzerin oder Benutzer

Benutzeroberflächenerweiterungen von Workfront nutzen Benutzerdaten gemeinsam. Das über den freigegebenen Kontext verfügbare Benutzerobjekt enthält eine Workfront-Benutzer-ID und die E-Mail-Adresse des Benutzers.

`user = (conn?.sharedContext?.get("user")); // {ID: '1', email: 'test@aaa.com'} userID = user.ID userEmail = user.email `

### Anwendungskontext

Beim Hinzufügen einer benutzerdefinierten Anwendung mit einem Sekundären Navigationserweiterungspunkt verwendet die benutzerdefinierte Anwendung häufig Kontextdaten wie eine Projekt-ID oder Dokument-ID. Für diese Daten enthält der freigegebene Kontext einen Objekt-Code und eine Objekt-ID.

Im Folgenden finden Sie ein Beispiel für das Abrufen des Anwendungskontexts für Dokumente:

`context = conn?.sharedContext; // Using the connection created above, grab the document details from the host tunnel. // conn?.host?.document?.getDocumentDetails().then(setDocDetails); `

## Testen der App in Workfront

Beim Entwickeln Ihres App Builder-Programms für Workfront müssen Sie Ihr Programm möglicherweise in Workfront testen, ohne es zu veröffentlichen.

Innerhalb Ihrer App Builder-App können Sie `aio app run` für die lokale Entwicklung initiieren. Dadurch erhalten Sie eine URL, normalerweise `https://localhost:9080`. Alternativ können Sie `aio app deploy` ausführen, um eine statische Adobe-Domain abzurufen. Notieren Sie sich diese URLs für die zukünftige Verwendung.

Navigieren Sie dann in Ihrem Browser zu der Seite, für die Sie eine Entwicklung durchführen möchten. Öffnen Sie die Entwickler-Tools und greifen Sie auf den lokalen Speicher für workfront.com oder workfront.adobe.com zu. Hier müssen Sie einen Eintrag hinzufügen. Verwenden Sie `extensionOverride` als Schlüssel und die zuvor erwähnte App Builder-URL als Wert.

Wenn die Konfiguration korrekt abgeschlossen wurde, werden beim Neuladen der Layoutvorlagenseite in Workfront die Schaltflächen in Ihrem App Builder-Programm angezeigt. Fügen Sie die App-Schaltflächen zum Hauptmenü und zum linken Bedienfeld für ein Objekt hinzu und überprüfen Sie, ob sie in diesen Bereichen korrekt angezeigt werden.

Weitere Anweisungen finden Sie auf der Adobe Developer-Site, unter Verwendung eines Beispiels aus AEM: https://developer.adobe.com/uix/docs/guides/preview-extension-locally/

## Anträge veröffentlichen und Einreichung genehmigen

Um das Programm zu veröffentlichen und zu genehmigen, folgen Sie den Anweisungen auf der [Adobe Developer Site](https://developer.adobe.com/uix/docs/guides/publication/).
