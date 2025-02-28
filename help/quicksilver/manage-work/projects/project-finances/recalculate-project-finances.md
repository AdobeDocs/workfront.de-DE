---
title: Projektfinanzen neu berechnen
product-area: projects
navigation-topic: financials
description: Die Finanzen werden für ein Projekt berechnet, da Änderungen in den für das Projekt protokollierten Stunden oder in den Sätzen auftreten, die zur Berechnung der Kosten und Einnahmen verwendet werden.
author: Lisa
feature: Work Management
exl-id: 5a90c5a1-8b26-4b6f-b9ec-f446a2e94ff0
source-git-commit: b983a780198743a2b87b4b48cf4d6afdf1cee437
workflow-type: tm+mt
source-wordcount: '1633'
ht-degree: 0%

---

# Projektfinanzen neu berechnen

Die Finanzen werden für ein Projekt berechnet, da Änderungen in den für das Projekt protokollierten Stunden oder in den Sätzen auftreten, die zur Berechnung der Kosten und Einnahmen verwendet werden.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan</td> 
   <td>Beliebig </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td>
   <p>Neu: Standard</p>
   <p>oder</p>
   <p>Aktuell: Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td>Zugriff auf Projekte und Finanzdaten bearbeiten</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td>Verwalten von Berechtigungen für das Projekt mit Berechtigungen zum Verwalten von Finanzen</td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Überlegungen zur Berechnung der Finanzen in Adobe Workfront

Die Finanzen werden in Enhanced Analytics wie folgt berechnet:

* Sie können Kosten und Einnahmen für ein Projekt manuell neu berechnen, indem Sie die Option Finanzen für ein Projekt neu berechnen verwenden.
* Darüber hinaus wird bei einigen Aktionen eine automatische Neuberechnung Trigger.

Wenn sich die Rate eines Benutzers oder einer Funktion während der Laufzeit eines Projekts ändert, kann Folgendes passieren:

* Wenn die Änderung vorgenommen wird, wird ab diesem Zeitpunkt der aktualisierte Satz verwendet, da Stunden protokolliert und die Finanzinformationen berechnet werden. Eine Änderung der Rate hat keinen Einfluss darauf, wie die Dinge berechnet wurden, bevor die Änderung vorgenommen wurde. Für alle protokollierten vorhandenen Stunden wird der alte Tarif zur Berechnung der Finanzinformationen verwendet.
* Sie können Adobe Workfront zwingen, den neuen Satz rückwirkend für alle bisher erfassten Stunden zu verwenden, indem Sie die Option „Finanzen neu berechnen“ verwenden. Dadurch ist Workfront gezwungen, alle zuvor eingegebenen Stunden, geplanten Kosten und Einnahmen rückwirkend entsprechend den neuen Tarifinformationen neu zu berechnen.

Der Berichtstyp „Projekt (Finanzdaten)“ führt nicht automatisch eine Neuberechnung Ihrer Finanzdaten durch. Um die Daten in diesem Berichtstyp zu aktualisieren, müssen Sie die Finanzen für einzelne Projekte manuell neu berechnen.

>[!CAUTION]
>
>Vor der manuellen Neuberechnung der Finanzen für ein bestimmtes Projekt sollten Sie alle Finanzdaten beibehalten, die bereits mit einem früheren Satz berechnet wurden. Es wird empfohlen, die Option Finanzen neu berechnen nur zu verwenden, wenn Sie sicher sind, dass Sie keine Änderungen an vorhandenen Informationen vornehmen, oder nur, wenn diese Änderungen gewünscht sind.

## Finanzdaten für Aufgaben mit vorhandenen Stunden beibehalten {#preserve-financial-data-for-tasks-with-existing-hours}

Wenn Finanzdaten für ein Projekt neu berechnet werden, berechnet Workfront rückwirkend alle zuvor protokollierten Stunden, geplanten Kosten, Istkosten sowie geplanten und tatsächlichen Einnahmen entsprechend neuen oder aktualisierten Finanzinformationen neu.

* [Projekteinnahmen erhalten](#preserve-project-revenue)
* [Projektkosten beibehalten](#preserve-project-cost)

### Projekteinnahmen beibehalten  {#preserve-project-revenue}

Die Umsatzraten können sich während der Laufzeit eines Projekts ändern.

Weitere Informationen zu Abrechnungssätzen und Umsatz finden Sie im Artikel [Übersicht über Abrechnung und Umsatz](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

Die Umsatzraten können sich auf den folgenden Ebenen ändern:

* Systemebene (für Aufgabengebiete)\
  Weitere Informationen zum Erstellen von Aufgabengebieten mit Abrechnungssätzen auf Systemebene finden Sie im Artikel [Erstellen und Verwalten von Aufgabengebieten](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

* Die Benutzerebene\
  Weitere Informationen zum Ändern der Abrechnungssatzinformationen für Benutzer finden Sie im Artikel [Bearbeiten des Benutzerprofils](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

* Auf Unternehmensebene (für Aufgabengebiete)\
  Weitere Informationen finden Sie unter [Überschreiben von Abrechnungssätzen für Aufgabengebiete auf Unternehmensebene](../../../administration-and-setup/set-up-workfront/organizational-setup/override-job-role-billing-rates-company-level.md).

* Die Projektebene (für Aufgabengebiete)\
  Weitere Informationen zum Überschreiben von Abrechnungssätzen für Aufgabengebiete auf Projektebene finden Sie im Artikel [Übersicht über das Überschreiben von Abrechnungssätzen für Aufgabengebiete und die Berechnung des Umsatzes für ein Projekt](../../../manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).

Beispielsweise ändert sich der Abrechnungssatz eines Benutzers während eines Projekts von 50 $ auf 75 $ pro Stunde, und Sie möchten, dass alle vorhandenen Daten mit dem alten Satz (50 $ und Stunde) berechnet werden. Wenn die Projektfinanzen jedoch neu berechnet werden, wird der Umsatz von Aufgaben, für die bereits Finanzdaten vorhanden sind, aktualisiert, um den neuen Abrechnungssatz (von 75 USD pro Stunde) widerzuspiegeln.

* [Beibehaltung des Projektumsatzes durch Erstellung eines Rechnungsnachweises](#preserve-project-revenue-by-creating-a-billing-record)
* [Projektumsatz durch Verwendung mehrerer Abrechnungssatz-Überschreibungen beibehalten](#preserve-project-revenue-by-using-multiple-billing-rate-overrides)

#### Beibehaltung des Projektumsatzes durch Erstellung eines Rechnungsnachweises {#preserve-project-revenue-by-creating-a-billing-record}

Wenn sich die Abrechnungssätze auf einer der oben genannten Ebenen ändern, können Sie bestehende Einnahmen, die bereits für das Projekt berechnet wurden, beibehalten, indem Sie vermeiden, die Option „Finanzen manuell neu berechnen“ zu verwenden, oder indem Sie die im Projekt aufgezeichnete Zeit, die mithilfe des alten Satzes berechnet wurde, in einen Abrechnungs-Datensatz mit dem Status „In Rechnung gestellt“ sperren.

Wenn Sie die Finanzierungsdaten für das Projekt nicht neu berechnen oder wenn Sie die Stunden, die in einem abgerechneten Abrechnungs-Datensatz erfasst sind, sperren, werden die Stunden, die nach den Tarifänderungen protokolliert werden, mit dem neuen Satz berechnet, und die Stunden, die protokolliert werden, bevor die Änderungen des Kostensatzes vorgenommen werden, bleiben mit dem alten Satz berechnet.

Weitere Informationen zum Erstellen von Rechnungsnachweisen finden Sie im Artikel [Erstellen von Rechnungsnachweisen](../../../manage-work/projects/project-finances/create-billing-records.md).

#### Projektumsatz durch Verwendung mehrerer Abrechnungssatz-Überschreibungen beibehalten {#preserve-project-revenue-by-using-multiple-billing-rate-overrides}

Wenn sich Abrechnungssätze für Aufgabengebiete auf Projektebene ändern, können Sie den vorhandenen Umsatz, der bereits für das Projekt berechnet wurde, beibehalten, indem Sie Überschreibungen mehrerer Abrechnungssätze verwenden, die innerhalb eines bestimmten Zeitraums gesperrt werden.

Weitere Informationen zur Verwendung mehrerer Abrechnungssatzüberschreibungen finden Sie im Artikel [Übersicht über das Überschreiben von Abrechnungssätzen für Aufgabengebiete und die Berechnung des Umsatzes für ein Projekt](../../../manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).

>[!NOTE]
>
>Dies gilt nur für Abrechnungssätze für Aufgabengebiete, die auf Projektebene geändert werden.

### Projektkosten beibehalten {#preserve-project-cost}

Die Kostensätze können sich auf folgenden Ebenen ändern:

* Systemebene (für Aufgabengebiete)\
  Weitere Informationen zum Erstellen von Aufgabengebieten mit Kostensätzen auf Systemebene finden Sie im Artikel [Erstellen und Verwalten von Aufgabengebieten](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

* Benutzerebene\
  Weitere Informationen zum Ändern der Kostensatzinformationen für Benutzer finden Sie im Artikel [Bearbeiten des Benutzerprofils](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

Wenn sich die Verrechnungssätze auf einer der oben genannten Ebenen ändern, können Sie bestehende Kosten, die bereits für das Projekt berechnet wurden, beibehalten, indem Sie die im Projekt aufgezeichnete Zeit, die mithilfe des alten Satzes berechnet wurde, in einen Verrechnungsdatensatz mit dem Status In Rechnung gestellt sperren. Weitere Informationen zum Erstellen von Rechnungsnachweisen finden Sie im Artikel [Erstellen von Rechnungsnachweisen](../../../manage-work/projects/project-finances/create-billing-records.md).

Sie können auch vermeiden, die Option „Finanzen manuell neu berechnen“ zu verwenden, wenn Sie keinen Rechnungsnachweis erstellen möchten, wie im Abschnitt [Finanzen für ein Projekt manuell neu berechnen](#manually-recalculate-finances-for-a-project) in diesem Artikel beschrieben.

Wenn Sie die Finanzierungsdaten für das Projekt nicht neu berechnen oder wenn Sie die Stunden, die in einem abgerechneten Abrechnungs-Datensatz erfasst sind, sperren, werden die Stunden, die nach den Tarifänderungen protokolliert werden, mit dem neuen Satz berechnet, und die Stunden, die protokolliert werden, bevor die Änderungen des Kostensatzes vorgenommen werden, bleiben mit dem alten Satz berechnet.

## Finanzen für ein Projekt manuell neu berechnen {#manually-recalculate-finances-for-a-project}

Wenn sich Ihre Sätze während der Laufzeit eines Projekts ändern und Ihre Kosten- und Umsatzberechnungen die neuen Sätze widerspiegeln sollen, müssen Sie die Finanzierungsdaten für das Projekt manuell neu berechnen.

>[!NOTE]
>
>Sie können verhindern, dass Umsatzwerte aktualisiert werden, um die neuen Sätze widerzuspiegeln, wenn Sie die Finanzen manuell neu berechnen. Befolgen Sie dazu die Schritte im Abschnitt [Beibehalten von Finanzdaten für Aufgaben mit vorhandenen Stunden](#preserve-financial-data-for-tasks-with-existing-hours) dieses Artikels. Kostenwerte werden immer aktualisiert, um die neuen Sätze widerzuspiegeln, wenn Sie die Finanzierungsdaten für ein Projekt manuell neu berechnen.

Sie können die Finanzen von Projekten in Workfront auf der Projektseite oder in einer Projektliste oder einem Bericht neu berechnen.

Sie können die Finanzen neu berechnen, während Sie sie stapelweise bearbeiten. Weitere Informationen finden Sie im Abschnitt [Manuelles Neuberechnen der Finanzen in ](#manually-recalculate-finances-in-bulk)) in diesem Artikel.

1. Wechseln Sie zu dem Projekt, für das Sie die Finanzen neu berechnen möchten, und klicken Sie auf das **Mehr**-Symbol ![Mehr ](assets/qs-more-icon-on-an-object.png) rechts neben dem Projektnamen.

   ![Dropdown „Mehr“ auf Projektebene](assets/project-level-more-drop-down-expanded-nwe-350x516.png)

   Oder

   Gehen Sie zu einer Projektliste oder einem Bericht, wählen Sie ein oder mehrere Projekte aus und klicken Sie dann oben in der Liste auf das **Mehr**-Symbol ![](assets/qs-more-icon-on-an-object.png)Mehr Menü).

   ![Ausdrücke neu ](assets/recalculate-expressions-timeline-finances-drop-down-in-project-list-nwe.png)

   >[!TIP]
   >
   >Je nach Komplexität Ihrer Projekte empfehlen wir, bei der Massenberechnung ihrer Finanzen keine große Anzahl von Projekten auszuwählen, um eine optimale Leistung zu gewährleisten. Ein Projekt zu komplex kann beispielsweise durch mehrere Abhängigkeiten oder Zuweisungen oder eine große Anzahl benutzerdefinierter Felder werden.

1. Klicken Sie auf **Finanzen neu**.

   Alle geplanten Kosten und Einnahmen für das Projekt werden mit neuen Informationen neu berechnet.

   Sie sollten oben im Browser eine Bestätigung erhalten, dass die Finanzen des Projekts erfolgreich neu berechnet wurden.
Bestehende Kostenwerte und einige Umsatzwerte, die nicht gesperrt wurden, werden aktualisiert, um die neuen Sätze widerzuspiegeln.

## Finanzen stapelweise manuell neu berechnen{#manually-recalculate-finances-in-bulk}

Sie können die Finanzen mehrerer Projekte manuell neu berechnen, indem Sie sie stapelweise bearbeiten. Dadurch werden die Einnahmen aus den Projekten rückwirkend neu berechnet.

>[!IMPORTANT]
>
>Sie können verhindern, dass Umsatzwerte aktualisiert werden, um die neuen Sätze widerzuspiegeln, wenn Sie die Finanzen manuell neu berechnen. Befolgen Sie dazu die Schritte im Abschnitt [Beibehalten von Finanzdaten für Aufgaben mit vorhandenen Stunden](#preserve-financial-data-for-tasks-with-existing-hours) dieses Artikels. Kostenwerte werden immer aktualisiert, um die neuen Sätze widerzuspiegeln, wenn Sie die Finanzierungsdaten für Projekte manuell neu berechnen.

So berechnen Sie die Finanzen mehrerer Projekte manuell neu:

1. Zu einer Projektliste gehen.
1. Wählen Sie mehrere Projekte in der Liste aus und klicken Sie dann oben in der Liste auf **Mehr**-Symbol ![](assets/qs-more-icon-on-an-object.png)Mehr Menü).

   ![Ausdrücke neu ](assets/recalculate-expressions-timeline-finances-drop-down-in-project-list-nwe.png)

   >[!TIP]
   >
   >Je nach Komplexität Ihrer Projekte wird empfohlen, bei der Massenbearbeitung keine große Anzahl von Projekten auszuwählen, um eine optimale Leistung zu gewährleisten. Ein Projekt zu komplex kann beispielsweise durch mehrere Abhängigkeiten oder Zuweisungen oder eine große Anzahl benutzerdefinierter Felder werden.

1. Klicken Sie auf **Finanzen neu**.

   Alle geplanten Kosten und Einnahmen für die ausgewählten Projekte werden mit neuen Informationen neu berechnet.

   Sie sollten oben im Browser eine Bestätigung erhalten, dass die Finanzen der Projekte erfolgreich neu berechnet wurden.

## Maßnahmen, die eine automatische Neuberechnung der Finanzen in Trigger bringen

Die finanzielle Neuberechnung von Projekten in Workfront wird durch folgende Maßnahmen Trigger:

* Aufgabenstatus ändern
* Verschieben einer Aufgabe mit Stunden in ein anderes Projekt
* Ändern des Projektstatus von „Abgeschlossen“ in einen aktiven Status

>[!NOTE]
>
>Wenn Sie den Projektstatus ändern, werden nur die geplanten Werte neu berechnet.

Sie können die Finanzen auch manuell unter dem Menü **Mehr** ![Mehr](assets/qs-more-menu.png) auf Projektebene neu berechnen, indem Sie auf **Finanzen neu berechnen** klicken.
