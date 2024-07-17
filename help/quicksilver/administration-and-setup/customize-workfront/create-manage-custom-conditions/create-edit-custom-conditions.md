---
title: Benutzerdefinierte Bedingung erstellen oder bearbeiten
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-conditions
description: Als Adobe Workfront-Administrator können Sie eine benutzerdefinierte Bedingung für Projekte, Aufgaben und Probleme erstellen oder bearbeiten, um sie den Anforderungen Ihres Unternehmens anzupassen.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 5c950862-4358-4aab-997b-223972662150
source-git-commit: a3cb3d9d340d377e301c98480324bfe8bf507382
workflow-type: tm+mt
source-wordcount: '642'
ht-degree: 2%

---

# Benutzerdefinierte Bedingung erstellen oder bearbeiten

Als Adobe Workfront-Administrator können Sie eine benutzerdefinierte Bedingung für Projekte, Aufgaben und Probleme erstellen oder bearbeiten, um sie den Anforderungen Ihres Unternehmens anzupassen.

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront-Abo</td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront-Lizenz</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td>Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Sie müssen Workfront-Administrator sein.</p> <p><b>HINWEIS</b>: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Benutzerdefinierte Bedingung erstellen oder bearbeiten

1. Klicken Sie auf das Symbol **Hauptmenü** oben rechts in Adobe Workfront und klicken Sie dann auf **Setup** ![](assets/gear-icon-settings.png).![](assets/main-menu-icon.png)

1. Klicken Sie auf **Projekteinstellungen** > **Bedingungen**.

1. Klicken Sie auf die Registerkarte des Objekttyps (**Projekt**, **Aufgabe** oder **Problem**), den Sie mit der Bedingung verknüpfen möchten.

1. Um eine neue Bedingung zu erstellen, klicken Sie auf **Neue Bedingung hinzufügen**.

   Oder

   Um eine vorhandene Bedingung zu bearbeiten, bewegen Sie den Mauszeiger über die zu bearbeitende Bedingung und klicken Sie dann auf das Symbol **Bearbeiten** , das ganz rechts angezeigt wird.

   ![](assets/custom-condition-edit-nwe.jpg)

1. Konfigurieren Sie Ihre benutzerdefinierte Bedingung mithilfe der folgenden Optionen:

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
      <td>(Optional) Geben Sie eine Beschreibung des Zwecks der Bedingung für diejenigen ein, die sie verwenden werden.</td> 
     </tr> 
     <tr> 
      <td>Farbe</td> 
      <td>(Optional) Klicken Sie auf das Farbsymbol und wählen Sie dann die gewünschte Farbe für die Bedingung aus, wenn sie in Projekten, Aufgaben oder Problemen angezeigt wird. Sie können auch eine Hexadezimalzahl eingeben.</td> 
     </tr> 
     <tr> 
      <td>Entspricht </td> 
      <td><p>(Erforderlich, nur für Projekte) Klicken Sie auf die Option in der Dropdownliste, die die Funktion Ihrer neuen Bedingung am besten beschreibt. Beispielsweise würden Sie für eine Bedingung mit dem Namen Tracking Well auf Auf Target klicken. Dadurch wird bestimmt, wie Ihre Standardbedingungen funktionieren. Jede von Ihnen erstellte Bedingung muss mit einer der Optionen im Dropdown-Menü übereinstimmen.</p>
      <p>Informationen zu Standardbedingungen finden Sie unter <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-projects.md" class="MCXref xref">Festlegen einer benutzerdefinierten Bedingung als Standard für Projekte</a> und <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-tasks-issues.md" class="MCXref xref">Festlegen einer benutzerdefinierten Bedingung als Standard für Aufgaben und Probleme</a>.</p>
      <p>Diese Option kann nach der Erstellung der Bedingung nicht mehr geändert werden.</p></td> 
     </tr> 
     <tr> 
      <td>Schlüssel</td> 
      <td><p>(Erforderlich) Geben Sie für eine Projektbedingung eine alphanumerische Abkürzung ein, die Benutzer erkennen können. Geben Sie für eine Aufgaben- oder Problembedingung einen zweistelligen numerischen Code von 01 bis 99 ein. </p>
      <p>Dieser Schlüssel, der in der API verwendet wird und für Berichterstellungszwecke verwendet werden kann, muss für jedes Objekt eindeutig sein.</p>
      <p>Nach dem Speichern der Bedingung können Sie den Schlüssel für eine Bedingung nicht mehr ändern. </p></td> 
     </tr> 
     <tr> 
      <td>Bedingung ausblenden</td> 
      <td><p>(Optional) Diese Option ist für benutzerdefinierte Bedingungen verfügbar, die Sie nicht mehr verwenden möchten, die Sie aber aus historischen Gründen beibehalten möchten. </p>
      <p>Wenn Sie eine benutzerdefinierte Bedingung ausblenden, die für Arbeitselemente verwendet wurde, wird sie nach dem Ausblenden weiterhin in diesen Arbeitselementen angezeigt. </p></td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >Sie können die Terminologie und Farben von Bedingungen für alle drei Objektarten standardisieren. Kopieren Sie dazu den Bedingungsnamen und den Farb-Hex-Code von einer Registerkarte (Projekt, Aufgabe, Problem) in die entsprechende Bedingung auf den anderen beiden Registerkarten.

1. (Optional) Ziehen Sie ![](assets/move-icon---dots.png) beliebige Bedingungen an eine neue Position, um die Liste neu anzuordnen.

   Dadurch ändert sich die Reihenfolge, in der Bedingungen in Projekten, Aufgaben und Problemen angezeigt werden:

   * Wenn ein Benutzer ein Projekt bearbeitet

     ![](assets/change-condition-edit-project.png)

   * Wenn ein Benutzer die Bedingung für eine Aufgabe oder ein Problem auf der Registerkarte Updates ändert:

     ![](assets/change-condition-update-comment.png)

   * Wenn ein Benutzer die Bedingung für eine Aufgabe oder ein Problem in einer Listenansicht ändert:

     ![](assets/change-conditions-list-dropdown-only.png)

1. Klicken Sie auf **Speichern**.

Sie können Ihre benutzerdefinierte Bedingung als Standardbedingung für Projekte oder für Aufgaben und Probleme festlegen. Weitere Informationen finden Sie unter [Festlegen einer benutzerdefinierten Bedingung als Standard für Projekte](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-projects.md) und [Festlegen einer benutzerdefinierten Bedingung als Standard für Aufgaben und Probleme](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-tasks-issues.md).

Weitere Informationen zu benutzerdefinierten Bedingungen finden Sie unter [Benutzerdefinierte Bedingungen](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/custom-conditions.md).
