---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Verwenden von Workflows in der Integration von Experience Manager Assets Essentials
description: Verwenden von Workflows in der Integration von Experience Manager Assets Essentials
author: Courtney, Becky
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: 4c1e5ec1-3fd1-4527-ba8a-9db1a2350f69
source-git-commit: b87839d6c6dbfe978a3e14ef4b448560742f95c3
workflow-type: tm+mt
source-wordcount: '1053'
ht-degree: 0%

---

# Workflows in der Experience Manager Assets-Integration verwenden

Ein Workflow besteht aus einer Reihe von Aktionen, die Workfront mit Adobe Experience Manager as a Cloud Service verbinden. Ein Workfront-Administrator kann Workflows in Workfront konfigurieren und sie dann Projektvorlagen zuweisen. Wenn ein Projekt mit einer Projektvorlage erstellt wird, der ein Workflow zugewiesen ist, werden die im Workflow definierten Aktionen ausgelöst.

>[!NOTE]
>
>Workflows sind nur in einer Adobe Experience Manager as a Cloud Service-Integration verfügbar. Sie sind nicht in Integrationen mit Adobe Experience Manager Assets Essentials verfügbar.


## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

Sie müssen über Folgendes verfügen:

<table>
  <tr>
   <td><strong>Adobe Workfront-Plan*</strong>
   </td>
   <td>Alle
   </td>
  </tr>
  <tr>
   <td><strong>Adobe Workfront-Lizenzen*</strong>
   </td>
   <td>Anforderung oder höher
   </td>
  </tr>
  <tr>
   <td><strong>Produkt</strong>
   </td>
   <td><p>Sie müssen über as a Cloud Service oder Assets Essentials von Experience Manager Assets verfügen und dem Produkt als Benutzer in der Admin Console hinzugefügt werden.</p><p>Sie müssen über Schreibzugriff auf das Repository in Adobe Experience Manager verfügen.</p>
   </td>
  </tr>
  <tr>
   <td><strong>Konfigurationen auf Zugriffsebene*</strong>
   </td>
   <td>Zugriff auf Dokumente bearbeiten
<p>
<strong>Hinweis: </strong>Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <strong>Benutzerdefinierte Zugriffsebenen erstellen oder ändern</strong>.
   </td>
  </tr>
  <tr>
   <td><strong>Objektberechtigungen</strong>
   </td>
   <td>Zugriff auf das Projekt verwalten oder höher 
<p>
Weitere Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <strong>Anfordern des Zugriffs auf Objekte </strong>.
   </td>
  </tr>
</table>

+++

## Voraussetzungen

Bevor Sie beginnen

* Ihr Workfront-Administrator muss Workflows in einer Adobe Experience Manager-Integration konfigurieren. Weitere Informationen finden Sie unter [Konfigurieren der Experience Manager Assets as a Cloud Service-Integration](../../administration-and-setup/configure-integrations/configure-aacs-integration.md#set-up-workflows-optional).

## Workflow zu einer Vorlage hinzufügen

Sie können einen Workflow zu einer Projektvorlage hinzufügen. Der Workflow wird auf alle aus der Vorlage erstellten Projekte angewendet.

1. Öffnen Sie eine Vorlage, indem Sie im Hauptmenü auf **Vorlagen** klicken und dann die Vorlage aus der Liste auswählen.
1. Klicken Sie im linken Navigationsbereich auf **Experience Manager Assets** .

   >[!NOTE]
   >
   >Wenn der Abschnitt &quot;Experience Manager Assets&quot;nicht im linken Navigationsbereich angezeigt wird, hat Ihr Workfront-Administrator die Workflows für Ihr Unternehmen nicht aktiviert. <!--Is this right?-->

1. Wählen Sie im Feld **Integration für automatisierte Workflows auswählen** die Integration mit den Workflows aus, die Sie für aus dieser Vorlage erstellte Projekte verwenden möchten.
1. (Optional) Bearbeiten Sie alle Workflow-Werte, die Sie auf Projekte anwenden möchten, die mit dieser Vorlage erstellt wurden.

   Anweisungen zu bestimmten Workflows finden Sie unter [Workflow-Werte in einem Projekt bearbeiten](#edit-workflow-values-in-a-project) in diesem Artikel.

   In Vorlagen oder Projekten sind nur Workflows verfügbar, die im Experience Manager-Bereich der Einrichtung aktiviert wurden.

1. Ihre Änderungen werden automatisch gespeichert. <!-- do they though??-->

## Workflow zu einem Projekt hinzufügen

Sie können beim Erstellen eines Projekts einen Workflow hinzufügen oder einen Workflow zu einem vorhandenen Projekt hinzufügen. In beiden Fällen verwenden Sie eine Projektvorlage, um den Workflow hinzuzufügen.

### Hinzufügen eines Workflows beim Erstellen eines Projekts

1. Beginnen Sie mit der Erstellung eines Projekts.

   Anweisungen finden Sie unter [Erstellen eines Projekts mit einer Vorlage](/help/quicksilver/manage-work/projects/create-projects/create-project-from-template.md).

1. Wählen Sie bei der Auswahl einer Vorlage für das Projekt die Vorlage aus, die die Workflows enthält, die Sie für dieses Projekt verwenden möchten.
1. (Optional) Bearbeiten Sie alle Workflow-Werte für das Projekt, wie unter [Workflow-Werte in einem Projekt bearbeiten](#edit-workflow-values-in-a-project) beschrieben.

   In Vorlagen oder Projekten sind nur Workflows verfügbar, die im Experience Manager-Bereich der Einrichtung aktiviert wurden.


### Hinzufügen eines Workflows zu einem vorhandenen Projekt

>[!NOTE]
>
>Workflows, die bei der Erstellung eines Projekts ausgeführt werden (z. B. die Erstellung eines verknüpften Ordners), werden nicht ausgeführt, wenn die Vorlage an ein vorhandenes Projekt angehängt wird. Sie werden nur ausgeführt, wenn ein Projekt aus einer Vorlage erstellt wird.

1. Fügen Sie dem Projekt eine Vorlage hinzu.

   Anweisungen finden Sie unter [Anhängen einer Vorlage an ein Projekt](/help/quicksilver/manage-work/projects/create-and-manage-templates/attach-template-to-project.md).

1. Wählen Sie bei der Auswahl einer Vorlage für das Projekt die Vorlage aus, die die Workflows enthält, die Sie für dieses Projekt verwenden möchten.
1. (Optional) Bearbeiten Sie alle Workflow-Werte für das Projekt, wie unter [Workflow-Werte in einem Projekt bearbeiten](#edit-workflow-values-in-a-project) beschrieben.

   In Vorlagen oder Projekten sind nur Workflows verfügbar, die im Experience Manager-Bereich der Einrichtung aktiviert wurden.



### Workflow-Werte in einem Projekt bearbeiten

Sie können Workflow-Werte auf Projektebene bearbeiten. Workflow-Werte auf Projektebene überschreiben die Werte, die in der Projektvorlage festgelegt sind, wodurch die in der Adobe Experience Manager Assets-Integration festgelegten Standardwerte außer Kraft gesetzt werden.

Alle Workflow-Werte finden Sie unter:

* Der Abschnitt Workflows oder verknüpfte Ordner im Fenster Projekt erstellen oder Projekt bearbeiten .
* Der Abschnitt Adobe Experience Manager im linken Navigationsbereich.


  >[!NOTE]
  >
  >Wenn diese Bereiche nicht sichtbar sind, hat Ihr Workfront-Administrator die Workflows für Ihr Unternehmen nicht aktiviert.



#### Verknüpfte Ordner

>[!NOTE]
>
>Da verknüpfte Ordner beim Erstellen des Projekts erstellt werden, ist die Bearbeitung des Workflows für verknüpfte Ordner in einem vorhandenen Projekt nicht wirksam. Die Bearbeitung dieser Werte beim Erstellen eines Projekts funktioniert erwartungsgemäß.

So bearbeiten Sie den Workflow für verknüpfte Ordner:

1. Schalten Sie den Ordner **[!UICONTROL Verknüpften Ordner erstellen]** nach Bedarf ein oder aus. Wenn Sie sie aktivieren, können Sie die Konfiguration des verknüpften Ordners bearbeiten.

   Weitere Informationen zur Konfiguration des verknüpften Ordners finden Sie unter [Erstellen von mit Adobe Experience Manager verknüpften Ordnern](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md#create-adobe-experience-manager-linked-folders) im Artikel [Konfigurieren der Integration von [!UICONTROL Experience Manager Assets as a Cloud Service]](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md) .

1. (Optional) Wenn Sie möchten, dass die Ordnerstruktur nur erstellt wird, wenn bestimmte Werte in einem benutzerdefinierten Formular vorhanden sind, das an das Projekt angehängt ist, klicken Sie auf &quot;**Filter anwenden**&quot;für diese Ordnerstruktur und wählen Sie dann das benutzerdefinierte Formular aus, das das Feld, das Feld und den Feldwert enthält. Wenn das Feld im benutzerdefinierten Formular, das an das neue Projekt angehängt ist, den ausgewählten Wert enthält, wird die Ordnerstruktur erstellt.
1. (Optional) Beim Konfigurieren von Ordnernamen können Sie aus den folgenden Optionen auswählen:

   * **Name**: Geben Sie einen Namen für den Ordner ein.

   * **Objektdaten**: Wählen Sie die Quelle für den Ordnernamen aus, z. B. den Projektnamen.

   * **Benutzerdefinierte Formulardaten**: Wählen Sie die benutzerdefinierten Formulardaten aus, die als Ordnername verwendet werden sollen.

     Die Verwendung benutzerdefinierter Formulardaten für Ordnernamen ist nur auf Vorlagenebene verfügbar und kann nicht auf Integrationsebene konfiguriert werden.

     Wenn ein Ordnername auf benutzerdefinierte Daten festgelegt ist, die nicht in dem benutzerdefinierten für , das an das Projekt angehängt ist, vorhanden sind, wird eine zufällige ID als Ordnername zugewiesen.

1. Um die Ordnerstruktur anzuzeigen, klicken Sie auf das Symbol **Vorschau** ![Vorschau-Symbol](assets/preview-icon.png)
1. Klicken Sie auf **[!UICONTROL Speichern]**.

#### Assets veröffentlichen

So bearbeiten Sie den Workflow zum Veröffentlichen von Assets:

1. Schalten Sie die **Publish-Assets automatisch** ein oder aus.
1. (Bedingt) Wenn Sie die Veröffentlichung aktivieren, wählen Sie aus, ob Sie die Veröffentlichung im Veröffentlichungsdienst, im Brand Portal oder beidem durchführen möchten.
1. Klicken Sie auf **[!UICONTROL Speichern]**.
