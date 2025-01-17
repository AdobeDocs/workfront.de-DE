---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: Steckverbinder
navigation-topic: apps-and-their-modules
title: GitHub-Module
description: Die Dokumentation zu Adobe Workfront Fusion wurde an einen neuen Speicherort verschoben. Dieser Artikel ist veraltet, enthält jedoch einen Link zum neuen Artikel, der diese Funktion behandelt.
author: Becky
feature: Workfront Fusion
exl-id: 5e520aab-8307-4a52-96b6-13b284f9cb53
source-git-commit: efbe888d370e20c895dc40f18f999f2d01ec6337
workflow-type: tm+mt
source-wordcount: '1891'
ht-degree: 0%

---

# [!DNL GitHub]

>[!IMPORTANT]
>
>Die Dokumentation zu Adobe Workfront Fusion wurde an einen neuen Speicherort verschoben.
>
>Die Informationen in diesem Artikel finden Sie jetzt im Artikel:
>
>* [GitHub-Module](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/github.html)
>
>Bitte aktualisieren Sie alle Lesezeichen.
>
>Dieser Artikel wird nicht mehr aktualisiert und in naher Zukunft entfernt.

In einem [!DNL Adobe Workfront Fusion] Szenario können Sie Workflows automatisieren, die [!UICONTROL GitHub] verwenden, und sie mit mehreren Anwendungen und Services von Drittanbietern verbinden.

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Funktion in diesem Artikel verwenden zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Plan*</td>
  <td> <p>[!UICONTROL Pro] oder höher</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] Lizenz*</td>
   <td> <p>[!UICONTROL-Plan], [!UICONTROL-Arbeit]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] Lizenz **</td> 
   <td>
   <p>Aktuelle Lizenzanforderung: Keine [!DNL Workfront Fusion].</p>
   <p>Oder</p>
   <p>Legacy-Lizenzanforderung: [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>
   <p>Aktuelle Produktanforderung: Wenn Sie über den [!DNL Adobe Workfront] [!UICONTROL Select] oder [!UICONTROL Prime] verfügen, muss Ihr Unternehmen [!DNL Adobe Workfront Fusion] erwerben und [!DNL Adobe Workfront], die in diesem Artikel beschriebenen Funktionen zu nutzen. [!DNL Workfront Fusion] ist im [!DNL Workfront] [!UICONTROL Ultimate] enthalten.</p>
   <p>Oder</p>
   <p>Legacy-Produktanforderung: Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] erwerben und [!DNL Adobe Workfront], die in diesem Artikel beschriebenen Funktionen zu verwenden.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Wenden Sie sich an Ihren [!DNL Workfront], um herauszufinden, über welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie verfügen.

Informationen zu [!DNL Adobe Workfront Fusion] finden Sie unter [[!DNL Adobe Workfront Fusion] Lizenzen](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Voraussetzungen

Um [!DNL GitHub] Module verwenden zu können, müssen Sie über ein [!DNL GitHub] Konto verfügen.

## [!DNL GitHub] mit [!DNL Workfront Fusion] verbinden

Anweisungen zum Verbinden Ihres [!DNL GitHub]-Kontos mit [!UICONTROL Workfront Fusion] finden Sie unter [Erstellen einer Verbindung mit [!UICONTROL Adobe Workfront Fusion] - Grundlegende Anweisungen](../../workfront-fusion/connections/connect-to-fusion-general.md)

## [!DNL GitHub] Module und ihre Felder.

Beim Konfigurieren [!DNL GitHub] Module zeigt [!DNL Workfront Fusion] die unten aufgeführten Felder an. Darüber hinaus können abhängig von Faktoren wie Ihrer Zugriffsebene in der App oder dem Service weitere [!DNL GitHub] angezeigt werden. Ein fett gedruckter Titel in einem Modul gibt ein erforderliches Feld an.

Wenn die Zuordnungsschaltfläche über einem Feld oder einer Funktion angezeigt wird, können Sie damit Variablen und Funktionen für dieses Feld festlegen. Weitere Informationen finden Sie unter [Zuordnen von Informationen zu einem anderen Modul in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Trigger](#triggers)
* [Aktionen](#actions)

### Trigger

* [[!UICONTROL Probleme ansehen]](#watch-issues)
* [[!UICONTROL Überwachen von Repositorys]](#watch-repositories)
* [[!UICONTROL Gabeln ansehen]](#watch-forks)
* [[!UICONTROL Kommentare ansehen]](#watch-comments)
* [[!UICONTROL Pull-Anforderungen beobachten]](#watch-pull-requests)

#### [!UICONTROL Probleme ansehen]

Dieses Modul wird Trigger, wenn ein neues Problem hinzugefügt oder ein vorhandenes Problem geändert wird.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL GitHub]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL, die ich beobachten möchte]</td> 
   <td>Wählen Sie aus, ob alle Repositorys oder nur ein Repository überwacht werden sollen.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Repository]</td> 
   <td>Wenn Sie ausgewählt haben, dass Probleme nur in einem Repository überwacht werden sollen, wählen Sie das Repository aus, das überwacht werden soll.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Maximale Anzahl der zurückgegebenen Probleme]</td> 
   <td>Legen Sie die maximale Anzahl von Ergebnissen fest, mit denen [!DNL Workfront Fusion] während eines Zyklus arbeiten soll. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Uhr]</td> 
   <td>Wählen Sie aus, ob nur auf neue Probleme oder auf neue Probleme und alle Änderungen geachtet werden soll.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL filter]</td> 
   <td> <p>Sie können die Probleme, die Sie im Auge behalten möchten, nach ihrer Zuordnung filtern.</p> 
    <ul> 
     <li>[!UICONTROL Alle Probleme]</li> 
     <li>[!UICONTROL Nur mir zugewiesene Anfragen]</li> 
     <li>[!Nur von mir erstellte UICONTROL-Anfragen]</li> 
     <li>[!UICONTROL nur Probleme, die mich erwähnen]</li> 
     <li>[!UICONTROL Nur Probleme, für die ich Aktualisierungen abonniert habe]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Status]</td> 
   <td>Wählen Sie aus, ob nur offene oder nur geschlossene Anfragen angezeigt werden sollen. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Kennzeichnungen]</td> 
   <td>Fügen Sie ein Tag hinzu. Das Modul überwacht Probleme mit diesem Tag.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Überwachen von Repositorys]

Trigger Dieses Modul tritt beim Erstellen oder Ändern eines Repositorys nicht mehr auf.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL GitHub]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Maximale Anzahl der zurückgegebenen Repositorys]</td> 
   <td>Legen Sie die maximale Anzahl von Ergebnissen fest, mit denen [!DNL Workfront Fusion] während eines Zyklus arbeiten soll. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Uhr]</td> 
   <td>Wählen Sie aus, ob Sie auf neue Repositorys und alle Änderungen oder nur auf neue Repositorys achten möchten.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Gabeln ansehen]

Dieses Modul wird beim Erstellen einer neuen Verzweigung Trigger.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL GitHub]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Repository]</td> 
   <td>Wählen Sie das Repository aus, auf das Sie Formulare überwachen möchten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Maximale Anzahl der zurückgegebenen Formulare]</td> 
   <td>Legen Sie die maximale Anzahl von Ergebnissen fest, mit denen [!DNL Workfront Fusion] während eines Zyklus arbeiten soll. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Kommentare ansehen]

Dieses Modul wird Trigger, wenn ein neuer Kommentar hinzugefügt oder ein vorhandener Kommentar geändert wird.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL GitHub]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Repository]</td> 
   <td>Wählen Sie das Repository aus, das Sie überwachen möchten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Anfragenummer]</td> 
   <td>Wenn Sie die Suche einschränken möchten, indem Sie nur nach neuen Kommentaren zu einem bestimmten Problem suchen, geben Sie die Problemnummer ein.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Maximale Anzahl der zurückgegebenen Probleme]</td> 
   <td>Legen Sie die maximale Anzahl von Ergebnissen fest, mit denen [!DNL Workfront Fusion] während eines Zyklus arbeiten soll. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Uhr]</td> 
   <td>Wählen Sie aus, ob nur nach neuen Kommentaren oder Kommentaren und allen Änderungen gesucht werden soll.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Pull-Anforderungen beobachten]

Dieses Modul wird Trigger, wenn eine neue Pull-Anforderung hinzugefügt oder eine vorhandene Pull-Anforderung geändert wird.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL GitHub]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Repository]</td> 
   <td>Wählen Sie das Repository aus, das Sie überwachen möchten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Maximale Anzahl der zurückgegebenen Pull-Anforderungen]</td> 
   <td>Legen Sie die maximale Anzahl von Ergebnissen fest, mit denen [!DNL Workfront Fusion] während eines Zyklus arbeiten soll. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Status]</td> 
   <td>Wählen Sie aus, ob Sie [!UICONTROL only open pull]-Anfragen, [!UICONTROL only closed ones] oder alle Pull-Anfragen beobachten möchten. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Uhr]</td> 
   <td>Wählen Sie aus, ob Sie nur auf neue Pull-Anforderungen oder neue Pull-Anforderungen und alle Änderungen achten möchten.</td> 
  </tr> 
 </tbody> 
</table>

### Aktionen

* [[!UICONTROL Nach einem Problem suchen]](#search-for-an-issue)
* [[!UICONTROL Anfrage erstellen]](#create-an-issue)
* [[!UICONTROL Problem aktualisieren]](#update-an-issue)
* [[!UICONTROL Problem abrufen]](#get-an-issue)
* [[!UICONTROL Empfänger hinzufügen]](#add-assignees)
* [[!UICONTROL Bevollmächtigte entfernen]](#remove-assignees)
* [[!UICONTROL Kennzeichnungen zu einem Problem hinzufügen]](#add-labels-to-an-issue)
* [[!UICONTROL Entfernen einer Kennzeichnung aus einem Problem]](#remove-a-label-from-an-issue)
* [[!UICONTROL Kommentar erstellen]](#create-a-comment)
* [[!UICONTROL Kommentare auflisten]](#list-comments)

#### [!UICONTROL Nach einem Problem suchen]

Dieses Modul sucht nach Problemen, die Ihren Suchkriterien entsprechen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL GitHub]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Maximale Anzahl der zurückgegebenen Probleme]</td> 
   <td>Legen Sie die maximale Anzahl von Ergebnissen fest, mit denen [!DNL Workfront Fusion] während eines Zyklus arbeiten soll (die Anzahl der Wiederholungen pro Szenario-Ausführung). </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sortieren nach]</td> 
   <td> <p>Wählen Sie aus, wie die Suchergebnisse sortiert werden sollen.</p> 
    <ul> 
     <li> <p>[!UICONTROL Beste Übereinstimmung] </p> </li> 
     <li>[!UICONTROL Datum erstellt]</li> 
     <li>[!UICONTROL Datum aktualisiert]</li> 
     <li>[!UICONTROL Anzahl Kommentare]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sortierrichtung]</td> 
   <td> <p>Aufsteigend oder absteigend auswählen. </p> <p>Bei Datumsangaben wird bei Auswahl von <strong>[!UICONTROL absteigend]</strong> zuerst das neueste Datum zurückgegeben. </p> <p>Wenn Sie für [!UICONTROL Anzahl der Kommentare] <strong>[!UICONTROL absteigend]</strong> auswählen, wird das Problem mit der höchsten Anzahl von Kommentaren zuerst zurückgegeben.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Abfrage]</td> 
   <td>Geben Sie Ihre Suchanfrage ein oder ordnen Sie sie zu. Eine ausführliche Beschreibung der Suchoptionen finden Sie unter <a href="https://docs.github.com/en/github/searching-for-information-on-github/searching-issues-and-pull-requests">Suchen von Problemen und Pull-</a> auf der [!DNL GitHub]-Hilfeseite.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Anfrage erstellen]

Dieses Modul erstellt ein neues Problem im ausgewählten Repository.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL GitHub]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Repository]</td> 
   <td>Wählen Sie das Repository aus, in dem Sie ein Problem erstellen möchten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Bevollmächtigter]</td> 
   <td>Wählen Sie die Personen aus, die Sie dem Problem zuweisen möchten. Zu den verfügbaren Bevollmächtigten gehören alle Personen mit Schreibberechtigungen für das Repository sowie Organisationsmitglieder mit Leseberechtigungen für das Repository. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Milestone]</td> 
   <td>Wählen Sie den Meilenstein aus, den Sie mit dem neuen Problem verknüpfen möchten. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Kennzeichnungen]</td> 
   <td>Wählen Sie alle Kennzeichnungen aus, die Sie auf das neue Problem anwenden möchten. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Titel]</td> 
   <td>Geben Sie einen Titel für die neue Anfrage ein oder ordnen Sie ihn zu.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL body]</td> 
   <td>Geben Sie den Hauptteil des Problems ein, z. B. eine Beschreibung oder zusätzliche Informationen, oder ordnen Sie ihn zu</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Problem aktualisieren]

Dieses Modul aktualisiert ein vorhandenes [!DNL GitHub].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL GitHub]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Repository]</td> 
   <td>Wählen Sie das Repository aus, in dem Sie ein Problem aktualisieren möchten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Bevollmächtigter]</td> 
   <td>Wählen Sie die Personen aus, die Sie dem Problem zuweisen möchten. Zu den verfügbaren Bevollmächtigten gehören alle mit Schreibberechtigungen für das Repository sowie Organisationsmitglieder mit Leseberechtigungen für das Repository. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Milestone]</td> 
   <td>Wählen Sie den Meilenstein aus, den Sie mit dem Problem verknüpfen möchten. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Kennzeichnungen]</td> 
   <td>Wählen Sie alle Kennzeichnungen aus, die Sie auf das Problem anwenden möchten. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Nummer]</td> 
   <td>Geben Sie die Anfragenummer des Problems ein, das Sie aktualisieren möchten, oder mappen Sie sie. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Status]</td> 
   <td>Wählen Sie den Status aus, auf den Sie das Problem aktualisieren möchten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Titel]</td> 
   <td>Geben Sie einen Titel für das Problem ein oder ordnen Sie ihn zu.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL body]</td> 
   <td>Geben Sie den Hauptteil des Problems ein, z. B. eine Beschreibung oder zusätzliche Informationen, oder ordnen Sie ihn zu</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Problem abrufen]

Dieses Modul ruft Details zum angegebenen Problem ab

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL GitHub]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Repository]</td> 
   <td>Wählen Sie das Repository aus, das das Problem enthält, zu dem Sie Details abrufen möchten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Nummer]</td> 
   <td>Geben Sie die Anfragenummer des Problems ein, zu dem Sie Details abrufen möchten, oder ordnen Sie sie zu. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Empfänger hinzufügen]

Dieses Modul fügt dem angegebenen Problem Verantwortliche hinzu

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL GitHub]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Repository]</td> 
   <td>Wählen Sie das Repository aus, das das Problem enthält, dem Sie Verantwortliche hinzufügen möchten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Bevollmächtigter]</td> 
   <td>Wählen Sie die Personen aus, die Sie dem Problem zuweisen möchten. Zu den verfügbaren Bevollmächtigten gehören alle mit Schreibberechtigungen für das Repository sowie Organisationsmitglieder mit Leseberechtigungen für das Repository. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Nummer]</td> 
   <td>Geben Sie die Problemnummer des Problems ein, dem Sie Bevollmächtigte hinzufügen möchten, oder ordnen Sie sie zu. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Bevollmächtigte entfernen]

Dieses Modul entfernt Verantwortliche aus dem angegebenen Problem.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL GitHub]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Repository]</td> 
   <td>Wählen Sie das Repository aus, das das Problem enthält, aus dem Sie die Zugewiesenen entfernen möchten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Bevollmächtigter]</td> 
   <td>Wählen Sie die Personen aus, die Sie aus dem Problem entfernen möchten. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Nummer]</td> 
   <td>Geben Sie die Problemnummer des Problems ein, aus dem Sie Zugewiesene entfernen möchten, oder ordnen Sie sie zu. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Kennzeichnungen zu einem Problem hinzufügen]

Dieses Modul fügt einem Problem Kennzeichnungen hinzu. Kennzeichnungen werden auf Repository-Ebene definiert und können nur von einer Person mit Schreibzugriff auf das Repository erstellt werden.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL GitHub]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Repository]</td> 
   <td>Wählen Sie das Repository aus, das das Problem enthält, dem Sie Kennzeichnungen hinzufügen möchten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Kennzeichnungen]</td> 
   <td>Wählen Sie die Kennzeichnungen aus, die Sie dem Problem hinzufügen möchten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Nummer]</td> 
   <td>Geben Sie die Problemnummer des Problems ein, dem Sie Kennzeichnungen hinzufügen möchten, oder ordnen Sie sie zu.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Entfernen einer Kennzeichnung aus einem Problem]

Dieses Modul entfernt eine einzelne Kennzeichnung aus einem Problem.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL GitHub]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Repository]</td> 
   <td>Wählen Sie das Repository aus, das das Problem enthält, aus dem Sie eine Kennzeichnung entfernen möchten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Kennzeichnungen]</td> 
   <td>Wählen Sie die Bezeichnung aus, die Sie aus dem Problem entfernen möchten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Nummer]</td> 
   <td>Geben Sie die Problemnummer des Problems ein, von dem Sie einen Titel entfernen möchten, oder ordnen Sie sie zu.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Kommentar erstellen]

Dieses Modul erstellt einen Kommentar zum angegebenen Problem.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL GitHub]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Repository]</td> 
   <td>Wählen Sie das Repository aus, das das Problem enthält, zu dem Sie einen Kommentar erstellen möchten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Nummer]</td> 
   <td>Geben Sie die Problemnummer des Problems ein, zu dem Sie einen Kommentar erstellen möchten, oder ordnen Sie sie zu.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL body]</td> 
   <td>Geben Sie den Inhalt des Kommentars ein oder mappen Sie ihn.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Kommentare auflisten]

Dieses Modul listet alle Kommentare zum angegebenen Problem auf.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL GitHub]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Repository]</td> 
   <td>Wählen Sie das Repository aus, das das Problem enthält, aus dem Sie Kommentare auflisten möchten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Nummer]</td> 
   <td>Geben Sie die Problemnummer des Problems ein, zu dem Sie Kommentare auflisten möchten, oder ordnen Sie sie zu.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL seit]</td> 
   <td>Das Modul gibt die Kommentare zurück, die nach diesem Datum erstellt wurden. Eine Liste der unterstützten Datumsformate finden Sie unter "<a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref"> in [!DNL Adobe Workfront Fusion]</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Maximale Anzahl der zurückgegebenen Kommentare]</td> 
   <td>Legen Sie die maximale Anzahl von Ergebnissen fest, mit denen [!DNL Workfront Fusion] während eines Zyklus arbeiten soll. </td> 
  </tr> 
 </tbody> 
</table>

<!--
<h2 data-mc-conditions="QuicksilverOrClassic.Draft mode">Troubleshooting</h2>
-->

<!--
<h3 data-mc-conditions="QuicksilverOrClassic.Draft mode">Module does not receive any events</h3>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">If a module does not receive any events, check the webhook settings in Github and make sure that:</p>
-->

<!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You have set the correct type of event that the chosen module should receive</p>
  -->

<!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You have entered the correct Payload URL</p>
  -->
