---
content-type: overview
product-area: projects
navigation-topic: financials
title: Aufgabengebiet für Abrechnung einrichten
description: Mit Workfront können Sie einem Benutzer ein anderes Aufgabengebiet in Rechnung stellen als sein primäres. Dies ist nützlich, wenn eine Person vorübergehend Arbeiten erledigt, die zu einem anderen Satz in Rechnung gestellt werden sollten.
author: Lisa
feature: Work Management
exl-id: d6e2947d-2f40-4591-b048-9a769caadf43
source-git-commit: 39630b50384d710dadb1f48342113b74338a9104
workflow-type: tm+mt
source-wordcount: '680'
ht-degree: 5%

---

# Aufgabengebiet für Abrechnung einrichten

Mit Workfront können Sie einem Benutzer ein anderes Aufgabengebiet in Rechnung stellen als sein primäres. Dies ist nützlich, wenn eine Person vorübergehend Arbeiten erledigt, die zu einem anderen Satz in Rechnung gestellt werden sollten.

Sie können ein Aufgabengebiet für die Fakturierung auf zwei Arten zuweisen:

* Auf Projektebene: Verwenden Sie diese Option, wenn der Person für das gesamte Projekt dasselbe Aufgabengebiet in Rechnung gestellt werden soll.
* Auf Zuordnungsebene: Verwenden Sie diese Option, wenn Sie für bestimmte Aufgaben eine andere Rechnung erstellen möchten.

>[!NOTE]
>
>* Ein Aufgabengebiet für die Fakturierung gilt nur für Personen (Benutzer). Dies gilt nicht für generische Aufgabengebiete oder Platzhalter.
>* Das Hinzufügen eines Aufgabengebiets für die Abrechnung wirkt sich nur auf den Abrechnungssatz aus, nicht auf die Kosten.
>* Die Fakturierung auf Zuordnungsebene hat immer Vorrang vor der Fakturierung auf Projektebene.

Weitere Informationen finden Sie unter [Übersicht über Umsatz und Kostenhierarchie](/help/quicksilver/manage-work/projects/project-finances/overview-revenue-cost-hierarchy.md) und [Erweiterte Zuordnungen erstellen](/help/quicksilver/manage-work/tasks/assign-tasks/create-advanced-assignments.md).

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
   <td> Zugriff auf Tarifkarten bearbeiten</td> 
  </tr> 
  <tr> 
   <td>Objektberechtigungen</td> 
   <td>Verwalten von Berechtigungen für das Projekt </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) in der Dokumentation zu Workfront.

+++

## Aufgabengebiet für die Fakturierung auf Projektebene zuweisen

Wenn Sie ein Aufgabengebiet für die Fakturierung eines Projekts erstellen:

* Die Funktion Abrechnung gilt für alle Aufgaben und Zuweisungen innerhalb des Projekts für diesen Benutzer.
* Für die Fakturierung wird der Abrechnungssatz des ausgewählten Aufgabengebiets verwendet, die Kosten folgen jedoch weiterhin der primären Funktion des Benutzers.

So weisen Sie ein Aufgabengebiet für die Fakturierung auf Projektebene zu:

1. Öffnen Sie ein Projekt.
1. Klicken Sie **linken Bedienfeld auf** Ressource für Abrechnung“.
1. Wählen Sie die Registerkarte **Aufgabengebiet für Abrechnung** aus, falls sie noch nicht angezeigt wird.
1. Klicken Sie **Hinzufügen > Aufgabengebiet für Abrechnung hinzufügen**.
1. Wählen Sie im Feld **Aufgabengebiet für Abrechnung hinzufügen** die Option **Benutzer** aus.
1. Wählen Sie das **Aufgabengebiet** aus, das als Aufgabengebiet für die Fakturierung für diesen Benutzer für dieses Projekt verwendet werden soll.
1. (Optional) Klicken Sie auf **Aufgabengebiet hinzufügen**, um Gültigkeitsdaten für das Aufgabengebiet „Abrechnung“ zu definieren. Geben Sie die **Start** und **Ende** für das Aufgabengebiet ein.

[Aufgabengebiet für die Fakturierung auf Projektebene hinzufügen](assets/jrfb-project-level.png)

1. Klicken **erneut auf „Aufgabengebiet hinzufügen**, um zusätzliche Rollen für die Abrechnung für verschiedene Zeiträume anzugeben.
1. Klicken Sie auf **Speichern**.

### Beispiel auf Projektebene

>[!BEGINSHADEBOX]

Johns wichtigstes Aufgabengebiet ist Designer 1. Für das Projekt ist ein Senior Designer erforderlich, und John wird eingeschaltet.

In diesem Fall würden Sie das Aufgabengebiet für Abrechnung auf Projektebene **Senior** Designer) festlegen.

Ergebnis:

* Der Fakturaerlös ist der Senior Designer-Satz
* Kosten ist der Designer 1-Kostensatz (Ist-Kostensatz von John)

>[!ENDSHADEBOX]

## Aufgabengebiet für die Fakturierung auf Zuordnungsebene zuweisen

Wenn Sie ein Aufgabengebiet für die Fakturierung für einen Arbeitsauftrag hinzufügen, überschreibt die Einstellung nur für diesen bestimmten Arbeitsauftrag ein Fakturierungsgebiet auf Projektebene.

So weisen Sie ein Aufgabengebiet für die Fakturierung auf Zuordnungsebene zu:

1. Öffnen Sie ein Projekt und suchen Sie die Aufgabe.
1. Navigieren Sie zu „Erweiterte **&quot; der**.

   Weitere Informationen finden Sie unter [Erstellen erweiterter Zuweisungen](/help/quicksilver/manage-work/tasks/assign-tasks/create-advanced-assignments.md).

1. Suchen Sie im Aufgabenzuweisungsraster die Spalte **Aufgabengebiet für die Abrechnung**.
1. Wählen Sie für jede Stelle, für die Sie unterschiedliche Abrechnungen benötigen, ein Aufgabengebiet aus.

   >[!NOTE]
   >
   >Wenn ein Aufgabengebiet für die Fakturierung auf Projektebene zugewiesen wurde, wird es in der Zuweisung angezeigt. Sie können in das Feld **Aufgabengebiet für die Abrechnung** klicken und ein anderes Aufgabengebiet auswählen, das für die Zuweisung verwendet werden soll.
   >Das Informationssymbol informiert Sie darüber, ob ein Aufgabengebiet für die Fakturierung auf Projekt- oder Zuordnungsebene definiert wurde.

   ![Aufgabengebiet für die Fakturierung für einen Arbeitsauftrag](assets/jrfb-assignment-level.png)

### Beispiel auf Zuweisungsebene

>[!BEGINSHADEBOX]

Johns wichtigstes Aufgabengebiet ist Designer 1. Er wird auf Projektebene als Senior Designer abgerechnet. Für eine Sonderaufgabe ist jedoch ein Principal Designer-Abrechnungssatz erforderlich.

Sie würden das Aufgabengebiet für die Fakturierung nur für diese Zuweisung auf den Prinzipal-Designer festlegen.

Ergebnis:

* Alle anderen Aufgaben von John werden als Senior Designer abgerechnet
* Diese eine Aufgabe wird als Prinzipal-Designer abgerechnet
* Kosten bleiben Designer 1

>[!ENDSHADEBOX]
