---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-with-anaplan
title: Senden von [!DNL Adobe Workfront] Projektaktualisierungen an ein [!DNL Anaplan] Listenelement
description: Dieses Integrationsszenario teilt Fortschritt, Status und wichtige Zeitplandetails aus einem [!DNL Adobe Workfront] Projekt mit einem [!DNL Anaplan] Budgetlistenelement. Durch die Freigabe dieser Informationen können Sie die Ausgabenoptimierung und die Finanzanalyse, die [!DNL Anaplan] bietet, besser nutzen.
author: Becky
feature: Workfront Integrations and Apps, Workfront Fusion
exl-id: 97e9dac6-f5b5-4d6e-b58b-93acd19048ee
source-git-commit: 1ae65d18419bf4235a7c97614b539811643110cc
workflow-type: tm+mt
source-wordcount: '912'
ht-degree: 0%

---

# Senden von [!DNL Adobe Workfront] -Projektaktualisierungen an ein [!DNL Anaplan] -Listenelement

Dieses Integrationsszenario teilt Fortschritt, Status und wichtige Zeitplandetails aus einem [!DNL Adobe Workfront] -Projekt mit einem [!DNL Anaplan] -Budgetlistenelement. Durch die Freigabe dieser Informationen können Sie die Ausgabenoptimierung und Finanzanalyse, die [!DNL Anaplan] bietet, besser nutzen.

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
   <td> <p>Workfront Fusion für Arbeitsautomatisierung und -integration </p> </td> 
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

* Ein Benutzerprofil mit dem Namen **[!UICONTROL [!DNL Anaplan]Integration]** in [!DNL Workfront] mit Systemadministrator-Berechtigungen.

  Informationen zum Erstellen eines Benutzers in [!DNL Workfront] finden Sie unter [Benutzer hinzufügen](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

* Ein benutzerdefiniertes **[!UICONTROL Kampagnenbeschreibung]** -Formular, das an das Projektobjekt angehängt ist, um benutzerdefinierte Datenwerte zu speichern, die Sie an Anaplan senden möchten.

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

  Informationen zum Erstellen benutzerdefinierter Formulare finden Sie unter [Entwerfen eines Formulars mit dem Formularentwickler](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

<!--
<note type="note">  
<p>The above configuration is available through the Marketing Financial Management Configuration blueprint:</p>
<p>https://MYDOMAIN.my.workfront.com/blueprints/7ebe85c4-05a1-4efe-a018-50ee55f5654c/details </p>
<p><span style="color: #ff0000;">This note is currently not marked for publication.</span> </p>
</note>
-->

## Erwartete [!DNL Anaplan] Konfiguration

Sie müssen Folgendes in [!DNL Anaplan] haben, um dieses Szenario zu verwenden:

* Ein Benutzerprofil mit dem Namen **[!UICONTROL [!DNL Workfront]Integration]** in [!DNL Anaplan] mit Systemadministrator-Berechtigungen.
* Das [!DNL Anaplan]-Modell, das Sie für dieses Szenario verwenden möchten.
* Die Liste innerhalb des [!DNL Anaplan]-Modells, das Sie für dieses Szenario verwenden möchten.
* Eine Datei vom Typ **[!UICONTROL Import des Projekts aktualisieren]** mit den folgenden Spalten in dieser Reihenfolge:

1. [!UICONTROL itemID]

2. [!UICONTROL [!DNL Workfront] Projekt-GUID]

3. [!UICONTROL Kampagnenname]

4. [!UICONTROL Prozent abgeschlossen]

5. [!UICONTROL Geplantes Startdatum]

6. [!UICONTROL Geplantes Abschlussdatum]

7. [!UICONTROL Geplante Stunden]

8. [!UICONTROL Geplante Kosten]

9. [!UICONTROL Geplante Kosten]

10. [!UICONTROL Tatsächliche Arbeitskosten]

11. [!UICONTROL Geplante Arbeitskosten]

12. [!UICONTROL Status]

Vorbereiten der Datei [!UICONTROL [!DNL Anaplan] Geplanter Ausgabenimport] :

1. Kopieren Sie Folgendes und fügen Sie es in einen Texteditor oder [!DNL Excel] ein
1. Datei im CSV-Format speichern
1. Laden Sie die Datei in Anaplan hoch.

   Anweisungen finden Sie in der [!DNL Anaplan] -Dokumentation zum Importieren von Daten in Module aus einer Datei.

1. Notieren Sie sich den Namen, den Sie der Datei gegeben haben. Er wird während der Bereitstellung der Szenario-Vorlage [!UICONTROL Fusion] verwendet.

Beispiel-CSV-Inhalte

<!-- [Copy](javascript:void(0);) -->
<pre><code>"itemID","Workfront Project GUID","Campaign Name","Percent Complete","Planned Start Date","Planned Completion Date","Planned Hours","Planned Cost","Planned Expense Cost","Actual Labor Cost","Planned Labor Cost","Status","Campaign Overview","Key Message","In Market Start Date","In Market End Date","Target Audience"<br>"202000001019","6182bc1f0025e184b2c00d9205e22c49","Launch Be U APAC Styles Catalog","0","2022-03-31","2022-05-31","88.25","0","0","0","0","Planning","","","","",""</code></pre>Optionale Spalten können Folgendes umfassen:

1. [!UICONTROL Kampagnenübersicht]

2. [!UICONTROL Schlüsselmeldung]

3. [!UICONTROL  In Market Start Date]

4. [!UICONTROL In Market-End-Datum]

5. [!UICONTROL Target-Zielgruppe]

Schließen Sie auch alle anderen Felder ein, die Sie in der Zuordnung festlegen möchten.

* Ein **[!UICONTROL Import von Projektaktualisierungen]** -Prozess, der zum Ausführen des Imports von Daten vorbereitet wird, die beim Hochladen einer Datei bereitgestellt wurden.

Anweisungen zu diesen Aktionen finden Sie in der Dokumentation zu [!DNL Anaplan] .

## Bereitstellen unter [!DNL Workfront Fusion]

Führen Sie die folgenden Schritte aus, um dieses Integrationsszenario in Ihrem Fusion-Konto bereitzustellen. Dies sollte erst nach Abschluss der erforderlichen [!DNL Workfront] - und [!DNL Anaplan] -Konfiguration erfolgen.

1. Navigieren Sie zum Menü [!UICONTROL Vorlagen] in [!DNL Workfront Fusion] und klicken Sie auf die Vorlage **[!UICONTROL Workfront-Projektaktualisierungen an [!DNL Anaplan] Listenelement senden]** .
1. Ersetzen Sie die Variablenwerte für die folgenden [!DNL Anaplan] -Variablen:

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
      <td role="rowheader">[!UICONTROL Dateiname: Import von Projektaktualisierungen]</td> 
      <td>Der Name der Datei, an die die Projekt-Update-Daten gesendet werden.<p>(Beispiel: WorkfrontUpdateLinkedProject.csv)</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Process Name: Project Update Import]</td> 
      <td> <p>Der Name des Prozesses, der den Import von Projektdaten ausführt.</p> <p>(Beispiel: WF Int - Update der Kampagnendetails)</p> </td> 
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

   Der Filter ist so konfiguriert, dass er alle unvollständigen verknüpften Projekte und Projekte abruft, die in den letzten 29 Minuten abgeschlossen wurden. Wenn Sie die Häufigkeit des [!DNL Fusion] -Szenarios ändern, sollten Sie diesen Wert aktualisieren, sobald die Szenario-Vorlage bereitgestellt wurde.

1. Fügen Sie im Modul **[!UICONTROL Projekte erstellen - Aktualisierung von CSV]** eine neue Datenstruktur hinzu, um die Projektattribute CSV-Spalten zuzuordnen.

   <!-- [Copy](javascript:void(0);) -->
   <pre><code>[<br>    {<br>        "itemID": 1000001,<br>        "Workfront Project GUID":"text",<br>        "Campaign Name":"text",<br>        "Percent Complete": 10.01,<br>        "Planned Start Date":"2022-02-22",<br>        "Planned Completion Date":"2022-02-22",<br>        "Planned Hours": 12.5,<br>        "Planned Cost": 123.45,<br>        "Planned Expense Cost": 123.45,<br>        "Planned Labor Cost": 123.45,<br>        "Status": "CUR",<br>        "Campaign Overview":"text",<br>        "Key Message":"text",<br>        "In Market Start Date":"2022-02-22",<br>        "In Market End Date":"2022-02-22",<br>        "Target Audience":"text"<br>    }<br>]<br></code></pre>

1. Aktualisieren Sie bei Aufforderung alle verbleibenden [!DNL Workfront] -Module mit einer [!DNL Workfront] -Verbindung.

## Andere empfohlene Szenario-Vorlagen

Diese Szenario-Vorlage wird durch die folgenden Ausgabenoptimierungsszenarien ergänzt, die ebenfalls bereitgestellt werden können:

* [[!UICONTROL Sende [!DNL Adobe Workfront] tatsächliche Stunden-Aktualisierungen an ein  [!DNL Anaplan] Listenelement]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-actual-hours-updates-to-anaplan-list-item.md)
* [[!UICONTROL Senden [!DNL Adobe Workfront] der Ausgaben an einen  [!DNL Anaplan] Listeneintrag]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-expenses-to-anaplan-list-item.md)

Zusätzliche Szenarien für die Verknüpfung von Budgetanforderungen:

* [[!UICONTROL Erstellen eines  [!DNL Anaplan] Listenelements aus einer  [!DNL Adobe Workfront] Budgetanforderung]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-budget-request.md)
* [[!UICONTROL Anwenden einer [!DNL Anaplan] Budgetzuordnung auf ein [!DNL Adobe Workfront] Projekt]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-projects.md)

Zusätzliche Szenarien für die Verknüpfung von Kampagnenanforderungen:

* [[!UICONTROL Erstellen eines  [!DNL Anaplan] Listenelements aus einer [!DNL Adobe Workfront] Kampagnenanforderung]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-campaign-request.md)
* [[!UICONTROL Anwenden einer [!DNL Anaplan] Budgetzuordnung auf eine [!DNL Adobe Workfront] Kampagnenanforderung oder ein Kampagnenprojekt]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-campaign-requests-and-projects.md)
