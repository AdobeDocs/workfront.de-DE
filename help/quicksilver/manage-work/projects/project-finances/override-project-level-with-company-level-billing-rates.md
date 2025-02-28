---
product-area: projects
navigation-topic: financials
title: Abrechnungssätze auf Projektebene mit Abrechnungssätzen auf Firmenebene überschreiben
description: Abrechnungssätze auf Projektebene mit Abrechnungssätzen auf Firmenebene überschreiben
author: Lisa
feature: Work Management
exl-id: 02ea4c7c-0473-4cc4-913c-3baa613767b7
source-git-commit: b983a780198743a2b87b4b48cf4d6afdf1cee437
workflow-type: tm+mt
source-wordcount: '476'
ht-degree: 1%

---

# Abrechnungssätze auf Projektebene mit Abrechnungssätzen auf Firmenebene überschreiben

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: THIS IS LINKED TO THE UI IN THE EDIT PROJECT MODAL)</p>
-->

Sie können ein Projekt so konfigurieren, dass Abrechnungssätze auf Firmenebene anstelle von Abrechnungssätzen auf Projektebene verwendet werden.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan</td> 
   <td>Beliebig</td> 
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

## Aktivieren Sie die Option „Überschreiben der Abrechnungssätze auf Firmenebene“

Wenn eine Firma mit einem Projekt verknüpft ist und diese Option aktiviert ist, wird durch eine Änderung an den Abrechnungssätzen auf Firmenebene der für das Projekt festgelegte Abrechnungssatz überschrieben.

Wenn ein(e) Benutzende(r) die Finanzierungsdaten für das Projekt manuell neu berechnet, werden alle Änderungen an den Abrechnungssätzen auf Firmenebene angewendet. Historische Einnahmenberechnungen werden ebenfalls überschrieben, es sei denn, sie sind als „In Rechnung gestellt“ gekennzeichnet.

1. Gehe zu einem Projekt.
1. Klicken Sie auf das **Mehr** Menü ![Mehr](assets/qs-more-icon-on-an-object.png) neben dem Namen des Projekts in der Kopfzeile und dann auf **Bearbeiten**.
1. Aktivieren **im Abschnitt** die Option **Zulassen, dass Abrechnungssätze auf Firmenebene Abrechnungssätze auf Projektebene überschreiben**.

   >[!CAUTION]
   >
   >Durch Aktivierung dieser Option werden historische Umsatzberechnungen überschrieben, es sei denn, sie sind als „In Rechnung gestellt“ gekennzeichnet. Sie können die historischen Umsatzberechnungen beibehalten, indem Sie einen Rechnungsnachweis erstellen. Weitere Informationen finden Sie im Artikel [Rechnungsnachweise erstellen](../../../manage-work/projects/project-finances/create-billing-records.md)

1. Klicken Sie auf **Änderungen speichern**.

## Abrechnungssätze auf Firmenebene aktualisieren und auf ein Projekt anwenden

Nachdem Sie die Option zum Außerkraftsetzen der Abrechnungssätze auf Firmenebene für ein Projekt aktiviert haben, werden Änderungen an den Abrechnungssätzen des Unternehmens immer dann auf das Projekt angewendet, wenn die Finanzen neu berechnet werden.

>[!NOTE]
>
>Benutzer müssen Zugriff auf Firmen in ihrer Zugriffsebene haben, um Abrechnungssätze auf Firmenebene aktualisieren zu können.

{{step-1-to-setup}}

1. Klicken Sie auf **Firmen**.
1. Klicken Sie auf den Namen der Firma, die dem Projekt zugeordnet ist, für das Sie die Außerkraftsetzung der Abrechnungssätze auf Firmenebene aktiviert haben.
1. Klicken **im linken** auf „Abrechnungssätze“.
1. Aktualisieren Sie den **Abrechnungssatz des Unternehmens** und das Start-/Enddatum für ein vorhandenes Aufgabengebiet und drücken Sie dann die Eingabetaste.

   Um einen neuen Datumswert für den effektiven Abrechnungssatz des Unternehmens hinzuzufügen, wählen Sie einen Abrechnungssatz für das Aufgabengebiet aus und klicken Sie auf **Bearbeiten**. Weitere Informationen zu Datumsangaben für Abrechnungssätze für Unternehmen finden Sie unter [Abrechnungssätze für Aufgabengebiete auf Firmenebene überschreiben](/help/quicksilver/administration-and-setup/set-up-workfront/organizational-setup/override-job-role-billing-rates-company-level.md).

1. Führen Sie einen der folgenden Schritte aus, um die Unternehmenstarife für ein oder mehrere Projekte zu aktualisieren:

   * Mehrere Projekte:

      1. Zu einer Projektliste gehen.
      1. Aktivieren Sie das Kontrollkästchen entsprechend den Projekten, die Sie aktualisieren möchten.
      1. Klicken Sie **Bearbeiten**.
      1. Aktivieren Sie im Abschnitt Einstellungen die Option **Kosten und Einnahmen neu berechnen**.
      1. Klicken Sie auf **Änderungen speichern**.

   * Einzelnes Projekt:

      1. Gehen Sie zu dem Projekt, für das Sie die Außerkraftsetzung der Abrechnungssätze auf Firmenebene aktiviert haben.
      1. Klicken Sie auf das **Mehr** Menü ![Mehr](assets/qs-more-icon-on-an-object.png) neben dem Projektnamen in der Kopfzeile und dann auf **Finanzen neu berechnen**.
