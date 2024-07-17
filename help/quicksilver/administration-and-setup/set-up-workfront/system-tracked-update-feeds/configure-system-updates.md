---
user-type: administrator
product-area: system-administration;setup
navigation-topic: system-tracked-update-feeds
title: Systemaktualisierungen konfigurieren
description: Workfront generiert automatische Systemaktualisierungen im Bereich [!UICONTROL Aktualisierungen] eines Objekts, um die Änderungen aufzuzeichnen, die der Benutzer am Objekt vornimmt. Als [!DNL Workfront] Administrator können Sie konfigurieren, welche Objektfelder und Aktionen von [!DNL Workfront] aufgezeichnet werden, um Systemaktualisierungen aufzuzeichnen.
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: 54fc3f77-57d1-47f1-8e16-73626a6733ec
source-git-commit: c2c09486756db021b6edaf380c5a54d531ffa723
workflow-type: tm+mt
source-wordcount: '889'
ht-degree: 7%

---

# Systemaktualisierungen konfigurieren

[!DNL Adobe Workfront] generiert automatische Systemaktualisierungen im Bereich [!UICONTROL Aktualisierungen] eines Objekts, um die folgenden Ereignisse aufzuzeichnen:

* Änderungen, die Benutzer in einem Objektfeld vornehmen
* Aktionen, die Benutzer für ein Objekt ausführen

Diese Systemaktualisierungen umfassen die folgenden Informationen:

* Die Änderung, die vorgenommen wurde
* Der Name des Benutzers, der die Änderung vorgenommen hat
* Datum und Uhrzeit der Änderung

Weitere Informationen zu Systemaktualisierungen finden Sie unter [Vom System getrackte Updates](../system-tracked-update-feeds/system-tracked-update-feeds.md).

Als [!DNL Workfront] -Administrator können Sie konfigurieren, welche Objektfelder und Aktionen von [!DNL Workfront] verfolgt werden, um Systemaktualisierungen aufzuzeichnen.

Beispielsweise könnten Sie [!DNL Workfront] alle Änderungen verfolgen, die Benutzer an den Namen von Problemen im gesamten System vornehmen. Jede Änderung des Namens eines Problems wird dann als Systemaktualisierung im Bereich [!UICONTROL Aktualisierungen] des Problems angezeigt.

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Plan</td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Lizenz</td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Sie müssen ein [!DNL Workfront] -Administrator sein.</p> <p><b>HINWEIS</b>: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren [!DNL Workfront] -Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein [!DNL Workfront] -Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Bestimmen, welche Felder [!DNL Workfront] für einen Objekttyp nachverfolgt

Sie können festlegen, welche Informationen [!DNL Workfront] verfolgt, wenn Benutzer Informationen ändern, die mit einem bestimmten Objekttyp in der gesamten [!DNL Workfront] -Oberfläche verknüpft sind. Fügen Sie dazu die Felder hinzu oder entfernen Sie die Felder, die [!DNL Workfront] für diesen Objekttyp verfolgen soll.

>[!NOTE]
>
>* [!DNL Workfront] kann keine Aktualisierungen zu berechneten benutzerdefinierten Feldern verfolgen und aufzeichnen.
>* Sie können die Systemaktualisierung für Projekte, Aufgaben, Probleme, Portfolios, Programme und Benutzer anpassen. Sie können die Systemaktualisierung für Vorlagen, Dokumente oder Timesheets nicht anpassen, aber [!DNL Workfront] zeichnet Systemaktualisierungen für diese Objekte auf.
>



* [Fügen Sie die Felder hinzu, die  [!DNL Workfront]  verfolgen soll](#add-fields-you-want-workfront-to-track)
* [Felder entfernen, die nicht verfolgt werden sollen](#remove-fields-that-you-don-t-want-tracked)

### Felder hinzufügen, die [!DNL Workfront] verfolgen soll {#add-fields-you-want-workfront-to-track}

Sie können Felder hinzufügen, die [!DNL Workfront] für einen bestimmten Objekttyp in der [!DNL Workfront] -Oberfläche verfolgen soll. Wenn Benutzer Informationen in diesem Feld ändern, zeichnet [!DNL Workfront] Informationen über die Änderung als Systemaktualisierung im Bereich [!UICONTROL Aktualisierungen] für das Objekt auf.

>[!NOTE]
>
>Sie können bis zu 300 integrierte und benutzerdefinierte Felder in den Update-Feeds verfolgen. Wenn Sie die maximale Anzahl von Feldern verfolgen und zusätzliche Felder verfolgen möchten, die nicht auf der Unterregisterkarte [!UICONTROL Alle Felder] angezeigt werden, müssen Sie zunächst einige der verfolgten Felder entfernen, um neue Felder zu verfolgen. Weitere Informationen zum Entfernen von Feldern aus den Aktualisierungsfeldern finden Sie unter [Felder entfernen, die nicht verfolgt werden sollen](#remove-fields-that-you-don-t-want-tracked).

1. Klicken Sie auf das Symbol **[!UICONTROL Hauptmenü]** oben rechts in [!DNL Adobe Workfront] und dann auf **[!UICONTROL Setup]** ![](assets/gear-icon-settings.png).![](assets/main-menu-icon.png)

1. Klicken Sie im Bedienfeld auf der linken Seite auf **[!UICONTROL Schnittstelle]** > **[!UICONTROL Feeds aktualisieren]**.

1. &#x200B; auf **[!UICONTROL Felder hinzufügen]** und klicken Sie dann auf das Objekt, das verfolgt werden soll.

1. Geben Sie im angezeigten Feld &#x200B; **[!UICONTROL Feeds aktualisieren]** entweder ein integriertes (standardmäßiges) Feld oder ein benutzerdefiniertes Feld für das Objekt ein und klicken Sie dann auf , um es auszuwählen, wenn es in der Liste angezeigt wird.

   Wenn [!DNL Workfront] das Feld bereits verfolgt, können Sie es nicht erneut aus der Liste hinzufügen.

1. Nachdem Sie alle Felder hinzugefügt haben, die [!DNL Workfront] verfolgen soll, klicken Sie auf **[!UICONTROL Felder hinzufügen]**.

   Die von Ihnen hinzugefügten integrierten Felder werden auf der Unterregisterkarte **[!UICONTROL Integrierte Felder]** angezeigt.

   Die von Ihnen hinzugefügten benutzerdefinierten Felder werden auf der Unterregisterkarte **[!UICONTROL Benutzerdefinierte Felder]** angezeigt.

   Auf der Unterregisterkarte **[!UICONTROL Alle Felder]** werden sowohl die integrierten als auch die benutzerdefinierten Felder angezeigt, die verfolgt werden.

### Felder entfernen, die nicht verfolgt werden sollen {#remove-fields-that-you-don-t-want-tracked}

Sie können Felder entfernen, die das System nicht für einen bestimmten Objekttyp in der [!DNL Workfront] -Oberfläche verfolgen soll.

1. Klicken Sie auf das Symbol **[!UICONTROL Hauptmenü]** oben rechts in [!DNL Adobe Workfront] und dann auf **[!UICONTROL Setup]** ![](assets/gear-icon-settings.png).![](assets/main-menu-icon.png)

1. Klicken Sie auf **[!UICONTROL Schnittstelle]** > **[!UICONTROL Feeds aktualisieren]**.

1. Wählen Sie auf der Registerkarte **[!UICONTROL Verfolgte Felder]** die Unterregisterkarte **[!UICONTROL Alle Felder]** aus.

   Dies zeigt sowohl die integrierten als auch die benutzerdefinierten Felder, die derzeit verfolgt werden.

1. Wählen Sie das Feld aus, das die Verfolgung stoppen soll, und klicken Sie dann auf **[!UICONTROL Entfernen]**.

1. Klicken Sie im angezeigten Feld **[!UICONTROL Feld entfernen]** auf **[!UICONTROL Ja, entfernen Sie es]**, um zu bestätigen.

Alle Aktualisierungen zu den zuvor verfolgten Feldern bleiben im Bereich [!UICONTROL Aktualisierungen] erhalten, in dem sie aufgezeichnet wurden.

## Bestimmen, welche Aktionen [!DNL Workfront] für einen Objekttyp verfolgt

Sie können festlegen, dass [!DNL Workfront] die folgenden Aktionen verfolgt, die Benutzer auf Objekten in der [!DNL Workfront] -Oberfläche ausführen können.

Beispielsweise können Sie festlegen, dass [!DNL Workfront] jedes Mal, wenn ein Benutzer eine Zuweisung zu einer Aufgabe oder einem Problem ändert, ein Update aufzeichnet. Die Änderung wird dann als Systemaktualisierung im Bereich [!UICONTROL Aktualisierungen] für die Aufgabe oder das Problem angezeigt.

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
   <td>Rechnungsdatensatz wird erstellt oder gelöscht</td> 
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

So konfigurieren Sie, welche Aktionen [!DNL Workfront] verfolgen soll:

1. Klicken Sie auf das Symbol **[!UICONTROL Hauptmenü]** oben rechts in [!DNL Adobe Workfront] und dann auf **[!UICONTROL Setup]** ![](assets/gear-icon-settings.png).![](assets/main-menu-icon.png)

1. Klicken Sie auf **[!UICONTROL Schnittstelle]** > **[!UICONTROL Feeds aktualisieren]**.

1. Klicken Sie auf die Registerkarte **[!UICONTROL Aktionen]**.

1. Wählen Sie eine Aktion aus, um sie zu aktivieren, oder deaktivieren Sie eine Aktion, um sie zu deaktivieren.
1. Klicken Sie auf **[!UICONTROL Speichern]**.

Wenn Sie eine Aktion deaktivieren, werden alle zuvor aufgezeichneten Aktualisierungen dieser Aktion im Bereich [!UICONTROL Aktualisierungen] beibehalten, in dem sie aufgezeichnet wurde.
