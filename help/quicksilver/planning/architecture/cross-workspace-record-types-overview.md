---
title: Übersicht über arbeitsbereichsübergreifende Datensatztypen
description: Sie können Datensatztypen als global oder verbindbar aktivieren. Globale Datensatztypen können in Adobe Workfront Planning über einen zentralen oder primären Arbeitsbereich zu mehreren Arbeitsbereichen hinzugefügt werden, während verbindbare Datensatztypen über andere Arbeitsbereiche als ihren eigenen mit verbunden werden können.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: aeedd871-dcd3-4fb3-bfc5-99db3e7c9296
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/G0zsfMcj1dSM-QN3lPprt8rPSoG1Wli4lWqDzMiG3c4
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2:
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 1751
ht-degree: 0%

---

# Übersicht über Workspace-übergreifende Datensatztypen

<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>
-->

{{planning-important-intro}}

In Adobe Workfront Planning können Sie Workspace-übergreifende Funktionen für einen Datensatztyp aktivieren. Ein arbeitsbereichsübergreifender Datensatztyp kann von mehr als einem Arbeitsbereich aus referenziert oder aufgerufen werden.

>[!IMPORTANT]
>
>Ihr Unternehmen muss die folgenden Pakete erwerben, um arbeitsbereichsübergreifende Funktionen für Datensatztypen aktivieren zu können:
>
>So konfigurieren Sie verbindbare Datensatztypen:
>
>
>* Jedes Workfront-Paket und jedes Planungspaket
>
>   ODER
>
>* Beliebiger Workflow und ein Planning Prime- oder Ultimate-Paket
>
>So konfigurieren Sie globale Datensatztypen:
>
>* Beliebiges Workfront-Paket und Planning Plus-Paket
>     
>   ODER
>
>* Beliebiger Workflow und ein Planning Prime- oder Ultimate-Paket
>
>Weitere Informationen zu den einzelnen Workfront-Planungspaketen erhalten Sie von Ihrem Workfront-Kundenbetreuer.
>Weitere Informationen finden Sie unter [Übersicht über den Zugriff auf Adobe Workfront Planning](/help/quicksilver/planning/access/access-overview.md).

Im Folgenden finden Sie arbeitsbereichsübergreifende Funktionen von Datensatztypen:

* **Globale Datensatztypen**: Benutzer können globale Datensatztypen zu anderen von ihnen verwalteten Arbeitsbereichen hinzufügen.

* **Verbindbare Datensatztypen**: Benutzer können von anderen Arbeitsbereichen aus eine Verbindung zu diesem Datensatztyp herstellen.

In diesem Artikel erhalten Sie einen Überblick über arbeitsbereichsübergreifende Datensatztypen. Informationen zum Definieren der arbeitsbereichsübergreifenden Funktionen eines Datensatztyps finden Sie unter [Konfigurieren von arbeitsbereichsübergreifenden Funktionen für Datensatztypen](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md).

## Übersicht über globale Datensatztypen

Globale Datensatztypen können in Workfront Planning über einen zentralen oder primären Arbeitsbereich zu mehreren Arbeitsbereichen hinzugefügt werden.

Bei der Implementierung von Workfront Planning für ein Unternehmen mit mehreren Teams mit gemeinsamen Workflows müssen Sie möglicherweise eine zusammenhängende Struktur und Metadaten für wichtige Datensatztypen (wie Kampagnen oder Ergebnisse) definieren, die den Arbeitsbereichen jedes Teams hinzugefügt werden können, um ihre Arbeit zu erfassen und zu verwalten.

Möglicherweise benötigen Sie auch die Arbeit jedes Teams, um eine zentrale Ebene zu erreichen.

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

### Überlegungen zu den globalen Datensatztypen in ihrem ursprünglichen Primären Arbeitsbereich

Der als „global“ konfigurierte Datensatztyp hat die folgenden Eigenschaften:

* Alle zugehörigen Informationen (Erscheinungsbild, ursprüngliche Felder) können nur im ursprünglichen Arbeitsbereich bearbeitet werden.

* Sie können die folgenden Aktionen für den globalen Datensatztyp in seinem ursprünglichen Arbeitsbereich ausführen:

   * Bearbeiten

     Das Bearbeiten eines globalen Datensatztyps umfasst das Bearbeiten seines Erscheinungsbilds, seiner arbeitsbereichsübergreifenden Funktionen und aller im ursprünglichen Arbeitsbereich erstellten Felder.
   * Freigeben

     Durch die Freigabe eines Datensatztyps werden Benutzer zum Arbeitsbereich hinzugefügt und die Datensätze für diese Benutzer freigegeben.
   * Löschen

     Sie können einen globalen Datensatztyp erst aus seinem ursprünglichen Arbeitsbereich löschen, nachdem Sie alle Instanzen des Datensatztyps aus allen sekundären Arbeitsbereichen gelöscht haben, in denen er hinzugefügt wurde.

     Weitere Informationen finden Sie unter [Datensatztypen löschen](/help/quicksilver/planning/architecture/delete-record-types.md).
   * Herstellen einer Verbindung von anderen Arbeitsbereichen
   * Anfrageformulare erstellen und verwalten
   * Automatisierungen erstellen und verwalten

* Die folgenden Datensätze werden im Primären Arbeitsbereich eines globalen Datensatztyps angezeigt:

   * Vom globalen Datensatztyp im Primären Arbeitsbereich hinzugefügte Datensätze
   * Datensätze, die von globalen Datensatztypen in den sekundären Arbeitsbereichen hinzugefügt wurden, in denen sie hinzugefügt wurden

     Die Datensätze, die Sie aus einem sekundären Arbeitsbereich hinzufügen, werden aggregiert und im primären Arbeitsbereich angezeigt. Alle Mitglieder des ursprünglichen primären Arbeitsbereichs erhalten Ansichtsberechtigungen für sie, und die Datensätze sind für sie nur im Primären Arbeitsbereich sichtbar, selbst wenn sie keine Berechtigungen für den sekundären Arbeitsbereich haben.
* Die folgenden Szenarien zeigen, welche Berechtigungen Sie für die im primären Arbeitsbereich angezeigten Datensätze haben, je nachdem, aus welcher Quelle sie hinzugefügt wurden:

   * Sie haben für die im Primären Arbeitsbereich erstellten Datensätze dieselben Berechtigungen wie für den Arbeitsbereich und den ursprünglichen globalen Datensatztyp.
   * Sie haben dieselben Berechtigungen für die in einem sekundären Arbeitsbereich erstellten Datensätze wie für den sekundären Arbeitsbereich und den globalen Datensatztyp in diesem Bereich.

  <!--
    Removed this as this was too confusing: 
    * When the original global record type is added to multiple secondary workspaces, users gain the following visibility to the records added to the global record types: 
        * Members of the original workspace automatically gain View permissions to all records added from any workspace, even if they are  not members of those workspaces. They can view these records in the following workspaces, only if they are a member of these following workspaces: 
            * The primary workspace
            * The secondary workspace where the records were added. Secondary workspace members can view only records from workspaces where they are a member.
    -->

* Die mit einem globalen Datensatztyp verbundenen Datensatztypen werden für die Verbindung in den Arbeitsbereichen verfügbar, in denen dieser Datensatztyp hinzugefügt wird.

  Wenn Sie beispielsweise über einen globalen Campaign-Datensatztyp verfügen, der eine Verbindung mit dem Datensatztyp Regionen aufweist, und Sie den Campaign-Datensatztyp einem sekundären Arbeitsbereich hinzufügen, werden Regionen vom sekundären Arbeitsbereich aus arbeitsbereichsübergreifend verbindbar. Die Mitglieder des sekundären Arbeitsbereichs können jetzt Kampagnen erstellen und sie mit Regionen verknüpfen.

* Felder, die für einen globalen Datensatztyp aus dem ursprünglichen Arbeitsbereich erstellt wurden, sind in allen Arbeitsbereichen sichtbar, in denen der Datensatztyp hinzugefügt wird.

  Sie können Feldeinstellungen nur über den ursprünglichen Arbeitsbereich bearbeiten.

  Die Einstellungen der im ursprünglichen Arbeitsbereich erstellten Felder sind in den sekundären Arbeitsbereichen für alle Mitglieder schreibgeschützt, unabhängig von ihren Berechtigungen für den sekundären Arbeitsbereich.

  Sekundär Workspace-Manager können die Feldeinstellungen für Felder, die im ursprünglichen Workspace konfiguriert wurden, nicht ändern. Nur die Arbeitsbereich-Manager des ursprünglichen Arbeitsbereichs können die Feldeinstellungen im ursprünglichen Arbeitsbereich ändern.

### Überlegungen zu globalen Datensatztypen in einem sekundären Arbeitsbereich

* Sekundäre Arbeitsbereich-Mitwirkende erhalten die Berechtigung Beitragen für den globalen Datensatztyp im Arbeitsbereich ihres Teams. Sie können Datensätze darin vom sekundären Arbeitsbereich hinzufügen und verwalten.

* Sekundäre Arbeitsbereich-Betrachter erhalten die Berechtigung zum Anzeigen des globalen Datensatztyps im Arbeitsbereich ihres Teams. Sie können darin keine Datensätze hinzufügen und verwalten.

* Sekundär Workspace-Manager können die folgenden zusätzlichen Aktionen für den Datensatztyp ausführen, der von einem globalen Datensatztyp in einem sekundären Workspace hinzugefügt wurde:

   * Löschen.

     Wenn Sie den Datensatztyp aus einem sekundären Arbeitsbereich löschen, wird er nur aus dem sekundären Arbeitsbereich entfernt. Die Datensätze und Felder, die ihm aus dem sekundären Arbeitsbereich hinzugefügt wurden, werden auch aus dem sekundären Arbeitsbereich gelöscht. Die im sekundären Bereich hinzugefügten Datensätze verbleiben im primären Arbeitsbereich. Dadurch wird der Datensatztyp nicht aus seinem ursprünglichen Arbeitsbereich oder aus anderen sekundären Arbeitsbereichen, in denen er hinzugefügt wurde, gelöscht.

     Weitere Informationen finden Sie unter [Datensatztypen löschen](/help/quicksilver/planning/architecture/delete-record-types.md).

   * Freigeben

     Durch die Freigabe eines globalen Datensatztyps in einem sekundären Arbeitsbereich treten auch folgende Situationen ein:

      * Benutzende werden zum Arbeitsbereich mit Anzeigeberechtigungen hinzugefügt.
      * Benutzer erhalten dieselben Berechtigungen für alle Datensätze des globalen Datensatztyps im sekundären Arbeitsbereich.
   * Geben Sie die Ansichten der Datensatztypen frei.

     Sie können eine Ansicht nicht öffentlich über einen globalen Datensatztyp in einem sekundären Arbeitsbereich freigeben. Sie können Ansichten nur intern über einen sekundären Arbeitsbereich freigeben. Sie können eine Ansicht intern und öffentlich für einen globalen Datensatztyp in seinem ursprünglichen Arbeitsbereich freigeben.

     Weitere Informationen finden Sie unter [Freigeben von Ansichten](/help/quicksilver/planning/access/share-views.md).


<!--
when they will be able to add fields to the secondary space, this bullet will need this extra information: 
After adding fields to the global record type in the secondary workspace, shared views might not open for other users in workspaces. The fields exist only in the secondary workspace and they would not be visible in any other workspace. Only fields created in the primary workspace are visible in all secondary workspaces where there the record type is added.
-->

<!--
These two capabilities will come later - and edit some of the bullets below after these capabilities are released:
* Add new fields
    Fields added to a global record from a secondary workspace are visible only from the secondary workspace. 
* Add request forms to it
* Add automations to it
-->

* Kein Benutzer kann die folgenden Aktionen für einen globalen Datensatztyp in einem sekundären Arbeitsbereich ausführen:

   * Bearbeiten

     Sie können weder sein Erscheinungsbild noch seine Workspace-übergreifenden Funktionen oder die Felder bearbeiten, die aus dem ursprünglichen Workspace hinzugefügt wurden.
   * Anfrageformulare erstellen und verwalten
   * Automatisierungen erstellen und verwalten

* Datensätze, die in einem sekundären Arbeitsbereich hinzugefügt wurden, sind in den folgenden Arbeitsbereichen sichtbar, wenn Sie über Anzeigen- oder höhere Berechtigungen für diese Arbeitsbereiche verfügen:

   * Der sekundäre Ort, an dem sie hinzugefügt wurden
   * Der ursprüngliche primäre Arbeitsbereich des globalen Datensatztyps

* Die folgenden Szenarien sind für den Zugriff auf Datensätze vorhanden, die in sekundären Arbeitsbereichen erstellt wurden:

   * Wenn Sie über Verwaltungsberechtigungen für den ursprünglichen Arbeitsbereich und keine Berechtigungen für sekundäre Arbeitsbereiche verfügen, können Sie Datensätze anzeigen, die von den sekundären Arbeitsbereichen im ursprünglichen Arbeitsbereich hinzugefügt wurden. Sie können diese jedoch nicht über den ursprünglichen Arbeitsbereich verwalten.
   * Wenn Sie über Verwaltungsberechtigungen für den ursprünglichen und den sekundären Arbeitsbereich verfügen, können Sie die Datensätze sowohl aus dem ursprünglichen Arbeitsbereich des globalen Datensatztyps als auch aus dem sekundären Arbeitsbereich verwalten, in dem sie hinzugefügt wurden.
  <!--
    not anymore: * You can view the records in additional secondary workspaces where the global record type is added only if you have View permissions to those workspaces
    -->
* Es ist nicht möglich, Ansichten eines globalen Datensatztyps in einem sekundären Arbeitsbereich öffentlich freizugeben.

### Zugriff auf die Verbindungen eines globalen Datensatztyps

Datensatztypen, die mit dem globalen Datensatztyp im ursprünglichen Arbeitsbereich verbunden sind, werden in anderen Arbeitsbereichen sichtbar, in denen der globale Datensatztyp hinzugefügt wird, und sie sind für Verbindungen von den sekundären Arbeitsbereichen verfügbar, in denen der globale Datensatztyp hinzugefügt wird.

### API-Zugriff eines globalen Datensatztyps

Beim Hinzufügen von Datensätzen zu einem globalen Datensatztyp aus einem sekundären Arbeitsbereich mithilfe der Workfront Planning-API überprüft das System, ob der Benutzer Zugriff zum Erstellen von Datensätzen im ursprünglichen Arbeitsbereich des globalen Datensatztyps hat.

Die folgenden Fälle liegen vor:

* Wenn der/die Benutzende Zugriff hat, wird der Datensatz im ursprünglichen Arbeitsbereich globaler Datensatztypen erstellt.

* Wenn der/die Benutzende keinen Zugriff hat, erhält der/die Benutzende die Fehlermeldung, dass er/sie keinen Zugriff auf den ursprünglichen Arbeitsbereich des globalen Datensatztyps hat und er/sie die Arbeitsbereich-ID angeben muss, unter der er/sie Zugriff zum Erstellen von Datensätzen hat.

## Übersicht über verbindbare Datensatztypen

Sie können eine Verbindung zu einem Datensatztyp herstellen, der als von jedem von Ihnen verwalteten Arbeitsbereich aus verbindbar definiert wurde.

Möglicherweise müssen Ihre Teams ihre Datensätze mit Datensatztypen aus anderen Arbeitsbereichen verknüpfen oder Informationen anzeigen, die in Datensätzen erfasst wurden, die zu Datensätzen in anderen Arbeitsbereichen gehören. Sie können diese Konfiguration erreichen, indem Sie einen Datensatztyp als „verbindbar“ festlegen.

Gehen Sie wie folgt vor, um verbindbare Datensatztypen zu verwenden:

1. Konfigurieren Sie einen Datensatztyp, der in einem bestimmten Arbeitsbereich verbunden werden kann.

   Ein Workspace-Manager kann auswählen, mit welchen Arbeitsbereichen ein bestimmter Datensatztyp verbunden werden kann.

   Der ursprüngliche Datensatztyp ist im ursprünglichen Arbeitsbereich vorhanden und kann von einem anderen Arbeitsbereich aus aufgerufen werden, um eine Verbindung zu herzustellen.

   >[!TIP]
   >
   >Nur Systemadministratoren können einen Datensatztyp festlegen, der über alle Arbeitsbereiche im System verbunden werden kann. Alle anderen Workspace-Manager können bestimmte Workspaces bestimmen, von denen aus eine Verbindung mit dem Datensatztyp hergestellt werden soll.
   >
   >Weitere Informationen finden Sie unter [Konfigurieren von arbeitsbereichsübergreifenden Funktionen für Datensatztypen](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md).
1. Stellen Sie eine Verbindung zu einem Datensatztyp her, der als von einem anderen von Ihnen verwalteten Arbeitsbereich aus verbindbar gekennzeichnet ist.

   Weitere Informationen finden Sie unter [Verbinden von Datensatztypen](/help/quicksilver/planning/architecture/connect-record-types.md).
