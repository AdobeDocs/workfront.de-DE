---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-with-anaplan
title: Senden [!DNL Adobe Workfront] Kosten für [!DNL Anaplan] Listenelement
description: Dieses Integrationsszenario teilt Spesendetails von einem [!DNL Adobe Workfront] Projekt mit [!DNL Anaplan] Budgetlisteneintrag. Durch die Freigabe dieser Informationen können Sie die Ausgabenoptimierung und die Finanzanalyse besser nutzen, die [!DNL Anaplan] bietet.
author: Becky
feature: Workfront Integrations and Apps, Workfront Fusion
exl-id: f9198017-9bbb-4776-86aa-3f78705dbb22
source-git-commit: 4ab731b14dc5435386fd0d887501788fa37223a2
workflow-type: tm+mt
source-wordcount: '922'
ht-degree: 2%

---

# Senden [!DNL Adobe Workfront] Kosten für [!DNL Anaplan] Listenelement

Dieses Integrationsszenario teilt Spesendetails von einem [!DNL Adobe Workfront] Projekt mit [!DNL Anaplan] Budgetlisteneintrag. Durch die Freigabe dieser Informationen können Sie die Ausgabenoptimierung und die Finanzanalyse besser nutzen, die [!DNL Anaplan] bietet.

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
   <td> <p>Workfront Fusion für Arbeitsautomatisierung und -integration </p> </td> 
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

* Ein Benutzerprofil in [!DNL Workfront] benannt *[!UICONTROL *[!DNL Anaplan] Integration]**, das über Systemadministratorrechte verfügt.

   Informationen zum Erstellen eines Benutzers in [!DNL Workfront], siehe [Benutzer hinzufügen](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

* A **[!UICONTROL Kampagnenbeschreibung]** benutzerdefiniertes Formular, das an das Projektobjekt angehängt ist, um benutzerdefinierte Datenwerte zu speichern, an die Sie senden möchten [!DNL Anaplan].

   Das Formular muss die folgenden Felder enthalten:

   | Feldname | Feldtyp |
   |---|---|
   | [!UICONTROL Letztes Übermittlungsdatum] | Datum |
   | [!UICONTROL Integrationshinweise] | Absatztextfeld |

   Informationen zum Erstellen benutzerdefinierter Formulare finden Sie unter [Benutzerdefiniertes Formular erstellen oder bearbeiten](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md)

## Erwartet [!DNL Anaplan] Konfiguration

Sie müssen Folgendes in der [!DNL Anaplan] um dieses Szenario zu verwenden:

* Ein Benutzerprofil in [!DNL Anaplan] benannt **[!UICONTROL [!DNL Workfront ]Integration]**, der über Systemadministratorberechtigungen verfügt.
* Die [!DNL Anaplan] Modell, das Sie für dieses Szenario verwenden möchten.
* Die Liste innerhalb der [!DNL Anaplan] Modell, das Kampagnenbudgets erfassen soll.
* Ein **[!UICONTROL Importieren von tatsächlichen Kosten in Anaplan]** -Datei, die die folgenden Spalten enthält, in dieser Reihenfolge:

   1. [!UICONTROL [!DNL Workfront] AusgabenGUID]

   2. [!UICONTROL [!DNL Workfront] Projekt-GUID]

   3. [!UICONTROL Tatsächlicher Betrag]

   4. [!UICONTROL Beschreibung]

   5. [!UICONTROL Ausgabentyp]

   6. [!UICONTROL Datum des Inkrafttretens]

   7. [!UICONTROL Name der Kampagne]

   8. [!UICONTROL [!DNL Anaplan] Listenelement-ID]
   Vorbereiten der [!UICONTROL [!DNL Anaplan] Tatsächlicher Import von Ausgaben] Datei:

   1. Kopieren Sie Folgendes und fügen Sie es in einen Texteditor ein oder [!DNL Excel].
   1. Speichern Sie die Datei im CSV-Format.
   1. Laden Sie die Datei in hoch. [!DNL Anaplan].

      Anweisungen finden Sie in der [!DNL Anaplan] Dokumentation zum Importieren von Daten in Module aus einer Datei.

   1. Notieren Sie sich den Namen, den Sie der Datei gegeben haben. wird während der Bereitstellung der [!UICONTROL Fusion] Szenario.

   Beispiel-CSV-Inhalte

   <!-- [Copy](javascript:void(0);) -->
   <pre></pre>

* Ein **[!UICONTROL [!DNL Anaplan]Geplanter Kostenimport]** -Datei, die die folgenden Spalten enthält, in dieser Reihenfolge:

   1. [!UICONTROL [!DNL Workfront] AusgabenGUID]

   2. [!UICONTROL [!DNL Workfront] Projekt-GUID]

   3. [!UICONTROL Tatsächlicher Betrag]

   4. [!UICONTROL Beschreibung]

   5. [!UICONTROL Ausgabentyp]

   6. [!UICONTROL Datum des Inkrafttretens]

   7. [!UICONTROL Name der Kampagne]

   8. [!UICONTROL [!DNL Anaplan] Listenelement-ID]
   Vorbereiten der [!UICONTROL [!DNL Anaplan] Geplanter Kostenimport] Datei:

   1. Kopieren Sie Folgendes und fügen Sie es in einen Texteditor ein oder [!DNL Excel]
   1. Datei im CSV-Format speichern
   1. Laden Sie die Datei in Anaplan hoch.

      Anweisungen finden Sie in der [!DNL Anaplan] Dokumentation zum Importieren von Daten in Module aus einer Datei.

   1. Notieren Sie sich den Namen, den Sie der Datei gegeben haben. wird während der Bereitstellung der [!UICONTROL Fusion] Szenario.

   Beispiel-CSV-Inhalte

   <!-- [Copy](javascript:void(0);) -->
   <pre></pre>


* A **[!UICONTROL Import von Projekten]** Prozess, der zum Ausführen des Imports von Daten vorbereitet wird, die in einem Datei-Upload bereitgestellt werden.

>[!NOTE]
>
>Es gibt separate Importdateien für geplante und tatsächliche Ausgaben, sodass sie unabhängig über ihre geplanten bzw. tatsächlichen Daten gemeldet werden können.

Anweisungen zu diesen Aktionen finden Sie in der [!DNL Anaplan] Dokumentation.

## Bereitstellen unter [!DNL Fusion]

Führen Sie die folgenden Schritte aus, um dieses Integrationsszenario für Ihre [!DNL Fusion] -Konto. Dies sollte nur nach Abschluss der erforderlichen [!DNL Workfront] und [!DNL Anaplan] Konfiguration.

1. Navigieren Sie zum [!UICONTROL Vorlagen] Menü in [!DNL Workfront Fusion] und klicken Sie auf **[!UICONTROL Senden von Aktualisierungen der Workfront-Ausgaben an [!DNL Anaplan] Listenelement]** Szenario.
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
      <td>Die ID des Arbeitsbereichs aus Ihrer [!DNL Anaplan] -Konto, das Sie für dieses Szenario verwenden möchten.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL Anaplan] Modell-ID] </td> 
      <td>Die Kennung des Modells aus Ihrer [!DNL Anaplan] und dem ausgewählten Arbeitsbereich, den Sie für dieses Szenario verwenden möchten.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Kampagnenlisten-Name]</td> 
      <td>Der Name der Liste aus Ihrem [!DNL Anaplan] und dem ausgewählten Arbeitsbereich und Modell, die Sie für dieses Szenario verwenden möchten.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Dateiname: Tatsächlicher Kostenimport]</td> 
      <td> <p>Der Name der Datei, die die tatsächlichen Projektausgaben erhält.</p> <p> (Beispiel: WorkfrontUpdateLinkedProjects_ActExpenses.csv) </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Dateiname: Geplanter Kostenimport]</td> 
      <td> <p>Der Name der Datei, die die geplanten Ausgabedaten des Projekts erhält.</p> <p> (Beispiel: WorkfrontUpdateLinkedProjects_PlannedExpenses.csv) </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Prozessname: Import von Projektaktualisierungen]</td> 
      <td> <p>Der Name des Prozesses, der den Import von Projektausgabedaten ausführt.</p> <p>(Beispiel: WF Int - Projektausgaben laden)</p> </td> 
     </tr> 
    </tbody> 
   </table>

   Weitere Informationen zum Einrichten der Dateien und Prozesse finden Sie im Abschnitt [!DNL Anaplan] Dokumentation einrichten.

1. Auswählen oder Hinzufügen von [!DNL Anaplan] Verbindungsprofil.
1. Alle verbleibenden aktualisieren [!DNL Anaplan] Module mit einer [!DNL Anaplan] Verbindung, wenn Sie dazu aufgefordert werden.
1. Auswählen oder Hinzufügen von [!DNL Workfront] Verbindungsprofil.
1. Alle verbleibenden aktualisieren [!DNL Workfront] Module mit [!DNL Workfront] Verbindung, wenn Sie dazu aufgefordert werden.
1. Im **[!UICONTROL Erstellen der tatsächlichen CSV-Kosten]** -Modul eine neue Datenstruktur hinzufügen, um die Projektattribute CSV-Spalten zuzuordnen.

   <!-- [Copy](javascript:void(0);) -->
   <pre></pre>

1. Im **[!UICONTROL Erstellen von CSV-Dateien mit geplanten Kosten]** -Modul eine neue Datenstruktur hinzufügen, um die Projektattribute CSV-Spalten zuzuordnen.

   <!-- [Copy](javascript:void(0);) -->
   <pre></pre>

## Andere empfohlene Szenario-Vorlagen

Diese Szenario-Vorlage wird durch die folgenden Ausgabenoptimierungsszenarien ergänzt, die ebenfalls bereitgestellt werden können:

* [[!UICONTROL Senden [!DNL Adobe Workfront] Projekt-Updates für [!DNL Anaplan] Listenelement]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-updates-to-anaplan-list-item.md)
* [[!UICONTROL Senden [!DNL Adobe Workfront] Aktualisierungen der tatsächlichen Stunden für eine [!DNL Anaplan] Listenelement]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-actual-hours-updates-to-anaplan-list-item.md)

Zusätzliche Szenarien für die Verknüpfung von Budgetanforderungen:

* [[!UICONTROL Erstellen Sie eine [!DNL Anaplan] Listenelement aus [!DNL Adobe Workfront] Budgetanfrage]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-budget-request.md)
* [[!UICONTROL Anwenden eines [!DNL Anaplan] Mittelzuweisung an [!DNL Adobe Workfront] Projekt]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-projects.md)

Zusätzliche Szenarien für die Verknüpfung von Kampagnenanforderungen:

* [[!UICONTROL Erstellen Sie eine [!DNL Anaplan] Listenelement aus [!DNL Adobe Workfront] Kampagnenanforderung]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-campaign-request.md)
* [[!UICONTROL Anwenden eines [!DNL Anaplan] Mittelzuweisung an [!DNL Adobe Workfront] Kampagnenanforderung oder Kampagnenprojekt]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-campaign-requests-and-projects.md)
