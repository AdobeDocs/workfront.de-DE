---
product-area: projects
navigation-topic: financials
title: Überschreiben von Abrechnungsraten auf Projektebene mit Abrechnungsraten auf Unternehmensebene
description: Überschreiben von Abrechnungsraten auf Projektebene mit Abrechnungsraten auf Unternehmensebene
author: Lisa
feature: Work Management
exl-id: 02ea4c7c-0473-4cc4-913c-3baa613767b7
source-git-commit: e5a87b92bf1f6c2e0485ba8a2eb73e52c422b2fc
workflow-type: tm+mt
source-wordcount: '472'
ht-degree: 1%

---

# Überschreiben von Abrechnungsraten auf Projektebene mit Abrechnungsraten auf Unternehmensebene

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: THIS IS LINKED TO THE UI IN THE EDIT PROJECT MODAL)</p>
-->

Sie können ein Projekt so konfigurieren, dass Abrechnungssätze auf Unternehmensebene anstelle von Abrechnungsraten auf Projektebene verwendet werden.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

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
   <td>
   <p>Neu: Standard</p>
   <p>oder</p>
   <p>Aktuell: Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td>Zugriff auf Projekte und Finanzdaten bearbeiten</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td>Verwalten von Berechtigungen für das Projekt mit Berechtigungen zum Verwalten der Finanzen</td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Aktivieren Sie die Option Außerkraftsetzen der Abrechnungsraten auf Unternehmensebene .

Wenn ein Unternehmen mit einem Projekt verknüpft ist und diese Option aktiviert ist, setzen Änderungen an den Abrechnungsraten auf Unternehmensebene den für das Projekt festgelegten Abrechnungskurs außer Kraft.

Wenn ein Benutzer die Projektfinanzierung manuell neu berechnet, werden alle Änderungen an den Abrechnungsraten auf Unternehmensebene angewendet. Historische Umsatzberechnungen werden ebenfalls überschrieben, es sei denn, sie sind als abgerechnet gekennzeichnet.

1. Wechseln Sie zu einem Projekt.
1. Klicken Sie auf das Menü **Mehr** neben dem Namen des Projekts in der Kopfzeile und dann auf **Bearbeiten**.![](assets/qs-more-icon-on-an-object.png)
1. Aktivieren Sie im Abschnitt **Finanzen** die Option **Zulassen von Abrechnungsraten auf Unternehmensebene, um die Abrechnungsraten auf Projektebene zu überschreiben**.

   >[!CAUTION]
   >
   >Wenn Sie diese Option aktivieren, werden historische Umsatzberechnungen überschrieben, es sei denn, sie sind als abgerechnet gekennzeichnet. Sie können die historischen Umsatzberechnungen beibehalten, indem Sie einen Rechnungsdatensatz erstellen. Weitere Informationen finden Sie im Artikel [Erstellen von Rechnungsdatensätzen](../../../manage-work/projects/project-finances/create-billing-records.md) .

1. Klicken Sie auf **Änderungen speichern**.

## Aktualisierung der Abrechnungsraten auf Unternehmensebene und Anwendung auf ein Projekt

Nachdem Sie die Option zum Außerkraftsetzen der Abrechnungsraten auf Unternehmensebene für ein Projekt aktiviert haben, gelten die Änderungen an den Abrechnungskursen des Unternehmens für das Projekt jedes Mal, wenn die Finanzen neu berechnet werden.

>[!NOTE]
>
>Benutzer müssen auf der Zugriffsebene auf Unternehmen Zugriff haben, um die Abrechnungsraten auf Unternehmensebene zu aktualisieren.

{{step-1-to-setup}}

1. Klicken Sie auf **Unternehmen**.
1. Klicken Sie auf den Namen des Unternehmens, das mit dem Projekt verknüpft ist, für das Sie die Außerkraftsetzung der Abrechnungsraten auf Unternehmensebene aktiviert haben.
1. Klicken Sie im linken Bereich auf **Abrechnungsraten**.
1. Aktualisieren Sie die **Abrechnungsrate des Unternehmens** und das Start-/Enddatum für eine vorhandene Auftragsrolle und drücken Sie dann die Eingabetaste.

   Um einen neuen effektiven Abrechnungskurs für das Datum hinzuzufügen, wählen Sie einen Abrechnungskurs für die Auftragsrolle aus und klicken Sie auf **Bearbeiten**. Weitere Informationen zu datumswirksamen Abrechnungskursen für Unternehmen finden Sie unter [Außerkraftsetzen der Abrechnungsraten für die Rolle des Auftrags auf Unternehmensebene](/help/quicksilver/administration-and-setup/set-up-workfront/organizational-setup/override-job-role-billing-rates-company-level.md).

1. Führen Sie einen der folgenden Schritte aus, um die Unternehmenspreise für ein oder mehrere Projekte zu aktualisieren:

   * Mehrere Projekte:

      1. Gehen Sie zu einer Projektliste.
      1. Aktivieren Sie das Kontrollkästchen entsprechend den zu aktualisierenden Projekten.
      1. Klicken Sie auf **Bearbeiten**.
      1. Aktivieren Sie im Abschnitt Einstellungen die Option **Kosten und Umsatz neu berechnen** .
      1. Klicken Sie auf **Änderungen speichern**.

   * Einzelprojekt:

      1. Wechseln Sie zu dem Projekt, für das Sie die Außerkraftsetzung der Abrechnungsraten auf Unternehmensebene aktiviert haben.
      1. Klicken Sie auf das Menü **Mehr** neben dem Projektnamen in der Kopfzeile und dann auf **Finanzen neu berechnen**.![](assets/qs-more-icon-on-an-object.png)
