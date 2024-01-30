---
product-area: projects;templates
navigation-topic: create-projects
title: Erstellen eines Projekts mit einer Vorlage
description: Sie können Vorlagen als Framework zum Erstellen von Projekten in Adobe Workfront verwenden. Wenn Sie Projekte haben, die sich häufig wiederholen, sparen Sie sich durch die Verwendung von Vorlagen für die allgemeine Zeitleiste des neuen Projekts, dieselben Projekte wiederholt erstellen zu müssen.
author: Alina
feature: Work Management
exl-id: 622cbfe0-b8c0-4045-bef2-9e21d45bfda0
source-git-commit: 9447310f0d4cf4504ee6d690116fb62f718fe23d
workflow-type: tm+mt
source-wordcount: '1089'
ht-degree: 0%

---

# Erstellen eines Projekts mit einer Vorlage

<!-- Audited: 01/2024 -->

Sie können Vorlagen als Framework zum Erstellen von Projekten in Adobe Workfront verwenden. Wenn Sie Projekte haben, die sich häufig wiederholen, sparen Sie sich durch die Verwendung von Vorlagen für die allgemeine Zeitleiste des neuen Projekts, dieselben Projekte wiederholt erstellen zu müssen.

Vorlagen bieten Ihnen eine Möglichkeit, wiederholbare Prozesse, Informationen und Einstellungen zu erfassen, die mit Ihren Projekten verknüpft sind. Die mit einer Vorlage verknüpften Informationen werden an das Projekt übertragen. Dazu gehören Aufgaben, Zuweisungen, Dauern, Dokumente, Finanzdetails, Risiken und benutzerdefinierte Formulare.

>[!TIP]
>
>Workfront definiert die Gruppe und den Status des neuen Projekts wie folgt:
>
>* Der Standardstatus eines neuen Projekts, das aus einer Vorlage erstellt wurde, entspricht dem Status, der von Ihrem Workfront-Administrator im Hauptbereich &quot;Projekteinstellungen&quot;oder von einem Gruppenadministrator (oder Workfront-Administrator) im Bereich &quot;Projekteinstellungen&quot;für eine Gruppe definiert wurde. Informationen zum Konfigurieren von Projektvoreinstellungen finden Sie unter [Systemweite Projektvoreinstellungen konfigurieren](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md) oder [Konfigurieren von Projektvoreinstellungen für eine Gruppe](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md).
>
>* Die Gruppe des neuen Projekts ist die Gruppe der Vorlage. Wenn die Vorlage nicht mit einer Gruppe verknüpft ist, ist die Gruppe des Projekts die Startseite des Benutzers, der das Projekt erstellt.
>
>* Die für ein neues Projekt verfügbaren Status stimmen mit den Status der Gruppe des Projekts überein, bei der es sich entweder um die Gruppe der Vorlage oder um die Home-Gruppe des Benutzers handelt, der das Projekt erstellt.

Sie haben die folgenden Optionen zum Erstellen eines Projekts aus einer Vorlage:

* Erstellen eines Projekts aus einer Vorlage im Bereich &quot;Projekte&quot;
* Erstellen eines Projekts aus einer Vorlage auf Vorlagenebene
* Eine Vorlage an ein vorhandenes Projekt anhängen

  Weitere Informationen finden Sie unter [Eine Vorlage an ein Projekt anhängen](../../../manage-work/projects/create-and-manage-templates/attach-template-to-project.md).

* Erstellen eines Projekts aus einer Vorlage im Bereich &quot;Gruppen&quot;

## Zugriffsanforderungen

<!--drafted for P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Workfront license*</td> 
   <td> <p>Current license: Standard </p>
   Or
   <p>Legacy license: Plan </p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects and to Templates</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information about access to projects, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md" class="MCXref xref">Grant access to projects</a>. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View permissions to a template</p> <p>When you create a project you automatically receive Manage permissions to the project </p> <p> For information about project permissions, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Share a project in Adobe Workfront</a>.</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Abo</td> 
   <td> <p>Alle </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Workfront-Lizenz</td> 
   <td> <p>Neu: Standard</p>
        <p>oder</p>
        <p>Aktuell: Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Zugriff auf Projekte und Vorlagen bearbeiten</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Berechtigungen für eine Vorlage anzeigen</p> <p>Wenn Sie ein Projekt erstellen, erhalten Sie automatisch Verwaltungsberechtigungen für das Projekt.</p></td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Erstellen eines Projekts aus einer Vorlage im Bereich &quot;Projekte&quot;

Sie können ein Projekt im Bereich Projekte im Hauptmenü oder im Bereich Projekte eines Portfolios oder Programms erstellen.

1. Führen Sie einen der folgenden Schritte aus:

   * Klicken Sie auf **[!UICONTROL Hauptmenü]** icon ![Hauptmenü](/help/_includes/assets/main-menu-icon.png) in der oberen rechten Ecke von Adobe Workfront oder (falls verfügbar) klicken Sie auf das **[!UICONTROL Hauptmenü]** icon ![Hauptmenü](/help/_includes/assets/main-menu-icon-left-nav.png) in der oberen linken Ecke. Klicks **Projekte**, dann erweitern **Neues Projekt**.
   * Wechseln Sie zu einem Portfolio und erweitern Sie **Neues Projekt**.

     >[!TIP]
     >
     >Wenn Sie ein Projekt mit einer Vorlage aus einem Portfolio erstellen, wird das Projektfeld des neuen Portfolios aktualisiert, um das Portfolio anzuzeigen, aus dem Sie das Projekt erstellen möchten. Dadurch wird das Feld Portfolio in der Vorlage überschrieben, sofern angegeben.

   * Öffnen Sie ein Programm und erweitern Sie **Neues Projekt**.

     >[!TIP]
     >
     >Wenn Sie ein Projekt mithilfe einer Vorlage aus einem Programm erstellen, wird das Programmfeld der neuen Projekte aktualisiert, um das Programm anzuzeigen, aus dem Sie das Projekt erstellen möchten. Das Feld Portfolio der Vorlage wird aktualisiert und zeigt das Portfolio des Programms an, aus dem Sie das Projekt erstellen möchten. Dadurch werden die Portfolio- und Programmfelder in der Vorlage überschrieben, sofern sie angegeben wurden.

   * Als Gruppenadministrator können Sie auch ein Projekt im Abschnitt &quot;Projekte&quot;einer von Ihnen verwalteten Gruppe erstellen. Weitere Informationen finden Sie unter [Erstellen und Ändern von Gruppenprojekten](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-projects.md).

     >[!TIP]
     >
     >Wenn Sie ein Projekt mit einer Vorlage aus einer Gruppe erstellen, wird die Gruppe, aus der Sie das Projekt erstellen, nur dann im Feld Gruppe des neuen Projekts angezeigt, wenn das Feld Gruppe der Vorlage nicht angegeben ist. Wenn das Vorlagengruppenfeld angegeben ist, ist das Gruppenfeld des neuen Projekts das des Vorlagenfelds.

   <!--
   <p>(this, above, is hyperlinked to the classic version of this article; the Milestone View steps are similar to creating a project in Classic than to the way you do it in NWE)</p>
   -->

   ![Neue Projektoptionen](assets/new-project-dropdown.png)

1. Klicken Sie auf den Namen einer Vorlage im **Favoritenvorlagen** Liste.

   ![Favoritenvorlage auswählen](assets/new-project-from-template-dropdown-with-template-favorites.png)

   Oder

   Gehen Sie wie folgt vor:

   1. Auswählen **Neues Projekt aus Vorlage**.
   1. Im **Suchvorlagen** eingeben, den Namen einer Vorlage eingeben und auf diese klicken, wenn sie in der Liste angezeigt wird.
   1. Überprüfen Sie die Vorlagendetails auf der rechten Seite.

      Die Vorlagendetails umfassen Folgendes:

      * Vorlagendauer
      * Vorlageninhaber
      * Die Anzahl der Aufgaben auf oberster Ebene, einschließlich der Namen der drei wichtigsten Aufgaben
      * Die Anzahl aller Aufgaben in der Vorlage
      * Die Namen der benutzerdefinierten Vorlagen-Formulare

   1. (Optional) Bewegen Sie den Mauszeiger im linken Bereich über den Namen einer Vorlage und klicken Sie auf **Favoriten** **icon** ![](assets/favorites-icon-small.png) , um ihn als Favoriten für die zukünftige Verwendung zu kennzeichnen.

      Oder

      Erweitern Sie die **Favoritenvorlagen** und wählen Sie eine Vorlage aus der Dropdownliste aus.

      >[!TIP]
      >
      >Sie können bis zu 40 Workfront-Elemente als Favoriten markieren. Dazu gehören Vorlagen und andere Elemente.

   1. Klicks **Vorlage verwenden** wenn Sie eine Vorlage ausgewählt haben.

      ![Vorlagendetails](assets/new-project-from-template-small-box-with-template-details-panel.png)

      >[!NOTE]
      >
      >Wenn Sie die Meilensteinansicht auf die Liste der Projekte angewendet haben, klicken Sie auf den Namen einer Vorlage in der **Neuer Bereich &quot;Vorlage&quot;**.
      >
      >
      >![Meilensteinansicht zum Erstellen eines Projekts aus einer Vorlage](assets/create-project-from-template-box-from-milestone-view-nwe-350x275.png)
      >

   Die **Neues Projekt** wird geöffnet.

   ![Neues Projekt](assets/new-project-from-template-box.png)

1. Wenn ein Feld bereits in der Vorlage ausgefüllt ist, wird das Feld im **Neues Projekt** ankreuzen. Sie können die vorausgefüllten Werte bearbeiten, um sie besser an Ihr Projekt anzupassen. Weitere Informationen finden Sie unter [Projekte bearbeiten](../../../manage-work/projects/manage-projects/edit-projects.md).
1. Klicks **Projekt erstellen**.

   Alle in der Vorlage definierten Details werden automatisch mit dem neu erstellten Projekt verknüpft, wenn Sie sie im vorherigen Schritt nicht geändert haben.

## Erstellen eines Projekts aus einer Vorlage im Bereich &quot;Vorlagen&quot;

Anstatt im Bereich &quot;Projekte&quot;zu beginnen, können Sie ein Projekt aus einer Vorlage erstellen, indem Sie mit der Vorlage beginnen.

{{step1-to-templates}}

1. Klicken Sie auf den Namen einer Vorlage, die Sie verwenden möchten.
1. Klicken Sie auf **Mehr** Menü ![](assets/more-icon.png)Klicken Sie auf **Projekt erstellen**.

   ![Projekt aus Vorlage erstellen](assets/project-sharing-on-template.png)

   Die **Neues Projekt** wird geöffnet.

1. Geben Sie einen Namen für das Projekt ein, überprüfen Sie dann jeden Abschnitt und nehmen Sie die erforderlichen Änderungen vor.

   ![Neues Projekt](assets/new-project-from-template-box.png)

   Wenn ein Feld bereits in der Vorlage ausgefüllt ist, wird das Feld im **Neues Projekt** ankreuzen. Sie können die vorausgefüllten Werte bearbeiten, um sie besser an Ihr Projekt anzupassen. Weitere Informationen finden Sie unter [Projekte bearbeiten](../../../manage-work/projects/manage-projects/edit-projects.md).

1. Klicks **Projekt erstellen**.

   Alle in der Vorlage definierten Details werden automatisch mit dem neu erstellten Projekt verknüpft, wenn Sie sie im vorherigen Schritt nicht geändert haben.
