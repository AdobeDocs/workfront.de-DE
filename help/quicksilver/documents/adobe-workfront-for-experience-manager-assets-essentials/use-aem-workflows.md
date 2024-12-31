---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Verwenden von Workflows in der Experience Manager Assets Essentials-Integration
description: Verwenden von Workflows in der Experience Manager Assets Essentials-Integration
author: Courtney, Becky
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: 4c1e5ec1-3fd1-4527-ba8a-9db1a2350f69
source-git-commit: 99924f690c53584c090d19fff90d23d84ec306d4
workflow-type: tm+mt
source-wordcount: '1053'
ht-degree: 0%

---

# Verwenden von Workflows in der Experience Manager Assets-Integration

Ein Workflow ist eine Reihe von Aktionen, die Workfront mit Adobe Experience Manager as a Cloud Service verbinden. Ein Workfront-Administrator kann Workflows in Workfront konfigurieren und sie dann Projektvorlagen zuweisen.

Wenn ein Projekt mithilfe einer Projektvorlage erstellt wird, der ein Workflow zugewiesen ist, werden die im Workflow definierten Aktionen ausgelöst.

>[!NOTE]
>
>Workflows sind nur in einer Adobe Experience Manager as a Cloud Service-Integration verfügbar. Sie sind nicht in Integrationen mit Adobe Experience Manager Assets Essentials verfügbar.


## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über Folgendes verfügen:

<table>
  <tr>
   <td><strong>Adobe Workfront-Plan*</strong>
   </td>
   <td>Beliebig
   </td>
  </tr>
  <tr>
   <td><strong>Adobe Workfront-Lizenzen*</strong>
   </td>
   <td>Anfrage oder höher
   </td>
  </tr>
  <tr>
   <td><strong>Produkt</strong>
   </td>
   <td><p>Sie müssen über Experience Manager Assets as a Cloud Service oder Assets Essentials verfügen und Sie müssen dem Produkt als Benutzer in der Admin Console hinzugefügt werden.</p><p>Sie müssen Schreibzugriff auf das Repository in Adobe Experience Manager haben.</p>
   </td>
  </tr>
  <tr>
   <td><strong>Konfigurationen der Zugriffsebene*</strong>
   </td>
   <td>Zugriff auf Dokumente bearbeiten
<p>
<strong>Hinweis: </strong>Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Einschränkungen in Ihrer Zugriffsebene festgelegt hat. Informationen dazu, wie Workfront-Admins Ihre Zugriffsebene ändern können, finden Sie unter <strong>Erstellen oder Ändern benutzerdefinierter Zugriffsebenen</strong>.
   </td>
  </tr>
  <tr>
   <td><strong>Objektberechtigungen</strong>
   </td>
   <td>Zugriff verwalten oder höher für das Projekt 
<p>
Informationen zum Anfordern zusätzlicher Zugriffsberechtigungen finden Sie unter <strong>Anfordern von Zugriffsberechtigungen für Objekte </strong>.
   </td>
  </tr>
</table>

+++

## Voraussetzungen

Bevor Sie beginnen,

* Ihr Workfront-Administrator muss Workflows in einer Adobe Experience Manager-Integration konfigurieren. Weitere Informationen finden Sie unter [Konfigurieren der Experience Manager Assets as a Cloud Service-Integration](../../administration-and-setup/configure-integrations/configure-aacs-integration.md#set-up-workflows-optional).

## Hinzufügen eines Workflows zu einer Vorlage

Sie können einen Workflow zu einer Projektvorlage hinzufügen. Der Workflow wird auf alle Projekte angewendet, die aus der Vorlage erstellt wurden.

1. Öffnen Sie eine Vorlage, indem **Hauptmenü auf** Vorlagen“ klicken und die Vorlage dann aus der Liste auswählen.
1. Klicken Sie im **Navigationsbereich auf** Experience Manager Assets.

   >[!NOTE]
   >
   >Wenn der Abschnitt Experience Manager Assets im linken Navigationsbereich nicht sichtbar ist, hat Ihr Workfront-Administrator keine Workflows für Ihr Unternehmen aktiviert. <!--Is this right?-->

1. Wählen Sie im Feld **Integration für automatisierte Workflows auswählen** die Integration mit den Workflows aus, die Sie für Projekte verwenden möchten, die aus dieser Vorlage erstellt wurden.
1. (Optional) Bearbeiten Sie alle Workflow-Werte, die Sie auf Projekte anwenden möchten, die aus dieser Vorlage erstellt wurden.

   Anweisungen zu bestimmten Workflows finden Sie unter [Bearbeiten von Workflow-Werten in einem Projekt](#edit-workflow-values-in-a-project) in diesem Artikel.

   Nur Workflows, die im Bereich Experience Manager von Setup aktiviert wurden, sind in Vorlagen oder Projekten verfügbar.

1. Ihre Änderungen werden automatisch gespeichert. <!-- do they though??-->

## Hinzufügen eines Workflows zu einem Projekt

Sie können beim Erstellen eines Projekts einen Workflow hinzufügen oder einen Workflow zu einem vorhandenen Projekt hinzufügen. In beiden Fällen verwenden Sie eine Projektvorlage, um den Workflow hinzuzufügen.

### Hinzufügen eines Workflows beim Erstellen eines Projekts

1. Erstellen Sie ein Projekt.

   Anweisungen finden Sie unter [Erstellen eines Projekts mithilfe einer Vorlage](/help/quicksilver/manage-work/projects/create-projects/create-project-from-template.md).

1. Wählen Sie bei der Auswahl einer Vorlage für das Projekt die Vorlage aus, die die Workflows enthält, die Sie für dieses Projekt verwenden möchten.
1. (Optional) Bearbeiten Sie alle Workflow-Werte für das Projekt, wie unter [Bearbeiten von Workflow-Werten in einem Projekt](#edit-workflow-values-in-a-project) beschrieben.

   Nur Workflows, die im Bereich Experience Manager von Setup aktiviert wurden, sind in Vorlagen oder Projekten verfügbar.


### Hinzufügen eines Workflows zu einem vorhandenen Projekt

>[!NOTE]
>
>Workflows, die beim Erstellen eines Projekts ausgeführt werden (z. B. Erstellung verknüpfter Ordner), werden nicht ausgeführt, wenn die Vorlage an ein vorhandenes Projekt angehängt wird. Sie werden nur ausgeführt, wenn ein Projekt über eine Vorlage erstellt wird.

1. Beginnen Sie mit dem Hinzufügen einer Vorlage zum Projekt.

   Anweisungen finden Sie unter [Anhängen einer Vorlage an ein Projekt](/help/quicksilver/manage-work/projects/create-and-manage-templates/attach-template-to-project.md).

1. Wählen Sie bei der Auswahl einer Vorlage für das Projekt die Vorlage aus, die die Workflows enthält, die Sie für dieses Projekt verwenden möchten.
1. (Optional) Bearbeiten Sie alle Workflow-Werte für das Projekt, wie unter [Bearbeiten von Workflow-Werten in einem Projekt](#edit-workflow-values-in-a-project) beschrieben.

   Nur Workflows, die im Bereich Experience Manager von Setup aktiviert wurden, sind in Vorlagen oder Projekten verfügbar.



### Workflow-Werte in einem Projekt bearbeiten

Sie können Workflow-Werte auf Projektebene bearbeiten. Workflow-Werte auf Projektebene überschreiben die in der Projektvorlage festgelegten Werte, die die in der Adobe Experience Manager Assets-Integration festgelegten Standardwerte überschreiben.

Alle Workflow-Werte finden Sie unter:

* Der Abschnitt Workflows oder Verknüpfte Ordner im Fenster Projekt erstellen oder Projekt bearbeiten .
* Der Abschnitt Adobe Experience Manager der linken Navigationsleiste.


  >[!NOTE]
  >
  >Wenn diese Bereiche nicht sichtbar sind, hat Ihr Workfront-Administrator Workflows für Ihr Unternehmen nicht aktiviert.



#### Verknüpfte Ordner

>[!NOTE]
>
>Da verknüpfte Ordner beim Erstellen des Projekts erstellt werden, ist die Bearbeitung des Workflows „Verknüpfter Ordner“ für ein vorhandenes Projekt ineffektiv. Das Bearbeiten dieser Werte beim Erstellen eines Projekts funktioniert erwartungsgemäß.

So bearbeiten Sie den Workflow für verknüpfte Ordner:

1. Schalten Sie den **[!UICONTROL Verknüpften Ordner erstellen]** nach Bedarf ein oder aus. Wenn Sie sie aktivieren, können Sie die Konfiguration Verknüpfter Ordner bearbeiten.

   Weitere Informationen zur Konfiguration verknüpfter Ordner finden Sie unter [Erstellen verknüpfter Adobe Experience Manager-Ordner](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md#create-adobe-experience-manager-linked-folders) im Artikel [Konfigurieren der [!UICONTROL Experience Manager Assets as a Cloud Service]-Integration](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md).

1. (Optional) Wenn die Ordnerstruktur nur erstellt werden soll, wenn bestimmte Werte in einem benutzerdefinierten Formular vorhanden sind, das an das Projekt angehängt ist, klicken Sie auf **Filter anwenden** für diese Ordnerstruktur und wählen Sie dann das benutzerdefinierte Formular aus, das das Feld, das Feld und den Feldwert enthält. Wenn das Feld im benutzerdefinierten Formular, das an das neue Projekt angehängt ist, den ausgewählten Wert enthält, wird die Ordnerstruktur erstellt.
1. (Optional) Bei der Konfiguration von Ordnernamen können Sie aus den folgenden Optionen auswählen:

   * **Name**: Geben Sie einen Namen für den Ordner ein.

   * **Objektdaten**: Wählen Sie die Quelle für den Ordnernamen aus, z. B. Projektnamen.

   * **Benutzerdefinierte Formulardaten**: Wählen Sie die benutzerdefinierten Formulardaten aus, die als Ordnername verwendet werden sollen.

     Die Verwendung benutzerdefinierter Formulardaten für Ordnernamen ist nur auf Vorlagenebene verfügbar und kann nicht auf Integrationsebene konfiguriert werden.

     Wenn ein Ordnername auf benutzerdefinierte Daten festgelegt ist, die im benutzerdefinierten für, das an das Projekt angehängt ist, nicht vorhanden sind, wird eine zufällige ID als Ordnername zugewiesen.

1. Um die Ordnerstruktur anzuzeigen, klicken Sie auf das Symbol **Vorschau** ![Vorschau](assets/preview-icon.png) .
1. Klicken Sie auf **[!UICONTROL Speichern]**.

#### Veröffentlichen von Assets

So bearbeiten Sie den Workflow zum Veröffentlichen von Assets:

1. **Publish-Assets automatisch ein** oder aus.
1. (Bedingt) Wenn Sie die Veröffentlichung aktivieren, wählen Sie aus, ob Sie im Veröffentlichungs-Service, Brand Portal oder in beiden veröffentlichen möchten.
1. Klicken Sie auf **[!UICONTROL Speichern]**.
