---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-with-anaplan
title: Senden [!DNL Adobe Workfront] Projekt-Updates für [!DNL Anaplan] Listenelement
description: Dieses Integrationsszenario teilt Fortschritt, Status und wichtige Zeitplandetails aus einem [!DNL Adobe Workfront] Projekt mit [!DNL Anaplan] Budgetlisteneintrag. Durch die Freigabe dieser Informationen können Sie die Ausgabenoptimierung und die Finanzanalyse besser nutzen, die [!DNL Anaplan] bietet.
author: Becky
feature: Workfront Integrations and Apps, Workfront Fusion
exl-id: 97e9dac6-f5b5-4d6e-b58b-93acd19048ee
source-git-commit: 4ab731b14dc5435386fd0d887501788fa37223a2
workflow-type: tm+mt
source-wordcount: '905'
ht-degree: 2%

---

# Senden [!DNL Adobe Workfront] Projekt-Updates für [!DNL Anaplan] Listenelement

Dieses Integrationsszenario teilt Fortschritt, Status und wichtige Zeitplandetails aus einem [!DNL Adobe Workfront] Projekt mit [!DNL Anaplan] Budgetlisteneintrag. Durch die Freigabe dieser Informationen können Sie die Ausgabenoptimierung und die Finanzanalyse besser nutzen, die [!DNL Anaplan] bietet.

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

* Ein Benutzerprofil in [!DNL Workfront] benannt **[!UICONTROL [!DNL Anaplan]Integration]**, der über Systemadministratorberechtigungen verfügt.

   Informationen zum Erstellen eines Benutzers in [!DNL Workfront], siehe [Benutzer hinzufügen](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

* A **[!UICONTROL Kampagnenbeschreibung]** benutzerdefiniertes Formular, das an das Projektobjekt angehängt ist, um benutzerdefinierte Datenwerte zu speichern, die Sie an Anaplan senden möchten.

   Die folgenden Felder stellen Beispiele für Felder dar, die im benutzerdefinierten Formular enthalten sein können, um die Datenzuordnung zu Anaplan zu erleichtern. Für dieses Integrationsszenario sind sie jedoch nicht erforderlich:

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
     <td role="rowheader">[!UICONTROL In Market Start Date]</td> 
     <td>[!UICONTROL Datum] </td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL Am Marktenddatum]</td> 
     <td>[!UICONTROL Datum]</td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL Campaign Übersicht]</td> 
     <td>[!UICONTROL Absatztext-Feld]</td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL Schlüsselmeldung]</td> 
     <td>[!UICONTROL Absatztext-Feld]</td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL Target Audience]</td> 
     <td> <p>[!UICONTROL Dropdown]</p> <p>Schließen Sie Optionen ein, die zu Ihren Prozessen passen.</p> </td> 
    </tr> 
   </tbody> 
  </table>

   Informationen zum Erstellen benutzerdefinierter Formulare finden Sie unter [Benutzerdefiniertes Formular erstellen oder bearbeiten](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md)

<!--
<note type="note">  
<p>The above configuration is available through the Marketing Financial Management Configuration blueprint:</p>
<p>https://MYDOMAIN.my.workfront.com/blueprints/7ebe85c4-05a1-4efe-a018-50ee55f5654c/details </p>
<p><span style="color: #ff0000;">This note is currently not marked for publication.</span> </p>
</note>
-->

## Erwartet [!DNL Anaplan] Konfiguration

Sie müssen Folgendes in der [!DNL Anaplan] um dieses Szenario zu verwenden:

* Ein Benutzerprofil in [!DNL Anaplan] benannt **[!UICONTROL [!DNL Workfront]Integration]**, der über Systemadministratorberechtigungen verfügt.
* Die [!DNL Anaplan] Modell, das Sie für dieses Szenario verwenden möchten.
* Die Liste innerhalb der [!DNL Anaplan] Modell, das Sie für dieses Szenario verwenden möchten.
* A **[!UICONTROL Import von Projekten]** -Datei, die die folgenden Spalten enthält, in dieser Reihenfolge:

1. [!UICONTROL itemID]

2. [!UICONTROL [!DNL Workfront] Projekt-GUID]

3. [!UICONTROL Name der Kampagne]

4. [!UICONTROL Prozent abgeschlossen]

5. [!UICONTROL Geplantes Startdatum]

6. [!UICONTROL Geplantes Abschlussdatum]

7. [!UICONTROL Geplante Stunden]

8. [!UICONTROL Geplante Kosten]

9. [!UICONTROL Geplante Ausgaben]

10. [!UICONTROL Ist-Lohnkosten]

11. [!UICONTROL Geplante Lohnkosten]

12. [!UICONTROL Status]

Vorbereiten der [!UICONTROL [!DNL Anaplan] Geplanter Kostenimport] Datei:

1. Kopieren Sie Folgendes und fügen Sie es in einen Texteditor ein oder [!DNL Excel]
1. Datei im CSV-Format speichern
1. Laden Sie die Datei in Anaplan hoch.

   Anweisungen finden Sie in der [!DNL Anaplan] Dokumentation zum Importieren von Daten in Module aus einer Datei.

1. Notieren Sie sich den Namen, den Sie der Datei gegeben haben. wird während der Bereitstellung der [!UICONTROL Fusion] Szenario.

Beispiel-CSV-Inhalte

<!-- [Copy](javascript:void(0);) -->
<pre></pre>

1. [!UICONTROL Kampagnenübersicht]

2. [!UICONTROL Schlüsselmeldung]

3. [!UICONTROL Marktstartdatum]

4. [!UICONTROL Marktenddatum]

5. [!UICONTROL Zielgruppe]

Schließen Sie auch alle anderen Felder ein, die Sie in der Zuordnung festlegen möchten.

* A **[!UICONTROL Import von Projekten]** Prozess, der zum Ausführen des Imports von Daten vorbereitet wird, die in einem Datei-Upload bereitgestellt werden.

Anweisungen zu diesen Aktionen finden Sie in der [!DNL Anaplan] Dokumentation.

## Bereitstellen unter [!DNL Workfront Fusion]

Führen Sie die folgenden Schritte aus, um dieses Integrationsszenario in Ihrem Fusion-Konto bereitzustellen. Dies sollte nur nach Abschluss der erforderlichen [!DNL Workfront] und [!DNL Anaplan] Konfiguration.

1. Navigieren Sie zum [!UICONTROL Vorlagen] Menü in [!DNL Workfront Fusion] und klicken Sie auf **[!UICONTROL Senden von Workfront-Projektaktualisierungen an [!DNL Anaplan] Listenelement]** Szenario.
1. Ersetzen Sie die Variablenwerte für Folgendes [!DNL Anaplan] Variablen:

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
      <td role="rowheader">[!UICONTROL Dateiname: Import von Projektaktualisierungen]</td> 
      <td>Der Name der Datei, an die die Projekt-Update-Daten gesendet werden.<p>(Beispiel: WorkfrontUpdateLinkedProject.csv)</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Prozessname: Import von Projektaktualisierungen]</td> 
      <td> <p>Der Name des Prozesses, der den Import von Projektdaten ausführt.</p> <p>(Beispiel: WF Int - Update der Kampagnendetails)</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL Workfront] Subdomain]</td> 
      <td>Die Subdomäne Ihrer [!DNL Workfront] -Konto. Dadurch wird ein Link zu Ihrer [!DNL Workfront] -Projekt in einem Hinweis, der generiert werden kann.</td> 
     </tr> 
    </tbody> 
   </table>

   Weitere Informationen zum Einrichten der Dateien und Prozesse finden Sie im Abschnitt [!DNL Anaplan] Dokumentation einrichten.

1. Auswählen oder Hinzufügen von [!DNL Anaplan] Verbindungsprofil.
1. Alle verbleibenden aktualisieren [!DNL Anaplan] Module mit einer [!DNL Anaplan] Verbindung, wenn Sie dazu aufgefordert werden.
1. Auswählen oder Hinzufügen von [!DNL Workfront] Verbindungsprofil.

   Der Filter ist so konfiguriert, dass er alle unvollständigen verknüpften Projekte und Projekte abruft, die in den letzten 29 Minuten abgeschlossen wurden. Wenn Sie die Häufigkeit der [!DNL Fusion] Szenario können Sie diesen Wert aktualisieren, sobald die Szenario-Vorlage bereitgestellt wurde.

1. Im **[!UICONTROL Erstellen von Projekten Aktualisieren von CSV]** -Modul eine neue Datenstruktur hinzufügen, um die Projektattribute CSV-Spalten zuzuordnen.

   <!-- [Copy](javascript:void(0);) -->
   <pre></pre>

1. Alle verbleibenden aktualisieren [!DNL Workfront] Module mit [!DNL Workfront] Verbindung, wenn Sie dazu aufgefordert werden.

## Andere empfohlene Szenario-Vorlagen

Diese Szenario-Vorlage wird durch die folgenden Ausgabenoptimierungsszenarien ergänzt, die ebenfalls bereitgestellt werden können:

* [[!UICONTROL Senden [!DNL Adobe Workfront] Aktualisierungen der tatsächlichen Stunden für eine [!DNL Anaplan] Listenelement]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-actual-hours-updates-to-anaplan-list-item.md)
* [[!UICONTROL Senden [!DNL Adobe Workfront] Kosten für [!DNL Anaplan] Listenelement]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-expenses-to-anaplan-list-item.md)

Zusätzliche Szenarien für die Verknüpfung von Budgetanforderungen:

* [[!UICONTROL Erstellen Sie eine [!DNL Anaplan] Listenelement aus [!DNL Adobe Workfront] Budgetanfrage]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-budget-request.md)
* [[!UICONTROL Anwenden eines [!DNL Anaplan] Mittelzuweisung an [!DNL Adobe Workfront] Projekt]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-projects.md)

Zusätzliche Szenarien für die Verknüpfung von Kampagnenanforderungen:

* [[!UICONTROL Erstellen Sie eine [!DNL Anaplan] Listenelement aus [!DNL Adobe Workfront] Kampagnenanforderung]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-campaign-request.md)
* [[!UICONTROL Anwenden eines [!DNL Anaplan] Mittelzuweisung an [!DNL Adobe Workfront] Kampagnenanforderung oder Kampagnenprojekt]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-campaign-requests-and-projects.md)
