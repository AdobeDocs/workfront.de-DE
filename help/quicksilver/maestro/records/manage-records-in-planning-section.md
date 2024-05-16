---
title: Verwalten von Datensätzen im Bereich "Planung"von Adobe Workfront-Objekten
description: Sie können die mit Adobe Workfront-Objekten verbundenen Datensätze im Abschnitt Planung eines Workfront-Objekts im linken Bereich anzeigen.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: 4d76ef1b34d484e3da2af94543a5fd660ad0a4ef
workflow-type: tm+mt
source-wordcount: '652'
ht-degree: 1%

---

<!--add this to the main TOC and the mini TOC-->

<!--update the metadata with real information when making this available in TOC and in the left nav-->

<!--add also Group and Company when they are available-->


# Verwalten von Datensätzen im Bereich &quot;Planung&quot;von Adobe Workfront-Objekten

{{maestro-important-intro}}

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
<p>Ihr Unternehmen muss am Betaprogramm für die Adobe Workfront-Planung teilnehmen. Wenden Sie sich an Ihren Kundenbetreuer, um sich über dieses neue Angebot zu informieren. </p>
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
   <p>In der Workfront-Planung können Sie Berechtigungen für einen Arbeitsbereich anzeigen oder höher anzeigen</a> </p>  
   <p>Systemadministratoren haben Berechtigungen für alle Arbeitsbereiche der Workfront-Planung, einschließlich derjenigen, die sie nicht erstellt haben</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Layout-Vorlage</p></td>
   <td> <p>Ihr Workfront- oder Gruppenadministrator muss den Planungsbereich im Hauptmenü und den Planungsabschnitt im linken Bereich zu Ihrer Layoutvorlage hinzufügen. Weitere Informationen finden Sie unter <a href="../access/access-overview.md">Zugriffsübersicht</a>. </p>  
</td>
  </tr>

</tbody>
</table>

*Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Überlegungen zum Abschnitt &quot;Planung&quot;von Workfront-Objekten

* Zunächst müssen Sie Datensatztypen mit Workfront-Objekttypen und Datensätze mit Workfront-Objekten verbinden, um sie in Workfront anzuzeigen.

  Weitere Informationen finden Sie in den folgenden Artikeln:

   * [Datensatztypen verbinden](/help/quicksilver/maestro/architecture/connect-record-types.md)
   * [Datensätze verbinden](/help/quicksilver/maestro/records/connect-records.md)
* Sie können den Abschnitt Planung in einem Workfront-Objekt anzeigen, auch wenn dem Workfront-Objekt keine Datensätze zugeordnet sind.
* Sie können über Workfront im Bereich Planung Datensätze mit Workfront-Objekten verbinden.

## Verwalten von Datensätzen im Abschnitt &quot;Planung&quot;

{{step1-to-maestro}}

Der zuletzt aufgerufene Arbeitsbereich wird standardmäßig geöffnet.

1. Klicken Sie auf die Karte eines Datensatztyps, der mit einem Workfront-Projekt, -Portfolio oder -Programm verbunden ist.
1. Wählen Sie eine Tabellenansicht aus dem **Ansicht** Dropdown-Menü.
1. (Bedingt) Wechseln Sie zum Feld für den verbundenen Datensatz in der Tabelle und fügen Sie ein Workfront-Objekt hinzu. Klicken Sie dann im Feld auf den Namen des Workfront-Objekts. Weitere Informationen finden Sie unter [Datensätze verbinden](/help/quicksilver/maestro/records/connect-records.md).
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
1. (Optional) Klicken Sie auf die **In neuer Registerkarte öffnen** icon ![](assets/open-details-in-a-new-tab-icon.png) in der rechten oberen Ecke des Vorschaufelds, um die Detailseite des Datensatzes zu öffnen.
1. Bewegen Sie den Mauszeiger über eine Datensatzkarte und klicken Sie dann auf das Symbol zum Trennen des Datensatzes **-** Klicken Sie auf **Trennen**.
Folgendes geschieht:
   * Der Datensatz ist nicht mehr mit dem Workfront-Objekt verbunden.
   * Das Workfront-Objekt wird auch aus dem verbundenen Feld des Datensatzes aus der Workfront-Planung entfernt.
   * Die Werte für die mit dem Planungsdatensatz verbundenen Workfront-Felder werden ebenfalls gelöscht.
1. Klicks **Verbinden** , um weitere Datensätze zu verbinden.

   <!--checking with the team on the below note - not sure if if should stay Manage or Contribute - Lilit said Contribute??-->

   >[!NOTE]
   >
   >   Die Schaltfläche Verbinden wird nur für die Arbeitsbereiche angezeigt, für die Sie Beitragsberechtigungen haben.

1. Klicken Sie auf die Datensätze, die Sie verbinden möchten. Folgendes geschieht:

   * Die Datensätze sind sofort mit dem Workfront-Objekt verbunden und werden im Abschnitt Planung angezeigt.
   * Das Workfront-Objekt wird dem Verbindungsfeld des Workfront-Planungsdatensatzes hinzugefügt.
   * Die Werte für die mit dem Planungsdatensatz verbundenen Workfront-Felder werden in der Workfront-Planung ausgefüllt.

<!--add more steps here for what happens after clicking Connect-->


