---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-with-anaplan
title: Senden [!DNL Adobe Workfront] Aktualisierungen der tatsächlichen Stunden für eine [!DNL Anaplan] Listenelement
description: Dieses Integrationsszenario teilt die tatsächlichen Stundendetails mit, die in einem [!DNL Adobe Workfront] Projekt mit [!DNL Anaplan] Budgetlisteneintrag. Durch die Freigabe dieser Informationen können Sie die Ausgabenoptimierung und die Finanzanalyse besser nutzen, die [!DNL Anaplan] bietet.
author: Becky
feature: Workfront Integrations and Apps, Workfront Fusion
exl-id: 450b9a87-79c6-4d10-a9ea-29766b4f5962
source-git-commit: 4ab731b14dc5435386fd0d887501788fa37223a2
workflow-type: tm+mt
source-wordcount: '725'
ht-degree: 0%

---

# Senden [!DNL Adobe Workfront] Aktualisierungen der tatsächlichen Stunden für eine [!DNL Anaplan] Listenelement

Dieses Integrationsszenario teilt die tatsächlichen Stundendetails mit, die in einem [!DNL Adobe Workfront] Projekt mit [!DNL Anaplan] Budgetlisteneintrag. Durch die Freigabe dieser Informationen können Sie die Ausgabenoptimierung und die Finanzanalyse besser nutzen, die [!DNL Anaplan] bietet.

Diese Szenario-Vorlage bietet eine Liste der Stunden, die nach Projekt, Tag und Rolle zusammengefasst sind, die in den letzten 3 Monaten bei aktiven Projekten aufgezeichnet wurden.

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

* Ein Benutzerprofil in [!DNL Workfront] benannt **[!UICONTROL Anaplan-Integration]**, der über Systemadministratorberechtigungen verfügt.

   Informationen zum Erstellen eines Benutzers in [!DNL Workfront], siehe [Benutzer hinzufügen](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

## Erwartet [!DNL Anaplan] Konfiguration

Sie müssen Folgendes in der [!DNL Anaplan] um dieses Szenario zu verwenden:

* Ein Benutzerprofil in [!DNL Anaplan] benannt **[!UICONTROL [!DNL Workfront ]Integration]**, der über Systemadministratorberechtigungen verfügt.
* Die [!DNL Anaplan] Modell, das Sie für dieses Szenario verwenden möchten.
* Die Liste innerhalb der [!DNL Anaplan] Modell, das Sie für dieses Szenario verwenden möchten.
* Eine Datei in [!DNL Anaplan] benannt **[!UICONTROL Importieren von Anaplan-Stunden]** die die folgenden Spalten enthält, in dieser Reihenfolge:

   1. [!UICONTROL Workfront-Projekt-GUID]

   2. [!UICONTROL Stunden]

   3. [!UICONTROL Geschätzte Stundenkosten]

   4. [!UICONTROL Eingabedatum]

   5. [!UICONTROL Rollenname]

   6. [!UICONTROL Name der Kampagne]

   7. [!UICONTROL [!DNL Anaplan] Listenelement-ID]
   Vorbereiten der [!DNL Anaplan] Berichtsdatei zu tatsächlichen Ausgaben:

   1. Kopieren Sie Folgendes und fügen Sie es in einen Texteditor ein oder [!DNL Excel]
   1. Datei im CSV-Format speichern
   1. Laden Sie die Datei in hoch. [!DNL Anaplan].

      Anweisungen finden Sie in der [!DNL Anaplan] Dokumentation zum Importieren von Daten in Module aus einer Datei.

   1. Notieren Sie sich den Namen, den Sie der Datei gegeben haben. wird während der Bereitstellung der [!UICONTROL Fusion] Szenario.

   Beispiel-CSV-Inhalte

   <!-- [Copy](javascript:void(0);) -->
   <pre></pre>

* A **[!UICONTROL Import der tatsächlichen Projektstunden]** Prozess, der zum Ausführen des Imports von Daten vorbereitet wird, die in einem Datei-Upload bereitgestellt werden.

Anweisungen zu diesen Aktionen finden Sie in der [!DNL Anaplan] Dokumentation.

## Bereitstellen unter [!DNL Workfront Fusion]

Führen Sie die folgenden Schritte aus, um dieses Integrationsszenario für Ihre [!DNL Fusion] -Konto. Dies sollte nur nach Abschluss der erforderlichen [!DNL Workfront] und [!DNL Anaplan] Konfiguration.

1. Navigieren Sie zum [!UICONTROL Vorlagen] Menü in [!DNL Workfront Fusion] und klicken Sie auf **[!UICONTROL Senden von Aktualisierungen der tatsächlichen Workfront-Stunden an [!DNL Anaplan] Listenelement]** Szenario.
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
      <td role="rowheader">[!UICONTROL Dateiname: Tatsächlicher Stundenimport]</td> 
      <td> <p>Der Name der Datei, die die Daten zu den tatsächlichen Projektstunden erhält.</p> <p> (Beispiel: WorkfrontUpdateLinkedProjects_HoursRoles.csv) </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Prozessname: Tatsächlicher Stundenimport]</td> 
      <td> <p>Der Name des Prozesses, der den Import von Projektstundendaten ausführt.</p> <p>(Beispiel: WF Int - Projektzeiten nach Rolle laden)</p> </td> 
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
1. Alle verbleibenden aktualisieren [!DNL Workfront] Module mit [!DNL Workfront] Verbindung, wenn Sie dazu aufgefordert werden.

## Andere empfohlene Szenario-Vorlagen

Diese Szenario-Vorlage wird durch die folgenden Ausgabenoptimierungsszenarien ergänzt, die ebenfalls bereitgestellt werden können:

* [[!UICONTROL Senden [!DNL Adobe Workfront] Projekt-Updates für [!DNL Anaplan] Listenelement]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-updates-to-anaplan-list-item.md)
* [[!UICONTROL Senden [!DNL Adobe Workfront] Kosten für [!DNL Anaplan] Listenelement]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-expenses-to-anaplan-list-item.md)

Zusätzliche Szenarien für die Verknüpfung von Budgetanforderungen:

* [[!UICONTROL Erstellen Sie eine [!DNL Anaplan] Listenelement aus [!DNL Adobe Workfront] Budgetanfrage]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-budget-request.md)
* [[!UICONTROL Anwenden eines [!DNL Anaplan] Mittelzuweisung an [!DNL Adobe Workfront] Projekt]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-projects.md)

Zusätzliche Szenarien für die Verknüpfung von Kampagnenanforderungen:

* [[!UICONTROL Erstellen Sie eine [!DNL Anaplan] Listenelement aus [!DNL Adobe Workfront] Kampagnenanforderung]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-campaign-request.md)
* [[!UICONTROL Anwenden eines [!DNL Anaplan] Mittelzuweisung an [!DNL Adobe Workfront] Kampagnenanforderung oder Kampagnenprojekt]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-campaign-requests-and-projects.md)
