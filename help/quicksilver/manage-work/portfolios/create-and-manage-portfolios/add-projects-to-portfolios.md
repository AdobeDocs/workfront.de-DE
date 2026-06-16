---
product-area: portfolios;projects
navigation-topic: create-and-manage-portfolios
title: Hinzufügen von Projekten zu einer Portfolio
description: Es wird empfohlen, Projekte zu Portfolios hinzuzufügen, wenn Sie sie initiieren. Sie können sie jedoch jederzeit während ihres Lebenszyklus zu einem Portfolio hinzufügen.
author: Alina
feature: Work Management, Strategic Planning
exl-id: 97f36c18-3ac8-45ac-b5bc-dfe8b1363faf
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/UkUQdW12tLqRjh5zmbwtjNfRxFwc-Uhj2gGwjmDyKb8
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2:
  - id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: bce87dde-a4ab-44c9-8a18-ad66e4ddb377
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 397e5e36632872bb7be3f4e219b36e33b44136e9
workflow-type: tm+mt
source-wordcount: 674
ht-degree: 3%

---

# Hinzufügen von Projekten zu einem Portfolio

<!--Audited: 08/2025-->

<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. The same features will also be available in the Production environment for all customers after a week from the Preview release. </span>   

<span class="preview">For more information, see [Interface modernization](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md). </span>
-->

Es wird empfohlen, Projekte zu Portfolios hinzuzufügen, wenn Sie sie initiieren. Sie können sie jedoch jederzeit während ihres Lebenszyklus zu einem Portfolio hinzufügen.

Beachten Sie beim Hinzufügen von Projekten zu Portfolios Folgendes:

* Sie können nur ein Portfolio mit einem Projekt verknüpfen.
* Ein Projekt verbleibt in einem Portfolio, bis es entfernt oder mit einem anderen Portfolio verknüpft wird.
* Ein Portfolio kann eine unbegrenzte Anzahl von Projekten enthalten.

>[!CAUTION]
>
>Vererbte Berechtigungen werden möglicherweise nicht korrekt angewendet, wenn sie für eine große Anzahl untergeordneter Objekte verwendet werden.
>   
>Um Probleme mit geerbten Berechtigungen zu vermeiden, empfehlen wir Folgendes:
>
>* Begrenzen Sie die Anzahl der untergeordneten Objekte (Projekte) unter einem einzelnen übergeordneten Element (Portfolio oder Programm). Pro Portfolio oder Programm empfehlen wir nicht mehr als 10.000 Projekte.
>
>* Verringern der Vererbungstiefe durch Anwenden von Berechtigungen auf ein Objekt auf niedrigerer Ebene.
>
>  Wenden Sie beispielsweise Berechtigungen direkt auf Projektebene an, anstatt sich auf die vom Portfolio geerbten Berechtigungen für das Programm und dann für das Projekt zu verlassen.
>
>* Teilen Sie Programme auf, um weniger Projekte zu enthalten, was die Komplexität der Berechtigungen verringert.
>


## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Packstück</td> 
   <td> <p>Beliebig</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Lizenz</td> 
   <td><p>Standard</p> 
   <p>[!UICONTROL Plan] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfiguration der Zugriffsebene</td> 
   <td> <p>[!UICONTROL Bearbeiten] Zugriff auf Portfolios</p> <p>[!UICONTROL Bearbeiten] Zugriff auf Projekte</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>[!UICONTROL Manage]-Berechtigungen für das Portfolio</p> <p>[!UICONTROL Manage]-Berechtigungen für die Projekte</p>  </td> 
  </tr> 
 </tbody> 
</table>

*Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--
Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td> <p>Any</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td><p>New: Standard</p> 
   <p>Current: [!UICONTROL Plan] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level</td> 
   <td> <p>[!UICONTROL Edit] access Portfolios</p> <p>[!UICONTROL Edit] access to Projects</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>[!UICONTROL Manage] permissions to the portfolio</p> <p>[!UICONTROL Manage] permissions to the projects</p>  </td> 
  </tr> 
 </tbody> 
</table>
-->

## Hinzufügen eines Projekts zu einem Portfolio

1. Gehen Sie zu einem Portfolio und klicken Sie **[!UICONTROL linken Bereich]** Projekte“.

   ![Portfolio mit Projekten](assets/qs-portfolio-with-projects-350x90.png)

1. Klicken Sie **[!UICONTROL Neues Projekt]** und wählen Sie eine Methode zum Hinzufügen eines Projekts aus.

   >[!TIP]
   >
   >Sie können kein Projekt hinzufügen, wenn Sie die Liste der Projekte in der Ansicht &quot;[!UICONTROL &quot; &#x200B;].

   Wählen Sie aus den folgenden Optionen aus:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody>

   <tr> 
      <td role="rowheader">[!UICONTROL Neues Projekt]</td> 
      <td> <p>Ein neues Projekt hinzufügen. </p> <p>Weitere Informationen zum Erstellen eines Projekts finden Sie unter <a href="../../../manage-work/projects/create-projects/create-project.md" class="MCXref xref">Erstellen eines Projekts</a>. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Neues Projekt (Legacy-Speicher)]</td> 
      <td> <p>Fügen Sie ein neues Workfront-Speicherprojekt hinzu. </p>
      <p>Die Option wird nur angezeigt, wenn Ihr Unternehmen sowohl Workfront als auch Adobe Cloud Document Storage verwendet. Ihre Workfront-Instanz verfügt möglicherweise nicht über beide Speichertypen.</p>
       <p>Weitere Informationen zum Erstellen eines Projekts finden Sie unter <a href="../../../manage-work/projects/create-projects/create-project.md" class="MCXref xref">Erstellen eines Projekts</a>. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Neues Projekt aus Vorlage]</td> 
      <td> <p>Ein neues Projekt mithilfe einer vorhandenen Vorlage hinzufügen. </p> <p>Weitere Informationen zum Erstellen eines Projekts über eine Vorlage finden Sie unter <a href="../../../manage-work/projects/create-projects/create-project-from-template.md" class="MCXref xref">Erstellen eines Projekts über eine Vorlage</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Import [!DNL MS Project]] </td> 
      <td> <p>Fügen Sie ein Projekt hinzu, das Sie zuvor aus [!DNL MS Project] exportiert und auf Ihrem Computer gespeichert haben. </p> <p>Weitere Informationen zum Erstellen eines neuen Projekts durch Importieren aus [!DNL Microsoft Project] finden Sie unter <a href="../../../manage-work/projects/create-projects/import-project-from-ms-project.md" class="MCXref xref">Projekt aus [!DNL Microsoft Project]</a> importieren.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL -Anforderungsprojekt]</td> 
      <td> <p>Fordern Sie die Genehmigung eines Projekts an.</p> <p>Informationen zum Anfordern von Projekten finden Sie unter <a href="../../../manage-work/projects/create-projects/request-project.md">Anfordern eines Projekts</a>. </p> </td> 
     </tr> 
          <tr> 
      <td role="rowheader">[!UICONTROL Vorhandenes Projekt]</td> 
      <td> <p>Ein bereits erstelltes Projekt hinzufügen.</p> </td> 
     </tr>
    </tbody> 
   </table>

   <!-- update screen shot for both kinds of storages??-->

   ![Dropdown-Liste „Neues Projekt“](assets/new-project-dropdown-expanded-from-portfolio-nwe-350x376.png)

1. (Bedingt) Wenn Sie ein vorhandenes Projekt hinzufügen möchten, wird das Feld **Projekte hinzufügen** geöffnet. <!--check this after UI changes-->

   ![Vorhandenes Projekt hinzufügen](assets/add-existing-projects-to-portfolios-box.png) <!--check this after UI changes-->

1. Geben Sie den Namen eines Projekts in das Feld **[!UICONTROL Projekte zu diesem Portfolio hinzufügen]** ein und klicken Sie darauf, wenn sie in der Liste angezeigt werden.  <!--check this after UI changes-->

   Sie können mehr als ein Projekt hinzufügen.

   >[!NOTE]
   >
   >Wenn Ihr Unternehmen sowohl den veralteten Workfront- als auch den Adobe-Cloud-Speicher für Dokumente verwendet, gibt es die folgenden Szenarien:
   >
   >
   >* Sie können kein Legacy-Speicherprojekt zu einem Adobe Cloud-Speicherportfolio hinzufügen oder ein Adobe Cloud-Speicherprojekt zu einem Legacy-Speicherportfolio hinzufügen.
   >* Sie können kein Projekt aus einer Adobe Cloud-Speichervorlage in einem Legacy-Speicherportfolio erstellen.
   >* Sie können ein Projekt aus einer Legacy-Speichervorlage in einem Adobe Cloud-Speicherportfolio erstellen, die Dokumente und Ordner in der Vorlage werden jedoch nicht zum neuen Projekt hinzugefügt. Das Projekt erhält Adobe Cloud-Speicher.
   >
   >Weitere Informationen finden Sie unter [Übersicht über das Dokumentenmanagement für Projekte und verwandte Objekte](/help/quicksilver/manage-work/projects/manage-projects/manage-documents-on-projects.md).
   >
   >Nicht alle Workfront-Instanzen verfügen über beide Arten von Dokumentspeichern.


1. (Optional) Klicken Sie auf das **X**-Symbol rechts neben dem Projektnamen, um es aus der Liste zu entfernen, wenn Sie es nicht zum Portfolio hinzufügen möchten.

   <!--replace last step with this, for unshim: 1. (Optional) Click the **Delete** icon ![Delete icon](assets/delete-icon.png) next to the name of a project if you decide not to add it to the portfolio.-->

1. Klicken Sie **[!UICONTROL Projekte hinzufügen]**. <!--check this after UI changes-->

   Das bzw. die ausgewählte(n) Projekt(e) sind nun mit dem Portfolio verknüpft.
