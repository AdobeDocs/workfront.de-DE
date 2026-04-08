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
source-git-commit: cada5387ddfb710029d06cd38841ecb9c8a6484b
workflow-type: tm+mt
source-wordcount: '1703'
ht-degree: 1%

---

# Erstellen und Verwalten von Aufgabengebieten

<!-- Audited: 1/2024 -->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

{{highlighted-preview}}

>[!IMPORTANT]
>
>Mit Version 25.11 wurde die Überschreibungswährung für Aufgabengebiete in der Produktionsumgebung eingestellt. (Die Einstellung erfolgte am 30. Oktober in der Vorschau-Umgebung.) Anstatt eine Basiswährung zu haben und Währungen zu überschreiben, ist jetzt eine Währung für Aufgabengebiete verfügbar und die Kosten- und Abrechnungssätze werden mit dieser Währung definiert.

Als [!DNL Adobe Workfront] oder Benutzer mit administrativem Zugriff auf Aufgabengebiete können Sie Aufgabengebiete erstellen, die Benutzern zugewiesen werden können, und Standardaufgabengebiete löschen, die für Ihr Unternehmen nicht relevant sind. Informationen zum administrativen Zugriff in [!DNL Workfront] finden Sie unter [Gewähren von administrativem Zugriff für Benutzer auf bestimmte Bereiche](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

>[!TIP]
>
>Aufgabengebiete sind ein integraler Bestandteil der Verwaltung von Ressourcen. Um die Ressourcenplanungs-Tools verwenden zu können, müssen den Aufgabengebieten Kosten und Abrechnungssätze zugeordnet sein. Weitere Informationen finden Sie [Erste Schritte mit der Ressourcenverwaltung](../../../resource-mgmt/resource-mgmt-overview/get-started-resource-management.md).

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] Packstück</td> 
   <td><p>So erstellen oder bearbeiten Sie ein Aufgabengebiet: Beliebiges Workfront- oder Workflow-Paket</p>
   <p>So wenden Sie Tarifattribute an und fügen benutzerdefinierte Formulare zum Aufgabengebiet hinzu: Workflow-Ultimate</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] Lizenz</td> 
   <td><p>[!UICONTROL Standard]</p>
       <p>[!UICONTROL Plan]</p></td>
  </tr> 
  <tr> 
   <td>Konfigurationen der Zugriffsebene</td> 
   <td>Administrativer Zugriff auf Aufgabengebiete</td>
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) in der Dokumentation zu Workfront.

+++

## Erstellen eines Aufgabengebiets

So erstellen Sie ein Aufgabengebiet:

{{step-1-to-setup}}

1. Klicken Sie im linken Bedienfeld auf **[!UICONTROL Aufgabengebiete]**.
1. Klicken Sie **[!UICONTROL Neues Aufgabengebiet] <span class="preview">> Neues Aufgabengebiet erstellen**.</span>
1. Geben Sie Informationen in die folgenden Felder ein:

   * **Name**: Geben Sie einen Namen für das Aufgabengebiet an. Dies ist der Name, der überall in Workfront angezeigt wird, wo das Feld Aufgabengebiet angezeigt wird.

     >[!TIP]
     >
     >Der Name eines Aufgabengebiets kann bis zu 255 Zeichen lang sein. Längere Namen können jedoch in bestimmten Bereichen von Workfront abgeschnitten werden.

   * **Beschreibung**: Geben Sie eine Beschreibung für die Rolle ein, die angibt, was eindeutig ist.
   * **Ist Aktiv**: Wählen Sie **Ja**, wenn die Rolle überall in Workfront aktiv und verfügbar sein soll, um sie mit Benutzenden, Arbeitselementen usw. zu verknüpfen. Wählen Sie **Nein** aus, wenn die Rolle deaktiviert und nicht für die Zuweisung zu Benutzern, Arbeitselementen usw. verfügbar sein soll.

     Informationen zur Deaktivierung von Aufgabengebieten finden Sie unter [Deaktivieren von Aufgabengebieten](/help/quicksilver/administration-and-setup/set-up-workfront/organizational-setup/deactivate-job-roles.md).

   * **Währung**: Die Basiswährung wird standardmäßig angezeigt. Der Workfront-Administrator fügt die Basiswährung im Bereich „Setup“ hinzu. Sie können die Auswahl in eine andere verfügbare Währung ändern und die Währung in gültigen Datumsbereichen ändern.

     >[!TIP]
     >
     >In diesem Feld sind nur Währungen verfügbar, die im Bereich Wechselkurse Ihres Systems verfügbar sind. Wenn Sie nur eine Währung eingerichtet haben, ist nur diese Währung verfügbar.

     Weitere Informationen zum Einrichten der Basiswährung in Workfront finden Sie unter [Einrichten von Wechselkursen](/help/quicksilver/administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md).

     Informationen zum Ändern der Währung eines Projekts finden Sie unter [Ändern der &#x200B;](/help/quicksilver/manage-work/projects/project-finances/change-project-currency.md).

   * **Kostensatz**: Der Kostensatz pro Stunde für das Aufgabengebiet. Dieser Wert berechnet die geplanten Kosten und Istkosten für Aufgaben und Probleme im Zusammenhang mit der Funktion sowie letztendlich die geplanten Kosten und Istkosten der Projekte. Geben Sie den Kurs in der gewählten Währung ein.

     Klicken Sie für gültige Datumssätze auf &quot;**hinzufügen**. Geben Sie den Wert der Kosten/Stunde für den Zeitraum ein und weisen Sie gegebenenfalls ein Start- und Enddatum zu. Der erste Kostensatz hat kein Startdatum und der letzte Kostensatz hat kein Enddatum.

     Einige Daten werden automatisch hinzugefügt. Wenn beispielsweise der erste Kostensatz kein Enddatum hat und Sie einen zweiten Kostensatz mit dem Startdatum 1. Mai 2025 hinzufügen, wird dem ersten Kostensatz das Enddatum 30. April 2025 hinzugefügt, damit keine Lücken entstehen.

     Weitere Informationen zur Kostenberechnung in Workfront finden Sie unter [Kosten nachverfolgen](/help/quicksilver/manage-work/projects/project-finances/track-costs.md).

     >[!TIP]
     >
     >Beim Bearbeiten eines vorhandenen Aufgabengebiets können Sie die Liste sortieren, damit das neueste Startdatum oben in der Tarifliste angezeigt wird.

   * **Abrechnungssatz**: Der Abrechnungssatz pro Stunde für das Aufgabengebiet. Dieser Wert berechnet die geplanten und tatsächlichen Einnahmen aus Aufgaben und Problemen im Zusammenhang mit der Rolle sowie letztendlich die geplanten und tatsächlichen Einnahmen der Projekte. Geben Sie den Kurs in der gewählten Währung ein.

     Klicken Sie für Abrechnungssätze mit Gültigkeitsdatum auf **Abrechnungssatz hinzufügen**. Geben Sie den Wert der Abrechnung/Stunde für den Zeitraum ein und weisen Sie gegebenenfalls ein Start- und Enddatum zu. Der erste Abrechnungssatz hat kein Startdatum und der letzte Abrechnungssatz hat kein Enddatum.

     Einige Daten werden automatisch hinzugefügt. Wenn beispielsweise der erste Abrechnungssatz kein Enddatum hat und Sie einen zweiten mit dem Startdatum 1. Mai 2025 hinzufügen, wird dem ersten Abrechnungssatz das Enddatum 30. April 2025 hinzugefügt, sodass keine Lücken bestehen.

     Informationen zur Umsatzberechnung in Workfront finden Sie unter [Übersicht über Abrechnung und Umsatz](/help/quicksilver/manage-work/projects/project-finances/billing-and-revenue-overview.md).

     >[!TIP]
     >
     >Beim Bearbeiten eines vorhandenen Aufgabengebiets können Sie die Liste sortieren, damit das neueste Startdatum oben in der Tarifliste angezeigt wird.

<!-- Remove or hide the billing rate and cost rate bullets on April 16 for GA -->

1. Klicken Sie **[!UICONTROL Aufgabengebiet erstellen]**. Das Aufgabengebiet kann jetzt Aufgaben, Problemen, Genehmigungen zugewiesen werden oder Sie können Layout-Vorlagen oder andere Objekte für das Aufgabengebiet freigeben. Informationen zu allen Verwendungen von Aufgabengebieten in [!DNL Workfront] finden Sie unter [Aufgabengebiet - Übersicht](../../../administration-and-setup/set-up-workfront/organizational-setup/job-role-overview.md). Informationen zum Löschen eines Aufgabengebiets finden Sie unter [Aufgabengebiet löschen](../../../administration-and-setup/set-up-workfront/organizational-setup/delete-job-roles.md).

<div class="preview">

## Hinzufügen von Tarifen und Attributen zu einem Aufgabengebiet

Abrechnungs- und Kostensätze für ein Aufgabengebiet werden in Finanzberechnungen verwendet.

Tarifattribute werden in Bereichen von Workfront unterstützt, in denen es Tarife gibt, z. B. Aufgabengebiete und Anwender. Wenn Attribute auf ein Aufgabengebiet angewendet werden, werden ihre Zuweisungen automatisch mit den richtigen Raten aufgelöst.

Weitere Informationen finden Sie unter [Definieren von &#x200B;](/help/quicksilver/administration-and-setup/manage-enterprise-operations/define-rate-attributes.md).

{{step-1-to-setup}}

1. Klicken Sie im linken Bedienfeld auf **[!UICONTROL Aufgabengebiete]**.
1. Klicken Sie auf den Namen eines vorhandenen Aufgabengebiets, um es zu bearbeiten.
1. Um die Details des Aufgabengebiets zu aktualisieren, klicken Sie **linken Bereich** Details“.
1. (Optional) Um ein benutzerdefiniertes Formular an das Aufgabengebiet anzuhängen, klicken Sie auf das Feld **Benutzerdefiniertes Formular hinzufügen** in der oberen rechten Ecke der Detailseite und wählen Sie ein benutzerdefiniertes Formular aus der angezeigten Liste aus.

   Weitere Informationen zum Anhängen eines benutzerdefinierten Formulars finden Sie unter [Hinzufügen eines benutzerdefinierten Formulars zu einem Objekt](/help/quicksilver/workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

1. Klicken Sie [!UICONTROL **linken**] auf „Tarife“.
1. Klicken Sie auf [!UICONTROL **Abrechnung**] oder [!UICONTROL **Kosten**], um den Tariftyp auszuwählen.
1. Klicken Sie [!UICONTROL **Tarife hinzufügen**], um einen neuen Tarif hinzuzufügen.

   Oder

   Wählen Sie einen vorhandenen Tarif aus und klicken Sie auf das Symbol **Bearbeiten** ![Symbol „Bearbeiten](assets/edit-icon.png), um ihn zu aktualisieren.

   >[!NOTE]
   >
   >Da jeder Satz mit der Kombination aus Funktion und Attributen verknüpft ist, um einen eindeutigen Satz zu erstellen, können die Attribute beim Bearbeiten eines Satzes nicht geändert werden.

1. Wählen Sie im Feld **Neuer Tarif** Attribute für den Tarif aus, z. B. Agentur, Standort oder Kostenstelle.

   >[!NOTE]
   >
   >Diese Attribute werden separat definiert und können sich auf Umsatz- und Kostenberechnungen auswirken. Weitere Informationen finden Sie unter [Definieren von &#x200B;](/help/quicksilver/administration-and-setup/manage-enterprise-operations/define-rate-attributes.md).

1. Wählen Sie die **Währung** für den Kurs. Der Workfront-Administrator fügt die Basiswährung im Bereich „Setup“ hinzu. Sie können die Auswahl in eine andere verfügbare Währung ändern und die Währung in gültigen Datumsbereichen ändern.

   >[!TIP]
   >
   >In diesem Feld sind nur Währungen verfügbar, die im Bereich Wechselkurse Ihres Systems verfügbar sind. Wenn Sie nur eine Währung eingerichtet haben, ist nur diese Währung verfügbar.

   Weitere Informationen zum Einrichten der Basiswährung in Workfront finden Sie unter [Einrichten von Wechselkursen](/help/quicksilver/administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md).

   Informationen zum Ändern der Währung eines Projekts finden Sie unter [Ändern der &#x200B;](/help/quicksilver/manage-work/projects/project-finances/change-project-currency.md).

1. (Bedingt) Geben Sie für einen Abrechnungssatz den **Abrechnungssatz** für dieses Aufgabengebiet ein.

   Dies ist der Abrechnungssatz pro Stunde für das Aufgabengebiet. Dieser Wert berechnet die geplanten und tatsächlichen Einnahmen aus Aufgaben und Problemen im Zusammenhang mit der Rolle sowie letztendlich die geplanten und tatsächlichen Einnahmen der Projekte. Geben Sie den Kurs in der gewählten Währung ein.

   Wenn Sie Attribute verwenden, werden die Attribute und das Aufgabengebiet kombiniert, um einen eindeutigen Satz zu definieren. Beispielsweise kann eine Designer-Funktion in New York für die Agentur A einen anderen Tarif als eine Designer-Funktion in Paris für die Agentur B haben.

   Klicken Sie für Abrechnungssätze mit Gültigkeitsdatum auf **Abrechnungssatz hinzufügen**. Geben Sie den Wert der Abrechnung/Stunde für den Zeitraum ein und weisen Sie gegebenenfalls ein Start- und Enddatum zu. Der erste Abrechnungssatz hat kein Startdatum und der letzte Abrechnungssatz hat kein Enddatum.

   Einige Daten werden automatisch hinzugefügt. Wenn beispielsweise der erste Abrechnungssatz kein Enddatum hat und Sie einen zweiten mit dem Startdatum 1. Mai hinzufügen, wird dem ersten Abrechnungssatz das Enddatum 30. April hinzugefügt, damit keine Lücken entstehen.

   Informationen zur Umsatzberechnung in Workfront finden Sie unter [Übersicht über Abrechnung und Umsatz](/help/quicksilver/manage-work/projects/project-finances/billing-and-revenue-overview.md).

   >[!TIP]
   >
   >Beim Bearbeiten eines vorhandenen Aufgabengebiets können Sie die Liste sortieren, damit das neueste Startdatum oben in der Tarifliste angezeigt wird.

1. (Bedingt) Geben Sie für einen Kostensatz den **Kostensatz** für dieses Aufgabengebiet ein.

   Dies ist der Stundensatz (Cost per Hour Rate) des Aufgabengebiets. Dieser Wert berechnet die geplanten Kosten und Istkosten für Aufgaben und Probleme im Zusammenhang mit der Funktion sowie letztendlich die geplanten Kosten und Istkosten der Projekte. Geben Sie den Kurs in der gewählten Währung ein.

   Wenn Sie Attribute verwenden, werden die Attribute und das Aufgabengebiet kombiniert, um einen eindeutigen Satz zu definieren. Beispielsweise kann eine Designer-Funktion in New York für die Agentur A einen anderen Tarif als eine Designer-Funktion in Paris für die Agentur B haben.

   Klicken Sie für gültige Datumssätze auf &quot;**hinzufügen**. Geben Sie den Wert der Kosten/Stunde für den Zeitraum ein und weisen Sie gegebenenfalls ein Start- und Enddatum zu. Der erste Kostensatz hat kein Startdatum und der letzte Kostensatz hat kein Enddatum.

   Einige Daten werden automatisch hinzugefügt. Wenn beispielsweise der erste Kostensatz kein Enddatum hat und Sie einen zweiten Kostensatz mit dem Startdatum 1. Mai hinzufügen, wird der erste Kostensatz um das Enddatum 30. April erweitert, sodass keine Lücken entstehen.

   Weitere Informationen zur Kostenberechnung in Workfront finden Sie unter [Kosten nachverfolgen](/help/quicksilver/manage-work/projects/project-finances/track-costs.md).

   >[!TIP]
   >
   >Beim Bearbeiten eines vorhandenen Aufgabengebiets können Sie die Liste sortieren, damit das neueste Startdatum oben in der Tarifliste angezeigt wird.

1. Klicken Sie auf [!UICONTROL **Speichern**].

</div>

<!--
   * **Override Currency Cost Rate**: This is the cost per hour rate of the job role using the selected Override Currency. Workfront uses this value to calculate the planned and the actual costs of tasks and issues associated with the job role.

     Enter the rate in the Override Currency specified above. This also updates the Cost Rate for this job role when using the Base Currency.

     For information about how Workfront calculates cost, see [Track costs](/help/quicksilver/manage-work/projects/project-finances/track-costs.md).

     >[!TIP]
     >
     >When updating an existing job role that already has a cost rate associated with it, Workfront calculates the Override Currency rate based on the conversion rate in your system. If you update the Override Currency Cost Rate, the cost rate of the job role also updates automatically.

   * **Override Currency Billing Rate**: This is the billing per hour rate of the job role using the selected Override Currency. Workfront uses this value to calculate the planned and the actual revenue of tasks and issues associated with the job role.

      Enter the rate in the Override Currency specified above. This also updates the Billing Rate for this job role when using the Base Currency.

      For information about how Workfront calculates revenue, see [Overview of Billing and Revenue](/help/quicksilver/manage-work/projects/project-finances/billing-and-revenue-overview.md).

     >[!TIP]
     >
     >When updating an existing job role that already has a billing rate associated with it, Workfront calculates the Override Currency rate based on the conversion rate in your system. If you update the Override Currency Billing Rate, the billing rate of the job role also updates automatically.

-->



