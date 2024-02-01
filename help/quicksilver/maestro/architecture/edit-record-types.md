---
title: Datensatztypen bearbeiten
description: Sie können Datensatztypen nach dem Speichern bearbeiten. Datensatztypen sind die Objekttypen von Adobe Maestro.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 7d6de742-9657-4286-968c-1fc78ebbb94e
source-git-commit: 4016ba2c1b94ba84037612bdc9c1136267513fd5
workflow-type: tm+mt
source-wordcount: '448'
ht-degree: 0%

---

<!--update the metadata with real information when making this available in TOC and in the left nav
---
title: Edit record types
description: You can edit record types after they have been saved. Record types are the objec types of Adobe Maestro.
author: Alina
role: User
feature: Work Management 
topic: Architecture
hidefromtoc: yes
hide: yes
---

-->

# Datensatztypen bearbeiten

{{maestro-important-intro}}

Datensatztypen sind die Objekttypen von Adobe Maestro. Sie können das Erscheinungsbild von Datensatztypen bearbeiten, die Sie oder andere Benutzer erstellt haben. Informationen zum Erstellen von Maestro-Datensatztypen finden Sie unter [Erstellen von Datensatztypen](../architecture/create-record-types.md).

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
   <p> Adobe Workfront</p> <p>Um Maestro-Record-Typen mit Experience Manager Assets zu verbinden, müssen Sie über eine Adobe Experience Manager Assets-Lizenz verfügen und die Workfront-Instanz Ihres Unternehmens muss mit der Adobe Business Platform oder der Adobe Admin Console integriert sein.</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront-Abkommen</p></td>
   <td>
<p>Ihr Unternehmen muss am Adobe Maestro Closed-Beta-Programm teilnehmen. Wenden Sie sich an Ihren Kundenbetreuer, um sich über dieses neue Angebot zu informieren. </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront-Abo</p></td>
   <td>
<p>Alle</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront-Lizenz</p></td>
   <td>
   <p>Alle</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>Konfigurationen auf Zugriffsebene</p></td>
   <td> <p>Es gibt keine Zugriffssteuerungsebenen für Maestro</p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Berechtigungen</p></td>
   <td> <p>Berechtigungen für einen Arbeitsbereich verwalten</a> </p>  
   <p>Systemadministratoren haben Berechtigungen für alle Arbeitsbereiche, einschließlich derjenigen, die sie nicht erstellt haben
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Layout-Vorlage</p></td>
   <td> <p>Ihr Workfront- oder Gruppenadministrator muss den Maestro-Bereich in Ihre Layoutvorlage einfügen. Weitere Informationen finden Sie unter <a href="../access/access-overview.md">Zugriffsübersicht</a>. </p>  
</td>
  </tr>

</tbody>
</table>

<!--Maybe enable this at GA - but Maestro is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

## Datensatztypen bearbeiten

{{step1-to-maestro}}

Der zuletzt aufgerufene Arbeitsbereich sollte standardmäßig geöffnet werden.

1. (Optional) Erweitern Sie den nach unten zeigenden Pfeil rechts neben einem vorhandenen Workspace-Namen und wählen Sie den Arbeitsbereich aus, für den Sie Datensatztypen erstellen möchten.
1. Bewegen Sie den Mauszeiger über die Karte eines Datensatztyps und klicken Sie auf **Mehr** Menü ![](assets/more-menu.png) in der rechten oberen Ecke der Datensatztypkarte klicken Sie auf **Erscheinungsbild aktualisieren**.

   ![](assets/update-appearance-link-from-more-menu-on-record-type-card.png)

1. Aktualisieren Sie im Feld Datensatz-Typ aktualisieren die folgenden Informationen:

   * **Name des Eintrags**: Bearbeiten Sie bei Bedarf den Namen des Datensatztyps. <!--correct this - I asked Garik to change this field to "Record type name"-->
   * **Erscheinungsbild**: Bearbeiten Sie die Farbe und Form des Symbols, das dem Datensatztyp zugeordnet ist. Gehen Sie wie folgt vor:
      * Wählen Sie eine Farbe aus, um den Datensatztyp zu identifizieren. Dies ist die Farbe des Symbols für den Datensatztyp. Graustufen ist standardmäßig ausgewählt.
      * Wählen Sie ein Symbol aus der Liste aus oder geben Sie den Namen eines Symbols ein, um zu beschreiben, was es darstellt, und wählen Sie es dann aus, wenn es angezeigt wird. Dies ist das Symbol des Datensatztyps. Standardmäßig ist ein Dateisymbol ausgewählt.

     ![](assets/update-record-type-box.png)

1. Klicken Sie außerhalb des Felds Datensatz-Typ aktualisieren auf , um Ihre Änderungen zu speichern.
1. (Optional) Klicken Sie im Arbeitsbereich auf die Karte vom Typ Datensatz , um die Seite des Datensatztyps zu öffnen.
1. Klicken Sie auf **Mehr** Menü rechts neben dem Namen des Datensatztyps und klicken Sie auf **Umbenennen** zum Umbenennen des Datensatztyps

   Oder

   Benennen Sie den Datensatztyp in der Kopfzeile um.  <!--check to see if they renamed this to "Rename" - it kept going back and forth between Rename and Edit-->

   ![](assets/more-menu-options-from-record-details-page.png) <!--check this screen shot - not sure this is valid ???-->

   Sie können auch einen Datensatztyp in der Kopfzeile der Seite des Datensatztyps umbenennen.
1. (Optional) Erweitern Sie den nach unten zeigenden Pfeil rechts neben einem Datensatztypnamen und wählen Sie einen anderen zu bearbeitenden Datensatztyp aus.
