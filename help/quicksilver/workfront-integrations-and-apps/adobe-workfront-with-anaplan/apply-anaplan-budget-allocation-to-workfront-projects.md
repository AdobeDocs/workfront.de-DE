---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-with-anaplan
title: 'Anwenden  [!DNL Anaplan]  Budgetzuweisung auf ein  [!DNL Adobe Workfront] '
description: In diesem Integrationsszenario werden alle Budgetzuweisungen synchronisiert, die  [!DNL Anaplan]  vorgenommen wurden [!DNL Workfront]. Das Szenario ruft alle verknüpften Kampagnenbudgetposten ab und übergibt dann den budgetierten Wert an das verknüpfte Workfront-Projekt, wenn der Budgetwert geändert wurde.
author: Becky
feature: Workfront Integrations and Apps, Workfront Fusion
exl-id: 9b8add8f-1978-4ab4-87ac-f1159e7d6cbb
source-git-commit: d3f234313677d916318c181c91cb951948454006
workflow-type: tm+mt
source-wordcount: '731'
ht-degree: 0%

---

# [!DNL Anaplan] Budgetzuweisung auf ein [!DNL Adobe Workfront] Projekt anwenden

Dieses Integrationsszenario synchronisiert alle Budgetzuweisungen, die in [!DNL Anaplan] vorgenommen wurden, mit [!DNL Workfront]. Das Szenario ruft alle verknüpften Kampagnenbudgetposten ab und übergibt dann den budgetierten Wert an das verknüpfte [!DNL Workfront]-Projekt, wenn der Budgetwert geändert wurde.

>[!IMPORTANT]
>
>„Kampagne“ in diesem Artikel bezieht sich auf den Anwendungsfall der Marketing-Kampagne, den dieses Szenario darstellt, und ist in keiner Weise mit dem [!DNL Workfront Fusion] Adobe Campaign-Connector oder dem kürzlich veralteten Objekt [!UICONTROL Kampagne] in [!DNL Workfront] verbunden.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Paket</td> 
   <td> <p>Jedes Adobe Workfront-Workflow-Paket und jedes Adobe Workfront-Automatisierungs- und Integrationspaket</p><p>Workfront Ultimate</p><p>Workfront Prime und Select-Pakete, mit einem zusätzlichen Kauf von Workfront Fusion.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Adobe Workfront-Lizenzen</td> 
   <td> <p>Standard</p><p>Arbeit oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront Fusion-Lizenz</td> 
   <td>
   <p>Betriebsbasiert: Keine Workfront Fusion-Lizenzanforderung</p>
   <p>Connector-basiert (veraltet): Workfront Fusion for Work Automation and Integration </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>
   <p>Wenn Ihr Unternehmen über ein Select- oder Prime Workfront-Paket verfügt, das keine Workfront-Automatisierung und -Integration enthält, muss Ihr Unternehmen Adobe Workfront Fusion erwerben.</li></ul>
   </td> 
  </tr>
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

Informationen zu Adobe Workfront Fusion-Lizenzen finden Sie unter [Adobe Workfront Fusion-Lizenzen](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/set-up-and-manage-fusion/licensing-and-operations-overviews/license-automation-vs-integration).

## Auslösendes Ereignis

Dieses Szenario ist so geplant, dass es alle 15 Minuten ausgeführt wird.

## Erwartete [!DNL Workfront]

Sie müssen über Folgendes verfügen, [!DNL Workfront] dieses Szenario verwenden zu können:

* Ein Benutzerprofil in [!DNL Workfront] mit dem Namen **Anaplan-Integration**, das über Systemadministratorrechte verfügt.

  Informationen zum Erstellen eines Benutzers in [!DNL Workfront] finden Sie unter [Benutzer hinzufügen](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

## Erwartete [!DNL Anaplan]

Sie müssen über Folgendes verfügen, [!DNL Anaplan] dieses Szenario verwenden zu können:

* Ein Benutzerprofil in [!DNL Anaplan] mit dem Namen **[!DNL Workfront]Integration**, das über Systemadministratorrechte verfügt.
* Das [!DNL Anaplan], das Sie für dieses Szenario verwenden möchten.
* Die Liste innerhalb des [!DNL Anaplan], das Kampagnenbudgets erfasst.

  Das -Modul der Liste muss den Empfang der folgenden Attribute unterstützen:

   * [!UICONTROL Workfront-Projekt-GUID]
   * [!UICONTROL Kampagnenname]
   * [!UICONTROL Beantragte Arbeitsmittel]
   * [!UICONTROL Geschätzte Einnahmen]
   * [!UICONTROL Marke]

  Diese Liste und dieses Modul müssen zusätzliche Details speichern, die für die normale Funktionalität von [!DNL Anaplan] erforderlich sind, einschließlich der Möglichkeit, ein Budget festzulegen und mitzuteilen, dass das Budgetlistenelement bereit ist, wieder mit [!DNL Workfront] synchronisiert zu werden.

* Eine Ansicht in [!DNL Anaplan] mit dem Namen **[!UICONTROL Kampagnen.Kampagnen aktualisieren in Adobe Workfront]**.

  Diese Ansicht muss die folgenden Spalten in dieser Reihenfolge enthalten:

   1. [!UICONTROL Elementname]

   2. [!UICONTROL [!DNL Workfront] Projekt-GUID]

   3. [!UICONTROL Kampagnenname]

   4. [!UICONTROL Budget]

   5. [!UICONTROL Geschätzte Einnahmen]

   6. [!UICONTROL Marke]

  Die Ansicht sollte so gefiltert werden, dass Elemente mit einer [!UICONTROL [!DNL Workfront] Projekt-GUID &#x200B;] einige Indikatoren angezeigt werden, die darauf hinweisen, dass Budgetzuweisungen an [!DNL Workfront] übermittelt werden sollen.

Anweisungen zu diesen Aktionen finden Sie in der [!DNL Anaplan]-Dokumentation.

## Bereitstellen für [!DNL Workfront Fusion]

Führen Sie die folgenden Schritte aus, um dieses Integrationsszenario in Ihrem [!DNL Fusion]-Konto bereitzustellen. Dies sollte erst nach Abschluss der erforderlichen [!DNL Workfront]- und [!DNL Anaplan]-Konfiguration erfolgen.

1. Navigieren Sie zum Menü [!UICONTROL Vorlagen] in [!DNL Workfront Fusion] und klicken Sie auf die **[!UICONTROL Anwenden [!DNL Anaplan] Budgetzuweisungen auf Workfront-Projekte]** Szenariovorlage.
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
      <td role="rowheader">[!UICONTROL [!DNL Anaplan] Modulname]</td> 
      <td>Der Name des Moduls, das die Kampagnenattribute in der ausgewählten [!DNL Anaplan] beschreibt.</td> 
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
1. Fügen Sie **[!UICONTROL Modul „CSV in JSON-Objekt]**&quot; eine neue Datenstruktur hinzu, um die CSV-Spalten einem verwendbaren JSON-Objekt zuzuordnen.

   <!-- [Copy](javascript:void(0);) -->
   <pre><code>[<br>    {<br>        "Anaplan Name":"text",<br>        "Workfront Project GUID":"text",<br>        "Campaign Name":"text",<br>        "Budget": 100.01,<br>        "Estimated Revenue": 100.01,<br>        "Brand":"text"<br>    }<br>]<br></code></pre>

1. Wählen Sie bei Aufforderung diese Datenstruktur für andere Module in dieser Bereitstellungsszenario aus.
1. Wählen **[!UICONTROL im Modul]** Projekt überprüfen ein [!DNL Workfront] Verbindungsprofil aus oder fügen Sie es hinzu.
1. Aktualisieren Sie alle verbleibenden [!DNL Workfront]-Module mit einer [!DNL Workfront] Verbindung, wenn Sie dazu aufgefordert werden.

## Andere empfohlene Szenariovorlagen

Um den durch diese Vorlage dargestellten Workflow abzuschließen, müssen Sie auch die folgende zusätzliche Vorlage bereitstellen:

* [[!UICONTROL Erstellen eines  [!DNL Anaplan] -Listenelements aus einer  [!DNL Adobe Workfront] -Anfrage]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-budget-request.md)

Weitere Szenarien für die Ausgabenoptimierung sind:

* [[!UICONTROL Projektaktualisierungen  [!DNL Adobe Workfront]  ein  [!DNL Anaplan]  senden]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-updates-to-anaplan-list-item.md)

* [[!UICONTROL Senden von  [!DNL Adobe Workfront] -Stunden-Aktualisierungen an ein  [!DNL Anaplan] -Element]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-actual-hours-updates-to-anaplan-list-item.md)

* [[!UICONTROL Senden [!DNL Adobe Workfront] Ausgaben an  [!DNL Anaplan] /Listenelement]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-expenses-to-anaplan-list-item.md)
