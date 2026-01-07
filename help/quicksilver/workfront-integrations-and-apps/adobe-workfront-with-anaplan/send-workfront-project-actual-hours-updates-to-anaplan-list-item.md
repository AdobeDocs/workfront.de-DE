---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-with-anaplan
title: ' [!DNL Adobe Workfront]  Stunden-Aktualisierungen an ein  [!DNL Anaplan]  senden'
description: Dieses Integrationsszenario teilt die tatsächlichen Stundendetails, die in einem Projekt  [!DNL Adobe Workfront]  einem  [!DNL Anaplan] -Budgetlistenelement erfasst werden. Durch die Weitergabe dieser Informationen können Sie die Ausgabenoptimierung und die Finanzanalyse, die  [!DNL Anaplan]  bietet, besser nutzen.
author: Becky
feature: Workfront Integrations and Apps, Workfront Fusion
exl-id: 450b9a87-79c6-4d10-a9ea-29766b4f5962
source-git-commit: 53596271a838733b858c0b14a4e22b07a7cd20f6
workflow-type: tm+mt
source-wordcount: '781'
ht-degree: 15%

---

# Senden [!DNL Adobe Workfront] tatsächlichen Stundenaktualisierungen an ein [!DNL Anaplan] Listenelement

Dieses Integrationsszenario teilt die tatsächlichen Stundendetails, die in einem [!DNL Adobe Workfront] Projekt mit einem [!DNL Anaplan] Budgetlistenelement erfasst werden. Durch die Weitergabe dieser Informationen können Sie die von [!DNL Anaplan] bereitgestellten Funktionen zur Ausgabenoptimierung und Finanzanalyse besser nutzen.

Diese Szenario-Vorlage liefert eine Liste der Stunden, die nach Projekt, Tag und Rolle in den aktiven Projekten der letzten drei Monate zusammengefasst wurden.

>[!IMPORTANT]
>
>„Kampagne“ in diesem Artikel bezieht sich auf den Anwendungsfall der Marketing-Kampagne, den dieses Szenario darstellt, und ist in keiner Weise mit dem [!DNL Workfront Fusion] Adobe Campaign-Connector oder dem kürzlich veralteten Objekt [!UICONTROL Kampagne] in [!DNL Workfront] verbunden.

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Paket</td> 
   <td> <p>Ein beliebiges Adobe Workfront Workflow- und Adobe Workfront Automation and Integration-Paket</p><p>Workfront Ultimate</p><p>Workfront Prime- und Select-Pakete bei zusätzlichem Kauf von Workfront Fusion.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Adobe Workfront-Lizenzen</td> 
   <td> <p>Standard</p><p>Work oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront Fusion-Lizenz</td> 
   <td>
   <p>Betriebsbasiert: keine Workfront Fusion-Lizenz erforderlich</p>
   <p>Connector-basiert (veraltet): Workfront Fusion for Work Automation and Integration </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>
   <p>Wenn Ihre Organisation über ein Workfront Select- oder Prime-Paket ohne Workfront Automation and Integration verfügt, muss Ihre Organisation Adobe Workfront Fusion erwerben.</li></ul>
   </td> 
  </tr>
 </tbody> 
</table>

Weitere Details zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

Informationen zu Adobe Workfront Fusion-Lizenzen finden Sie unter [Adobe Workfront Fusion-Lizenzen](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/set-up-and-manage-fusion/licensing-and-operations-overviews/license-automation-vs-integration).

+++

## Auslösendes Ereignis

Dieses Szenario ist so geplant, dass es alle 15 Minuten ausgeführt wird.

## Erwartete [!DNL Workfront]

Sie müssen über Folgendes verfügen, [!DNL Workfront] dieses Szenario verwenden zu können:

* Ein Benutzerprofil in [!DNL Workfront] mit dem Namen **[!UICONTROL Anaplan-Integration]**, das über Systemadministratorrechte verfügt.

  Informationen zum Erstellen eines Benutzers in [!DNL Workfront] finden Sie unter [Benutzer hinzufügen](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

## Erwartete [!DNL Anaplan]

Sie müssen über Folgendes verfügen, [!DNL Anaplan] dieses Szenario verwenden zu können:

* Ein Benutzerprofil in [!DNL Anaplan] mit dem Namen **[!UICONTROL [!DNL Workfront]Integration]**, das über Systemadministratorrechte verfügt.
* Das [!DNL Anaplan], das Sie für dieses Szenario verwenden möchten.
* Die Liste innerhalb des [!DNL Anaplan], die Sie für dieses Szenario verwenden möchten.
* Eine Datei in [!DNL Anaplan] mit dem Namen **[!UICONTROL Anaplan Actual Hours Import]**, die die folgenden Spalten in der folgenden Reihenfolge enthält:

   1. [!UICONTROL Workfront-Projekt-GUID]

   2. [!UICONTROL Stunden]

   3. [!UICONTROL Geschätzte Kosten für Stunden]

   4. [!UICONTROL Eingabedatum]

   5. [!UICONTROL Rollenname]

   6. [!UICONTROL Kampagnenname]

   7. [!UICONTROL [!DNL Anaplan] Listenelement-ID]

  So bereiten Sie die [!DNL Anaplan] Ist-Ausgabenberichtsdatei vor:

   1. Folgendes kopieren und in einen Texteditor oder [!DNL Excel] einfügen
   1. Speichern Sie die Datei im CSV-Format
   1. Laden Sie die Datei in [!DNL Anaplan] hoch.

      Anweisungen finden Sie in der [!DNL Anaplan] Dokumentation zum Importieren von Daten aus einer Datei in -Module.

   1. Notieren Sie sich den Namen, den Sie der Datei gegeben haben. Er wird während der Bereitstellung der Szenariovorlage [!UICONTROL Fusion] verwendet.

  Beispiel für CSV-Inhalte

  <!-- [Copy](javascript:void(0);) -->
  <pre><code>[!DNL Workfront] Project GUID,Hours,Hours Estimated Cost,Entry Date,Role Name,Workfront Project Name,Item ID<br>6218062a000d0442903fcfa21e11f556,2,0,3/7/22,Designer,New Project 6,202000001030</code></pre>

* Ein **[!UICONTROL Projekt - Tatsächlicher Stunden]** Importprozess, der auf den Import von Daten vorbereitet ist, die über einen Datei-Upload bereitgestellt werden.

Anweisungen zu diesen Aktionen finden Sie in der [!DNL Anaplan]-Dokumentation.

## Bereitstellen für [!DNL Workfront Fusion]

Führen Sie die folgenden Schritte aus, um dieses Integrationsszenario in Ihrem [!DNL Fusion]-Konto bereitzustellen. Dies sollte erst nach Abschluss der erforderlichen [!DNL Workfront]- und [!DNL Anaplan]-Konfiguration erfolgen.

1. Navigieren Sie zum Menü [!UICONTROL Vorlagen] in [!DNL Workfront Fusion] und klicken Sie auf die Szenariovorlage **[!UICONTROL Workfront tatsächliche Stundenaktualisierungen an [!DNL Anaplan] Listenelement senden]**.
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
      <td role="rowheader">[!UICONTROL Dateiname: Tatsächlicher Stundenimport]</td> 
      <td> <p>Der Name der Datei, die die tatsächlichen Stunden des Projekts erhält.</p> <p> (Beispiel: WorkfrontUpdateLinkedProjects_HoursRoles.csv) </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Prozessname: Tatsächliche Stunden importieren]</td> 
      <td> <p>Der Name des Prozesses, der den Import von Projektstundendaten ausführt.</p> <p>(Beispiel: WF int - Projektstunden nach Rolle laden)</p> </td> 
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
1. Aktualisieren Sie alle verbleibenden [!DNL Workfront]-Module mit einer [!DNL Workfront] Verbindung, wenn Sie dazu aufgefordert werden.

## Andere empfohlene Szenariovorlagen

Diese Szenariovorlage wird durch die folgenden Vorlagen für Ausgabenoptimierungsszenarien ergänzt, die ebenfalls bereitgestellt werden können:

* [[!UICONTROL Projektaktualisierungen  [!DNL Adobe Workfront]  ein  [!DNL Anaplan]  senden]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-updates-to-anaplan-list-item.md)
* [[!UICONTROL Senden [!DNL Adobe Workfront] Ausgaben an  [!DNL Anaplan] /Listenelement]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-expenses-to-anaplan-list-item.md)

Zusätzliche Szenarien für die Verknüpfung von Budgetanfragen:

* [[!UICONTROL Erstellen eines  [!DNL Anaplan] -Listenelements aus einer  [!DNL Adobe Workfront] -Anfrage]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-budget-request.md)
* [[!UICONTROL Budgetzuweisung  [!DNL Anaplan]  ein Projekt  [!DNL Adobe Workfront] ]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-projects.md)

Zusätzliche Szenarien für die Verknüpfung von Kampagnenanfragen:

* [[!UICONTROL Erstellen eines  [!DNL Anaplan] -Listenelements aus einer  [!DNL Adobe Workfront] -Anfrage]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-campaign-request.md)
* [[!UICONTROL Budgetzuweisung  [!DNL Anaplan]  eine Kampagnenanfrage  [!DNL Adobe Workfront]  ein Kampagnenprojekt anwenden]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-campaign-requests-and-projects.md)
