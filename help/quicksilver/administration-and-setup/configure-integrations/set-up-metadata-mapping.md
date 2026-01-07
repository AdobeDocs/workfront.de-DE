---
title: Einrichten der Metadatenzuordnung
user-type: administrator
product-area: system-administration;workfront-integrations
navigation-topic: administrator-integrations
description: Metadaten sind beschreibende Informationen, die mit einem Dokument verknüpft sind. Sie können so einrichten [!DNL Adobe Workfront]  dass Metadaten in Dokumente aufgenommen werden, die an - [!DNL Workfront]  gesendet werden.
author: Courtney, Becky
feature: System Setup and Administration, Workfront Integrations and Apps
role: Admin
exl-id: 7cf4787d-7cff-489e-bd5b-69db3ff09f6e
source-git-commit: 53596271a838733b858c0b14a4e22b07a7cd20f6
workflow-type: tm+mt
source-wordcount: '558'
ht-degree: 5%

---

# Einrichten der Metadatenzuordnung

Metadaten sind beschreibende Informationen, die mit einem Dokument verknüpft sind. Sie können [!DNL Adobe Workfront] so einrichten, dass Metadaten in Dokumente eingefügt werden, die an [!DNL Workfront] Programme gesendet werden.

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

<table>
  <tr>
   <td>Adobe Workfront-Paket
   </td>
   <td> <p>Prime oder Ultimate</p>
    <p>Workflow Ultimate</p>
   </td>
  </tr>
  <tr>
   <td>Adobe Workfront-Lizenzen
   </td>
   <td><p>Standard</p>
   <p>Plan</p>
   </td>
  </tr>
   <tr>
   <td>Konfigurationen der Zugriffsebene
   </td>
   <td>Sie müssen [!DNL Workfront] sein.
   </td>
  </tr>
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Über [!DNL Workfront] Metadaten

Metadaten für Dokumente in [!DNL Workfront] können Informationen wie den zugehörigen Projektnamen, die Aufgabenbeschreibung oder das geplante Abschlussdatum enthalten. Als [!DNL Workfront] können Sie [!DNL Workfront] so konfigurieren, dass Metadaten in Dokumente aufgenommen werden, die von [!DNL Workfront] an die folgenden [!DNL Workfront]-Programme gesendet werden:

* [!DNL Workfront DAM]

Bevor Metadaten mit Dokumenten gesendet werden können, müssen Sie zunächst die Metadaten angeben oder zuordnen, die Sie einbeziehen möchten. Sie können jedes Feld zuordnen, das in [!DNL Workfront] verwendet wird. Nachdem Sie die Metadatenzuordnung eingerichtet haben, enthalten alle Dokumente, die in ein [!DNL Workfront]-Programm hochgeladen werden, die zugeordneten Metadaten.

Wenn ein(e) Benutzende(r) ein Dokument von [!DNL Workfront] an eine [!DNL Workfront]-Anwendung sendet, werden zugeordnete Metadaten zusammen mit dem Dokument übertragen. Während die Version des Dokuments in der [!DNL Workfront]-Anwendung mit [!DNL Workfront] verknüpft ist, werden Änderungen an den Metadaten des Dokuments in [!DNL Workfront] nicht in den Metadaten des Dokuments in der [!DNL Workfront]-Anwendung übernommen. Wenn ein zugeordnetes Feld in [!DNL Workfront] geändert wird, müssen Sie eine neue Version des Dokuments mit den aktualisierten Metadaten an die [!DNL Workfront]-Anwendung senden.

>[!NOTE]
>
>Metadaten können nur in eine Richtung zugeordnet werden: von [!DNL Workfront] zu [!DNL Workfront DAM]. Metadaten für Dokumente, die mit [!DNL Workfront] von [!DNL Workfront DAM] verknüpft sind, können nicht an Workfront übertragen werden.

Sie können dasselbe [!DNL Workfront] verschiedenen Metadatenfeldern in [!DNL Workfront DAM] zuordnen, aber Sie können in keinem dieser Programme ein Metadatenfeld für mehrere [!DNL Workfront] Metadatenfelder verwenden.

Um mehrere [!DNL Workfront] zu konfigurieren, die in ein Metadatenfeld in einem [!DNL Workfront]-Programm exportiert werden, erstellen Sie zunächst ein berechnetes benutzerdefiniertes Feld, [!DNL Workfront] alle individuellen Felder eines Objekts anzuzeigen. Ordnen Sie dann das berechnete [!DNL Workfront] einem Metadatenfeld in der [!DNL Workfront] zu. Weitere Informationen zu berechneten benutzerdefinierten Feldern finden Sie unter [Hinzufügen berechneter Felder zu einem Formular](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md).

Bevor Sie Felder für den Metadatenzuordnungsprozess zuordnen können, müssen Sie die Anwendung in [!DNL Workfront] aktivieren. Weitere Informationen finden Sie unter [Konfigurieren von Dokumentintegrationen](../../administration-and-setup/configure-integrations/configure-document-integrations.md).

## Konfigurieren von [!DNL Workfront] zum Senden von Metadaten

{{step-1-to-setup}}

1. Klicken Sie im linken Bereich auf **[!UICONTROL Dokumente]** > **[!UICONTROL Metadatenzuordnung]**.

   ![Metadatenzuordnung](assets/metadata-mapping.png)

1. Geben **[!UICONTROL in das Feld Source-Feld für Zuordnung auswählen]** den Namen des Workfront-Felds ein, dem Sie [!DNL Workfront DAM] zuordnen möchten, und wählen Sie es aus, wenn es in der Liste angezeigt wird.
1. Wählen **[!UICONTROL im Feld Zielfeld für Zuordnung auswählen]** das Feld aus, das Sie mit den Informationen im ausgewählten [!DNL Workfront] füllen möchten.

1. Klicken Sie **[!UICONTROL Zuordnung hinzufügen]**.

   Das zugeordnete Feld wird in den zugeordneten Feldern angezeigt, die unten auf der Seite aufgeführt sind.

1. Wiederholen Sie die Schritte 5 und 6, bis Sie alle gewünschten [!DNL Workfront] und die entsprechenden [!DNL Workfront DAM] Felder hinzufügen.

## Zugeordnete Felder löschen

1. Melden Sie sich bei [!DNL Workfront] als Admin an.

{{step-1-to-setup}}

1. Klicken Sie im linken Bereich auf **[!UICONTROL Dokumente]** > **[!UICONTROL Metadatenzuordnung]**.

1. Wählen Sie in der Liste der zugeordneten Felder die Felder aus, die Sie aus der Metadatenzuordnung entfernen möchten.
1. Klicken Sie auf **[!UICONTROL Löschen]**.

   Die angegebenen Felder werden nicht mehr zugeordnet. Wenn ein(e) Benutzende(r) jetzt ein Dokument von [!DNL Workfront] an [!DNL Workfront DAM] sendet, werden die in den gelöschten Feldern enthaltenen Metadaten nicht mit dem Dokument übertragen.

   Ein Dokument, das vor dem Löschen der zugeordneten Felder gesendet wird, behält die ursprünglichen Metadaten bei, die damit gesendet wurden, einschließlich der Metadaten für die gelöschten Felder.
