---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-with-anaplan
title: Projektaktualisierungen  [!DNL Adobe Workfront]  ein  [!DNL Anaplan]  senden
description: Dieses Integrationsszenario teilt den Fortschritt, den Status und die wichtigsten Zeitplandetails aus einem  [!DNL Adobe Workfront]  mit  [!DNL Anaplan]  Budgetlistenelement. Durch die Weitergabe dieser Informationen können Sie die Ausgabenoptimierung und die Finanzanalyse, die  [!DNL Anaplan]  bietet, besser nutzen.
author: Becky
feature: Workfront Integrations and Apps, Workfront Fusion
exl-id: 97e9dac6-f5b5-4d6e-b58b-93acd19048ee
source-git-commit: d3f234313677d916318c181c91cb951948454006
workflow-type: tm+mt
source-wordcount: '963'
ht-degree: 1%

---

# Senden [!DNL Adobe Workfront] Projektaktualisierungen an ein [!DNL Anaplan] Listenelement

Dieses Integrationsszenario teilt den Fortschritt, den Status und die wichtigsten Zeitplandetails aus einem [!DNL Adobe Workfront] mit einem [!DNL Anaplan] Budgetlistenelement. Durch die Weitergabe dieser Informationen können Sie die von [!DNL Anaplan] bereitgestellten Funktionen zur Ausgabenoptimierung und Finanzanalyse besser nutzen.

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

Informationen zu Adobe Workfront Fusion-Lizenzen finden Sie unter [Adobe Workfront Fusion-Lizenzen](https://experienceleague.adobe.com/de/docs/workfront-fusion/using/set-up-and-manage-fusion/licensing-and-operations-overviews/license-automation-vs-integration).

## Auslösendes Ereignis

Dieses Szenario ist so geplant, dass es alle 15 Minuten ausgeführt wird.

## Erwartete [!DNL Workfront]

Sie müssen über Folgendes verfügen, [!DNL Workfront] dieses Szenario verwenden zu können:

* Ein Benutzerprofil in [!DNL Workfront] mit dem Namen **[!UICONTROL [!DNL Anaplan]Integration]**, das über Systemadministratorrechte verfügt.

  Informationen zum Erstellen eines Benutzers in [!DNL Workfront] finden Sie unter [Benutzer hinzufügen](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

* Ein **[!UICONTROL Kampagnenübersicht]** benutzerdefiniertes Formular, das an das Projektobjekt angehängt ist, um benutzerdefinierte Datenwerte zu speichern, die Sie an Anaplan senden möchten.

  Die folgenden Felder stellen Beispiele für Felder dar, die im benutzerdefinierten Formular enthalten sein können, um die Datenzuordnung zu Anaplan zu unterstützen, sie sind jedoch für dieses Integrationsszenario nicht erforderlich:

  <table style="table-layout:auto"> 
   <col> 
   <col> 
   <thead> 
    <tr> 
     <th>Feldname</th> 
     <th>Feldtyp</th> 
    </tr> 
   </thead> 
   <tbody> 
    <tr> 
     <td role="rowheader">[!UICONTROL in Market Start Date]</td> 
     <td>[!UICONTROL Datum] </td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL in Market End Date]</td> 
     <td>[!UICONTROL Datum]</td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL Kampagnenübersicht]</td> 
     <td>[!UICONTROL Absatztextfeld]</td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL Schlüsselmeldung]</td> 
     <td>[!UICONTROL Absatztextfeld]</td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL Zielgruppe]</td> 
     <td> <p>[!UICONTROL Dropdown]</p> <p>Optionen einschließen, die zu Ihren Prozessen passen.</p> </td> 
    </tr> 
   </tbody> 
  </table>

  Informationen zum Erstellen benutzerdefinierter Formulare finden Sie unter [Erstellen eines benutzerdefinierten Formulars](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

<!--
<note type="note">  
<p>The above configuration is available through the Marketing Financial Management Configuration blueprint:</p>
<p>https://MYDOMAIN.my.workfront.com/blueprints/7ebe85c4-05a1-4efe-a018-50ee55f5654c/details </p>
<p><span style="color: #ff0000;">This note is currently not marked for publication.</span> </p>
</note>
-->

## Erwartete [!DNL Anaplan]

Sie müssen über Folgendes verfügen, [!DNL Anaplan] dieses Szenario verwenden zu können:

* Ein Benutzerprofil in [!DNL Anaplan] mit dem Namen **[!UICONTROL [!DNL Workfront]Integration]**, das über Systemadministratorrechte verfügt.
* Das [!DNL Anaplan], das Sie für dieses Szenario verwenden möchten.
* Die Liste innerhalb des [!DNL Anaplan], die Sie für dieses Szenario verwenden möchten.
* Eine **[!UICONTROL Projektaktualisierungs-Import]**-Datei, die die folgenden Spalten in dieser Reihenfolge enthält:

1. [!UICONTROL itemID]

2. [!UICONTROL [!DNL Workfront] Projekt-GUID]

3. [!UICONTROL Kampagnenname]

4. [!UICONTROL Prozent abgeschlossen]

5. [!UICONTROL Geplantes Startdatum]

6. [!UICONTROL Geplantes Abschlussdatum]

7. [!UICONTROL Geplante Stunden]

8. [!UICONTROL Geplante Kosten]

9. [!UICONTROL Geplante Ausgabenkosten]

10. [!UICONTROL Ist-Lohnkosten]

11. [!UICONTROL Geplante Arbeitskosten]

12. [!UICONTROL Status]

So bereiten Sie die [!UICONTROL [!DNL Anaplan] Importdatei für geplante &#x200B;] vor:

1. Folgendes kopieren und in einen Texteditor oder [!DNL Excel] einfügen
1. Speichern Sie die Datei im CSV-Format
1. Laden Sie die Datei in Anaplan hoch.

   Anweisungen finden Sie in der [!DNL Anaplan] Dokumentation zum Importieren von Daten aus einer Datei in -Module.

1. Notieren Sie sich den Namen, den Sie der Datei gegeben haben. Er wird während der Bereitstellung der Szenariovorlage [!UICONTROL Fusion] verwendet.

Beispiel für CSV-Inhalte

<!-- [Copy](javascript:void(0);) -->
<pre><code>"itemID","Workfront Project GUID","Campaign Name","Percent Complete","Planned Start Date","Planned Completion Date","Planned Hours","Planned Cost","Planned Expense Cost","Actual Labor Cost","Planned Labor Cost","Status","Campaign Overview","Key Message","In Market Start Date","In Market End Date","Target Audience"<br>"202000001019","6182bc1f0025e184b2c00d9205e22c49","Launch Be U APAC Styles Catalog","0","2022-03-31","2022-05-31","88.25","0","0","0","0","Planning","","","","",""</code></pre>Optionale Spalten können Folgendes enthalten:

1. [!UICONTROL Kampagnenübersicht]

2. [!UICONTROL Schlüsselbotschaft]

3. [!UICONTROL In Markt Startdatum]

4. [!UICONTROL Marktenddatum]

5. [!UICONTROL Zielgruppe]

Schließen Sie auch alle anderen Felder ein, die Sie in der Zuordnung festlegen möchten.

* Ein **[!UICONTROL Import von Projektaktualisierungen]**, der auf den Import von Daten vorbereitet ist, die über einen Datei-Upload bereitgestellt werden.

Anweisungen zu diesen Aktionen finden Sie in der [!DNL Anaplan]-Dokumentation.

## Bereitstellen für [!DNL Workfront Fusion]

Führen Sie die folgenden Schritte aus, um dieses Integrationsszenario in Ihrem Fusion-Konto bereitzustellen. Dies sollte erst nach Abschluss der erforderlichen [!DNL Workfront]- und [!DNL Anaplan]-Konfiguration erfolgen.

1. Navigieren Sie zum Menü [!UICONTROL Vorlagen] in [!DNL Workfront Fusion] und klicken Sie auf die Szenariovorlage **[!UICONTROL Workfront-Projektaktualisierungen an [!DNL Anaplan] Listenelement senden]**.
1. Ersetzen Sie die Variablenwerte für die folgenden [!DNL Anaplan]:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
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
      <td role="rowheader">[!UICONTROL Dateiname: Projektaktualisierungs-Import]</td> 
      <td>Der Name der Datei, die Projektaktualisierungsdaten erhält.<p>(Beispiel: WorkfrontUpdateLinkedProject.csv)</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Prozessname: Projektaktualisierungs-Import]</td> 
      <td> <p>Der Name des Prozesses, der den Import von Projektdaten ausführt.</p> <p>(Beispiel: WF int - Kampagnendetails aktualisieren)</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL Workfront] Subdomain]</td> 
      <td>Die Subdomain Ihres [!DNL Workfront]. Auf diese Weise wird in einer eventuell generierten Anmerkung ein Link zurück zu Ihrem [!DNL Workfront]-Projekt erstellt.</td> 
     </tr> 
    </tbody> 
   </table>

   Einzelheiten zum Einrichten der Dateien und Prozesse finden Sie in der Dokumentation zur [!DNL Anaplan].

1. Wählen Sie ein [!DNL Anaplan] Verbindungsprofil aus oder fügen Sie es hinzu.
1. Aktualisieren Sie alle verbleibenden [!DNL Anaplan]-Module mit einer [!DNL Anaplan] Verbindung, wenn Sie dazu aufgefordert werden.
1. Wählen Sie ein [!DNL Workfront] Verbindungsprofil aus oder fügen Sie es hinzu.

   Der Filter ist so konfiguriert, dass er alle unvollständigen verknüpften Projekte und die Projekte abruft, die in den letzten 29 Minuten abgeschlossen wurden. Wenn Sie die Häufigkeit des [!DNL Fusion] ändern, sollten Sie diesen Wert nach der Bereitstellung der Szenariovorlage aktualisieren.

1. Fügen Sie im **[!UICONTROL Build Projects Update CSV]**-Modul eine neue Datenstruktur hinzu, um die Projektattribute CSV-Spalten zuzuordnen.

   <!-- [Copy](javascript:void(0);) -->
   <pre><code>[<br>    {<br>        "itemID": 1000001,<br>        "Workfront Project GUID":"text",<br>        "Campaign Name":"text",<br>        "Percent Complete": 10.01,<br>        "Planned Start Date":"2022-02-22",<br>        "Planned Completion Date":"2022-02-22",<br>        "Planned Hours": 12.5,<br>        "Planned Cost": 123.45,<br>        "Planned Expense Cost": 123.45,<br>        "Planned Labor Cost": 123.45,<br>        "Status": "CUR",<br>        "Campaign Overview":"text",<br>        "Key Message":"text",<br>        "In Market Start Date":"2022-02-22",<br>        "In Market End Date":"2022-02-22",<br>        "Target Audience":"text"<br>    }<br>]<br></code></pre>

1. Aktualisieren Sie alle verbleibenden [!DNL Workfront]-Module mit einer [!DNL Workfront] Verbindung, wenn Sie dazu aufgefordert werden.

## Andere empfohlene Szenariovorlagen

Diese Szenariovorlage wird durch die folgenden Vorlagen für Ausgabenoptimierungsszenarien ergänzt, die ebenfalls bereitgestellt werden können:

* [[!UICONTROL Senden von  [!DNL Adobe Workfront] -Stunden-Aktualisierungen an ein  [!DNL Anaplan] -Element]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-actual-hours-updates-to-anaplan-list-item.md)
* [[!UICONTROL Senden [!DNL Adobe Workfront] Ausgaben an  [!DNL Anaplan] /Listenelement]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-expenses-to-anaplan-list-item.md)

Zusätzliche Szenarien für die Verknüpfung von Budgetanfragen:

* [[!UICONTROL Erstellen eines  [!DNL Anaplan] -Listenelements aus einer  [!DNL Adobe Workfront] -Anfrage]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-budget-request.md)
* [[!UICONTROL Budgetzuweisung  [!DNL Anaplan]  ein Projekt  [!DNL Adobe Workfront] &#x200B;]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-projects.md)

Zusätzliche Szenarien für die Verknüpfung von Kampagnenanfragen:

* [[!UICONTROL Erstellen eines  [!DNL Anaplan] -Listenelements aus einer  [!DNL Adobe Workfront] -Anfrage]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-campaign-request.md)
* [[!UICONTROL Budgetzuweisung  [!DNL Anaplan]  eine Kampagnenanfrage  [!DNL Adobe Workfront]  ein Kampagnenprojekt anwenden]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-campaign-requests-and-projects.md)
