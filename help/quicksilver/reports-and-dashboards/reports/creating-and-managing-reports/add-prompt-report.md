---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Hinzufügen einer Eingabeaufforderung zu einem Bericht
description: Filter und Eingabeaufforderungen ähneln sich insofern, als sie beide die Menge der Informationen einschränken, die Sie in einem Bericht anzeigen.
author: Nolan
feature: Reports and Dashboards
exl-id: b4058fb3-7360-474f-8be1-1c6b584749b0
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '1252'
ht-degree: 0%

---

# Hinzufügen einer Eingabeaufforderung zu einem Bericht

## Der Unterschied zwischen Eingabeaufforderungen und Filtern

Filter und Eingabeaufforderungen ähneln sich insofern, als sie beide die Menge der Informationen einschränken, die Sie in einem Bericht anzeigen.

Sie erstellen einen Filter, wenn die im Bericht angezeigten Informationen bei jeder Ausführung des Berichts nach denselben Kriterien gefiltert werden sollen. Filter werden einmal erstellt und im Bericht hartcodiert. Weitere Informationen zum Erstellen von Filtern finden Sie im Artikel [Filterübersicht in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

Eingabeaufforderungen sind offene Filter, die bei jeder Ausführung eines Berichts unterschiedlich angepasst und angewendet werden können.

Wenn Sie Eingabeaufforderungen zum Bericht hinzufügen, können Sie die Filterinformationen anpassen, indem Sie die Eingabeaufforderungskriterien jedes Mal bearbeiten, wenn Sie den Bericht ausführen. Der Bericht wird jedes Mal mit einem anderen Filter ausgeführt, je nachdem, welche Modifikatoren Sie auswählen, anstatt die Modifikatoren einmal im Filter des Berichts fest zu kodieren.

Eingabeaufforderungen dienen als anpassbarer Filter für Berichte, die direkt vor Ausführung des Berichts aktualisiert werden können. Sie können generische Berichte erstellen und dann die Ergebnisse anhand der Informationen einschränken, die Sie für diesen Tag sehen möchten, oder anhand der Informationen, die für eine Reihe von für Sie individuellen Kriterien relevant sind. Wenn Sie beispielsweise über einen Stundenbericht verfügen und die Berichtinformationen anhand der folgenden Kriterien ändern möchten:

* Die Daten, zu denen die Stunden protokolliert wurden
* Die Benutzer, die in die Stunden eingestiegen sind
* Die eingegebene Stundenzahl

Sie würden drei Eingabeaufforderungen erstellen, bei denen die Bedingungen die erforderlichen Kriterien sind und der Bericht bei jeder Ausführung unterschiedlich aussehen würde, je nachdem, welche Informationen Sie für Ihre Eingabeaufforderungen auswählen.

Ein Filter kann Adobe Workfront anweisen, nur die Stunden anzuzeigen, die zwischen Juni und August dieses Jahres eingegeben wurden. Mit einer Eingabeaufforderung können Sie jedoch jedes Mal, wenn Sie den Bericht ausführen, einen anderen Zeitrahmen verwenden (z. B. zwischen Januar und Februar oder Oktober und Dezember).

## Zugriffsanforderungen

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
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf Berichte, Dashboards und Kalender bearbeiten</p> <p>Zugriff auf Filter, Ansichten, Gruppierungen bearbeiten</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Berechtigungen für einen Bericht verwalten</p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Voraussetzungen

Sie müssen einen Bericht erstellen, bevor Sie eine Eingabeaufforderung hinzufügen können.

Anweisungen zum Erstellen eines Berichts finden Sie unter [Bericht erstellen](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md)

## Erstellen einer Eingabeaufforderung

1. Wechseln Sie zum Bericht, dem Sie eine Eingabeaufforderung hinzufügen möchten.
1. Erweitern **Berichtaktionen** und klicken Sie anschließend auf **Bearbeiten**.

1. Klicken **Berichtseinstellungen**.
1. Im **Berichtsaufforderungen** Bereich, klicken Sie **Eine Eingabeaufforderung hinzufügen**.\
   ![](assets/qs-add-a-prompt-350x216.png)

1. (Bedingt) Wählen Sie das Feld aus, auf dem die Eingabeaufforderung basieren soll. Geben Sie den Namen des Felds ein und wählen Sie ihn aus, wenn er in der Liste angezeigt wird.\
   Die für Benutzer, die den Bericht ausführen, verfügbaren Optionen variieren je nach ausgewähltem Feld.\
   Wenn Sie beispielsweise ein Datumsfeld wie &quot;Tatsächliches Abschlussdatum&quot;in einem Aufgabenbericht auswählen, ist &quot;Tatsächliches Abschlussdatum&quot;der Name der Eingabeaufforderung. Wenn Sie diese Eingabeaufforderung während der Ausführung dieses Berichts bearbeiten, können Sie aus einer Reihe von Modifikatoren auswählen, um Ihre Filteranweisung zu erstellen. Dieser Vorgang entspricht dem Erstellen eines Filters. Weitere Informationen zu Modifikatoren finden Sie unter [Filter- und Bedingungs-Modifikatoren](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

1. (Bedingt) Klicken Sie auf **Benutzerdefinierte Eingabeaufforderung** , um eine benutzerdefinierte Eingabeaufforderung zu erstellen.

   Eine benutzerdefinierte Eingabeaufforderung ist eine vordefinierte Eingabeaufforderung, an der Sie die Filterkriterien vor der Ausführung des Berichts hartcodieren. In diesem Sinne ist eine benutzerdefinierte Eingabeaufforderung näher an einem Filter als an einer Eingabeaufforderung.

   Die Eingabeaufforderung bleibt jedoch genauso flexibel wie eine reguläre Eingabeaufforderung, da Sie aus mehreren vordefinierten Anweisungen wählen können, anstatt nur einen hartcodierten Filter im Bericht zu haben.

   Geben Sie die folgenden Informationen für die benutzerdefinierte Eingabeaufforderung an: Die Bedingung einer benutzerdefinierten Eingabeaufforderung kann nur im Textmodus bearbeitet werden. Dadurch können mehrere Bedingungen in einem Feld angewendet werden.

   * **Feldname:** Dies ist der Name der Eingabeaufforderung, wie er vor Ausführung des Berichts angezeigt wird.
   * **Titel:** Dies ist der Name einer der Optionen in der Eingabeaufforderung, wie Sie sie sehen, bevor Sie den Bericht ausführen.
   * **Bedingung:** Geben Sie eine Bedingung ein, die die Eingabeaufforderung definiert.

   Verwenden Sie dieselbe Syntax, die Sie beim Aufrufen eines Textmodusfilters verwenden würden, und fügen Sie Ihre Anweisungen mit &quot;&amp;&quot;ein. Weitere Informationen zum Bearbeiten eines Filters im Textmodus finden Sie unter [Filter im Textmodus bearbeiten](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md).

   Beispiel: die **Bedingung** -Feld der benutzerdefinierten Eingabeaufforderung für die folgenden Szenarien könnte wie folgt aussehen:

   * alle Aufgaben für zukünftige Projekte, bei denen der Projektstatus Ideen, angefordert, Geplant und Aktuell lautet:

      ```
      project:plannedStartDate=$$TODAY&project:plannedStartDate_Mod=gte&project:status=IDA,REQ,PLN,CUR&project:status_Mod=in
      ```

   * alle Aufgaben in abgeschlossenen (vergangenen) Projekten, bei denen der Projektstatus abgeschlossen oder abgelaufen ist:

      ```
      project:actualCompletionDate=$$TODAY&project:actualCompletionDate_Mod=lte&project:status=CPL,DED&project:status_Mod=in
      ```
   Weitere Informationen zu Textmodus-Modifikatoren finden Sie unter [Filter- und Bedingungs-Modifikatoren](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

   >[!NOTE]
   >
   >Sie können die Bedingungen einer benutzerdefinierten Eingabeaufforderung beim Ausführen des Berichts nicht wie eine Standardaufforderung ändern. Sie können für eine benutzerdefinierte Eingabeaufforderung so viele vordefinierte Bedingungen wie nötig haben.

1. (Optional) Wiederholen Sie Schritt 4 oder Schritt 5, um so viele Eingabeaufforderungen wie nötig zu erstellen.
1. Klicken **Fertig** Klicken Sie auf **Speichern+Schließen** , um den Bericht zu speichern.

## Anwenden einer Eingabeaufforderung auf einen Bericht

Wenn Sie eine Eingabeaufforderung zu einem Bericht hinzugefügt haben, ist die Standardregisterkarte des Berichts immer der Tab Eingabeaufforderungen .

So führen Sie einen Bericht mit einer Eingabeaufforderung aus:

1. Wechseln Sie mit der Eingabeaufforderung zum Bericht.

   ![](assets/qs-prompt-drop-downs-350x229.png)

1. Wählen Sie eine Bedingung für einen oder alle auf der Seite **Eingabeaufforderungen** Registerkarte.\
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
>Wenn Sie einen erforderlichen Bericht außerhalb von Workfront freigeben, muss der Benutzer, der den Bericht anzeigt, bei Workfront angemeldet sein, damit der Bericht über die Eingabeaufforderung ausgeführt werden kann. Wenn der Benutzer, der den Bericht anzeigt, nicht angemeldet ist, werden alle Ergebnisse des Berichts angezeigt, ohne die Eingabeaufforderung anzuwenden.

Die Freigabe erforderlicher Berichte aus Workfront unterliegt folgenden Einschränkungen:

* Wenn Sie einen Bericht öffentlich freigeben, können Benutzer den Bericht nicht über die Aufforderung ausführen, es sei denn, sie verfügen über Workfront-Anmeldeinformationen und melden sich zuerst an, um den Bericht in Workfront anzuzeigen.

   Weitere Informationen zum Freigeben von Berichten finden Sie im Artikel [Bericht in Adobe Workfront freigeben](../../../reports-and-dashboards/reports/creating-and-managing-reports/share-report.md).
* Wenn Sie einen Bericht planen, der zum Versand aufgefordert wird, enthält der Bericht im E-Mail-Anhang die Daten des Berichts, die Sie umbenannt haben. Wenn der Benutzer auf den Link in der E-Mail klickt, um auf den Bericht zuzugreifen, muss er sich zuerst anmelden, um den Bericht anzuzeigen und die Eingabeaufforderung selbst auszuführen.

   Informationen zur Planung eines gelieferten Berichts finden Sie unter [Planen eines automatischen Berichtversands](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-automatic-report-delivery.md).
