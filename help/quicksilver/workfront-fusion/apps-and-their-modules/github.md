---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: Connector
navigation-topic: apps-and-their-modules
title: GitHub-Module
description: In einem [!DNL Adobe Workfront Fusion] Szenario können Sie Workflows automatisieren, die GitHub verwenden, und sie mit mehreren Anwendungen und Diensten von Drittanbietern verbinden.
author: Becky
feature: Workfront Fusion
exl-id: 5e520aab-8307-4a52-96b6-13b284f9cb53
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '1839'
ht-degree: 0%

---

# [!DNL GitHub] Module

In einem [!DNL Adobe Workfront Fusion] -Szenario können Sie Workflows automatisieren, die [!UICONTROL GitHub] verwenden, und sie mit mehreren Anwendungen und Diensten von Drittanbietern verbinden.

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
   <p>Aktuelle Produktanforderung: Wenn Sie über den [!UICONTROL Select]- oder [!UICONTROL Prime] [!DNL Adobe Workfront]-Plan verfügen, muss Ihr Unternehmen [!DNL Adobe Workfront Fusion] sowie [!DNL Adobe Workfront] erwerben, um die in diesem Artikel beschriebenen Funktionen nutzen zu können. [!DNL Workfront Fusion] ist im [!UICONTROL Ultimate] [!DNL Workfront]-Plan enthalten.</p>
   <p>Oder</p>
   <p>Alte Produktanforderung: Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] sowie [!DNL Adobe Workfront] erwerben, um die in diesem Artikel beschriebenen Funktionen nutzen zu können.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Wenden Sie sich an Ihren [!DNL Workfront] -Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

Informationen zu [!DNL Adobe Workfront Fusion] -Lizenzen finden Sie unter [[!DNL Adobe Workfront Fusion] Lizenzen](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Voraussetzungen

Um [!DNL GitHub] -Module zu verwenden, müssen Sie über ein [!DNL GitHub] -Konto verfügen.

## [!DNL GitHub] mit [!DNL Workfront Fusion] verbinden

Anweisungen zum Verbinden Ihres [!DNL GitHub]-Kontos mit [!UICONTROL Workfront Fusion] finden Sie unter [Erstellen einer Verbindung mit [!UICONTROL Adobe Workfront Fusion] - Grundlegende Anweisungen](../../workfront-fusion/connections/connect-to-fusion-general.md)

## [!DNL GitHub] -Module und ihre Felder.

Wenn Sie [!DNL GitHub] -Module konfigurieren, zeigt [!DNL Workfront Fusion] die unten aufgeführten Felder an. Darüber hinaus können abhängig von Faktoren wie Ihrer Zugriffsebene in der App oder im Dienst zusätzliche [!DNL GitHub] -Felder angezeigt werden. Ein fett hervorgehobener Titel in einem Modul zeigt ein erforderliches Feld an.

Wenn Sie die Zuordnungsschaltfläche über einem Feld oder einer Funktion sehen, können Sie damit Variablen und Funktionen für dieses Feld festlegen. Weitere Informationen finden Sie unter [Informationen von einem Modul einem anderen zuordnen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Trigger](#triggers)
* [Aktionen](#actions)

### Trigger

* [[!UICONTROL Überwachungsprobleme]](#watch-issues)
* [[!UICONTROL Überwachen von Repositorys]](#watch-repositories)
* [[!UICONTROL Überwachungsspuren]](#watch-forks)
* [[!UICONTROL Kommentare ansehen]](#watch-comments)
* [[!UICONTROL Pull-Anforderungen überwachen]](#watch-pull-requests)

#### [!UICONTROL Überwachungsprobleme]

Dieses Modul wird Trigger, wenn ein neues Problem hinzugefügt oder ein vorhandenes Problem geändert wird.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL GitHub]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ich möchte sehen]</td> 
   <td>Wählen Sie aus, ob Sie alle Repositorys oder nur ein Repository überwachen möchten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Repository]</td> 
   <td>Wenn Sie sich dafür entschieden haben, Probleme nur in einem Repository zu beobachten, wählen Sie das Repository aus, das Sie beobachten möchten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Maximale Anzahl der zurückgegebenen Probleme]</td> 
   <td>Legen Sie die maximale Anzahl von Ergebnissen fest, mit denen [!DNL Workfront Fusion] während eines Zyklus arbeiten soll. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Watch]</td> 
   <td>Wählen Sie aus, ob Sie nur auf neue Probleme, neue Probleme und alle Änderungen achten möchten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filter]</td> 
   <td> <p>Sie können die Probleme, die Sie beobachten möchten, nach der Art ihrer Zuordnung filtern.</p> 
    <ul> 
     <li>[!UICONTROL Alle Probleme]</li> 
     <li>[!UICONTROL Nur Probleme, die mir zugewiesen sind]</li> 
     <li>[!UICONTROL Nur von mir erstellte Probleme]</li> 
     <li>[!UICONTROL Nur Probleme, die mich erwähnen]</li> 
     <li>[!UICONTROL Nur Probleme, für die ich Updates abonniert habe]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL State]</td> 
   <td>Wählen Sie aus, ob Sie nur offene Probleme oder nur geschlossene Probleme sehen möchten. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Beschriftungen]</td> 
   <td>Fügen Sie ein Tag hinzu. Das Modul überwacht Probleme mit diesem Tag.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Überwachen von Repositorys]

Dieses Modul wird bei der Erstellung oder Änderung eines Repositorys Trigger.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL GitHub]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Maximale Anzahl an zurückgegebenen Repositorys]</td> 
   <td>Legen Sie die maximale Anzahl von Ergebnissen fest, mit denen [!DNL Workfront Fusion] während eines Zyklus arbeiten soll. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Watch]</td> 
   <td>Wählen Sie aus, ob Sie nach neuen Repositorys und allen Änderungen oder nur neuen Repositorys suchen möchten.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Überwachungsspuren]

Dieses Modul wird bei der Erstellung einer neuen Abspaltung Trigger.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL GitHub]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Repository]</td> 
   <td>Wählen Sie das Repository aus, das Sie auf Verzweigungen überwachen möchten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Maximale Anzahl der zurückgegebenen Gabeln]</td> 
   <td>Legen Sie die maximale Anzahl von Ergebnissen fest, mit denen [!DNL Workfront Fusion] während eines Zyklus arbeiten soll. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Kommentare ansehen]

Dieses Modul wird Trigger, wenn ein neuer Kommentar hinzugefügt oder ein bestehender Kommentar geändert wird.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL GitHub]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Repository]</td> 
   <td>Wählen Sie das Repository aus, das Sie ansehen möchten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Problemnummer]</td> 
   <td>Wenn Sie die Suche einschränken möchten, indem Sie nur nach neuen Kommentaren zu einem bestimmten Thema suchen, geben Sie die Problemnummer ein.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Maximale Anzahl der zurückgegebenen Probleme]</td> 
   <td>Legen Sie die maximale Anzahl von Ergebnissen fest, mit denen [!DNL Workfront Fusion] während eines Zyklus arbeiten soll. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Watch]</td> 
   <td>Wählen Sie aus, ob Sie nur nach neuen Kommentaren, Kommentaren und allen Änderungen suchen möchten.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Pull-Anforderungen überwachen]

Dieses Modul wird Trigger, wenn eine neue Pull-Anforderung hinzugefügt oder eine vorhandene Pull-Anforderung geändert wird.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL GitHub]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Repository]</td> 
   <td>Wählen Sie das Repository aus, das Sie ansehen möchten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Maximale Anzahl der zurückgegebenen Pull-Anforderungen]</td> 
   <td>Legen Sie die maximale Anzahl von Ergebnissen fest, mit denen [!DNL Workfront Fusion] während eines Zyklus arbeiten soll. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL State]</td> 
   <td>Wählen Sie aus, ob Sie [!UICONTROL nur geöffnete Pull]-Anforderungen, [!UICONTROL nur geschlossene Anforderungen] oder alle Pull-Anforderungen überwachen möchten. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Watch]</td> 
   <td>Wählen Sie aus, ob Sie nur auf neue Pull-Anforderungen oder neue Pull-Anforderungen und alle Änderungen achten möchten.</td> 
  </tr> 
 </tbody> 
</table>

### Aktionen

* [[!UICONTROL Suchen nach einem Problem]](#search-for-an-issue)
* [[!UICONTROL Erstellen eines Problems]](#create-an-issue)
* [[!UICONTROL Aktualisieren eines Problems]](#update-an-issue)
* [[!UICONTROL Problem abrufen]](#get-an-issue)
* [[!UICONTROL Hinzufügen von Bevollmächtigten]](#add-assignees)
* [[!UICONTROL Bevollmächtigte entfernen]](#remove-assignees)
* [[!UICONTROL Hinzufügen von Bezeichnungen zu einem Problem]](#add-labels-to-an-issue)
* [[!UICONTROL Entfernen einer Bezeichnung aus einem Problem]](#remove-a-label-from-an-issue)
* [[!UICONTROL Erstellen eines Kommentars]](#create-a-comment)
* [[!UICONTROL Kommentare auflisten]](#list-comments)

#### [!UICONTROL Suchen nach einem Problem]

Dieses Modul sucht nach Problemen, die Ihren Suchkriterien entsprechen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL GitHub]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Maximale Anzahl der zurückgegebenen Probleme]</td> 
   <td>Legen Sie die maximale Anzahl von Ergebnissen fest, mit denen [!DNL Workfront Fusion] während eines Zyklus arbeitet (die Anzahl der Wiederholungen pro Szenario-Ausführung). </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Sortieren nach</td> 
   <td> <p>Wählen Sie aus, wie die Suchergebnisse sortiert werden sollen.</p> 
    <ul> 
     <li> <p>[!UICONTROL Best Match] </p> </li> 
     <li>[!UICONTROL Datum]</li> 
     <li>[!UICONTROL Datum aktualisiert]</li> 
     <li>[!UICONTROL Anzahl Kommentare]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sortierrichtung]</td> 
   <td> <p>Wählen Sie auf- oder absteigend aus. </p> <p>Für Datumsangaben wird bei Auswahl von <strong>[!UICONTROL Absteigend]</strong> zunächst das neueste Datum zurückgegeben. </p> <p>Bei [!UICONTROL Anzahl Kommentare] wird durch die Auswahl von <strong>[!UICONTROL Absteigend]</strong> das Problem mit der höchsten Anzahl von Kommentaren zuerst zurückgegeben.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Abfrage]</td> 
   <td>Geben Sie Ihre Suchabfrage ein oder ordnen Sie sie zu. Eine detaillierte Beschreibung der Suchoptionen finden Sie unter <a href="https://docs.github.com/en/github/searching-for-information-on-github/searching-issues-and-pull-requests">Suchprobleme und Pull-Anforderungen</a> auf der Hilfeseite [!DNL GitHub].</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Erstellen eines Problems]

Dieses Modul erstellt ein neues Problem im ausgewählten Repository.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL GitHub]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Repository]</td> 
   <td>Wählen Sie das Repository aus, in dem Sie ein Problem erstellen möchten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Zuweisung]</td> 
   <td>Wählen Sie die Personen aus, die Sie dem Problem zuweisen möchten. Verfügbare Zuweisungsberechtigungen umfassen alle Personen mit Schreibberechtigungen für das Repository und Organisationsmitglieder mit Leserechten für das Repository. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Milestone]</td> 
   <td>Wählen Sie den Meilenstein aus, den Sie mit dem neuen Problem verbinden möchten. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Beschriftungen]</td> 
   <td>Wählen Sie alle Bezeichnungen aus, die Sie auf die neue Ausgabe anwenden möchten. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Titel]</td> 
   <td>Geben Sie einen Titel für das neue Problem ein oder ordnen Sie ihn zu.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td>Geben Sie den Hauptteil des Problems ein oder ordnen Sie ihn zu, z. B. eine Beschreibung oder zusätzliche Informationen</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Aktualisieren eines Problems]

Dieses Modul aktualisiert ein vorhandenes [!DNL GitHub] -Problem.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL GitHub]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Repository]</td> 
   <td>Wählen Sie das Repository aus, in dem Sie ein Problem aktualisieren möchten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Zuweisung]</td> 
   <td>Wählen Sie die Personen aus, die Sie dem Problem zuweisen möchten. Verfügbare Zuweisungsberechtigungen beinhalten alle Personen mit Schreibberechtigungen für das Repository und die Mitglieder der Organisation mit Leserechten für das Repository. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Milestone]</td> 
   <td>Wählen Sie den Meilenstein aus, den Sie mit dem Problem verbinden möchten. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Beschriftungen]</td> 
   <td>Wählen Sie alle Bezeichnungen aus, die Sie auf das Problem anwenden möchten. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Number]</td> 
   <td>Geben Sie die Problemnummer des Problems ein, das Sie aktualisieren möchten, oder ordnen Sie sie zu. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL State]</td> 
   <td>Wählen Sie den Status aus, auf den Sie das Problem aktualisieren möchten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Titel]</td> 
   <td>Geben Sie einen Titel für das Problem ein oder ordnen Sie ihn zu.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td>Geben Sie den Hauptteil des Problems ein oder ordnen Sie ihn zu, z. B. eine Beschreibung oder zusätzliche Informationen</td> 
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
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL GitHub]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Repository]</td> 
   <td>Wählen Sie das Repository aus, das das Problem enthält, zu dem Sie Details abrufen möchten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Number]</td> 
   <td>Geben Sie die Problemnummer des Problems ein oder ordnen Sie sie zu, zu dem Sie Details abrufen möchten. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Hinzufügen von Bevollmächtigten]

Dieses Modul fügt dem angegebenen Problem Bevollmächtigte hinzu

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL GitHub]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Repository]</td> 
   <td>Wählen Sie das Repository aus, das das Problem enthält, dem Sie Bevollmächtigte hinzufügen möchten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Zuweisung]</td> 
   <td>Wählen Sie die Personen aus, die Sie dem Problem zuweisen möchten. Verfügbare Zuweisungsberechtigungen beinhalten alle Personen mit Schreibberechtigungen für das Repository und die Mitglieder der Organisation mit Leserechten für das Repository. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Number]</td> 
   <td>Geben Sie die Problemnummer des Problems ein oder ordnen Sie sie zu, dem Sie Bevollmächtigte hinzufügen möchten. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Bevollmächtigte entfernen]

Dieses Modul entfernt Bevollmächtigte aus dem angegebenen Problem.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL GitHub]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Repository]</td> 
   <td>Wählen Sie das Repository aus, das das Problem enthält, aus dem Sie Bevollmächtigte entfernen möchten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Zuweisung]</td> 
   <td>Wählen Sie die Personen aus, die Sie aus dem Problem entfernen möchten. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Number]</td> 
   <td>Geben Sie die Problemnummer des Problems ein oder ordnen Sie sie zu, aus dem Sie Bevollmächtigte entfernen möchten. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Hinzufügen von Bezeichnungen zu einem Problem]

Dieses Modul fügt einem Problem Beschriftungen hinzu. Beschriftungen werden auf Repository-Ebene definiert und können nur von einer Person mit Schreibzugriff auf das Repository erstellt werden.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL GitHub]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Repository]</td> 
   <td>Wählen Sie das Repository aus, das das Problem enthält, dem Sie Beschriftungen hinzufügen möchten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Beschriftungen]</td> 
   <td>Wählen Sie die Titel aus, die Sie dem Problem hinzufügen möchten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Number]</td> 
   <td>Geben Sie die Problemnummer des Problems ein oder ordnen Sie sie zu, dem Sie Beschriftungen hinzufügen möchten.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Entfernen einer Bezeichnung aus einem Problem]

Dieses Modul entfernt eine einzelne Bezeichnung aus einem Problem.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL GitHub]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Repository]</td> 
   <td>Wählen Sie das Repository aus, das das Problem enthält, aus dem Sie eine Beschriftung entfernen möchten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Beschriftungen]</td> 
   <td>Wählen Sie den Titel aus, den Sie aus dem Problem entfernen möchten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Number]</td> 
   <td>Geben Sie die Problemnummer des Problems ein oder ordnen Sie sie zu, aus dem Sie einen Titel entfernen möchten.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Erstellen eines Kommentars]

Dieses Modul erstellt einen Kommentar zum angegebenen Problem.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL GitHub]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Repository]</td> 
   <td>Wählen Sie das Repository aus, das das Problem enthält, für das Sie einen Kommentar erstellen möchten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Number]</td> 
   <td>Geben Sie die Problemnummer des Problems ein oder ordnen Sie sie zu, für das Sie einen Kommentar erstellen möchten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td>Geben Sie den Inhalt des Kommentars ein oder ordnen Sie ihn zu.</td> 
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
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL GitHub]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Repository]</td> 
   <td>Wählen Sie das Repository aus, das das Problem enthält, aus dem Sie Kommentare auflisten möchten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Number]</td> 
   <td>Geben Sie die Problemnummer des Problems ein oder ordnen Sie sie zu, in dem Sie Kommentare auflisten möchten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Seit]</td> 
   <td>Das Modul gibt nach diesem Datum erstellte Kommentare zurück. Eine Liste der unterstützten Datumsformate finden Sie unter <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Typerzwingung in [!DNL Adobe Workfront Fusion]</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Maximale Anzahl zurückgegebener Kommentare]</td> 
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
