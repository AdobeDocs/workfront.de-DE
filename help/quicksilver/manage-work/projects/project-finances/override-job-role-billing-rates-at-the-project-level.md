---
product-area: projects
navigation-topic: financials
title: Aufgabengebiet-Abrechnungssätze auf Projektebene überschreiben
description: Als Projekt-Manager können Sie den Abrechnungssatz für ein Aufgabengebiet in einem bestimmten Projekt angeben. Dieser Abrechnungssatz auf Projektebene überschreibt den Abrechnungssatz auf Systemebene für dieses Aufgabengebiet. Workfront verwendet zur Berechnung des Umsatzes den Abrechnungssatz auf Projektebene des Aufgabengebiets, anstatt den Abrechnungssatz auf Systemebene zu verwenden.
author: Lisa
feature: Work Management
exl-id: b7a33459-6929-4611-8546-06ca979e5dbe
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: b9e0747a58618353caf3ce1c7e8521d22d2b412d
workflow-type: tm+mt
source-wordcount: '856'
ht-degree: 6%

---

# Überschreiben von Abrechnungssätzen für Aufgabengebiete auf Projektebene

{{highlighted-preview}}

Als Projekt-Manager können Sie den Abrechnungssatz für ein Aufgabengebiet in einem bestimmten Projekt angeben. Dieser Abrechnungssatz auf Projektebene überschreibt den Abrechnungssatz auf Systemebene für dieses Aufgabengebiet. Workfront verwendet zur Berechnung des Umsatzes den Abrechnungssatz auf Projektebene des Aufgabengebiets, anstatt den Abrechnungssatz auf Systemebene zu verwenden.

In diesem Artikel wird beschrieben, wie Sie die Abrechnungssätze für Systemaufgaben für ein Projekt überschreiben können.

Allgemeine Informationen zum Überschreiben der Verrechnungssätze für Aufgabengebiete für Projekte und zur Berechnung des Projektumsatzes finden Sie unter [Übersicht über das Überschreiben von Verrechnungssätzen und die Berechnung des Umsatzes für ein Projekt](/help/quicksilver/manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).

Weitere Informationen dazu, welches Aufgabengebiet zur Berechnung des Umsatzes für das Projekt verwendet wird, finden Sie [&#x200B; Abschnitt „Übersicht über Umsatz- und &#x200B;](/help/quicksilver/manage-work/projects/project-finances/overview-revenue-cost-hierarchy.md)&quot; und [Umsatzberechnungen für Aufgaben basierend auf Benutzer- und &#x200B;](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md#revenue-calculations-for-tasks-based-on-user-and-role-assignments)&quot; im Artikel [Übersicht über Abrechnung und Umsatz](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

>[!NOTE]
>
>Bei tatsächlichen Einnahmen sollten die Abrechnungssätze, die auf Stunden angewendet werden, die einem als „In Rechnung gestellt“ markierten Abrechnungs-Datensatz hinzugefügt werden, nicht von Abrechnungssatz-Überschreibungen beeinflusst werden, die nach der Abrechnung des Abrechnungs-Datensatzes auftreten.

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront-Paket</td> 
   <td> <p>So überschreiben Sie einen Abrechnungssatz für ein Aufgabengebiet für ein Projekt: Beliebiges Workfront- oder Workflow-Paket</p>
        <p>So wenden Sie Attribute auf das Aufgabengebiet an: Workflow-Ultimate</p> </td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront-Lizenz</td> 
   <td>
   <p>Standard</p>
   <p>Abo</p></td> 
  </tr> 
  <tr> 
   <td>Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriff auf Projekte und Finanzdaten bearbeiten</p> <p>Administratorzugriff für Aufgabengebiete</p></td> 
  </tr> 
  <tr> 
   <td>Objektberechtigungen</td> 
   <td>Verwalten Sie Berechtigungen für das Projekt, das die Option Finanzdaten bearbeiten enthält. </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) in der Dokumentation zu Workfront.

+++

## Überschreiben von Abrechnungssätzen für Aufgabengebiete auf Projektebene

Wenn Sie den Abrechnungssatz eines Vorgangs für ein Projekt überschreiben, können Sie ein Gültigkeitsdatum zuweisen, und jeder Datumsbereich hat einen anderen Satz. Wenn Sie keine Gültigkeitsdaten zuordnen, wird die von Ihnen eingegebene Abrechnungssatzüberschreibungen für die gesamte Projektdauer zur Berechnung des Umsatzes verwendet.

Sie können einer Projektvorlage neue Abrechnungssätze hinzufügen, die beim Erstellen des Projekts aus dieser Vorlage zu Projekt-Abrechnungssätzen werden. Informationen zum Bearbeiten von Vorlagen finden Sie unter [Projektvorlagen bearbeiten](/help/quicksilver/manage-work/projects/create-and-manage-templates/edit-templates.md).

>[!TIP]
>
>Sie können Benutzerabrechnungssätze für ein Projekt nur überschreiben, wenn Sie über das Workflow-Ultimate-Paket verfügen.

So überschreiben Sie einen Abrechnungssatz für ein Projekt:

1. Wechseln Sie zu dem Projekt, für das Sie die Abrechnungssätze überschreiben möchten.
1. Klicken **im linken** auf „Abrechnungssätze“.

   Oder

   <span class="preview">Klicken Sie im linken **auf** Tarife“ und klicken Sie auf die Registerkarte **Abrechnung**, falls diese nicht bereits ausgewählt ist.</span>

1. Klicken Sie **Abrechnungssatz hinzufügen** > **Neuer Abrechnungssatz**.

   Oder

   <span class="preview">Klicken Sie **Abrechnungssatz hinzufügen > Abrechnungssatz für neues Aufgabengebiet hinzufügen**.</span>

   Das Feld „Neuer Abrechnungssatz“ wird geöffnet.

1. Wählen **im Feld** das Aufgabengebiet aus, für das Sie den Abrechnungssatz ändern möchten.

1. <span class="preview">(Optional) Wählen Sie Attribute für den Abrechnungssatz aus, z. B. Agentur oder Standort.</span>

   <span class="preview">Der Systemadministrator definiert Tarifattribute im Bereich „Setup“.</span>

1. Wählen Sie **Währung** für die Außerkraftsetzung des Abrechnungssatzes aus.
1. Geben Sie im Feld **Abrechnungssatz** die Überschreibung des Abrechnungssatzes ein und klicken Sie dann auf **Speichern**, um den Abrechnungssatz einmal zu überschreiben

   ODER

   Klicken Sie **Abrechnungssatz hinzufügen**, um weitere Abrechnungssatz-Überschreibungen hinzuzufügen.

1. (Bedingt) Geben Sie für Datumsüberschreibungen des effektiven Abrechnungssatzes die folgenden Informationen für jede Zeile ein:

   * **Abrechnungssatz**: Der Wert des Abrechnungssatzes vom Beginn des Projekts bis zum ersten Datum der ersten Überschreibung.
   * **Startdatum**: Das Datum, an dem die Überschreibung des Abrechnungssatzes beginnt.
   * **Enddatum**: Das Datum, an dem die Überschreibung des Abrechnungssatzes endet.

   ![Abrechnungssätze mit Überschreibungsdaten](assets/new-job-role-billing-rate-on-project2.png)

   Workfront wendet den Satz für Aufgabengebiete überschreiben auf die Stunden an, die während dieser Zeitrahmen bei der Berechnung des Umsatzes für das Projekt auftreten.

   Workfront ermöglicht es Ihnen, Lücken zwischen Überschreibungszeitrahmen zu hinterlassen, Sie erhalten jedoch eine Warnung, die bestätigt, dass dies beabsichtigt ist.

   Es ist nicht erforderlich, ein Startdatum für den ersten Überschreibungssatz oder ein Enddatum für den letzten Überschreibungssatz anzugeben.

   Wenn Sie nur eine einzige Abrechnungssatz-Überschreibung eingeben, gilt dieser Satz für die gesamte Dauer des Projekts. Wenn Sie mehrere datumswirksame Überschreibungen hinzufügen, geht Workfront davon aus, dass die erste Überschreibung für alle Stunden vor dem Enddatum und die letzte Überschreibung für alle Stunden nach dem Startdatum gilt.

   Workfront geht davon aus, dass die erste Überschreibungsrate auf alle Stunden angewendet wird, deren Datum älter als das Enddatum der ersten Überschreibungsrate ist, und dass die letzte Überschreibungsrate auf alle Stunden angewendet wird, deren Datum neuer als das Startdatum der letzten Überschreibung ist.

   Wenn eine Stunde vor dem geplanten Startdatum des Projekts protokolliert wird, wird der allererste Abrechnungssatz verwendet.

   Wird eine Stunde nach dem geplanten Abschlussdatum des Projekts protokolliert, wird der letzte Abrechnungssatz verwendet.

1. Klicken Sie auf **Speichern**.
