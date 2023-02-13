---
product-area: projects
navigation-topic: financials
title: Außerkraftsetzen der Abrechnungsraten für Auftragsrollen auf Projektebene
description: Als Projektmanager können Sie festlegen, welcher Abrechnungskurs für eine Auftragsrolle in einem bestimmten Projekt gilt. Diese Abrechnungsrate auf Projektebene überschreibt die Abrechnungsrate auf Systemebene für diese Arbeitsplatzrolle. Workfront verwendet zur Berechnung des Umsatzes die Abrechnungsrate auf Projektebene der Auftragsrolle, anstatt die Abrechnungsrate auf Systemebene zu verwenden.
author: Alina
feature: Work Management
exl-id: b7a33459-6929-4611-8546-06ca979e5dbe
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '858'
ht-degree: 0%

---

# Außerkraftsetzen der Abrechnungsraten für Auftragsrollen auf Projektebene

Als Projektmanager können Sie festlegen, welcher Abrechnungskurs für eine Auftragsrolle in einem bestimmten Projekt gilt. Diese Abrechnungsrate auf Projektebene überschreibt die Abrechnungsrate auf Systemebene für diese Arbeitsplatzrolle. Workfront verwendet zur Berechnung des Umsatzes die Abrechnungsrate auf Projektebene der Auftragsrolle, anstatt die Abrechnungsrate auf Systemebene zu verwenden.

In diesem Artikel wird beschrieben, wie Sie die Abrechnungsraten für Systemaufträge für ein Projekt überschreiben können.

Allgemeine Informationen über das Außerkraftsetzen von Gebühren für die Abrechnung von Aufgaben für Projekte und die Berechnung der Projekterlöse finden Sie unter [Übersicht über die Außerkraftsetzung der Abrechnungsraten von Auftragsrollen und die Berechnung des Umsatzes eines Projekts](../../../manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).

Weitere Informationen dazu, welche Auftragsrolle zur Berechnung des Umsatzes für das Projekt verwendet wird, finden Sie im Abschnitt &quot;Verstehen der Umsatzberechnungen für Aufgaben basierend auf Benutzer- und Rollenzuweisungen&quot;im Artikel [Übersicht über Rechnungsstellung und Umsatz](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

>[!NOTE]
>
>Im Falle des tatsächlichen Umsatzes sollten die Abrechnungsraten, die auf Stunden angewendet werden, die zu einem Abrechnungsdatensatz hinzugefügt werden, der als Abrechnung gekennzeichnet ist, nicht durch Überschreibungen des Abrechnungskurses beeinträchtigt werden, die nach Abrechnung des Abrechnungsdatensatzes auftreten.

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf Projekte und Finanzdaten bearbeiten</p> <p>Administratorzugriff für Job-Rollen</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Berechtigungen für das Projekt verwalten, das die Bearbeitung von Finanzdaten enthält </p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Außerkraftsetzen der Abrechnungsraten für Auftragsrollen auf Projektebene

Sie können die Abrechnungsrate einer Auftragsrolle in einem Projekt wie folgt überschreiben:

* Einmalig durch Auswahl einer neuen Rate für die Auftragsrolle.\
   Der neue Satz wird für die gesamte Dauer des Projekts verwendet, um den Umsatz zu berechnen.

* Mehrmals durch Auswahl mehrerer neuer Raten für bestimmte Datumsbereiche.\
   Für jeden angegebenen Datumsbereich kann eine andere Rate verwendet werden.

>[!TIP]
>
>Sie können die Abrechnungsraten von Benutzern für ein Projekt nicht überschreiben.

So überschreiben Sie die Abrechnungsrate für ein Projekt:

1. Wechseln Sie zu dem Projekt, für das Sie die Abrechnungssätze außer Kraft setzen möchten.
1. Klicken **Abrechnungssätze** im linken Bereich. Möglicherweise müssen Sie zuerst klicken **Mehr anzeigen**.
1. Klicken **Abrechnungsrate hinzufügen** > **Neuer Abrechnungskurs**.

   Das Feld &quot;Neue Abrechnungsrate&quot;wird geöffnet.

1. Im **Auftragsrolle** -Feld die Auftragsrolle auswählen, für die Sie den Abrechnungskurs ändern möchten.

   ![](assets/override-billing-rate-on-project-nwe-350x310.png)

   Die **Standardabrechnungsrate** zeigt die Rate auf Systemebene für diese Auftragsrolle an.

1. Im **Abrechnungssätze 1** ein, geben Sie die einmalige Außerkraftsetzung der Abrechnungsrate ein und klicken Sie auf **Speichern** einmalig den Abrechnungskurs außer Kraft setzen

   Oder

   Klicken **Rate hinzufügen** , um weitere Außerkraftsetzungen der Abrechnungsrate hinzuzufügen.

1. (Bedingt) Wenn Sie mehr als eine Überschreibung der Abrechnungsrate hinzufügen, geben Sie die folgenden Informationen an:

   * **Abrechnungssätze 1**: den Wert des Abrechnungskurses vom Projektbeginn bis zum ersten Datum der ersten Außerkraftsetzung. Dies entspricht normalerweise dem Betrag der **Standardrate**.
   * **Startdatum**: Dies ist das Datum, an dem die Standardrate endet.
   * **Enddatum**: das Datum, an dem die neue Abrechnungsrate außer Kraft gesetzt wird.

   ![new_billing_rate_with_Adjustment_dates.png](assets/new-billing-rate-with-adjustment-dates-350x266.png)

1. Die Zeitzone für die ausgewählten Daten wird unten im Feld &quot;Neue Abrechnungsrate&quot;angezeigt. Dies ist die Zeitzone, die mit Ihrer Workfront-Instanz verknüpft ist, wie im Bereich &quot;Kundeninformationen&quot;unter &quot;Einrichtung&quot;angezeigt. Weitere Informationen finden Sie unter [Grundlegende Informationen für Ihr System konfigurieren](../../../administration-and-setup/get-started-wf-administration/configure-basic-info.md).
1. Workfront wendet die Rollenrate für Aufträge überschreiben auf die Stunden an, die während der bei der Berechnung des Projektumsatzes festgelegten Zeiträume auftreten.
1. Zwischen den Zeitrahmen zweier Überschreibungsraten sollten keine Lücken bestehen. Die **Startdatum** einer Überschreibungsrate sollte der Tag sein, der auf den folgenden Tag folgt **Enddatum** des vorherigen Überschreibungsdatums.

1. Sie können weder ein Startdatum für die erste Überschreibungsrate noch ein Enddatum für die letzte Überschreibungsrate angeben.\
   Es wird empfohlen, die Standardrate für die erste Überschreibungsrate zu verwenden.\
   Workfront geht davon aus, dass die erste Überschreibungsrate für alle Stunden angewendet wird, deren Datum älter als das Enddatum der ersten Außerkraftsetzung ist, und dass die letzte Überschreibungsrate für alle Stunden mit einem Datum angewendet wird, das neuer als das Anfangsdatum der letzten Überschreibung ist.\
   Wenn eine Stunde vor dem geplanten Startdatum des Projekts protokolliert wird, wird die allererste Abrechnungsrate verwendet.\
   Wenn eine Stunde nach dem geplanten Abschlussdatum des Projekts protokolliert wird, wird die letzte Abrechnungsrate verwendet.

1. Klicken Sie auf **Speichern**.
