---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-with-anaplan
title: Anwenden  [!DNL Anaplan]  Budgetzuweisung auf eine Kampagnenanfrage  [!DNL Adobe Workfront]  ein Kampagnenprojekt
description: In diesem Integrationsszenario werden alle Budgetzuweisungen synchronisiert, die  [!DNL Anaplan]  vorgenommen wurden [!DNL Workfront]. Das Szenario ruft alle verknüpften Kampagnenbudgetposten ab und übergibt dann den budgetierten Wert an das verknüpfte Workfront-Projekt, wenn der Budgetwert geändert wurde.
author: Becky
feature: Workfront Integrations and Apps, Workfront Fusion
exl-id: 8ae28911-fa18-459a-aa50-cfb347e70e61
source-git-commit: 4ab731b14dc5435386fd0d887501788fa37223a2
workflow-type: tm+mt
source-wordcount: '674'
ht-degree: 0%

---

# Anwenden einer [!DNL Anaplan] Budgetzuweisung auf eine [!DNL Adobe Workfront] Kampagnenanfrage oder ein Kampagnenprojekt

Dieses Integrationsszenario synchronisiert alle Budgetzuweisungen, die in [!DNL Anaplan] vorgenommen wurden, mit [!DNL Workfront]. Das Szenario ruft alle verknüpften Kampagnenbudgetposten ab und übergibt dann den Budgetwert an das verknüpfte [!DNL Workfront]-Projekt, wenn der Budgetwert geändert wurde.

>[!IMPORTANT]
>
>„Kampagne“ in diesem Artikel bezieht sich auf den Anwendungsfall der Marketing-Kampagne, den dieses Szenario darstellt, und ist in keiner Weise mit dem [!DNL Workfront Fusion] Adobe Campaign-Connector oder dem kürzlich veralteten Objekt [!UICONTROL Kampagne] in [!DNL Workfront] verbunden.


## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Funktion in diesem Artikel verwenden zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Plan*</td> 
   <td> <p>[!UICONTROL Pro] oder höher</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] Lizenz*</td> 
   <td> <p>[!UICONTROL-Plan], [!UICONTROL-Arbeit]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] Lizenz **</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] für Arbeitsautomatisierung und -integration] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] erwerben und [!DNL Adobe Workfront], die in diesem Artikel beschriebenen Funktionen zu nutzen.</td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren [!DNL Workfront], um herauszufinden, über welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie verfügen.

&#42;&#42;Informationen zu [!DNL Adobe Workfront Fusion] finden Sie unter [[!DNL Adobe Workfront Fusion] Lizenzen](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Auslösendes Ereignis

Dieses Szenario ist so geplant, dass es alle 15 Minuten ausgeführt wird.

## Erwartete [!DNL Workfront]

Sie müssen über Folgendes verfügen, [!DNL Workfront] dieses Szenario verwenden zu können:

* Ein Benutzerprofil in [!DNL Workfront] mit dem Namen **[!DNL Anaplan Integration]**, das über Systemadministratorrechte verfügt.

  Informationen zum Erstellen eines Benutzers in [!DNL Workfront] finden Sie unter [Benutzer hinzufügen](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

## Erwartete [!DNL Anaplan]

Sie müssen über Folgendes verfügen, [!DNL Anaplan] dieses Szenario verwenden zu können:

* Ein Benutzerprofil in [!DNL Anaplan] mit dem Namen **[!UICONTROL [!DNL Workfront]Integration]**, das über Systemadministratorrechte verfügt.
* Das [!DNL Anaplan], das Sie für dieses Szenario verwenden möchten.
* Die Liste innerhalb des [!DNL Anaplan], das Kampagnenbudgets erfasst.

  Das -Modul der Liste muss den Empfang der folgenden Attribute unterstützen:

   * [!UICONTROL [!DNL Workfront] Anfrage-GUID]
   * [!UICONTROL [!DNL Workfront] Projekt-GUID]
   * [!UICONTROL Kampagnenname]
   * [!UICONTROL Beantragte Arbeitsmittel]
   * [!UICONTROL Geschätzte Einnahmen]
   * [!UICONTROL Marke]

  Diese Liste und dieses Modul müssen zusätzliche Details speichern, die für die normale Funktionalität von [!DNL Anaplan] erforderlich sind, einschließlich der Möglichkeit, ein Budget festzulegen und mitzuteilen, dass das Budgetlistenelement bereit ist, wieder mit [!DNL Workfront] synchronisiert zu werden.

* Eine Ansicht in [!DNL Anaplan] namens **[!UICONTROL Kampagnen.Kampagnen aktualisieren in Adobe Workfront]**.

  Diese Ansicht muss die folgenden Spalten in dieser Reihenfolge enthalten:

   1. [!UICONTROL Elementname]

   2. [!UICONTROL [!DNL Workfront] Anfrage-GUID]

   3. [!UICONTROL [!DNL Workfront] Projekt-GUID]

   4. [!UICONTROL Kampagnenname]

   5. [!UICONTROL Budget]

   6. [!UICONTROL Geschätzte Einnahmen]

   7. [!UICONTROL Marke]

  Die Ansicht sollte so gefiltert werden, dass Elemente mit einer [!UICONTROL [!DNL Workfront] Projekt-GUID ] einige Indikatoren angezeigt werden, die darauf hinweisen, dass Budgetzuweisungen an Workfront übermittelt werden sollen.

Anweisungen zu diesen Aktionen finden Sie in der [!DNL Anaplan]-Dokumentation.

## Bereitstellen in Workfront Fusion

Führen Sie die folgenden Schritte aus, um dieses Integrationsszenario in Ihrem Fusion-Konto bereitzustellen. Dies sollte erst nach Abschluss der erforderlichen [!DNL Workfront]- und [!DNL Anaplan]-Konfiguration erfolgen.

1. Navigieren Sie zum Menü [!UICONTROL Vorlagen] in [!DNL Workfront Fusion] und klicken Sie auf die Szenariovorlage **[!UICONTROL Anwenden [!DNL Anaplan] Budgetzuweisungen auf Workfront-Kampagnenanfragen und -Projekte]**.
1. Ersetzen Sie die Variablenwerte für die folgenden [!DNL Anaplan]:

   <table style="table-layout:auto"> 
    <col> 
    </col> 
    <col> 
    </col> 
    <thead> 
     <tr> 
      <th>Variablenname</th> 
      <th>Wert ersetzen durch</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL Anaplan] Workspace ID]</td> 
      <td>Die ID eines Arbeitsbereichs aus Ihrem [!DNL Anaplan].</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL Anaplan]-Modell-ID] </td> 
      <td>Die ID eines Modells aus Ihrem [!DNL Anaplan] und dem ausgewählten Arbeitsbereich.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Kampagnenlistenname]</td> 
      <td>Der Name der Liste aus Ihrem [!DNL Anaplan] und dem ausgewählten Arbeitsbereich und Modell.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL Anaplan]]</td> 
      <td> <p>Der Name der Ansicht, die Kampagnenbudgets enthält, die zur Übertragung an [!DNL Workfront] bereit sind.</p> <p>(Beispiel: [!UICONTROL CAMPAIGNS.LOAD CAMPAIGNS TO [!DNL Adobe Workfront]]) </p> </td> 
     </tr> 
    </tbody> 
   </table>

   Einzelheiten zum Einrichten der Dateien und Prozesse finden Sie in der Dokumentation zur [!DNL Anaplan].

1. Wählen Sie ein [!DNL Anaplan] Verbindungsprofil aus oder fügen Sie es hinzu.
1. Aktualisieren Sie alle verbleibenden [!DNL Anaplan]-Module mit einer [!DNL Anaplan] Verbindung, wenn Sie dazu aufgefordert werden.
1. Fügen Sie im **[!UICONTROL CSV in JSON-]** konvertieren“ eine neue Datenstruktur hinzu, um die CSV-Spalten einem verwendbaren JSON-Objekt zuzuordnen.

   <!-- [Copy](javascript:void(0);) -->
   <pre><code>[<br>    {<br>        "Anaplan Name":"text",<br>        "Workfront Request GUID":"text",<br>        "Workfront Project GUID":"text",<br>        "Campaign Name":"text",<br>        "Budget": 100.01,<br>        "Estimated Revenue": 100.01,<br>        "Brand":"text"<br>    }<br>]<br></code></pre>

1. Wählen Sie bei Aufforderung diese Datenstruktur für andere Module in dieser Bereitstellungsszenario aus.
1. Wählen **[!UICONTROL im Modul]** Projekt überprüfen ein [!DNL Workfront] Verbindungsprofil aus oder fügen Sie es hinzu.
1. Aktualisieren Sie alle verbleibenden [!DNL Workfront]-Module mit einer [!DNL Workfront] Verbindung, wenn Sie dazu aufgefordert werden.

## Andere empfohlene Szenariovorlagen

Um den durch diese Vorlage dargestellten Workflow abzuschließen, müssen Sie auch die folgende zusätzliche Vorlage bereitstellen:

* [[!UICONTROL Erstellen eines  [!DNL Anaplan] -Listenelements aus einer  [!DNL Adobe Workfront] -Anfrage]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-campaign-request.md)

Weitere Szenarien für die Ausgabenoptimierung sind:

* [[!UICONTROL Projektaktualisierungen  [!DNL Adobe Workfront]  ein  [!DNL Anaplan]  senden]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-updates-to-anaplan-list-item.md)

* [[!UICONTROL Senden von  [!DNL Adobe Workfront] -Stunden-Aktualisierungen an ein  [!DNL Anaplan] -Element]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-actual-hours-updates-to-anaplan-list-item.md)

* [[!UICONTROL Senden [!DNL Adobe Workfront] Ausgaben an  [!DNL Anaplan] /Listenelement]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-expenses-to-anaplan-list-item.md)
