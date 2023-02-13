---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-with-anaplan
title: Erstellen Sie eine [!DNL Anaplan] Listenelement aus [!DNL Adobe Workfront] Budgetanfrage
description: Dieses Integrationsszenario verknüpft eine [!DNL Adobe Workfront] Projekt (Kampagne) mit einer [!DNL Anaplan] Budgetlisteneintrag. Dies wird erreicht, indem eine Budgetanforderung zum [!DNL Workfront] Projekt, für das eine Finanzierung erforderlich ist. Dieses Szenario überwacht nicht verarbeitete Budgetanforderungen und führt dann einen Prozess aus, um ein leeres Budgetlistenelement in [!DNL Anaplan] zur Einleitung von Haushaltszuweisungsverfahren in Anaplan.
author: Becky
feature: Workfront Integrations and Apps, Workfront Fusion
exl-id: e6505ece-21aa-4397-8d68-543bf89d2f00
source-git-commit: 4ab731b14dc5435386fd0d887501788fa37223a2
workflow-type: tm+mt
source-wordcount: '810'
ht-degree: 1%

---

# Erstellen Sie eine [!DNL Anaplan] Listenelement aus [!DNL Adobe Workfront] Budgetanfrage

Dieses Integrationsszenario verknüpft eine [!DNL Adobe Workfront] Projekt (Kampagne) mit einer [!DNL Anaplan] Budgetlisteneintrag. Dies wird erreicht, indem eine Budgetanforderung zum [!DNL Workfront] Projekt, für das eine Finanzierung erforderlich ist. Dieses Szenario überwacht nicht verarbeitete Budgetanforderungen und führt dann einen Prozess aus, um ein leeres Budgetlistenelement in [!DNL Anaplan] zur Einleitung von Verfahren zur Zuweisung von Budgets in [!DNL Anaplan].

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
   <td role="rowheader" [!DNL>Adobe Workfront Fusion]-Lizenz**</td> 
   <td> <p>[!UICONTROL Workfront Fusion für Arbeitsautomatisierung und -integration] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] sowie [!DNL Adobe Workfront] , um die in diesem Artikel beschriebenen Funktionen zu verwenden.</td> 
  </tr>
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren [!DNL Workfront] Administrator.

&#42;&#42;Informationen über[!DNL  Adobe Workfront Fusion] Lizenzen, siehe [[!DNL Adobe Workfront Fusion] Lizenzen](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Auslösen eines Ereignisses

Dieses Szenario wird alle 15 Minuten ausgeführt.

## Erwartet [!DNL Workfront] Konfiguration

Sie müssen Folgendes in der [!DNL Workfront] um dieses Szenario zu verwenden:

* Ein Benutzerprofil in [!DNL Workfront] benannt *[!UICONTROL *[!DNL Anaplan] Integration]**, das über Systemadministratorrechte verfügt.

   Informationen zum Erstellen eines Benutzers in [!DNL Workfront], siehe [Benutzer hinzufügen](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

* A **[!UICONTROL Budgetanfrage]** benutzerdefiniertes Formular, das an das [!UICONTROL Anfrage] -Objekt.

   Die folgenden erforderlichen Felder müssen in das benutzerdefinierte Formular eingefügt werden, damit die Datenzuordnung zu [!DNL Anaplan]:

   <table style="table-layout:auto"> 
   <col> 
   </col> 
   <col> 
   </col> 
   <thead> 
    <tr> 
     <th>Feldname</th> 
     <th>Feldtyp</th> 
    </tr> 
   </thead> 
   <tbody> 
    <tr> 
     <td role="rowheader">[!UICONTROL Budgetanfragetyp]</td> 
     <td> <p>[!UICONTROL Dropdown]</p> <p>Optionen:</p> 
      <ul> 
       <li> <p>[!UICONTROL Anpassung an die Finanzierung]</p> </li> 
       <li> <p>[!UICONTROL Ursprüngliche Finanzierung]</p> </li> 
      </ul> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL Beantragter Arbeitsfonds]</td> 
     <td> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL Angeforderte Ausgabenfonds]</td> 
     <td> </td> 
    </tr> 
   </tbody> 
  </table>

   Informationen zum Erstellen benutzerdefinierter Formulare finden Sie unter [Benutzerdefiniertes Formular erstellen oder bearbeiten](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md)

* Projektvorlagen, die Kampagnen und andere Projekte darstellen, für die eine Finanzierung erforderlich ist, konfiguriert mit einer [!UICONTROL Budgetanfrage] Warteschlangenthema. Die [!UICONTROL Budgetanfrage] das Warteschlangenthema zugewiesen wird, um [!UICONTROL Budgetanfrage] benutzerdefiniertes Formular.
* A **[!UICONTROL Kampagnenbeschreibung]** Formular für das Projektobjekt.

   Dieses Formular muss die folgenden Felder enthalten:

   <table style="table-layout:auto"> 
   <col> 
   </col> 
   <col> 
   </col> 
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
     <td>[!UICONTROL Rich-Text-Feld]</td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL Schlüsselmeldung]</td> 
     <td>[!UICONTROL Rich-Text-Feld]</td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL Target Audience]</td> 
     <td> <p>[!UICONTROL Dropdown]</p> <p>Schließen Sie Optionen ein, die zu Ihren Prozessen passen.</p> </td> 
    </tr> 
   </tbody> 
  </table>

   Informationen zum Erstellen benutzerdefinierter Formulare finden Sie unter [Benutzerdefiniertes Formular erstellen oder bearbeiten](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md)

## Erwartet [!DNL Anaplan] Konfiguration

Sie müssen Folgendes in der [!DNL Anaplan] um dieses Szenario zu verwenden:

* Ein Benutzerprofil in [!DNL Anaplan] benannt **[!UICONTROL [!DNL Workfront]Integration]**, der über Systemadministratorberechtigungen verfügt.
* Die [!DNL Anaplan] Modell, das Sie für dieses Szenario verwenden möchten.
* Die Liste innerhalb der [!DNL Anaplan] Modell, das Kampagnenbudgets erfasst.

   Das Modul der Liste muss den Empfang der folgenden Attribute unterstützen:

   * [!UICONTROL Workfront-Projekt-GUID]
   * [!UICONTROL Name der Kampagne]
   * [!UICONTROL Beantragte Arbeitsfonds]
   * [!UICONTROL Beantragte Ausgabenfonds]
   * [!UICONTROL Budgetanforderungstyp]
   * [!UICONTROL Grund für die Anpassung der Finanzmittel]

   Diese Liste und dieses Modul müssen zusätzliche Details speichern, die für die normale Funktionalität von [!DNL Anaplan], einschließlich der Möglichkeit, ein Budget festzulegen und mitzuteilen, dass das Budgetlistenelement zur erneuten Synchronisierung mit [!DNL Workfront].

Anweisungen zu diesen Aktionen finden Sie in der [!DNL Anaplan] Dokumentation.

## Bereitstellen unter [!DNL Workfront Fusion]

Führen Sie die folgenden Schritte aus, um dieses Integrationsszenario für Ihre [!DNL Fusion] -Konto. Dies sollte nur nach Abschluss der erforderlichen [!DNL Workfront] und [!DNL Anaplan] Konfiguration.

1. Navigieren Sie zum [!UICONTROL Vorlagen] Menü in [!DNL Workfront Fusion] und klicken Sie auf **[!UICONTROL Erstellen Sie eine [!DNL Anaplan] Listenelement aus einer Workfront-Budgetanfrage]** Szenario.
1. Ersetzen Sie die Variablenwerte für Folgendes [!DNL Anaplan] Variablen:

   | Variablenname | Wert ersetzen durch |
   |---|---|
   | [!UICONTROL [!DNL Anaplan] Workspace-ID] | Die ID eines Arbeitsbereichs aus Ihrer [!DNL Anaplan] -Konto. |
   | [!UICONTROL [!DNL Anaplan] Modell-ID] | Die Kennung eines Modells aus Ihrer [!DNL Anaplan] und dem ausgewählten Arbeitsbereich. |
   | [!UICONTROL [!DNL Anaplan] Modulname] | Der Name des Moduls, das die Kampagnenattribute in der ausgewählten [!DNL Anaplan] Liste. |
   | [!UICONTROL Kampagnenlisten-Name] | Der Name der Liste aus Ihrem [!DNL Anaplan] und dem ausgewählten Arbeitsbereich und Modell. |

   {style=&quot;table-layout:auto&quot;}

   Weitere Informationen zum Einrichten der Dateien und Prozesse finden Sie im Abschnitt [!DNL Anaplan] Dokumentation einrichten.

1. Auswählen oder Hinzufügen von [!DNL Anaplan] Verbindungsprofil.
1. Alle verbleibenden aktualisieren [!DNL Anaplan] Module mit einer [!DNL Anaplan] Verbindung, wenn Sie dazu aufgefordert werden.
1. Auswählen oder Hinzufügen von [!DNL Workfront] Verbindungsprofil.

   Nach der Bereitstellung der Vorlage wird dieses Modul aktualisiert, um benutzerdefinierte Feldverweise aus dem Wert der Feldeigenschaft hinzuzufügen oder daraus zu entfernen, wenn Sie die standardmäßig zugeordneten Felder ändern möchten zu [!DNL Anaplan].

1. Alle verbleibenden aktualisieren [!DNL Workfront] Module mit [!DNL Workfront] Verbindung, wenn Sie dazu aufgefordert werden.

## Andere empfohlene Szenario-Vorlagen

Um den von dieser Vorlage dargestellten Workflow abzuschließen, müssen Sie außerdem die folgende zusätzliche Vorlage bereitstellen:

* [[!UICONTROL Anwenden eines [!DNL Anaplan] Mittelzuweisung an [!DNL Adobe Workfront] Projekt]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-projects.md)

Weitere Szenarien für die Ausgabenoptimierung sind:

* [[!UICONTROL Senden [!DNL Adobe Workfront] Projekt-Updates für [!DNL Anaplan] Listenelement]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-updates-to-anaplan-list-item.md)
* [[!UICONTROL Senden [!DNL Adobe Workfront] Aktualisierungen der tatsächlichen Stunden für eine [!DNL Anaplan] Listenelement]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-actual-hours-updates-to-anaplan-list-item.md)
* [[!UICONTROL Senden [!DNL Adobe Workfront] Kosten für [!DNL Anaplan] Listenelement]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-expenses-to-anaplan-list-item.md)
