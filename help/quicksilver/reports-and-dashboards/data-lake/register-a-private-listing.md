---
content-type: reference
product-area: reports and dashboards
navigation-topic: data connect
title: Registrieren eines privaten Listeneintrags für Workfront Data Connect
description: Registrieren Sie einen privaten Snowflake-Eintrag, um Ihre Workfront Data Connect-Daten direkt mit dem Snowflake-Konto Ihres Unternehmens zu teilen.
author: Courtney
feature: Reports and Dashboards
exl-id:
last-update: 2026-09-15T00:00:00.000Z
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
    internal-label: Reporting
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: ed31fce397f9e99e7049d4f55eaca94f43dfcf5c
workflow-type: tm+mt
source-wordcount: '1060'
ht-degree: 3%
---
# Registrieren eines privaten Listeneintrags für Workfront Data Connect

Sie können Ihre Workfront Data Connect-Daten direkt mit dem Snowflake-Konto Ihres Unternehmens teilen, indem Sie einen privaten Eintrag registrieren. Diese Verbindungsmethode verwendet die Funktion der privaten Auflistung von Snowflake, um Daten sicher zwischen Organisationen auszutauschen, ohne sie öffentlich zugänglich zu machen, und funktioniert über Regionen und Hosting-Plattformen hinweg.

Ein privater Eintrag ist nützlich, wenn Sie Ihre Workfront-Daten mit anderen Daten in Ihrem Unternehmens-Data Warehouse verbinden möchten. Da die Daten in Ihrem eigenen Snowflake-Konto landen, können Sie sie zusammen mit den anderen Daten abfragen.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Paket</td> 
   <td><p>Ultimate</p>
    <p>Workflow Ultimate</p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td>
   <p>Standard</p>
   <p>Abo</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Sie müssen ein Workfront-Administrator sein</p></td> 
  </tr> 
 </tbody> 
</table>

Weitere Details zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

Sie benötigen außerdem ein Snowflake-Konto mit Berechtigungen zum Akzeptieren von Auflistungen und Erstellen von Datenbanken sowie eine Berechtigung für Workfront Data Connect.

## Was eine private Börsennotierung angibt

Ein privater Eintrag bietet Ihnen Zugriff auf:

* Über 100 Datenansichten für Workfront-Objekte. Beschreibungen der einzelnen Ansichten finden Sie unter [Datenwörterbuch für Workfront Data Connect](/help/quicksilver/reports-and-dashboards/data-lake/data-dictionary.md).
* Die `*_event` Datenansichten, die jede an die Data Connect-Datenpipelines gesendete Änderungstransaktion enthalten.
* Benutzerdefinierte Datenwerte für datenerweiterbare Objekte. Ein Beispiel finden Sie im Beispiel für eine benutzerdefinierte Datenabfrage unter [Workfront Data Connect-Abfragebeispiele](/help/quicksilver/reports-and-dashboards/data-lake/basic-query-examples.md).

## Unterschiede zu einer Leserkontenverbindung

Bei einem privaten Eintrag wird ein anderer Satz von Ansichten verwendet als bei einer Leserkontoverbindung, und die Daten werden nach einem anderen Zeitplan empfangen. Beachten Sie die folgenden Unterschiede:

* Eine private Liste gibt nur die `*_event` Ansichten frei. Die `*_current`- und `*_daily_history` sind über ein Leserkonto verfügbar, jedoch nicht über einen privaten Eintrag. Sie können sie in Ihrem eigenen Snowflake-Konto erstellen. Weitere Informationen finden Sie unter [Einrichten der aktuellen und täglichen Verlaufsansichten](#set-up-current-and-daily-history-views) in diesem Artikel.
* Ein privater Eintrag enthält möglicherweise nicht alle Ansichten, die über ein Leserkonto verfügbar sind. Beispiele für nicht freigegebene Ansichten sind Workfront Planning-Objekte, `MONITORING_DATA_REFRESHES`, `BOOKINGS` und `CLASSIFIER`. Diese Liste ist nicht vollständig.
* Data Connect lädt alle 4 Stunden Änderungsereignisse. Da für eine private Auflistung ein zusätzlicher Replikationsschritt erforderlich ist, um die Daten anzuzeigen, dauert das Eintreffen der Daten etwa eine Stunde länger als bei einem Leserkonto.
* Die Datenreplikation wird um 13:01 Uhr, 05:01 Uhr, 09:01 Uhr, 13:01 Uhr, 17:01 Uhr und 21:01 Uhr UTC durchgeführt. Die Daten sind in der Regel innerhalb von etwa 10 Minuten nach jedem Durchlauf verfügbar.
* Die `MONITORING_DATA_REFRESHES`- und `JOB_HISTORY` spiegeln nicht die Zeitpunkte wider, zu denen Daten über einen privaten Eintrag verfügbar werden. Obwohl die `JOB_HISTORY` Ansicht über den privaten Eintrag freigegeben ist, empfehlen wir, sie über ein Leserkonto zu lesen, um fehlgeschlagene Aufträge schneller zu identifizieren.

## Registrieren eines privaten Listeneintrags

Um einen privaten Eintrag zu registrieren, erfassen Sie zunächst Ihre Snowflake-Kontodetails und fügen Sie dann den Eintrag in Workfront hinzu.

### Erfassen von Snowflake-Kontodetails

Workfront verwendet Ihre Snowflake-Kontodetails, um den Eintrag auf Ihr Konto auszurichten. Sammeln Sie die folgenden Details:

* Kontostandort
* Konto-URL
* Kontoorganisation
* Kontoname

Jeder dieser Werte ist über das Modal „Kontodetails“ in Snowflake verfügbar.

So finden Sie Ihre Kontodetails:

1. Klicken Sie, während Sie bei Ihrem Snowflake-Konto angemeldet sind, auf das Benutzermenü unten links.

1. Wählen Sie Ihr Konto im Bereich **Konto** des Menüs aus.

1. Klicken Sie **Kontodetails anzeigen** für das Konto.

1. Notieren Sie sich jeden der oben aufgeführten Werte.

Legen Sie außerdem den Namen der Datenbank fest, über die Sie auf Ihre verknüpften Workfront-Daten zugreifen möchten. Diesen Namen geben Sie bei der Registrierung des Listeneintrags ein.

### Privaten Eintrag in Workfront hinzufügen

Sie registrieren den privaten Eintrag über die Adobe Workfront-Oberfläche.

>[!IMPORTANT]
>
>Pro Konto-Locator kann nur ein privater Eintrag erstellt werden.

1. Klicken Sie auf das **[!UICONTROL Hauptmenü]**-Symbol ![Hauptmenü](/help/_includes/assets/main-menu-icon.png) in der oberen rechten Ecke von Adobe Workfront oder (falls verfügbar) klicken Sie auf das **[!UICONTROL Hauptmenü]**-Symbol ![Hauptmenü](/help/_includes/assets/main-menu-icon-left-nav.png) in der oberen linken Ecke und klicken Sie dann auf **Setup**.

1. Klicken Sie im linken Bedienfeld auf **System** > **Datenverbindung**.

1. Klicken Sie auf die Registerkarte **Snowflake** Verbindungen.

1. Klicken Sie **Privaten Eintrag hinzufügen**.

1. Füllen Sie das Formular mit den erfassten Kontodetails aus, einschließlich Ihres bevorzugten Datenbanknamens.

1. Klicken Sie **Privaten Eintrag hinzufügen**.

### Herstellen einer Verbindung zum Listeneintrag in Snowflake

Stellen Sie in Ihrem Snowflake-Konto eine Verbindung zur privaten Liste als externe Datenquelle her. Sie können dann Ihre Workfront-Daten zusammen mit den anderen Daten abfragen.

## Aktuelle und tägliche Verlaufsansichten einrichten

Eine Leserkontenverbindung bietet drei Datenansichten für jede Objekttabelle:

* **Aktuell** - Eine Darstellung der Daten mit niedriger Latenz, wie sie derzeit in der Quellanwendung vorhanden sind.
* **Daily History** - eine Darstellung der Daten, wie sie um 23:59 Uhr UTC für jeden Tag waren.
* **Ereignis** - jede Änderungstransaktion, die an die Data Connect-Datenpipelines gesendet wird.

Eine private Auflistung gibt nur die Ereignisansicht frei. Dieser Abschnitt enthält SQL zum Erstellen der Ansichten „Aktuell“, „Täglicher Verlauf“ und „Ereignis“ in Ihrem eigenen Snowflake-Konto.

Alle in der Liste enthaltenen Ereignisansichten verfügen über die Felder, die für die unten stehende Ansichtslogik benötigt werden. Bei diesen Beispielen wird davon ausgegangen, dass Sie eine neue Datenbank und ein neues Schema Ihrer Wahl im Snowflake-Zielkonto erstellt haben und dass sie die `projects_event` verwenden. Ersetzen Sie in jedem Beispiel `<listing_db>` und `<listing_schema>` durch Ihre eigenen Werte.

>[!TIP]
>
>Es wird empfohlen, `select *` durch eine Liste der Spalten zu ersetzen, die Sie für Ihre Analysen verwenden. Wenn Sie `select *` verwenden und Spalten später zur Ereignisansicht des Listeneintrags hinzugefügt werden, müssen Sie die Ansicht neu erstellen, um die neuen Spalten zu aktivieren.

### Aktuelle Ansichten

Die aktuelle Ansicht eines Objekts ist der letzte in Data Connect gespeicherte Änderungsereignisdatensatz. Wenn sich der letzte Datensatz in einem gelöschten Status befindet, wird der Datensatz in der aktuellen Ansicht weggelassen. Alle Ereignisansichten haben dieselbe Struktur.

```sql
create or replace view projects_current copy grants
as
select *
from <listing_db>.<listing_schema>.projects_event
where end_effective_timestamp = '2300-01-01'::timestamp_ntz
 and nvl(deleted, 0) != 1;
```

Die Spalten `deleted` und `end_effective_timestamp` sind in der aktuellen Ansicht nicht erforderlich. Die Ansicht filtert die Daten auf einen einzelnen Wert und entfernt den Datensatz vollständig, wenn der Datensatz gelöscht wird.

### Tägliche Verlaufsansichten

Die Ansicht „Täglicher Verlauf“ identifiziert den Änderungsereignis-Datensatz, der am 23:59:59. eines bestimmten Datums aktiv war, sodass Sie den Status des Datensatzes im Zeitverlauf verfolgen können. Das folgende Beispiel zeigt den Status eines Projektdatensatzes am Ende jedes Kalendertages.

```sql
create or replace view projects_daily_history copy grants
as
select d.calendardate as
 , p.*
from <listing_db>.<listing_schema>.calendar_dates d
join <listing_db>.<listing_schema>.projects_event p
 on p.begin_effective_timestamp <= d.calendareodtimestamp
and d.calendareodtimestamp < p.end_effective_timestamp
where d.calendareodtimestamp < current_date() - 1
 and nvl(deleted, 0) != 1;
```

### Ereignisansichten

Aus Konsistenzgründen empfehlen wir, eine Kopie der Ereignisansicht aus der Auflistungsdatenbank zu erstellen und sie im selben Schema wie die aktuellen und täglichen Verlaufsansichten zu platzieren.

```sql
create or replace view projects_event copy grants
as
select *
from <listing_db>.<listing_schema>.projects_event;
```
