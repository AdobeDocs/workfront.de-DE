---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: Überblick über das tatsächliche Startdatum des Projekts
description: Projekte, Aufgaben und Probleme haben in Adobe Workfront ein tatsächliches Startdatum. Bei Aufgaben und Problemen ist dies das Datum, an dem sie als In Bearbeitung markiert wurden. Bei Projekten ist dies das Datum, an dem die erste Aufgabe für das Projekt als In Bearbeitung markiert oder abgeschlossen wurde.
author: Alina
feature: Work Management
exl-id: 4357b072-24f6-4f89-b624-f066f8af0722
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/DWzx7-PW4nb78Q-XuI0AUjcCOFFap-f3qunguTclLpE
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2:
  - id: b91c0848-76c4-4da4-8b81-3aade0518dd0
  - id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 530
ht-degree: 8%

---

# Überblick über das tatsächliche Startdatum des Projekts

Projekte, Aufgaben und Probleme haben in Adobe Workfront ein tatsächliches Startdatum. Bei Aufgaben und Problemen ist dies das Datum, an dem sie als In Bearbeitung markiert wurden. Bei Projekten ist dies das Datum, an dem die erste Aufgabe für das Projekt als In Bearbeitung markiert oder abgeschlossen wurde.

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Paket</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td><p>Licht oder höher</p> 
   <p>Überprüfen oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriff auf Projekte anzeigen oder höher</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Anzeigen oder Erweitern von Berechtigungen für ein Projekt</p>  </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) in der Dokumentation zu Workfront.

+++

<!--
Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Review or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>View or higher access to Projects</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View or higher permissions to a project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

## Überlegungen zu tatsächlichen Startdaten in Workfront

* Das tatsächliche Startdatum befindet sich im Abschnitt Details von Projekten, Aufgaben und Problemen.
* Das tatsächliche Startdatum eines Projekts, einer Aufgabe oder eines Problems wird beim Erstellen dieser Elemente nicht angegeben.
* Das tatsächliche Startdatum wird zu Beginn der eigentlichen Arbeit an dem Projekt, der Aufgabe oder dem Problem angegeben.
* Das tatsächliche Startdatum wird nicht auf der Registerkarte Projektdetails angezeigt, wenn die Arbeit am Projekt noch nicht begonnen hat.

  Das tatsächliche Startdatum wird auf den Registerkarten „Aufgabe“ und „Problemdetails“ leer angezeigt, wenn die Arbeit daran noch nicht begonnen hat.

* Sie können das tatsächliche Startdatum einer Aufgabe oder eines Problems manuell ändern, aber nicht das tatsächliche Startdatum eines Projekts.

## Überlegungen zu tatsächlichen Startdaten für Projekte

* Workfront legt automatisch das tatsächliche Datum eines Projekts fest, wenn eine der folgenden Situationen eintritt:

   * Ein Aufgabenbevollmächtigter ändert den Status einer Aufgabe von *Neu* in einen anderen Status, der nicht *Neu* entspricht.

   * Ein Aufgabenbevollmächtigter ändert den Bereich „Prozent abgeschlossen“ einer Aufgabe.

     >[!IMPORTANT]
     >
     >Das tatsächliche Startdatum des Projekts wird nicht angezeigt, wenn das Projekt als aktuell markiert ist. Die tatsächliche Arbeit an den Aufgaben des Projekts muss beginnen, bevor das tatsächliche Startdatum des Projekts angegeben wird.

     In diesen Fällen wird das tatsächliche Startdatum des Projekts auf das Datum und die Uhrzeit festgelegt, zu der diese Aktionen für die früheste Aufgabe im Projekt stattgefunden haben. Dies zeigt an, dass das Projekt tatsächlich an diesem Datum und zu dieser Uhrzeit gestartet wurde.

## Suchen des tatsächlichen Startdatums eines Projekts

Sie können das tatsächliche Startdatum eines Projekts in den folgenden Bereichen ermitteln:

* Im Abschnitt Details eines Projekts.
* Wenn Sie in einem Projektbericht oder einer Projektansicht das **Tatsächliche Startdatum** für das Projektobjekt im Bericht hinzufügen.

  Informationen zum Erstellen von Berichten finden Sie im Artikel [Erstellen eines benutzerdefinierten Berichts](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

So suchen Sie das tatsächliche Startdatum im Abschnitt Details des Projekts:

{{step1-to-projects}}

1. Klicken Sie auf das Projekt, für das Sie das tatsächliche Startdatum anzeigen möchten.
1. Klicken Sie **linken Bereich auf** Projektdetails“ und navigieren Sie dann zum Abschnitt **Übersicht**.

   ![Tatsächliches Startdatum des Projekts hervorgehoben](assets/nwe-project-actual-start-date--highlighted-350x367.png)

   Das **Tatsächliches Startdatum** wird zusammen mit anderen Projektdaten angezeigt.


