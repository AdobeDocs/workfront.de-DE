---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: organization-setup
title: Erstellen und Verwalten von Aufgabengebieten
description: Als  [!DNL Adobe Workfront]  oder Benutzer mit administrativem Zugriff auf Aufgabengebiete können Sie Aufgabengebiete erstellen, die Benutzern zugewiesen werden können, und Standardaufgabengebiete löschen, die für Ihr Unternehmen nicht relevant sind.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 664fb2fe-ff7e-4807-9a43-b37e7d5d57eb
source-git-commit: 15063d937a5ba9b5285c66a0987e8deea6cc6d74
workflow-type: tm+mt
source-wordcount: '1139'
ht-degree: 0%

---

# Erstellen und Verwalten von Aufgabengebieten

<!-- Audited: 1/2024 -->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

Als [!DNL Adobe Workfront] oder Benutzer mit administrativem Zugriff auf Aufgabengebiete können Sie Aufgabengebiete erstellen, die Benutzern zugewiesen werden können, und Standardaufgabengebiete löschen, die für Ihr Unternehmen nicht relevant sind. Informationen zum administrativen Zugriff in [!DNL Workfront] finden Sie unter [Gewähren von administrativem Zugriff für Benutzer auf bestimmte Bereiche](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] Packstück</td> 
   <td><p>Beliebig</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] Lizenz</td> 
   <td><p>[!UICONTROL Standard]</p>
       <p>[!UICONTROL-Plan]</p></td>
  </tr> 
  <tr> 
   <td>Konfigurationen der Zugriffsebene</td> 
   <td>Administrativer Zugriff auf Aufgabengebiete</td>
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Erstellen eines Aufgabengebiets

So erstellen Sie ein Aufgabengebiet:

{{step-1-to-setup}}

1. Klicken Sie im linken Bedienfeld auf &#x200B;**[!UICONTROL Aufgabengebiete].**
1. Klicken Sie **[!UICONTROL Neues Aufgabengebiet].**
1. Konfigurieren Sie Folgendes:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Name]</td> 
      <td> <p>Geben Sie einen Namen für das Aufgabengebiet an. Dieser Name wird überall in [!DNL Workfront] angezeigt, wo das Feld [!UICONTROL Aufgabengebiet] angezeigt wird. </p> <p>Tipp: Der Name eines Aufgabengebiets kann bis zu 255 Zeichen lang sein. Längere Namen können jedoch in bestimmten Bereichen von [!DNL Workfront] abgeschnitten werden. </p> </td> 
     </tr>
     <tr> 
      <td role="rowheader">[!UICONTROL Beschreibung]</td> 
      <td>Geben Sie eine Beschreibung für die Rolle ein, die angibt, was eindeutig ist. </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL ist aktiv]</span> </td> 
      <td> 
       <ul> 
        <li> <p>Wählen Sie <b>[!UICONTROL Yes]</b>, wenn die Rolle überall aktiv und verfügbar sein soll, [!DNL Workfront] sie mit Benutzern, Arbeitselementen usw. verknüpft werden soll. </p> </li> 
        <li> <p>Wählen Sie <b>[!UICONTROL No]</b> aus, wenn Sie möchten, dass die Rolle deaktiviert wird und nicht für die Zuweisung an Benutzer, Arbeitselemente usw. verfügbar ist. </p> </li> 
       </ul> <p><span>Informationen zur Deaktivierung von Aufgabengebieten finden Sie unter</span> <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/deactivate-job-roles.md" class="MCXref xref">Deaktivieren von Aufgabengebieten</a>. </p> </td> 
     </tr>
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL Basiswährung]</span> </td> 
      <td> <p><span>Dies ist die [!UICONTROL Basiswährung], wie von Ihrem Workfront-Administrator im Bereich [!UICONTROL Setup] festgelegt. Weitere Informationen finden </span> unter <a href="../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md" class="MCXref xref">Einrichten von Wechselkursen</a> .</p> <p>Tipp: <span>Sie können die [!UICONTROL Basiswährung] nicht auf Aufgabengebiet-Ebene bearbeiten. Dieses Feld ist abgeblendet und dient als Erinnerung daran, was die Basiswährung für Ihr System ist.</span> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Kostensatz]</td> 
      <td><p>Dies ist der Stundensatz (Cost per Hour Rate) des Aufgabengebiets. Dieser Wert berechnet die geplanten Kosten und Istkosten für Aufgaben und Probleme im Zusammenhang mit der Funktion sowie letztendlich die geplanten Kosten und Istkosten der Projekte. Geben Sie den Kurs mithilfe der [!UICONTROL Basiswährung] ein.</p> 
      <p>Klicken Sie auf <strong>[!UICONTROL Tarif hinzufügen]</strong>, um die gültigen Kostensätze anzuzeigen. Geben Sie den Wert der Kosten/Stunde für den Zeitraum ein und weisen Sie nach Bedarf ein [!UICONTROL Startdatum] und ein [!UICONTROL Enddatum] zu. Der erste Kostensatz hat kein Startdatum und der letzte Kostensatz hat kein Enddatum.</p> <p>Einige Daten werden automatisch hinzugefügt. Wenn beispielsweise der erste Kostensatz kein Enddatum hat und Sie einen zweiten Kostensatz mit dem Startdatum 1. Mai 2023 hinzufügen, wird dem ersten Kostensatz das Enddatum 30. April 2023 hinzugefügt, damit keine Lücken entstehen.</p> <p>Tipp: Beim Bearbeiten eines vorhandenen Aufgabengebiets können Sie <strong>Sortieren nach Startdatum</strong> auswählen, um das neueste Startdatum oben in der Tarifliste anzuzeigen.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Abrechnungssatz] </td> 
      <td><p>Dies ist der Abrechnungssatz pro Stunde für das Aufgabengebiet. Dieser Wert berechnet die geplanten und tatsächlichen Einnahmen aus Aufgaben und Problemen im Zusammenhang mit der Rolle sowie letztendlich die geplanten und tatsächlichen Einnahmen der Projekte. Geben Sie den Kurs mithilfe der [!UICONTROL Basiswährung] ein.</p> <p>Klicken Sie auf <strong>[!UICONTROL Abrechnungssatz hinzufügen]</strong>, um das Datum der Abrechnungssätze anzuzeigen. Geben Sie den Wert der Abrechnung/Stunde für den Zeitraum ein und weisen Sie nach Bedarf ein [!UICONTROL Startdatum] und ein [!UICONTROL Enddatum] zu. Der erste Abrechnungssatz hat kein Startdatum und der letzte Abrechnungssatz hat kein Enddatum.</p> <p>Einige Daten werden automatisch hinzugefügt. Wenn beispielsweise der erste Abrechnungssatz kein Enddatum hat und Sie einen zweiten mit dem Startdatum 1. Mai 2023 hinzufügen, wird dem ersten Abrechnungssatz das Enddatum 30. April 2023 hinzugefügt, sodass keine Lücken bestehen.</p> <p>Tipp: Beim Bearbeiten eines vorhandenen Aufgabengebiets können Sie <strong>Sortieren nach Startdatum</strong> auswählen, um das neueste Startdatum oben in der Tarifliste anzuzeigen.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL Währung überschreiben]</span> </td> 
      <td>
        <p>Wählen Sie eine Währung aus, die mit diesem Aufgabengebiet verknüpft ist. Dies ist die Währung, die [!DNL Workfront] für die Berechnung der Kosten und Einnahmen im Zusammenhang mit diesem Aufgabengebiet verwendet. </p> 
        <p><span>Diese Währung unterscheidet sich von der [!UICONTROL Basiswährung], die von Ihrem [!DNL Workfront] im Bereich [!UICONTROL Setup] eingerichtet wurde, und kann sich von der Währung unterscheiden, die einem Projekt zugeordnet ist.</span> </p> 
        <p>Tipp: In diesem Feld sind nur Währungen verfügbar, die im Bereich [!UICONTROL Wechselkurse] in Ihrem System verfügbar sind. Wenn Sie nur eine Währung eingerichtet haben, wird dieses Feld nicht angezeigt.</p> 
       <p><span>Informationen zum Einrichten der [!UICONTROL Basiswährung] in [!DNL Workfront] finden Sie </span><a href="../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md" class="MCXref xref">Einrichten von Wechselkursen</a>.</p> <p><span>Informationen zum Ändern der Währung eines Projekts finden Sie unter </span>Ändern <a href="../../../manage-work/projects/project-finances/change-project-currency.md" class="MCXref xref"> Projektwährung</a>.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL Währungskostensatz überschreiben]</span> </td> 
      <td>
        <p>Dies ist der Stundensatz des Aufgabengebiets unter Verwendung der ausgewählten [!UICONTROL Überschreibungswährung]. [!DNL Workfront] verwendet diesen Wert, um die geplanten und tatsächlichen Kosten von Aufgaben und Problemen im Zusammenhang mit dem Aufgabengebiet zu berechnen. </p> 
        <p><span>Geben Sie den Kurs in die oben angegebene [!UICONTROL Überschreibungswährung] ein. Dadurch wird auch der Kostensatz für dieses Aufgabengebiet aktualisiert, wenn die [!UICONTROL Basiswährung] verwendet wird.</span> </p> 
        <p>Weitere Informationen zur Kostenberechnung durch [!DNL Workfront] finden Sie unter <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Kosten nachverfolgen</a>.</p> 
       <p>Tipp: Beim Aktualisieren eines vorhandenen Aufgabengebiets, dem bereits ein Kostensatz zugeordnet ist, berechnet [!DNL Workfront] den Kurs [!UICONTROL Währung überschreiben] auf der Grundlage des Konversionssatzes in Ihrem System. Wenn Sie den Kostensatz für die Währung [!UICONTROL Überschreiben] aktualisieren, wird auch der Kostensatz des Aufgabengebiets automatisch aktualisiert.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL Überschreiben Währung Abrechnungssatz]</span> </td> 
      <td>
        <p>Dies ist der Abrechnungssatz pro Stunde für das Aufgabengebiet unter Verwendung der ausgewählten [!UICONTROL Überschreibungswährung]. [!DNL Workfront] verwendet diesen Wert, um den geplanten und tatsächlichen Umsatz von Aufgaben und Problemen im Zusammenhang mit dem Aufgabengebiet zu berechnen. </p>
        <p><span>Geben Sie den Kurs in die oben angegebene [!UICONTROL Überschreibungswährung] ein. Dadurch wird auch der Abrechnungssatz für dieses Aufgabengebiet aktualisiert, wenn die [!UICONTROL Basiswährung] verwendet wird.</span> </p>
        <p>Weitere Informationen zur Berechnung des Umsatzes durch [!DNL Workfront] finden Sie unter <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">Übersicht über Abrechnung und Umsatz</a>.</p>
        <p>Tipp: Beim Aktualisieren eines vorhandenen Aufgabengebiets, dem bereits ein Abrechnungssatz zugeordnet ist, berechnet [!DNL Workfront] den Wechselkurs zum Überschreiben der Währung anhand des Konversionssatzes in Ihrem System. Wenn Sie den Abrechnungssatz Währung überschreiben aktualisieren, wird auch der Abrechnungssatz des Aufgabengebiets automatisch aktualisiert. </p>
       </td>
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >Aufgabengebiete sind ein integraler Bestandteil der Verwaltung von Ressourcen. Um die Ressourcenplanungs-Tools verwenden zu können, müssen den Aufgabengebieten Kosten und Abrechnungssätze zugeordnet sein. Weitere Informationen finden Sie [Erste Schritte mit der Ressourcenverwaltung](../../../resource-mgmt/resource-mgmt-overview/get-started-resource-management.md).

1. Klicken Sie **[!UICONTROL Aufgabengebiet erstellen]**. Das Aufgabengebiet kann jetzt Aufgaben, Problemen, Genehmigungen zugewiesen werden oder Sie können Layout-Vorlagen oder andere Objekte für das Aufgabengebiet freigeben. Informationen zu allen Verwendungen von Aufgabengebieten in [!DNL Workfront] finden Sie unter [Aufgabengebiet - Übersicht](../../../administration-and-setup/set-up-workfront/organizational-setup/job-role-overview.md). Informationen zum Löschen eines Aufgabengebiets finden Sie unter [Aufgabengebiet löschen](../../../administration-and-setup/set-up-workfront/organizational-setup/delete-job-roles.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Delete a job role</h2>
<ol data-mc-continue="false">
<li value="1">Click the <strong>Main Menu</strong> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of Adobe Workfront, then click <strong>Setup</strong> <img src="assets/gear-icon-settings.png">.</li>
<li value="2">Click<strong>Job Roles.</strong></li>
<li value="3">Select the job role that you want to delete, then click <strong>Delete.</strong></li>
<li value="4">If there are any objects (users, tasks, issues) that are assigned to the job role, do one of the following:<br>
<ul>
<li><p><strong>Replace the job role with a different job role:</strong> Select the new job role from the drop-down list.</p><p>Any current and past resource allocations that are associated with the deleted job role are transferred to the job role that you select.</p><p>Users who have only one job role assigned to them are reassigned to the job role that you select; users who have a secondary job role assigned to them are not reassigned to the job role that you select.</p></li>
<li><p><strong>Delete the job role and its resource allocation:</strong> Select<strong>None</strong> from the drop-down list.</p><note type="important">
Deleting a job role deletes all current and past resource allocation related to that job role for all projects.
</note><p>​For example, if a task or issue is assigned to only that job role, the task or issue is unassigned after the job role is deleted.</p></li>
</ul></li>
<li value="5">Click  <strong>Yes, Delete It</strong>. </li>
</ol>
</div>
-->
