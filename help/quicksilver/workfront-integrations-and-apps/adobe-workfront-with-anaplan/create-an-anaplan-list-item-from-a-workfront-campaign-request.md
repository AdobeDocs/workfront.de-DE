---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-with-anaplan
title: Erstellen  [!DNL Anaplan]  Listenelements aus einer  [!DNL Adobe Workfront] -Anfrage
description: Dieses Integrationsszenario verknüpft ein Projekt  [!DNL Adobe Workfront]  einem  [!DNL Anaplan] .
author: Becky
feature: Workfront Integrations and Apps, Workfront Fusion
exl-id: daf6a18d-a3df-497d-a612-8a4645b1a8c9
source-git-commit: cb38223c4dd8048fd2ab105abce2c9a79b84c43f
workflow-type: tm+mt
source-wordcount: '730'
ht-degree: 2%

---

# Erstellen eines [!DNL Anaplan] Listenelements aus einer [!DNL Adobe Workfront] Kampagnenanfrage

Dieses Integrationsszenario verknüpft ein [!DNL Adobe Workfront] Projekt mit einem [!DNL Anaplan] Budgetlistenelement.

In diesem Szenario wird nach neuen Kampagnenanfragen gesucht, die einer Anfragewarteschlange hinzugefügt werden. Sobald eine Kampagnenanfrage erfasst wird, wird ein Budgetposten hinzugefügt, [!DNL Anaplan] der Finanzierungsprozess zu starten.

>[!IMPORTANT]
>
>„Kampagne“ in diesem Artikel bezieht sich auf den Anwendungsfall der Marketing-Kampagne, den dieses Szenario darstellt, und ist in keiner Weise mit dem [!DNL Workfront Fusion] Adobe Campaign-Connector oder dem kürzlich veralteten Objekt [!UICONTROL Kampagne] in [!DNL Workfront] verbunden.

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Funktion in diesem Artikel verwenden zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront] Plan*</td> 
   <td> <p>[!UICONTROL Pro] oder höher</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] Lizenz*</td> 
   <td> <p>[!UICONTROL -Plan], [!UICONTROL -Arbeit]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] Lizenz **</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] für Arbeitsautomatisierung und -integration] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] erwerben und [!DNL Adobe Workfront], die in diesem Artikel beschriebenen Funktionen zu nutzen.</td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren [!DNL Workfront], um herauszufinden, über welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie verfügen.

&#42;&#42;Informationen zu [!DNL Adobe Workfront Fusion] finden Sie unter [[!DNL Adobe Workfront Fusion] Lizenzen](https://experienceleague.adobe.com/de/docs/workfront-fusion/using/set-up-and-manage-fusion/licensing-and-operations-overviews/license-automation-vs-integration).

## Auslösendes Ereignis

Dieses Szenario ist so geplant, dass es alle 15 Minuten ausgeführt wird.

## Erwartete [!DNL Workfront]

Sie müssen über Folgendes verfügen, [!DNL Workfront] dieses Szenario verwenden zu können:

* Ein Benutzerprofil in [!DNL Workfront] mit dem Namen **[!UICONTROL [!DNL Anaplan]Integration]**, das über Systemadministratorrechte verfügt.

  Informationen zum Erstellen eines Benutzers in [!DNL Workfront] finden Sie unter [Benutzer hinzufügen](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

* Ein **[!UICONTROL Kampagnenübersicht]** benutzerdefiniertes Formular, das an das [!UICONTROL Anfrage]-Objekt angehängt ist.

  Die folgenden erforderlichen Felder müssen im benutzerdefinierten Formular enthalten sein, um die Datenzuordnung zu Anaplan zu unterstützen:

  | Feldname | Feldtyp |
  |---|---|
  | [!UICONTROL Insgesamt beantragte Mittel] |   |
  | [!UICONTROL Beantragte Arbeitsmittel] |   |
  | [!UICONTROL Angeforderte Ausgabenmittel] |   |
  | [!UICONTROL An [!DNL Anaplan]] gesendet | Kontrollkästchen |

  Die folgenden optionalen Felder können im Formular vorhanden sein. In diesem Szenario werden nur die oben genannten Felder zugeordnet, es können jedoch auch alle weiteren Felder auf der Kampagnenübersicht zugeordnet werden.

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
     <td role="rowheader">[!UICONTROL in Market Start Date]</td> 
     <td>Datum </td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL in Market End Date]</td> 
     <td>Datum</td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL Kampagnenübersicht]</td> 
     <td>Absatztextfeld</td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL Schlüsselmeldung]</td> 
     <td>Absatztextfeld</td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL Zielgruppe]</td> 
     <td> <p>Dropdown</p> <p>Optionen einschließen, die zu Ihren Prozessen passen.</p> </td> 
    </tr> 
   </tbody> 
  </table>

  Informationen zum Erstellen benutzerdefinierter Formulare finden Sie unter [Erstellen eines benutzerdefinierten Formulars](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

* Ein Projekt, das als Anfrage-Warteschlange eingerichtet wird, um neue Kampagnen-Anfragen zu erfassen. Diesen [!UICONTROL &#x200B; muss &#x200B;] Formular „Kampagnenbeschreibung“ beigefügt werden.

## Erwartete [!DNL Anaplan]

Sie müssen über Folgendes verfügen, [!DNL Anaplan] dieses Szenario verwenden zu können:

* Ein Benutzerprofil in [!DNL Anaplan] mit dem Namen **[!UICONTROL [!DNL Workfront]Integration]**, das über Systemadministratorrechte verfügt.
* Das [!DNL Anaplan], das Sie für dieses Szenario verwenden möchten.
* Die Liste innerhalb des [!DNL Anaplan], das Kampagnenbudgets erfasst.

  Das -Modul der Liste muss den Empfang der folgenden Attribute unterstützen:

   * [!UICONTROL [!DNL Workfront] Anfrage-GUID]
   * [!UICONTROL [!DNL Workfront] Projekt-GUID]
   * [!UICONTROL Kampagnenname]
   * [!UICONTROL Beantragte Arbeitsmittel]
   * [!UICONTROL Angeforderte Ausgabenmittel]
   * [!UICONTROL Budgetanfragetyp]

  Diese Liste und dieses Modul müssen zusätzliche Details speichern, die für die normale Funktionalität von [!DNL Anaplan] erforderlich sind, einschließlich der Möglichkeit, ein Budget festzulegen und mitzuteilen, dass das Budgetlistenelement bereit ist, wieder mit [!DNL Workfront] synchronisiert zu werden.

Anweisungen zu diesen Aktionen finden Sie in der [!DNL Anaplan]-Dokumentation.

## Bereitstellen für [!DNL Workfront Fusion]

Führen Sie die folgenden Schritte aus, um dieses Integrationsszenario in Ihrem [!DNL Fusion]-Konto bereitzustellen. Dies sollte erst nach Abschluss der erforderlichen [!DNL Workfront]- und [!DNL Anaplan]-Konfiguration erfolgen.

1. Navigieren Sie zum Menü [!UICONTROL Vorlagen] in [!DNL Workfront Fusion] und klicken Sie auf die **[!UICONTROL Erstellen eines [!DNL Anaplan] Listenelements aus einer Workfront-Kampagnenanfrage]**-Szenariovorlage.
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

* [[!UICONTROL Budgetzuweisung  [!DNL Anaplan]  eine Kampagnenanfrage  [!DNL Adobe Workfront]  ein Kampagnenprojekt anwenden]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-campaign-requests-and-projects.md)

Weitere Szenarien für die Ausgabenoptimierung sind:

* [[!UICONTROL Projektaktualisierungen  [!DNL Adobe Workfront]  ein  [!DNL Anaplan]  senden]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-updates-to-anaplan-list-item.md)

* [[!UICONTROL Senden von  [!DNL Adobe Workfront] -Stunden-Aktualisierungen an ein  [!DNL Anaplan] -Element]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-actual-hours-updates-to-anaplan-list-item.md)

* [[!UICONTROL Senden [!DNL Adobe Workfront] Ausgaben an  [!DNL Anaplan] /Listenelement]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-expenses-to-anaplan-list-item.md)
