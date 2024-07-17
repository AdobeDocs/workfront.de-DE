---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-with-anaplan
title: Senden von [!DNL Adobe Workfront] tatsächlichen Stunden-Aktualisierungen an ein [!DNL Anaplan] Listenelement
description: Dieses Integrationsszenario teilt die tatsächlichen Stunden-Details eines [!DNL Adobe Workfront] Projekts mit einem [!DNL Anaplan] Budgetlistenelement. Durch die Freigabe dieser Informationen können Sie die Ausgabenoptimierung und die Finanzanalyse, die [!DNL Anaplan] bietet, besser nutzen.
author: Becky
feature: Workfront Integrations and Apps, Workfront Fusion
exl-id: 450b9a87-79c6-4d10-a9ea-29766b4f5962
source-git-commit: 4ab731b14dc5435386fd0d887501788fa37223a2
workflow-type: tm+mt
source-wordcount: '726'
ht-degree: 0%

---

# Senden von [!DNL Adobe Workfront] tatsächlichen Stunden-Aktualisierungen an ein [!DNL Anaplan] Listenelement

Dieses Integrationsszenario teilt die tatsächlichen Stundendetails eines [!DNL Adobe Workfront]-Projekts mit einem [!DNL Anaplan] Budgetlistenelement. Durch die Freigabe dieser Informationen können Sie die Ausgabenoptimierung und Finanzanalyse, die [!DNL Anaplan] bietet, besser nutzen.

Diese Szenario-Vorlage bietet eine Liste der Stunden, die nach Projekt, Tag und Rolle zusammengefasst sind, die in den letzten 3 Monaten bei aktiven Projekten aufgezeichnet wurden.

>[!IMPORTANT]
>
>&quot;Kampagne&quot;in diesem Artikel bezieht sich auf den Anwendungsfall der Marketing-Kampagne, den dieses Szenario darstellt und in keiner Weise mit dem [!DNL Workfront Fusion] Adobe Campaign-Connector oder dem kürzlich veralteten [!UICONTROL Campaign] -Objekt in [!DNL Workfront] verknüpft ist.

## Zugriffsanforderungen

Sie müssen über den folgenden Zugriff verfügen, um die Funktionalität in diesem Artikel verwenden zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
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
   <td>Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] sowie [!DNL Adobe Workfront] erwerben, um die in diesem Artikel beschriebenen Funktionen nutzen zu können.</td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren [!DNL Workfront] -Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

&#42;&#42;Informationen zu [!DNL Adobe Workfront Fusion] Lizenzen finden Sie unter [[!DNL Adobe Workfront Fusion] Lizenzen](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Ereignis auslösen

Dieses Szenario wird alle 15 Minuten ausgeführt.

## Erwartete [!DNL Workfront] Konfiguration

Sie müssen Folgendes in [!DNL Workfront] haben, um dieses Szenario zu verwenden:

* Ein Benutzerprofil mit dem Namen [!DNL Workfront] mit dem Namen **[!UICONTROL Anaplan-Integration]**, das über Systemadministrator-Rechte verfügt.

  Informationen zum Erstellen eines Benutzers in [!DNL Workfront] finden Sie unter [Benutzer hinzufügen](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

## Erwartete [!DNL Anaplan] Konfiguration

Sie müssen Folgendes in [!DNL Anaplan] haben, um dieses Szenario zu verwenden:

* Ein Benutzerprofil mit dem Namen **[!UICONTROL [!DNL Workfront]Integration]** in [!DNL Anaplan] mit Systemadministrator-Berechtigungen.
* Das [!DNL Anaplan]-Modell, das Sie für dieses Szenario verwenden möchten.
* Die Liste innerhalb des [!DNL Anaplan]-Modells, das Sie für dieses Szenario verwenden möchten.
* Eine Datei mit dem Namen [!DNL Anaplan] namens **[!UICONTROL Import der tatsächlichen Öffnungszeiten von Anaplan]**, die die folgenden Spalten in dieser Reihenfolge enthält:

   1. [!UICONTROL Workfront Project GUID]

   2. [!UICONTROL Stunden]

   3. [!UICONTROL Geschätzte Kosten pro Stunde]

   4. [!UICONTROL Einstiegsdatum]

   5. [!UICONTROL Rollenname]

   6. [!UICONTROL Kampagnenname]

   7. [!UICONTROL [!DNL Anaplan] Listenelement-ID]

  So bereiten Sie die Datei mit dem Bericht &quot;[!DNL Anaplan] Tatsächliche Ausgaben&quot;vor:

   1. Kopieren Sie Folgendes und fügen Sie es in einen Texteditor oder [!DNL Excel] ein
   1. Datei im CSV-Format speichern
   1. Laden Sie die Datei in [!DNL Anaplan] hoch.

      Anweisungen finden Sie in der [!DNL Anaplan] -Dokumentation zum Importieren von Daten in Module aus einer Datei.

   1. Notieren Sie sich den Namen, den Sie der Datei gegeben haben. Er wird während der Bereitstellung der Szenario-Vorlage [!UICONTROL Fusion] verwendet.

  Beispiel-CSV-Inhalte

  <!-- [Copy](javascript:void(0);) -->
  <pre><code>[!DNL Workfront] Project GUID,Hours,Hours Estimated Cost,Entry Date,Role Name,Workfront Project Name,Item ID<br>6218062a000d0442903fcfa21e11f556,2,0,3/7/22,Designer,New Project 6,202000001030</code></pre>

* Ein **[!UICONTROL Projekt Actual Hours Import]** -Prozess, der für die Ausführung des Imports von Daten vorbereitet wird, die in einem Datei-Upload bereitgestellt werden.

Anweisungen zu diesen Aktionen finden Sie in der Dokumentation zu [!DNL Anaplan] .

## Bereitstellen unter [!DNL Workfront Fusion]

Führen Sie die folgenden Schritte aus, um dieses Integrationsszenario in Ihrem [!DNL Fusion]-Konto bereitzustellen. Dies sollte erst nach Abschluss der erforderlichen [!DNL Workfront] - und [!DNL Anaplan] -Konfiguration erfolgen.

1. Navigieren Sie zum Menü [!UICONTROL Vorlagen] in [!DNL Workfront Fusion] und klicken Sie auf die Vorlage **[!UICONTROL Workfront-Aktualisierungen bezüglich aktueller Stunden an [!DNL Anaplan] Listenelement]** senden .
1. Ersetzen Sie die Variablenwerte für die folgenden [!DNL Anaplan] -Variablen:

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
      <td>Die ID eines Workspace aus Ihrem [!DNL Anaplan]-Konto.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL Anaplan] Modell-ID] </td> 
      <td>Die ID eines Modells aus Ihrem [!DNL Anaplan] -Konto und dem ausgewählten Arbeitsbereich.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Kampagnenlisten-Name]</td> 
      <td>Der Name der Liste aus Ihrem [!DNL Anaplan] -Konto und der ausgewählte Arbeitsbereich und das ausgewählte Modell.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Dateiname: Tatsächlicher Stundenimport]</td> 
      <td> <p>Der Name der Datei, die die Daten zu den tatsächlichen Projektstunden erhält.</p> <p> (Beispiel: WorkfrontUpdateLinkedProjects_HoursRoles.csv) </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Prozessname: Tatsächlicher Stundenimport]</td> 
      <td> <p>Der Name des Prozesses, der den Import von Projektstundendaten ausführt.</p> <p>(Beispiel: WF Int - Projektstunden nach Rolle laden)</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL Workfront] Subdomain]</td> 
      <td>Die Subdomäne Ihres [!DNL Workfront]-Kontos. Damit wird ein Link zu Ihrem [!DNL Workfront]-Projekt in einem Hinweis erstellt, der möglicherweise generiert wird.</td> 
     </tr> 
    </tbody> 
   </table>

   Weitere Informationen zum Einrichten der Dateien und Prozesse finden Sie in der Dokumentation zur Einrichtung von [!DNL Anaplan] .

1. Wählen Sie ein Verbindungsprofil vom Typ [!DNL Anaplan] aus oder fügen Sie es hinzu.
1. Aktualisieren Sie bei Aufforderung alle verbleibenden [!DNL Anaplan] -Module mit einer [!DNL Anaplan] -Verbindung.
1. Wählen Sie ein Verbindungsprofil vom Typ [!DNL Workfront] aus oder fügen Sie es hinzu.
1. Aktualisieren Sie bei Aufforderung alle verbleibenden [!DNL Workfront] -Module mit einer [!DNL Workfront] -Verbindung.

## Andere empfohlene Szenario-Vorlagen

Diese Szenario-Vorlage wird durch die folgenden Ausgabenoptimierungsszenarien ergänzt, die ebenfalls bereitgestellt werden können:

* [[!UICONTROL Senden von [!DNL Adobe Workfront] Projektaktualisierungen an ein [!DNL Anaplan] Listenelement]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-updates-to-anaplan-list-item.md)
* [[!UICONTROL Senden [!DNL Adobe Workfront] der Ausgaben an einen  [!DNL Anaplan] Listeneintrag]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-expenses-to-anaplan-list-item.md)

Zusätzliche Szenarien für die Verknüpfung von Budgetanforderungen:

* [[!UICONTROL Erstellen eines  [!DNL Anaplan] Listenelements aus einer  [!DNL Adobe Workfront] Budgetanforderung]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-budget-request.md)
* [[!UICONTROL Anwenden einer [!DNL Anaplan] Budgetzuordnung auf ein [!DNL Adobe Workfront] Projekt]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-projects.md)

Zusätzliche Szenarien für die Verknüpfung von Kampagnenanforderungen:

* [[!UICONTROL Erstellen eines  [!DNL Anaplan] Listenelements aus einer [!DNL Adobe Workfront] Kampagnenanforderung]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-campaign-request.md)
* [[!UICONTROL Anwenden einer [!DNL Anaplan] Budgetzuordnung auf eine [!DNL Adobe Workfront] Kampagnenanforderung oder ein Kampagnenprojekt]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-campaign-requests-and-projects.md)
