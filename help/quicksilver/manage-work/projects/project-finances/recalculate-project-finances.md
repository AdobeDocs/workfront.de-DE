---
title: Neuberechnung der Projektfinanzen
product-area: projects
navigation-topic: financials
description: Die Finanzmittel werden für ein Projekt berechnet, da Änderungen in den für das Projekt angemeldeten Stunden oder in den zur Berechnung der Kosten und Einnahmen verwendeten Raten auftreten.
author: Lisa
feature: Work Management
exl-id: 5a90c5a1-8b26-4b6f-b9ec-f446a2e94ff0
source-git-commit: 69afad9af3f1e703487fdab092bc84457ee00922
workflow-type: tm+mt
source-wordcount: '1678'
ht-degree: 0%

---

# Neuberechnung der Projektfinanzen

Die Finanzmittel werden für ein Projekt berechnet, da Änderungen in den für das Projekt angemeldeten Stunden oder in den zur Berechnung der Kosten und Einnahmen verwendeten Raten auftreten.

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf Projekte und Finanzdaten bearbeiten</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Verwalten von Berechtigungen für das Projekt mit Berechtigungen zum Verwalten der Finanzen</p> <p>Weitere Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Anfordern des Zugriffs auf Objekte </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Überlegungen zur Finanzberechnung in Adobe Workfront

Die Berechnung der Beträge erfolgt in der erweiterten Analyse wie folgt:

* Sie können Kosten und Einnahmen eines Projekts manuell neu berechnen, indem Sie für ein Projekt die Option Finanzen neu berechnen verwenden.
* Darüber hinaus wird bei einigen Aktionen eine automatische Neuberechnung Trigger.

Wenn sich die Rate eines Benutzers oder einer Rolle während der Lebensdauer eines Projekts ändert, kann Folgendes auftreten:

* Wenn die Änderung vorgenommen wird, wird die aktualisierte Rate ab diesem Zeitpunkt verwendet, da Stunden protokolliert und die Finanzinformationen berechnet werden. Eine Änderung der Rate hat keinen Einfluss darauf, wie die Dinge vor der Änderung berechnet wurden. Für alle vorhandenen Stunden wird der alte Satz zur Berechnung der Finanzinformationen verwendet.
* Mit der Option Finanzen neu berechnen können Sie Adobe Workfront zwingen, die neue Rate rückwirkend für alle bisher angemeldeten Stunden zu verwenden. Dies zwingt Workfront dazu, alle zuvor eingegebenen Stunden, geplanten Kosten und Einnahmen entsprechend den neuen Ratsinformationen rückwirkend neu zu berechnen.

Der Berichtstyp Projekt (Finanzdaten) wird vor dem Laden der Daten nicht automatisch neu berechnet. Um die Daten dieses Berichtstyps zu aktualisieren, müssen Sie die Finanzen für einzelne Projekte manuell neu berechnen.

>[!CAUTION]
>
>Vor der manuellen Neuberechnung der Finanzen für ein bestimmtes Projekt möchten Sie möglicherweise alle Finanzdaten beibehalten, die bereits zu einem früheren Zeitpunkt berechnet wurden. Es wird empfohlen, die Option &quot;Finanzen neu berechnen&quot;nur zu verwenden, wenn Sie sicher sind, dass Sie keine Änderungen an vorhandenen Informationen vornehmen, oder nur, wenn solche Änderungen gewünscht werden.
>
>Beachten Sie, dass beim Ausführen eines Berichts über ein Projekt (Finanzdaten) Ihre Finanzdaten neu berechnet werden. Daher sollten Sie dieselben Überlegungen anstellen, bevor Sie den Bericht ausführen.

## Finanzielle Daten für Aufgaben mit vorhandenen Stunden beibehalten {#preserve-financial-data-for-tasks-with-existing-hours}

Wenn die Finanzdaten für ein Projekt neu berechnet werden, berechnet Workfront alle zuvor protokollierten Stunden, geplanten, tatsächlichen Kosten sowie geplanten und tatsächlichen Einnahmen gemäß neuen oder aktualisierten Finanzinformationen rückwirkend neu.

* [Projektumsatz beibehalten](#preserve-project-revenue)
* [Projektkosten beibehalten](#preserve-project-cost)

### Projektumsatz beibehalten  {#preserve-project-revenue}

Die Umsatzraten können sich während der Lebensdauer eines Projekts ändern.

Weitere Informationen zu Abrechnungsraten und Umsätzen finden Sie im Artikel [Übersicht über Abrechnung und Umsatz](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

Die Umsatzraten können sich auf folgenden Ebenen ändern:

* Die Systemebene (für Aufgabenrollen)\
  Weitere Informationen zum Erstellen von Auftrags-Rollen mit Abrechnungsraten auf Systemebene finden Sie im Artikel [Erstellen und Verwalten von Auftragsrollen](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

* Benutzerebene\
  Weitere Informationen zum Ändern der Rechnungsrateninformationen für Benutzer finden Sie im Artikel [Profil eines Benutzers bearbeiten](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md) .

* Auf Unternehmensebene (für Jobrollen)\
  Weitere Informationen finden Sie unter [Außerkraftsetzen der Abrechnungsraten für Auftragsrollen auf Unternehmensebene](../../../administration-and-setup/set-up-workfront/organizational-setup/override-job-role-billing-rates-company-level.md).

* Die Projektebene (für Auftragsrollen)\
  Weitere Informationen zum Außerkraftsetzen von Einstellungen für Auftragsrollen auf Projektebene finden Sie im Artikel [Überblick über das Überschreiben der Abrechnungsraten für Auftragsrollen und Berechnung des Umsatzes für ein Projekt](../../../manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).

Beispielsweise ändert sich der Abrechnungskurs eines Benutzers im Laufe eines Projekts von 50 auf 75 USD pro Stunde und Sie möchten, dass alle vorhandenen Daten zum alten Preis (50 USD pro Stunde) berechnet bleiben. Bei der Neuberechnung der Projektfinanzierungen werden die Einnahmen jedoch für Aufgaben, die bereits über vorhandene Finanzdaten verfügen, aktualisiert, um die neue Abrechnungsrate (75 USD pro Stunde) widerzuspiegeln.

* [Bewahren Sie den Projektumsatz durch Erstellen eines Abrechnungsdatensatzes auf](#preserve-project-revenue-by-creating-a-billing-record)
* [Beibehalten des Projektumsatzes durch Verwendung mehrerer Außerkraftsetzungen der Abrechnungsrate](#preserve-project-revenue-by-using-multiple-billing-rate-overrides)

#### Beibehalten des Projektumsatzes durch Erstellen eines Abrechnungsdatensatzes {#preserve-project-revenue-by-creating-a-billing-record}

Wenn sich die Abrechnungssätze auf einer der oben genannten Ebenen ändern, können Sie den bereits für das Projekt berechneten Umsatz beibehalten, indem Sie die manuelle Option Finanzen neu berechnen vermeiden oder die im Projekt aufgezeichnete und anhand des alten Satzes berechnete Zeit in einen Abrechnungsdatensatz mit dem Status Abgerechnet sperren.

Wenn Sie die Projektfinanzierungen nicht neu berechnen oder die Stunden, die in einem abrechnungsfähigen Datensatz angemeldet sind, sperren, werden die Stunden, die nach den Ratenänderungen protokolliert werden, mit dem neuen Satz berechnet und die Stunden, die vor den Kostenratenänderungen protokolliert wurden, bleiben mit dem alten Satz berechnet.

Weitere Informationen zum Erstellen von Rechnungsdatensätzen finden Sie im Artikel [Erstellen von Rechnungsdatensätzen](../../../manage-work/projects/project-finances/create-billing-records.md).

#### Beibehalten des Projektumsatzes durch Verwendung mehrerer Außerkraftsetzungen der Abrechnungsrate {#preserve-project-revenue-by-using-multiple-billing-rate-overrides}

Wenn sich die Abrechnungsraten für Stellenangebote auf Projektebene ändern, können Sie vorhandenen Umsatz, der bereits für das Projekt berechnet wurde, beibehalten, indem Sie mehrere Überschreibungen für Abrechnungsraten verwenden, die innerhalb eines bestimmten Zeitraums gesperrt sind.

Weitere Informationen zur Verwendung mehrerer Außerkraftsetzungen von Abrechnungsraten finden Sie im Artikel [Überblick über die Außerkraftsetzung von Abrechnungsraten für Auftragsrollen und Berechnung des Umsatzes für ein Projekt](../../../manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).

>[!NOTE]
>
>Dies gilt nur für die Abrechnungssätze für die Rolle von Arbeitsplätzen, die auf Projektebene geändert werden.

### Projektkosten beibehalten {#preserve-project-cost}

Die Kostensätze können sich auf folgenden Ebenen ändern:

* Systemebene (für Aufgabenrollen)\
  Weitere Informationen zum Erstellen von Auftrags-Rollen mit Kostensätzen auf Systemebene finden Sie im Artikel [Erstellen und Verwalten von Auftragsrollen](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

* Benutzerebene\
  Weitere Informationen zum Ändern der Informationen zu den Kostensätzen für Benutzer finden Sie im Artikel [Profil eines Benutzers bearbeiten](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md) .

Wenn sich die Abrechnungssätze auf einer der oben genannten Ebenen ändern, können Sie die bereits für das Projekt berechneten vorhandenen Kosten beibehalten, indem Sie die im Projekt aufgezeichnete und unter Verwendung des alten Abrechnungssatzes berechnete Zeit in einen Abrechnungsdatensatz mit dem Status Abgerechnet sperren. Weitere Informationen zum Erstellen von Rechnungsdatensätzen finden Sie im Artikel [Erstellen von Rechnungsdatensätzen](../../../manage-work/projects/project-finances/create-billing-records.md).

Sie können auch die manuelle Option Finanzen neu berechnen vermeiden, wenn Sie keinen Rechnungsdatensatz erstellen möchten, wie im Abschnitt [Manuelles Neuberechnen der Finanzen für ein Projekt](#manually-recalculate-finances-for-a-project) in diesem Artikel beschrieben.

Wenn Sie die Projektfinanzierungen nicht neu berechnen oder die Stunden, die in einem abrechnungsfähigen Datensatz angemeldet sind, sperren, werden die Stunden, die nach den Ratenänderungen protokolliert werden, mit dem neuen Satz berechnet und die Stunden, die vor den Kostenratenänderungen protokolliert wurden, bleiben mit dem alten Satz berechnet.

## Manuelles Neuberechnen der Finanzen für ein Projekt {#manually-recalculate-finances-for-a-project}

Wenn sich Ihre Beträge während der Laufzeit eines Projekts ändern und Sie möchten, dass Ihre Kosten- und Umsatzberechnungen den neuen Zinssätzen entsprechen, müssen Sie die Projektfinanzierungen manuell neu berechnen.

>[!NOTE]
>
>Sie können verhindern, dass die Umsatzwerte aktualisiert werden, um die neuen Zinssätze widerzuspiegeln, wenn Sie das Finanzwesen manuell neu berechnen, indem Sie die Schritte im Abschnitt [Finanzdaten für Aufgaben mit vorhandenen Stunden beibehalten](#preserve-financial-data-for-tasks-with-existing-hours) dieses Artikels befolgen. Die Kostenwerte werden immer aktualisiert, um die neuen Zinssätze widerzuspiegeln, wenn Sie die Finanzen eines Projekts manuell neu berechnen.

Sie können die Projektfinanzierung in Workfront von der Projektseite aus oder über eine Projektliste oder einen Bericht neu berechnen.

Sie können die Finanzen neu berechnen, während Sie sie stapelweise bearbeiten. Weitere Informationen finden Sie im Abschnitt [Manuelles Neuberechnen von Finanzierungen als Stapel](#manually-recalculate-finances-in-bulk) in diesem Artikel.

1. Wechseln Sie zu dem Projekt, in dem Sie die Finanzen neu berechnen möchten, und klicken Sie auf das Symbol **Mehr** ![](assets/qs-more-icon-on-an-object.png) rechts neben dem Projektnamen.

   ![](assets/project-level-more-drop-down-expanded-nwe-350x516.png)

   Oder

   Wechseln Sie zu einer Projektliste oder einem Bericht und wählen Sie ein oder mehrere Projekte aus. Klicken Sie dann oben in der Liste auf das Symbol **Mehr** ![](assets/qs-more-icon-on-an-object.png) .

   ![](assets/recalculate-expressions-timeline-finances-drop-down-in-project-list-nwe.png)

   >[!TIP]
   >
   >Je nach der Komplexität Ihrer Projekte empfehlen wir, bei der Neuberechnung ihrer Finanzen keine große Anzahl von Projekten auszuwählen, um eine optimale Leistung zu gewährleisten. Einige Dinge, die ein Projekt zu komplex machen könnten, sind möglicherweise mehrere Abhängigkeiten oder Zuweisungen oder eine große Anzahl benutzerdefinierter Felder.

1. Klicken Sie auf **Finanzen neu berechnen**.

   Alle geplanten Kosten und Einnahmen des Projekts werden mit neuen Informationen berechnet.

   Sie sollten oben im Browser eine Bestätigung erhalten, dass die Finanzen des Projekts erfolgreich neu berechnet wurden.
Bestehende Kostenwerte und einige Umsatzwerte, die nicht gesperrt wurden, werden entsprechend den neuen Raten aktualisiert.

## Manuelle Neuberechnung von Gesamtfinanzierungen{#manually-recalculate-finances-in-bulk}

Sie können die Finanzen mehrerer Projekte manuell neu berechnen, indem Sie sie stapelweise bearbeiten. Dadurch werden die Einnahmen aus den Projekten rückwirkend neu berechnet.

>[!IMPORTANT]
>
>Sie können verhindern, dass die Umsatzwerte aktualisiert werden, um die neuen Zinssätze widerzuspiegeln, wenn Sie das Finanzwesen manuell neu berechnen, indem Sie die Schritte im Abschnitt [Finanzdaten für Aufgaben mit vorhandenen Stunden beibehalten](#preserve-financial-data-for-tasks-with-existing-hours) dieses Artikels befolgen. Die Kostenwerte werden immer aktualisiert, um die neuen Zinssätze widerzuspiegeln, wenn Sie die Projektfinanzierung manuell neu berechnen.

So berechnen Sie die Finanzen mehrerer Projekte manuell neu:

1. Gehen Sie zu einer Projektliste.
1. Wählen Sie mehrere Projekte in der Liste aus und klicken Sie dann oben in der Liste auf das Symbol **Mehr** ![](assets/qs-more-icon-on-an-object.png) .

   ![](assets/recalculate-expressions-timeline-finances-drop-down-in-project-list-nwe.png)

   >[!TIP]
   >
   >Je nach Komplexität Ihrer Projekte empfehlen wir, bei der Massenbearbeitung keine große Anzahl von Projekten auszuwählen, um eine optimale Leistung zu gewährleisten. Einige Dinge, die ein Projekt zu komplex machen könnten, sind möglicherweise mehrere Abhängigkeiten oder Zuweisungen oder eine große Anzahl benutzerdefinierter Felder.

1. Klicken Sie auf **Finanzen neu berechnen**.

   Alle für die ausgewählten Projekte geplanten Kosten und Einnahmen werden mit neuen Informationen neu berechnet.

   Sie sollten oben im Browser eine Bestätigung erhalten, dass die Finanzierung der Projekte erfolgreich neu berechnet wurde.

## Maßnahmen, die eine automatische Neuberechnung der Finanzen Trigger haben

Die folgenden Maßnahmen Trigger die finanzielle Neuberechnung von Projekten in Workfront:

* Aufgabenstatus ändern
* Verschieben einer Aufgabe mit Stunden in ein anderes Projekt
* Ändern des Projektstatus von Fertig stellen in einen aktiven Status

>[!NOTE]
>
>Wenn Sie den Projektstatus ändern, werden nur die geplanten Werte neu berechnet.

Sie können die Finanzen auch manuell im Menü **Mehr** ![](assets/qs-more-menu.png) auf Projektebene neu berechnen, indem Sie auf **Finanzen neu berechnen** klicken.
