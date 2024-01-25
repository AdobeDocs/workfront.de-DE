---
title: Felder bearbeiten
description: In Adobe Maestro können Sie die Feldeinstellungen für bereits erstellte Felder bearbeiten.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 6c35c313-d6ed-428b-b70d-2ea242da4e8f
source-git-commit: c264c0c96b818934a7c25ed54c7666d2d6c95e54
workflow-type: tm+mt
source-wordcount: '528'
ht-degree: 0%

---

<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

<!---
title: Edit foelds
description: In Adobe Maestro, you can edit the field settings for fields that are already created.
hidefromtoc: yes
hide: yes
author: Alina
feature: (*******************WE NEED A NEW ONE*******************)
role: User, Administrator (************is this right???************)
recommendations: noDisplay, noCatalog
--->


# Felder bearbeiten

>[!IMPORTANT]
>
>Die Informationen in diesem Artikel beziehen sich auf Adobe Maestro, ein neues Angebot von Adobe Workfront.
>
>Derzeit ist Adobe Maestro Teil eines Betaprogramms, das für eine begrenzte Anzahl von Kunden geöffnet ist. Sie müssen Workfront-Kunde sein, um Maestro-Funktionen verwenden zu können.
>
>Wenden Sie sich an Ihren Kundenbetreuer, um weitere Informationen zum Betaprogramm für Maestro zu erhalten.
>
>Weitere Informationen finden Sie unter [Übersicht über Adobe Maestro](../maestro-overview.md).

Sie können die Feldeinstellungen für bereits erstellte Felder bearbeiten.

Informationen zum Erstellen von Adobe Maestro-Feldern finden Sie unter [Felder erstellen](../fields/create-fields.md).

Dieser Artikel beschreibt, wie Sie die Einstellungen für Maestro-Felder bearbeiten können. Informationen zum Bearbeiten von Feldwerten für Maestro-Datensätze finden Sie unter [Datensätze bearbeiten](/help/quicksilver/maestro/records/edit-records.md).

## Überlegungen zum Bearbeiten von Feldinformationen

* Sie können von Ihnen erstellte Felder oder von anderen Benutzern erstellte Felder bearbeiten, wenn Sie über Verwaltungsberechtigungen für den Arbeitsbereich verfügen, zu dem die Felder gehören.
* Sie können ein Feld in der Tabelle vom Typ Datensatz bearbeiten.
* Sie können ein Feld nicht auf der Detailseite eines Datensatzes oder in der Timeline-Ansicht bearbeiten.
* Nach dem Speichern des Felds können Sie den Feldtyp nicht mehr bearbeiten.
* Die Auswahl der zuvor ausgewählten Einstellung Negative Zahlen zulassen für ein Feld vom Typ Zahl, Prozentsatz oder Währung kann nicht aufgehoben werden, wenn bereits negative Werte in den Datensätzen gespeichert sind, an die das Feld angehängt ist.
<!--this is not true yet; one piece of it is true and I added it as the bullet above: 
* You cannot edit the options, or the special format of the following fields, after they are saved:

    * Allow negative numbers option from a Number, Percentage, or Currency field. 
    * The Options of a Single-select or a Multi-select field.
-->

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
   <td role="rowheader"><p>Konfiguration der Zugriffsebene</p></td>
   <td> <p>Es gibt keine Zugriffskontrollen für Maestro</p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Berechtigungen</p></td>
   <td> <p>Berechtigungen für einen Arbeitsbereich verwalten</a> </p>  
   <p>Systemadministratoren haben Berechtigungen für alle Arbeitsbereiche, einschließlich derjenigen, die sie nicht erstellt haben</p>
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

## Felder bearbeiten

1. Klicken Sie auf **Hauptmenü** icon ![](assets/main-menu-workfront.png) in der oberen rechten Ecke von Workfront oder **Hauptmenü** icon ![](assets/main-menu-shell.png)  in der oberen linken Ecke, falls verfügbar, klicken Sie auf **Maestro** ![](assets/maestro-icon.png).

   Der zuletzt aufgerufene Arbeitsbereich sollte standardmäßig geöffnet werden.

1. (Optional) Erweitern Sie den nach unten zeigenden Pfeil rechts neben einem vorhandenen Workspace-Namen und wählen Sie den Arbeitsbereich aus, für den Sie Datensatztypen löschen möchten.

   Der Arbeitsbereich wird geöffnet und die damit verbundenen Datensatztypen und Taxonomien werden angezeigt.
1. Klicken Sie auf die Karte für den Datensatztyp oder die Taxonomie, deren Felder Sie bearbeiten möchten.

   Dadurch wird die Seite des Datensatztyps geöffnet.
1. (Bedingt) Wählen Sie eine **Tabellenansicht** aus dem **Ansicht** Dropdown-Menü in der oberen rechten Ecke der Seite vom Typ Datensatz.
1. Bewegen Sie den Mauszeiger über die Spaltenüberschrift eines Felds, das Sie bearbeiten möchten, und klicken Sie dann auf den nach unten zeigenden Pfeil nach dem Feldnamen und klicken Sie dann auf **Feld bearbeiten**

   Oder

   Doppelklicken Sie auf die Spaltenüberschrift für das Feld.

   ![](assets/arrow-menu-after-name-of-field-in-table-header-highlighted.png)

1. Aktualisieren Sie die Informationen über das Feld und klicken Sie auf **Speichern**.

   <!--insert screen shot when finalized-->

   >[!TIP]
   >
   >Nach dem Speichern des Felds kann der Feldtyp nicht mehr aktualisiert werden.


1. (Bedingt) Klicken Sie für verknüpfte Datensatzfelder auf **Suchfelder bearbeiten** und fügen Sie eines der Felder aus dem verknüpften Datensatztyp hinzu oder entfernen Sie es.

   Weitere Informationen finden Sie unter [Datensatztypen verbinden](../architecture/connect-record-types.md).
