---
title: Verwalten von Datensätzen im Bereich "Planung"von Adobe Workfront-Objekten
description: Sie können die mit Adobe Workfront-Objekten verbundenen Datensätze im Abschnitt Planung eines Workfront-Objekts im linken Bereich anzeigen.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: d86cf3f9-cacc-4457-acb3-a5122ae91be8
source-git-commit: 64f187ed78b69db9b9ac0259e96ef0bf47abf4f4
workflow-type: tm+mt
source-wordcount: '676'
ht-degree: 1%

---

<!--update the metadata with real information when making this available in TOC and in the left nav-->

<!--add also Group and Company when they are available-->

<!-- opening the Details preview and page is not possible yet - hid those steps, but add them when released-->


# Verwalten von Datensätzen im Bereich &quot;Planung&quot;von Adobe Workfront-Objekten

{{planning-important-intro}}

Sie können die mit Adobe Workfront-Objekten verbundenen Datensätze im Abschnitt Planung eines Workfront-Objekts im linken Bereich anzeigen.

Der Abschnitt Planung ist für die folgenden Workfront-Objekte verfügbar:

* Projekt
* Portfolio
* Programm
<!--* Group
* Company-->

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

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
   <p>Aktuell: Plan</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>Konfigurationen auf Zugriffsebene</p></td>
   <td> <p>Anzeigen oder Aufrufen von Projekten, Programmen und Portfolios</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Berechtigungen</p></td>
   <td> <p>Zeigen Sie in Workfront die Berechtigungen für ein Projekt, ein Portfolio oder ein Programm an oder höher</a> </p> 
   <p>In der Workfront-Planung Contribute oder höhere Berechtigungen für einen Arbeitsbereich</a> </p>  
   <p>Systemadministratoren haben Berechtigungen für alle Arbeitsbereiche der Workfront-Planung, einschließlich derjenigen, die sie nicht erstellt haben</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Layout-Vorlage</p></td>
   <td> <p>Ihr Workfront- oder Gruppenadministrator muss den Planungsbereich im Hauptmenü und den Planungsabschnitt im linken Bereich zu Ihrer Layoutvorlage hinzufügen. Weitere Informationen finden Sie unter <a href="/help/quicksilver/planning/access/access-overview.md">Zugriffsübersicht</a>. </p>  
</td>
  </tr>

</tbody>
</table>

*Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Überlegungen zum Abschnitt &quot;Planung&quot;von Workfront-Objekten

* Zunächst müssen Sie Datensatztypen mit Workfront-Objekttypen und Datensätze mit Workfront-Objekten verbinden, um sie in Workfront anzuzeigen.

  Weitere Informationen finden Sie in den folgenden Artikeln:

   * [Datensatztypen verbinden](/help/quicksilver/planning/architecture/connect-record-types.md)
   * [Datensätze verbinden](/help/quicksilver/planning/records/connect-records.md)
* Sie können den Abschnitt Planung in einem Workfront-Objekt anzeigen, auch wenn dem Workfront-Objekt keine Datensätze zugeordnet sind.
* Sie können über Workfront im Bereich Planung Datensätze mit Workfront-Objekten verbinden, wenn mit dem Workfront-Objekt mindestens ein Datensatz verbunden ist.

## Verwalten von Datensätzen im Abschnitt &quot;Planung&quot;

{{step1-to-planning}}

1. Klicken Sie auf die Karte eines Arbeitsbereichs.

   Der Arbeitsbereich wird geöffnet und die Datensatztypen werden als Karten angezeigt.

1. Klicken Sie auf die Karte eines Datensatztyps, der mit einem Workfront-Projekt, -Portfolio oder -Programm verbunden ist.
1. Wechseln Sie zu einem verbundenen Datensatzfeld, das über eine Verbindung mit einem Workfront-Objekt verfügt, entweder in der Tabellenansicht oder auf der Detailseite eines Datensatzes. Weitere Informationen finden Sie unter [Datensätze verbinden](/help/quicksilver/planning/records/connect-records.md).
1. Klicken Sie im Feld &quot;Verbundener Datensatz&quot;auf den Namen eines Workfront-Objekts.
Die Seite der Objekte wird in der Workfront-Planung geöffnet.
1. Klicks **Zu Quelle wechseln** in der oberen rechten Ecke des Bildschirms.

   Die Seite des Objekts wird in Workfront geöffnet.
1. Klicks **Planung** im linken Bereich.

   >[!NOTE]
   >
   >   Ihr Workfront- oder Gruppenadministrator muss den Planungsabschnitt zu Ihrer Layoutvorlage hinzufügen, bevor er für ein Worfront-Projekt, ein -Portfolio oder ein Programm angezeigt wird.

   Der Abschnitt Planung wird mit den folgenden Informationen angezeigt:

   * Die verbundenen Datensätze werden auf einzelnen Karten angezeigt, die die folgenden Informationen enthalten:
      * Name des Datensatzes
      * Die Miniaturansicht des Datensatzes
      * Der Name des verbundenen Datensatzfelds, wie er in der Workfront-Planung angezeigt wird.
   * Datensätze werden in ihrem jeweiligen Arbeitsbereich angezeigt.

   ![](assets/planning-section-on-project.png)

1. Klicken Sie auf eine Datensatzkarte, um weitere Informationen zum Datensatz anzuzeigen. Das Vorschaufeld für Datensätze wird angezeigt.
1. (Optional) Beginnen Sie mit der Änderung der Felder im Vorschaufeld des Datensatzes. Ihre Änderungen werden automatisch gespeichert.
1. (Optional) Klicken Sie auf die **In neuer Registerkarte öffnen** icon ![](assets/open-details-in-a-new-tab-icon.png) in der rechten oberen Ecke des Vorschaufelds, um die Detailseite des Datensatzes zu öffnen. Die Detailseite des Datensatzes wird in der Workfront-Planung geöffnet.
1. Bewegen Sie den Mauszeiger über eine Datensatzkarte und klicken Sie dann auf das Symbol zum Trennen des Datensatzes **-** Klicken Sie auf **Trennen**.
Folgendes geschieht:
   * Der Datensatz ist nicht mehr mit dem Workfront-Objekt verbunden.
   * Das Workfront-Objekt wird auch aus dem verbundenen Feld des Datensatzes aus der Workfront-Planung entfernt.
   * Die Werte für die Workfront-Suchfelder, die mit dem Planungsdatensatz verbunden sind, werden ebenfalls gelöscht.
1. Klicks **Verbinden** , um weitere Datensätze zu verbinden.

   >[!NOTE]
   >
   >   Die Schaltfläche Verbinden wird nur für die Arbeitsbereiche angezeigt, für die Sie über Contribute-Berechtigungen verfügen. <!--they might replace this with one button at the top of the page. Rephrase-->

1. Klicken Sie auf die Datensätze, die Sie verbinden möchten. Folgendes geschieht:

   * Die Datensätze sind sofort mit dem Workfront-Objekt verbunden und werden im Abschnitt Planung angezeigt.
   * Das Workfront-Objekt wird dem Verbindungsfeld des Workfront-Planungsdatensatzes hinzugefügt.
   * Die Werte für die Workfront-Suchfelder, die mit dem Planungsdatensatz verbunden sind, werden in der Workfront-Planung ausgefüllt.

<!--add more steps here for what happens after clicking Connect-->
