---
title: Datensätze verbinden
description: Nachdem Sie Verbindungen zwischen Datensatztypen hergestellt haben, können Sie einzelne Datensätze miteinander verbinden.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 17796cdc-6de8-4209-a5af-b255dc64d70a
source-git-commit: c39782606358fbb9983b23421588e392dd12ae8a
workflow-type: tm+mt
source-wordcount: '1833'
ht-degree: 0%

---

<!--when you make this live, update the metadata above to this: 
---
title: Connect records and objects
description: In addition to connecting Maestro records to one another, you can also connect Maestro records to objects from other applications.  
topic: Architecture
role: User
hidefromtoc: yes
hide: yes
---
-->
<!--udpate the metadata with real information when making this available in TOC and in the left nav-->

<!--if you change steps here, also update steps in the "Connect records" article-->

# Datensätze verbinden

>[!IMPORTANT]
>
>Die Informationen in diesem Artikel beziehen sich auf Adobe Maestro, ein neues Angebot von Adobe.
>
>Derzeit ist Adobe Maestro Teil eines Betaprogramms, das für eine begrenzte Anzahl von Kunden geöffnet ist.
>
>Wenden Sie sich an Ihren Kundenbetreuer, um weitere Informationen zum Betaprogramm für Maestro zu erhalten.
>
>Weitere Informationen finden Sie unter [Übersicht über Adobe Maestro](../maestro-overview.md).

Sie können Adobe Maestro-Datensätze miteinander oder mit Objekten aus anderen Anwendungen verbinden.

Sie müssen zunächst zwei Datensatztypen oder einen Datensatztyp mit einem Objekttyp aus einer anderen Anwendung verbinden. Anschließend können Sie über die Tabellenansicht des Datensatztyps Datensätze miteinander oder Datensätze mit anderen Objekten verbinden.

Informationen zum Verbinden von Datensatztypen untereinander oder mit Objekttypen aus anderen Anwendungen finden Sie unter [Datensatztypen verbinden](../architecture-and-fields/connect-record-types.md).

Ein Beispiel für das Verbinden von Datensatztypen finden Sie unter [Beispiel für das Verbinden von Datensatztypen und Datensätzen](../architecture-and-fields/example-connect-record-types-and-records.md).

Sie können Folgendes verbinden:

* Betriebsaufzeichnungen von Maestro
* Maestro-Betriebsaufzeichnungen für Taxonomiedatensätze
* Maestro-Betriebsaufzeichnungen und -objekte aus anderen Anwendungen.

  Die folgenden Anwendungen und Objekttypen werden derzeit unterstützt:

   * Adobe Workfront

      * Projekte
      * Portfolios
      * Programme
      * Firma
      * Gruppe

  <!--when you add more objects, fix the Access Requirements below which right now refer only to projects-->

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto">
 <col>
<tbody>
<td>
   <p> Adobe</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront-Abkommen</p></td>
   <td>
<p>Ihr Unternehmen muss am Adobe Maestro Closed-Beta-Programm teilnehmen. Wenden Sie sich an Ihren Kundenbetreuer, um sich über dieses neue Angebot zu informieren. </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront-Abo</p></td>
   <td>
<p>Beliebig</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront-Lizenz</p></td>
   <td><p>Alle zum Erstellen von Maestro-Datensätzen</p> 
<p>Arbeiten oder höher zur Anzeige von Projekten in Workfront</p>
  <p>Weitere Informationen finden Sie unter <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md">Übersicht über Adobe Workfront-Lizenzen</a>.</p> 
  </td>
  </tr>
  <tr>
   <td role="rowheader">Zugriffsebene</td>
   <td> <p>Alle zum Erstellen von Maestro-Datensätzen</p>
<p>Anzeigen oder Verbessern des Zugriffs auf Projekte, Portfolios, Programme</p> 
<p>Zusätzlicher Zugriff auf Gruppen und Unternehmen, wenn Benutzer Gruppen oder Unternehmen anzeigen, gehören sie nicht zu</p>   
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Objektberechtigungen</p></td>
   <td> <p>Anzeigen oder höherer Berechtigungen für Objekte, die Sie mit Maestro-Datensätzen verknüpfen möchten  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Layout-Vorlage</p></td>
   <td> <p>Ihr Systemadministrator muss den Maestro-Bereich in Ihre Layoutvorlage einfügen. Weitere Informationen finden Sie unter <a href="../access/grant-access.md">Zugriff auf Adobe Maestro gewähren</a>. </p></td>
  </tr>
 </tbody>
</table>

<!--Maybe enable this at GA - but Maestro is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->

<!-- Notes for the table: for the "Workfront access" row: <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p>-->

## Datensätze verbinden

### Überlegungen zum Verbinden von Datensätzen

* Nachdem die Verbindung zwischen Datensatztypen hergestellt wurde, werden die verbundenen Datensatztypen in der Tabelle der Datensatztypen, aus denen sie verknüpft sind, als verknüpfte Datensatzfelder angezeigt.
* Sie können Datensätze und Objekte der verknüpften Datensätze und Objekttypen aus den verknüpften Datensatzfeldern durchsuchen und hinzufügen.
* Sie können der Tabelle des Datensatztyps, von dem Sie die Relation herstellen, Felder aus den verknüpften Datensatztypen hinzufügen.
* Die Werte verknüpfter Felder in den Datensätzen, aus denen Sie die Relation herstellen, können nicht manuell aktualisiert werden.

  Die Werte der verknüpften Felder aus den verknüpften Datensätzen füllen den Maestro-Datensatz, von dem Sie die Verknüpfung automatisch vornehmen.

* Jeder mit Zugriff auf Maestro kann die Verbindungen sehen, die Sie zwischen Maestro-Datensätzen oder zwischen Maestro-Datensätzen und Workfront-Objekten herstellen. Außerdem können Sie die Verbindungen aller anderen anzeigen und bearbeiten. <!--add that this is based on your permissions in both Maestro and Workfront (or, later, any other application)-->
* Sie können einen Maestro-Datensatz mit einem oder mehreren Objekten aus einer anderen Anwendung verbinden.
* Sie können keine Taxonomien mit Datensatztypen oder Objekten aus einer anderen Anwendung verbinden. <!-- this is temporary; there will be certain objects (teams, etc) that will be linked to taxonomies, per Lilit-->
* Derzeit können Sie Maestro-Datensätze nur mit Workfront-Objekten verknüpfen. Um Maestro-Datensätze mit Workfront-Objekten zu verknüpfen, benötigen Sie Folgendes:

   * Workfront-Objekte. Beispielsweise müssen Sie in Workfront zunächst Projekte, Portfolios, Programme, Unternehmen oder Gruppen erstellen.
   * Maestro-Arbeitsbereiche, Datensatztypen und Datensätze. Weitere Informationen finden Sie in den folgenden Artikeln:

      * [Erstellen von Arbeitsbereichen](../architecture-and-fields/create-workspaces.md)
      * [Erstellen von Datensatztypen](../architecture-and-fields/create-record-types.md)
      * [Datensätze erstellen](../records/create-records.md)

   * Verbindungen zwischen Datensatztypen oder zwischen Datensatztypen und Objekten aus anderen Anwendungen. Weitere Informationen finden Sie unter [Datensatztypen verbinden](../architecture-and-fields/connect-record-types.md).

### Maestro-Datensätze verbinden

1. Klicken Sie auf **Hauptmenü** icon ![](assets/main-menu-workfront.png) in der oberen rechten Ecke von Workfront, <!---or the **Main menu** icon ![](assets/main-menu-shell.png)  in the upper-left corner, if available--> Klicken Sie dann auf **Maestro** ![](assets/maestro-icon.png).

   Der zuletzt aufgerufene Arbeitsbereich sollte standardmäßig geöffnet werden.

1. (Optional) Erweitern Sie den nach unten zeigenden Pfeil rechts neben einem vorhandenen Workspace-Namen und wählen Sie den Arbeitsbereich aus, aus dem Sie Datensätze verbinden möchten.
1. Klicken Sie auf die Karte eines Datensatztyps, um die Seite vom Typ Datensatz zu öffnen.
1. Wählen Sie eine Tabellenansicht aus dem **Ansicht** Dropdown-Menü in der oberen rechten Ecke der Seite vom Typ Datensatz.
1. Fügen Sie eine Verbindung zu einem anderen Datensatz oder Objekttyp aus dem ausgewählten Datensatztyp hinzu. Weitere Informationen finden Sie unter [Datensatztypen verbinden](../architecture-and-fields/connect-record-types.md).

Der Tabelle wird eine neue Spalte hinzugefügt, um den verknüpften Datensatztyp anzuzeigen.

1. Fügen Sie dem ausgewählten Datensatztyp durch Hinzufügen einer neuen Zeile zur Tabelle Datensätze hinzu. Weitere Informationen finden Sie unter [Datensätze erstellen](../../maestro/records/create-records.md).
1. Wechseln Sie aus einem Datensatz, der in der Tabellenansicht aufgeführt ist, zur verknüpften Datensatzspalte und bewegen Sie den Mauszeiger über die Zelle, die dem Datensatz entspricht, den Sie mit anderen Maestro-Datensätzen verknüpfen möchten, und klicken Sie dann auf die Schaltfläche **+** Symbol.

   Die **Objekte verbinden** angezeigt.

   ![](assets/connected-objects-table-for-records.png)

1. Geben Sie den Namen eines Datensatzes in das Suchfeld ein und wählen Sie ihn aus, wenn er in der Liste angezeigt wird

   Oder

   Wählen Sie den Namen eines oder mehrerer Datensätze im Feld aus und klicken Sie auf **Objekte verbinden** in der oberen rechten Ecke des Felds &quot;Objekte verbinden&quot;ein.

   Folgendes wird hinzugefügt:

   * Die verknüpften Datensätze werden im verknüpften Datensatzfeld des Datensatzes angezeigt, den Sie in Schritt 3 ausgewählt haben. Durch die Aktualisierung der verknüpften Datensätze werden automatisch die verknüpften Datensatzfelder für die Datensätze aktualisiert, von denen Sie die Relation herstellen. <!--ensure the number of the step stays accurate-->
   * Die verknüpften Felder, die zu den verknüpften Datensätzen gehören, werden automatisch mit den Informationen aus den ursprünglich verknüpften Datensätzen ausgefüllt. Verknüpfte Felder können nicht manuell bearbeitet werden.

     >[!TIP]
     >
     >* &quot;Verknüpfte Felder&quot;und &quot;Suchfelder&quot;werden synonym verwendet.
     >
     >* Wenn Sie die Einstellung Mehrere Datensätze zulassen aktiviert haben, wenn Sie die Datensatztypen verbunden haben, werden die Feldwerte für die verschiedenen ausgewählten Objekte entweder durch Kommas getrennt oder gemäß dem ausgewählten Aggregator aggregiert.

1. (Optional) Schließen Sie die Maestro-Datensatztyp-Seite und wechseln Sie zum ausgewählten Arbeitsbereich.
1. Klicken Sie auf die Karte des Datensatztyps, mit dem Sie verknüpft sind.

   Wenn Sie beispielsweise den Campaign-Datensatz mit dem Produktdatensatz verbunden haben, klicken Sie auf die **Produkt** Karte.

   Die Karte vom Typ Datensatz sollte in der Tabellenansicht geöffnet werden.

   Beachten Sie, dass im Feld Kampagnenverknüpfter Datensatz die Namen der Kampagnen angezeigt werden, die Sie mit Produkten verknüpft haben, und zwar auf der Seite Produktdatensatz . Durch die Aktualisierung der Campaign-Informationen wird das Campaign-verknüpfte Datensatzfeld für den Produktdatensatz-Typ automatisch aktualisiert.

### Maestro-Datensätze mit Workfront-Objekten verbinden

<!--when we will have more applications to link to from Maestro, change the title to soemthing like: Connect Maestro records to objects from other applications-->

Nachdem Sie eine Verbindung zwischen einem Maestro-Record-Typ und einem Workfront-Objekttyp hergestellt haben, können Sie einzelne Maestro-Datensätze mit Objekten in Workfront verbinden. Sie können auch Felder vom Workfront-Objekt mit dem Maestro-Datensatztyp verbinden.

1. Klicken Sie auf **Hauptmenü** icon ![](assets/main-menu-workfront.png) in der oberen rechten Ecke von Workfront, <!---or the **Main menu** icon ![](assets/main-menu-shell.png)  in the upper-left corner, if available--> Klicken Sie dann auf **Maestro** ![](assets/maestro-icon.png).

   Der zuletzt aufgerufene Arbeitsbereich sollte standardmäßig geöffnet werden.

1. (Optional) Erweitern Sie den nach unten zeigenden Pfeil rechts neben einem vorhandenen Workspace-Namen und wählen Sie den Arbeitsbereich aus, aus dem Sie Datensätze verbinden möchten.
1. Klicken Sie auf die Karte eines Datensatztyps, um die Seite vom Typ Datensatz zu öffnen.
1. Wählen Sie eine Tabellenansicht aus dem **Ansicht** Dropdown-Menü in der oberen rechten Ecke der Seite vom Typ Datensatz.
1. Fügen Sie einem Objekttyp vom ausgewählten Datensatztyp aus eine neue Verbindung hinzu. Wählen Sie unter den folgenden Objekten im Abschnitt Workfront aus:

   * Projekt
   * Portfolio
   * Programm
   * Firma
   * Gruppe

   Weitere Informationen finden Sie unter [Datensatztypen verbinden](../architecture-and-fields/connect-record-types.md).

   Der Tabelle wird eine neue Spalte hinzugefügt, um den verknüpften Objekttyp anzuzeigen.

1. Fügen Sie dem ausgewählten Datensatztyp einzelne Datensätze hinzu, indem Sie der Tabelle eine neue Zeile hinzufügen. Weitere Informationen finden Sie unter [Datensätze erstellen](../../maestro/records/create-records.md).
1. Wechseln Sie aus einem in der Tabellenansicht aufgelisteten Datensatz zur verknüpften Objektspalte und bewegen Sie den Mauszeiger über die Zelle, die dem Datensatz entspricht, den Sie mit anderen Objekten aus Workfront verknüpfen möchten. Klicken Sie dann auf die Schaltfläche **+** Symbol. <!--change Workfront to other applications, when this will be possible-->

   Die **Objekte verbinden** angezeigt.

   ![](assets/connect-objects-box-to-select-projects.png)

1. Geben Sie den Namen eines Workfront-Objekts in das Suchfeld ein und wählen Sie es dann aus, wenn es in der Liste angezeigt wird

   Oder

   Wählen Sie den Namen eines oder mehrerer Objekte im Feld aus und klicken Sie dann auf **Objekte verbinden** in der oberen rechten Ecke des Felds &quot;Objekte verbinden&quot;ein.

   Maestro wird wie folgt ergänzt:

   * Die ausgewählten Workfront-Objekte werden dem verknüpften Datensatzfeld hinzugefügt.
   * Für jedes verknüpfte Feld, das Sie beim Hinzufügen der Felder zum verknüpften Datensatz ausgewählt haben, wird ein neues verknüpftes Feld (oder ein Lookup-Feld) erstellt.
   * Der neue Datensatztyp &quot;Workfront-Objekt&quot;wird im selben Arbeitsbereich wie der Maestro-Datensatz erstellt, von dem Sie die Verknüpfung herstellen. Der Name des Objekts ist Teil des Namens dieses Datensatztyps. Wenn Sie beispielsweise mit Workfront-Projekten verknüpfen, wird der Workfront-Projektarchatyp in Maestro erstellt.

     Dies ist ein schreibgeschützter Datensatztyp und zeigt Workfront-Objekte an, die in dem neuen verknüpften Objektfeld ausgewählt sind, das Sie aus dem Maestro-Datensatz erstellt haben. Die verknüpften Felder des verknüpften Objekts werden auch in den schreibgeschützten verknüpften Workfront-Datensätzen angezeigt.

     >[!IMPORTANT]
     >
     > Der schreibgeschützte Workfront-Objektdatensatz wird nur erstellt, wenn einzelne Projekte zu Maestro-Datensätzen hinzugefügt werden. Beim Erstellen einer Verbindung zwischen einem Maestro-Record-Typ und einem Workfront-Objekttyp wird der Workfront-Record-Typ nicht erstellt.

     Alle vorhandenen Informationen aus den Feldern der Workfront-Objekte werden in den verknüpften Feldern oder Suchfeldern angezeigt.

     >[!TIP]
     >
     >
     >* Wenn Sie die Einstellung Mehrere Datensätze zulassen aktiviert haben, werden die Werte der verschiedenen Objekte entweder durch Kommas getrennt oder nach dem von Ihnen ausgewählten Aggregator aggregiert.
     >
     >* Für die verknüpften Workfront-Objekte wird kein verknüpftes Datensatzfeld mit den verknüpften Maestro-Datensätzen erstellt.


1. (Optional) Schließen Sie die Maestro-Datensatztyp-Seite und wechseln Sie zum ausgewählten Arbeitsbereich.
1. Klicken Sie auf die Karte für den Workfront-Objektdatensatztyp. Klicken Sie beispielsweise auf die **Workfront-Projekt** -Karte, wenn Sie mit Workfront-Projekten verknüpft sind. Die schreibgeschützte Workfront-Datensatztypkarte sollte in der Tabellenansicht geöffnet werden.

   >[!NOTE]
   >
   >    * Die auf der Seite Workfront-Datensatztyp aufgelisteten Datensätze sind schreibgeschützte Workfront-Objekte. Die vom Workfront-Datensatztyp verknüpften Felder werden ebenfalls als schreibgeschützte Spalten angezeigt und automatisch ausgefüllt, wenn sie in Workfront ausgefüllt werden.
   >    * Workfront-Felder können in Maestro nicht manuell aktualisiert werden. Workfront-Objektfelder müssen in Workfront ausgefüllt und die Feldwerte werden automatisch im Workfront-Datensatz in Maestro angezeigt.
   >
   >    * Um den Workfront-Objektdatensatz-Typ in der Timeline-Ansicht anzuzeigen, müssen Sie mindestens zwei Datumsfelder in der Tabellenansicht der schreibgeschützten Workfront-Datensatztypseite anzeigen.

1. (Optional) Klicken Sie auf die **Mehr** Menü ![](assets/more-menu.png) neben dem Workfront-Objekt-Datensatztyp-Namen in der Kopfzeile der Seite, und klicken Sie auf **Umbenennen** , um den Namen des Datensatzes zu bearbeiten.

   >[!NOTE]
   >
   >    Sie können einen verknüpften Workfront-Record-Typ oder andere Objekte nicht von der Workfront-Record-Type-Seite löschen.

1. (Optional) Klicken Sie auf die **Felder hinzufügen** icon ![](assets/add-fields-icon.png) in der rechten oberen Ecke der Tabellenansicht auf der Workfront-Datensatztypseite, um Workfront-Felder zum Workfront-Datensatztyp hinzuzufügen oder daraus zu entfernen.

   >[!NOTE]
   >
   >  Die Felder, die Sie auf der Seite &quot;Workfront-Objektdatensatz&quot;hinzufügen oder entfernen, werden nicht zum Maestro-Datensatztyp hinzugefügt oder entfernt, der mit dem Workfront-Objekttyp verknüpft ist. Die Felder sind nur auf der schreibgeschützten Workfront-Datensatztypseite sichtbar, sodass Sie sie in Maestro überprüfen können.

1. (Optional und bedingt) Wenn Sie dem Workfront-Objekt mindestens zwei Datumsfelder hinzugefügt haben, klicken Sie auf die Schaltfläche **Ansicht** Dropdown-Menü auf der Seite Workfront-Objektdatensatztyp auswählen und **Timeline** anzeigen. Die mit Workfront verknüpften Objekte werden in der Timeline-Ansicht angezeigt.
