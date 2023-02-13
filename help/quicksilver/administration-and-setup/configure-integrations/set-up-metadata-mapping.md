---
title: Einrichten der Metadaten-Zuordnung
user-type: administrator
product-area: system-administration;workfront-integrations
navigation-topic: administrator-integrations
description: Metadaten sind beschreibende Informationen, die mit einem Dokument verknüpft sind. Sie können [!DNL Adobe Workfront] , um Metadaten mit Dokumenten einzuschließen, die an gesendet werden [!DNL Workfront] Anwendungen.
author: Caroline
feature: System Setup and Administration, Workfront Integrations and Apps
role: Admin
exl-id: 7cf4787d-7cff-489e-bd5b-69db3ff09f6e
source-git-commit: ceda437684f565b91dbb8b02f6b03cbe8d27a70a
workflow-type: tm+mt
source-wordcount: '614'
ht-degree: 0%

---

# Einrichten der Metadaten-Zuordnung

Metadaten sind beschreibende Informationen, die mit einem Dokument verknüpft sind. Sie können [!DNL Adobe Workfront] , um Metadaten mit Dokumenten einzuschließen, die an gesendet werden [!DNL Workfront] Anwendungen.

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
   <td> <p>Sie müssen [!DNL Workfront] Administrator. Weitere Informationen finden Sie unter <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Gewähren eines vollen Administratorzugriffs</a>.</p> <p><b>NOTE</b>: Wenn Sie noch keinen Zugriff haben, fragen Sie Ihren [!DNL Workfront] Administrator , wenn sie zusätzliche Einschränkungen für Ihre Zugriffsebene festlegen. Für Informationen zur [!DNL Workfront] Administrator kann Ihre Zugriffsebene ändern, siehe <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Info [!DNL Workfront] Metadaten

Metadaten für Dokumente in [!DNL Workfront] kann Informationen wie den zugehörigen Projektnamen, die Aufgabenbeschreibung oder das geplante Abschlussdatum enthalten. Als [!DNL Workfront] Administrator, können Sie [!DNL Workfront] zum Hinzufügen von Metadaten zu Dokumenten, die von gesendet werden [!DNL Workfront] an [!DNL Workfront] Anwendungen:

* [!DNL Workfront DAM]

Bevor Metadaten mit Dokumenten gesendet werden können, müssen Sie zunächst die Metadaten angeben oder zuordnen, die eingeschlossen werden sollen. Sie können jedes Feld zuordnen, das in [!DNL Workfront]. Nachdem Sie die Metadatenzuordnung eingerichtet haben, werden alle Dokumente in eine [!DNL Workfront] Die Anwendung enthält die zugeordneten Metadaten.

Wenn ein Benutzer ein Dokument von [!DNL Workfront] zu [!DNL Workfront] -Anwendung werden zugeordnete Metadaten entlang des Dokuments übertragen. Während die Version des Dokuments im [!DNL Workfront] -Anwendung ist verknüpft mit [!DNL Workfront], Änderungen an den Metadaten des Dokuments in [!DNL Workfront] nicht in den Metadaten des Dokuments im [!DNL Workfront] Anwendung. Wenn ein zugeordnetes Feld in [!DNL Workfront] geändert wurde, müssen Sie eine neue Version des Dokuments mit den aktualisierten Metadaten an die [!DNL Workfront] Anwendung.

>[!NOTE]
>
>Sie können Metadaten nur in eine Richtung zuordnen: von [!DNL Workfront] nach [!DNL Workfront DAM]. Metadaten für Dokumente, die verknüpft sind mit [!DNL Workfront] von [!DNL Workfront DAM] kann nicht an Workfront übertragen werden.

Sie können die gleiche [!DNL Workfront] Feld für verschiedene Metadatenfelder in [!DNL Workfront DAM], Sie können jedoch kein Metadatenfeld in einer dieser Anwendungen für mehrere [!DNL Workfront] Metadatenfelder.

So konfigurieren Sie mehrere [!DNL Workfront] Felder, die in ein Metadatenfeld in einem [!DNL Workfront] -Anwendung erstellen Sie zunächst ein berechnetes benutzerdefiniertes Feld in [!DNL Workfront] , um alle einzelnen benutzerdefinierten Felder eines Objekts anzuzeigen. Ordnen Sie dann die berechnete [!DNL Workfront] in ein Metadatenfeld im [!DNL Workfront] Anwendung. Weitere Informationen zu berechneten benutzerdefinierten Feldern finden Sie unter [Hinzufügen errechneter Daten zu einem benutzerdefinierten Formular](../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

Bevor Sie Felder für den Metadaten-Zuordnungsprozess zuordnen können, müssen Sie die Anwendung in [!DNL Workfront]. Weitere Informationen finden Sie unter [Dokumentintegrationen konfigurieren](../../administration-and-setup/configure-integrations/configure-document-integrations.md).

## Konfigurieren [!DNL Workfront] Senden von Metadaten

1. Klicken Sie auf **[!UICONTROL Hauptmenü]** icon ![](assets/main-menu-icon.png) in der oberen rechten Ecke von [!DNL Adobe Workfront]Klicken Sie auf **[!UICONTROL Einrichtung]** ![](assets/gear-icon-settings.png).

1. Klicken Sie im linken Bereich auf **[!UICONTROL Dokumente]** > **[!UICONTROL Metadatenzuordnung]**.

   ![](assets/metadata-mapping.png)

1. Im **[!UICONTROL Quellfeld für Zuordnung auswählen]** eingeben, beginnen Sie mit der Eingabe des Namens des Workfront-Felds, das Sie zuordnen möchten. [!DNL Workfront DAM], und wählen Sie es aus, wenn Sie es in der Liste sehen.
1. Im **[!UICONTROL Zielfeld für Zuordnung auswählen]** auswählen, wählen Sie das Feld aus, das mit den Informationen in der ausgewählten [!DNL Workfront] -Feld.

1. Klicken **[!UICONTROL Zuordnung hinzufügen]**.

   Das zugeordnete Feld wird in den zugeordneten Feldern angezeigt, die unten auf der Seite aufgeführt sind.

1. Wiederholen Sie die Schritte 5 und 6, bis Sie alle gewünschten Elemente hinzufügen. [!DNL Workfront] -Felder und die entsprechenden [!DNL Workfront DAM] -Felder.

## Zugeordnete Felder löschen

1. Anmelden bei [!DNL Workfront] als Administrator.
1. Klicken Sie auf **[!UICONTROL Hauptmenü]** icon ![](assets/main-menu-icon.png) in der oberen rechten Ecke von [!DNL Adobe Workfront]Klicken Sie auf **[!UICONTROL Einrichtung]** ![](assets/gear-icon-settings.png).

1. Klicken Sie im linken Bereich auf **[!UICONTROL Dokumente]** > **[!UICONTROL Metadatenzuordnung]**.

1. Wählen Sie in der Liste der zugeordneten Felder die Felder aus, die Sie aus der Metadaten-Zuordnung entfernen möchten.
1. Klicken **[!UICONTROL Löschen]**.

   Die vorgesehenen Felder werden nicht mehr zugeordnet. Jetzt, wenn ein Benutzer ein Dokument sendet von [!DNL Workfront] nach [!DNL Workfront DAM], werden die in den gelöschten Feldern enthaltenen Metadaten nicht mit dem Dokument übertragen.

   Ein Dokument, das vor dem Löschen der zugeordneten Felder gesendet wurde, behält die mit ihm gesendeten ursprünglichen Metadaten, einschließlich der Metadaten für die gelöschten Felder, bei.
