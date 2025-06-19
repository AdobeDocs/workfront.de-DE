---
user-type: administrator
product-area: system-administration;setup
navigation-topic: system-tracked-update-feeds
title: Systemaktualisierungen konfigurieren
description: Workfront generiert automatische Systemaktualisierungen im Bereich [!UICONTROL Updates“ eines ], um die Änderungen aufzuzeichnen, die Benutzende am Objekt vornehmen. Als  [!DNL Workfront]  können Sie konfigurieren, welche Objektfelder und Aktionen  [!DNL Workfront]  Systemaktualisierungen aufgezeichnet werden sollen.
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: 54fc3f77-57d1-47f1-8e16-73626a6733ec
source-git-commit: f7cb314067d105d5534f4be356024aea8e8f9a28
workflow-type: tm+mt
source-wordcount: '931'
ht-degree: 8%

---

# Systemaktualisierungen konfigurieren

<!-- Audited: 6/2025 -->

<!--<div class="preview">

The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. The same features will also be available in the Production environment for all customers after a week from the Preview release.     

For more information, see [Interface modernization](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md). 

</div> -->

[!DNL Adobe Workfront] generiert automatische Systemaktualisierungen im Bereich [!UICONTROL Updates“ eines ], um die folgenden Ereignisse aufzuzeichnen:

* Änderungen, die Benutzer in einem Objektfeld vornehmen
* Aktionen, die Benutzer für ein Objekt ausführen

Diese Systemaktualisierungen enthalten die folgenden Informationen:

* Die vorgenommene Änderung
* Der Name des Benutzers, der die Änderung vorgenommen hat
* Uhrzeit und Datum der Änderung

Weitere Informationen zu Systemaktualisierungen finden Sie unter [System-getrackte Aktualisierungen](../system-tracked-update-feeds/system-tracked-update-feeds.md).

Als [!DNL Workfront] können Sie konfigurieren, welche Objektfelder und Aktionen verfolgt [!DNL Workfront], um Systemaktualisierungen aufzuzeichnen.

Sie könnten beispielsweise alle Änderungen nachverfolgen [!DNL Workfront], die Benutzer an den Namen von Problemen im gesamten System vornehmen. Jede Änderung des Problemnamens wird dann als Systemaktualisierung im Bereich [!UICONTROL Updates] des Problems angezeigt.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Plan</td> 
   <td>Beliebig</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Lizenz*</td> 
   <td><p>Neu: [!UICONTROL Standard]</p>
   Oder
   <p>Aktuell: [!UICONTROL Plan]</p>
   </td> 
  </tr>  
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td>[!UICONTROL Systemadministrator]</td>
  </tr> 
 </tbody> 
</table>

*Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Bestimmen, welche Felder [!DNL Workfront] für einen Objekttyp nachverfolgt

Sie können bestimmen, welche Informationen [!DNL Workfront] nachverfolgt, wenn Benutzende in der gesamten [!DNL Workfront] Informationen ändern, die einem bestimmten Objekttyp zugeordnet sind. Dies geschieht durch Hinzufügen oder Entfernen der Felder, die für diesen Objekttyp nachverfolgt werden [!DNL Workfront].

>[!NOTE]
>
>* [!DNL Workfront] können Aktualisierungen über berechnete benutzerdefinierte Felder nicht verfolgen und aufzeichnen.
>* Sie können die Systemaktualisierung für Projekte, Aufgaben, Probleme, Portfolios, Programme und Benutzer anpassen. Sie können die Systemaktualisierung für Vorlagen, Dokumente oder Arbeitszeittabellen nicht anpassen, [!DNL Workfront] zeichnet jedoch Systemaktualisierungen für diese Objekte auf.
>


### Felder hinzufügen, die verfolgt werden [!DNL Workfront] {#add-fields-you-want-workfront-to-track}

Sie können Felder hinzufügen, die [!DNL Workfront] für einen bestimmten Objekttyp in der gesamten [!DNL Workfront] nachverfolgen möchten. Wenn Benutzende Informationen in diesem Feld ändern, zeichnet [!DNL Workfront] Informationen über die Änderung als Systemaktualisierung im Bereich [!UICONTROL Updates] für das Objekt auf.

>[!NOTE]
>
>Sie können bis zu 300 integrierte und benutzerdefinierte Felder in den Aktualisierungs-Feeds verfolgen. Wenn Sie die maximale Anzahl von Feldern verfolgen und zusätzliche Felder verfolgen möchten, die nicht auf der Unterregisterkarte [!UICONTROL Alle Felder] angezeigt werden, müssen Sie zunächst einige der verfolgten Felder entfernen, um neue Felder zu verfolgen. Weitere Informationen zum Entfernen von Feldern aus den Aktualisierungsfeldern finden Sie unter [Entfernen von Feldern, die nicht verfolgt werden sollen](#remove-fields-you-don-t-want-tracked).

{{step-1-to-setup}}

1. Klicken Sie im Bedienfeld links auf **[!UICONTROL Schnittstelle]** und dann auf **[!UICONTROL Feeds aktualisieren]**.
1. (Optional) Klicken Sie auf der Registerkarte **Nachverfolgte Felder** auf eine der folgenden Unterregisterkarten, je nachdem, welche Feldtypen Sie im Aktualisierungsfeed nachverfolgen möchten:

   * **Integrierte Felder**: Zeigt eine Liste der integrierten Felder an.
   * **Benutzerdefinierte Felder**: Zeigt eine Liste der benutzerdefinierten Felder an. Sie müssen die benutzerdefinierten Felder erstellen, bevor sie in der Liste verfügbar sind.
   * **Alle Felder**: Zeigt eine Liste der integrierten und benutzerdefinierten Felder an.

1. Klicken Sie **[!UICONTROL Felder hinzufügen]** und wählen Sie dann aus der Dropdown-Liste das Objekt aus, das verfolgt werden soll.

   Die manuelle Auswahl von Feldern ist nicht für alle Objekte verfügbar, die einen Bereich „Aktualisierungen“ aufweisen.

   Auswahl aus Feldern für die folgenden Objekte:

   * Projekt
   * Aufgabe
   * Problem
   * Portfolio
   * Programm
   * Benutzerin oder Benutzer

   Das **Felder hinzufügen** wird für jedes ausgewählte Objekt geöffnet.
1. Beginnen Sie **Feld „Felder hinzufügen** entweder mit der Eingabe eines integrierten (standardmäßigen) Felds oder eines benutzerdefinierten Felds für das Objekt und wählen Sie es aus, wenn es in der Liste angezeigt wird.

   >[!NOTE]
   >
   >Wenn [!DNL Workfront] das Feld bereits nachverfolgt, können Sie es nicht ein zweites Mal aus der Liste hinzufügen.

1. Nachdem Sie alle Felder hinzugefügt haben, die Sie verfolgen [!DNL Workfront], klicken Sie auf **[!UICONTROL Felder hinzufügen]**.
Die hinzugefügten integrierten Felder werden auf der Unterregisterkarte **[!UICONTROL Integrierte Felder]** und die benutzerdefinierten Felder auf der Unterregisterkarte **[!UICONTROL Benutzerdefinierte Felder]** angezeigt.
Die Unterregisterkarte **[!UICONTROL Alle Felder]** zeigt sowohl die integrierten als auch die benutzerdefinierten Felder an, die [!DNL Workfront] nachverfolgt.

<!-- replace the above when releasing to Preview: 

1. In the panel on the left, click **[!UICONTROL Interface]**, then **[!UICONTROL Update Feeds]**.
1. (Optional) In the <span class="preview">**Tracked fields** tab</span>, click one of the following subtabs, depending on which types of fields you want to track in the update feed:

   * <span class="preview">**Built-in fields**</span>: Displays a list of built-in fields.
   * <span class="preview">**Custom fields**</span>: Displays a list of custom fields. You must create the custom fields before they are available in the list. 
   * <span class="preview">**All fields**</span>: Displays a list of both built-in and custom fields. 

1. Click <span class="preview">**[!UICONTROL Add fields]**,</span> then select the object that you want to be tracked from the drop-down. 

   Manually selecting fields is not available for all the objects that have an Updates area.

   Select from fields for the following objects:

      * Project
      * Task
      * Issue
      * Portfolio
      * Program
      * User

   The <span class="preview">**Add fields** </span> box opens, for each object selected.
1. In the <span class="preview">**Add fields** </span> box, start typing either a built-in (standard) field or a custom field for the object, then select it when it appears in the list.

   >[!NOTE]
   >
   >If [!DNL Workfront] is already tracking the field, you can't add it a second time from the list.

1. After adding all the fields you want [!DNL Workfront] to track, <span class="preview"> click **[!UICONTROL Add]**.
   The built-in fields that you added show under the **[!UICONTROL Built-in fields]** subtab, and the custom fields show under the **[!UICONTROL Custom fields]** subtab.
   The **[!UICONTROL All fields]** subtab shows both the built-in and the custom fields that [!DNL Workfront] tracks.</span>

-->

### Felder entfernen, die nicht verfolgt werden sollen {#remove-fields-you-don-t-want-tracked}

Sie können Felder entfernen, die das System nicht für einen bestimmten Objekttyp über die [!DNL Workfront] nachverfolgen soll.

{{step-1-to-setup}}

1. Klicken Sie **[!UICONTROL Schnittstelle]** und dann **[!UICONTROL Feeds aktualisieren]**.

1. Wählen Sie auf **[!UICONTROL Registerkarte]** Getrackte Felder“ die Unterregisterkarte **[!UICONTROL Alle Felder]** aus. Sowohl die integrierten als auch die benutzerdefinierten Felder, die derzeit verfolgt werden, werden angezeigt.

1. Wählen Sie das Feld aus, das Sie nicht mehr verfolgen möchten, und klicken Sie dann auf **[!UICONTROL Entfernen]**.


<!--replace above at Preview release with this:

1. On the <span class="preview">**[!UICONTROL Tracked fields]** tab</span>, select the **[!UICONTROL All fields]** subtab. Both the built-in and custom fields that are currently being tracked display.

1. Select the field you want to stop tracking, then click the <span class="preview">**[!UICONTROL Remove]** icon ![Remove icon](assets/remove-icon.png).</span>

-->

1. Klicken Sie im angezeigten **[!UICONTROL Feld]** Feld entfernen“ zur Bestätigung auf **[!UICONTROL Ja,]** entfernen.

   Aktualisierungen zu den zuvor verfolgten Feldern bleiben im Bereich [!UICONTROL Aktualisierungen] erhalten, in dem sie aufgezeichnet wurden.

## Bestimmen, welche Aktionen [!DNL Workfront] für einen Objekttyp nachverfolgt

Sie können [!DNL Workfront] Aktionen verfolgen, die Benutzer für Objekte in der [!DNL Workfront] ausführen.

Sie können beispielsweise jedes Mal eine Aktualisierung aufzeichnen [!DNL Workfront], wenn ein Benutzer eine Zuweisung zu einer Aufgabe oder einem Problem ändert.

Die Änderung wird dann als Systemaktualisierung im Bereich [!UICONTROL Updates] für die Aufgabe oder das Problem angezeigt.

In der folgenden Tabelle werden die Aktionen beschrieben, die Sie für Objekte in [!DNL Workfront] nachverfolgen können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Aktion</strong> </th> 
   <th><strong>Objekte</strong> </th> 
   <th><strong>Standardstatus</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Zuweisung wurde geändert</td> 
   <td>Aufgaben, Probleme</td> 
   <td> <p>Aktiviert</p> </td> 
  </tr> 
  <tr> 
   <td>Baseline wird gelöscht</td> 
   <td>Projekte</td> 
   <td> <p>Deaktiviert</p> </td> 
  </tr> 
  <tr> 
   <td>Rechnungsnachweis wird erstellt oder gelöscht</td> 
   <td>Projekte</td> 
   <td> <p>Aktiviert</p> </td> 
  </tr> 
  <tr> 
   <td>Dokument wird erstellt bzw. gelöscht</td> 
   <td>Projekte, Aufgaben, Probleme, Portfolios, Programme</td> 
   <td> <p>Aktiviert</p> </td> 
  </tr> 
  <tr> 
   <td>Ausgabe wird erstellt bzw. gelöscht</td> 
   <td>Projekte, Aufgaben</td> 
   <td> <p>Aktiviert</p> </td> 
  </tr> 
  <tr> 
   <td>Stunde wird protokolliert bzw. gelöscht</td> 
   <td>Projekte, Aufgaben, Probleme</td> 
   <td> <p>Aktiviert</p> </td> 
  </tr> 
  <tr> 
   <td>Problem wurde gelöscht</td> 
   <td>Projekte</td> 
   <td> <p>Aktiviert</p> </td> 
  </tr> 
  <tr> 
   <td>Aufgabe wird gelöscht</td> 
   <td>Projekte</td> 
   <td> <p>Aktiviert</p> </td> 
  </tr> 
  <tr> 
   <td>Der Zugriff einer Person wird geändert</td> 
   <td>Projekte, Aufgaben, Probleme, Dokumente, Portfolios, Programme</td> 
   <td> <p>Aktiviert</p> </td> 
  </tr> 
  <tr> 
   <td>Kommentarobjekt abonnieren</td> 
   <td>Projekte, Aufgaben, Probleme</td> 
   <td> <p>Aktiviert</p> </td> 
  </tr> 
 </tbody> 
</table>

So konfigurieren Sie, welche Aktionen Sie verfolgen [!DNL Workfront]:

{{step-1-to-setup}}

1. Klicken Sie **[!UICONTROL Schnittstelle]** und dann **[!UICONTROL Feeds aktualisieren]**.

1. Klicken Sie auf **[!UICONTROL Registerkarte]** Aktionen“.

1. Aktivieren Sie das Kontrollkästchen einer Aktion, um sie zu aktivieren, oder deaktivieren Sie sie, um sie zu deaktivieren.
1. Klicken Sie auf **[!UICONTROL Speichern]**.

   Wenn Sie eine Aktion deaktivieren, werden alle zuvor aufgezeichneten Aktualisierungen zu dieser Aktion im Bereich [!UICONTROL Updates] beibehalten, in dem sie aufgezeichnet wurde. [!DNL Workfront] Beendet die Aufzeichnung neuer Aktualisierungen für die deaktivierte Aktion.
