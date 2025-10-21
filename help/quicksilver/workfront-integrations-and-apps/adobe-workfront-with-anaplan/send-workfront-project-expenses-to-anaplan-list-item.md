---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-with-anaplan
title: Senden  [!DNL Adobe Workfront]  Ausgaben an  [!DNL Anaplan]  Listenelement
description: Dieses Integrationsszenario gibt kostenbezogene Details aus einem Projekt  [!DNL Adobe Workfront]  einem  [!DNL Anaplan] -Budgetlistenelement frei. Durch die Weitergabe dieser Informationen können Sie die Ausgabenoptimierung und die Finanzanalyse, die  [!DNL Anaplan]  bietet, besser nutzen.
author: Becky
feature: Workfront Integrations and Apps, Workfront Fusion
exl-id: f9198017-9bbb-4776-86aa-3f78705dbb22
source-git-commit: cd0214917620e0b147d0da3402ea2d34e28bc9c3
workflow-type: tm+mt
source-wordcount: '974'
ht-degree: 1%

---

# Senden [!DNL Adobe Workfront] Ausgaben an ein [!DNL Anaplan] Listenelement

Dieses Integrationsszenario gibt kostenbezogene Details aus einem [!DNL Adobe Workfront] mit einem [!DNL Anaplan] Budgetlistenelement frei. Durch die Weitergabe dieser Informationen können Sie die von [!DNL Anaplan] bereitgestellten Funktionen zur Ausgabenoptimierung und Finanzanalyse besser nutzen.

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

* Ein Benutzerprofil in [!DNL Workfront] mit dem Namen *Anaplan-Integration*, das über Systemadministratorrechte verfügt.

  Informationen zum Erstellen eines Benutzers in [!DNL Workfront] finden Sie unter [Benutzer hinzufügen](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

* Ein **[!UICONTROL Kampagnenübersicht]** benutzerdefiniertes Formular, das an das Projektobjekt angehängt ist, um benutzerdefinierte Datenwerte zu speichern, die Sie an [!DNL Anaplan] senden möchten.

  Das Formular muss die folgenden Felder enthalten:

  | Feldname | Feldtyp |
  |---|---|
  | [!UICONTROL Letztes Übertragungsdatum] | Datum |
  | [!UICONTROL Integrationshinweise] | Absatztextfeld |

  Informationen zum Erstellen benutzerdefinierter Formulare finden Sie unter [Erstellen eines benutzerdefinierten Formulars](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

## Erwartete [!DNL Anaplan]

Sie müssen über Folgendes verfügen, [!DNL Anaplan] dieses Szenario verwenden zu können:

* Ein Benutzerprofil in [!DNL Anaplan] mit dem Namen **[!UICONTROL [!DNL Workfront]Integration]**, das über Systemadministratorrechte verfügt.
* Das [!DNL Anaplan], das Sie für dieses Szenario verwenden möchten.
* Die Liste innerhalb des [!DNL Anaplan], die Kampagnenbudgets erfassen soll.
* Eine **[!UICONTROL Anaplan Actual Expense Import]**-Datei, die die folgenden Spalten in dieser Reihenfolge enthält:

   1. [!UICONTROL [!DNL Workfront] Ausgabe-GUID]

   2. [!UICONTROL [!DNL Workfront] Projekt-GUID]

   3. [!UICONTROL Tatsächlicher Betrag]

   4. [!UICONTROL Beschreibung]

   5. [!UICONTROL Ausgabentyp]

   6. [!UICONTROL Wirksamkeitsdatum]

   7. [!UICONTROL Kampagnenname]

   8. [!UICONTROL [!DNL Anaplan] Listenelement-ID]

  So bereiten Sie die [!UICONTROL [!DNL Anaplan] Actual Expense Import]-Datei vor:

   1. Kopieren Sie Folgendes und fügen Sie es in einen Texteditor oder ein [!DNL Excel] ein.
   1. Speichern Sie die Datei im CSV-Format.
   1. Laden Sie die Datei in [!DNL Anaplan] hoch.

      Anweisungen finden Sie in der [!DNL Anaplan] Dokumentation zum Importieren von Daten aus einer Datei in -Module.

   1. Notieren Sie sich den Namen, den Sie der Datei gegeben haben. Er wird während der Bereitstellung der Szenariovorlage [!UICONTROL Fusion] verwendet.

  Beispiel für CSV-Inhalte

  <!-- [Copy](javascript:void(0);) -->
  <pre><code>"Workfront Expense GUID","Workfront Project GUID","Actual Amount","Description","Expense Type","Effective Date","Campaign Name","Anaplan List Item ID"<br>"622aead400423eb2e4479fece9a72987","6218062a000d0442903fcfa21e11f556","2345","Expense 1","","2022-03-09","New Project 6","202000001030"</code></pre>

* Eine **[!UICONTROL [!DNL Anaplan]Importdatei für geplante Ausgaben]** die die folgenden Spalten in der folgenden Reihenfolge enthält:

   1. [!UICONTROL [!DNL Workfront] Ausgabe-GUID]

   2. [!UICONTROL [!DNL Workfront] Projekt-GUID]

   3. [!UICONTROL Tatsächlicher Betrag]

   4. [!UICONTROL Beschreibung]

   5. [!UICONTROL Ausgabentyp]

   6. [!UICONTROL Wirksamkeitsdatum]

   7. [!UICONTROL Kampagnenname]

   8. [!UICONTROL [!DNL Anaplan] Listenelement-ID]

  So bereiten Sie die [!UICONTROL [!DNL Anaplan] Importdatei für geplante &#x200B;] vor:

   1. Folgendes kopieren und in einen Texteditor oder [!DNL Excel] einfügen
   1. Speichern Sie die Datei im CSV-Format
   1. Laden Sie die Datei in Anaplan hoch.

      Anweisungen finden Sie in der [!DNL Anaplan] Dokumentation zum Importieren von Daten aus einer Datei in -Module.

   1. Notieren Sie sich den Namen, den Sie der Datei gegeben haben. Er wird während der Bereitstellung der Szenariovorlage [!UICONTROL Fusion] verwendet.

  Beispiel für CSV-Inhalte

  <!-- [Copy](javascript:void(0);) -->
  <pre><code>"Workfront Expense GUID","Workfront Project GUID","Planned Amount","Description","Expense Type","Planned Date","Campaign Name","Anaplan List Item ID"<br>"622aead400423eb2e4479fece9a72987","6218062a000d0442903fcfa21e11f556","1234","Expense 1","Entertainment","2022-03-08","New Project 6","202000001030"</code></pre>


* Ein **[!UICONTROL Import von Projektaktualisierungen]**, der auf den Import von Daten vorbereitet ist, die über einen Datei-Upload bereitgestellt werden.

>[!NOTE]
>
>Es gibt separate Importdateien für geplante und tatsächliche Ausgaben, sodass diese unabhängig über das geplante bzw. das Wirksamkeitsdatum gemeldet werden können.

Anweisungen zu diesen Aktionen finden Sie in der [!DNL Anaplan]-Dokumentation.

## Bereitstellen für [!DNL Fusion]

Führen Sie die folgenden Schritte aus, um dieses Integrationsszenario in Ihrem [!DNL Fusion]-Konto bereitzustellen. Dies sollte erst nach Abschluss der erforderlichen [!DNL Workfront]- und [!DNL Anaplan]-Konfiguration erfolgen.

1. Navigieren Sie zum Menü [!UICONTROL Vorlagen] in [!DNL Workfront Fusion] und klicken Sie auf die Szenariovorlage **[!UICONTROL Senden von Workfront-Ausgaben-Updates an [!DNL Anaplan] Listenelement]**.
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
      <td>Die ID des Arbeitsbereichs aus Ihrem [!DNL Anaplan]-Konto, den Sie für dieses Szenario verwenden möchten.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL Anaplan]-Modell-ID] </td> 
      <td>Die ID des Modells aus Ihrem [!DNL Anaplan]-Konto und dem ausgewählten Arbeitsbereich, den Sie für dieses Szenario verwenden möchten.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Kampagnenlistenname]</td> 
      <td>Der Name der Liste aus Ihrem [!DNL Anaplan]-Konto und dem ausgewählten Arbeitsbereich und Modell, die Sie für dieses Szenario verwenden möchten.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Dateiname: Tatsächlicher Kostenimport]</td> 
      <td> <p>Der Name der Datei, die die tatsächlichen Ausgabendaten des Projekts erhält.</p> <p> (Beispiel: WorkfrontUpdateLinkedProjects_ActExpenses.csv) </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Dateiname: Geplanter Kostenimport]</td> 
      <td> <p>Der Name der Datei, die die Daten zu den geplanten Projektausgaben erhält.</p> <p> (Beispiel: WorkfrontUpdateLinkedProjects_PlannedExpenses.csv) </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Prozessname: Projektaktualisierungs-Import]</td> 
      <td> <p>Der Name des Prozesses, der den Import von Projektausgabendaten ausführt.</p> <p>(Beispiel: WF int - Projektausgaben laden)</p> </td> 
     </tr> 
    </tbody> 
   </table>

   Einzelheiten zum Einrichten der Dateien und Prozesse finden Sie in der Dokumentation zur [!DNL Anaplan].

1. Wählen Sie ein [!DNL Anaplan] Verbindungsprofil aus oder fügen Sie es hinzu.
1. Aktualisieren Sie alle verbleibenden [!DNL Anaplan]-Module mit einer [!DNL Anaplan] Verbindung, wenn Sie dazu aufgefordert werden.
1. Wählen Sie ein [!DNL Workfront] Verbindungsprofil aus oder fügen Sie es hinzu.
1. Aktualisieren Sie alle verbleibenden [!DNL Workfront]-Module mit einer [!DNL Workfront] Verbindung, wenn Sie dazu aufgefordert werden.
1. Fügen Sie **[!UICONTROL Modul „Tatsächliche Ausgaben-CSV erstellen]** eine neue Datenstruktur hinzu, um die Projektattribute CSV-Spalten zuzuordnen.

   <!-- [Copy](javascript:void(0);) -->
   <pre><code>[<br>    {<br>        "Workfront Expense GUID":"text",<br>        "Workfront Project GUID":"text",<br>        "Actual Amount": 100.01,<br>        "Description":"text",<br>        "Expense Type":"text",<br>        "Effective Date":"text",<br>        "Campaign Name":"text",<br>        "Anaplan List Item ID": 10000001<br>    }<br>]<br></code></pre>

1. Fügen Sie im **[!UICONTROL CSV für geplante Ausgaben erstellen]** eine neue Datenstruktur hinzu, um die Projektattribute CSV-Spalten zuzuordnen.

   <!-- [Copy](javascript:void(0);) -->
   <pre><code>[<br>    {<br>        "Workfront Expense GUID":"text",<br>        "Workfront Project GUID":"text",<br>        "Planned Amount": 100.01,<br>        "Description":"text",<br>        "Expense Type":"text",<br>        "Planned Date":"text",<br>        "Campaign Name":"text",<br>        "Anaplan List Item ID": 10000001<br>    }<br>]<br></code></pre>

## Andere empfohlene Szenariovorlagen

Diese Szenariovorlage wird durch die folgenden Vorlagen für Ausgabenoptimierungsszenarien ergänzt, die ebenfalls bereitgestellt werden können:

* [[!UICONTROL Projektaktualisierungen  [!DNL Adobe Workfront]  ein  [!DNL Anaplan]  senden]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-updates-to-anaplan-list-item.md)
* [[!UICONTROL Senden von  [!DNL Adobe Workfront] -Stunden-Aktualisierungen an ein  [!DNL Anaplan] -Element]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-actual-hours-updates-to-anaplan-list-item.md)

Zusätzliche Szenarien für die Verknüpfung von Budgetanfragen:

* [[!UICONTROL Erstellen eines  [!DNL Anaplan] -Listenelements aus einer  [!DNL Adobe Workfront] -Anfrage]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-budget-request.md)
* [[!UICONTROL Budgetzuweisung  [!DNL Anaplan]  ein Projekt  [!DNL Adobe Workfront] &#x200B;]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-projects.md)

Zusätzliche Szenarien für die Verknüpfung von Kampagnenanfragen:

* [[!UICONTROL Erstellen eines  [!DNL Anaplan] -Listenelements aus einer  [!DNL Adobe Workfront] -Anfrage]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-campaign-request.md)
* [[!UICONTROL Budgetzuweisung  [!DNL Anaplan]  eine Kampagnenanfrage  [!DNL Adobe Workfront]  ein Kampagnenprojekt anwenden]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-campaign-requests-and-projects.md)
