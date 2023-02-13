---
product-area: projects
navigation-topic: financials
title: Überschreiben von Abrechnungsraten auf Projektebene mit Abrechnungsraten auf Unternehmensebene
description: Überschreiben von Abrechnungsraten auf Projektebene mit Abrechnungsraten auf Unternehmensebene
author: Alina
feature: Work Management
exl-id: 02ea4c7c-0473-4cc4-913c-3baa613767b7
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '485'
ht-degree: 0%

---

# Überschreiben von Abrechnungsraten auf Projektebene mit Abrechnungsraten auf Unternehmensebene

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: THIS IS LINKED TO THE UI IN THE EDIT PROJECT MODAL)</p>
-->

Sie können ein Projekt so konfigurieren, dass Abrechnungssätze auf Unternehmensebene anstelle von Abrechnungsraten auf Projektebene verwendet werden.

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
   <td> <p>Zugriff auf Projekte und Finanzdaten bearbeiten</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Verwalten von Berechtigungen für das Projekt mit Berechtigungen zum Verwalten der Finanzen</p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Aktivieren Sie die Option Außerkraftsetzen der Abrechnungsraten auf Unternehmensebene .

Wenn ein Unternehmen mit einem Projekt verknüpft ist und diese Option aktiviert ist, setzen Änderungen an den Abrechnungsraten auf Unternehmensebene den für das Projekt festgelegten Abrechnungskurs außer Kraft.

Wenn ein Benutzer die Projektfinanzierung manuell neu berechnet, werden alle Änderungen an den Abrechnungsraten auf Unternehmensebene angewendet. Historische Umsatzberechnungen werden ebenfalls überschrieben, es sei denn, sie sind als abgerechnet gekennzeichnet.

1. Wechseln Sie zu einem Projekt.
1. Klicken Sie auf **Mehr** Menü ![](assets/qs-more-icon-on-an-object.png) neben dem Namen des Projekts in der Kopfzeile und klicken Sie dann auf **Bearbeiten**.
1. Im **Finanzen** aktivieren Sie die **Erlauben Sie, dass die Abrechnungsraten auf Unternehmensebene die Abrechnungsraten auf Projektebene außer Kraft setzen.**.

   >[!CAUTION]
   >
   >Wenn Sie diese Option aktivieren, werden historische Umsatzberechnungen überschrieben, es sei denn, sie sind als abgerechnet gekennzeichnet. Sie können die historischen Umsatzberechnungen beibehalten, indem Sie einen Rechnungsdatensatz erstellen. Weitere Informationen finden Sie im Artikel [Rechnungsdatensätze erstellen](../../../manage-work/projects/project-finances/create-billing-records.md)

1. Klicken **Änderungen speichern**.

## Aktualisierung der Abrechnungsraten auf Unternehmensebene und Anwendung auf ein Projekt

Nachdem Sie die Option zum Außerkraftsetzen der Abrechnungsraten auf Unternehmensebene für ein Projekt aktiviert haben, gelten die Änderungen an den Abrechnungskursen des Unternehmens für das Projekt jedes Mal, wenn die Finanzen neu berechnet werden.

>[!NOTE]
>
>Benutzer müssen auf der Zugriffsebene auf Unternehmen Zugriff haben, um die Abrechnungsraten auf Unternehmensebene zu aktualisieren.

1. Klicken Sie auf **Hauptmenü** icon ![](assets/main-menu-icon.png) Klicken Sie oben rechts in Adobe Workfront auf **Einrichtung**.
1. Klicken **Unternehmen**.
1. Klicken Sie auf den Namen des Unternehmens, das mit dem Projekt verknüpft ist, für das Sie die Außerkraftsetzung der Abrechnungsraten auf Unternehmensebene aktiviert haben.
1. Klicken **Abrechnungssätze** im linken Bereich.
1. Geben Sie die neue Abrechnungsrate für eine vorhandene Auftragsrolle in der **Abrechnungsrate des Unternehmens** und drücken Sie die Eingabetaste.
1. Führen Sie einen der folgenden Schritte aus, um die Unternehmenspreise für ein oder mehrere Projekte zu aktualisieren:

   * Mehrere Projekte:
   1. Gehen Sie zu einer Projektliste.
   1. Aktivieren Sie das Kontrollkästchen entsprechend den zu aktualisierenden Projekten.
   1. Klicken **Bearbeiten**.
   1. Aktivieren Sie im Abschnitt Einstellungen die Option **Neuberechnung von Kosten und Einnahmen** -Option.
   1. Klicken **Änderungen speichern**.
   * Einzelprojekt:

      1. Wechseln Sie zu dem Projekt, für das Sie die Außerkraftsetzung der Abrechnungsraten auf Unternehmensebene aktiviert haben.
      1. Klicken Sie auf **Mehr** Menü ![](assets/qs-more-icon-on-an-object.png) neben dem Projektnamen in der Kopfzeile und klicken Sie dann auf **Finanzen neu berechnen**.
