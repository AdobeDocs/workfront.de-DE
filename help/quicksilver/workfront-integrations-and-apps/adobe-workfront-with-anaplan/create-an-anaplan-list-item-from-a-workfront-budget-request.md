---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-with-anaplan
title: 'Erstellen  [!DNL Anaplan]  Listenelements aus einer  [!DNL Adobe Workfront] '
description: Dieses Integrationsszenario verknüpft ein Projekt [!DNL Adobe Workfront] Projekt (Kampagne) mit einem  [!DNL Anaplan] -Budgetlistenelement. Dies wird erreicht, indem eine Budgetanforderung zu dem Projekt hinzugefügt  [!DNL Workfront] , das Finanzmittel erhalten muss. Dieses Szenario überwacht nicht verarbeitete Budgetanfragen und führt dann einen Prozess aus, um ein leeres Budgetlistenelement in zu erstellen [!DNL Anaplan]  um Budgetzuordnungsprozesse in Anaplan zu starten.
author: Becky
feature: Workfront Integrations and Apps, Workfront Fusion
exl-id: e6505ece-21aa-4397-8d68-543bf89d2f00
source-git-commit: 53596271a838733b858c0b14a4e22b07a7cd20f6
workflow-type: tm+mt
source-wordcount: '854'
ht-degree: 14%

---

# Erstellen eines [!DNL Anaplan] Listenelements aus einer [!DNL Adobe Workfront] Budgetanforderung

Dieses Integrationsszenario verknüpft ein [!DNL Adobe Workfront] Projekt (Kampagne) mit einem [!DNL Anaplan] Budgetlistenelement. Dies wird erreicht, indem dem [!DNL Workfront]-Projekt, das Finanzmittel erhalten muss, eine Budgetanforderung hinzugefügt wird. In diesem Szenario werden nicht verarbeitete Budgetanfragen überwacht und dann ein Prozess ausgeführt, um einen leeren Budgetlisteneintrag zu erstellen, [!DNL Anaplan] Budgetzuordnungsprozesse in [!DNL Anaplan] zu starten.

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

Informationen zu Adobe Workfront Fusion-Lizenzen finden Sie unter [Adobe Workfront Fusion-Lizenzen](https://experienceleague.adobe.com/de/docs/workfront-fusion/using/set-up-and-manage-fusion/licensing-and-operations-overviews/license-automation-vs-integration).

+++

## Auslösendes Ereignis

Dieses Szenario ist so geplant, dass es alle 15 Minuten ausgeführt wird.

## Erwartete [!DNL Workfront]

Sie müssen über Folgendes verfügen, [!DNL Workfront] dieses Szenario verwenden zu können:

* Ein Benutzerprofil in [!DNL Workfront] mit dem Namen **[!DNL Anaplan]Integration**, das über Systemadministratorrechte verfügt.

  Informationen zum Erstellen eines Benutzers in [!DNL Workfront] finden Sie unter [Benutzer hinzufügen](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

* Ein **[!UICONTROL Budgetanfrage]** benutzerdefiniertes Formular, das an das [!UICONTROL Anfrage]-Objekt angehängt ist.

  Die folgenden erforderlichen Felder müssen im benutzerdefinierten Formular enthalten sein, um bei der Datenzuordnung zu [!DNL Anaplan] zu helfen:

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
     <td role="rowheader">[!UICONTROL Budgetanforderungstyp]</td> 
     <td> <p>[!UICONTROL Dropdown]</p> <p>Optionen:</p> 
      <ul> 
       <li> <p>[!UICONTROL Anpassung der Finanzierung]</p> </li> 
       <li> <p>[!UICONTROL Erstfinanzierung]</p> </li> 
      </ul> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL angeforderte Arbeitsmittel]</td> 
     <td> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL hat Ausgabenmittel angefordert]</td> 
     <td> </td> 
    </tr> 
   </tbody> 
  </table>

  Informationen zum Erstellen benutzerdefinierter Formulare finden Sie unter [Erstellen eines benutzerdefinierten Formulars](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

* Projektvorlagen, die Kampagnen und andere finanzierungspflichtige Projekte darstellen, konfiguriert mit einem Warteschlangenthema [!UICONTROL Budgetanfrage]. Das [!UICONTROL Budgetanfrage] Warteschlangenthema ist zugewiesen, um das benutzerdefinierte [!UICONTROL Budgetanfrage] zu verwenden.
* Ein **[!UICONTROL Kampagnenübersicht]**-Formular für das Projektobjekt.

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
     <td role="rowheader">[!UICONTROL in Market Start Date]</td> 
     <td>[!UICONTROL Datum] </td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL in Market End Date]</td> 
     <td>[!UICONTROL Datum]</td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL Kampagnenübersicht]</td> 
     <td>[!UICONTROL Rich-Text-Feld]</td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL Schlüsselmeldung]</td> 
     <td>[!UICONTROL Rich-Text-Feld]</td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL Zielgruppe]</td> 
     <td> <p>[!UICONTROL Dropdown]</p> <p>Optionen einschließen, die zu Ihren Prozessen passen.</p> </td> 
    </tr> 
   </tbody> 
  </table>

  Informationen zum Erstellen benutzerdefinierter Formulare finden Sie unter [Erstellen eines benutzerdefinierten Formulars](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

## Erwartete [!DNL Anaplan]

Sie müssen über Folgendes verfügen, [!DNL Anaplan] dieses Szenario verwenden zu können:

* Ein Benutzerprofil in [!DNL Anaplan] mit dem Namen **[!UICONTROL [!DNL Workfront]Integration]**, das über Systemadministratorrechte verfügt.
* Das [!DNL Anaplan], das Sie für dieses Szenario verwenden möchten.
* Die Liste innerhalb des [!DNL Anaplan], das Kampagnenbudgets erfasst.

  Das -Modul der Liste muss den Empfang der folgenden Attribute unterstützen:

   * [!UICONTROL Workfront-Projekt-GUID]
   * [!UICONTROL Kampagnenname]
   * [!UICONTROL Beantragte Arbeitsmittel]
   * [!UICONTROL Angeforderte Ausgabenmittel]
   * [!UICONTROL Budgetanfragetyp]
   * [!UICONTROL Grund für die Finanzierungsanpassung]

  Diese Liste und dieses Modul müssen zusätzliche Details speichern, die für die normale Funktionalität von [!DNL Anaplan] erforderlich sind, einschließlich der Möglichkeit, ein Budget festzulegen und mitzuteilen, dass das Budgetlistenelement bereit ist, wieder mit [!DNL Workfront] synchronisiert zu werden.

Anweisungen zu diesen Aktionen finden Sie in der [!DNL Anaplan]-Dokumentation.

## Bereitstellen für [!DNL Workfront Fusion]

Führen Sie die folgenden Schritte aus, um dieses Integrationsszenario in Ihrem [!DNL Fusion]-Konto bereitzustellen. Dies sollte erst nach Abschluss der erforderlichen [!DNL Workfront]- und [!DNL Anaplan]-Konfiguration erfolgen.

1. Navigieren Sie zum Menü [!UICONTROL Vorlagen] in [!DNL Workfront Fusion] und klicken Sie auf die **[!UICONTROL Erstellen eines [!DNL Anaplan] Listenelements aus einer Workfront-]**).
1. Ersetzen Sie die Variablenwerte für die folgenden [!DNL Anaplan]:

   | Variablenname | Wert ersetzen durch |
   |---|---|
   | [!UICONTROL [!DNL Anaplan] Workspace ID] | Die ID eines Arbeitsbereichs aus Ihrem [!DNL Anaplan]. |
   | [!UICONTROL [!DNL Anaplan]-Modell-ID] | Die ID eines Modells aus Ihrem [!DNL Anaplan] und dem ausgewählten Arbeitsbereich. |
   | [!UICONTROL [!DNL Anaplan] Modulname] | Der Name des Moduls, das die Kampagnenattribute in der ausgewählten [!DNL Anaplan] beschreibt. |
   | [!UICONTROL Name der Kampagnenliste] | Der Name der Liste aus Ihrem [!DNL Anaplan] und dem ausgewählten Arbeitsbereich und Modell. |

   {style="table-layout:auto"}

   Einzelheiten zum Einrichten der Dateien und Prozesse finden Sie in der Dokumentation zur [!DNL Anaplan].

1. Wählen Sie ein [!DNL Anaplan] Verbindungsprofil aus oder fügen Sie es hinzu.
1. Aktualisieren Sie alle verbleibenden [!DNL Anaplan]-Module mit einer [!DNL Anaplan] Verbindung, wenn Sie dazu aufgefordert werden.
1. Wählen Sie ein [!DNL Workfront] Verbindungsprofil aus oder fügen Sie es hinzu.

   Nach Bereitstellung der Vorlage aktualisieren Sie dieses Modul, um benutzerdefinierte Feldverweise zum Wert der Eigenschaft fields hinzuzufügen oder daraus zu entfernen, wenn Sie die standardmäßig zugeordneten Felder in [!DNL Anaplan] ändern möchten.

1. Aktualisieren Sie alle verbleibenden [!DNL Workfront]-Module mit einer [!DNL Workfront] Verbindung, wenn Sie dazu aufgefordert werden.

## Andere empfohlene Szenariovorlagen

Um den durch diese Vorlage dargestellten Workflow abzuschließen, müssen Sie auch die folgende zusätzliche Vorlage bereitstellen:

* [[!UICONTROL Budgetzuweisung  [!DNL Anaplan]  ein Projekt  [!DNL Adobe Workfront] &#x200B;]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-projects.md)

Weitere Szenarien für die Ausgabenoptimierung sind:

* [[!UICONTROL Projektaktualisierungen  [!DNL Adobe Workfront]  ein  [!DNL Anaplan]  senden]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-updates-to-anaplan-list-item.md)
* [[!UICONTROL Senden von  [!DNL Adobe Workfront] -Stunden-Aktualisierungen an ein  [!DNL Anaplan] -Element]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-actual-hours-updates-to-anaplan-list-item.md)
* [[!UICONTROL Senden [!DNL Adobe Workfront] Ausgaben an  [!DNL Anaplan] /Listenelement]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-expenses-to-anaplan-list-item.md)
