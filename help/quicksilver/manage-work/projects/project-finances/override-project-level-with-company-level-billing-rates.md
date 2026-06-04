---
product-area: projects
navigation-topic: financials
title: Überschreiben der Abrechnungssätze auf Projektebene mit Abrechnungssätzen auf Firmenebene
description: Überschreiben der Abrechnungssätze auf Projektebene mit Abrechnungssätzen auf Firmenebene
author: Lisa
feature: Work Management
exl-id: 02ea4c7c-0473-4cc4-913c-3baa613767b7
TQID: https://experienceleague.adobe.com/GQSQGGHBZsBLtI8IEUltVXzxmEtOxue0iE6fpHmYWP4
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40cid: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 475
ht-degree: 15%

---

# Überschreiben der Abrechnungssätze auf Projektebene mit Abrechnungssätzen auf Firmenebene

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: THIS IS LINKED TO THE UI IN THE EDIT PROJECT MODAL)</p>
-->

Sie können ein Projekt so konfigurieren, dass Abrechnungssätze auf Firmenebene anstelle von Abrechnungssätzen auf Projektebene verwendet werden.

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront-Paket</td> 
   <td>Beliebig</td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront-Lizenz</td> 
   <td>
   <p>Standard</p>
   <p>Abo</p></td> 
  </tr> 
  <tr> 
   <td>Konfigurationen der Zugriffsebene</td> 
   <td>Zugriff auf Projekte und Finanzdaten bearbeiten</td> 
  </tr> 
  <tr> 
   <td>Objektberechtigungen</td> 
   <td>Verwalten Sie die Berechtigungen für das Projekt mit den Berechtigungen zum Bearbeiten von Abrechnungssätzen und allgemeiner Finanzen.</td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) in der Dokumentation zu Workfront.

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
      1. Klicken Sie auf **Bearbeiten**.
      1. Aktivieren Sie im Abschnitt Einstellungen die Option **Kosten und Einnahmen neu berechnen**.
      1. Klicken Sie auf **Änderungen speichern**.

   * Einzelnes Projekt:

      1. Gehen Sie zu dem Projekt, für das Sie die Außerkraftsetzung der Abrechnungssätze auf Firmenebene aktiviert haben.
      1. Klicken Sie auf das **Mehr** Menü ![Mehr](assets/qs-more-icon-on-an-object.png) neben dem Projektnamen in der Kopfzeile und dann auf **Finanzen neu berechnen**.
