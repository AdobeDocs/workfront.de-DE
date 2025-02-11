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
source-git-commit: 85aa6cc865bfc28498cca17e1942c146eeb8e4fc
workflow-type: tm+mt
source-wordcount: '899'
ht-degree: 8%

---

# Systemaktualisierungen konfigurieren

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

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Plan</td> 
   <td>Beliebig</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Lizenz</td> 
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

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Bestimmen, welche Felder [!DNL Workfront] für einen Objekttyp nachverfolgt

Sie können bestimmen, welche Informationen [!DNL Workfront] nachverfolgt, wenn Benutzende in der gesamten [!DNL Workfront] Informationen ändern, die einem bestimmten Objekttyp zugeordnet sind. Dies geschieht durch Hinzufügen oder Entfernen der Felder, die für diesen Objekttyp nachverfolgt werden [!DNL Workfront].

>[!NOTE]
>
>* [!DNL Workfront] können Aktualisierungen über berechnete benutzerdefinierte Felder nicht verfolgen und aufzeichnen.
>* Sie können die Systemaktualisierung für Projekte, Aufgaben, Probleme, Portfolios, Programme und Benutzer anpassen. Sie können die Systemaktualisierung für Vorlagen, Dokumente oder Arbeitszeittabellen nicht anpassen, [!DNL Workfront] zeichnet jedoch Systemaktualisierungen für diese Objekte auf.
>



* [Felder hinzufügen,  [!DNL Workfront]  verfolgt werden sollen](#add-fields-you-want-workfront-to-track)
* [Felder entfernen, die nicht verfolgt werden sollen](#remove-fields-that-you-don-t-want-tracked)

### Felder hinzufügen, die verfolgt werden [!DNL Workfront] {#add-fields-you-want-workfront-to-track}

Sie können Felder hinzufügen, die [!DNL Workfront] für einen bestimmten Objekttyp in der gesamten [!DNL Workfront] nachverfolgen möchten. Wenn Benutzende Informationen in diesem Feld ändern, zeichnet [!DNL Workfront] Informationen über die Änderung als Systemaktualisierung im Bereich [!UICONTROL Updates] für das Objekt auf.

>[!NOTE]
>
>Sie können bis zu 300 integrierte und benutzerdefinierte Felder in den Aktualisierungs-Feeds verfolgen. Wenn Sie die maximale Anzahl von Feldern nachverfolgen und zusätzliche Felder nachverfolgen möchten, die nicht auf der Unterregisterkarte [!UICONTROL Alle Felder] angezeigt werden, müssen Sie zunächst einige der nachverfolgten Felder entfernen, um neue Felder nachverfolgen zu können. Weitere Informationen zum Entfernen von Feldern aus den Aktualisierungsfeldern finden Sie unter [Entfernen von Feldern, die nicht verfolgt werden sollen](#remove-fields-that-you-don-t-want-tracked).

1. Klicken Sie auf **[!UICONTROL Hauptmenü]**-Symbol ![Hauptmenüsymbol](assets/main-menu-icon.png) in der oberen rechten Ecke von [!DNL Adobe Workfront] und klicken Sie dann auf **[!UICONTROL Setup]** ![Zahnradeinstellungssymbol](assets/gear-icon-settings.png).

1. Klicken Sie im Bedienfeld links auf **[!UICONTROL Schnittstelle]** > **[!UICONTROL Feeds aktualisieren]**.

1. &#x200B;Klicken Sie auf **[!UICONTROL Felder hinzufügen]** und klicken Sie dann auf das Objekt, das verfolgt werden soll.

1. **[!UICONTROL Beginnen Sie im &#x200B;]** Aktualisierungsfeeds“ mit der Eingabe eines integrierten (standardmäßigen) Felds oder eines benutzerdefinierten Felds für das Objekt und klicken Sie auf das Objekt, um es auszuwählen, wenn es in der Liste angezeigt wird.

   Wenn [!DNL Workfront] das Feld bereits nachverfolgt, können Sie es nicht erneut aus der Liste hinzufügen.

1. Nachdem Sie alle Felder hinzugefügt haben, die Sie verfolgen [!DNL Workfront], klicken Sie auf **[!UICONTROL Felder hinzufügen]**.

   Die hinzugefügten integrierten Felder werden auf der Unterregisterkarte **[!UICONTROL Integrierte Felder]** angezeigt.

   Die hinzugefügten benutzerdefinierten Felder werden auf der Unterregisterkarte **[!UICONTROL Benutzerdefinierte Felder]** angezeigt.

   Die Unterregisterkarte **[!UICONTROL Alle Felder]** zeigt sowohl die integrierten als auch die benutzerdefinierten Felder an, die verfolgt werden.

### Felder entfernen, die nicht verfolgt werden sollen {#remove-fields-that-you-don-t-want-tracked}

Sie können Felder entfernen, die das System nicht für einen bestimmten Objekttyp über die [!DNL Workfront] nachverfolgen soll.

1. Klicken Sie auf **[!UICONTROL Hauptmenü]**-Symbol ![Hauptmenüsymbol](assets/main-menu-icon.png) in der oberen rechten Ecke von [!DNL Adobe Workfront] und klicken Sie dann auf **[!UICONTROL Setup]** ![Zahnradeinstellungssymbol](assets/gear-icon-settings.png).

1. Klicken Sie auf **[!UICONTROL Schnittstelle]** > **[!UICONTROL Feeds aktualisieren]**.

1. Wählen Sie auf **[!UICONTROL Registerkarte]** Getrackte Felder **[!UICONTROL die Unterregisterkarte Alle Felder]** aus.

   Hier werden sowohl die integrierten als auch die benutzerdefinierten Felder angezeigt, die derzeit verfolgt werden.

1. Wählen Sie das Feld aus, das Sie nicht mehr verfolgen möchten, und klicken Sie dann auf **[!UICONTROL Entfernen]**.

1. Klicken Sie im angezeigten **[!UICONTROL Feld]** Feld entfernen“ zur Bestätigung auf **[!UICONTROL Ja,]** entfernen.

Aktualisierungen zu den zuvor verfolgten Feldern bleiben im Bereich [!UICONTROL Aktualisierungen] erhalten, in dem sie aufgezeichnet wurden.

## Bestimmen, welche Aktionen [!DNL Workfront] für einen Objekttyp nachverfolgt

Sie [!DNL Workfront] die folgenden Aktionen verfolgen, die Benutzer an Objekten in der gesamten [!DNL Workfront] ausführen können.

Sie können beispielsweise jedes Mal eine Aktualisierung aufzeichnen [!DNL Workfront], wenn ein Benutzer eine Zuweisung zu einer Aufgabe oder einem Problem ändert. Die Änderung wird dann als Systemaktualisierung im Bereich [!UICONTROL Updates] für die Aufgabe oder das Problem angezeigt.

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

1. Klicken Sie auf **[!UICONTROL Hauptmenü]**-Symbol ![Hauptmenüsymbol](assets/main-menu-icon.png) in der oberen rechten Ecke von [!DNL Adobe Workfront] und klicken Sie dann auf **[!UICONTROL Setup]** ![Zahnradeinstellungssymbol](assets/gear-icon-settings.png).

1. Klicken Sie auf **[!UICONTROL Schnittstelle]** > **[!UICONTROL Feeds aktualisieren]**.

1. Klicken Sie auf **[!UICONTROL Registerkarte]** Aktionen“.

1. Wählen Sie eine Aktion aus, um sie zu aktivieren, oder heben Sie die Auswahl einer Aktion auf, um sie zu deaktivieren.
1. Klicken Sie auf **[!UICONTROL Speichern]**.

Wenn Sie eine Aktion deaktivieren, werden alle zuvor aufgezeichneten Aktualisierungen zu dieser Aktion im Bereich [!UICONTROL Updates] beibehalten, in dem sie aufgezeichnet wurde.
