---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-with-anaplan
title: Senden von  [!DNL Adobe Workfront] Aufwendungen an einen  [!DNL Anaplan] -Listenelement
description: Dieses Integrationsszenario teilt die aufwendigen Details eines [!DNL Adobe Workfront] Projekts mit einem [!DNL Anaplan] Budgetlistenelement. Durch die Freigabe dieser Informationen können Sie die Ausgabenoptimierung und die Finanzanalyse, die [!DNL Anaplan] bietet, besser nutzen.
author: Becky
feature: Workfront Integrations and Apps, Workfront Fusion
exl-id: f9198017-9bbb-4776-86aa-3f78705dbb22
source-git-commit: 7697327455a7ffdc1a15bfa1676c3a0b091abd04
workflow-type: tm+mt
source-wordcount: '919'
ht-degree: 0%

---

# Senden von [!DNL Adobe Workfront]-Ausgaben an ein [!DNL Anaplan]-Listenelement

Dieses Integrationsszenario teilt die aufwendungen-bezogenen Details eines [!DNL Adobe Workfront] -Projekts mit einem [!DNL Anaplan] Budgetlistenelement. Durch die Freigabe dieser Informationen können Sie die Ausgabenoptimierung und Finanzanalyse, die [!DNL Anaplan] bietet, besser nutzen.

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

* Ein Benutzerprofil mit dem Namen *[!UICONTROL *[!DNL Anaplan] Integration]*** mit Systemadministrator-Berechtigungen.[!DNL Workfront]

  Informationen zum Erstellen eines Benutzers in [!DNL Workfront] finden Sie unter [Benutzer hinzufügen](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

* Ein benutzerdefiniertes **[!UICONTROL Kampagnenbeschreibung]** -Formular, das an das Projektobjekt angehängt ist, um benutzerdefinierte Datenwerte zu speichern, die Sie an [!DNL Anaplan] senden möchten.

  Das Formular muss die folgenden Felder enthalten:

  | Feldname | Feldtyp |
  |---|---|
  | [!UICONTROL Letztes Übermittlungsdatum] | Datum |
  | [!UICONTROL Integrationshinweise] | Absatztextfeld |

  Informationen zum Erstellen benutzerdefinierter Formulare finden Sie unter [Erstellen eines benutzerdefinierten Formulars](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

## Erwartete [!DNL Anaplan] Konfiguration

Sie müssen Folgendes in [!DNL Anaplan] haben, um dieses Szenario zu verwenden:

* Ein Benutzerprofil mit dem Namen **[!UICONTROL [!DNL Workfront]Integration]** in [!DNL Anaplan] mit Systemadministrator-Berechtigungen.
* Das [!DNL Anaplan]-Modell, das Sie für dieses Szenario verwenden möchten.
* Die Liste innerhalb des [!DNL Anaplan]-Modells, das die Kampagnenbudgets erfassen soll.
* Eine **[!UICONTROL Anaplan Tatsächlicher Ausgabenimport]** -Datei, die die folgenden Spalten in dieser Reihenfolge enthält:

   1. [!UICONTROL [!DNL Workfront] AusgabenGUID]

   2. [!UICONTROL [!DNL Workfront] Projekt-GUID]

   3. [!UICONTROL Tatsächlicher Betrag]

   4. [!UICONTROL Beschreibung]

   5. [!UICONTROL Ausgabentyp]

   6. [!UICONTROL  Datum des In-Kraft-Tretens]

   7. [!UICONTROL Kampagnenname]

   8. [!UICONTROL [!DNL Anaplan] Listenelement-ID]

  Vorbereiten der Datei [!UICONTROL [!DNL Anaplan] Tatsächlicher Import von Ausgaben]:

   1. Kopieren Sie Folgendes und fügen Sie es in einen Texteditor oder [!DNL Excel] ein.
   1. Speichern Sie die Datei im CSV-Format.
   1. Laden Sie die Datei in [!DNL Anaplan] hoch.

      Anweisungen finden Sie in der [!DNL Anaplan] -Dokumentation zum Importieren von Daten in Module aus einer Datei.

   1. Notieren Sie sich den Namen, den Sie der Datei gegeben haben. Er wird während der Bereitstellung der Szenario-Vorlage [!UICONTROL Fusion] verwendet.

  Beispiel-CSV-Inhalte

  <!-- [Copy](javascript:void(0);) -->
  <pre><code>"Workfront Expense GUID","Workfront Project GUID","Actual Amount","Description","Expense Type","Effective Date","Campaign Name","Anaplan List Item ID"<br>"622aead400423eb2e4479fece9a72987","6218062a000d0442903fcfa21e11f556","2345","Expense 1","","2022-03-09","New Project 6","202000001030"</code></pre>

* Eine Datei vom Typ **[!UICONTROL [!DNL Anaplan]Geplanter Ausgabenimport]** mit den folgenden Spalten in dieser Reihenfolge:

   1. [!UICONTROL [!DNL Workfront] AusgabenGUID]

   2. [!UICONTROL [!DNL Workfront] Projekt-GUID]

   3. [!UICONTROL Tatsächlicher Betrag]

   4. [!UICONTROL Beschreibung]

   5. [!UICONTROL Ausgabentyp]

   6. [!UICONTROL  Datum des In-Kraft-Tretens]

   7. [!UICONTROL Kampagnenname]

   8. [!UICONTROL [!DNL Anaplan] Listenelement-ID]

  Vorbereiten der Datei [!UICONTROL [!DNL Anaplan] Geplanter Ausgabenimport] :

   1. Kopieren Sie Folgendes und fügen Sie es in einen Texteditor oder [!DNL Excel] ein
   1. Datei im CSV-Format speichern
   1. Laden Sie die Datei in Anaplan hoch.

      Anweisungen finden Sie in der [!DNL Anaplan] -Dokumentation zum Importieren von Daten in Module aus einer Datei.

   1. Notieren Sie sich den Namen, den Sie der Datei gegeben haben. Er wird während der Bereitstellung der Szenario-Vorlage [!UICONTROL Fusion] verwendet.

  Beispiel-CSV-Inhalte

  <!-- [Copy](javascript:void(0);) -->
  <pre><code>"Workfront Expense GUID","Workfront Project GUID","Planned Amount","Description","Expense Type","Planned Date","Campaign Name","Anaplan List Item ID"<br>"622aead400423eb2e4479fece9a72987","6218062a000d0442903fcfa21e11f556","1234","Expense 1","Entertainment","2022-03-08","New Project 6","202000001030"</code></pre>


* Ein **[!UICONTROL Import von Projektaktualisierungen]** -Prozess, der zum Ausführen des Imports von Daten vorbereitet wird, die beim Hochladen einer Datei bereitgestellt wurden.

>[!NOTE]
>
>Es gibt separate Importdateien für geplante und tatsächliche Ausgaben, damit sie unabhängig über ihre geplanten bzw. tatsächlichen Daten gemeldet werden können.

Anweisungen zu diesen Aktionen finden Sie in der Dokumentation zu [!DNL Anaplan] .

## Bereitstellen unter [!DNL Fusion]

Führen Sie die folgenden Schritte aus, um dieses Integrationsszenario in Ihrem [!DNL Fusion]-Konto bereitzustellen. Dies sollte erst nach Abschluss der erforderlichen [!DNL Workfront] - und [!DNL Anaplan] -Konfiguration erfolgen.

1. Navigieren Sie zum Menü [!UICONTROL Vorlagen] in [!DNL Workfront Fusion] und klicken Sie auf die Vorlage **[!UICONTROL Senden von Workfront-Ausgabenaktualisierungen an den Listeneintrag [!DNL Anaplan]]** .
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
      <td>Die ID des Workspace aus Ihrem [!DNL Anaplan]-Konto, das Sie für dieses Szenario verwenden möchten.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL Anaplan] Modell-ID] </td> 
      <td>Die Kennung des Modells aus Ihrem [!DNL Anaplan] -Konto und dem ausgewählten Arbeitsbereich, den Sie für dieses Szenario verwenden möchten.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Kampagnenlisten-Name]</td> 
      <td>Der Name der Liste aus Ihrem [!DNL Anaplan]-Konto sowie der ausgewählte Arbeitsbereich und das Modell, die Sie für dieses Szenario verwenden möchten.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Dateiname: Tatsächlicher Import von Ausgaben]</td> 
      <td> <p>Der Name der Datei, die die tatsächlichen Projektausgaben erhält.</p> <p> (Beispiel: WorkfrontUpdateLinkedProjects_ActExpenses.csv) </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Dateiname: Geplanter Import von Ausgaben]</td> 
      <td> <p>Der Name der Datei, die die geplanten Ausgabedaten des Projekts erhält.</p> <p> (Beispiel: WorkfrontUpdateLinkedProjects_PlannedExpenses.csv) </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Process Name: Project Update Import]</td> 
      <td> <p>Der Name des Prozesses, der den Import von Projektausgabedaten ausführt.</p> <p>(Beispiel: WF Int - Projektausgaben laden)</p> </td> 
     </tr> 
    </tbody> 
   </table>

   Weitere Informationen zum Einrichten der Dateien und Prozesse finden Sie in der Dokumentation zur Einrichtung von [!DNL Anaplan] .

1. Wählen Sie ein Verbindungsprofil vom Typ [!DNL Anaplan] aus oder fügen Sie es hinzu.
1. Aktualisieren Sie bei Aufforderung alle verbleibenden [!DNL Anaplan] -Module mit einer [!DNL Anaplan] -Verbindung.
1. Wählen Sie ein Verbindungsprofil vom Typ [!DNL Workfront] aus oder fügen Sie es hinzu.
1. Aktualisieren Sie bei Aufforderung alle verbleibenden [!DNL Workfront] -Module mit einer [!DNL Workfront] -Verbindung.
1. Fügen Sie im Modul **[!UICONTROL Tatsächliche Ausgaben erstellen CSV]** eine neue Datenstruktur hinzu, um die Projektattribute CSV-Spalten zuzuordnen.

   <!-- [Copy](javascript:void(0);) -->
   <pre><code>[<br>    {<br>        "Workfront Expense GUID":"text",<br>        "Workfront Project GUID":"text",<br>        "Actual Amount": 100.01,<br>        "Description":"text",<br>        "Expense Type":"text",<br>        "Effective Date":"text",<br>        "Campaign Name":"text",<br>        "Anaplan List Item ID": 10000001<br>    }<br>]<br></code></pre>

1. Fügen Sie im Modul **[!UICONTROL Vorgesehene Ausgaben erstellen CSV]** eine neue Datenstruktur hinzu, um die Projektattribute CSV-Spalten zuzuordnen.

   <!-- [Copy](javascript:void(0);) -->
   <pre><code>[<br>    {<br>        "Workfront Expense GUID":"text",<br>        "Workfront Project GUID":"text",<br>        "Planned Amount": 100.01,<br>        "Description":"text",<br>        "Expense Type":"text",<br>        "Planned Date":"text",<br>        "Campaign Name":"text",<br>        "Anaplan List Item ID": 10000001<br>    }<br>]<br></code></pre>

## Andere empfohlene Szenario-Vorlagen

Diese Szenario-Vorlage wird durch die folgenden Ausgabenoptimierungsszenarien ergänzt, die ebenfalls bereitgestellt werden können:

* [[!UICONTROL Senden von [!DNL Adobe Workfront] Projektaktualisierungen an ein [!DNL Anaplan] Listenelement]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-updates-to-anaplan-list-item.md)
* [[!UICONTROL Sende [!DNL Adobe Workfront] tatsächliche Stunden-Aktualisierungen an ein  [!DNL Anaplan] Listenelement]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-actual-hours-updates-to-anaplan-list-item.md)

Zusätzliche Szenarien für die Verknüpfung von Budgetanforderungen:

* [[!UICONTROL Erstellen eines  [!DNL Anaplan] Listenelements aus einer  [!DNL Adobe Workfront] Budgetanforderung]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-budget-request.md)
* [[!UICONTROL Anwenden einer [!DNL Anaplan] Budgetzuordnung auf ein [!DNL Adobe Workfront] Projekt]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-projects.md)

Zusätzliche Szenarien für die Verknüpfung von Kampagnenanforderungen:

* [[!UICONTROL Erstellen eines  [!DNL Anaplan] Listenelements aus einer [!DNL Adobe Workfront] Kampagnenanforderung]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-campaign-request.md)
* [[!UICONTROL Anwenden einer [!DNL Anaplan] Budgetzuordnung auf eine [!DNL Adobe Workfront] Kampagnenanforderung oder ein Kampagnenprojekt]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-campaign-requests-and-projects.md)
