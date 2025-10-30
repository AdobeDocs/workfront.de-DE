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
source-git-commit: e5416fab4f4ad1f2c31edf962554ddd6a4c2f1e5
workflow-type: tm+mt
source-wordcount: '1165'
ht-degree: 0%

---

# Erstellen und Verwalten von Aufgabengebieten

<!-- Audited: 1/2024 -->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

>[!IMPORTANT]
>
>Mit Version 25.11 wird die Überschreibungswährung für Aufgabengebiete in der Produktion eingestellt. (Die Einstellung erfolgt am 30. Oktober in der Vorschau-Umgebung.) Anstatt eine Basiswährung zu haben und Währungen zu überschreiben, steht für Aufgabengebiete eine Währung zur Verfügung, und die Kosten und Abrechnungssätze werden mit dieser Währung definiert.

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
       <p>[!UICONTROL -Plan]</p></td>
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
1. Konfigurieren Sie die folgenden Felder:

   * **Name**: Geben Sie einen Namen für das Aufgabengebiet an. Dies ist der Name, der überall in Workfront angezeigt wird, wo das Feld Aufgabengebiet angezeigt wird.

     >[!TIP]
     >
     >Der Name eines Aufgabengebiets kann bis zu 255 Zeichen lang sein. Längere Namen können jedoch in bestimmten Bereichen von Workfront abgeschnitten werden.

   * **Beschreibung**: Geben Sie eine Beschreibung für die Rolle ein, die angibt, was eindeutig ist.
   * **Ist Aktiv**: Wählen Sie **Ja**, wenn die Rolle überall in Workfront aktiv und verfügbar sein soll, um sie mit Benutzenden, Arbeitselementen usw. zu verknüpfen. Wählen Sie **Nein** aus, wenn die Rolle deaktiviert und nicht für die Zuweisung zu Benutzern, Arbeitselementen usw. verfügbar sein soll.

     Informationen zur Deaktivierung von Aufgabengebieten finden Sie unter [Deaktivieren von Aufgabengebieten](/help/quicksilver/administration-and-setup/set-up-workfront/organizational-setup/deactivate-job-roles.md).

   * **Basiswährung**: Dies ist die Basiswährung, die von Ihrem Workfront-Administrator im Bereich „Setup“ festgelegt wurde. Weitere Informationen finden Sie [Einrichten von Wechselkursen](/help/quicksilver/administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md).

     >[!TIP]
     >
     >Die Basiswährung kann nicht auf Aufgabengebiet-Ebene bearbeitet werden. Dieses Feld ist abgeblendet und dient als Erinnerung daran, was die Basiswährung für Ihr System ist.

   * **Kostensatz**: Der Kostensatz pro Stunde für das Aufgabengebiet. Dieser Wert berechnet die geplanten Kosten und Istkosten für Aufgaben und Probleme im Zusammenhang mit der Funktion sowie letztendlich die geplanten Kosten und Istkosten der Projekte. Geben Sie den Kurs unter Verwendung der Basiswährung ein.

     Klicken Sie für gültige Datumssätze auf &quot;**hinzufügen**. Geben Sie den Wert der Kosten/Stunde für den Zeitraum ein und weisen Sie gegebenenfalls ein Start- und Enddatum zu. Der erste Kostensatz hat kein Startdatum und der letzte Kostensatz hat kein Enddatum.

     Einige Daten werden automatisch hinzugefügt. Wenn beispielsweise der erste Kostensatz kein Enddatum hat und Sie einen zweiten Kostensatz mit dem Startdatum 1. Mai 2025 hinzufügen, wird dem ersten Kostensatz das Enddatum 30. April 2025 hinzugefügt, damit keine Lücken entstehen.

     >[!TIP]
     >
     >Beim Bearbeiten eines vorhandenen Aufgabengebiets können Sie **Sortieren nach Startdatum** auswählen, um das neueste Startdatum oben in der Tarifliste anzuzeigen.

   * **Abrechnungssatz**: Der Abrechnungssatz pro Stunde für das Aufgabengebiet. Dieser Wert berechnet die geplanten und tatsächlichen Einnahmen aus Aufgaben und Problemen im Zusammenhang mit der Rolle sowie letztendlich die geplanten und tatsächlichen Einnahmen der Projekte. Geben Sie den Kurs unter Verwendung der Basiswährung ein.

     Klicken Sie für Abrechnungssätze mit Gültigkeitsdatum auf **Abrechnungssatz hinzufügen**. Geben Sie den Wert der Abrechnung/Stunde für den Zeitraum ein und weisen Sie gegebenenfalls ein Start- und Enddatum zu. Der erste Abrechnungssatz hat kein Startdatum und der letzte Abrechnungssatz hat kein Enddatum.

     Einige Daten werden automatisch hinzugefügt. Wenn beispielsweise der erste Abrechnungssatz kein Enddatum hat und Sie einen zweiten mit dem Startdatum 1. Mai 2025 hinzufügen, wird dem ersten Abrechnungssatz das Enddatum 30. April 2025 hinzugefügt, sodass keine Lücken bestehen.

     >[!TIP]
     >
     >Beim Bearbeiten eines vorhandenen Aufgabengebiets können Sie **Sortieren nach Startdatum** auswählen, um das neueste Startdatum oben in der Tarifliste anzuzeigen.

   * **Währung überschreiben**: Wählen Sie eine Währung aus, die mit diesem Aufgabengebiet verknüpft ist. Dies ist die Währung, die Workfront zur Berechnung der Kosten und Einnahmen im Zusammenhang mit diesem Aufgabengebiet verwendet.

     Diese Währung unterscheidet sich von der Basiswährung, die von Ihrem Workfront-Administrator im Bereich „Setup“ festgelegt wurde, und kann sich von der einem Projekt zugeordneten Währung unterscheiden.

     >[!TIP]
     >
     >In diesem Feld sind nur Währungen verfügbar, die im Bereich Wechselkurse Ihres Systems verfügbar sind. Wenn Sie nur eine Währung eingerichtet haben, wird dieses Feld nicht angezeigt.

     Weitere Informationen zum Einrichten der Basiswährung in Workfront finden Sie unter [Einrichten von Wechselkursen](/help/quicksilver/administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md).

     Informationen zum Ändern der Währung eines Projekts finden Sie unter [Ändern der &#x200B;](/help/quicksilver/manage-work/projects/project-finances/change-project-currency.md).

   * **Währungskostensatz überschreiben**: Dies ist der Kostensatz pro Stunde für das Aufgabengebiet unter Verwendung der ausgewählten Überschreibungswährung. Workfront verwendet diesen Wert, um die geplanten Kosten und Istkosten für Aufgaben und Probleme im Zusammenhang mit dem Aufgabengebiet zu berechnen.

     Geben Sie den Kurs in die oben angegebene Währung zum Überschreiben ein. Dadurch wird auch der Kostensatz für dieses Aufgabengebiet bei Verwendung der Basiswährung aktualisiert.

     Weitere Informationen zur Kostenberechnung in Workfront finden Sie unter [Kosten nachverfolgen](/help/quicksilver/manage-work/projects/project-finances/track-costs.md).

     >[!TIP]
     >
     >Beim Aktualisieren eines bestehenden Aufgabengebiets, dem bereits ein Kostensatz zugeordnet ist, berechnet Workfront den Wechselkurs zum Überschreiben der Währung anhand des Konversionssatzes in Ihrem System. Wenn Sie den Kostensatz Währung überschreiben aktualisieren, wird auch der Kostensatz des Aufgabengebiets automatisch aktualisiert.

   * **Währung überschreiben Abrechnungssatz**: Dies ist der Abrechnungssatz pro Stunde für das Aufgabengebiet unter Verwendung der ausgewählten Überschreibungswährung. Workfront verwendet diesen Wert, um den geplanten und tatsächlichen Umsatz von Aufgaben und Problemen im Zusammenhang mit dem Aufgabengebiet zu berechnen.

     Geben Sie den Kurs in die oben angegebene Währung zum Überschreiben ein. Dadurch wird auch der Abrechnungssatz für dieses Aufgabengebiet aktualisiert, wenn die Basiswährung verwendet wird.

     Informationen zur Umsatzberechnung in Workfront finden Sie unter [Übersicht über Abrechnung und Umsatz](/help/quicksilver/manage-work/projects/project-finances/billing-and-revenue-overview.md).

     >[!TIP]
     >
     >Beim Aktualisieren eines bestehenden Aufgabengebiets, dem bereits ein Abrechnungssatz zugeordnet ist, berechnet Workfront den Überschreibungswährungssatz auf der Grundlage des Konversionssatzes in Ihrem System. Wenn Sie den Abrechnungssatz Währung überschreiben aktualisieren, wird auch der Abrechnungssatz des Aufgabengebiets automatisch aktualisiert.

<!--
   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Name]</td> 
      <td> <p>Indicate a name for the job role. This is the name that displays everywhere in [!DNL Workfront] where the [!UICONTROL Job Role] field displays. </p> <p>Tip: The name of a job role may contain up to 255 characters. However, longer names might be truncated in certain areas of [!DNL Workfront]. </p> </td> 
     </tr>
     <tr> 
      <td role="rowheader">[!UICONTROL Description]</td> 
      <td>Enter a description for the role that indicates what is unique about it. </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL Is Active]</span> </td> 
      <td> 
       <ul> 
        <li> <p>Select <b>[!UICONTROL Yes]</b> if you want the role to be active and available everywhere in [!DNL Workfront] to be associated with users, work items, etc. </p> </li> 
        <li> <p>Select <b>[!UICONTROL No]</b>, if you want the role to be deactivated and not available to assign to users, work items, etc. </p> </li> 
       </ul> <p><span>For information about deactivating job roles, see</span> <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/deactivate-job-roles.md" class="MCXref xref">Deactivate job roles</a>. </p> </td> 
     </tr>
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL Base Currency]</span> </td> 
      <td> <p><span>This is the [!UICONTROL Base Currency], as set in the [!UICONTROL Setup] area by your Workfront administrator. For information, see</span> <a href="../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md" class="MCXref xref">Set up exchange rates</a> .</p> <p>Tip: <span>You cannot edit the [!UICONTROL Base Currency] at the job role level. This field is dimmed and serves as a reminder for what the base currency is for your system.</span> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Cost Rate]</td> 
      <td><p>This is the cost per hour rate of the job role. This value calculates the planned and the actual costs of tasks and issues associated with the role, and ultimately the planned and actual costs of the projects. Enter the rate using the [!UICONTROL Base Currency].</p> 
      <p>For date effective cost rates, click <strong>[!UICONTROL Add Rate]</strong>. Enter the value of the cost/hour for the time period, and assign a [!UICONTROL Start Date] and [!UICONTROL End Date] as needed. The first cost rate will not have a start date and the last cost rate will not have an end date.</p> <p>Some dates are added automatically. For example, if the first cost rate does not have an end date, and you add a second cost rate with a start date of May 1, 2023, an end date of April 30, 2023 is added to the first cost rate so that no gaps exist.</p> <p>Tip: When editing an existing job role, you can select <strong>Sort by start date</strong> to see the most recent start date at the top of the rate list.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Billing Rate] </td> 
      <td><p>This is the billing per hour rate of the job role. This value calculates the planned and actual revenues of tasks and issues associated with the role, and ultimately the planned and actual revenues of the projects. Enter the rate using the [!UICONTROL Base Currency].</p> <p>For date effective billing rates, click <strong>[!UICONTROL Add Rate]</strong>. Enter the value of the billing/hour for the time period, and assign a [!UICONTROL Start Date] and [!UICONTROL End Date] as needed. The first billing rate will not have a start date and the last billing rate will not have an end date.</p> <p>Some dates are added automatically. For example, if the first billing rate does not have an end date, and you add a second with a start date of May 1, 2023, an end date of April 30, 2023 is added to the first billing rate so that no gaps exist.</p> <p>Tip: When editing an existing job role, you can select <strong>Sort by start date</strong> to see the most recent start date at the top of the rate list.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL Override Currency]</span> </td> 
      <td>
        <p>Select a currency associated with this job role. This is the currency that [!DNL Workfront] uses for calculating costs and revenue associated with this job role. </p> 
        <p><span>This is different than the [!UICONTROL Base Currency] set up by your [!DNL Workfront] administrator in the [!UICONTROL Setup] area, and can be different than the currency associated with a project.</span> </p> 
        <p>Tip: Only currencies available in the [!UICONTROL Exchange Rates] area in your system are available in this field. If you only have one currency set up, this field is does not appear.</p> 
       <p><span>For information about setting up the [!UICONTROL Base Currency] in [!DNL Workfront], see</span> <a href="../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md" class="MCXref xref">Set up exchange rates</a>.</p> <p><span>For information about changing the currency of a project, see</span> <a href="../../../manage-work/projects/project-finances/change-project-currency.md" class="MCXref xref">Change the project currency</a>.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL Override Currency Cost Rate]</span> </td> 
      <td>
        <p>This is the cost per hour rate of the job role using the selected [!UICONTROL Override Currency]. [!DNL Workfront] uses this value to calculate the planned and the actual costs of tasks and issues associated with the job role. </p> 
        <p><span>Enter the rate in the [!UICONTROL Override Currency] specified above. This also updates the Cost Rate for this job role when using the [!UICONTROL Base Currency].</span> </p> 
        <p>For information about how [!DNL Workfront] calculates cost, see <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Track costs</a>.</p> 
       <p>Tip: When updating an existing job role that already has a Cost Rate associated with it, [!DNL Workfront] calculates the [!UICONTROL Override Currency] rate based on the conversion rate in your system. If you update the [!UICONTROL Override Currency Cost Rate], the Cost Rate of the job role also updates automatically.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL Override Currency Billing Rate]</span> </td> 
      <td>
        <p>This is the billing per hour rate of the job role using the selected [!UICONTROL Override Currency]. [!DNL Workfront] uses this value to calculate the planned and the actual revenue of tasks and issues associated with the job role. </p>
        <p><span>Enter the rate in the [!UICONTROL Override Currency] specified above. This also updates the Billing Rateate for this job role when using the [!UICONTROL Base Currency].</span> </p>
        <p>For information about how [!DNL Workfront] calculates revenue, see <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">Overview of Billing and Revenue</a>.</p>
        <p>Tip: When updating an existing job role that already has a Billing Rate associated with it, [!DNL Workfront] calculates the Override Currency rate based on the conversion rate in your system. If you update the Override Currency Billing Rate, the Billing Rate of the job role also updates automatically. </p>
       </td>
     </tr> 
    </tbody> 
   </table>
-->

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
