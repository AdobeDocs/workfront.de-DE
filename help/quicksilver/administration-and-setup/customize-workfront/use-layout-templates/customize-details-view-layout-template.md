---
title: Detailansicht mithilfe einer Layoutvorlage anpassen
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: Als Workfront-Administrator können Sie mit einer Layoutvorlage festlegen, welche Informationen angezeigt werden, wenn ein Benutzer beim Anzeigen einer Aufgabe, eines Problems, eines Dokuments, eines Programms oder Portfolios den Bereich Details im linken Bereich auswählt.
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: 1474e1dd-9b10-476e-9526-6577efa8d1c2
source-git-commit: 7c624eff8931d206285b6c4d91083f4bf09a88b0
workflow-type: tm+mt
source-wordcount: '558'
ht-degree: 0%

---

# Detailansicht mithilfe einer Layoutvorlage anpassen

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available for all customers in the Preview environment and for a select group of customers in the Production environment.</span>-->

Als Adobe Workfront-Administrator können Sie mit einer Layoutvorlage festlegen, welche Informationen angezeigt werden, wenn ein Benutzer beim Anzeigen einer Aufgabe, eines Problems, eines Dokuments, eines Programms oder Portfolios auf das Detailsymbol (![](assets/project-details-icon.png) ) im linken Bereich klickt.

<!--
or billing record
-->

Sie können auch die Reihenfolge der Informationen ändern, in der diese Informationen angezeigt werden. Beispielsweise können Sie für alle Aufgaben, die Ihren Benutzern angezeigt werden, benutzerdefinierte Forms-Informationen für alle Aufgaben, die Ihren Benutzern angezeigt werden, an den Anfang der Detailansicht verschieben.

Informationen zum Erstellen von Layoutvorlagen finden Sie unter [Erstellen und Verwalten von Layoutvorlagen](../use-layout-templates/create-and-manage-layout-templates.md).

Weitere Informationen zu Layoutvorlagen für Gruppen finden Sie unter [Erstellen und Ändern von Layoutvorlagen für Gruppen](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

Nachdem Sie eine Layoutvorlage konfiguriert haben, müssen Sie sie Benutzern zuweisen, damit die vorgenommenen Änderungen für andere sichtbar sind. Informationen zum Zuweisen einer Layoutvorlage zu Benutzern finden Sie unter [Zuweisen von Benutzern zu einer Layoutvorlage](../use-layout-templates/assign-users-to-layout-template.md).

Die Änderungen, die Sie an der Detailansicht für ein Objekt vornehmen, bestimmen auch die Verfügbarkeit und Reihenfolge der Felder, die Benutzer in den folgenden Bereichen sehen:


* &quot;Objekt erstellen&quot;-Felder, z. B. Aufgabe erstellen

  ![](assets/new-task-dialog.png)


* Bildschirme vom Typ &quot;Objekt bearbeiten&quot;beim Bearbeiten eines Objekts wie &quot;Aufgabe bearbeiten&quot;, &quot;Problem bearbeiten&quot;und &quot;Projekt bearbeiten&quot;

  ![](assets/edit-task-screen.png)


* Bildschirme vom Typ &quot;Objekte bearbeiten&quot;bei der Massenbearbeitung von Objekten Derzeit wird dies für die Bearbeitung von Projekten in großen Mengen unterstützt.

  ![](assets/customize-edit-projects-in-bulk-box-with-layout-template.png)


* Zusammenfassung ![](assets/summary-panel-icon.png) für Listen von Aufgaben und Problemen

  ![](assets/summary-area.png)

  >[!NOTE]
  >
  >Änderungen an den Layoutvorlagen wirken sich nur für die Aufgaben und Probleme aus, die dem angemeldeten Benutzer zugewiesen sind, und betreffen die Reihenfolge und Verfügbarkeit der Felder im Bereich &quot;Zusammenfassung&quot;.

* Konversionsfelder, z. B. &quot;Problem in Aufgabe konvertieren&quot;oder &quot;Problem in Projekt konvertieren&quot;.

  ![Problem in Aufgabenfeld konvertieren](assets/convert-issue-to-task-box.png)

Weitere Informationen zu Layoutvorlagen für Gruppen finden Sie unter [Erstellen und Ändern von Layoutvorlagen für Gruppen](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Abo</td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Um diese Schritte auf Systemebene durchzuführen, benötigen Sie die Zugriffsebene des Systemadministrators.
Um sie für eine Gruppe durchzuführen, müssen Sie Manager dieser Gruppe sein</p> <p><b>HINWEIS</b>: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Anpassen der Ansicht der Benutzer in der Detailansicht

1. Beginnen Sie mit der Arbeit an einer Layoutvorlage, wie in [Erstellen und Verwalten von Layoutvorlagen](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md) beschrieben.
1. Klicken Sie auf den Abwärtspfeil ![](assets/dropdown-arrow-12x12.png) unter **Anpassen, was Benutzer sehen**, und klicken Sie dann auf **Projekt**, **Aufgabe**, **Problem**, **Programm** oder **Portfolio.**
<!--
, or billing record
-->

1. Führen Sie im Abschnitt **Details** einen der folgenden Schritte aus, um anzupassen, was Benutzer in der Detailansicht sehen:

   * Ziehen Sie beliebige Abschnittskopfzeilen ![](assets/move-icon---dots.png) , um ihre Reihenfolge zu ändern.
   * Aktivieren oder deaktivieren Sie die Optionen unter **Überblick** und **Benutzerdefinierter Forms** , um sie ein- oder auszublenden.

     Wenn Sie alle Felder in einem dieser Abschnitte ausblenden, wird der gesamte Abschnitt ausgeblendet.

     Alle Felder sind standardmäßig aktiviert.

1. Fahren Sie mit der Anpassung der Layoutvorlage fort.

   Oder

   Wenn Sie mit dem Anpassen fertig sind, klicken Sie auf **Speichern**.

   >[!TIP]
   >
   >Sie können jederzeit auf Speichern klicken, um den Fortschritt zu speichern, und die Vorlage später weiter ändern.
