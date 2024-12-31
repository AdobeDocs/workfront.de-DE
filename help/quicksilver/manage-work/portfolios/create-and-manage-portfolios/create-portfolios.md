---
product-area: portfolios
navigation-topic: create-and-manage-portfolios
title: Erstellen von Portfolios
description: Ein Portfolio ist eine Zusammenstellung von Projekten, die um dieselben Ressourcen, Budgets und Zeitpläne konkurrieren. Die Projekte in einem Portfolio sind so ähnlich, dass sie denselben Ressourcenpool verwenden und mit derselben Scorecard gemessen werden würden.
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

Ein Portfolio ist eine Zusammenstellung von Projekten, die um dieselben Ressourcen, Budgets und Zeitpläne konkurrieren. Die Projekte in einem Portfolio sind so ähnlich, dass sie denselben Ressourcenpool verwenden und mit derselben Scorecard gemessen werden würden.

Sie können Portfolios verwenden, um Projekte zu gruppieren, die zu denselben Produktlinien, Geschäftsbereichen, Abteilungen, Unternehmen oder anderen Geschäftsbereichen gehören.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Plan*</td> 
   <td> <p>Beliebig</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Lizenz*</td> 
   <td> <p>Neu: [!UICONTROL Standard]</p>
   <p>Aktuell:[!UICONTROL Plan] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>[!UICONTROL Bearbeiten] Zugriff auf Portfolios</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Nachdem Sie ein Portfolio erstellt haben, haben Sie standardmäßig Verwaltungsberechtigungen dafür</p>  </td> 
  </tr> 
 </tbody> 
</table>

*Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Möglichkeiten zum Erstellen von Portfolios

Sie können Portfolios in Workfront mit einer der folgenden Methoden erstellen:

* Erstellen Sie ein Portfolio von Grund auf neu, beginnend im Bereich Portfolios des Hauptmenüs. Dieser Artikel beschreibt, wie Sie ein Portfolio von Grund auf neu erstellen können.

* Importieren Sie ein Portfolio mithilfe von Kickstarts.

  Als Workfront-Administrator können Sie Portfolios über einen Kickstart importieren.

  Informationen zum Importieren von Daten mithilfe von Kickstarts in Workfront finden Sie unter [Importieren von Daten in Adobe Workfront mithilfe einer Kickstart-Vorlage](/help/quicksilver/administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md).

* Portfolios hinzufügen, während Sie sie mit einem Datensatztyp in Workfront Planning verbinden.

  Sie müssen über eine neue Workfront-Lizenz und eine zusätzliche Workfront Planning-Lizenz für Workfront Planning verfügen.

  Informationen zum Zugriff auf Workfront Planning finden Sie unter [Zugriffsübersicht](/help/quicksilver/planning/access/access-overview.md).

  Informationen zum Erstellen von Portfolios durch Hinzufügen zu Datensätzen finden Sie im Abschnitt „Erstellen von Datensätzen, während Sie sie verbinden“ im Artikel [Erstellen von Datensätzen](/help/quicksilver/planning/records/create-records.md).


## Erstellen von Portfolios

{{step1-click-main-menu}}

1. Klicken Sie auf **[!UICONTROL Portfolios]**.
1. Klicken Sie auf **[!UICONTROL Neues Portfolio]**.
1. Ersetzen **[!UICONTROL Nicht benanntes Portfolio]** durch den Namen, den Sie für das Portfolio verwenden möchten.

   Der Name kann bis zu 255 Zeichen lang sein.

1. (Optional) Klicken Sie oben auf der Portfolio-]**auf den Namen unter**[!UICONTROL  Portfoliomanager, um einen anderen Portfoliomanager zuzuweisen.

   ![](assets/portfolio-manager-name-350x51.jpg)

   Als Ersteller des Portfolios werden Sie standardmäßig als Portfolio-Manager zugewiesen.

1. Klicken Sie im linken Bereich ]****[!UICONTROL  Portfolio-Details.
1. Ändern Sie **[!UICONTROL Bereich]**&#x200B;Übersicht“ eine der folgenden Informationen:

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
      <td> <p>Geben Sie den Namen eines Benutzers ein, den Sie als Portfolio-Manager angeben möchten, und wählen Sie ihn aus, wenn er in der Liste angezeigt wird. Dies ist dasselbe wie der [!UICONTROL Portfolio Owner]. Dies ist die Person, die die in den Projekten des Portfolios definierten Arbeiten überwachen und den Business Case genehmigen kann.</p> <p>Wichtig: Wenn Sie jemanden als [!UICONTROL Portfolio Manager] festlegen, erhält er automatisch [!UICONTROL Manage]-Berechtigungen für das Portfolio, die Programme und die Projekte im Portfolio. </p> <p>Tipp: Sie können den [!UICONTROL Portfolio Manager] auch in der Kopfzeile oben auf der Seite aktualisieren.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Gruppe </td> 
      <td> <p>Fügen Sie den Namen einer einzelnen Gruppe hinzu, wenn die Gruppe Eigentümer des Portfolios ist oder für dessen Fertigstellung verantwortlich ist. </p> <p>Sie können sicherstellen, dass Sie die richtige Gruppe auswählen, indem Sie den Mauszeiger darüber bewegen und auf das <img src="assets/info-icon.png"> [!UICONTROL information] klicken, das neben der Gruppe angezeigt wird. Dadurch wird eine QuickInfo angezeigt, die Informationen über die Gruppe auflistet, wie z. B. die Hierarchie der darüber liegenden Gruppen und deren Administratoren.</p> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <img src="assets/group-details-widget-portfolios-350x250.png" style="width: 350;height: 250;"> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Optional) Klicken Sie in das Feld **[!UICONTROL Benutzerdefiniertes Formular hinzufügen]** oben rechts auf der Seite [!UICONTROL Portfoliodetails], um ein benutzerdefiniertes Formular für das Portfolio auszuwählen und die benutzerdefinierten Felder zu aktualisieren.

   >[!TIP]
   >
   >Benutzerdefinierte Portfolioformulare müssen bereits erstellt worden sein, bevor Sie sie Portfolios anhängen können.

1. Klicken Sie auf **[!UICONTROL Änderungen speichern]**.
1. (Optional) Klicken Sie **[!UICONTROL linken]** auf „Programme“ und dann auf **[!UICONTROL Programme hinzufügen]**, um dem Portfolio Programme hinzuzufügen.

   Weitere Informationen zum Erstellen von Programmen finden Sie unter [Erstellen eines Programms](../../../manage-work/portfolios/create-and-manage-programs/create-program.md).

1. (Optional) Klicken Sie **[!UICONTROL linken Bereich]** Projekte) und dann auf **[!UICONTROL Projekte hinzufügen]**, um Projekte zum Portfolio hinzuzufügen.

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
