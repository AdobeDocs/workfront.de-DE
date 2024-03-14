---
user-type: administrator
product-area: system-administration
navigation-topic: organization-setup
title: Erstellen und Bearbeiten von Unternehmen
description: Sie können Unternehmen zu [!DNL Adobe Workfront] und verwenden sie für Finanzplanung, Reporting, um Berechtigungen für Objekte zu definieren und Informationen vertraulich zu behandeln.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: bb597032-3395-4c9a-b622-5c920ba55131
source-git-commit: 155a2a8f5f266006629a28917a6a7565a95b37a9
workflow-type: tm+mt
source-wordcount: '1461'
ht-degree: 0%

---

# Erstellen und Bearbeiten von Unternehmen

{{highlighted-preview}}

<!--Audited: 01/2024-->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

Ein Unternehmen ist eine Organisationseinheit in [!DNL Adobe Workfront] die Ihre Organisation, eine Abteilung innerhalb der Organisation oder einen Kunden, mit dem Sie arbeiten, vertreten können. Sie können Unternehmen zu [!DNL Workfront] und verwenden sie für Finanzplanung, Reporting, um Berechtigungen für Objekte zu definieren und Informationen vertraulich zu behandeln.

## Zugriffsanforderungen

Sie müssen über Folgendes verfügen, um Unternehmen in [!DNL Workfront]:

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Workfront] Plan</p> </td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Adobe Workfront] license*</p> </td> 
   <td><p>Aktuell: [!UICONTROL Plan]</p>
   Oder
   <p>Neu: [!UICONTROL Standard]</p>
   </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Konfiguration der Zugriffsebene</td> 
   <td> <p>Eine der folgenden Optionen:</p> 
    <ul> 
     <li> <p>Die Zugriffsstufe [!UICONTROL Systemadministrator], mit der Sie jedes Unternehmen im System bearbeiten können. Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md">Gewähren eines vollen Administratorzugriffs</a>. </p> </li> 
     <li> <p>Verwaltungszugriff zur Verwaltung von Unternehmen, mit dem Sie jedes Unternehmen im System bearbeiten können. Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md">Benutzern administrativen Zugriff auf bestimmte Bereiche gewähren</a>.</p> </li> 
    </ul> <p><b>NOTE</b>:  
     <ul> 
      <li> <p>Sie können auch Unternehmen verwalten, die mit einer beliebigen Gruppe verbunden sind, der Sie als Gruppenadministrator zugewiesen sind.</p> </li> 
      <li> <p>Um Benutzer zum hinzuzufügen und aus dem [!DNL Workfront] -System verwenden, müssen Sie über einen der folgenden Schritte verfügen:</p> 
       <ul> 
        <li> <p>Die Zugriffsstufe des [!UICONTROL Systemadministrators]. Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Gewähren eines vollen Administratorzugriffs</a>. </p> </li> 
        <li> <p>In Ihrer Zugriffsebene muss [!UICONTROL Bearbeiten] für die Einstellung [!UICONTROL Benutzer] ausgewählt sein. Außerdem können Sie für die Einstellung [!UICONTROL Benutzer] unter [!UICONTROL Feinabstimmung Ihrer Einstellungen] <img src="assets/gear-icon-in-access-levels.png">, müssen die Option [!UICONTROL Erstellen] und mindestens eine der beiden [!UICONTROL User Admin]-Optionen aktiviert sein. </p> <p> <img src="assets/access-req-users.png"> </p> <p>Wenn Sie die Option [!UICONTROL Benutzeradministrator (Gruppenbenutzer)] verwenden, müssen Sie Gruppenadministrator einer Gruppe sein, der der Benutzer angehört.</p> </li> 
       </ul> <p>Informationen zur Benutzereinstellung auf Zugriffsebene finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Benutzern Zugriff gewähren</a>.</p> </li> 
     </ul> </p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren [!DNL Workfront] Administrator. Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Vorteile beim Hinzufügen von Benutzern zu einem Unternehmen {#benefits-of-adding-users-to-a-company}

* Sie können das Organisationsdiagramm eines Unternehmens erstellen, indem Sie Benutzer direkten Berichten zuordnen. Nur Benutzer desselben Unternehmens können als direkte Berichte eines anderen Benutzers aus diesem Unternehmen hinzugefügt werden.
* Als Projektmanager können Sie verfügbare Ressourcen innerhalb desselben Unternehmens identifizieren.
* Sie können Informationen zwischen Unternehmen privat halten, indem Sie eine oder alle der folgenden Einstellungen auswählen:

   * Benutzer desselben Unternehmens können die Anforderungen der anderen Benutzer sehen.

     Weitere Informationen zum [!DNL Workfront] -Administrator kann ähnlichen Zugriff auf Anforderungen auf Grundlage des Unternehmens der Benutzer gewähren. Weitere Informationen finden Sie im Abschnitt [Konfigurieren Sie die Voreinstellungen für Aufgaben und Probleme für alle Benutzer in [!DNL Workfront]](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md#changing-task-and-issue-preferences) im Artikel [Systemweite Aufgaben- und Problemeinstellungen konfigurieren](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

     Weitere Informationen dazu, wie ein Gruppenadministrator ähnlichen Zugriff auf Anforderungen je nach Unternehmen der Benutzer gewähren kann, finden Sie unter [Konfigurieren von Aufgaben- und Problemeinstellungen für eine Gruppe](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

   * Benutzer können nur Anforderungswarteschlangen sehen, die mit ihren Unternehmen verknüpft sind. Weitere Informationen zum Einschränken der Sichtbarkeit einer Anforderungswarteschlange finden Sie unter [Zugriff auf Anforderungswarteschlangen gewähren](../../../manage-work/requests/create-and-manage-request-queues/provide-access-to-request-queues.md).
   * Sie können Benutzer so einschränken, dass sie nur Benutzer in ihrem Unternehmen oder ihrem Unternehmen und dem primären Unternehmen sehen. Informationen zur primären Unternehmensfunktionalität bezüglich des Datenschutzes für Benutzer finden Sie unter [Benutzerdefinierte Zugriffsebenen erstellen oder ändern](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
   * Benutzer können die Aktualisierungen, die sie an Elementen vornehmen, so beschränken, dass sie nur für ihre Benutzer im Unternehmen sichtbar sind. Weitere Informationen dazu, wie Sie eine Aktualisierung für ein Unternehmen privat machen, finden Sie unter [Update der Arbeit](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

## Erstellen oder bearbeiten Sie ein Unternehmen in [!DNL Workfront] {#create-or-edit-a-company-in-workfront}

Die Anzahl der Unternehmen, die Sie hinzufügen können, ist unbegrenzt. Es wird jedoch empfohlen, die Anzahl der von Ihnen verwendeten Unternehmen aufgrund von Problemen zu begrenzen, die bei Objektberechtigungen auftreten können. Eine zu starke Fragmentierung kann die Sichtbarkeit der Benutzer auf Arbeitselemente beeinträchtigen.

Standardmäßig ist das Unternehmen mit Ihrer Instanz von [!DNL Workfront] bereits in Ihrer [!DNL Workfront] und ist das Primäre Unternehmen für Ihre Organisation. Sie hat denselben Namen wie Ihr Kundenname. Weitere Informationen zu Ihren Kundeninformationen finden Sie unter [!DNL Workfront], siehe [Grundlegende Informationen für Ihr System konfigurieren](../../../administration-and-setup/get-started-wf-administration/configure-basic-info.md).

So fügen Sie ein Unternehmen hinzu oder bearbeiten es:

{#step-1-to-setup}

1. Klicks **[!UICONTROL Unternehmen]**.

   Eine Liste der Unternehmen wird angezeigt.
1. Wenn Sie ein Unternehmen hinzufügen, klicken Sie auf **[!UICONTROL Neue Firma]**.

   Oder

   Wenn Sie ein vorhandenes Unternehmen bearbeiten, wählen Sie das Unternehmen aus und klicken Sie auf **[!UICONTROL Bearbeiten]** oben in der Unternehmensliste.

1. Aktualisieren Sie die folgenden Informationen:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Abschnitt "Grundlegende Informationen"</td> 
      <td> 
       <ul> 
        <li> <p><b>[!UICONTROL Firmenname]</b>: Geben Sie einen Namen für das Unternehmen ein.</p> </li> 
        <li> <p><b>[!UICONTROL ist aktiv]</b>: Wenn diese Option aktiviert ist, können Benutzer das Unternehmen suchen und es an Projekte anhängen, die sie erstellen und bearbeiten. Ein inaktives Unternehmen kann nicht an Projekte angehängt werden. Diese Option ist standardmäßig aktiviert.</p> </li> 
        <li> <p><b>[!UICONTROL Dies ist das Primäre Unternehmen]</b>: Weist das Unternehmen als Hauptunternehmen Ihres Unternehmens zu. Das primäre Unternehmen repräsentiert normalerweise Ihre [!DNL Workfront] -Konto, in dem die meisten Ihrer Benutzer arbeiten.</p> <p>Sie können ein Unternehmen oder kein Unternehmen als Hauptunternehmen festlegen, aber Sie können nicht mehrere Unternehmen als Primärunternehmen bestimmen lassen. Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> <p><b>NOTE</b>: Durch Änderung der Zugriffsebene können Sie Benutzer so einschränken, dass sie andere Benutzer sehen: nur in ihrem primären Unternehmen oder in ihrem verbundenen Unternehmen und dem primären Unternehmen. Informationen dazu, wie das primäre Unternehmen mit den Zugriffsebenen der Benutzer arbeitet, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </li> 
        <li> <p><b>[!UICONTROL Group]</b>: Wenn es eine Gruppe gibt, die mit dem Unternehmen Geschäfte tätigt, können Sie hier den Namen der Gruppe hinzufügen. Dies ist nützlich für Gruppenadministratoren, die über alle Unternehmen berichten und diese verwalten müssen, mit denen ihre Gruppen Geschäfte tätigen.</p> <p><b>WICHTIG</b>: Wenn Sie die Gruppe, die mit diesem Unternehmen zusammenarbeitet, nicht zuordnen, können Administratoren der Gruppe nur dann auf das Unternehmen zugreifen, wenn sie über Administratorzugriff auf Unternehmen in ihrer Zugriffsstufe verfügen. Informationen dazu, wie dieser Zugriff gewährt wird, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Benutzern administrativen Zugriff auf bestimmte Bereiche gewähren</a>.</p> <p data-mc-conditions="SnippetConditions-wf-groups.system-level">Geben Sie den Gruppennamen ein und drücken Sie dann die Eingabetaste <strong>[!UICONTROL Eingabe]</strong> angezeigt.</p> <p data-mc-conditions="SnippetConditions-wf-groups.system-level">Wenn Sie einer Firma eine Gruppe zuweisen, erhalten die Gruppenadministratoren für die Gruppe [!UICONTROL Manager] Zugriff auf das Unternehmen. Weitere Informationen finden Sie unter <a href="#group-administrators-and-companies" class="MCXref xref">Gruppenadministratoren und Unternehmen</a> in diesem Artikel.</p> </li> 
        <li> <p><b>[!UICONTROL Firmenmitglieder]</b>: Fügen Sie dem Unternehmen vorhandene Benutzer hinzu. Dadurch verknüpfen Sie diese Benutzer mit diesem Unternehmen.</p> <p>Es gibt keine Beschränkung dafür, wie viele Benutzer Sie mit einem Unternehmen verknüpfen, aber ein Benutzer kann nicht mit mehr als einem Unternehmen verknüpft werden.</p> </li> 
       </ul> </td> 
     </tr>
     <tr> 
      <td role="rowheader">Abschnitt "Benutzerdefinierter Forms"</td> 
      <td> <p>Wenn es Felder gibt, die Sie Ihrem Unternehmen hinzufügen möchten, die in nicht verfügbar sind. [!DNL Workfront]können Sie ein benutzerdefiniertes Formular erstellen und es mit Ihrem Unternehmen verknüpfen. </p> <p>Sie können dieses Formular an Ihr Unternehmen anhängen, indem Sie es aus dem Dropdown-Menü auswählen. Im Menü werden nur aktive benutzerdefinierte Formulare aufgeführt.</p> <p><span class="preview"><strong>Hinweis:</strong> Erweiterte benutzerdefinierte Formularfunktionen wie externe Suchfelder und native Workfront-Felder sind nur verfügbar, wenn Sie den Firmendatensatz auf der Detailseite und nicht im Dialogfeld Unternehmen bearbeiten öffnen. (Klicken Sie in der Liste der Unternehmen auf den Unternehmensnamen, um die Details zu öffnen.)</span></p> <p> Informationen zum Erstellen benutzerdefinierter Formulare finden Sie unter <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">Benutzerdefiniertes Formular erstellen oder bearbeiten</a>. </p> </td>
     </tr> 
    </tbody> 
   </table>

1. (Bedingt) Klicken Sie beim Erstellen eines Unternehmens auf **[!UICONTROL Unternehmen erstellen]**.

   Oder

   Wenn Sie ein vorhandenes Unternehmen bearbeiten, klicken Sie auf **[!UICONTROL Änderungen speichern]**.

## Verwalten von Firmenmitgliedschaften

Informationen zur Verwaltung von Mitgliedschaften für ein bestehendes Unternehmen finden Sie unter [Verwalten von Firmenmitgliedschaften](../../../administration-and-setup/set-up-workfront/organizational-setup/manage-company-memberships.md).

## Rechnungssätze verwalten

Informationen zum Außerkraftsetzen der Abrechnungssätze auf Unternehmensebene finden Sie unter [Außerkraftsetzen der Abrechnungssätze für Stellenangebote auf Unternehmensebene](/help/quicksilver/administration-and-setup/set-up-workfront/organizational-setup/override-job-role-billing-rates-company-level.md).

## Übersicht über die Freigabe von Objekten für Unternehmen

Bestimmte Berechtigungen stehen Benutzern zur Verfügung, die mit einem Unternehmen verbunden sind, wie im Abschnitt beschrieben [Vorteile beim Hinzufügen von Benutzern zu einem Unternehmen](#benefits-of-adding-users-to-a-company). Zusätzlich zu diesen Berechtigungen können Sie Benutzern Berechtigungen erteilen, Objekte in der [!DNL Workfront] , indem Sie das Objekt für das Unternehmen freigeben.

Anstatt ein Objekt für einen einzelnen Benutzer freizugeben, können Sie es für das gesamte Unternehmen freigeben. Jeder Benutzer im Unternehmen verfügt über die gleichen Berechtigungen für dieses Objekt.

Weitere Informationen zum Freigeben von Objekten finden Sie unter [Übersicht über die Freigabe von Berechtigungen für Objekte](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

## Gruppenadministratoren und Unternehmen {#group-administrators-and-companies}

Wenn eine [!DNL Workfront] Administrator weist einem Unternehmen eine Gruppe zu, die Gruppenadministratoren für die Gruppe gewinnen [!UICONTROL Verwalten] Zugang zum Unternehmen in [!UICONTROL Einrichtung]. Dazu gehört auch der Zugriff auf die [!UICONTROL Unternehmen] Seite in [!UICONTROL Einrichtung], wo sie das mit ihrer Gruppe verbundene Unternehmen sehen und verwalten können.

Mit diesem Zugriff auf [!UICONTROL Unternehmen] -Seite kann ein Gruppenadministrator einem Unternehmen eine Gruppe zuweisen, es muss jedoch ein Unternehmen sein, das der Gruppenadministrator erstellt hat. Wenn die Zugriffsebene des Gruppenadministrators nicht mit Administratorzugriff auf Unternehmen konfiguriert ist, wird die [!UICONTROL Gruppe] -Feld ist erforderlich, wenn der Gruppenadministrator das Unternehmen erstellt. Der fettgedruckte Titel gibt Folgendes an:

![Unternehmen bearbeiten](assets/group-admin-add-company.png)

Informationen dazu, wie Benutzer administrativen Zugriff auf Unternehmen in ihrer Zugriffsebene erhalten, finden Sie unter [Benutzern administrativen Zugriff auf bestimmte Bereiche gewähren](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

Informationen zum Verwalten eines Unternehmens finden Sie im [!UICONTROL Einrichtung] -Bereich, siehe [Erstellen oder bearbeiten Sie ein Unternehmen in [!DNL Workfront]](#create-or-edit-a-company-in-workfront) in diesem Artikel.
