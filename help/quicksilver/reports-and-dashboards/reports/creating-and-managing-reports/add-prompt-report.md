---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Hinzufügen einer Eingabeaufforderung zu einem Bericht
description: Filter und Eingabeaufforderungen sind insofern ähnlich, als sie beide die Menge an Informationen einschränken, die Sie in einem Bericht anzeigen.
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

## Unterschied zwischen Eingabeaufforderungen und Filtern

Filter und Eingabeaufforderungen sind insofern ähnlich, als sie beide die Menge an Informationen einschränken, die Sie in einem Bericht anzeigen.

Sie erstellen einen Filter, wenn die im Bericht angezeigten Informationen bei jeder Ausführung des Berichts nach denselben Kriterien gefiltert werden sollen. Filter werden einmal erstellt und im Bericht hartcodiert. Weitere Informationen zum Erstellen von Filtern finden Sie im Artikel [Filter - Übersicht](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

Eingabeaufforderungen sind offene Filter, die bei jeder Ausführung eines Berichts anders angepasst und angewendet werden können.

Wenn Sie Eingabeaufforderungen zu Ihrem Bericht hinzufügen, können Sie die Filterinformationen anpassen, indem Sie die Eingabeaufforderungskriterien bei jeder Ausführung des Berichts bearbeiten. Der Bericht wird jedes Mal mit einem anderen Filter ausgeführt, je nachdem, welche Modifikatoren Sie auswählen, anstatt die Modifikatoren einmal im Filter des Berichts hartcodiert zu haben.

Eingabeaufforderungen dienen als anpassbarer Filter für Berichte, die direkt vor der Ausführung des Berichts aktualisiert werden können. Sie können generische Berichte erstellen und die Ergebnisse dann auf der Grundlage von Informationen eingrenzen, die Sie für diesen Tag sehen möchten, oder auf der Grundlage der Informationen, die für einen Satz von für Sie individuellen Kriterien relevant sind. Wenn Sie beispielsweise über einen Stundenbericht verfügen und die Berichtsinformationen anhand der folgenden Kriterien ändern möchten:

* Die Daten, an denen die Stunden protokolliert wurden
* Die Benutzer, die die Stunden eingegeben haben
* Die eingegebene Anzahl von Stunden

Je nachdem, welche Informationen Sie für Ihre Eingabeaufforderungen auswählen, erstellen Sie drei Eingabeaufforderungen, bei denen die Bedingungen die erforderlichen Kriterien sind und der Bericht bei jeder Ausführung anders aussieht.

Ein Filter kann Adobe Workfront anweisen, nur die zwischen Juni und August dieses Jahres eingegebenen Stunden anzuzeigen. Bei einer Eingabeaufforderung können Sie jedoch jedes Mal, wenn Sie den Bericht ausführen, einen anderen Zeitrahmen verwenden (z. B. zwischen Januar und Februar oder zwischen Oktober und Dezember).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Beliebig</p> </td> 
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
   <td role="rowheader">Konfigurationen der Zugriffsebene*</td> 
   <td> <p>Zugriff auf Berichte, Dashboards, Kalender bearbeiten</p> <p>Zugriff auf Filter, Ansichten, Gruppierungen bearbeiten</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen*</td> 
   <td> <p>Verwalten von Berechtigungen für einen Bericht</p></td> 
  </tr> 
 </tbody> 
</table>

*Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Voraussetzungen

Sie müssen einen Bericht erstellen, bevor Sie ihm eine Eingabeaufforderung hinzufügen können.

Anweisungen zum Erstellen eines Berichts finden Sie unter [Erstellen eines Berichts](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md)

## Eingabeaufforderung erstellen

1. Wechseln Sie zum Bericht, dem Sie eine Eingabeaufforderung hinzufügen möchten.
1. Erweitern Sie **Berichtsaktionen** und klicken Sie dann auf **Bearbeiten**.

1. Klicken Sie auf **Schaltfläche &quot;**&quot;.
1. Klicken Sie auf **Registerkarte** Eingabeaufforderungen“ und dann auf **Eingabeaufforderung hinzufügen**.\
   ![](assets/create-report-prompt-tab.png)

1. (Bedingt) Wählen Sie das Feld aus, auf dem die Eingabeaufforderung basieren soll. Geben Sie den Namen des Felds ein und klicken Sie auf das Feld, um es auszuwählen, wenn es in der Liste angezeigt wird.\
   Die Optionen, die Benutzern zur Verfügung stehen, die den Bericht ausführen, unterscheiden sich je nach ausgewähltem Feld.\
   Wenn Sie beispielsweise ein Datumsfeld wie „Tatsächliches Abschlussdatum“ in einem Aufgabenbericht auswählen, ist „Tatsächliches Abschlussdatum“ der Name der Eingabeaufforderung. Beim Bearbeiten dieser Eingabeaufforderung während der Ausführung dieses Berichts können Sie aus einer Reihe von Modifikatoren auswählen, um Ihre Filteranweisung zu erstellen. Dieser Prozess ist identisch mit dem Erstellen eines Filters. Weitere Informationen zu Modifikatoren finden Sie unter [Filter- und Bedingungsmodifikatoren](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

1. (Bedingt) Klicken Sie auf **Benutzerdefinierte Eingabeaufforderung**, um eine benutzerdefinierte Eingabeaufforderung zu erstellen.

   Eine benutzerdefinierte Eingabeaufforderung ist eine vordefinierte Eingabeaufforderung, in der Sie die Filterkriterien fest codieren, bevor Sie den Bericht ausführen. In diesem Sinne ist eine benutzerdefinierte Eingabeaufforderung näher an einem Filter als an einer Eingabeaufforderung.

   Die Eingabeaufforderung bleibt jedoch so flexibel wie eine reguläre Eingabeaufforderung, da Sie aus mehreren vordefinierten Anweisungen auswählen können, anstatt nur einen hartcodierten Filter im Bericht zu haben.

   Geben Sie die folgenden Informationen für die benutzerdefinierte Eingabeaufforderung an: Die Bedingung einer benutzerdefinierten Eingabeaufforderung kann nur im Textmodus bearbeitet werden. Auf diese Weise können mehrere Bedingungen in einem einzigen Feld angewendet werden.

   * **Feldname:** Dies ist der Name der Eingabeaufforderung, wie er vor der Ausführung des Berichts angezeigt wird.
   * **Dropdown-Elementbeschriftung** Dies ist der Name einer der Optionen innerhalb der Eingabeaufforderung, wie sie vor der Ausführung des Berichts angezeigt wird.
   * **Bedingung:** Geben Sie eine Bedingung ein, die die Eingabeaufforderung definiert.
   * **Standard** Sie können ein Element als Standardoption für diese Eingabeaufforderung auswählen.

   Verwenden Sie dieselbe Syntax, die Sie beim Eingeben eines Textmodusfilters verwenden würden, und verbinden Sie Ihre Anweisungen mit &quot;&amp;&quot;. Weitere Informationen zum Bearbeiten eines Filters im Textmodus finden Sie unter [Bearbeiten eines Filters im Textmodus](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md).

   Beispielsweise könnte das Feld **Bedingung** der benutzerdefinierten Eingabeaufforderung für die folgenden Szenarien wie folgt aussehen:

   * alle Aufgaben für zukünftige Projekte, bei denen der Projektstatus „Idee“, „Angefordert“, „Geplant“ und „Aktuell“ ist:

     ```
     project:plannedStartDate=$$TODAY&project:plannedStartDate_Mod=gte&project:status=IDA,REQ,PLN,CUR&project:status_Mod=in
     ```

   * alle Aufgaben in abgeschlossenen (vergangenen) Projekten, bei denen der Projektstatus „Abgeschlossen“ oder „Inaktiv“ lautet:

     ```
     project:actualCompletionDate=$$TODAY&project:actualCompletionDate_Mod=lte&project:status=CPL,DED&project:status_Mod=in
     ```

   Weitere Informationen zu Textmodusmodifikatoren finden Sie unter [Filter- und Bedingungsmodifikatoren](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

   >[!NOTE]
   >
   >Sie können die Bedingungen einer benutzerdefinierten Eingabeaufforderung beim Ausführen des Berichts nicht ändern, wie dies bei einer Standardaufforderung der Fall wäre. Für eine benutzerdefinierte Eingabeaufforderung können beliebig viele vordefinierte Bedingungen angegeben werden.

1. (Optional) Wiederholen Sie Schritt 4 oder Schritt 5, um so viele Eingabeaufforderungen wie nötig zu erstellen.
1. Klicken Sie **Fertig** und anschließend auf **Speichern+Schließen**, um den Bericht zu speichern.

## Anwenden einer Eingabeaufforderung auf einen Bericht

Wenn Sie eine Eingabeaufforderung zu einem Bericht hinzugefügt haben, ist die Standardregisterkarte des Berichts immer die Registerkarte Eingabeaufforderungen .

So führen Sie einen Bericht mit einer Eingabeaufforderung aus:

1. Rufen Sie den Bericht über die Eingabeaufforderung auf.

   ![](assets/run-report-prompts.png)

1. Bedingung für eine oder alle Eingabeaufforderungen auf der Registerkarte **Eingabeaufforderungen“**.\
   (Optional) Sie können die Eingabeaufforderungen leer lassen und den Bericht nicht nach den Eingabeaufforderungsbedingungen filtern.

1. Klicken Sie auf **Bericht ausführen**.\
   (Bedingt) Wenn Sie die Eingabeaufforderungen ausgefüllt haben, wird der Bericht nach den Bedingungen gefiltert, die Sie für Ihre Eingabeaufforderungen ausgewählt haben.\
   (Bedingt) Wenn Sie die Eingabeaufforderungen leer gelassen haben, wird der Bericht nicht nach den Eingabeaufforderungsbedingungen gefiltert. Der Bericht wird angezeigt, als ob er nicht gefiltert wäre.

   >[!NOTE]
   >
   >Ein Bericht, der zusätzlich zu einer Eingabeaufforderung einen Filter enthält, filtert die Ergebnisse sowohl nach den im Filter definierten Kriterien als auch nach der kombinierten Eingabeaufforderung.

## Einschränkungen bei der Freigabe von ausgelösten Berichten

>[!CAUTION]
>
>Wenn Sie einen Bericht freigeben, können sowohl angemeldete als auch nicht angemeldete Benutzende, die den Bericht über den öffentlichen Freigabe-Link anzeigen, den Bericht nicht über die Eingabeaufforderungen ausführen. In diesem Fall werden die Ergebnisse des Berichts ohne Eingabeaufforderungen angezeigt. Die angezeigten Informationen basieren stattdessen auf der Zugriffsebene und den Berechtigungen des Benutzers oder, falls eine solche festgelegt ist, auf der Zugriffsebene Als Benutzer ausführen und den Berechtigungen des Berichts.

Im Folgenden finden Sie Einschränkungen bei der Freigabe von Berichten, die von Workfront aufgefordert werden:

* Wenn Sie einen Bericht öffentlich freigeben, können Benutzende den Bericht nicht mit angewendeten Eingabeaufforderungen ausführen, es sei denn, sie verfügen über Workfront-Anmeldeinformationen, melden sich zuerst an und navigieren direkt in Workfront zum Bericht (nicht über den öffentlichen Freigabe-Link).

  Weitere Informationen zum Freigeben von Berichten finden Sie im Artikel [Freigeben eines Berichts in Adobe Workfront](../../../reports-and-dashboards/reports/creating-and-managing-reports/share-report.md).

* Wenn Sie einen Bericht planen, der zur Bereitstellung aufgefordert wird, enthält der Bericht im E-Mail-Anhang die Daten des unaufgeforderten Berichts. Wenn der/die Benutzende auf den Link in der E-Mail klickt, um auf den Bericht zuzugreifen, muss er/sie sich zuerst anmelden, um den Bericht anzuzeigen, und die Eingabeaufforderung selbst ausführen.

  Informationen zur Planung eines zugestellten Berichts finden Sie unter [Planen eines automatischen Berichtsversands](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-automatic-report-delivery.md).

* Wenn Sie einen Bericht mit einer datumsbasierten Eingabeaufforderung ausführen, werden die Berichtsergebnisse anhand der Zeitzoneneinstellungen Ihres Browsers gefiltert. Dies kann bei Datumsbereichen, die in einem Bericht zu Datumsangaben am Anfang oder Ende eines Monats angezeigt werden, zu geringfügigen Abweichungen führen. Wenn die Zeitzoneneinstellungen Ihres Browsers an einen bestimmten Ort gebunden sind, werden Variationen der Ortszeit dieses Ortes (z. B. die Einhaltung der Sommerzeit) auch in die für einen Bericht angezeigten Datumsangaben einbezogen. Dies kann zu geringfügigen Diskrepanzen im Datumsbereich zwischen Benutzenden in derselben Zeitzone, aber mit unterschiedlichen Standorteinstellungen führen.
