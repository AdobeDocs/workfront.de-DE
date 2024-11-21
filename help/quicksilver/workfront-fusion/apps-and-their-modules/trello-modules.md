---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: Connector
navigation-topic: apps-and-their-modules
title: Trello-Module
description: In einem [!DNL Adobe Workfront Fusion] Szenario können Sie Workflows automatisieren, die Trello verwenden, und sie mit mehreren Anwendungen und Diensten von Drittanbietern verbinden.
author: Becky
feature: Workfront Fusion
exl-id: 60630b23-e057-4ecf-a014-6e63b6d69b48
source-git-commit: 55485da1ea650121b5537a3f19d8102623ed4f43
workflow-type: tm+mt
source-wordcount: '5113'
ht-degree: 0%

---

# [!UICONTROL Trello] -Module

In einem [!DNL Adobe Workfront Fusion] -Szenario können Sie Workflows automatisieren, die [!UICONTROL Trello] verwenden, und sie mit mehreren Anwendungen und Diensten von Drittanbietern verbinden.

Wenn Sie Anweisungen zum Erstellen eines Szenarios benötigen, finden Sie weitere Informationen unter [Erstellen eines Szenarios in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

Weitere Informationen zu Modulen finden Sie unter [Module in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

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
   <td>
   <p>Aktuelle Lizenzanforderungen: Keine [!DNL Workfront Fusion] Lizenzanforderungen.</p>
   <p>Oder</p>
   <p>Alte Lizenzanforderung: [!UICONTROL [!DNL Workfront Fusion] für die Arbeitsautomatisierung und -integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>
   <p>Aktuelle Produktanforderung: Wenn Sie über den [!UICONTROL Select]- oder [!UICONTROL Prime] [!DNL Adobe Workfront]-Plan verfügen, muss Ihr Unternehmen [!DNL Adobe Workfront Fusion] sowie [!DNL Adobe Workfront] erwerben, um die in diesem Artikel beschriebene Funktionalität nutzen zu können. [!DNL Workfront Fusion] ist im [!UICONTROL Ultimate] [!DNL Workfront]-Plan enthalten.</p>
   <p>Oder</p>
   <p>Alte Produktanforderung: Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] sowie [!DNL Adobe Workfront] erwerben, um die in diesem Artikel beschriebenen Funktionen nutzen zu können.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Wenden Sie sich an Ihren [!DNL Workfront] -Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

Informationen zu [!DNL Adobe Workfront Fusion] -Lizenzen finden Sie unter [[!DNL Adobe Workfront Fusion] Lizenzen](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Voraussetzungen

Um [!DNL Trello] -Module zu verwenden, müssen Sie über ein [!UICONTROL Trello] -Konto verfügen.

## Trello-API-Informationen

Der Trello-Connector verwendet Folgendes:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Basis-URL</td> 
   <td> https://api.trello.com/1</td>
  </tr> 
  <tr> 
   <td role="rowheader">API-Version</td> 
   <td> v1 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">API-Tag</td> 
   <td>v4.12.37</td> 
  </tr>
 </tbody> 
 </table>

## [!UICONTROL Trello] mit [!DNL Workfront Fusion] verbinden

Anweisungen zum Verbinden Ihres [!UICONTROL Trello]-Kontos mit [!DNL Workfront Fusion] finden Sie unter [Erstellen einer Verbindung zu  [!DNL Adobe Workfront Fusion]  - Grundlegende Anweisungen](../../workfront-fusion/connections/connect-to-fusion-general.md)

## [!UICONTROL Trello] -Module und ihre Felder

Wenn Sie die Module [!UICONTROL Trello] konfigurieren, zeigt [!DNL Workfront Fusion] die unten aufgeführten Felder an. Darüber hinaus können abhängig von Faktoren wie Ihrer Zugriffsebene in der App oder im Dienst zusätzliche [!UICONTROL Trello] -Felder angezeigt werden. Ein fett hervorgehobener Titel in einem Modul zeigt ein erforderliches Feld an.

Wenn Sie die Zuordnungsschaltfläche über einem Feld oder einer Funktion sehen, können Sie damit Variablen und Funktionen für dieses Feld festlegen. Weitere Informationen finden Sie unter [Informationen von einem Modul einem anderen zuordnen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Pinnwände](#boards)
* [Listen](#lists)
* [Karten](#cards)
* [Abonnenten](#members)
* [Checklisten](#checklists)
* [Kennzeichnungen](#labels)
* [Kommentare](#comments)

### Pinnwände

+++ **[!UICONTROL Pinnwände]**

Dieses Trigger-Modul beginnt mit einem neuen Pinnwand.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!UICONTROL Trello]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung mit [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit] </td> 
   <td> <p>Die maximale Anzahl von Pinnwänden [!DNL Workfront Fusion] wird während eines Ausführungszyklus zurückgegeben.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Erstellen einer Pinnwand]**

Dieses Aktionsmodul erstellt eine neue Pinnwand mit den ausgewählten Einstellungen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!UICONTROL Trello]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung mit [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Name] </td> 
   <td> <p>Geben Sie einen Namen für die neue Pinnwand ein oder ordnen Sie ihn zu.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Beschreibung]</td> 
   <td> <p>Geben Sie bei Bedarf die Beschreibung der Pinnwand ein oder ordnen Sie sie zu.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Organisations-ID]</p> </td> 
   <td> <p>Geben Sie die Kennung der Organisation ein oder ordnen Sie sie zu. Die Organisations-ID kann mithilfe eines anderen Moduls abgerufen werden, z. B. über das Modul "Überwachungsaktivitäten".</p> <p> <img src="assets/id-of-org.png"> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Berechtigungsebene]</p> </td> 
   <td> <p>Die Regeln für Abstimmungen und Kommentaren in den Foren sind je nach Berechtigungsstufe unterschiedlich. Beispiel: Wenn Ihr Forum [!UICONTROL Private] ist und Sie die Abstimmungs- und Kommentarregeln auf [!UICONTROL All] setzen, erhalten Sie einen Fehler. </p> <p>Abstimmung und Kommentar sind auf die folgenden Gruppen für jede Berechtigungsebene beschränkt:</p> 
    <ul> 
     <li><strong>[!UICONTROL Private]</strong>: 
      —&gt;Mitglieder, Mitglieder und Beobachter</li> 
     <li><strong>[!UICONTROL Für Organisation]</strong>: 
      —&gt;Mitglieder, Mitglieder und Beobachter, Mitglieder der Organisation</li> 
     <li><strong>[!UICONTROL Public]</strong>: 
      —&gt;Mitglieder, Mitglieder und Beobachter, Mitglieder der Organisation, Alle</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Abstimmung]</p> </td> 
   <td> <p>Wählen Sie eine Option aus, um festzulegen, wer an dieser Pinnwand teilnehmen kann. Informationen zu den Stimmbeschränkungen für Berechtigungsstufen finden Sie im Feld [!UICONTROL Berechtigungsstufe] .</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Kommentare]</p> </td> 
   <td> <p>Wählen Sie eine Option aus, um festzulegen, wer auf Karten für diese Pinnwand Kommentare abgeben kann. Kommentare zu Berechtigungsebenen finden Sie im Feld [!UICONTROL Berechtigungsebene] .</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Einladungen]</p> </td> 
   <td> <p>Wählen Sie aus, wer andere Personen zu dieser Pinnwand einladen kann.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Self-join]</p> </td> 
   <td> <p>Wählen Sie aus, ob Teammitglieder dem Forum selbst beitreten können oder eingeladen werden müssen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Standardbeschriftungen]</p> </td> 
   <td> <p>Wählen Sie aus, ob der Standardsatz mit Beschriftungen für die neue Pinnwand verwendet werden soll.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Standardlisten]</p> </td> 
   <td> <p>Wählen Sie aus, ob der Standardsatz von Listen zur Pinnwand hinzugefügt werden soll ([!UICONTROL Aufgaben], [!UICONTROL Aufgaben], [!UICONTROL Fertig]).</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Board source ID]</p> </td> 
   <td> <p>Wählen Sie die ID der Pinnwand aus oder ordnen Sie sie zu, die Sie in die neue Pinnwand kopieren möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Kartenabdeckungen]</p> </td> 
   <td> <p>Wählen Sie <strong>[!UICONTROL Ja]</strong> aus, wenn Sie Kartenabschlüsse für die Pinnwand aktivieren möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Hintergrund]</p> </td> 
   <td> <p>Wählen Sie die Hintergrundfarbe oder den benutzerdefinierten Hintergrund aus.</p> <p>Hinweis: Benutzerdefinierte Hintergründe stehen nur [!UICONTROL Trello Gold- und Business Class]-Abonnenten zur Verfügung.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Karten-Alterung]</p> </td> 
   <td> <p>Wählen Sie zwischen zwei Modi der Kartenalterung aus. </p> 
    <ul> 
     <li><strong>[!UICONTROL Normal]</strong>: Karten werden im Alter immer transparenter. </li> 
     <li><strong>[!UICONTROL Pirate]</strong>: Karten reißen, gelb und rissen wie eine alte Piratenkarte, wenn sie altern.</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Bearbeiten einer Pinnwand]**

Dieses Aktionsmodul bearbeitet die Einstellungen einer vorhandenen Pinnwand.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!UICONTROL Trello]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung mit [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Pinnwandkennung]</p> </td> 
   <td> <p>Geben Sie die eindeutige [!UICONTROL Trello]-ID der Pinnwand ein oder ordnen Sie sie zu, die das Modul erstellen soll. Sie können die Pinnwand-ID mit einem anderen Modul abrufen, z. B. dem Modul "Pinnwände"</p> <p> <img src="assets/watch-boards.png"> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Neuer Name]</td> 
   <td> <p> Geben Sie einen neuen Namen für die Pinnwand ein oder ordnen Sie ihn zu.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Neue Beschreibung]</td> 
   <td> <p> Geben Sie bei Bedarf eine neue Pinnwandbeschreibung ein oder ordnen Sie sie zu.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Organisations-ID]</p> </td> 
   <td> <p>Geben Sie die eindeutige [!UICONTROL Trello]-ID der Pinnwand ein oder ordnen Sie sie zu, die das Modul bearbeiten soll. Sie können die Pinnwand-ID mit einem anderen Modul abrufen, z. B. dem Modul [!DNL Watch Activities] .</p> <p> <img src="assets/org-id.png"> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Abonnieren] </td> 
   <td> <p>Wählen Sie eine Option aus, um anzugeben, ob der aktive Benutzer die Pinnwand abonniert hat.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Berechtigungsebene]</p> </td> 
   <td> <p>Die Regeln für Abstimmungen und Kommentaren in den Foren sind je nach Berechtigungsstufe unterschiedlich. Beispiel: Wenn Ihr Forum [!UICONTROL Private] ist und Sie die Abstimmungs- und Kommentarregeln auf [!UICONTROL All] setzen, erhalten Sie einen Fehler. </p> <p>Abstimmung und Kommentar sind auf die folgenden Gruppen für jede Berechtigungsebene beschränkt:</p> 
    <ul> 
     <li><strong>[!UICONTROL Private]</strong>: 
      —&gt;Mitglieder, Mitglieder und Beobachter</li> 
     <li><strong>[!UICONTROL Für Organisation]</strong>: 
      —&gt;Mitglieder, Mitglieder und Beobachter, Mitglieder der Organisation</li> 
     <li><strong>[!UICONTROL Public]</strong>: 
      —&gt;Mitglieder, Mitglieder und Beobachter, Mitglieder der Organisation, Alle</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Abstimmung]</p> </td> 
   <td> <p>Wählen Sie eine Option aus, um festzulegen, wer an dieser Pinnwand teilnehmen kann. Informationen zu den Stimmbeschränkungen für Berechtigungsstufen finden Sie im Feld [!UICONTROL Berechtigungsstufe] .</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Kommentare]</p> </td> 
   <td> <p>Wählen Sie eine Option aus, um festzulegen, wer auf Karten für diese Pinnwand Kommentare abgeben kann. Kommentare zu Berechtigungsebenen finden Sie im Feld [!UICONTROL Berechtigungsebene] .</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Einladungen] </td> 
   <td> <p>Wählen Sie aus, wer Personen zu dieser Pinnwand einladen kann.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Self-join]</td> 
   <td> <p> Wählen Sie aus, ob Teammitglieder dem Forum selbst beitreten können oder eingeladen werden müssen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Kartenabdeckungen]</td> 
   <td> <p> Wählen Sie aus, ob Kartenabdeckungen auf dieser Pinnwand angezeigt werden sollen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Hintergrund] </td> 
   <td> <p>Wählen Sie die Hintergrundfarbe oder den benutzerdefinierten Hintergrund aus.</p> <p>Hinweis: Benutzerdefinierte Hintergründe stehen nur [!UICONTROL Trello Gold- und Business Class]-Abonnenten zur Verfügung.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Hintergrund-ID]</td> 
   <td> <p> Wenn Sie im Feld [!UICONTROL Hintergrund] einen benutzerdefinierten Hintergrund ausgewählt haben, geben Sie die Kennung des zu verwendenden Hintergrunds ein oder ordnen Sie sie zu.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Karten-Alterung]</p> </td> 
   <td> <p>Wählen Sie zwischen zwei Modi der Kartenalterung aus. </p> 
    <ul> 
     <li><strong>[!UICONTROL Normal]</strong>: Karten werden im Alter immer transparenter. </li> 
     <li><strong>[!UICONTROL Pirate]</strong>: Karten reißen, gelb und rissen wie eine alte Piratenkarte, wenn sie altern.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Kalender-Feed aktiviert]</td> 
   <td> <p> Wählen Sie aus, ob der Kalender-Feed aktiviert ist.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL &lt;Color&gt; label name]</td> 
   <td> <p> Weisen Sie der gewünschten Farbbeschriftung einen Namen zu.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Archiv] </td> 
   <td> <p>Wählen Sie eine Option aus, um anzugeben, ob Sie die Pinnwand archivieren (schließen) möchten. </p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Pinnwand abrufen]**

Dieses Aktionsmodul ruft die Details einer Pinnwand ab.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!UICONTROL Trello]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung mit [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Pinnwandkennung]</p> </td> 
   <td> <p>Geben Sie die ID der Pinnwand ein oder ordnen Sie sie zu, über die Sie Informationen abrufen möchten.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!DNL Search for Boards]**

Dieses Suchmodul ruft Informationen zu einer von Ihnen angegebenen Pinnwand ab.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!UICONTROL Trello]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung mit [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Abfrage] </td> 
   <td> <p>Geben Sie den Namen (oder einen Teil des Namens) der Pinnwand ein oder ordnen Sie ihn zu, über die Sie Informationen erhalten möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Maximale Anzahl der zurückgegebenen Pinnwände]</td> 
   <td> <p> Geben Sie die maximale Anzahl von Pinnwänden ein, die [!DNL Workfront Fusion] während eines Ausführungszyklus zurückgibt. Dieser Wert muss kleiner oder gleich 1000 sein.</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Teil] </p> </td> 
   <td> <p>Standardmäßig sucht dieses Modul den Mitgliederinhalt nach exakten Übereinstimmungen jedes Wortes in Ihrer Abfrage. Wenn [!UICONTROL Partial] aktiviert ist, sucht das Modul nach Inhalten, die mit einem beliebigen Wort in Ihrer Abfrage beginnen.</p> <p> Wenn Sie beispielsweise das Wort "Entwicklung"verwenden, um nach einer Pinnwand mit dem Titel "Mein Entwicklungsstatus-Bericht"zu suchen, müssen Sie standardmäßig nach dem gesamten Wort suchen. Wenn Sie [!UICONTROL Partial] aktiviert haben, können Sie nach "dev", aber nicht nach "development"suchen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Pinnwände] </td> 
   <td> <p>Geben Sie "mine"ein oder ordnen Sie eine kommagetrennte Liste von Pinnwand-IDs zu.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Archivieren oder Archivieren einer Pinnwand aufheben]**

Dieses Aktionsmodul schließt oder öffnet eine von Ihnen angegebene Pinnwand erneut.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!UICONTROL Trello]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung mit [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Pinnwandkennung]</td> 
   <td> <p> Geben Sie die ID der Pinnwand ein oder ordnen Sie sie zu, die Sie schließen oder erneut öffnen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Archiv oder Archivierung aufheben]</td> 
   <td> <p> Wählen Sie aus, ob Sie die Pinnwand schließen (archivieren) oder erneut öffnen (Archivierung aufheben) möchten.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Mitglieder einer Pinnwand zuweisen]**

Dieses Aktionsmodul weist ein Mitglied einer Pinnwand zu, die Sie angeben.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!UICONTROL Trello]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung mit [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Pinnwandkennung]</td> 
   <td> <p> Wählen Sie die Pinnwand aus, der Sie ein Mitglied hinzufügen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL E-Mail-Adresse]</td> 
   <td> <p> Geben Sie die E-Mail-Adresse des Mitglieds ein, das Sie zur Pinnwand hinzufügen möchten, oder ordnen Sie sie zu.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Mitgliedertyp]</p> </td> 
   <td> <p>Wählen Sie den Typ des Mitglieds aus, das Sie der Pinnwand hinzufügen möchten.</p> 
    <ul> 
     <li><strong>[!UICONTROL Admin]</strong>: Ein Pinnwandadministrator kann jede beliebige Pinnwandaktion auf der Pinnwand durchführen.</li> 
     <li><strong>[!UICONTROL Normal]</strong>: Ein normales Mitglied ist einfach Mitglied der Pinnwand.</li> 
     <li><strong>[!UICONTROL Beobachter]</strong>: Ein Beobachter ist Mitglied mit schreibgeschütztem Zugriff auf die Pinnwand. <br>Beobachter sind nur für Teams mit [!UICONTROL Trello Business Class] verfügbar.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Vollständiger Name]</td> 
   <td> <p> Geben Sie den vollständigen Namen des Benutzers ein, den Sie der Pinnwand hinzufügen möchten.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Zuweisung eines Mitglieds zu einer Pinnwand aufheben]**

Dieses Aktionsmodul entfernt ein Mitglied aus einer Pinnwand.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!UICONTROL Trello]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung mit [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Pinnwandkennung]</td> 
   <td> <p> Geben Sie die ID der Pinnwand ein (zuordnen oder auswählen), aus der Sie den Benutzer entfernen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Mitglied] </td> 
   <td> <p>Wählen Sie das Element aus, das Sie aus der Pinnwand entfernen möchten.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

### Listen

+++ **[!UICONTROL Überwachungskarten in eine Liste verschoben]**

Dieses Trigger-Modul wird aktiviert, wenn eine Karte in eine bestimmte Liste verschoben wird.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!UICONTROL Trello]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung mit [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Board]</td> 
   <td>Wählen Sie die Pinnwand aus, die die Liste enthält, die Sie auf Karten achten möchten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Liste]</td> 
   <td>Wählen Sie die Liste aus, die Sie auf Karten achten möchten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit] </td> 
   <td> <p>Die maximale Anzahl der Karten [!DNL Workfront Fusion] wird während eines Ausführungszyklus zurückgegeben.</p>  </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Erstellen einer Liste]**

Dieses Aktionsmodul erstellt eine Liste auf einer Pinnwand, die Sie angeben.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!UICONTROL Trello]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung mit [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Pinnwandkennung]</td> 
   <td> <p> Geben Sie die Kennung der Pinnwand ein oder ordnen Sie sie zu, auf der Sie eine Liste erstellen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Name] </td> 
   <td> <p>Geben Sie einen Namen für die neue Liste ein oder ordnen Sie ihn zu.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Position] </td> 
   <td> <p>Wählen Sie aus, ob Sie die Liste oben hinzufügen oder am unteren Rand der Karte anhängen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Liste kopieren]</td> 
   <td> <p> Wählen Sie aus, wie die Kennung der Liste eingegeben werden soll, die Sie kopieren möchten.</p> 
    <ul> 
     <li> <p><strong>Eingabetaste manuell</strong> </p> <p>Geben Sie im Feld <strong>[!UICONTROL List ID]</strong> die Kennung der Liste ein, die Sie kopieren möchten, oder ordnen Sie sie zu.<br></p> </li> 
     <li> <p><strong>Select</strong> </p> <p>Wählen Sie die Pinnwand aus, die die zu kopierende Liste enthält, und wählen Sie dann die Liste aus.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Eine Liste bearbeiten]**

Dieses Aktionsmodul bearbeitet eine vorhandene Liste.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!UICONTROL Trello]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung mit [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Listen-ID]</td> 
   <td> <p> Geben Sie die Kennung der Liste ein, die Sie aktualisieren möchten, oder ordnen Sie sie zu.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Name] </td> 
   <td> <p>Geben Sie einen neuen Namen für die Liste ein oder ordnen Sie ihn zu.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Pinnwandkennung]</td> 
   <td> <p> Ordnen Sie die Pinnwand zu oder wählen Sie sie aus, auf der Sie die Liste verschieben möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Position] </td> 
   <td> <p>Wählen Sie aus, ob Sie die Liste oben hinzufügen oder am unteren Rand der Karte anhängen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Abonniert]</td> 
   <td> <p>Aktivieren Sie diese Option, wenn Sie das aktive Mitglied für die Liste anmelden möchten.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Liste abrufen]**

Dieses Aktionsmodul ruft Details zu einer bestimmten Liste ab.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!UICONTROL Trello]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung mit [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Listen-ID]</p> </td> 
   <td> <p>Geben Sie die Kennung der Liste ein oder ordnen Sie sie zu, über die Sie Informationen abrufen möchten.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

### Karten

+++ **[!UICONTROL Karten beobachten]**

Dieses Trigger-Modul wird aktiviert, wenn eine neue Karte hinzugefügt wird.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!UICONTROL Trello]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung mit [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Watched Object]</td> 
   <td> <p>Wählen Sie die Position aus, die Sie für Karten beobachten möchten.</p> 
    <ul> 
     <li><strong>[!UICONTROL Alle Karten]</strong> </li> 
     <li> <p><strong>Karten auf einer bestimmten Pinnwand</strong> </p> <p>Wählen Sie die Pinnwand aus, die Sie auf Karten überwachen möchten</p> </li> 
     <li> <p><strong>[!UICONTROL Karten auf einer bestimmten Liste]</strong> </p> <p>Wählen Sie die Pinnwand aus, die die Liste enthält, die Sie auf Karten achten möchten, und wählen Sie dann die Liste aus.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit] </td> 
   <td> <p>Die maximale Anzahl der Karten [!DNL Workfront Fusion] wird während eines Ausführungszyklus zurückgegeben.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Erstellen einer Karte]**

Dieses Aktionsmodul erstellt eine Karte in einer ausgewählten Liste.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!UICONTROL Trello]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung mit [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Listen-ID eingeben]</td> 
   <td> <p> Wählen Sie aus, wie die Kennung der Liste eingegeben werden soll, in der Sie eine Karte hinzufügen möchten.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL manuell eingeben]</strong> </p> <p>Geben Sie im Feld <strong>[!UICONTROL List ID]</strong> die Kennung der Liste ein, der Sie eine Karte hinzufügen möchten, oder ordnen Sie sie zu.<br></p> </li> 
     <li> <p><strong>[!UICONTROL Select]</strong> </p> <p>Wählen Sie die Pinnwand aus, die die zu kopierende Liste enthält, und wählen Sie dann die Liste aus.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Beschriftungen] </td> 
   <td> <p>Geben Sie für jeden Titel, den Sie der Karte hinzufügen möchten, die Kennung des Titels ein. Die ID kann beispielsweise mithilfe des Moduls [!UICONTROL Bezeichnungen abrufen] abgerufen werden.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Member]</td> 
   <td>Geben Sie für jedes Mitglied, das Sie der Karte hinzufügen möchten, die Kennung des Mitglieds ein. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Name] </td> 
   <td> <p>Geben Sie einen Namen für die neue Karte ein.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Beschreibung]</p> </td> 
   <td> <p>Geben Sie die Beschreibung für die Karte ein.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Position] </td> 
   <td> <p>Wählen Sie aus, ob Sie die Karte oben hinzufügen oder die Karte am Ende der Liste anhängen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Fälligkeitsdatum]</td> 
   <td> <p> Geben Sie ein Fälligkeitsdatum für die Karte ein. Eine Liste der unterstützten Datums- und Uhrzeitformate finden Sie unter <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Typerzwingung in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Fällig abgeschlossen]</td> 
   <td> <p> Aktivieren Sie diese Option, um zu kennzeichnen, dass die Karte am Fälligkeitsdatum abgeschlossen ist.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Datei-URL]</td> 
   <td> <p>Geben Sie die URL einer Datei ein oder ordnen Sie sie der Karte als Anlage hinzu.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Source-Datei]</p> </td> 
   <td> <p>Geben Sie Informationen für eine Datei ein, die Sie als Anlage zur Karte hinzufügen möchten, oder ordnen Sie sie zu.</p> 
    <ul> 
     <li>[!UICONTROL Dateiname]: Geben Sie den Dateinamen einschließlich der Dateierweiterung ein oder ordnen Sie ihn zu.</li> 
     <li> 
     <p>Wählen Sie eine Datei aus einem vorherigen Modul aus oder ordnen Sie den Namen und die Daten der Datei zu.</p> 
     <p>Hinweis: Pro Anhang gilt eine Upload-Grenze von 10 MB. Die Mitglieder [!UICONTROL Business Class] und [!UICONTROL Trello Gold] haben jedoch eine Dateiupload-Grenze von 250 MB pro Anlage.</p> 
     </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Kopierkarte]</td> 
   <td> <p> Wählen Sie aus, wie Sie die Kennung der Karte eingeben möchten, die Sie kopieren möchten.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL manuell eingeben]</strong> </p> <p>Geben Sie im Feld <strong>[!UICONTROL Card ID]</strong> die ID der Karte ein, die Sie kopieren möchten, oder ordnen Sie sie zu.<br></p> </li> 
     <li> <p><strong>[!UICONTROL Select]</strong> </p> <p>Wählen Sie die Pinnwand aus, die die zu kopierende Karte enthält, wählen Sie dann die Liste aus, die die Karte enthält, und wählen Sie dann die Karte aus.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Bearbeiten einer Karte]**

Dieses Aktionsmodul bearbeitet eine vorhandene Karte.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!UICONTROL Trello]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung mit [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Karten-ID eingeben]</td> 
   <td> <p> Wählen Sie aus, wie Sie die Kennung der Karte eingeben möchten, die Sie bearbeiten möchten.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL manuell eingeben]</strong> </p> <p>Geben Sie im Feld <strong>[!UICONTROL Card ID]</strong> die ID der Karte ein, die Sie bearbeiten möchten, oder ordnen Sie sie zu.<br></p> </li> 
     <li> <p><strong>[!UICONTROL Select]</strong> </p> <p>Wählen Sie die Pinnwand mit der Karte aus, die Sie bearbeiten möchten, wählen Sie die Liste aus, die die Karte enthält, und wählen Sie dann die Karte aus.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Neuer Name]</td> 
   <td> <p>Geben Sie einen neuen Namen für die Karte ein oder ordnen Sie ihn zu.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Neue Beschreibung]</p> </td> 
   <td> <p>Geben Sie eine neue Beschreibung für die Karte ein oder ordnen Sie sie zu.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Karte verschieben]</p> </td> 
   <td> <p>Wählen Sie die Pinnwand oder die Pinnwand und Liste aus, in die Sie die Karte verschieben möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Beschriftungen] </td> 
   <td> <p>Fügen Sie die IDs aller Bezeichnungen hinzu, die Sie zur Karte hinzufügen möchten. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Position] </td> 
   <td> <p>Wählen Sie aus, ob Sie die Karte oben hinzufügen oder die Karte am Ende der Liste anhängen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Fälligkeitsdatum]</td> 
   <td> <p> Geben Sie ein Fälligkeitsdatum für die Karte ein. Eine Liste der unterstützten Datums- und Uhrzeitformate finden Sie unter <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Typerzwingung in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Fällig abgeschlossen]</td> 
   <td> <p> Wenn diese Option aktiviert ist, wird die Karte am Fälligkeitsdatum als abgeschlossen markiert.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Member] </td> 
   <td> <p>Fügen Sie die ID aller Mitglieder hinzu oder ordnen Sie sie der Karte zu.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Attachment Cover ID]</p> </td> 
   <td> <p>Geben Sie die ID des Bildanhangs ein oder ordnen Sie sie zu, den die Karte als Deckblatt verwenden soll.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Abonnieren] </td> 
   <td> <p>Wählen Sie aus, ob das Mitglied für die Karte angemeldet sein soll.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Archiv] </td> 
   <td> <p>Wählen Sie eine Option aus, um anzugeben, ob Sie die Karte archivieren (schließen) möchten. </p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Eine Karte abrufen]**

Dieses Aktionsmodul ruft die Details einer ausgewählten Karte ab.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!UICONTROL Trello]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung mit [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Pinnwandkennung]</td> 
   <td> <p>Geben Sie die ID der Pinnwand ein, die die Karte enthält, über die Sie Details abrufen möchten. Auf diese Weise können Sie die Namen der benutzerdefinierten Felder der Pinnwand anzeigen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Karte-ID]</td> 
   <td> <p> Wählen Sie aus, wie Sie die Kennung der Karte eingeben möchten, über die Sie Details abrufen möchten.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL manuell eingeben]</strong> </p> <p>Geben Sie im Feld <strong>[!UICONTROL Card ID]</strong> die ID der Karte ein, über die Sie Details abrufen möchten, oder ordnen Sie sie zu.<br></p> </li> 
     <li> <p><strong>[!UICONTROL Select]</strong> </p> <p>Wählen Sie die Pinnwand aus, die die Karte enthält, über die Sie Details abrufen möchten, wählen Sie dann die Liste aus, die die Karte enthält, und wählen Sie dann die Karte aus.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Suche nach Karten]**

Dieses Aktionsmodul gibt Karten zurück, die mit der Suchabfrage übereinstimmen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!UICONTROL Trello]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung mit [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Board] </td> 
   <td> <p>Wählen Sie die Pinnwände aus, die durchsucht werden sollen. Wenn keine Pinnwand ausgewählt ist, werden alle Pinnwände durchsucht.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Abfrage]</p> </td> 
   <td> <p>Geben Sie die Suchabfrage ein. Sie können Ihre Suche mithilfe der folgenden Suchoperatoren verfeinern:</p> 
    <ul> 
     <li><code><strong>-operator</strong></code> <p>Sie können jedem Operator "-"hinzufügen, um eine negative Suche durchzuführen, z. B. <code>[!UICONTROL -has:members]</code>, um nach Karten zu suchen, denen keine Mitglieder zugewiesen sind.</p> </li> 
     <li><code><strong>@name</strong></code> <p>Gibt einem Mitglied zugewiesene Karten zurück. Sie können auch <code>member:</code> verwenden. Verwenden Sie <code>@me</code> , um nur Ihre Karten einzuschließen.</p> </li> 
     <li><code><strong>#label</strong></code> <p>Gibt gekennzeichnete Karten zurück. Sie können auch <code>label:</code> verwenden. Beispielsweise gibt <code>label:"FIX IT"</code> Karten mit der Bezeichnung "FIX IT"zurück.</p> </li> 
     <li><code><strong>board:id</strong></code> <p>Gibt Karten innerhalb einer bestimmten Pinnwand zurück. Beispielsweise gibt <code>board:Trello</code> Karten auf Pinnwänden mit [!UICONTROL Trello] im Pinnwandnamen zurück.</p> </li> 
     <li><code><strong>list:name</strong></code> <p>Gibt Karten innerhalb der Liste mit dem Namen "name"zurück.</p> </li> 
     <li><code><strong>has:attachments</strong></code> <p>Gibt Karten mit Anlagen zurück. Der Operator <code>has</code>: kann auch mit anderen Attributen wie <code>has:description</code>, <code>has:cover</code>, <code>has:members</code> oder <code>has:stickers</code> verwendet werden.</p> </li> 
     <li><code><strong>due:day</strong></code> <p>Gibt alle Karten zurück, die innerhalb von 24 Stunden fällig sind. Der Operator <code>due:</code> kann auch mit anderen Zeitrahmen wie <code>due:week</code>, <code>due:month</code> oder <code>due:overdue</code> verwendet werden. Sie können auch nach einem bestimmten Tagesbereich suchen. Wenn Sie beispielsweise <code>due:14</code> zur Suche hinzufügen, werden die Karten, die in den nächsten 14 Tagen fällig sind, einbezogen.</p> </li> 
     <li><code><strong>created:day</strong></code> <p>Gibt in den letzten 24 Stunden erstellte Karten zurück. Der <code> created:</code> -Operator kann auch mit anderen Zeitrahmen wie <code>created:week</code> oder <code>created:month</code> verwendet werden. Sie können auch nach einem bestimmten Tagesbereich suchen. Wenn Sie beispielsweise <code>created:14</code> zur Suche hinzufügen, werden Karten angezeigt, die in den letzten 14 Tagen erstellt wurden.</p> </li> 
     <li><code><strong>edited:day</strong></code> <p>Gibt die in den letzten 24 Stunden bearbeiteten Karten zurück. Der Operator <code>edited:</code> kann auch mit anderen Zeitrahmen wie <code>edited:week</code> oder <code>edited:month</code> verwendet werden. Sie können auch nach einem bestimmten Tagesbereich suchen. Wenn Sie beispielsweise <code>edited:21</code> zur Suche hinzufügen, werden auch die Karten angezeigt, die in den letzten 21 Tagen bearbeitet wurden.</p> </li> 
     <li><code><strong>description:</strong>, <strong>checklist:</strong>, <strong>comment:</strong>, and <strong>name:</strong></code> <p>Gibt Karten zurück, die dem Text von Kartenbeschreibungen, Checklisten, Kommentaren oder Namen entsprechen. Beispiel: "FIX IT"gibt Karten mit "FIX IT"in einem Kommentar zurück.</p> </li> 
     <li><code><strong>is:open</strong> and <strong>is:archived</strong></code> <p>Gibt offene oder archivierte Karten zurück. Wenn keiner der beiden Typen angegeben ist, gibt [!UICONTROL Trello] beide Typen zurück.</p> </li> 
     <li><code><strong>is:starred</strong> </code> <p>Nur Karten auf Startplatinen sind enthalten.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Maximale Anzahl zurückgegebener Karten]</td> 
   <td> <p> Die maximale Anzahl der Karten [!DNL Workfront Fusion] wird während eines Ausführungszyklus zurückgegeben. Dieser Wert muss kleiner oder gleich 1000 sein.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Teil] </td> 
   <td> <p>Standardmäßig sucht dieses Modul den Mitgliederinhalt nach exakten Übereinstimmungen jedes Wortes in Ihrer Abfrage. Wenn [!UICONTROL Partial] aktiviert ist, sucht das Modul nach Inhalten, die mit einem beliebigen Wort in Ihrer Abfrage beginnen.</p> <p> Wenn Sie beispielsweise das Wort "Entwicklung"verwenden, um nach einer Pinnwand mit dem Titel "Mein Entwicklungsstatus-Bericht"zu suchen, müssen Sie standardmäßig nach dem gesamten Wort suchen. Wenn Sie [!UICONTROL Partial] aktiviert haben, können Sie nach "dev", aber nicht nach "development"suchen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Karten] </td> 
   <td> <p>Fügen Sie alle Karten hinzu, nach denen Sie speziell suchen möchten.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Archivieren oder Archivieren einer Karte aufheben]**

Dieses Aktionsmodul archiviert oder sendet eine Karte zurück an die Pinnwand.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!UICONTROL Trello]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung mit [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Karten-ID]</td> 
   <td> <p> Geben Sie die Kennung der Karte ein, die Sie archivieren oder an die Pinnwand zurücksenden möchten, oder ordnen Sie sie zu.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Archiv oder Archivierung aufheben]</td> 
   <td> <p> Wählen Sie aus, ob Sie die Karte (Archiv) schließen oder zurück an die Pinnwand senden möchten (Archivierung aufheben).</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Anlage hinzufügen]**

Dieses Aktionsmodul fügt der ausgewählten Karte einen Anhang hinzu.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!UICONTROL Trello]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung mit [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Karte-ID]</td> 
   <td> <p> Wählen Sie aus, wie Sie die Kennung der Karte eingeben möchten, über die Sie Details abrufen möchten.</p> 
    <ul> 
     <li> <p><strong>Eingabetaste manuell</strong> </p> <p>Geben Sie im Feld <strong>[!UICONTROL Card ID]</strong> die ID der Karte ein, über die Sie Details abrufen möchten, oder ordnen Sie sie zu.<br></p> </li> 
     <li> <p><strong>[!UICONTROL Select]</strong> </p> <p>Wählen Sie die Pinnwand aus, die die Karte enthält, über die Sie Details abrufen möchten, wählen Sie dann die Liste aus, die die Karte enthält, und wählen Sie dann die Karte aus.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Anlagentyp]</p> </td> 
   <td> <p>Wählen Sie aus, ob Sie die Datei direkt hochladen möchten, oder geben Sie eine URL für die Datei an.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Datei]</strong> </p> <p>Wählen Sie eine Quelldatei aus einem vorherigen Modul aus oder ordnen Sie den Namen und die Daten der Quelldatei zu.</p> </li> 
     <li> <p><strong>[!UICONTROL URL]</strong> </p> <p>Geben Sie die URL zur Datei ein und geben Sie einen Namen für die Anlage an.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

+++

### Abonnenten

+++ **[!UICONTROL Mitglieder einer Pinnwand zuweisen]**

Siehe &quot;[!UICONTROL Zuweisen eines Mitglieds zu einer Pinnwand]&quot;unter [Pinnwände](#boards).

+++

+++ **[!UICONTROL Zuweisung eines Mitglieds zu einer Pinnwand aufheben]**

Siehe &quot;[!UICONTROL Zuweisung eines Mitglieds aus einer Pinnwand aufheben]&quot;unter [Pinnwände](#boards).

+++

+++ **[!UICONTROL Mitglieder zu einer Karte hinzufügen]**

Dieses Aktionsmodul fügt das angegebene Element zur angegebenen Karte hinzu.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!UICONTROL Trello]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung mit [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Karte-ID und Mitglieds-ID eingeben]</p> </td> 
   <td> <p>Wählen Sie aus, wie Sie die Karten-ID und die Mitglieds-ID eingeben möchten.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL manuell eingeben]</strong> </p> <p>Geben Sie die <strong>[!UICONTROL Karten-ID]</strong> und die <strong>[!UICONTROL Mitglieds-ID]</strong> ein oder ordnen Sie sie zu.</p> </li> 
     <li> <p><strong>[!UICONTROL Select]</strong> </p> <p>Wählen Sie die Pinnwand aus, die die Karte enthält, der Sie ein Mitglied hinzufügen möchten, und wählen Sie dann die Liste aus, die die Karte enthält, die Karte selbst und das Mitglied, das Sie der Karte hinzufügen möchten.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Suche nach Mitgliedern]**

Dieses Aktionsmodul ruft Informationen zu [!UICONTROL Trello] -Mitgliedern ab.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!UICONTROL Trello]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung mit [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Abfrage] </td> 
   <td> <p>Geben Sie den vollständigen Namen oder Benutzernamen des Benutzers ein, den Sie suchen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Teil] </td> 
   <td> <p>Standardmäßig sucht dieses Modul den Mitgliederinhalt nach exakten Übereinstimmungen jedes Wortes in Ihrer Abfrage. Wenn [!UICONTROL Partial] aktiviert ist, sucht das Modul nach Inhalten, die mit einem beliebigen Wort in Ihrer Abfrage beginnen.</p> <p> Wenn Sie beispielsweise das Wort "Entwicklung"verwenden, um nach einer Pinnwand mit dem Titel "Mein Entwicklungsstatus-Bericht"zu suchen, müssen Sie standardmäßig nach dem gesamten Wort suchen. Wenn Sie [!UICONTROL Partial] aktiviert haben, können Sie nach "dev", aber nicht nach "development"suchen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Maximale Anzahl der zurückgegebenen Mitglieder]</td> 
   <td> <p> Die maximale Anzahl der Mitglieder [!DNL Workfront Fusion] gibt während eines Ausführungszyklus zurück.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

### Checklisten

+++ **[!UICONTROL Erstellen einer Checkliste]**

Dieses Aktionsmodul erstellt eine Checkliste auf der ausgewählten Karte.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!UICONTROL Trello]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung mit [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Kartenkennung eingeben]</td> 
   <td> <p> Wählen Sie aus, wie Sie die Kennung der Karte eingeben möchten, auf der Sie eine Checkliste hinzufügen möchten.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL manuell eingeben]</strong> </p> <p>Geben Sie im Feld <strong>[!UICONTROL Card ID]</strong> die ID der Karte ein, der Sie eine Checkliste hinzufügen möchten, oder ordnen Sie sie zu.<br></p> </li> 
     <li> <p><strong>[!UICONTROL Select]</strong> </p> <p>Wählen Sie die Pinnwand mit der Karte aus, auf der Sie eine Checkliste hinzufügen möchten, wählen Sie dann die Liste aus, die die Karte enthält, und wählen Sie dann die Karte aus.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Name] </td> 
   <td> <p>Geben Sie einen Namen für die Checkliste ein oder ordnen Sie ihn zu.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Position] </td> 
   <td> <p>Wählen Sie aus, ob Sie die Checkliste oben oder [!UICONTROL die] Checkliste am unteren Rand der Karte anhängen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Checklisten-ID eingeben]</p> </td> 
   <td> <p>Geben Sie die Kennung einer Quell-Checkliste ein oder ordnen Sie sie zu, die Sie in die neue Checkliste kopieren möchten.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Erstellen eines Checklisten-Elements]**

Dieses Aktionsmodul fügt ein Element zu einer bestimmten Checkliste hinzu.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!UICONTROL Trello]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung mit [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Checklisten-ID eingeben]</td> 
   <td> <p> Wählen Sie aus, wie Sie die Kennung der Checkliste eingeben möchten, der Sie ein Element hinzufügen möchten.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL manuell eingeben]</strong> </p> <p>Geben Sie im Feld <strong>[!UICONTROL Checkliste-ID]</strong> die Kennung der Karte ein, der Sie eine Checkliste hinzufügen möchten, oder ordnen Sie sie zu.<br></p> </li> 
     <li> <p><strong>[!UICONTROL Select]</strong> </p> <p>Wählen Sie die Pinnwand mit der Karte aus, auf der Sie eine Checkliste hinzufügen möchten, wählen Sie dann die Liste aus, die die Karte enthält, wählen Sie die Karte aus und wählen Sie dann die Checkliste aus.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Elementname]</p> </td> 
   <td> <p>Geben Sie einen Namen für das neue Element ein oder ordnen Sie ihn zu.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Position]</p> </td> 
   <td> <p>Wählen Sie aus, ob das Element oben oder am Ende der Checkliste angehängt werden soll.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Checked]</p> </td> 
   <td> <p>Aktivieren Sie diese Option, wenn Sie das Element wie bereits aktiviert hinzufügen möchten.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Bearbeiten eines Checklisten-Elements]**

Dieses Aktionsmodul bearbeitet eine vorhandene Checkliste.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!UICONTROL Trello]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung mit [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Karten-ID und Checklisten-Element-ID eingeben]</td> 
   <td> <p> Wählen Sie aus, wie Sie die Kennung der Karte und Checkliste eingeben möchten, in der Sie ein Element bearbeiten möchten.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL manuell eingeben]</strong> </p> <p>Geben Sie im Feld <strong>[!UICONTROL Checkliste-ID]</strong> die Kennung der Karte ein, der Sie eine Checkliste hinzufügen möchten, oder ordnen Sie sie zu.</p> <p>Geben Sie im Feld <strong>[!UICONTROL Checklist Item ID]</strong> die Kennung der Checkliste ein oder ordnen Sie sie zu.</p> </li> 
     <li> <p><strong>[!UICONTROL Select]</strong> </p> <p>Wählen Sie die Pinnwand mit der Karte aus, auf der Sie eine Checkliste hinzufügen möchten, wählen Sie dann die Liste aus, die die Karte enthält, wählen Sie die Karte aus und wählen Sie dann die Checkliste aus.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Checklisten-ID]</td> 
   <td>Wählen Sie die Checkliste aus oder ordnen Sie sie zu, in die Sie das Checklisten-Element verschieben möchten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Elementname]</p> </td> 
   <td> <p>Geben Sie einen Namen für das neue Element ein oder ordnen Sie ihn zu.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Position]</p> </td> 
   <td> <p>Wählen Sie aus, ob das Element oben oder unten in der Checkliste angehängt werden soll.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL State]</p> </td> 
   <td> <p>Wählen Sie aus, ob das Element der Checkliste vollständig oder unvollständig ist.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

### Kennzeichnungen

+++ **[!UICONTROL Hinzufügen einer Bezeichnung zu einer Karte]**

Dieses Aktionsmodul fügt einer ausgewählten Karte eine Bezeichnung hinzu.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!UICONTROL Trello]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung mit [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Karte-ID]</td> 
   <td> <p> Wählen Sie aus, wie Sie die Kennung der Karte eingeben möchten, auf der Sie eine Checkliste hinzufügen möchten.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL manuell eingeben]</strong> </p> <p>Geben Sie im Feld <strong>[!UICONTROL Card ID]</strong> die ID der Karte ein, der Sie eine Checkliste hinzufügen möchten, oder ordnen Sie sie zu. Geben Sie im Feld<strong>[!UICONTROL Titel-ID]</strong> die Kennung der Bezeichnung ein, die Sie hinzufügen möchten, oder ordnen Sie sie zu.<br></p> </li> 
     <li> <p><strong>[!UICONTROL Select]</strong> </p> <p>Wählen Sie die Pinnwand mit der Karte aus, auf der Sie eine Checkliste hinzufügen möchten, wählen Sie dann die Liste aus, die die Karte enthält, und wählen Sie dann die Karte aus. </p> <p>Wählen Sie den Titel aus, den Sie der Karte hinzufügen möchten.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

+++

### Kommentare

+++ **[!UICONTROL Kommentare ansehen]**

Ruft Kommentardetails ab, wenn sich ein neuer Kommentar an einem angegebenen Speicherort befindet.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!UICONTROL Trello]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung mit [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Watched Object]</td> 
   <td> <p>Wählen Sie den Speicherort aus, den Sie für Kommentare überwachen möchten.</p> 
    <ul> 
     <li><strong>[!UICONTROL Alle Karten] überall</strong> </li> 
     <li> <p><strong>[!UICONTROL Pinnwand]</strong> </p> <p>Wählen Sie die Pinnwand aus, die Sie für Kommentare überwachen möchten</p> </li> 
     <li> <p><strong>[!UICONTROL List]</strong> </p> <p>Wählen Sie die Pinnwand aus, die die Liste enthält, die Sie für Kommentare überwachen möchten, und wählen Sie dann die Liste aus.</p> </li> 
     <li><strong>[!UICONTROL Card]</strong> </li> 
     <li>Wählen Sie die Pinnwand aus, die die Karte enthält, die Sie für Kommentare ansehen möchten, wählen Sie dann die Liste aus, die die Karte enthält, und wählen Sie dann die Karte aus.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit] </td> 
   <td> <p>Die maximale Anzahl von Kommentaren [!DNL Workfront Fusion] wird während eines Ausführungszyklus zurückgegeben.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Erstellen eines Kommentars in einer Karte]**

Dieses Aktionsmodul fügt einer ausgewählten Karte einen Kommentar hinzu.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!UICONTROL Trello]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung mit [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Kartenkennung eingeben]</td> 
   <td> <p> Wählen Sie aus, wie Sie die Kennung der Karte eingeben möchten, auf der Sie einen Kommentar hinzufügen möchten.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL manuell eingeben]</strong> </p> <p>Geben Sie im Feld <strong>[!UICONTROL Card ID]</strong> die ID der Karte ein, zu der Sie einen Kommentar hinzufügen möchten, oder ordnen Sie sie zu.<br></p> </li> 
     <li> <p><strong>[!UICONTROL Select]</strong> </p> <p>Wählen Sie die Pinnwand aus, auf der sich der Kommentar befinden soll, wählen Sie die Karte aus, die die Karte enthält, und wählen Sie die Karte aus.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Kommentar] </td> 
   <td> <p>Geben Sie den Kommentar ein, den Sie der ausgewählten Karte hinzufügen möchten.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Kommentare in einer Karte auflisten]**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!UICONTROL Trello]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung mit [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Kartenkennung eingeben]</td> 
   <td> <p> Wählen Sie aus, wie Sie die Kennung der Karte eingeben möchten, auf der Sie einen Kommentar hinzufügen möchten.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL manuell eingeben]</strong> </p> <p>Geben Sie im Feld <strong>[!UICONTROL Card ID]</strong> die ID der Karte ein, zu der Sie einen Kommentar hinzufügen möchten, oder ordnen Sie sie zu.<br></p> </li> 
     <li> <p><strong>[!UICONTROL Select]</strong> </p> <p>Wählen Sie die Pinnwand aus, auf der sich der Kommentar befinden soll, wählen Sie die Karte aus, die die Karte enthält, und wählen Sie die Karte aus.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Maximale Anzahl zurückgegebener Kommentare]</td> 
   <td> <p> Geben Sie die maximale Anzahl von Kommentaren ein, die [!DNL Workfront Fusion] während eines Ausführungszyklus zurückgibt.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Seit] </td> 
   <td> <p>Legen Sie das Startdatum des Zeitraums fest, in dem der Kommentar erstellt wurde. Eine Liste der unterstützten Datums- und Uhrzeitformate finden Sie unter <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Typerzwingung in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Before] </td> 
   <td> <p>Legen Sie das Enddatum des Zeitraums fest, in dem der Kommentar erstellt wurde. Eine Liste der unterstützten Datums- und Uhrzeitformate finden Sie unter <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Typerzwingung in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## [!UICONTROL Trello] Objekt-IDs

* [So finden Sie die ID oder den Kurzlink einer Karte in [!DNL Trello]](#how-to-find-the-id-or-the-shortlink-of-a-card-in-trello)
* [Suchen von IDs anderer Objekte in  [!DNL Trello]](#how-to-find-ids-of-other-objects-in-trello)

### So finden Sie die ID oder den Kurzlink einer Karte in [!DNL Trello]

Wenn Sie eine Karte bearbeiten oder einen neuen Kommentar erstellen möchten, müssen Sie die Kennung der Karte oder deren Shortlink kennen. Sie können diese Informationen aus der Ausgabe des Triggers [!UICONTROL Neue Karte] abrufen. Der Kurzlink für eine Karte kann auch abgerufen werden, indem Sie die Karte öffnen und auf die Schaltfläche [!UICONTROL Freigeben] klicken. Der Shortlink befindet sich im Feld [!UICONTROL Link zu dieser Karte] am Ende der URL nach `https://trello.com/c/`.

![](assets/share-and-more-350x575.png)

### Suchen von IDs anderer Objekte in [!DNL Trello]

Pinnwand-, Listen- und Kommentar-IDs können nur mit Triggern abgerufen werden. Auf der [!DNL trello.com] -Website werden diese IDs nicht angezeigt.
