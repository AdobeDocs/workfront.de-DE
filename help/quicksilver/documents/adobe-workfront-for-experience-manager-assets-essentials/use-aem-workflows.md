---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Verwenden von Workflows in der Integration von Experience Manager Assets Essentials
description: Verwenden von Workflows in der Integration von Experience Manager Assets Essentials
author: Courtney, Becky
feature: Digital Content and Documents, Workfront Integrations and Apps
source-git-commit: 038f5f3c941ea69feb43492a30b5abea39f7c932
workflow-type: tm+mt
source-wordcount: '738'
ht-degree: 0%

---

# Workflows in der Experience Manager Assets-Integration verwenden

Ein Workflow besteht aus einer Reihe von Aktionen, die Workfront mit Adobe Experience Manager as a Cloud Service verbinden. Ein Workfront-Administrator kann Workflows in Workfront konfigurieren und sie dann Projektvorlagen zuweisen. Wenn ein Projekt mit einer Projektvorlage erstellt wird, der ein Workflow zugewiesen ist, werden die im Workflow definierten Aktionen ausgelöst.

>[!NOTE]
>
>Workflows sind nur in einer Adobe Experience Manager as a Cloud Service-Integration verfügbar. Sie sind nicht in Integrationen mit Adobe Experience Manager Assets Essentials verfügbar.


## Zugriffsanforderungen

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
   <td>Anforderung oder höher
   </td>
  </tr>
  <tr>
   <td><strong>Produkt</strong>
   </td>
   <td><p>Sie müssen über Experience Manager Assets as a Cloud Service oder Assets Essentials verfügen und dem Produkt als Benutzer in der Admin Console hinzugefügt werden.</p><p>Sie müssen über Schreibzugriff auf das Repository in Adobe Experience Manager verfügen, um verknüpfte Ordner erstellen zu können.</p>&gt;
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
Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <strong>Zugriff auf Objekte anfordern </strong>.
   </td>
  </tr>
</table>

## Voraussetzungen

Bevor Sie beginnen,

* Ihr Workfront-Administrator muss Workflows in einer Adobe Experience Manager-Integration konfigurieren. Weitere Informationen finden Sie unter [Konfigurieren der as a Cloud Service Integration von Experience Manager Assets](../../administration-and-setup/configure-integrations/configure-aacs-integration.md#set-up-workflows-optional).

## Workflow zu einer Vorlage hinzufügen

Sie können einen Workflow zu einer Projektvorlage hinzufügen. Der Workflow wird auf alle aus der Vorlage erstellten Projekte angewendet.

1. <!-- main menu snippet??--> Öffnen Sie eine Vorlage durch Klicken auf **Vorlagen** im Hauptmenü und wählen Sie dann die Vorlage aus der Liste aus.
1. Klicken **Experience Manager Assets** im linken Navigationsbereich.

   >[!NOTE]
   >
   >Wenn der Abschnitt Experience Manager Assets nicht im linken Navigationsbereich angezeigt wird, hat Ihr Workfront-Administrator die Workflows für Ihr Unternehmen nicht aktiviert. <!--Is this right?-->

1. Im **Auswählen einer Integration für das Feld &quot;Automatisierte Workflows&quot;**, wählen Sie die Integration mit den Workflows aus, die Sie für Projekte verwenden möchten, die aus dieser Vorlage erstellt wurden.
1. (Optional) Bearbeiten Sie alle Workflow-Werte, die Sie auf Projekte anwenden möchten, die mit dieser Vorlage erstellt wurden.

   Um beispielsweise einen verknüpften Ordner an einem anderen Speicherort als dem Standardwert zu erstellen, geben Sie den verknüpften Ordnerspeicherort ein.

   In Vorlagen oder Projekten sind nur Workflows verfügbar, die im Experience Manager-Bereich der Einrichtung aktiviert wurden.

1. Ihre Änderungen werden automatisch gespeichert. <!-- do they though??-->

## Workflow zu einem Projekt hinzufügen

Sie können beim Erstellen eines Projekts einen Workflow hinzufügen oder einen Workflow zu einem vorhandenen Projekt hinzufügen. In beiden Fällen verwenden Sie eine Projektvorlage, um den Workflow hinzuzufügen.

### Workflow beim Erstellen eines Projekts hinzufügen

1. Erstellen Sie ein Projekt.

   Anweisungen finden Sie unter [Erstellen eines Projekts mit einer Vorlage](/help/quicksilver/manage-work/projects/create-projects/create-project-from-template.md).

1. Wählen Sie bei der Auswahl einer Vorlage für das Projekt die Vorlage aus, die die Workflows enthält, die Sie für dieses Projekt verwenden möchten.
1. (Optional) Bearbeiten Sie alle Workflow-Werte für das Projekt, wie unter [Workflow-Werte in einem Projekt bearbeiten](#edit-workflow-values-in-a-project).

   In Vorlagen oder Projekten sind nur Workflows verfügbar, die im Experience Manager-Bereich der Einrichtung aktiviert wurden.


### Hinzufügen eines Workflows zu einem vorhandenen Projekt

1. Beginnen Sie mit dem Hinzufügen einer Vorlage zum Projekt.

   Anweisungen finden Sie unter [Eine Vorlage an ein Projekt anhängen](/help/quicksilver/manage-work/projects/create-and-manage-templates/attach-template-to-project.md).

1. Wählen Sie bei der Auswahl einer Vorlage für das Projekt die Vorlage aus, die die Workflows enthält, die Sie für dieses Projekt verwenden möchten.
1. (Optional) Bearbeiten Sie alle Workflow-Werte für das Projekt, wie unter [Workflow-Werte in einem Projekt bearbeiten](#edit-workflow-values-in-a-project).

### Workflow-Werte in einem Projekt bearbeiten

Sie können Workflow-Werte auf Projektebene bearbeiten. Workflow-Werte auf Projektebene überschreiben die Werte, die in der Projektvorlage festgelegt sind, wodurch die in der Adobe Experience Manager Assets-Integration festgelegten Standardwerte außer Kraft gesetzt werden.

Alle Workflow-Werte finden Sie unter:

* Der Abschnitt Workflows des Fensters Projekt erstellen oder Projekt bearbeiten .
* Der Abschnitt Adobe Experience Manager im linken Navigationsbereich.


   >[!NOTE]
   >
   >Wenn diese Bereiche nicht sichtbar sind, hat Ihr Workfront-Administrator die Workflows für Ihr Unternehmen nicht aktiviert.

#### Verknüpfte Ordner

So bearbeiten Sie den Workflow für verknüpfte Ordner:

1. Umschalten zwischen **[!UICONTROL Verknüpften Ordner erstellen]** auf.
1. Wählen Sie einen Ordnerpfad aus, um anzugeben, wo alle mit dieser Integration verknüpften Ordner gespeichert werden sollen.
1. Klicken Sie auf Speichern , wenn Sie das Fenster Projekt erstellen oder Projekt bearbeiten verwenden.

   Oder

   Wenn Sie sich im Adobe Experience Manager-Bereich befinden, werden Ihre Änderungen automatisch gespeichert. <!--Do they though?-->

