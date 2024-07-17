---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: organization-setup
title: Erstellen und Verwalten von Aufgabengebieten
description: Als [!DNL Adobe Workfront] Administrator oder Benutzer mit administrativem Zugriff auf "Vorgangsrollen"können Sie Auftragsrollen erstellen, die Benutzern zugewiesen werden können, und Standardauftragsrollen löschen, die für Ihr Unternehmen nicht relevant sind.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 664fb2fe-ff7e-4807-9a43-b37e7d5d57eb
source-git-commit: 4572ea9bb0679c599a55d5a87c1397c7b819c963
workflow-type: tm+mt
source-wordcount: '1151'
ht-degree: 0%

---

# Erstellen und Verwalten von Aufgabengebieten

<!-- Audited: 1/2024 -->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

Als [!DNL Adobe Workfront] -Administrator oder Benutzer mit administrativem Zugriff auf &quot;Vorgangsrollen&quot;können Sie Auftragsrollen erstellen, die Benutzern zugewiesen werden können, und Standardauftragsrollen löschen, die für Ihr Unternehmen nicht relevant sind. Informationen zum administrativen Zugriff in [!DNL Workfront] finden Sie unter [Gewähren von Benutzern administrativen Zugriff auf bestimmte Bereiche](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

Sie müssen über Folgendes verfügen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Plan</td> 
   <td> <p>Alle </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Lizenz</td> 
   <td>
   <p>Neu: Standard</p>
   <p>Aktuell: [!UICONTROL Plan]</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Administratorzugriff auf die Rollen "Aufträge"</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren [!DNL Workfront] -Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

+++

## Erstellen einer Auftragsrolle

So erstellen Sie eine Arbeitsplatzrolle:

{{step-1-to-setup}}

1. Klicken Sie im linken Bereich auf &#x200B; **[!UICONTROL Vorgangsrollen].**
1. Klicken Sie auf **[!UICONTROL Neue Auftragsrolle].**
1. Konfigurieren Sie Folgendes:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Name]</td> 
      <td> <p>Geben Sie einen Namen für die Auftragsrolle an. Dies ist der Name, der überall in [!DNL Workfront] angezeigt wird, wo das Feld [!UICONTROL Auftragsrolle] angezeigt wird. </p> <p>Tipp: Der Name einer Auftragsrolle kann bis zu 255 Zeichen enthalten. Längere Namen können jedoch in bestimmten Bereichen von [!DNL Workfront] abgeschnitten werden. </p> </td> 
     </tr>
     <tr> 
      <td role="rowheader">[!UICONTROL Beschreibung]</td> 
      <td>Geben Sie eine Beschreibung für die Rolle ein, die angibt, was eindeutig ist. </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL ist aktiv]</span> </td> 
      <td> 
       <ul> 
        <li> <p>Wählen Sie <b>[!UICONTROL Ja]</b> aus, wenn die Rolle aktiv sein und überall in [!DNL Workfront] verfügbar sein soll, damit sie mit Benutzern, Arbeitselementen usw. verknüpft werden kann. </p> </li> 
        <li> <p>Wählen Sie <b>[!UICONTROL No]</b> aus, wenn die Rolle deaktiviert und nicht für die Zuweisung an Benutzer, Arbeitselemente usw. verfügbar sein soll. </p> </li> 
       </ul> <p><span>Weitere Informationen zum Deaktivieren von Vorgangsrollen finden Sie unter </span> <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/deactivate-job-roles.md" class="MCXref xref">Deaktivieren von Vorgangsrollen</a>. </p> </td> 
     </tr>
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL Basiswährung]</span> </td> 
      <td> <p><span>Dies ist die [!UICONTROL Basiswährung], die von Ihrem Workfront-Administrator im Bereich [!UICONTROL Setup] festgelegt wurde. Weitere Informationen finden Sie unter</span> <a href="../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md" class="MCXref xref">Einrichten von Wechselkursen</a> .</p> <p>Tipp: <span>Sie können die [!UICONTROL Basiswährung] nicht auf Arbeitsplatzrollenebene bearbeiten. Dieses Feld ist abgeblendet und dient als Erinnerung an die Basiswährung für Ihr System.</span> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Kostensatz]</td> 
      <td><p>Dies ist die Kosten pro Stunde für die Rolle "Auftrag". Dieser Wert berechnet die geplanten und tatsächlichen Kosten der Aufgaben und Probleme im Zusammenhang mit der Rolle sowie schließlich die geplanten und tatsächlichen Kosten der Projekte. Geben Sie den Wechselkurs mithilfe der [!UICONTROL Basiswährung] ein.</p> 
      <p>Klicken Sie für Datumswerte mit effektiven Kostensätzen auf <strong>[!UICONTROL Rate hinzufügen]</strong>. Geben Sie den Wert der Kosten/Stunde für den Zeitraum ein und weisen Sie nach Bedarf ein [!UICONTROL Startdatum] und ein [!UICONTROL Enddatum] zu. Der erste Kostensatz hat kein Startdatum und der letzte Kostensatz hat kein Enddatum.</p> <p>Einige Daten werden automatisch hinzugefügt. Wenn beispielsweise der erste Kostensatz kein Enddatum hat und Sie einen zweiten Kostensatz mit einem Startdatum vom 1. Mai 2023 hinzufügen, wird dem ersten Kostensatz ein Enddatum vom 30. April 2023 hinzugefügt, sodass keine Lücken bestehen.</p> <p>Tipp: Wenn Sie eine vorhandene Auftragsrolle bearbeiten, können Sie <strong>Nach Startdatum sortieren</strong> auswählen, um das neueste Startdatum oben in der Ratenliste anzuzeigen.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Abrechnungsrate] </td> 
      <td><p>Dies ist die Abrechnungsrate pro Stunde für die Auftragsrolle. Dieser Wert berechnet die geplanten und tatsächlichen Einnahmen aus Aufgaben und Problemen im Zusammenhang mit der Rolle sowie letztlich die geplanten und tatsächlichen Einnahmen der Projekte. Geben Sie den Wechselkurs mithilfe der [!UICONTROL Basiswährung] ein.</p> <p>Klicken Sie für das Datum, an dem die effektiven Abrechnungsraten gelten, auf <strong>[!UICONTROL Zusatzrate]</strong>. Geben Sie den Wert der Abrechnung/Stunde für den Zeitraum ein und weisen Sie nach Bedarf ein [!UICONTROL Startdatum] und ein [!UICONTROL Enddatum] zu. Der erste Abrechnungskurs hat kein Startdatum und der letzte Abrechnungskurs hat kein Enddatum.</p> <p>Einige Daten werden automatisch hinzugefügt. Wenn beispielsweise der erste Abrechnungskurs kein Enddatum hat und Sie einen zweiten mit dem Startdatum 1. Mai 2023 hinzufügen, wird dem ersten Abrechnungskurs ein Enddatum vom 30. April 2023 hinzugefügt, sodass keine Lücken bestehen.</p> <p>Tipp: Wenn Sie eine vorhandene Auftragsrolle bearbeiten, können Sie <strong>Nach Startdatum sortieren</strong> auswählen, um das neueste Startdatum oben in der Ratenliste anzuzeigen.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL Währung überschreiben]</span> </td> 
      <td>
        <p>Wählen Sie eine Währung aus, die mit dieser Auftragsrolle verknüpft ist. Dies ist die Währung, die [!DNL Workfront] zur Berechnung der Kosten und Einnahmen im Zusammenhang mit dieser Stellenfunktion verwendet. </p> 
        <p><span>Dies unterscheidet sich von der [!UICONTROL Basiswährung], die von Ihrem [!DNL Workfront] -Administrator im [!UICONTROL Setup] -Bereich eingerichtet wurde, und kann sich von der mit einem Projekt verknüpften Währung unterscheiden.</span> </p> 
        <p>Tipp: In diesem Feld sind nur Währungen verfügbar, die im Bereich [!UICONTROL Wechselkurse] Ihres Systems verfügbar sind. Wenn Sie nur eine Währung eingerichtet haben, wird dieses Feld nicht angezeigt.</p> 
       <p><span>Informationen zum Einrichten der [!UICONTROL Basiswährung] in [!DNL Workfront] finden Sie unter </span> <a href="../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md" class="MCXref xref">Einrichten von Wechselkursen</a>.</p> <p><span>Informationen zum Ändern der Währung eines Projekts finden Sie unter </span> <a href="../../../manage-work/projects/project-finances/change-project-currency.md" class="MCXref xref">Ändern der Projektwährung</a>.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL Währungskostenrate überschreiben]</span> </td> 
      <td>
        <p>Dies ist die Kosten pro Stunde für die Rolle "Auftrag"unter Verwendung der ausgewählten [!UICONTROL Überschreibungswährung]. [!DNL Workfront] verwendet diesen Wert zur Berechnung der geplanten und tatsächlichen Kosten von Aufgaben und Problemen, die mit der Auftragsrolle verbunden sind. </p> 
        <p><span>Geben Sie die Rate in die oben angegebene [!UICONTROL Überschreibungswährung] ein. Dadurch wird auch der Kostensatz für diese Auftragsrolle bei Verwendung der [!UICONTROL Basiswährung] aktualisiert.</span> </p> 
        <p>Informationen zur Berechnung der Kosten durch [!DNL Workfront] finden Sie unter <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Kosten für die Nachverfolgung</a>.</p> 
       <p>Tipp: Beim Aktualisieren einer vorhandenen Auftragsrolle, der bereits eine Kostenquote zugeordnet ist, berechnet [!DNL Workfront] die [!UICONTROL Override Currency]-Rate basierend auf der Konversionsrate in Ihrem System. Wenn Sie die [!UICONTROL Override Currency Cost Rate] aktualisieren, wird auch die Kostenstelle der Auftragsrolle automatisch aktualisiert.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL Währungsabrechnungsrate überschreiben]</span> </td> 
      <td>
        <p>Dies ist die Abrechnungsrate pro Stunde der Auftragrolle unter Verwendung der ausgewählten [!UICONTROL Überschreibungswährung]. [!DNL Workfront] verwendet diesen Wert zur Berechnung des geplanten und des tatsächlichen Umsatzes von Aufgaben und Problemen, die mit der Auftragsrolle verbunden sind. </p>
        <p><span>Geben Sie die Rate in die oben angegebene [!UICONTROL Überschreibungswährung] ein. Dadurch wird auch der Abrechnungskurs für diese Auftragsrolle aktualisiert, wenn die [!UICONTROL Basiswährung] verwendet wird.</span> </p>
        <p>Informationen zur Berechnung des Umsatzes durch [!DNL Workfront] finden Sie unter <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">Übersicht über Rechnungsstellung und Umsatz</a>.</p>
        <p>Tipp: Beim Aktualisieren einer vorhandenen Auftragsrolle, der bereits eine Abrechnungsrate zugeordnet ist, berechnet [!DNL Workfront] die Überschreibungswährungsrate basierend auf der Konversionsrate in Ihrem System. Wenn Sie die Überschreiben der Währungsabrechnungsrate aktualisieren, wird auch die Abrechnungsrate der Auftragsrolle automatisch aktualisiert. </p>
       </td>
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >Die Rolle von Arbeitsplätzen ist ein integraler Bestandteil der Ressourcenverwaltung. Um die Tools zur Ressourcenplanung zu verwenden, benötigen die Rollen einen damit verbundenen Kosten- und Abrechnungskurs. Weitere Informationen finden Sie unter [Erste Schritte mit der Ressourcenverwaltung](../../../resource-mgmt/resource-mgmt-overview/get-started-resource-management.md).

1. Klicken Sie auf **[!UICONTROL Auftragsrolle erstellen]**. Die Rolle &quot;Auftrag&quot;kann jetzt Aufgaben, Problemen, Genehmigungen oder Layoutvorlagen oder anderen Objekten zugewiesen werden. Weitere Informationen zu allen Verwendungen von Auftragsrollen in [!DNL Workfront] finden Sie unter [Übersicht über Auftragsrollen](../../../administration-and-setup/set-up-workfront/organizational-setup/job-role-overview.md). Weitere Informationen zum Löschen einer Auftragsrolle finden Sie unter [Löschen von Auftragsrollen](../../../administration-and-setup/set-up-workfront/organizational-setup/delete-job-roles.md).

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
