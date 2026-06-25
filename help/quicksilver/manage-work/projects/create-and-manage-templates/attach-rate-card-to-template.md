---
content-type: overview
product-area: templates
navigation-topic: financials
title: Tarifkarte an eine Vorlage anhängen
description: Wenn Sie einer Vorlage eine Tarifkarte zuweisen, wird diese an alle aus der Vorlage erstellten Projekte angehängt.
author: Lisa
feature: Work Management
source-git-commit: 28a1c1cf30c2b4addbcc1b40f5fd65f99685c75c
workflow-type: tm+mt
source-wordcount: '628'
ht-degree: 8%

---

# Tarifkarte an eine Vorlage anhängen

{{highlighted-preview-article-level}}

Wenn Sie einer Vorlage eine Tarifkarte zuweisen, wird diese an alle aus der Vorlage erstellten Projekte angehängt. Die Tarifkarte wird zum Standard im Projekt, kann jedoch bei Bedarf überschrieben werden.

Weitere Informationen zu Tarifkarten finden Sie unter [Tarifkarten verwalten](/help/quicksilver/administration-and-setup/manage-enterprise-operations/manage-rate-cards.md).

Informationen zu Projektvorlagen finden Sie unter [Projektvorlage - Übersicht](/help/quicksilver/manage-work/projects/create-and-manage-templates/project-template-overview.md).

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront-Paket</td> 
   <td>Workflow Ultimate</td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront-Lizenz</td> 
   <td>Standard</td> 
  </tr> 
  <tr> 
   <td>Konfigurationen der Zugriffsebene</td> 
   <td>Zugriff auf Vorlagen bearbeiten</td> 
  </tr> 
  <tr> 
   <td>Objektberechtigungen</td> 
   <td>Verwalten Sie die Berechtigungen für die Tarifkarte mit den Berechtigungen zum Bearbeiten von Abrechnungssätzen</td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) in der Dokumentation zu Workfront.

+++

## Voraussetzungen

Die Tarifkarte, die Sie der Vorlage zuweisen möchten, muss in Workfront erstellt werden. Weitere Informationen finden Sie unter [Tarifkarten verwalten](/help/quicksilver/administration-and-setup/manage-enterprise-operations/manage-rate-cards.md).

Das Feld **Tarifkarte** muss für Vorlagen in Ihrer Layout-Vorlage aktiviert sein.

1. Klicken Sie in der Layout-Vorlage unter **Was Benutzer sehen, anpassen** auf den Abwärtspfeil und dann auf **Vorlage**.
1. Wählen Sie **Abschnitt** das Feld **Tarifkarte** im Bereich **Übersicht** aus.

   Weitere Informationen finden Sie unter [Anpassen der Detailansicht mithilfe einer Layout-Vorlage](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

## Tarifkarte an eine Vorlage anhängen

{{step1-to-templates}}

1. Neue Vorlage erstellen oder vorhandene Vorlage bearbeiten
1. Wählen Sie im Abschnitt Vorlagendetails > Übersicht > Vorlagenzuordnung im Feld **Tarifkarte** eine Tarifkarte aus.

   Es stehen nur Tarifkarten zur Auswahl, für die Sie über Berechtigungen verfügen.
Sie können mit der Eingabe des Namens einer Tarifkarte beginnen, um die Ergebnisliste einzugrenzen.

   ![Wählen Sie in der Vorlage eine Tarifkarte aus](assets/select-rate-card-on-template.png)

1. Speichern Sie die Vorlage, wenn Sie mit der Bearbeitung fertig sind.

   Weitere Informationen zum Erstellen einer Vorlage finden Sie unter [Erstellen einer Projektvorlage](/help/quicksilver/manage-work/projects/create-and-manage-templates/create-template.md).

   Weitere Informationen zum Bearbeiten einer Vorlage finden Sie unter [Projektvorlagen bearbeiten](/help/quicksilver/manage-work/projects/create-and-manage-templates/edit-templates.md).

## Anwenden der Vorlage auf ein Projekt

1. Erstellen Sie ein Projekt mithilfe der Vorlage .

   Es gibt mehrere Möglichkeiten, ein Projekt aus einer Vorlage zu erstellen. Weitere Informationen finden Sie in diesen Artikeln:

   * [Erstellen eines Projekts mithilfe einer Vorlage](/help/quicksilver/manage-work/projects/create-projects/create-project-from-template.md)
   * [Konvertieren einer Aufgabe in ein Projekt](/help/quicksilver/manage-work/tasks/manage-tasks/convert-task-to-project.md)
   * [Konvertieren eines Problems in ein Projekt](/help/quicksilver/manage-work/issues/convert-issues/convert-issue-to-project.md)

   Die Tarifkarte wird automatisch im Projekt gespeichert. Im Abschnitt Übersicht > Projektverknüpfung des Felds Neues Projekt können Sie die Tarifkarte entfernen oder im Feld **Tarifkarte** eine andere Tarifkarte auswählen.

   ![Tarifkarte aus der Vorlage wird in den Projektdetails angezeigt](assets/create-project-from-template-rate-card.png)

   Die Tarifkarte und die zugehörigen Tarife werden im Bereich Projekttarife angezeigt.

   Sie können die Tarifkarte auch aus dem Projekt entfernen oder eine andere Tarifkarte im Bereich Tarife anhängen. Weitere Informationen finden Sie unter [Anhängen einer Tarifkarte an ein Projekt](/help/quicksilver/manage-work/projects/project-finances/attach-rate-card-to-project.md).

   ![Tarifkarte aus der Vorlage im Projekt](assets/template-rates-on-project.png)

   >[!NOTE]
   >
   >Wenn sich ein individueller Tarif auf der Vorlage befindet und der Vorlage auch eine Tarifkarte beigefügt ist, werden beim Erstellen eines Projekts aus der Vorlage sowohl der individuelle Tarif als auch die Tarifkarte in der Liste der Tarife angezeigt.

1. (Optional) Um die Tarifkarte auf ein vorhandenes Projekt anzuwenden, fügen Sie die Vorlage an das Projekt an.

   Wenn Sie die Option **Anpassen und anhängen** in der Vorlagenvorschau verwenden, können Sie das Element **Tarifkarte** im Abschnitt Vorlage anhängen > Optionen auswählen, um die Tarifkarte zum Projekt hinzuzufügen. Deaktivieren Sie das Kontrollkästchen, um die Tarifkarte von der Übertragung zum Projekt auszuschließen.

   Weitere Informationen finden Sie unter [Anhängen einer Vorlage an ein Projekt](/help/quicksilver/manage-work/projects/create-and-manage-templates/attach-template-to-project.md).

1. (Optional) Speichern Sie das Projekt als Vorlage, um die Tarifkarte aus einem bestimmten Projekt in einer Vorlage zu speichern.

   Im Abschnitt Optionen im Feld Als Vorlage speichern können Sie das Element **Tarifkarte** auswählen, um die Tarifkarte zur Vorlage hinzuzufügen. Deaktivieren Sie das Kontrollkästchen, um die Tarifkarte von der Übertragung zur Vorlage auszuschließen.

   Weitere Informationen finden Sie unter [Speichern eines Projekts als Vorlage](/help/quicksilver/manage-work/projects/manage-projects/save-project-as-template.md)



