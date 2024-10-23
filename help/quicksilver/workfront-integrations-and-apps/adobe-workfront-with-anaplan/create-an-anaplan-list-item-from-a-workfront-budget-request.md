---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-with-anaplan
title: Erstellen eines  [!DNL Anaplan] Listenelements aus einer  [!DNL Adobe Workfront] -Budgetanfrage
description: Dieses Integrationsszenario verknüpft ein [!DNL Adobe Workfront] Projekt (Kampagne) mit einem [!DNL Anaplan] Budgetlistenelement. Dies wird erreicht, indem eine Budgetanforderung zum [!DNL Workfront] Projekt hinzugefügt wird, das Finanzmittel erhalten muss. Dieses Szenario überwacht nicht verarbeitete Budgetanforderungen und führt dann einen Prozess aus, um in [!DNL Anaplan] ein leeres Budgetlistenelement zu erstellen, um die Budgetzuweisungsprozesse in Anaplan zu starten.
author: Becky
feature: Workfront Integrations and Apps, Workfront Fusion
exl-id: e6505ece-21aa-4397-8d68-543bf89d2f00
source-git-commit: 7697327455a7ffdc1a15bfa1676c3a0b091abd04
workflow-type: tm+mt
source-wordcount: '801'
ht-degree: 0%

---

# Erstellen eines [!DNL Anaplan] Listenelements aus einer [!DNL Adobe Workfront] Budgetanforderung

Dieses Integrationsszenario verknüpft ein [!DNL Adobe Workfront] -Projekt (Kampagne) mit einem [!DNL Anaplan] -Budgetlistenelement. Dies wird erreicht, indem eine Budgetanforderung zum [!DNL Workfront] -Projekt hinzugefügt wird, das Finanzmittel erhalten muss. Dieses Szenario überwacht nicht verarbeitete Budgetanforderungen und führt dann einen Prozess aus, um ein leeres Budgetlistenelement in [!DNL Anaplan] zu erstellen, um die Budgetzuweisungsprozesse in [!DNL Anaplan] zu starten.

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

&#42;&#42;Informationen zu [!DNL  Adobe Workfront Fusion] Lizenzen finden Sie unter [[!DNL Adobe Workfront Fusion] Lizenzen](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Ereignis auslösen

Dieses Szenario wird alle 15 Minuten ausgeführt.

## Erwartete [!DNL Workfront] Konfiguration

Sie müssen Folgendes in [!DNL Workfront] haben, um dieses Szenario zu verwenden:

* Ein Benutzerprofil mit dem Namen *[!UICONTROL *[!DNL Anaplan] Integration]*** mit Systemadministrator-Berechtigungen.[!DNL Workfront]

  Informationen zum Erstellen eines Benutzers in [!DNL Workfront] finden Sie unter [Benutzer hinzufügen](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

* Ein benutzerdefiniertes **[!UICONTROL Budgetanforderung]**-Formular, das an das Objekt [!UICONTROL Anfrage] angehängt ist.

  Die folgenden erforderlichen Felder müssen im benutzerdefinierten Formular enthalten sein, um die Datenzuordnung zu [!DNL Anaplan] zu unterstützen:

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

  Informationen zum Erstellen benutzerdefinierter Formulare finden Sie unter [Erstellen eines benutzerdefinierten Formulars](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

* Projektvorlagen, die Kampagnen und andere Projekte darstellen, für die eine Finanzierung erforderlich ist, konfiguriert mit einem Warteschlangenthema [!UICONTROL Budgetanforderung] . Das Warteschlangenthema [!UICONTROL Budgetanforderung] wird zugewiesen, um das benutzerdefinierte Formular [!UICONTROL Budgetanforderung] zu verwenden.
* Ein Formular **[!UICONTROL Kampagnenbeschreibung]** für das Projektobjekt.

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

  Informationen zum Erstellen benutzerdefinierter Formulare finden Sie unter [Erstellen eines benutzerdefinierten Formulars](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

## Erwartete [!DNL Anaplan] Konfiguration

Sie müssen Folgendes in [!DNL Anaplan] haben, um dieses Szenario zu verwenden:

* Ein Benutzerprofil mit dem Namen **[!UICONTROL [!DNL Workfront]Integration]** in [!DNL Anaplan] mit Systemadministrator-Berechtigungen.
* Das [!DNL Anaplan]-Modell, das Sie für dieses Szenario verwenden möchten.
* Die Liste innerhalb des [!DNL Anaplan]-Modells, das Kampagnenbudgets erfasst.

  Das Modul der Liste muss den Empfang der folgenden Attribute unterstützen:

   * [!UICONTROL Workfront Project GUID]
   * [!UICONTROL Kampagnenname]
   * [!UICONTROL Beantragte Arbeitsfonds]
   * [!UICONTROL Beantragte Ausgabenfonds]
   * [!UICONTROL Budgetanforderungstyp]
   * [!UICONTROL Grund für die Anpassung der Finanzmittel]

  Diese Liste und dieses Modul müssen zusätzliche Details speichern, die für die normale Funktionalität von [!DNL Anaplan] erforderlich sind, einschließlich der Möglichkeit, ein Budget festzulegen und mitzuteilen, dass das Budgetlistenelement bereit ist, wieder mit [!DNL Workfront] synchronisiert zu werden.

Anweisungen zu diesen Aktionen finden Sie in der Dokumentation zu [!DNL Anaplan] .

## Bereitstellen unter [!DNL Workfront Fusion]

Führen Sie die folgenden Schritte aus, um dieses Integrationsszenario in Ihrem [!DNL Fusion]-Konto bereitzustellen. Dies sollte erst nach Abschluss der erforderlichen [!DNL Workfront] - und [!DNL Anaplan] -Konfiguration erfolgen.

1. Navigieren Sie zum Menü [!UICONTROL Vorlagen] in [!DNL Workfront Fusion] und klicken Sie auf die Vorlage **[!UICONTROL Listenelement [!DNL Anaplan] aus einer Workfront-Budgetanforderung erstellen]** .
1. Ersetzen Sie die Variablenwerte für die folgenden [!DNL Anaplan] -Variablen:

   | Variablenname | Wert ersetzen durch |
   |---|---|
   | [!UICONTROL [!DNL Anaplan] Workspace ID] | Die ID eines Workspace aus Ihrem [!DNL Anaplan]-Konto. |
   | [!UICONTROL [!DNL Anaplan] Modell-ID] | Die ID eines Modells aus Ihrem [!DNL Anaplan] -Konto und dem ausgewählten Arbeitsbereich. |
   | [!UICONTROL [!DNL Anaplan] Modulname] | Der Name des Moduls, das die Kampagnenattribute in der ausgewählten [!DNL Anaplan]-Liste beschreibt. |
   | [!UICONTROL Kampagnenlisten-Name] | Der Name der Liste aus Ihrem [!DNL Anaplan] -Konto und der ausgewählte Arbeitsbereich und das ausgewählte Modell. |

   {style="table-layout:auto"}

   Weitere Informationen zum Einrichten der Dateien und Prozesse finden Sie in der Dokumentation zur Einrichtung von [!DNL Anaplan] .

1. Wählen Sie ein Verbindungsprofil vom Typ [!DNL Anaplan] aus oder fügen Sie es hinzu.
1. Aktualisieren Sie bei Aufforderung alle verbleibenden [!DNL Anaplan] -Module mit einer [!DNL Anaplan] -Verbindung.
1. Wählen Sie ein Verbindungsprofil vom Typ [!DNL Workfront] aus oder fügen Sie es hinzu.

   Nach der Bereitstellung der Vorlage ist dies das Modul, das Sie aktualisieren, um benutzerdefinierte Feldverweise zum Wert der Feldeigenschaft hinzuzufügen oder daraus zu entfernen, wenn Sie die Standardzuordnungsfelder in [!DNL Anaplan] ändern möchten.

1. Aktualisieren Sie bei Aufforderung alle verbleibenden [!DNL Workfront] -Module mit einer [!DNL Workfront] -Verbindung.

## Andere empfohlene Szenario-Vorlagen

Um den von dieser Vorlage dargestellten Workflow abzuschließen, müssen Sie außerdem die folgende zusätzliche Vorlage bereitstellen:

* [[!UICONTROL Anwenden einer [!DNL Anaplan] Budgetzuordnung auf ein [!DNL Adobe Workfront] Projekt]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-projects.md)

Weitere Szenarien für die Ausgabenoptimierung sind:

* [[!UICONTROL Senden von [!DNL Adobe Workfront] Projektaktualisierungen an ein [!DNL Anaplan] Listenelement]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-updates-to-anaplan-list-item.md)
* [[!UICONTROL Sende [!DNL Adobe Workfront] tatsächliche Stunden-Aktualisierungen an ein  [!DNL Anaplan] Listenelement]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-actual-hours-updates-to-anaplan-list-item.md)
* [[!UICONTROL Senden [!DNL Adobe Workfront] der Ausgaben an einen  [!DNL Anaplan] Listeneintrag]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-expenses-to-anaplan-list-item.md)
