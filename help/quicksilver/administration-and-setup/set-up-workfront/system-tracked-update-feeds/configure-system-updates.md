---
user-type: administrator
product-area: system-administration;setup
navigation-topic: system-tracked-update-feeds
title: Systemaktualisierungen konfigurieren
description: Workfront generiert automatische Systemaktualisierungen im [!UICONTROL Updates] -Bereich, um die Änderungen aufzuzeichnen, die Benutzer am Objekt vornehmen. Als [!DNL Workfront] Administrator können Sie konfigurieren, welche Objektfelder und Aktionen [!DNL Workfront] verfolgt, um Systemaktualisierungen aufzuzeichnen.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 54fc3f77-57d1-47f1-8e16-73626a6733ec
source-git-commit: 413e5ff710b4c77b7ea2d870b34bb0627a4fcd86
workflow-type: tm+mt
source-wordcount: '884'
ht-degree: 7%

---

# Systemaktualisierungen konfigurieren

[!DNL Adobe Workfront] generiert automatische Systemaktualisierungen in der [!UICONTROL Updates] -Bereich, um die folgenden Ereignisse aufzuzeichnen:

* Änderungen, die Benutzer in einem Objektfeld vornehmen
* Aktionen, die Benutzer für ein Objekt ausführen

Zu diesen Systemaktualisierungen gehören die vorgenommene Änderung, der Name des Benutzers, der die Änderung vorgenommen hat, sowie Uhrzeit und Datum der Änderung.

Weitere Informationen zu Systemaktualisierungen finden Sie unter [Vom System getrackte Aktualisierungen](../system-tracked-update-feeds/system-tracked-update-feeds.md).

Als [!DNL Workfront] Administrator können Sie konfigurieren, welche Objektfelder und Aktionen [!DNL Workfront] verfolgt, um Systemaktualisierungen aufzuzeichnen.

Beispielsweise können Sie [!DNL Workfront] verfolgen Sie alle Änderungen, die Benutzer an den Namen von Problemen im gesamten System vornehmen. Jede Änderung des Problemnamens erscheint dann als Systemaktualisierung zum Problem [!UICONTROL Updates] Bereich.

## Zugriffsanforderungen

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
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Sie müssen [!DNL Workfront] Administrator.</p> <p><b>NOTE</b>: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren [!DNL Workfront] Administrator , wenn sie zusätzliche Einschränkungen für Ihre Zugriffsebene festlegen. Informationen zur Verwendung von [!DNL Workfront] Administrator kann Ihre Zugriffsebene ändern, siehe <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Bestimmen, welche Felder [!DNL Workfront] Tracks für einen Objekttyp

Sie können bestimmen, welche Informationen [!DNL Workfront] verfolgt, wenn Benutzer Informationen ändern, die mit einem bestimmten Objekttyp verknüpft sind, über die gesamte [!DNL Workfront] -Schnittstelle. Fügen Sie dazu die gewünschten Felder hinzu oder entfernen Sie sie. [!DNL Workfront] , um für diesen Objekttyp zu verfolgen.

>[!NOTE]
>
>* [!DNL Workfront] keine Aktualisierung berechneter benutzerdefinierter Felder nachverfolgen und aufzeichnen kann.
>* Sie können die Systemaktualisierung für Projekte, Aufgaben, Probleme, Portfolios, Programme und Benutzer anpassen. Sie können die Systemaktualisierung für Vorlagen, Dokumente oder Timesheets nicht anpassen, aber [!DNL Workfront] erfasst Systemaktualisierungen für diese Objekte.
>



* [Hinzufügen von gewünschten Feldern [!DNL Workfront] zum Tracking](#add-fields-you-want-workfront-to-track)
* [Felder entfernen, die nicht verfolgt werden sollen](#remove-fields-that-you-don-t-want-tracked)

### Hinzufügen von gewünschten Feldern [!DNL Workfront] zum Tracking {#add-fields-you-want-workfront-to-track}

Sie können die gewünschten Felder hinzufügen [!DNL Workfront] zur Verfolgung eines bestimmten Objekttyps im gesamten [!DNL Workfront] -Schnittstelle. Wenn Benutzer Informationen in diesem Feld ändern, [!DNL Workfront] erfasst Informationen über die Änderung als Systemaktualisierung im [!UICONTROL Updates] -Bereich für das Objekt.

>[!NOTE]
>
>Sie können bis zu 300 integrierte und benutzerdefinierte Felder in den Update-Feeds verfolgen. Wenn Sie die maximale Anzahl von Feldern verfolgen und zusätzliche Felder verfolgen möchten, die nicht im [!UICONTROL Alle Felder] Unter-Tab müssen Sie zunächst einige der verfolgten Felder entfernen, um neue Felder verfolgen zu können. Weitere Informationen zum Entfernen von Feldern aus den Aktualisierungsfeldern finden Sie unter [Felder entfernen, die nicht verfolgt werden sollen](#remove-fields-that-you-don-t-want-tracked).

1. Klicken Sie auf **[!UICONTROL Hauptmenü]** icon ![](assets/main-menu-icon.png) in der oberen rechten Ecke von [!DNL Adobe Workfront]Klicken Sie auf **[!UICONTROL Einrichtung]** ![](assets/gear-icon-settings.png).

1. Klicken Sie im linken Bereich auf **[!UICONTROL Schnittstelle]** > **[!UICONTROL Feeds aktualisieren]**.

1. &#x200B; **[!UICONTROL Felder hinzufügen]** und klicken Sie dann auf das Objekt, das Sie verfolgen möchten.

1. Im &#x200B; **[!UICONTROL Feeds aktualisieren]** in das Feld ein, beginnen Sie mit der Eingabe eines integrierten (Standard-) Felds oder eines benutzerdefinierten Felds für das Objekt und wählen Sie es dann aus, wenn es in der Liste angezeigt wird.

   Wenn [!DNL Workfront] das Feld bereits verfolgt, können Sie es nicht erneut aus der Liste hinzufügen.

1. Nachdem Sie alle gewünschten Felder hinzugefügt haben [!DNL Workfront] klicken Sie auf **[!UICONTROL Felder hinzufügen]**.

   Die von Ihnen hinzugefügten integrierten Felder werden unter dem **[!UICONTROL Integrierte Felder]** Unterregisterkarte.

   Die von Ihnen hinzugefügten benutzerdefinierten Felder werden unter dem **[!UICONTROL Benutzerdefinierte Felder]** Unterregisterkarte.

   Die **[!UICONTROL Alle Felder]** Unter-Tab zeigt sowohl die integrierten als auch die benutzerdefinierten Felder an, die verfolgt werden.

### Felder entfernen, die nicht verfolgt werden sollen {#remove-fields-that-you-don-t-want-tracked}

Sie können Felder entfernen, die das System nicht für einen bestimmten Objekttyp im gesamten [!DNL Workfront] -Schnittstelle.

1. Klicken Sie auf **[!UICONTROL Hauptmenü]** icon ![](assets/main-menu-icon.png) in der oberen rechten Ecke von [!DNL Adobe Workfront]Klicken Sie auf **[!UICONTROL Einrichtung]** ![](assets/gear-icon-settings.png).

1. Klicks **[!UICONTROL Schnittstelle]** > **[!UICONTROL Feeds aktualisieren]**.

1. Im **[!UICONTROL Verfolgte Felder]** auswählen, wählen Sie die **[!UICONTROL Alle Felder]** Unterregisterkarte.

   Dies zeigt sowohl die integrierten als auch die benutzerdefinierten Felder, die derzeit verfolgt werden.

1. Wählen Sie das Feld aus, das die Verfolgung stoppen soll, und klicken Sie auf **[!UICONTROL Entfernen]**.

1. Im **[!UICONTROL Feld entfernen]** wird angezeigt, klicken Sie auf **[!UICONTROL Ja, entfernen]** zur Bestätigung.

Alle Aktualisierungen bezüglich der zuvor verfolgten Felder bleiben im Abschnitt [!UICONTROL Updates] Gebiet, in dem sie aufgezeichnet wurden.

## Bestimmen der Aktionen [!DNL Workfront] Tracks für einen Objekttyp

Sie können [!DNL Workfront] Verfolgen Sie die folgenden Aktionen, die Benutzer für Objekte im gesamten [!DNL Workfront] -Schnittstelle.

Sie können beispielsweise [!DNL Workfront] eine Aktualisierung jedes Mal aufzeichnen, wenn ein Benutzer eine Zuweisung zu einer Aufgabe oder einem Problem ändert. Die Änderung wird dann als Systemaktualisierung im [!UICONTROL Updates] -Bereich für die Aufgabe oder das Problem.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Aktion</strong> </th> 
   <th><strong>Objekte</strong> </th> 
   <th><strong>Primärer Status</strong> </th> 
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

So konfigurieren Sie die gewünschten Aktionen [!DNL Workfront] zur Verfolgung:

1. Klicken Sie auf **[!UICONTROL Hauptmenü]** icon ![](assets/main-menu-icon.png) in der oberen rechten Ecke von [!DNL Adobe Workfront]Klicken Sie auf **[!UICONTROL Einrichtung]** ![](assets/gear-icon-settings.png).

1. Klicks **[!UICONTROL Schnittstelle]** > **[!UICONTROL Feeds aktualisieren]**.

1. Klicken Sie auf **[!UICONTROL Aktionen]** Registerkarte.

1. Wählen Sie eine Aktion aus, um sie zu aktivieren, oder deaktivieren Sie eine Aktion, um sie zu deaktivieren.
1. Klicken Sie auf **[!UICONTROL Speichern]**.

Wenn Sie eine Aktion deaktivieren, werden alle zuvor aufgezeichneten Aktualisierungen dieser Aktion im [!UICONTROL Updates] Bereich, in dem er aufgezeichnet wurde.
