---
title: Einrichten der Metadatenzuordnung
user-type: administrator
product-area: system-administration;workfront-integrations
navigation-topic: administrator-integrations
description: Metadaten sind beschreibende Informationen, die mit einem Dokument verknüpft sind. Sie können [!DNL Adobe Workfront] so einrichten, dass Metadaten mit Dokumenten eingefügt werden, die an [!DNL Workfront] Anwendungen gesendet werden.
author: Caroline
feature: System Setup and Administration, Workfront Integrations and Apps
role: Admin
exl-id: 7cf4787d-7cff-489e-bd5b-69db3ff09f6e
source-git-commit: 1ae65d18419bf4235a7c97614b539811643110cc
workflow-type: tm+mt
source-wordcount: '615'
ht-degree: 1%

---

# Einrichten der Metadatenzuordnung

Metadaten sind beschreibende Informationen, die mit einem Dokument verknüpft sind. Sie können &quot;[!DNL Adobe Workfront]&quot;einrichten, um Metadaten mit Dokumenten einzuschließen, die an [!DNL Workfront] -Anwendungen gesendet werden.

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
   <td> <p>Sie müssen ein [!DNL Workfront] -Administrator sein. Weitere Informationen finden Sie unter <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Gewähren des vollen Administratorzugriffs für einen Benutzer</a>.</p> <p><b>HINWEIS</b>: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren [!DNL Workfront] -Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein [!DNL Workfront] -Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Über [!DNL Workfront] Metadaten

Metadaten für Dokumente in [!DNL Workfront] können Informationen wie den zugehörigen Projektnamen, die Aufgabenbeschreibung oder das geplante Abschlussdatum enthalten. Als [!DNL Workfront] -Administrator können Sie [!DNL Workfront] so konfigurieren, dass Metadaten mit Dokumenten von [!DNL Workfront] an die folgenden [!DNL Workfront]-Anwendungen gesendet werden:

* [!DNL Workfront DAM]

Bevor Metadaten mit Dokumenten gesendet werden können, müssen Sie zunächst die Metadaten angeben oder zuordnen, die eingeschlossen werden sollen. Sie können jedes in [!DNL Workfront] verwendete Feld zuordnen. Nachdem Sie die Metadatenzuordnung eingerichtet haben, enthalten alle in eine [!DNL Workfront] -Anwendung hochgeladenen Dokumente die zugeordneten Metadaten.

Wenn ein Benutzer ein Dokument von [!DNL Workfront] an eine [!DNL Workfront] -Anwendung sendet, werden zugeordnete Metadaten entlang des Dokuments übertragen. Während die Version des Dokuments in der [!DNL Workfront]-Anwendung mit [!DNL Workfront] verknüpft ist, werden Änderungen an den Metadaten des Dokuments in [!DNL Workfront] nicht in den Metadaten des Dokuments in der [!DNL Workfront]-Anwendung angezeigt. Wenn ein zugeordnetes Feld in [!DNL Workfront] geändert wird, müssen Sie eine neue Version des Dokuments mit den aktualisierten Metadaten an die [!DNL Workfront]-Anwendung senden.

>[!NOTE]
>
>Sie können Metadaten nur in eine Richtung zuordnen: von [!DNL Workfront] zu [!DNL Workfront DAM]. Metadaten für Dokumente, die mit [!DNL Workfront] von [!DNL Workfront DAM] verknüpft sind, können nicht an Workfront übertragen werden.

Sie können dasselbe [!DNL Workfront] -Feld verschiedenen Metadatenfeldern in [!DNL Workfront DAM] zuordnen, aber Sie können in keiner dieser Anwendungen ein Metadatenfeld für mehrere [!DNL Workfront] -Metadatenfelder verwenden.

Um mehrere [!DNL Workfront] -Felder für den Export in ein Metadatenfeld in einer [!DNL Workfront] -Anwendung zu konfigurieren, erstellen Sie zunächst ein berechnetes benutzerdefiniertes Feld in [!DNL Workfront], um alle einzelnen benutzerdefinierten Felder eines Objekts anzuzeigen. Ordnen Sie dann das berechnete [!DNL Workfront] -Feld einem Metadatenfeld in der [!DNL Workfront] -Anwendung zu. Weitere Informationen zu berechneten benutzerdefinierten Feldern finden Sie unter [Berechnete Felder zu einem Formular hinzufügen](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md).

Bevor Sie Felder für den Metadaten-Zuordnungsprozess zuordnen können, müssen Sie die Anwendung in [!DNL Workfront] aktivieren. Weitere Informationen finden Sie unter [Dokumentintegrationen konfigurieren](../../administration-and-setup/configure-integrations/configure-document-integrations.md).

## Konfigurieren von [!DNL Workfront] zum Senden von Metadaten

1. Klicken Sie auf das Symbol **[!UICONTROL Hauptmenü]** oben rechts in [!DNL Adobe Workfront] und dann auf **[!UICONTROL Setup]** ![](assets/gear-icon-settings.png).![](assets/main-menu-icon.png)

1. Klicken Sie im linken Bereich auf **[!UICONTROL Dokumente]** > **[!UICONTROL Metadatenzuordnung]**.

   ![](assets/metadata-mapping.png)

1. Geben Sie im Feld **[!UICONTROL Source-Feld für Zuordnung auswählen]** den Namen des Workfront-Felds ein, das Sie [!DNL Workfront DAM] zuordnen möchten, und wählen Sie es aus, wenn es in der Liste angezeigt wird.
1. Wählen Sie im Feld **[!UICONTROL Zielfeld für Zuordnung auswählen]** das Feld aus, das mit den Informationen im ausgewählten Feld [!DNL Workfront] gefüllt werden soll.

1. Klicken Sie auf **[!UICONTROL Zuordnung hinzufügen]**.

   Das zugeordnete Feld wird in den zugeordneten Feldern angezeigt, die unten auf der Seite aufgeführt sind.

1. Wiederholen Sie die Schritte 5 und 6, bis Sie alle gewünschten [!DNL Workfront] -Felder und deren entsprechende [!DNL Workfront DAM] -Felder hinzufügen.

## Zugeordnete Felder löschen

1. Melden Sie sich bei [!DNL Workfront] als Administrator an.
1. Klicken Sie auf das Symbol **[!UICONTROL Hauptmenü]** oben rechts in [!DNL Adobe Workfront] und dann auf **[!UICONTROL Setup]** ![](assets/gear-icon-settings.png).![](assets/main-menu-icon.png)

1. Klicken Sie im linken Bereich auf **[!UICONTROL Dokumente]** > **[!UICONTROL Metadatenzuordnung]**.

1. Wählen Sie in der Liste der zugeordneten Felder die Felder aus, die Sie aus der Metadaten-Zuordnung entfernen möchten.
1. Klicken Sie auf **[!UICONTROL Löschen]**.

   Die vorgesehenen Felder werden nicht mehr zugeordnet. Wenn ein Benutzer jetzt ein Dokument von [!DNL Workfront] an [!DNL Workfront DAM] sendet, werden die in den gelöschten Feldern enthaltenen Metadaten nicht mit dem Dokument übertragen.

   Ein Dokument, das vor dem Löschen der zugeordneten Felder gesendet wurde, behält die mit ihm gesendeten ursprünglichen Metadaten, einschließlich der Metadaten für die gelöschten Felder, bei.
