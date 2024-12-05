---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Hinzufügen einer Eingabeaufforderung zu einem Bericht
description: Filter und Eingabeaufforderungen ähneln sich insofern, als sie beide die Menge der Informationen einschränken, die Sie in einem Bericht anzeigen.
author: Nolan
feature: Reports and Dashboards
exl-id: b4058fb3-7360-474f-8be1-1c6b584749b0
source-git-commit: 93fca2a98a8b9d4370841b10be10ed2ba15283c9
workflow-type: tm+mt
source-wordcount: '1363'
ht-degree: 0%

---

# Hinzufügen einer Eingabeaufforderung zu einem Bericht

<!-- Audited: 11/2024 -->

## Der Unterschied zwischen Eingabeaufforderungen und Filtern

Filter und Eingabeaufforderungen ähneln sich insofern, als sie beide die Menge der Informationen einschränken, die Sie in einem Bericht anzeigen.

Sie erstellen einen Filter, wenn die im Bericht angezeigten Informationen bei jeder Ausführung des Berichts nach denselben Kriterien gefiltert werden sollen. Filter werden einmal erstellt und im Bericht hartcodiert. Weitere Informationen zum Erstellen von Filtern finden Sie im Artikel [Filterübersicht](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

Eingabeaufforderungen sind offene Filter, die bei jeder Ausführung eines Berichts unterschiedlich angepasst und angewendet werden können.

Wenn Sie Eingabeaufforderungen zum Bericht hinzufügen, können Sie die Filterinformationen anpassen, indem Sie die Eingabeaufforderungskriterien jedes Mal bearbeiten, wenn Sie den Bericht ausführen. Der Bericht wird jedes Mal mit einem anderen Filter ausgeführt, je nachdem, welche Modifikatoren Sie auswählen, anstatt die Modifikatoren einmal im Filter des Berichts fest zu kodieren.

Eingabeaufforderungen dienen als anpassbarer Filter für Berichte, die direkt vor Ausführung des Berichts aktualisiert werden können. Sie können generische Berichte erstellen und dann die Ergebnisse anhand der Informationen einschränken, die Sie für diesen Tag sehen möchten, oder anhand der Informationen, die für eine Reihe von für Sie individuellen Kriterien relevant sind. Wenn Sie beispielsweise über einen Stundenbericht verfügen und die Berichtinformationen anhand der folgenden Kriterien ändern möchten:

* Die Daten, zu denen die Stunden protokolliert wurden
* Die Benutzer, die in die Stunden eingestiegen sind
* Die eingegebene Stundenzahl

Sie würden drei Eingabeaufforderungen erstellen, bei denen die Bedingungen die erforderlichen Kriterien sind und der Bericht bei jeder Ausführung unterschiedlich aussehen würde, je nachdem, welche Informationen Sie für Ihre Eingabeaufforderungen auswählen.

Ein Filter kann Adobe Workfront anweisen, nur die Stunden anzuzeigen, die zwischen Juni und August dieses Jahres eingegeben wurden. Mit einer Eingabeaufforderung können Sie jedoch jedes Mal, wenn Sie den Bericht ausführen, einen anderen Zeitrahmen verwenden (z. B. zwischen Januar und Februar oder Oktober und Dezember).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
    <td> 
      <p>Neu:</p>
         <ul>
         <li><p>Standard</p></li>
         </ul>
      <p>Aktuell:</p>
         <ul>
         <li><p>Plan</p></li>
         </ul>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf Berichte, Dashboards und Kalender bearbeiten</p> <p>Zugriff auf Filter, Ansichten, Gruppierungen bearbeiten</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen*</td> 
   <td> <p>Berechtigungen für einen Bericht verwalten</p></td> 
  </tr> 
 </tbody> 
</table>

*Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Voraussetzungen

Sie müssen einen Bericht erstellen, bevor Sie eine Aufforderung hinzufügen können.

Anweisungen zum Erstellen eines Berichts finden Sie unter [Erstellen eines Berichts](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md)

## Erstellen einer Eingabeaufforderung

1. Wechseln Sie zum Bericht, dem Sie eine Eingabeaufforderung hinzufügen möchten.
1. Erweitern Sie **Berichtaktionen** und klicken Sie dann auf **Bearbeiten**.

1. Klicken Sie auf die Schaltfläche **Berichtseinstellungen** .
1. Klicken Sie auf die Registerkarte **Berichtaufforderungen** und dann auf **Eingabeaufforderung hinzufügen**.\
   ![](assets/create-report-prompt-tab.png)

1. (Bedingt) Wählen Sie das Feld aus, auf dem die Eingabeaufforderung basieren soll. Geben Sie den Namen des Felds ein und wählen Sie ihn aus, wenn er in der Liste angezeigt wird.\
   Die für Benutzer, die den Bericht ausführen, verfügbaren Optionen variieren je nach ausgewähltem Feld.\
   Wenn Sie beispielsweise ein Datumsfeld wie &quot;Tatsächliches Abschlussdatum&quot;in einem Aufgabenbericht auswählen, ist &quot;Tatsächliches Abschlussdatum&quot;der Name der Eingabeaufforderung. Wenn Sie diese Eingabeaufforderung während der Ausführung dieses Berichts bearbeiten, können Sie aus einer Reihe von Modifikatoren auswählen, um Ihre Filteranweisung zu erstellen. Dieser Vorgang entspricht dem Erstellen eines Filters. Weitere Informationen zu Modifikatoren finden Sie unter [Filter und Bedingungsmodifikatoren](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

1. (Bedingt) Klicken Sie auf **Benutzerdefinierte Eingabeaufforderung** , um eine benutzerdefinierte Eingabeaufforderung zu erstellen.

   Eine benutzerdefinierte Eingabeaufforderung ist eine vordefinierte Eingabeaufforderung, an der Sie die Filterkriterien vor der Ausführung des Berichts hartcodieren. In diesem Sinne ist eine benutzerdefinierte Eingabeaufforderung näher an einem Filter als an einer Eingabeaufforderung.

   Die Eingabeaufforderung bleibt jedoch genauso flexibel wie eine reguläre Eingabeaufforderung, da Sie aus mehreren vordefinierten Anweisungen wählen können, anstatt nur einen hartcodierten Filter im Bericht zu haben.

   Geben Sie die folgenden Informationen für die benutzerdefinierte Eingabeaufforderung an: Die Bedingung einer benutzerdefinierten Eingabeaufforderung kann nur im Textmodus bearbeitet werden. Dadurch können mehrere Bedingungen in einem Feld angewendet werden.

   * **Feldname:** Dies ist der Name der Eingabeaufforderung, wie er angezeigt wird, bevor Sie den Bericht ausführen.
   * **Bezeichnung des Dropdown-Elements-Elements:** Dies ist der Name einer der Optionen in der Eingabeaufforderung, wie Sie sie sehen, bevor Sie den Bericht ausführen.
   * **Bedingung:** Geben Sie eine Bedingung ein, die die Eingabeaufforderung definiert.
   * **Standard:** Sie können ein Element als Standardoption für diese Eingabeaufforderung auswählen.

   Verwenden Sie dieselbe Syntax, die Sie beim Aufrufen eines Textmodusfilters verwenden würden, und fügen Sie Ihre Anweisungen mit &quot;&amp;&quot;ein. Weitere Informationen zum Bearbeiten eines Filters im Textmodus finden Sie unter [Bearbeiten eines Filters mit dem Textmodus](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md).

   Beispielsweise könnte das Feld **Bedingung** der benutzerdefinierten Eingabeaufforderung für die folgenden Szenarien wie folgt aussehen:

   * alle Aufgaben für zukünftige Projekte, bei denen der Projektstatus Ideen, angefordert, Geplant und Aktuell lautet:

     ```
     project:plannedStartDate=$$TODAY&project:plannedStartDate_Mod=gte&project:status=IDA,REQ,PLN,CUR&project:status_Mod=in
     ```

   * alle Aufgaben in abgeschlossenen (vergangenen) Projekten, bei denen der Projektstatus abgeschlossen oder abgelaufen ist:

     ```
     project:actualCompletionDate=$$TODAY&project:actualCompletionDate_Mod=lte&project:status=CPL,DED&project:status_Mod=in
     ```

   Weitere Informationen zu Textmodus-Modifikatoren finden Sie unter [Filter und Bedingungsmodifikatoren](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

   >[!NOTE]
   >
   >Sie können die Bedingungen einer benutzerdefinierten Eingabeaufforderung beim Ausführen des Berichts nicht wie eine Standardaufforderung ändern. Sie können für eine benutzerdefinierte Eingabeaufforderung so viele vordefinierte Bedingungen wie nötig haben.

1. (Optional) Wiederholen Sie Schritt 4 oder Schritt 5, um so viele Eingabeaufforderungen wie nötig zu erstellen.
1. Klicken Sie auf **Fertig** und dann auf **Speichern+Schließen** , um den Bericht zu speichern.

## Anwenden einer Meldung auf einen Bericht

Wenn Sie eine Eingabeaufforderung zu einem Bericht hinzugefügt haben, ist die Standardregisterkarte des Berichts immer der Tab Eingabeaufforderungen .

So führen Sie einen Bericht mit einer Eingabeaufforderung aus:

1. Wechseln Sie mit der Eingabeaufforderung zum Bericht.

   ![](assets/run-report-prompts.png)

1. Wählen Sie eine Bedingung für einen oder alle auf der Registerkarte **Eingabeaufforderungen** angezeigten Aufforderungen aus.\
   (Optional) Sie können die Eingabeaufforderungen leer lassen und den Bericht nicht nach den Eingabeaufforderungsbedingungen filtern.

1. Klicken Sie auf **Bericht ausführen**.\
   (Bedingt) Wenn Sie die Eingabeaufforderungen ausgefüllt haben, wird der Bericht nach den Bedingungen gefiltert, die Sie für Ihre Eingabeaufforderungen ausgewählt haben.\
   (Bedingt) Wenn Sie die Eingabeaufforderungen leer lassen, wird der Bericht nicht nach den Eingabeaufforderungsbedingungen gefiltert. Der Bericht wird so angezeigt, als wäre er nicht gefiltert.

   >[!NOTE]
   >
   >Ein Bericht, der zusätzlich zu einer Eingabeaufforderung einen Filter enthält, filtert die Ergebnisse sowohl nach den im Filter definierten Kriterien als auch nach der Kombination der Eingabeaufforderung.

## Einschränkungen bei der Freigabe erforderlicher Berichte

>[!CAUTION]
>
>Wenn Sie einen angezeigten Bericht freigeben, können sowohl angemeldete als auch nicht angemeldete Benutzer, die den Bericht über den öffentlichen Freigabe-Link anzeigen, den Bericht nicht mit den entsprechenden Eingabeaufforderungen ausführen. In diesem Fall werden die Ergebnisse des Berichts angezeigt, ohne dass eine Aufforderung eingeht. Stattdessen basieren die angezeigten Informationen auf der Zugriffsebene und den Berechtigungen des Benutzers oder auf der Zugriffsebene und den Berechtigungen des Berichts &quot;Als Benutzer ausführen&quot;, sofern eine festgelegt ist.

Die Freigabe erforderlicher Berichte aus Workfront unterliegt folgenden Einschränkungen:

* Wenn Sie einen Bericht öffentlich freigeben, können die Benutzer den Bericht nicht mit angewendeten Eingabeaufforderungen ausführen, es sei denn, sie verfügen über Workfront-Anmeldeinformationen, melden sich zuerst an und navigieren direkt in Workfront zum Bericht (nicht über den öffentlichen Freigabe-Link).

  Weitere Informationen zum Freigeben von Berichten finden Sie im Artikel [Berichtfreigabe in Adobe Workfront](../../../reports-and-dashboards/reports/creating-and-managing-reports/share-report.md).

* Wenn Sie einen Bericht planen, der zur Bereitstellung aufgefordert wird, enthält der Bericht im E-Mail-Anhang die Daten des Berichts, die nicht angefordert werden. Wenn der Benutzer auf den Link in der E-Mail klickt, um auf den Bericht zuzugreifen, muss er sich zuerst anmelden, um den Bericht anzuzeigen und die Eingabeaufforderung selbst auszuführen.

  Informationen zum Planen eines gelieferten Berichts finden Sie unter [Planen einer automatischen Berichtbereitstellung](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-automatic-report-delivery.md).

* Wenn Sie einen Bericht mit einer datumsbasierten Eingabeaufforderung ausführen, werden die Berichtsergebnisse anhand der Zeitzoneneinstellungen Ihres Browsers gefiltert. Dies kann zu leichten Abweichungen zwischen den Datumsbereichen führen, die in einem aufgerufenen Bericht für Datumsangaben am Anfang oder Ende eines Monats angezeigt werden. Wenn die Zeitzoneneinstellungen Ihres Browsers an einen bestimmten Ort gebunden sind, werden auch Variationen der lokalen Zeit dieses Standorts (z. B. Einhaltung der Sommerzeit) in den Datumsangaben berücksichtigt, die für einen aufgerufenen Bericht angezeigt werden. Dies kann zu leichten Abweichungen zwischen den Datumsbereichen zwischen Benutzern in derselben Zeitzone, aber mit unterschiedlichen Standorteinstellungen führen.
