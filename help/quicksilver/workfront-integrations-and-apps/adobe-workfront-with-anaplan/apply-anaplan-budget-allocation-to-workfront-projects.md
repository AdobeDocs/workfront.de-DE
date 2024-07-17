---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-with-anaplan
title: Anwenden einer [!DNL Anaplan] Budgetzuordnung auf ein [!DNL Adobe Workfront] Projekt
description: Dieses Integrationsszenario synchronisiert alle Budgetzuweisungen, die in [!DNL Anaplan] zurück zu [!DNL Workfront] vorgenommen wurden. Das Szenario ruft alle verknüpften Budgeteinträge der Kampagne ab und übergibt dann den gekürzten Wert an das verknüpfte Workfront-Projekt, wenn der Budgetwert geändert wurde.
author: Becky
feature: Workfront Integrations and Apps, Workfront Fusion
exl-id: 9b8add8f-1978-4ab4-87ac-f1159e7d6cbb
source-git-commit: 4ab731b14dc5435386fd0d887501788fa37223a2
workflow-type: tm+mt
source-wordcount: '678'
ht-degree: 0%

---

# Anwenden einer [!DNL Anaplan] Budgetzuordnung auf ein [!DNL Adobe Workfront] Projekt

Dieses Integrationsszenario synchronisiert alle Budgetzuweisungen, die in [!DNL Anaplan] vorgenommen wurden, wieder mit [!DNL Workfront]. Das Szenario ruft alle verknüpften Budgetelemente der Kampagne ab und übergibt dann den gekürzten Wert an das verknüpfte [!DNL Workfront] -Projekt, wenn der Budgetwert geändert wurde.

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
   <td> <p>[!UICONTROL Workfront Fusion für Arbeitsautomatisierung und -integration] </p> </td> 
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

* Ein Benutzerprofil mit dem Namen [!DNL Workfront] mit dem Namen **Anaplan-Integration**, das über Systemadministrator-Rechte verfügt.

  Informationen zum Erstellen eines Benutzers in [!DNL Workfront] finden Sie unter [Benutzer hinzufügen](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

## Erwartete [!DNL Anaplan] Konfiguration

Sie müssen Folgendes in [!DNL Anaplan] haben, um dieses Szenario zu verwenden:

* Ein Benutzerprofil mit dem Namen **[!DNL Workfront]Integration** in [!DNL Anaplan] mit Systemadministrator-Berechtigungen.
* Das [!DNL Anaplan]-Modell, das Sie für dieses Szenario verwenden möchten.
* Die Liste innerhalb des [!DNL Anaplan]-Modells, das Kampagnenbudgets erfasst.

  Das Modul der Liste muss den Empfang der folgenden Attribute unterstützen:

   * [!UICONTROL Workfront Project GUID]
   * [!UICONTROL Kampagnenname]
   * [!UICONTROL Beantragte Arbeitsfonds]
   * [!UICONTROL Geschätzter Umsatz]
   * [!UICONTROL Marke]

  Diese Liste und dieses Modul müssen zusätzliche Details speichern, die für die normale Funktionalität von [!DNL Anaplan] erforderlich sind, einschließlich der Möglichkeit, ein Budget festzulegen und mitzuteilen, dass das Budgetlistenelement bereit ist, wieder mit [!DNL Workfront] synchronisiert zu werden.

* Eine Ansicht in [!DNL Anaplan] namens **[!UICONTROL Campaigns.Update Campaigns in Adobe Workfront]**.

  Diese Ansicht muss die folgenden Spalten in dieser Reihenfolge enthalten:

   1. [!UICONTROL Elementname]

   2. [!UICONTROL [!DNL Workfront] Projekt-GUID]

   3. [!UICONTROL Kampagnenname]

   4. [!UICONTROL Budget]

   5. [!UICONTROL Geschätzter Umsatz]

   6. [!UICONTROL Marke]

  Die Ansicht sollte gefiltert werden, um Elemente mit einer [!UICONTROL [!DNL Workfront] Projekt-GUID] und einem Hinweis darauf anzuzeigen, dass Budgetzuweisungen an [!DNL Workfront] übertragen werden sollen.

Anweisungen zu diesen Aktionen finden Sie in der Dokumentation zu [!DNL Anaplan] .

## Bereitstellen unter [!DNL Workfront Fusion]

Führen Sie die folgenden Schritte aus, um dieses Integrationsszenario in Ihrem [!DNL Fusion]-Konto bereitzustellen. Dies sollte erst nach Abschluss der erforderlichen [!DNL Workfront] - und [!DNL Anaplan] -Konfiguration erfolgen.

1. Navigieren Sie zum Menü [!UICONTROL Vorlagen] in [!DNL Workfront Fusion] und klicken Sie auf die Vorlage **[!UICONTROL Budgetzuweisungen auf Workfront-Projekte anwenden]** .[!DNL Anaplan]
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
      <td role="rowheader">[!UICONTROL [!DNL Anaplan] Modulname]</td> 
      <td>Der Name des Moduls, das die Kampagnenattribute in der ausgewählten [!DNL Anaplan]-Liste beschreibt.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Kampagnenlisten-Name]</td> 
      <td>Der Name der Liste aus Ihrem [!DNL Anaplan] -Konto und der ausgewählte Arbeitsbereich und das ausgewählte Modell.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL Anaplan] Anzeigename]</td> 
      <td> <p>Der Name der Ansicht, die bereit zur Übertragung von Kampagnenbudgets an [!DNL Workfront] enthält.</p> <p>(Beispiel: [!UICONTROL Campaigns.Load Campaigns to [!DNL Adobe Workfront]]) </p> </td> 
     </tr> 
    </tbody> 
   </table>

   Weitere Informationen zum Einrichten der Dateien und Prozesse finden Sie in der Dokumentation zur Einrichtung von [!DNL Anaplan] .

1. Wählen Sie ein Verbindungsprofil vom Typ [!DNL Anaplan] aus oder fügen Sie es hinzu.
1. Aktualisieren Sie bei Aufforderung alle verbleibenden [!DNL Anaplan] -Module mit einer [!DNL Anaplan] -Verbindung.
1. Fügen Sie im Modul **[!UICONTROL CSV in JSON-Objekt konvertieren]** eine neue Datenstruktur hinzu, um die CSV-Spalten einem verwendbaren JSON-Objekt zuzuordnen.

   <!-- [Copy](javascript:void(0);) -->
   <pre><code>[<br>    {<br>        "Anaplan Name":"text",<br>        "Workfront Project GUID":"text",<br>        "Campaign Name":"text",<br>        "Budget": 100.01,<br>        "Estimated Revenue": 100.01,<br>        "Brand":"text"<br>    }<br>]<br></code></pre>

1. Wenn Sie dazu aufgefordert werden, wählen Sie diese Datenstruktur für andere Module in dieser Szenario-Bereitstellung aus.
1. Wählen Sie im Modul **[!UICONTROL Verknüpftes Projekt überprüfen]** ein Verbindungsprofil aus oder fügen Sie es hinzu.[!DNL Workfront]
1. Aktualisieren Sie bei Aufforderung alle verbleibenden [!DNL Workfront] -Module mit einer [!DNL Workfront] -Verbindung.

## Andere empfohlene Szenario-Vorlagen

Um den von dieser Vorlage dargestellten Workflow abzuschließen, müssen Sie außerdem die folgende zusätzliche Vorlage bereitstellen:

* [[!UICONTROL Erstellen eines  [!DNL Anaplan] Listenelements aus einer  [!DNL Adobe Workfront] Budgetanforderung]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-budget-request.md)

Weitere Szenarien für die Ausgabenoptimierung sind:

* [[!UICONTROL Senden von [!DNL Adobe Workfront] Projektaktualisierungen an ein [!DNL Anaplan] Listenelement]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-updates-to-anaplan-list-item.md)

* [[!UICONTROL Sende [!DNL Adobe Workfront] tatsächliche Stunden-Aktualisierungen an ein  [!DNL Anaplan] Listenelement]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-actual-hours-updates-to-anaplan-list-item.md)

* [[!UICONTROL Senden [!DNL Adobe Workfront] der Ausgaben an einen  [!DNL Anaplan] Listeneintrag]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-expenses-to-anaplan-list-item.md)
