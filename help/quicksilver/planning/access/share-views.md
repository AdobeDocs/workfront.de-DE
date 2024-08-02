---
title: Ansichten freigeben
description: Sie können eine Ansicht für andere freigeben, um die Zusammenarbeit bei der Verwendung der Adobe Workfront-Planung sicherzustellen.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 673dd888-3135-48b0-8198-c8d6d6706ddf
source-git-commit: 1ffd8a3dbb31154186dc37132c7e77c35de42ac3
workflow-type: tm+mt
source-wordcount: '1020'
ht-degree: 1%

---

<!--update the metadata and description when we turn this article live-->

# Ansichten freigeben

{{planning-important-intro}}

Sie können eine Ansicht für andere freigeben, um die Zusammenarbeit bei der Arbeit mit Datensätzen in der Adobe Workfront-Planung sicherzustellen.

Wenn Sie Berechtigungen für einen Arbeitsbereich erteilen, erhalten andere Benutzer keine Berechtigungen für die Ansichten auf den Seiten vom Typ Datensatz. Sie müssen einzelnen Ansichten auf einer Seite vom Typ Datensatz Berechtigungen erteilen, um sie für andere Benutzer freizugeben.

Wenn Sie eine Ansicht freigeben, gewähren Sie anderen Berechtigungen für den Zugriff auf alle Elemente der Ansicht. Wenn Sie ihnen beispielsweise Berechtigungen zum Verwalten für eine Ansicht erteilen, können sie die Gruppierung, den Filter, die Sortierung oder das Erscheinungsbild der Leiste ändern.


Sie können eine Ansicht für die folgenden Entitäten freigeben:

* Intern mit Workfront-Benutzern und -Gruppen
* Öffentlich für Benutzer außerhalb von Workfront

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Workfront-Planung anzuzeigen.

<!--at GA the plan below will change to Prime, Select and Ultimate only-->

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Produkt</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront-Abkommen</p></td>
   <td>
<p>Ihr Unternehmen muss in der Phase des frühen Zugriffs für die Workfront-Planung eingeschrieben sein </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront-Abo</p></td>
   <td>
<p>Alle</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront-Lizenz*</p></td>
   <td>
   <p>Neu: Standard</p>
   Oder
   <p>Aktuell: Plan </p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>Konfigurationen auf Zugriffsebene</p></td>
   <td> Es gibt keine Zugriffskontrollen für die Adobe Workfront-Planung</p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Berechtigungen</p></td>
   <td> <p>Berechtigungen für eine Ansicht verwalten</p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Layout-Vorlage</p></td>
   <td> <p>Allen Benutzern, einschließlich Workfront-Administratoren, muss eine Layoutvorlage zugewiesen werden, die den Planungsbereich im Hauptmenü enthält. </p> <p>Weitere Informationen finden Sie unter <a href="/help/quicksilver/planning/access/access-overview.md">Zugriffsübersicht</a>. </p> 
</td>
  </tr>
 </tbody>
</table>

*Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Überlegungen beim Freigeben von Ansichten

* Sie können internen Workfront-Benutzern Ansichts- oder Verwaltungsberechtigungen für eine Ansicht erteilen.

* Benutzer mit Verwaltungsberechtigungen können die Ansichtseinstellungen ändern, freigeben, duplizieren oder löschen.

* Sie können Ansichten für Personen außerhalb Ihres Unternehmens über einen öffentlichen Link freigeben.

* Wenn Sie eine Ansicht öffentlich freigeben, steht der Link für eine begrenzte Zeit für jedermann außerhalb Ihres Unternehmens zur Verfügung, angegeben durch das Ablaufdatum. Zum Anzeigen der freigegebenen Tabellenansicht ist keine Anmeldung erforderlich.

* Personen außerhalb Ihrer Organisation, die Zugriff auf eine Ansicht haben, können keine anderen Ansichten erstellen, die freigegebene Ansicht bearbeiten oder Datensatzinformationen in der Tabelle hinzufügen, löschen oder bearbeiten.

## Berechtigungen intern für eine Ansicht freigeben

Sie können von Ihnen erstellte Ansichten oder Ansichten, für die Sie über Verwaltungsberechtigungen verfügen, in Workfront für Benutzer oder Gruppen freigeben.

>[!NOTE]
>
>Systemadministratoren können keine Ansichten anzeigen oder freigeben, die sie selbst nicht erstellt haben. Sie können nur auf Ansichten zugreifen oder diese freigeben, die für sie freigegeben sind.
>
>Systemadministratoren können nur über Verwaltungsberechtigungen für eine Ansicht verfügen.

{{step1-to-planning}}

1. Öffnen Sie den Arbeitsbereich, dessen Ansicht Sie freigeben möchten, und klicken Sie dann auf eine Karte vom Typ Datensatz.

   Dadurch wird die Seite mit dem Datensatztyp geöffnet.

1. Bewegen Sie auf der Registerkarte &quot;Ansicht&quot;den Mauszeiger über die Ansicht, die Sie freigeben möchten, und klicken Sie auf das Menü **Mehr** Menü ![](assets/more-menu.png) rechts neben dem Ansichtsnamen und klicken Sie dann auf **Freigeben** .

   ![](assets/more-menu-for-views-expanded-with-share-option.png)

   Die Registerkarte **Interne Freigabe** sollte standardmäßig ausgewählt sein.

1. (Optional) Wählen Sie im Bereich **Wer Zugriff hat** aus den folgenden Optionen aus:

   * **Nur eingeladene Personen können auf** zugreifen: Sie müssen Benutzer oder Gruppen angeben, für die Sie die Ansicht freigeben möchten. Dies ist die Standardoption.
   * **Alle Benutzer im Arbeitsbereich können anzeigen**: Alle Benutzer mit der Berechtigung &quot;Ansicht&quot;oder höher für Arbeitsbereiche können auf die Ansicht zugreifen.

1. Geben Sie im Feld **Gewähren des Ansichtszugriffs auf** den Namen eines Benutzers oder einer Gruppe ein und klicken Sie dann auf diesen, wenn er in der Liste angezeigt wird.

   ![](assets/sharing-a-view-ui-with-groups.png)

1. Wählen Sie eine der folgenden Berechtigungsebenen aus dem Dropdown-Menü aus:
   * Anzeigen
   * Verwalten

     Informationen zu Berechtigungsebenen und zu den Aktionen, die Benutzer für die einzelnen Ebenen ausführen können, finden Sie unter [Übersicht über die Berechtigungen für die Freigabe in der Adobe Workfront-Planung](/help/quicksilver/planning/access/sharing-permissions-overview.md).

     Systemadministratoren erhalten immer Berechtigungen zum Verwalten von Ansichten, die für sie freigegeben sind.

1. Klicken Sie auf **Link kopieren** , um einen Link in die Ansicht in die Zwischenablage zu kopieren.
1. Geben Sie den kopierten Link für andere frei. Benutzer, die den Link erhalten, müssen aktive Benutzer sein und sich bei Workfront anmelden, um auf die Seite vom Typ Datensatz zugreifen und sie in der ausgewählten Ansicht anzeigen zu können.
1. Klicken Sie auf **Speichern**.

   >[!TIP]
   >
   >   Für Sie freigegebene Ansichten haben neben dem Ansichtssymbol einen Personenindikator ![](assets/view-shared-with-others-people-icon.png). Ansichten ohne Personen-Indikator sind Ansichten, die Sie erstellt haben.

## Berechtigungen öffentlich für eine Ansicht freigeben

Sie können von Ihnen erstellte Ansichten oder Ansichten, für die Sie über Verwaltungsberechtigungen verfügen, für Personen freigeben, die keine Workfront-Lizenz besitzen und die möglicherweise nicht zu Ihrem Unternehmen gehören.

So geben Sie eine Ansicht in der Workfront-Planung öffentlich frei:

{{step1-to-planning}}

1. Öffnen Sie den Arbeitsbereich, dessen Ansicht Sie freigeben möchten, und klicken Sie dann auf eine Karte vom Typ Datensatz.

   Dadurch wird die Seite mit dem Datensatztyp geöffnet.

1. Bewegen Sie auf der Registerkarte &quot;Ansicht&quot;den Mauszeiger über die Ansicht, die Sie freigeben möchten, und klicken Sie auf das Menü **Mehr** Menü ![](assets/more-menu.png) rechts neben dem Ansichtsnamen und klicken Sie dann auf **Freigeben** .

   ![](assets/more-menu-for-views-expanded-with-share-option.png)

1. Klicken Sie auf **Öffentliche Freigabe**.

   ![](assets/public-sharing-tab-for-views.png)

1. Aktivieren Sie die Einstellung **Öffentlichen Link erstellen** .

   Ein Link wird verfügbar. Dies ist ein öffentlicher Link. Bei der Freigabe kann jeder, der über den Link verfügt, einschließlich Personen außerhalb Ihrer Organisation, auf die Seite mit dem Datensatztyp zugreifen und Datensätze und Felder auf der Seite anzeigen.

1. Klicken Sie auf das Symbol **Link kopieren** ![](assets/copy-link-view.png) , um den Link in die Zwischenablage zu kopieren.

1. Geben Sie manuell ein Datum ein oder verwenden Sie den Kalender im Feld **Ablaufdatum des Links** , um ein Ablaufdatum für den öffentlichen Link auszuwählen. Nach dem ausgewählten Datum ist die Ansicht der Datensatzseite nicht mehr verfügbar.

1. Klicken Sie auf **Speichern**.

   Das Ansichtssymbol wird aktualisiert und zeigt an, dass die Ansicht öffentlich freigegeben ist.

   ![](assets/public-shared-view-icon-highlighted.png)

1. (Optional) Fügen Sie den kopierten Link in eine E-Mail, eine Chat-Nachricht, ein Dokument oder einen Workfront-Kommentar ein, um ihn für andere freizugeben.

## Berechtigungen für eine Ansicht entfernen

{{step1-to-planning}}

1. Öffnen Sie den Arbeitsbereich, dessen Ansicht Sie die Freigabe stoppen möchten, und klicken Sie dann auf eine Karte vom Typ Datensatz. Dadurch wird die Seite mit dem Datensatztyp geöffnet.
1. Bewegen Sie den Mauszeiger über den Registerkartennamen der Ansicht, von der Sie die Freigabe entfernen möchten, und klicken Sie auf das Menü **Mehr** ![](assets/more-menu.png) und klicken Sie dann auf **Freigeben**.
1. Gehen Sie wie folgt vor, um die interne Freigabe einer Ansicht zu entfernen:

   1. Stellen Sie sicher, dass die Registerkarte **Interne Freigabe** ausgewählt ist.
   1. Suchen Sie den Benutzer oder die Gruppe, was Sie entfernen möchten, erweitern Sie das Dropdown-Menü für Berechtigungen rechts neben dem Namen des Benutzers oder der Gruppe und klicken Sie dann auf **Entfernen**.

1. Gehen Sie wie folgt vor, um die öffentliche Freigabe einer Ansicht zu entfernen:

   1. Klicken Sie auf die Registerkarte **Öffentliche Freigabe**.
   1. Deaktivieren Sie die Option **Öffentlichen Link erstellen** .

1. Klicken Sie auf **Speichern**.

   Benutzer haben keinen Zugriff mehr auf die Ansicht. Es gibt keine Benachrichtigung für Benutzer, die nicht mehr auf die Ansicht zugreifen können, dass sie diesen Zugriff nicht mehr haben.