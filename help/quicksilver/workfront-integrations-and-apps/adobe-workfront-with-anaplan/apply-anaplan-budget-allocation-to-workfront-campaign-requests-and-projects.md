---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-with-anaplan
title: Anwenden eines [!DNL Anaplan] Mittelzuweisung an [!DNL Adobe Workfront] Kampagnenanforderung oder Kampagnenprojekt
description: Dieses Integrationsszenario synchronisiert alle Budgetzuweisungen, die in [!DNL Anaplan] zurück zu [!DNL Workfront]. Das Szenario ruft alle verknüpften Budgeteinträge der Kampagne ab und übergibt dann den gekürzten Wert an das verknüpfte Workfront-Projekt, wenn der Budgetwert geändert wurde.
author: Becky
feature: Workfront Integrations and Apps, Workfront Fusion
exl-id: 8ae28911-fa18-459a-aa50-cfb347e70e61
source-git-commit: 4ab731b14dc5435386fd0d887501788fa37223a2
workflow-type: tm+mt
source-wordcount: '673'
ht-degree: 0%

---

# Anwenden eines [!DNL Anaplan] Mittelzuweisung an [!DNL Adobe Workfront] Kampagnenanforderung oder Kampagnenprojekt

Dieses Integrationsszenario synchronisiert alle Budgetzuweisungen, die in [!DNL Anaplan] zurück zu [!DNL Workfront]. Das Szenario ruft alle verknüpften Budgetelemente der Kampagne ab und übergibt dann den Budgetwert an den verknüpften [!DNL Workfront] Projekt, wenn der Budgetwert geändert wurde.

>[!IMPORTANT]
>
>&quot;Kampagne&quot;in diesem Artikel bezieht sich auf den Anwendungsfall der Marketing-Kampagne, den dieses Szenario darstellt und in keiner Weise mit dem Szenario [!DNL Workfront Fusion] Adobe Campaign-Connector oder zum kürzlich nicht mehr unterstützten [!UICONTROL Kampagne] -Objekt in [!DNL Workfront].


## Zugriffsanforderungen

Sie müssen über den folgenden Zugriff verfügen, um die in diesem Artikel enthaltene Funktionalität nutzen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Plan*</td> 
   <td> <p>[!UICONTROL Pro] oder höher</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Arbeit]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] license**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] für Arbeitsautomatisierung und Integration] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] sowie [!DNL Adobe Workfront] , um die in diesem Artikel beschriebenen Funktionen zu verwenden.</td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren [!DNL Workfront] Administrator.

&#42;&#42;Informationen über [!DNL Adobe Workfront Fusion] Lizenzen, siehe [[!DNL Adobe Workfront Fusion] Lizenzen](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Auslösen eines Ereignisses

Dieses Szenario wird alle 15 Minuten ausgeführt.

## Erwartet [!DNL Workfront] Konfiguration

Sie müssen Folgendes in der [!DNL Workfront] um dieses Szenario zu verwenden:

* Ein Benutzerprofil in [!DNL Workfront] benannt **[!DNL Anaplan Integration]**, der über Systemadministratorberechtigungen verfügt.

   Informationen zum Erstellen eines Benutzers in [!DNL Workfront], siehe [Benutzer hinzufügen](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

## Erwartet [!DNL Anaplan] Konfiguration

Sie müssen Folgendes in der [!DNL Anaplan] um dieses Szenario zu verwenden:

* Ein Benutzerprofil in [!DNL Anaplan] benannt **[!UICONTROL [!DNL Workfront]Integration]**, der über Systemadministratorberechtigungen verfügt.
* Die [!DNL Anaplan] Modell, das Sie für dieses Szenario verwenden möchten.
* Die Liste innerhalb der [!DNL Anaplan] Modell, das Kampagnenbudgets erfasst.

   Das Modul der Liste muss den Empfang der folgenden Attribute unterstützen:

   * [!UICONTROL [!DNL Workfront] Antrags-GUID]
   * [!UICONTROL [!DNL Workfront] Projekt-GUID]
   * [!UICONTROL Name der Kampagne]
   * [!UICONTROL Beantragte Arbeitsfonds]
   * [!UICONTROL Geschätzter Umsatz]
   * [!UICONTROL Marke]

   Diese Liste und dieses Modul müssen zusätzliche Details speichern, die für die normale Funktionalität von [!DNL Anaplan], einschließlich der Möglichkeit, ein Budget festzulegen und mitzuteilen, dass das Budgetlistenelement zur erneuten Synchronisierung mit [!DNL Workfront].

* Eine Ansicht in [!DNL Anaplan] aufgerufen **[!UICONTROL Campaigns.Update von Kampagnen in Adobe Workfront]**.

   Diese Ansicht muss die folgenden Spalten in dieser Reihenfolge enthalten:

   1. [!UICONTROL Elementname]

   2. [!UICONTROL [!DNL Workfront] Antrags-GUID]

   3. [!UICONTROL [!DNL Workfront] Projekt-GUID]

   4. [!UICONTROL Name der Kampagne]

   5. [!UICONTROL Budget]

   6. [!UICONTROL Geschätzter Umsatz]

   7. [!UICONTROL Marke]
   Die Ansicht sollte gefiltert werden, um Elemente anzuzeigen, die eine [!UICONTROL [!DNL Workfront] Projekt-GUID] und einige Hinweise darauf, dass Haushaltsmittel an Workfront übermittelt werden sollten.

Anweisungen zu diesen Aktionen finden Sie in der [!DNL Anaplan] Dokumentation.

## Bereitstellen in Workfront Fusion

Führen Sie die folgenden Schritte aus, um dieses Integrationsszenario in Ihrem Fusion-Konto bereitzustellen. Dies sollte nur nach Abschluss der erforderlichen [!DNL Workfront] und [!DNL Anaplan] Konfiguration.

1. Navigieren Sie zum [!UICONTROL Vorlagen] Menü in [!DNL Workfront Fusion] und klicken Sie auf **[!UICONTROL Anwenden [!DNL Anaplan] Budgetzuweisungen für Workfront-Kampagnenanforderungen und -projekte]** Szenario.
1. Ersetzen Sie die Variablenwerte für Folgendes [!DNL Anaplan] Variablen:

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
      <td role="rowheader">[!UICONTROL [!DNL Anaplan] Arbeitsbereichs-ID]</td> 
      <td>Die ID eines Arbeitsbereichs aus Ihrer [!DNL Anaplan] -Konto.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL Anaplan] Modell-ID] </td> 
      <td>Die Kennung eines Modells aus Ihrer [!DNL Anaplan] und dem ausgewählten Arbeitsbereich.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Kampagnenlisten-Name]</td> 
      <td>Der Name der Liste aus Ihrem [!DNL Anaplan] und dem ausgewählten Arbeitsbereich und Modell.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL Anaplan] Ansichtsname]</td> 
      <td> <p>Der Name der Ansicht, die bereit zur Übermittlung von Kampagnenbudgets an enthält [!DNL Workfront].</p> <p>(Beispiel: [!UICONTROL Campaigns.Load-Kampagnen in [!DNL Adobe Workfront]]) </p> </td> 
     </tr> 
    </tbody> 
   </table>

   Weitere Informationen zum Einrichten der Dateien und Prozesse finden Sie im Abschnitt [!DNL Anaplan] Dokumentation einrichten.

1. Auswählen oder Hinzufügen von [!DNL Anaplan] Verbindungsprofil.
1. Alle verbleibenden aktualisieren [!DNL Anaplan] Module mit einer [!DNL Anaplan] Verbindung, wenn Sie dazu aufgefordert werden.
1. Im **[!UICONTROL CSV in JSON-Objekt konvertieren]** -Modul eine neue Datenstruktur hinzufügen, um die CSV-Spalten einem verwendbaren JSON-Objekt zuzuordnen.

   <!-- [Copy](javascript:void(0);) -->
   <pre></pre>

1. Wenn Sie dazu aufgefordert werden, wählen Sie diese Datenstruktur für andere Module in dieser Szenario-Bereitstellung aus.
1. Im **[!UICONTROL Überprüfen eines verknüpften Projekts]** -Modul, wählen Sie ein [!DNL Workfront] Verbindungsprofil.
1. Alle verbleibenden aktualisieren [!DNL Workfront] Module mit [!DNL Workfront] Verbindung, wenn Sie dazu aufgefordert werden.

## Andere empfohlene Szenario-Vorlagen

Um den von dieser Vorlage dargestellten Workflow abzuschließen, müssen Sie außerdem die folgende zusätzliche Vorlage bereitstellen:

* [[!UICONTROL Erstellen Sie eine [!DNL Anaplan] Listenelement aus [!DNL Adobe Workfront] Kampagnenanforderung]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-campaign-request.md)

Weitere Szenarien für die Ausgabenoptimierung sind:

* [[!UICONTROL Senden [!DNL Adobe Workfront] Projekt-Updates für [!DNL Anaplan] Listenelement]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-updates-to-anaplan-list-item.md)

* [[!UICONTROL Senden [!DNL Adobe Workfront] Aktualisierungen der tatsächlichen Stunden für eine [!DNL Anaplan] Listenelement]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-actual-hours-updates-to-anaplan-list-item.md)

* [[!UICONTROL Senden [!DNL Adobe Workfront] Kosten für [!DNL Anaplan] Listenelement]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-expenses-to-anaplan-list-item.md)
