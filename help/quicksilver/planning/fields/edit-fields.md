---
title: Felder bearbeiten
description: In der Adobe Workfront-Planung können Sie die Feldeinstellungen für bereits erstellte Felder bearbeiten. In diesem Artikel wird beschrieben, wie Sie die Einstellungen für die Workfront-Planungsfelder bearbeiten können.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 6c35c313-d6ed-428b-b70d-2ea242da4e8f
source-git-commit: 160bcc8796666c9615ebe8ead18813b96be26a71
workflow-type: tm+mt
source-wordcount: '565'
ht-degree: 0%

---

<!--update the metadata with real information when making this available in TOC and in the left nav-->

<!---
title: Edit foelds
description: In Adobe Workfront Planning, you can edit the field settings for fields that are already created.
hidefromtoc: yes
hide: yes
author: Alina
feature: (*******************WE NEED A NEW ONE*******************)
role: User, Administrator (************is this right???************)
recommendations: noDisplay, noCatalog
--->

# Felder bearbeiten

{{planning-important-intro}}

Sie können die Feldeinstellungen für Felder bearbeiten, die bereits in der Adobe Workfront-Planung erstellt wurden.

Informationen zum Erstellen von Adobe Workfront-Planungsfeldern finden Sie unter [Felder erstellen](/help/quicksilver/planning/fields/create-fields.md).

In diesem Artikel wird beschrieben, wie Sie die Einstellungen für die Workfront-Planungsfelder bearbeiten können. Informationen zum Bearbeiten von Feldwerten für Datensätze finden Sie unter [Datensätze bearbeiten](/help/quicksilver/planning/records/edit-records.md).

## Überlegungen zum Bearbeiten von Feldeinstellungen

Beachten Sie Folgendes, bevor Sie Änderungen an der Konfiguration eines Felds vornehmen:

* Sie können von Ihnen erstellte Felder oder von anderen Benutzern erstellte Felder bearbeiten, wenn Sie über Verwaltungsberechtigungen für den Arbeitsbereich verfügen, zu dem die Felder gehören.
* Sie können ein Feld in der Tabelle vom Typ Datensatz bearbeiten.
* Sie können ein Feld auf der Datensatzseite oder in einer anderen Ansicht außerhalb der Tabellenansicht nicht bearbeiten.
* Nach dem Speichern des Felds können Sie den Feldtyp nicht mehr bearbeiten.
* Die Auswahl der zuvor ausgewählten Einstellung Negative Zahlen zulassen für ein Feld vom Typ Zahl, Prozentsatz oder Währung kann nicht aufgehoben werden, wenn bereits negative Werte in den Datensätzen gespeichert sind, an die das Feld angehängt ist.
* Nach dem Speichern des Felds können Sie die Konfiguration der folgenden Feldelemente bearbeiten:

   * Der Name oder die Beschreibung eines beliebigen Felds
   * Die Optionen eines Einzelauswahl- oder eines Mehrfachauswahlfelds.
   * Der Ausdruck eines Formelfelds.

  >[!WARNING]
  >
  >Wenn sich Formelausdrücke ändern oder Optionen aus einem Auswahlfeld hinzugefügt oder entfernt werden, gehen Daten für die Datensätze verloren, die bereits über Informationen verfügen, die in den Feldern gespeichert sind, deren Konfiguration geändert wird.
  >
  >Es gibt keine Warnung oder Hinweise darauf, dass dieser Datenverlust auftreten kann, wenn Sie die Konfiguration der Felder ändern.
  >
  >Es gibt keine Benachrichtigung für andere Benutzer, dass die Feldkonfiguration geändert wurde.

<!--this is not yet true, but it might come later:
* You can deselect Allow negative numbers option from a Number, Percentage, or Currency field after you save the field. 
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
   <td role="rowheader"><p>Adobe Workfront-Lizenz</p></td>
   <td>
   <p>Alle</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>Konfiguration der Zugriffsebene</p></td>
   <td> <p>Es gibt keine Zugriffskontrollen für die Workfront-Planung</p>  
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
   <td> <p>Ihr Workfront- oder Gruppenadministrator muss den Planungsbereich in Ihre Layoutvorlage einfügen. Weitere Informationen finden Sie unter <a href="/help/quicksilver/planning/access/access-overview.md">Zugriffsübersicht</a>. </p>  
</td>
  </tr>

</tbody>
</table>

<!--Maybe enable this at GA - but Planning is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

## Feldeinstellungen bearbeiten

{{step1-to-planning}}

Der zuletzt aufgerufene Arbeitsbereich sollte standardmäßig geöffnet werden.

1. (Optional) Erweitern Sie den nach unten zeigenden Pfeil rechts neben einem vorhandenen Workspace-Namen und wählen Sie den Arbeitsbereich aus, für den Sie Datensatztypen löschen möchten.

   Der Arbeitsbereich wird geöffnet und die damit verknüpften Datensatztypen werden angezeigt.
1. Klicken Sie auf die Karte für den Datensatztyp, dessen Felder Sie bearbeiten möchten.

   Dadurch wird die Seite des Datensatztyps geöffnet.
1. (Bedingt) Klicken Sie auf die Registerkarte eines **Tabellenansicht**.
1. Bewegen Sie den Mauszeiger über die Spaltenüberschrift eines Felds, das Sie bearbeiten möchten, und klicken Sie dann auf den nach unten zeigenden Pfeil nach dem Feldnamen und klicken Sie dann auf **Feld bearbeiten**

   Oder

   Doppelklicken Sie auf die Spaltenüberschrift für das Feld.

   ![](assets/arrow-menu-after-name-of-field-in-table-header-highlighted.png)

1. Aktualisieren Sie die Informationen über das Feld und klicken Sie auf **Speichern**. <!--insert screen shot when finalized-->

   >[!TIP]
   >
   >Nach dem Speichern des Felds kann der Feldtyp nicht mehr aktualisiert werden.

   Die Feldinformationen werden für alle Benutzer mit Zugriff auf den Arbeitsbereich aktualisiert.

1. (Bedingt) Klicken Sie für verknüpfte Datensatzfelder auf **Suchfelder bearbeiten** und fügen Sie eines der Felder aus dem verknüpften Datensatztyp hinzu oder entfernen Sie es.

   Weitere Informationen finden Sie unter [Datensatztypen verbinden](/help/quicksilver/planning/architecture/connect-record-types.md).

<!--After the release of the RTBE for field configurations, replace the tip with this:
>[!TIP]
>
>* You cannot update the field type after the field is saved.
>
>* When you modify field configurations (field options or formula expressions), records that already contain information in the modified fields will update their values in real-time. There is no warning and no audit log for the value changes triggered by field configuration changes. All users who view the fields will immediately see the new values with the modifications. -->
