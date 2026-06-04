---
title: Erstellen oder Bearbeiten einer benutzerdefinierten Bedingung
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-conditions
description: Als Adobe Workfront-Administrator können Sie eine benutzerdefinierte Bedingung für Projekte, Aufgaben und Probleme erstellen oder bearbeiten, um sie an die Anforderungen Ihres Unternehmens anzupassen.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 5c950862-4358-4aab-997b-223972662150
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/3GEaVitQ5ATF7lE4cNeuSqbL6vMVg-WGKOeh8T66T8w
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: bce87dde-a4ab-44c9-8a18-ad66e4ddb377
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 627
ht-degree: 7%

---

# Erstellen oder Bearbeiten einer benutzerdefinierten Bedingung

Als Adobe Workfront-Administrator können Sie eine benutzerdefinierte Bedingung für Projekte, Aufgaben und Probleme erstellen oder bearbeiten, um sie an die Anforderungen Ihres Unternehmens anzupassen.

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront-Paket</td> 
   <td><p>Beliebig</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront-Lizenz</td> 
   <td><p>Standard</p>
       <p>Abo</p></td>
  </tr> 
  <tr> 
   <td>Konfigurationen der Zugriffsebene</td> 
   <td>Systemadmin</td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Erstellen oder Bearbeiten einer benutzerdefinierten Bedingung

{{step-1-to-setup}}

1. Klicken Sie **Projektvoreinstellungen** > **Bedingungen**.

1. Klicken Sie auf die Registerkarte des Objekttyps (**Projekt**, **Aufgabe** oder **Problem**), den Sie mit der Bedingung verknüpfen möchten.

1. Um eine neue Bedingung zu erstellen, klicken Sie auf **Neue Bedingung hinzufügen**.

   ODER

   Um eine vorhandene Bedingung zu bearbeiten, klicken Sie **Bearbeiten** neben dem Namen der Bedingung.

   ![Benutzerdefinierte Bedingung bearbeiten](assets/custom-conditions-0825.png)

1. Konfigurieren Sie Ihre benutzerdefinierte Bedingung mit den folgenden Optionen:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td>Name der Bedingung</td> 
      <td>(Erforderlich) Geben Sie einen beschreibenden Namen für die Bedingung ein.</td> 
     </tr> 
     <tr> 
      <td>Beschreibung</td> 
      <td>(Optional) Geben Sie eine Beschreibung des Zwecks der Bedingung für die Benutzer ein, die sie verwenden werden.</td> 
     </tr> 
     <tr> 
      <td>Farbe</td> 
      <td>(Optional) Klicken Sie auf das Farbsymbol und wählen Sie dann die Farbe aus, die Sie für die Bedingung verwenden möchten, wenn sie in Projekten, Aufgaben oder Problemen angezeigt wird. Sie können auch eine Hexadezimalzahl eingeben.</td> 
     </tr> 
     <tr> 
      <td>Entspricht </td> 
      <td><p>(Erforderlich, nur für Projekte) Klicken Sie auf die Option in der Dropdown-Liste, die die Funktion Ihrer neuen Bedingung am besten beschreibt. Beispiel: Für eine Bedingung mit dem Namen „Tracking Well“ würden Sie auf „Target“ klicken. Dadurch wird festgelegt, wie Ihre Standardbedingungen funktionieren. Jede von Ihnen erstellte Bedingung muss mit einer der Optionen im Dropdown-Menü übereinstimmen.</p>
      <p>Weitere Informationen zu Standardbedingungen finden Sie unter <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-projects.md" class="MCXref xref">Festlegen einer benutzerdefinierten Bedingung als Standard für Projekte</a> und <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-tasks-issues.md" class="MCXref xref">Festlegen einer benutzerdefinierten Bedingung als Standard für Aufgaben und Probleme</a>.</p>
      <p>Diese Option kann nach Abschluss der Erstellung der Bedingung nicht mehr geändert werden.</p></td> 
     </tr> 
     <tr> 
      <td>Schlüssel</td> 
      <td><p>(Erforderlich) Geben Sie für eine Projektbedingung eine alphanumerische Abkürzung ein, die Benutzende erkennen können. Geben Sie für eine Aufgaben- oder Problembedingung einen zweistelligen numerischen Code von 01 bis 99 ein. </p>
      <p>Dieser Schlüssel, der in der API verwendet wird und zu Berichtszwecken verwendet werden kann, muss für jedes Objekt eindeutig sein.</p>
      <p>Sie können den Schlüssel für eine Bedingung nach dem Speichern der Bedingung nicht mehr ändern. </p></td> 
     </tr> 
     <tr> 
      <td>Bedingung ausblenden</td> 
      <td><p>(Optional) Diese Option ist für benutzerdefinierte Bedingungen verfügbar, die Personen nicht mehr verwenden sollen, die sie jedoch aus historischen Gründen beibehalten möchten. </p>
      <p>Wenn Sie eine benutzerdefinierte Bedingung ausblenden, die für Arbeitselemente verwendet wurde, wird sie nach dem Ausblenden weiterhin in diesen Arbeitselementen angezeigt. </p></td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >Sie können Bedingungsterminologie und Farben für alle drei Objekttypen standardisieren. Kopieren Sie dazu den Bedingungsnamen und den Hex-Farb-Code von einer Registerkarte (Projekt, Aufgabe, Problem) in die entsprechende Bedingung auf den anderen beiden Registerkarten.

1. (Optional) Ziehen Sie ![Symbol Verschieben](assets/move-icon---dots.png) eine beliebige Bedingung an eine neue Position, um die Liste neu anzuordnen.

   Dadurch wird die Reihenfolge geändert, in der Bedingungen in Projekten, Aufgaben und Problemen angezeigt werden:

   * Wenn ein Benutzer ein Projekt bearbeitet

     ![Bedingung beim Bearbeiten eines Projekts ändern](assets/change-condition-edit-project-0825.png)

   * Wenn ein(e) Benutzende(r) die Bedingung für eine Aufgabe oder ein Problem in einer Listenansicht ändert:

     ![Bedingung in Liste ändern](assets/change-conditions-list-dropdown-0925.png)

     >[!NOTE]
     >
     >In der Ansicht „Standardbedingung“ ist **Feld** Bedingung“ ein Feldtyp, der nicht inline bearbeitet werden kann. Wenn Sie das Feld **Bedingung** separat zu einer Ansicht hinzufügen, kann es bearbeitet werden. Weitere Informationen zur Inline-Bearbeitung finden Sie unter [Inline-Bearbeitung von Elementen in einer Liste in Adobe Workfront](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/inline-edit-objects.md).

1. Klicken Sie auf **Speichern**.

Sie können Ihre benutzerdefinierte Bedingung als Standardbedingung für Projekte oder für Aufgaben und Probleme festlegen. Weitere Informationen finden Sie unter [Festlegen einer benutzerdefinierten Bedingung als Standard für Projekte](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-projects.md) und [Festlegen einer benutzerdefinierten Bedingung als Standard für Aufgaben und Probleme](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-tasks-issues.md).

Weitere Informationen zu benutzerdefinierten Bedingungen finden Sie unter [Benutzerdefinierte Bedingungen](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/custom-conditions.md).


<!-- 
   THIS WAS ORIGINALLY BETWEEN THE OTHER TWO BULLETS.
   * When a user is changing the condition for a task or issue on the Updates tab:

     ![Change condition when updating comment](assets/change-condition-update-comment.png)
   -->
