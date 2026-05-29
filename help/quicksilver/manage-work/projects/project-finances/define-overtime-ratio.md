---
content-type: overview
product-area: projects
navigation-topic: financials
title: Definieren eines Überstundenverhältnisses
description: Sie können ein Überstundenverhältnis für einen Vorgang definieren, um die Berechnung des geplanten Umsatzes für die Aufgabenzuordnungen anzupassen.
author: Lisa
feature: Work Management
exl-id: 832d3aab-3e09-4d83-91a6-be0145ce3554
source-git-commit: 39630b50384d710dadb1f48342113b74338a9104
workflow-type: tm+mt
source-wordcount: '349'
ht-degree: 11%

---

# Definieren eines Überstundenverhältnisses

Wenn einer Aufgabe ein Überstundenverhältnis hinzugefügt wird, wird es auf alle Zuweisungen der Aufgabe angewendet. Es multipliziert alle geplanten Stunden für diese Aufgabe und wirkt sich auf die Berechnungen des geplanten Umsatzes aus.

Das Überstundenverhältnis kann für Zuweisungen innerhalb derselben Aufgabe nicht variieren. Wenn verschiedene Überstundenmultiplikatoren erforderlich sind, müssen Sie separate Teilaufgaben unter einer übergeordneten Aufgabe erstellen.

>[!NOTE]
>
>Es gibt keine Validierung, die verhindert, dass das Überstundenverhältnis zu einer Aufgabe ohne Überstunden hinzugefügt wird.

## Berechnung der Überstunden bei den geplanten Einnahmen

Das System bestimmt zunächst den Abrechnungssatz anhand der Standard-Abrechnungssatz-Hierarchie. Weitere Informationen finden Sie unter [Übersicht über Umsatz und Kostenhierarchie](/help/quicksilver/manage-work/projects/project-finances/overview-revenue-cost-hierarchy.md).

Wenn das Überstundenverhältnis für die Aufgabe vorhanden ist, lautet die Berechnung:
Geplanter Umsatz = Abrechnungssatz × Verhältnis Überstunden × geplanten Stunden

Wenn das Überstundenverhältnis leer ist, lautet die Berechnung:
Geplanter Umsatz = Abrechnungssatz × geplante Stunden

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
   <td>Zugriff auf Aufgaben, Projekte und Finanzdaten bearbeiten</td> 
  </tr> 
  <tr> 
   <td>Objektberechtigungen</td> 
   <td><p>Berechtigungen für eine Aufgabe verwalten, einschließlich Verrechnungssätze bearbeiten</p>
     <p>Mitwirken an oder höhere Berechtigungen für das Projekt</p></td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) in der Dokumentation zu Workfront.

+++

## Voraussetzungen

Der Aufgabenumsatztyp muss „Benutzer und Funktion pro Stunde“ lauten. Weitere Informationen finden Sie unter [Übersicht über Umsatz und Kostenhierarchie](/help/quicksilver/manage-work/projects/project-finances/overview-revenue-cost-hierarchy.md).

Das Feld **Überstundenverhältnis** muss in Ihrer Layout-Vorlage aktiviert sein.

1. Klicken Sie in der Layout-Vorlage unter **Was Benutzer sehen“ auf den Abwärtspfeil** dann auf **Aufgabe**.
1. Wählen Sie **Abschnitt** das Feld **Überstundenverhältnis** im Bereich **Finanzen** aus.

   Weitere Informationen finden Sie unter [Anpassen der Detailansicht mithilfe einer Layout-Vorlage](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

## Definieren des Überstundenverhältnisses für eine Aufgabe

1. Wechseln Sie zu der Aufgabe, die Sie bearbeiten möchten.

   Weitere Informationen finden Sie unter [Verwalten der Aufgabenfinanzen im Abschnitt „Aufgabendetails“](/help/quicksilver/manage-work/tasks/manage-tasks/task-finances-in-details.md).

1. Klicken Sie **linken** auf „Aufgabendetails“.
1. Geben Sie **Bereich &quot;**&quot; den Multiplikator für Überstunden in das Feld **Überstundenverhältnis** ein.
1. Klicken Sie auf **Änderungen speichern**.
