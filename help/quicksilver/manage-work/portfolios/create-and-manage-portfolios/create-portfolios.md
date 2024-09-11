---
product-area: portfolios
navigation-topic: create-and-manage-portfolios
title: Erstellen von Portfolios
description: Ein Portfolio ist eine Sammlung von Projekten, die für dieselben Ressourcen, Budgets und Zeitpläne konkurrieren. Die Projekte in einem Portfolio sind so ähnlich, dass sie denselben Ressourcenpool verwenden und mit derselben Scorecard gemessen werden.
author: Alina
feature: Work Management, Strategic Planning
exl-id: fdaed68d-d9cc-4514-8f80-b169cdd739bd
source-git-commit: 2bfb6d03f3d0f792180a67ade8a704e4c899a671
workflow-type: tm+mt
source-wordcount: '668'
ht-degree: 1%

---

# Erstellen von Portfolios

<!--Audited: 7/2024-->

Ein Portfolio ist eine Sammlung von Projekten, die für dieselben Ressourcen, Budgets und Zeitpläne konkurrieren. Die Projekte in einem Portfolio sind so ähnlich, dass sie denselben Ressourcenpool verwenden und mit derselben Scorecard gemessen werden.

Sie können Portfolios verwenden, um Projekte zu gruppieren, die zu denselben Produktlinien, Geschäftsbereichen, Abteilungen, Unternehmen oder anderen Geschäftsbereichen gehören.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>Alle</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td> <p>Neu: [!UICONTROL Standard]</p>
   <p>Aktuell:[!UICONTROL Plan] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>[!UICONTROL] Zugriff auf Portfolios bearbeiten</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Nachdem Sie ein Portfolio erstellt haben, verfügen Sie standardmäßig über Verwaltungsberechtigungen</p>  </td> 
  </tr> 
 </tbody> 
</table>

*Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Möglichkeiten zum Erstellen von Portfolios

Sie können Portfolios in Workfront mit einer der folgenden Methoden erstellen:

* Erstellen Sie ein neues Portfolio, das im Bereich Portfolios des Hauptmenüs beginnt. In diesem Artikel wird beschrieben, wie Sie ein neues Portfolio erstellen können.

* Importieren Sie ein Portfolio mit Kick-Start.

  Als Workfront-Administrator können Sie Portfolios mit einem Kick-Start importieren.

  Informationen zum Importieren von Daten mithilfe von Kick-Start-Schritten in Workfront finden Sie unter [Importieren von Daten in Adobe Workfront mithilfe einer Kick-Start-Vorlage](/help/quicksilver/administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md).

* Fügen Sie Portfolios hinzu, während Sie sie aus einem Datensatztyp in der Workfront-Planung verbinden.

  Sie benötigen eine neue Workfront-Lizenz und eine zusätzliche Workfront Planning-Lizenz für Workfront Planning.

  Informationen zum Zugriff auf die Workfront-Planung finden Sie unter [Zugriffsübersicht](/help/quicksilver/planning/access/access-overview.md).

  Informationen zum Erstellen von Portfolios durch Hinzufügen zu Datensätzen finden Sie im Abschnitt &quot;Erstellen von Datensätzen während der Verbindung mit ihnen&quot; im Artikel [Erstellen von Datensätzen](/help/quicksilver/planning/records/create-records.md).


## Erstellen von Portfolios

{{step1-click-main-menu}}

1. Klicken Sie auf **[!UICONTROL Portfolio]**.
1. Klicken Sie auf **[!UICONTROL Neues Portfolio]**.
1. Ersetzen Sie **[!UICONTROL Unbenanntes Portfolio]** durch den Namen, den Sie für das Portfolio benötigen.

   Der Name kann bis zu 255 Zeichen enthalten.

1. (Optional) Klicken Sie in der Kopfzeile am oberen Seitenrand auf den Portfolio-Manager unter **[!UICONTROL 1} , um einen anderen Portfoliomanager zuzuweisen.]**

   ![](assets/portfolio-manager-name-350x51.jpg)

   Als Ersteller des Portfolios werden Sie standardmäßig als Portfolioverwalter zugewiesen.

1. Klicken Sie im linken Bereich auf **[!UICONTROL Portfolio Details]** .
1. Ändern Sie im Bereich **[!UICONTROL Überblick]** eine der folgenden Informationen:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Beschreibung]</td> 
      <td> <p>Geben Sie eine Beschreibung für das Portfolio ein, um anzugeben, was eindeutig ist. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Portfolio Manager]</td> 
      <td> <p>Beginnen Sie mit der Eingabe des Namens eines Benutzers, den Sie als Portfolio-Manager angeben möchten, und wählen Sie ihn aus, wenn er in der Liste angezeigt wird. Dies entspricht dem [!UICONTROL Portfolio Owner]. Diese Person kann die in den Projekten des Portfolios definierten Arbeiten überwachen und den Geschäftsfall genehmigen.</p> <p>Wichtig: Wenn Sie jemanden als [!UICONTROL Portfolio Manager] festlegen, erhält er automatisch [!UICONTROL Manager]-Berechtigungen für das Portfolio, die Programme und die  im Portfolio. </p> <p>Tipp: Sie können auch den [!UICONTROL Portfolio Manager] in der Kopfzeile oben auf der Seite aktualisieren.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Gruppe </td> 
      <td> <p>Fügen Sie den Namen einer einzelnen Gruppe hinzu, wenn die Gruppe Eigentümer des Portfolios ist oder für dessen Abschluss verantwortlich ist. </p> <p>Sie können sicherstellen, dass Sie die richtige Gruppe auswählen, indem Sie den Mauszeiger darüber bewegen und auf das [!UICONTROL Informationssymbol] <img src="assets/info-icon.png"> klicken, das daneben angezeigt wird. Dadurch wird eine QuickInfo mit Informationen zur Gruppe angezeigt, z. B. die Hierarchie der Gruppen darüber und deren Administratoren.</p> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <img src="assets/group-details-widget-portfolios-350x250.png" style="width: 350;height: 250;"> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Optional) Klicken Sie in das Feld **[!UICONTROL Benutzerdefiniertes Formular hinzufügen]** oben rechts auf der Seite [!UICONTROL Portfolio-Details] , um ein benutzerdefiniertes Formular für das Portfolio auszuwählen und die benutzerdefinierten Felder zu aktualisieren.

   >[!TIP]
   >
   >Sie müssen bereits benutzerdefinierte Portfolio-Formulare erstellt haben, bevor Sie sie an Portfolios anhängen können.

1. Klicken Sie auf **[!UICONTROL Änderungen speichern]**.
1. (Optional) Klicken Sie im linken Bereich auf **[!UICONTROL Programme]** und dann auf **[!UICONTROL Programme hinzufügen]** , um dem Portfolio Programme hinzuzufügen.

   Weitere Informationen zum Erstellen von Programmen finden Sie unter [Programm erstellen](../../../manage-work/portfolios/create-and-manage-programs/create-program.md).

1. (Optional) Klicken Sie im linken Bereich auf **[!UICONTROL Projekte]** und dann auf **[!UICONTROL Projekte hinzufügen]** , um Projekte zum Portfolio hinzuzufügen.

   Weitere Informationen zum Hinzufügen von Projekten zu einem Portfolio finden Sie unter [Hinzufügen von Projekten zu einem Portfolio](../../../manage-work/portfolios/create-and-manage-portfolios/add-projects-to-portfolios.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Deactivate a portfolio</h2>
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: drafted this and moved it to their own article: delete-deactivate-portfolios)</p>
<p>When you deactivate a portfolio, you can still access it from the Portfolios area, but it no longer displays in the list of portfolios when users try to add it to a project.</p>
<ol>
<li value="1">Click the <strong>Main Menu</strong> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of Adobe Workfront.</li>
<li value="2">Click <strong>Portfolios</strong> .</li>
<li value="3"> <p>Click the name of the portfolio.</p> </li>
<li value="4" data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the More menu <img src="assets/more-icon.png"> to the right of the portfolio name, then click <strong>Deactivate Portfolio</strong>.</li>
</ol>
<h2>Delete a portfolio</h2>
<ol>
<li value="1">Click the <strong>Main Menu</strong> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of Adobe Workfront.</li>
<li value="2"> <p>Click <strong>Portfolios</strong> .</p> </li>
<li value="3"> <p>Select the portfolio, then click the Delete icon <img src="assets/delete.png">.</p> </li>
<li value="4"> <p>In the box that appears, click <strong>Yes, Delete It</strong> to confirm.</p> </li>
</ol>
</div>
-->
