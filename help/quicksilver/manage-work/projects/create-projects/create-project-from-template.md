---
product-area: projects;templates
navigation-topic: create-projects
title: Erstellen eines Projekts mithilfe einer Vorlage
description: Sie können Vorlagen als Framework verwenden, um Projekte in Adobe Workfront zu erstellen. Bei Projekten, die sich oft wiederholen, erübrigt sich durch die Verwendung von Vorlagen für das neue Projekt das wiederholte Erstellen derselben Projekte.
author: Alina
feature: Work Management
exl-id: 622cbfe0-b8c0-4045-bef2-9e21d45bfda0
source-git-commit: d7600a55b3dffb242957234de9d85a0deb1ad2e3
workflow-type: tm+mt
source-wordcount: '1159'
ht-degree: 1%

---

# Erstellen eines Projekts mithilfe einer Vorlage

<!-- Audited: 01/2024 -->

Sie können Vorlagen als Framework verwenden, um Projekte in Adobe Workfront zu erstellen. Bei Projekten, die sich oft wiederholen, erübrigt sich die Verwendung von Vorlagen für die allgemeine Zeitleiste des neuen Projekts, dieselben Projekte wiederholt zu erstellen.

Mit Vorlagen können Sie wiederholbare Prozesse, Informationen und Einstellungen erfassen, die mit Ihren Projekten verknüpft sind. Die mit einer Vorlage verknüpften Informationen werden an das Projekt übertragen. Dazu gehören Aufgaben, Zuweisungen, Dauer, Dokumente, finanzielle Details, Risiken und benutzerdefinierte Formulare.

>[!TIP]
>
>Workfront definiert die Gruppe und den Status des neuen Projekts wie folgt:
>
>* Der Standardstatus eines neuen Projekts, das über eine Vorlage erstellt wurde, entspricht dem Status, den Ihr Workfront-Administrator im Hauptbereich Projektvoreinstellungen oder ein Gruppenadministrator (oder Workfront-Administrator) im Bereich Projektvoreinstellungen für eine Gruppe definiert hat. Informationen zum Konfigurieren von Projektvoreinstellungen finden Sie [Systemweite Projektvoreinstellungen konfigurieren](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md) oder [Projektvoreinstellungen für eine Gruppe konfigurieren](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md).
>
>* Die Gruppe des neuen Projekts ist die Gruppe der Vorlage. Wenn die Vorlage keiner Gruppe zugeordnet ist, ist die Gruppe des Projekts die Hauptgruppe des Benutzers, der das Projekt erstellt.
>
>* Die für ein neues Projekt verfügbaren Status stimmen mit den Status der Projektgruppe überein, bei der es sich entweder um die Gruppe der Vorlage oder die Hauptgruppe des Benutzers handelt, der das Projekt erstellt.

Sie haben die folgenden Optionen, um ein Projekt aus einer Vorlage zu erstellen:

* Erstellen eines Projekts über eine Vorlage im Bereich „Projekte“
* Erstellen eines Projekts anhand einer Vorlage auf Vorlagenebene
* Vorlage an ein vorhandenes Projekt anhängen

  Weitere Informationen finden Sie unter [Anhängen einer Vorlage an ein Projekt](../../../manage-work/projects/create-and-manage-templates/attach-template-to-project.md).

* Erstellen eines Projekts über eine Vorlage im Bereich Gruppen

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Paket</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Workfront-Lizenz</td> 
   <td> <p>Standard</p>
        <p>Plan</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfiguration der Zugriffsebene</td> 
   <td> <p>Zugriff auf Projekte und Vorlagen bearbeiten</p>
   <p>Bearbeiten Sie den Zugriff auf Portfolios und Programme, wenn die verwendete Vorlage einen Portfolio und ein Programm enthält</p>  
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Anzeigen von Berechtigungen für eine Vorlage</p> 
  <p>Wenn die verwendete Vorlage eine Portfolio und ein Programm enthält, müssen Sie über Verwaltungsberechtigungen für das Portfolio und das Programm verfügen, um das Projekt zu erstellen </p> 
   <p>Wenn Sie ein Projekt erstellen, erhalten Sie automatisch Verwaltungsberechtigungen für das Projekt.</p></td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Workfront license*</td> 
   <td> <p>New: Standard</p>
        <p>or</p>
        <p>Current: Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level</td> 
   <td> <p>Edit access to Projects and to Templates</p>
   
   <p>edit access to Portfolios and Programs, if the template you use contains a Portfolio and a Program</p>
   
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View permissions to a template</p> 
  <p>If the template you use contains a Portfolio and a Program, you must have Manage permissions to the portfolio and program to create the project </p> 
   <p>When you create a project, you automatically receive Manage permissions to the project.</p></td> 
  </tr> 
 </tbody> 
</table>-->

## Erstellen eines Projekts über eine Vorlage im Bereich „Projekte“

Sie können ein Projekt über den Bereich Projekte im Hauptmenü oder über den Bereich Projekte eines Portfolios oder Programms erstellen.

>[!NOTE]
>
>Der System- oder Gruppenadministrator kann die Benutzeroberfläche mithilfe einer Layout-Vorlage ändern. In diesem Fall können einige der Namen der Abschnitte und Bereiche, auf die in den folgenden Schritten verwiesen wird, in Ihrer Instanz von Workfront unterschiedlich sein.

1. Führen Sie einen der folgenden Schritte aus:

   * Klicken Sie auf das **[!UICONTROL Hauptmenü]**-Symbol ![Hauptmenü](/help/_includes/assets/main-menu-icon.png) in der oberen rechten Ecke von Adobe Workfront oder (falls verfügbar) klicken Sie auf das **[!UICONTROL Hauptmenü]**-Symbol ![Hauptmenü](/help/_includes/assets/main-menu-icon-left-nav.png) in der oberen linken Ecke. Klicken Sie auf **Projekte** und erweitern Sie dann **Neues Projekt**.
   * Gehen Sie zu einem Portfolio und erweitern Sie dann **Neues Projekt**.

     >[!TIP]
     >
     >Wenn Sie ein Projekt mit einer Vorlage aus einem Portfolio erstellen, wird das Portfolio-Feld des neuen Projekts aktualisiert und zeigt das Portfolio an, aus dem Sie das Projekt erstellen möchten. Dadurch wird das Portfolio-Feld in der Vorlage überschrieben, falls es angegeben ist.

   * Wechseln Sie zu einem Programm und erweitern Sie dann **Neues Projekt**.

     >[!TIP]
     >
     >Wenn Sie ein Projekt mithilfe einer Vorlage aus einem Programm erstellen, wird das Feld Programm der neuen Projekte aktualisiert und zeigt das Programm an, aus dem Sie das Projekt erstellen möchten. Das Feld Portfolio der Vorlage wird aktualisiert und zeigt das Portfolio des Programms an, aus dem Sie das Projekt erstellen möchten. Dadurch werden die Programmfelder und Portfolio-Felder in der Vorlage überschrieben, falls sie angegeben sind.

   * Wenn Sie Gruppenadministrator sind, können Sie im Abschnitt Projekte einer Gruppe, die Sie verwalten, auch ein Projekt erstellen. Weitere Informationen finden Sie unter [Erstellen und Ändern der Projekte einer Gruppe](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-projects.md).

     >[!TIP]
     >
     >Wenn Sie ein Projekt mit einer Vorlage aus einer Gruppe erstellen, wird die Gruppe, aus der Sie das Projekt erstellen, nur dann im Feld Gruppe des neuen Projekts angezeigt, wenn das Feld Gruppe der Vorlage nicht angegeben ist. Wenn das Feld Vorlagengruppe angegeben ist, wird für das neue Projekt das Feld Gruppe der Vorlage verwendet.

   <!--
   <p>(this, above, is hyperlinked to the classic version of this article; the Milestone View steps are similar to creating a project in Classic than to the way you do it in NWE)</p>
   -->

   ![Neue Projektoptionen](assets/new-project-dropdown.png)

1. Klicken Sie auf den Namen einer Vorlage in der Liste **Favoritenvorlagen**.

   ![Favoritenvorlage auswählen](assets/new-project-from-template-dropdown-with-template-favorites.png)

   Oder

   Gehen Sie folgendermaßen vor:

   1. Wählen Sie **Neues Projekt aus Vorlage** aus.
   1. Beginnen Sie im Feld **Vorlagen suchen** mit der Eingabe des Namens einer Vorlage und klicken Sie darauf, wenn sie in der Liste angezeigt wird.
   1. Überprüfen Sie die Vorlagendetails auf der rechten Seite.

      Die Vorlagendetails umfassen Folgendes:

      * Vorlagendauer
      * Inhaber der Vorlage
      * Die Anzahl der Aufgaben der obersten Ebene, einschließlich der Namen der drei wichtigsten Aufgaben
      * Die Anzahl aller Aufgaben in der Vorlage
      * Die Namen der benutzerdefinierten Vorlagenformulare

   1. (Optional) Bewegen Sie den Mauszeiger über den Namen einer Vorlage im linken Bereich und klicken Sie auf das Symbol **Favoriten** **Symbol** ![Favoriten](assets/favorites-icon-small.png), um sie für die zukünftige Verwendung als Favorit zu markieren.

      Oder

      Erweitern Sie die **Favoritenvorlagen** Liste und wählen Sie eine Vorlage aus der Dropdown-Liste aus.

      >[!TIP]
      >
      >Sie können bis zu 40 Workfront-Elemente als Favoriten markieren. Dazu gehören Vorlagen und andere Elemente.

   1. Klicken Sie **Vorlage verwenden** wenn Sie eine Vorlage ausgewählt haben.

      ![Vorlagendetails](assets/new-project-from-template-small-box-with-template-details-panel.png)

      >[!NOTE]
      >
      >Wenn die Meilenstein -Ansicht auf die Projektliste angewendet wurde, klicken Sie auf den Namen einer Vorlage im Abschnitt **Neu aus Vorlage**.
      >
      >
      >![Meilensteinansicht zum Erstellen eines Projekts aus einer Vorlage](assets/create-project-from-template-box-from-milestone-view-nwe-350x275.png)
      >

   Das **Neues Projekt** wird geöffnet.

   ![Feld Neues Projekt](assets/new-project-from-template-box.png)

1. Wenn ein Feld bereits in der Vorlage ausgefüllt ist, wird das Feld im Feld **Neues Projekt** vorausgefüllt. Sie können die vorausgefüllten Werte bearbeiten, um sie besser an Ihr Projekt anzupassen. Weitere Informationen finden Sie unter [Projekte bearbeiten](../../../manage-work/projects/manage-projects/edit-projects.md).
1. Klicken Sie **Projekt erstellen**.

   Alle in der Vorlage definierten Details werden automatisch dem neu erstellten Projekt zugeordnet, sofern Sie sie im vorherigen Schritt nicht geändert haben.

## Erstellen eines Projekts über eine Vorlage im Bereich Vorlagen

Anstatt im Bereich Projekte zu beginnen, können Sie ein Projekt aus einer Vorlage erstellen, indem Sie mit der Vorlage beginnen.

{{step1-to-templates}}

1. Klicken Sie auf den Namen einer Vorlage, die Sie verwenden möchten.
1. Klicken Sie auf das **Mehr**-Menü ![Mehr-Symbol](assets/more-icon.png) und dann auf **Projekt erstellen**.

   ![Erstellen eines Projekts aus einer Vorlage](assets/project-sharing-on-template.png)

   Das **Neues Projekt** wird geöffnet.

1. Geben Sie einen Namen für das Projekt ein, überprüfen Sie dann jeden Abschnitt und nehmen Sie die erforderlichen Änderungen vor.

   ![Feld Neues Projekt](assets/new-project-from-template-box.png)

   Wenn ein Feld bereits in der Vorlage ausgefüllt ist, wird das Feld im Feld **Neues Projekt** vorausgefüllt. Sie können die vorausgefüllten Werte bearbeiten, um sie besser an Ihr Projekt anzupassen. Weitere Informationen finden Sie unter [Projekte bearbeiten](../../../manage-work/projects/manage-projects/edit-projects.md).

1. Klicken Sie **Projekt erstellen**.

   Alle in der Vorlage definierten Details werden automatisch dem neu erstellten Projekt zugeordnet, sofern Sie sie im vorherigen Schritt nicht geändert haben.
