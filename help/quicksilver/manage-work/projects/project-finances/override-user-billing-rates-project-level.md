---
content-type: overview
product-area: projects
navigation-topic: financials
title: Benutzer-Abrechnungssätze auf Projektebene überschreiben
description: In diesem Artikel wird beschrieben, wie Sie die Abrechnungssätze der Systembenutzenden für ein Projekt überschreiben können.
author: Lisa
feature: Work Management
exl-id: eb7dbb6f-a31c-4569-be54-9a151dcf4135
source-git-commit: 39630b50384d710dadb1f48342113b74338a9104
workflow-type: tm+mt
source-wordcount: '744'
ht-degree: 4%

---

# Benutzer-Abrechnungssätze auf Projektebene überschreiben

Als Projekt-Manager können Sie den Abrechnungssatz für einen Benutzer für ein bestimmtes Projekt festlegen. Dieser Abrechnungssatz auf Projektebene überschreibt den Abrechnungssatz auf Systemebene für diesen Benutzer. Workfront verwendet zur Berechnung des Umsatzes den Abrechnungssatz auf Projektebene des Benutzers, anstatt den Abrechnungssatz auf Systemebene zu verwenden.

In diesem Artikel wird beschrieben, wie Sie die Abrechnungssätze der Systembenutzenden für ein Projekt überschreiben können.

Allgemeine Informationen zum Überschreiben von Abrechnungssätzen für Projekte und zur Berechnung des Projektumsatzes finden Sie [Übersicht über das Überschreiben von Abrechnungssätzen und die Berechnung des Umsatzes für ein Projekt](/help/quicksilver/manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).

Weitere Informationen zur Berechnung des Umsatzes für das Projekt finden Sie [ Abschnitt „Übersicht über die Umsatz- und ](/help/quicksilver/manage-work/projects/project-finances/overview-revenue-cost-hierarchy.md)&quot; und [Umsatzberechnungen für Aufgaben basierend auf Benutzer- und ](/help/quicksilver/manage-work/projects/project-finances/billing-and-revenue-overview.md#revenue-calculations-for-tasks-based-on-user-and-role-assignments)&quot; im Artikel [Übersicht über Abrechnung und Umsatz](/help/quicksilver/manage-work/projects/project-finances/billing-and-revenue-overview.md).

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
   <td>Workflow Ultimate</td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront-Lizenz</td> 
   <td>Standard</td> 
  </tr> 
  <tr> 
   <td>Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriff auf Projekte und Finanzdaten bearbeiten</p>
       <p><p>Sie müssen außerdem über eine der folgenden verfügen:</p> 
        <ul> 
          <li> <p>Die Zugriffsebene des Systemadministrators. </li> 
          <li> <p><b>Benutzer</b> Einstellung in Ihrer Zugriffsebene konfiguriert auf <b>Bearbeiten</b> Zugriff, mit <b>Erstellen</b> und mindestens einer der beiden <b>Benutzeradmin</b> Optionen unter <b>Optimieren Sie Ihre Einstellungen</b> <img src="assets/gear-icon-in-access-levels.png">. </p> <p>Wenn diese beiden Optionen <b>Benutzeradministrator (Gruppenbenutzer)) aktiviert </b>, müssen Sie Gruppenadministrator einer Gruppe sein, in der der Benutzer Mitglied ist.</p> </li> 
    </ul></td> 
  </tr> 
  <tr> 
   <td>Objektberechtigungen</td> 
   <td>Verwalten Sie Berechtigungen für das Projekt, das die Option Finanzdaten bearbeiten enthält. </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) in der Dokumentation zu Workfront.

+++

## Benutzer-Abrechnungssätze auf Projektebene überschreiben

Wenn Sie den Abrechnungssatz eines Benutzers für ein Projekt überschreiben, können Sie ein Gültigkeitsdatum zuweisen und jeder Datumsbereich hat einen anderen Satz. Wenn Sie keine Gültigkeitsdaten zuordnen, wird die von Ihnen eingegebene Abrechnungssatzüberschreibungen für die gesamte Projektdauer zur Berechnung des Umsatzes verwendet.

So überschreiben Sie einen Benutzer-Abrechnungssatz für ein Projekt:

1. Wechseln Sie zu dem Projekt, für das Sie die Abrechnungssätze überschreiben möchten.
1. Klicken Sie **linken** auf „Tarife“. Möglicherweise müssen Sie zunächst auf &quot;**anzeigen“**.
1. Klicken Sie auf **Registerkarte** Abrechnung“, falls diese Option noch nicht ausgewählt ist.
1. Klicken Sie **Abrechnungssatz hinzufügen** > **Abrechnungssatz für neue Benutzer**.

   Das Feld „Neuer Benutzer-Abrechnungssatz“ wird geöffnet.

1. Wählen **im Feld** den Benutzer aus, für den Sie den Abrechnungssatz ändern möchten.
1. Wählen Sie **Währung** für die Außerkraftsetzung des Abrechnungssatzes aus.
1. Geben Sie **Feld „Abrechnungssatz** die erste Überschreibung des Abrechnungssatzes ein.
1. (Optional) Klicken Sie auf **Datum des Wirksamwerdens hinzufügen**, um weitere Abrechnungssatz-Überschreibungen hinzuzufügen.
1. (Bedingt) Wenn Sie mehrere Abrechnungssatz-Überschreibungen hinzufügen, geben Sie die folgenden Informationen für jede Zeile an:

   * **Abrechnungssatz**: Der Wert des Abrechnungssatzes während des angegebenen Zeitraums.
   * **Startdatum**: Das Datum, an dem die Überschreibung des Abrechnungssatzes beginnt.
   * **Enddatum**: Das Datum, an dem die Überschreibung des Abrechnungssatzes endet.

   ![Feld „Neuer Benutzer-Abrechnungssatz“ mit Gültigkeitsdaten](assets/new-user-billing-rate-on-project2.png)

   Workfront wendet die Benutzerüberschreibungsrate bei der Berechnung des Umsatzes für das Projekt auf die Stunden an, die während dieser Zeitrahmen auftreten.

   Workfront ermöglicht es Ihnen, Lücken zwischen Überschreibungszeitrahmen zu hinterlassen, Sie erhalten jedoch eine Warnung, die bestätigt, dass dies beabsichtigt ist.

   Es ist nicht erforderlich, ein Startdatum für den ersten Überschreibungssatz oder ein Enddatum für den letzten Überschreibungssatz anzugeben.

   Wenn Sie nur eine einzige Abrechnungssatz-Überschreibung eingeben, gilt dieser Satz für die gesamte Dauer des Projekts. Wenn Sie mehrere datumswirksame Überschreibungen hinzufügen, geht Workfront davon aus, dass die erste Überschreibung für alle Stunden vor dem Enddatum und die letzte Überschreibung für alle Stunden nach dem Startdatum gilt.

   Workfront geht davon aus, dass die erste Überschreibungsrate auf alle Stunden angewendet wird, deren Datum älter als das Enddatum der ersten Überschreibungsrate ist, und dass die letzte Überschreibungsrate auf alle Stunden angewendet wird, deren Datum neuer als das Startdatum der letzten Überschreibung ist.

   Wenn eine Stunde vor dem geplanten Startdatum des Projekts protokolliert wird, wird der allererste Abrechnungssatz verwendet.

   Wird eine Stunde nach dem geplanten Abschlussdatum des Projekts protokolliert, wird der letzte Abrechnungssatz verwendet.

1. Klicken Sie auf **Speichern**.
