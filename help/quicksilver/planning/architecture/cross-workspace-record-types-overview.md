---
title: Übersicht über arbeitsbereichsübergreifende Datensatztypen
description: Sie können Datensatztypen als global oder verbindbar aktivieren. Globale Datensatztypen können in Adobe Workfront Planning über einen zentralen oder primären Arbeitsbereich zu mehreren Arbeitsbereichen hinzugefügt werden, während verbindbare Datensatztypen über andere Arbeitsbereiche als ihren eigenen mit verbunden werden können.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: aeedd871-dcd3-4fb3-bfc5-99db3e7c9296
source-git-commit: 2fb95d37c32984e248767993c4858038d27e0590
workflow-type: tm+mt
source-wordcount: '1534'
ht-degree: 0%

---


# Übersicht über Workspace-übergreifende Datensatztypen

<span class="preview">Die hervorgehobenen Informationen auf dieser Seite beziehen sich auf Funktionen, die noch nicht allgemein verfügbar sind. Sie ist nur in der Vorschau -Umgebung für alle Kunden verfügbar. Nach den monatlichen Releases in der Produktion stehen dieselben Funktionen auch in der Produktionsumgebung für Kunden zur Verfügung, die schnelle Releases aktiviert haben. </span>

<span class="preview">Informationen zu Schnellversionen finden Sie unter [Aktivieren oder Deaktivieren von Schnellversionen für Ihre Organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>

{{planning-important-intro}}

In Adobe Workfront Planning können Sie Workspace-übergreifende Funktionen für einen Datensatztyp aktivieren. Ein arbeitsbereichsübergreifender Datensatztyp kann von mehr als einem Arbeitsbereich aus referenziert oder aufgerufen werden.

>[!IMPORTANT]
>
>Es gibt erweiterte Workfront-Paketanforderungen, um arbeitsbereichsübergreifende Funktionen für Datensatztypen in Ihrem System aktivieren zu können. Weitere Informationen finden Sie unter [Adobe Workfront Planning-Zugriffsübersicht](/help/quicksilver/planning/access/access-overview.md).


Im Folgenden finden Sie arbeitsbereichsübergreifende Funktionen von Datensatztypen:

* <span class="preview">**Globale Datensatztypen**: Benutzer können globale Datensatztypen zu anderen von ihnen verwalteten Arbeitsbereichen hinzufügen.</span>

* **Verbindbare Datensatztypen**: Benutzer können von anderen Arbeitsbereichen aus eine Verbindung zu diesem Datensatztyp herstellen.

In diesem Artikel erhalten Sie einen Überblick über arbeitsbereichsübergreifende Datensatztypen. Informationen zum Definieren der arbeitsbereichsübergreifenden Funktionen eines Datensatztyps finden Sie unter [Konfigurieren von arbeitsbereichsübergreifenden Funktionen für Datensatztypen](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md).

<div class="preview">

## Übersicht über globale Datensatztypen

Globale Datensatztypen können in Workfront Planning über einen zentralen oder primären Arbeitsbereich zu mehreren Arbeitsbereichen hinzugefügt werden.

Bei der Implementierung von Workfront Planning für ein Unternehmen mit mehreren Teams mit gemeinsamen Workflows müssen Sie möglicherweise eine zusammenhängende Struktur und Metadaten für wichtige Datensatztypen (wie Kampagnen oder Ergebnisse) definieren, die den Arbeitsbereichen jedes Teams hinzugefügt werden können, um ihre Arbeit zu erfassen und zu verwalten.

Außerdem benötigen Sie möglicherweise die Arbeit jedes Teams, um eine zentrale Ebene zu erreichen.

In einem solchen Workflow können Sie sicherstellen, dass Teams ihre Arbeit konsistent erfassen, während Sie die Team-übergreifende Sichtbarkeit erschließen, ohne dass alles zu einem Arbeitsbereich oder alle Personen in der Organisation zu jedem Arbeitsbereich hinzugefügt werden müssen. Sie können dazu globale Datensatztypen verwenden.

Gehen Sie wie folgt vor, um globale Datensatztypen zu verwenden:

1. Konfigurieren Sie in einem von Ihnen verwalteten Arbeitsbereich einen Datensatztyp so, dass er global ist.

   Ein Workspace-Manager kann Benutzern mit einer Standardlizenz oder Teams, Gruppen, Rollen und Unternehmen Berechtigungen erteilen, um einen ausgewählten Datensatztyp zu einem von ihnen verwalteten Arbeitsbereich hinzuzufügen.

   Der ursprüngliche Datensatztyp ist in seinem ursprünglichen Arbeitsbereich vorhanden, wird jedoch in anderen Arbeitsbereichen sichtbar gemacht.

   Weitere Informationen finden Sie unter [Konfigurieren von arbeitsbereichsübergreifenden Funktionen für Datensatztypen](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md).
1. Fügen Sie einen Datensatztyp zu einem sekundären Arbeitsbereich hinzu, der von einem vorhandenen Arbeitsbereich stammt, der als globaler Datensatztyp konfiguriert wurde.

   Der Datensatztyp ist in den folgenden Arbeitsbereichen vorhanden:

   * Der ursprüngliche Arbeitsbereich, in dem er als globaler Datensatztyp angegeben war.
   * Ein sekundärer Arbeitsbereich.

   Weitere Informationen finden Sie unter [Hinzufügen vorhandener Datensatztypen aus einem anderen Arbeitsbereich](/help/quicksilver/planning/architecture/add-existing-record-types-from-another-workspace.md).

   In den folgenden Abschnitten werden Überlegungen zu globalen Datensatztypen und deren Funktionsweise in ihren ursprünglichen oder sekundären Arbeitsbereichen beschrieben.

### Überlegungen zu den globalen Datensatztypen in ihrem ursprünglichen Arbeitsbereich

Der als „global“ konfigurierte Datensatztyp hat die folgenden Eigenschaften:

* Alle zugehörigen Informationen (Erscheinungsbild, ursprüngliche Felder) können nur im ursprünglichen Arbeitsbereich bearbeitet werden.

* Sie können die folgenden Aktionen für den globalen Datensatztyp in seinem ursprünglichen Arbeitsbereich ausführen:

   * Bearbeiten

     Das Bearbeiten eines globalen Datensatztyps umfasst das Bearbeiten seines Erscheinungsbilds, seiner arbeitsbereichsübergreifenden Funktionen und aller im ursprünglichen Arbeitsbereich erstellten Felder.
   * Anfrageformulare erstellen und verwalten
   * Automatisierungen erstellen und verwalten

* Ein globaler Datensatztyp kann nur gelöscht werden, wenn er nicht zu einem sekundären Arbeitsbereich hinzugefügt wurde. Sie müssen sie zunächst (durch Löschen) aus den sekundären Arbeitsbereichen entfernen, bevor Sie sie aus dem ursprünglichen Arbeitsbereich löschen können.

  Weitere Informationen finden Sie unter [Datensatztypen löschen](/help/quicksilver/planning/architecture/delete-record-types.md).
* Die Datensätze, die Sie einem globalen Datensatztyp hinzufügen, sind nur für Benutzer sichtbar, die über Anzeigeberechtigungen für den Arbeitsbereich verfügen, in dem sie hinzugefügt wurden.
* Die Datensätze, die Sie aus einem sekundären Arbeitsbereich hinzufügen, werden aggregiert und im ursprünglichen Arbeitsbereich angezeigt. Alle Mitglieder des ursprünglichen Arbeitsbereichs erhalten Ansichtsberechtigungen für sie.
* Wenn der ursprüngliche globale Datensatztyp mehreren sekundären Arbeitsbereichen hinzugefügt wird, existieren die folgenden Szenarien:

   * Mitglieder des ursprünglichen Arbeitsbereichs erhalten automatisch Ansichtsberechtigungen für alle Datensätze, die aus einem Arbeitsbereich hinzugefügt wurden, selbst wenn sie nicht Mitglieder dieser Arbeitsbereiche sind.
   * Sekundäre Arbeitsbereichsmitglieder können nur Datensätze aus Arbeitsbereichen anzeigen, in denen sie Mitglied sind.
* Die verbundenen Datensatztypen eines globalen Datensatztyps werden für die Verbindung in den Arbeitsbereichen verfügbar, in denen dieser Datensatztyp hinzugefügt wird.

  Wenn Sie beispielsweise über einen globalen Campaign-Datensatztyp verfügen, der eine Verbindung mit dem Datensatztyp Regionen aufweist, und Sie den Campaign-Datensatztyp einem sekundären Arbeitsbereich hinzufügen, werden Regionen vom sekundären Arbeitsbereich aus arbeitsbereichsübergreifend verbindbar. Die Mitglieder des sekundären Arbeitsbereichs können jetzt Kampagnen erstellen und sie mit Regionen verknüpfen.

* Felder, die für einen globalen Datensatztyp aus dem ursprünglichen Arbeitsbereich erstellt wurden, sind in allen Arbeitsbereichen sichtbar, in denen der Datensatztyp hinzugefügt wird. Sie können Feldeinstellungen nur über den ursprünglichen Arbeitsbereich bearbeiten. Die Einstellungen der im ursprünglichen Arbeitsbereich erstellten Felder sind in den sekundären Arbeitsbereichen für alle Mitglieder schreibgeschützt, unabhängig von ihren Berechtigungen für den sekundären Arbeitsbereich. Sekundär Workspace-Manager können die Feldeinstellungen für Felder, die im ursprünglichen Workspace konfiguriert wurden, nicht ändern. Nur die Arbeitsbereich-Manager des ursprünglichen Arbeitsbereichs können die Feldeinstellungen im ursprünglichen Arbeitsbereich ändern.

### Überlegungen zu globalen Datensatztypen in einem sekundären Arbeitsbereich

* Sekundäre Arbeitsbereich-Mitwirkende erhalten die Berechtigung Beitragen für den globalen Datensatztyp im Arbeitsbereich ihres Teams. Sie können Datensätze darin vom sekundären Arbeitsbereich hinzufügen und verwalten.

* Sekundäre Arbeitsbereich-Betrachter erhalten die Berechtigung zum Anzeigen des globalen Datensatztyps im Arbeitsbereich ihres Teams. Sie können darin keine Datensätze hinzufügen und verwalten.

* Sekundär Workspace-Manager können die folgenden zusätzlichen Aktionen für den Datensatztyp ausführen, der von einem globalen Datensatztyp in einem sekundären Workspace hinzugefügt wurde:

   * Löschen.

     Wenn Sie den Datensatztyp aus einem sekundären Arbeitsbereich löschen, wird er nur aus dem sekundären Arbeitsbereich entfernt. Die Datensätze und Felder, die ihm aus dem sekundären Arbeitsbereich hinzugefügt wurden, werden ebenfalls gelöscht. Dadurch wird der Datensatztyp nicht aus seinem ursprünglichen Arbeitsbereich oder aus anderen sekundären Arbeitsbereichen, in denen er hinzugefügt wurde, gelöscht.

     Weitere Informationen finden Sie unter [Datensatztypen löschen](/help/quicksilver/planning/architecture/delete-record-types.md).

  <!--These two capabilities will come later - and edit some of the bullets below after these capabilities are released:
    * Add new fields
        Fields added to a global record from a secondary workspace are visible only from the secondary workspace. 
    * Share it
    * Add request forms to it
    * Add automations to it-->

* Kein Benutzer kann die folgenden Aktionen für einen globalen Datensatztyp in einem sekundären Arbeitsbereich ausführen:

   * Bearbeiten

     Sie können weder sein Erscheinungsbild noch seine Workspace-übergreifenden Funktionen oder die Felder bearbeiten, die aus dem ursprünglichen Workspace hinzugefügt wurden.
   * Freigeben
   * Anfrageformulare erstellen und verwalten
   * Automatisierungen erstellen und verwalten

* In einem sekundären Arbeitsbereich hinzugefügte Datensätze sind nur dann in den folgenden Arbeitsbereichen sichtbar, wenn Sie über die Berechtigung zum Anzeigen oder eine höhere Berechtigung für diese Arbeitsbereiche verfügen:

   * Der sekundäre Arbeitsbereich, in dem sie hinzugefügt werden.
   * Der ursprüngliche Arbeitsbereich des globalen Datensatztyps.
   * Alle anderen Arbeitsbereiche, bei denen der globale Arbeitsbereich hinzugefügt wird.

* Die folgenden Szenarien existieren für Datensätze, die in sekundären Arbeitsbereichen erstellt wurden:

   * Wenn Sie über Verwaltungsberechtigungen für den ursprünglichen Arbeitsbereich und keine Berechtigungen für sekundäre Arbeitsbereiche verfügen, können Sie Datensätze anzeigen, die von den sekundären Arbeitsbereichen im ursprünglichen Arbeitsbereich hinzugefügt wurden. Sie können diese jedoch nicht über den ursprünglichen Arbeitsbereich verwalten.
   * Wenn Sie über Verwaltungsberechtigungen für den sekundären Arbeitsbereich verfügen, können Sie die Datensätze sowohl aus dem ursprünglichen Arbeitsbereich des globalen Datensatztyps als auch aus dem sekundären Arbeitsbereich verwalten, in dem sie hinzugefügt wurden.
   * Sie können die Datensätze in zusätzlichen sekundären Arbeitsbereichen anzeigen, bei denen der globale Datensatztyp nur hinzugefügt wird, wenn Sie über Anzeigeberechtigungen für diese Arbeitsbereiche verfügen.

### Zugriff auf die Verbindungen eines globalen Datensatztyps

Datensatztypen, die mit dem globalen Datensatztyp im ursprünglichen Arbeitsbereich verbunden sind, werden in anderen Arbeitsbereichen sichtbar, in denen der globale Datensatztyp hinzugefügt wird, und sie sind für Verbindungen von den sekundären Arbeitsbereichen verfügbar, in denen der globale Datensatztyp hinzugefügt wird.

### API-Zugriff eines globalen Datensatztyps

Beim Hinzufügen von Datensätzen zu einem globalen Datensatztyp aus einem sekundären Arbeitsbereich mithilfe der Workfront Planning-API überprüft das System, ob der Benutzer Zugriff zum Erstellen von Datensätzen im ursprünglichen Arbeitsbereich des globalen Datensatztyps hat.

Die folgenden Fälle liegen vor:

* Wenn der/die Benutzende Zugriff hat, wird der Datensatz im ursprünglichen Arbeitsbereich globaler Datensatztypen erstellt.

* Wenn der/die Benutzende keinen Zugriff hat, erhält der/die Benutzende die Fehlermeldung, dass er/sie keinen Zugriff auf den ursprünglichen Arbeitsbereich des globalen Datensatztyps hat und er/sie die Arbeitsbereich-ID angeben muss, unter der er/sie Zugriff zum Erstellen von Datensätzen hat.

</div>

## Übersicht über verbindbare Datensatztypen

Sie können eine Verbindung zu einem Datensatztyp herstellen, der als von jedem von Ihnen verwalteten Arbeitsbereich aus verbindbar definiert wurde.

Möglicherweise müssen Ihre Teams ihre Datensätze mit Datensatztypen aus anderen Arbeitsbereichen verknüpfen oder Informationen anzeigen, die in Datensätzen erfasst wurden, die zu Datensätzen in anderen Arbeitsbereichen gehören. Sie können diese Konfiguration erreichen, indem Sie einen Datensatztyp als „verbindbar“ festlegen.

Gehen Sie wie folgt vor, um verbindbare Datensatztypen zu verwenden:

1. Konfigurieren Sie einen Datensatztyp, der in einem bestimmten Arbeitsbereich verbunden werden kann.

   Ein Workspace-Manager kann auswählen, mit welchen Arbeitsbereichen ein bestimmter Datensatztyp verbunden werden kann.

   Der ursprüngliche Datensatztyp ist im ursprünglichen Arbeitsbereich vorhanden und kann von einem anderen Arbeitsbereich aus aufgerufen werden, um eine Verbindung zu herzustellen.

   Weitere Informationen finden Sie unter [Konfigurieren von arbeitsbereichsübergreifenden Funktionen für Datensatztypen](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md).
1. Stellen Sie eine Verbindung zu einem Datensatztyp her, der als von einem anderen von Ihnen verwalteten Arbeitsbereich aus verbindbar gekennzeichnet ist.

   Weitere Informationen finden Sie unter [Verbinden von Datensatztypen](/help/quicksilver/planning/architecture/connect-record-types.md).
