---
user-type: administrator
product-area: system-administration
navigation-topic: organization-setup
title: Erstellen und Bearbeiten von Unternehmen
description: Sie können Unternehmen zu [!DNL Adobe Workfront] hinzufügen und sie für Finanzplanungs- und Berichtszwecke verwenden, um Berechtigungen für Objekte zu definieren und Informationen vertraulich zu behandeln.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: bb597032-3395-4c9a-b622-5c920ba55131
source-git-commit: 1b3e0ab2d8ee37b7583d0b8fb0472b2fc9623da0
workflow-type: tm+mt
source-wordcount: '1473'
ht-degree: 0%

---

# Erstellen und Bearbeiten von Unternehmen

<!--Audited: 01/2024-->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

Ein Unternehmen ist eine Organisationseinheit in [!DNL Adobe Workfront] , die Ihre Organisation, eine Abteilung innerhalb der Organisation oder einen Kunden, mit dem Sie arbeiten, repräsentieren kann. Sie können Unternehmen zu [!DNL Workfront] hinzufügen und sie für Finanzplanungs- und Berichtszwecke verwenden, um Berechtigungen für Objekte zu definieren und Informationen vertraulich zu behandeln.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

Sie müssen über Folgendes verfügen, um Unternehmen in [!DNL Workfront] zu verwalten:

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
     <li> <p>Die Zugriffsstufe [!UICONTROL Systemadministrator], mit der Sie jedes Unternehmen im System bearbeiten können. Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md">Gewähren des vollen Administratorzugriffs für einen Benutzer</a>. </p> </li> 
     <li> <p>Verwaltungszugriff zur Verwaltung von Unternehmen, mit dem Sie jedes Unternehmen im System bearbeiten können. Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md">Gewähren von Benutzern administrativen Zugriff auf bestimmte Bereiche</a>.</p> </li> 
    </ul> <p><b>NOTE</b>:  
     <ul> 
      <li> <p>Sie können auch Unternehmen verwalten, die mit einer beliebigen Gruppe verbunden sind, der Sie als Gruppenadministrator zugewiesen sind.</p> </li> 
      <li> <p>Um Benutzer zum System [!DNL Workfront] hinzuzufügen und daraus zu entfernen, müssen Sie über einen der folgenden Schritte verfügen:</p> 
       <ul> 
        <li> <p>Die Zugriffsstufe des [!UICONTROL Systemadministrators]. Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Gewähren des vollen Administratorzugriffs für einen Benutzer</a>. </p> </li> 
        <li> <p>In Ihrer Zugriffsebene muss [!UICONTROL Bearbeiten] für die Einstellung [!UICONTROL Benutzer] ausgewählt sein. Außerdem müssen für die Einstellung [!UICONTROL Benutzer] unter [!UICONTROL Feinabstimmung Ihrer Einstellungen] <img src="assets/gear-icon-in-access-levels.png"> die Option [!UICONTROL Erstellen] und mindestens eine der beiden Optionen [!UICONTROL Benutzeradministrator] aktiviert sein. </p> <p> <img src="assets/access-req-users.png"> </p> <p>Wenn Sie die Option [!UICONTROL Benutzeradministrator (Gruppenbenutzer)] verwenden, müssen Sie Gruppenadministrator einer Gruppe sein, der der Benutzer angehört.</p> </li> 
       </ul> <p>Weitere Informationen zur Einstellung "Benutzer"auf einer Zugriffsebene finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Gewähren des Zugriffs für Benutzer</a>.</p> </li> 
     </ul> </p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren [!DNL Workfront] -Administrator, um herauszufinden, welche Konfigurationen für Plan, Lizenztyp oder Zugriffsstufe Sie haben. Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Vorteile beim Hinzufügen von Benutzern zu einem Unternehmen {#benefits-of-adding-users-to-a-company}

* Sie können das Organisationsdiagramm eines Unternehmens erstellen, indem Sie Benutzer direkten Berichten zuordnen. Nur Benutzer desselben Unternehmens können als direkte Berichte eines anderen Benutzers aus diesem Unternehmen hinzugefügt werden.
* Als Projektmanager können Sie verfügbare Ressourcen innerhalb desselben Unternehmens identifizieren.
* Sie können Informationen zwischen Unternehmen privat halten, indem Sie eine oder alle der folgenden Einstellungen auswählen:

   * Benutzer desselben Unternehmens können die Anforderungen der anderen Benutzer sehen.

     Weitere Informationen dazu, wie ein [!DNL Workfront] -Administrator ähnlichen Zugriff auf Anforderungen gewähren kann, die auf dem Unternehmen des Benutzers basieren, finden Sie im Abschnitt [Konfigurieren von Aufgaben und Problemeinstellungen für alle in [!DNL Workfront]](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md#changing-task-and-issue-preferences) im Artikel [Konfigurieren von systemweiten Aufgaben und Ausgabevoreinstellungen](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

     Weitere Informationen dazu, wie ein Gruppenadministrator ähnlichen Zugriff auf Anforderungen gewähren kann, die auf dem Unternehmen des Benutzers basieren, finden Sie unter [Konfigurieren von Aufgaben- und Problemeinstellungen für eine Gruppe](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

   * Benutzer können nur Anforderungswarteschlangen sehen, die mit ihren Unternehmen verknüpft sind. Weitere Informationen zum Einschränken der Sichtbarkeit einer Anforderungswarteschlange finden Sie unter [Zugriff auf Anforderungswarteschlangen bereitstellen](../../../manage-work/requests/create-and-manage-request-queues/provide-access-to-request-queues.md).
   * Sie können Benutzer so einschränken, dass sie nur Benutzer in ihrem Unternehmen oder ihrem Unternehmen und dem primären Unternehmen sehen. Informationen zur primären Unternehmensfunktionalität in Bezug auf den Datenschutz der Benutzer finden Sie unter [Benutzerdefinierte Zugriffsebenen erstellen oder ändern](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
   * Benutzer können die Aktualisierungen, die sie an Elementen vornehmen, so beschränken, dass sie nur für ihre Benutzer im Unternehmen sichtbar sind. Weitere Informationen dazu, wie Sie eine Aktualisierung für ein Unternehmen privat machen, finden Sie unter [Funktionsweise aktualisieren](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

## Erstellen oder Bearbeiten eines Unternehmens in [!DNL Workfront] {#create-or-edit-a-company-in-workfront}

Die Anzahl der Unternehmen, die Sie hinzufügen können, ist unbegrenzt. Es wird jedoch empfohlen, die Anzahl der von Ihnen verwendeten Unternehmen aufgrund von Problemen zu begrenzen, die bei Objektberechtigungen auftreten können. Eine zu starke Fragmentierung kann die Sichtbarkeit der Benutzer auf Arbeitselemente beeinträchtigen.

Standardmäßig ist das mit Ihrer Instanz von [!DNL Workfront] verknüpfte Unternehmen bereits in Ihrem [!DNL Workfront]-System erstellt und ist das Primäre Unternehmen für Ihr Unternehmen. Sie hat denselben Namen wie Ihr Kundenname. Weitere Informationen zu Ihren Kundeninformationen in [!DNL Workfront] finden Sie unter [Grundlegende Informationen für Ihr System konfigurieren](../../../administration-and-setup/get-started-wf-administration/configure-basic-info.md).

So fügen Sie ein Unternehmen hinzu oder bearbeiten es:

{#step-1-to-setup}

1. Klicken Sie auf **[!UICONTROL Unternehmen]**.

   Eine Liste der Unternehmen wird angezeigt.
1. Wenn Sie ein Unternehmen hinzufügen, klicken Sie auf **[!UICONTROL Neues Unternehmen]**.

   Oder

   Wenn Sie ein vorhandenes Unternehmen bearbeiten, wählen Sie das Unternehmen aus und klicken Sie dann oben in der Unternehmensliste auf **[!UICONTROL Bearbeiten]** .

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
        <li> <p><b>[!UICONTROL Ist aktiv]</b>: Wenn diese Option aktiviert ist, können Benutzer das Unternehmen suchen und es an Projekte anhängen, die sie erstellen und bearbeiten. Ein inaktives Unternehmen kann nicht an Projekte angehängt werden. Diese Option ist standardmäßig aktiviert.</p> </li> 
        <li> <p><b>[!UICONTROL Dies ist das Primäre Unternehmen]</b>: Weist das Unternehmen als Hauptunternehmen Ihres Unternehmens zu. Das primäre Unternehmen stellt normalerweise Ihr [!DNL Workfront] -Konto dar, in dem die meisten Ihrer Benutzer arbeiten.</p> <p>Sie können ein Unternehmen oder kein Unternehmen als Hauptunternehmen festlegen, aber Sie können nicht mehrere Unternehmen als Primärunternehmen bestimmen lassen. Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> <p><b>HINWEIS</b>: Durch Änderung der Zugriffsebene können Sie Benutzer so einschränken, dass sie andere Benutzer sehen: nur in ihrer primären Firma oder in ihrem verbundenen Unternehmen und dem primären Unternehmen. Informationen dazu, wie das primäre Unternehmen mit den Zugriffsebenen der Benutzer arbeitet, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </li> 
        <li> <p><b>[!UICONTROL Group]</b>: Wenn es eine Gruppe gibt, die mit dem Unternehmen Geschäfte tätigt, können Sie hier den Namen der Gruppe hinzufügen. Dies ist nützlich für Gruppenadministratoren, die über alle Unternehmen berichten und diese verwalten müssen, mit denen ihre Gruppen Geschäfte tätigen.</p> <p><b>WICHTIG</b>: Wenn Sie die Gruppe, die mit diesem Unternehmen zusammenarbeitet, nicht verknüpfen, können Administratoren für die Gruppe nur dann auf das Unternehmen zugreifen, wenn sie über Administratorzugriff auf Unternehmen in ihrer Zugriffsebene verfügen. Informationen dazu, wie dieser Zugriff gewährt wird, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Gewähren von Administratorzugriff für bestimmte Bereiche</a>.</p> <p data-mc-conditions="SnippetConditions-wf-groups.system-level">Geben Sie den Namen der Gruppe ein und drücken Sie dann <strong>[!UICONTROL Enter]</strong> , wenn sie angezeigt wird.</p> <p data-mc-conditions="SnippetConditions-wf-groups.system-level">Wenn Sie einer Firma eine Gruppe zuweisen, erhalten die Gruppenadministratoren für die Gruppe [!UICONTROL Manager] Zugriff auf das Unternehmen. Weitere Informationen finden Sie unter <a href="#group-administrators-and-companies" class="MCXref xref">Gruppenadministratoren und Unternehmen</a> in diesem Artikel.</p> </li> 
        <li> <p><b>[!UICONTROL Firmenmitglieder]</b>: Fügen Sie dem Unternehmen vorhandene Benutzer hinzu. Dadurch verknüpfen Sie diese Benutzer mit diesem Unternehmen.</p> <p>Es gibt keine Beschränkung dafür, wie viele Benutzer Sie mit einem Unternehmen verknüpfen, aber ein Benutzer kann nicht mit mehr als einem Unternehmen verknüpft werden.</p> </li> 
       </ul> </td> 
     </tr>
     <tr> 
      <td role="rowheader">Abschnitt "Benutzerdefinierter Forms"</td> 
      <td> <p>Wenn Sie Ihrem Unternehmen Felder hinzufügen möchten, die in [!DNL Workfront] nicht verfügbar sind, können Sie ein benutzerdefiniertes Formular erstellen und es mit Ihrem Unternehmen verknüpfen. </p> <p>Sie können dieses Formular an Ihr Unternehmen anhängen, indem Sie es aus dem Dropdown-Menü auswählen. Im Menü werden nur aktive benutzerdefinierte Formulare aufgeführt.</p> <p><strong>Hinweis:</strong> Erweiterte benutzerdefinierte Formularfunktionen wie externe Suchfelder und native Workfront-Felder sind nur verfügbar, wenn Sie den Firmendatensatz auf der Detailseite und nicht im Dialogfeld "Unternehmen bearbeiten"öffnen. (Klicken Sie in der Liste der Unternehmen auf den Unternehmensnamen, um die Details zu öffnen.)</p> <p> Informationen zum Erstellen benutzerdefinierter Formulare finden Sie unter <a href="/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md">Entwerfen eines Formulars mit dem Formularentwickler</a>. </p> </td>
     </tr> 
    </tbody> 
   </table>

1. (Bedingt) Wenn Sie ein Unternehmen erstellen, klicken Sie auf **[!UICONTROL Unternehmen erstellen]**.

   Oder

   Wenn Sie ein vorhandenes Unternehmen bearbeiten, klicken Sie auf **[!UICONTROL Änderungen speichern]**.

## Verwalten von Firmenmitgliedschaften

Informationen zum Verwalten von Mitgliedschaften für ein vorhandenes Unternehmen finden Sie unter [Verwalten von Unternehmensmitgliedschaften](../../../administration-and-setup/set-up-workfront/organizational-setup/manage-company-memberships.md).

## Rechnungssätze verwalten

Informationen zum Außerkraftsetzen der Abrechnungsraten auf Unternehmensebene finden Sie unter [Außerkraftsetzen der Abrechnungsraten für die Rolle des Auftrags auf Unternehmensebene](/help/quicksilver/administration-and-setup/set-up-workfront/organizational-setup/override-job-role-billing-rates-company-level.md).

## Übersicht über die Freigabe von Objekten für Unternehmen

Bestimmte Berechtigungen stehen Benutzern zur Verfügung, die mit einem Unternehmen verbunden sind, wie im Abschnitt [Vorteile beim Hinzufügen von Benutzern zu einem Unternehmen](#benefits-of-adding-users-to-a-company) beschrieben. Zusätzlich zu diesen Berechtigungen können Sie Benutzern die Berechtigung zum Anzeigen, Beitragen oder Bearbeiten von Objekten in [!DNL Workfront] gewähren, indem Sie das Objekt für ihr Unternehmen freigeben.

Anstatt ein Objekt für einen einzelnen Benutzer freizugeben, können Sie es für das gesamte Unternehmen freigeben. Jeder Benutzer im Unternehmen verfügt über die gleichen Berechtigungen für dieses Objekt.

Weitere Informationen zum Freigeben von Objekten finden Sie unter [Übersicht über die Freigabe von Berechtigungen für Objekte](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

## Gruppenadministratoren und Unternehmen {#group-administrators-and-companies}

Wenn ein [!DNL Workfront] -Administrator einer Firma eine Gruppe zuweist, erhalten die Gruppenadministratoren für die Gruppe [!UICONTROL Verwalten] Zugriff auf das Unternehmen in der [!UICONTROL Einrichtung]. Dazu gehört auch der Zugriff auf die Seite [!UICONTROL Unternehmen] im [!UICONTROL Setup], auf der sie das mit ihrer Gruppe verbundene Unternehmen sehen und verwalten können.

Mit diesem Zugriff auf die Seite [!UICONTROL Unternehmen] kann ein Gruppenadministrator einem Unternehmen eine Gruppe zuweisen. Es muss sich jedoch um ein Unternehmen handeln, das der Gruppenadministrator erstellt hat. Wenn die Zugriffsebene des Gruppenadministrators nicht mit Administratorzugriff auf Unternehmen konfiguriert ist, ist das Feld [!UICONTROL Gruppe] erforderlich, wenn der Gruppenadministrator das Unternehmen erstellt. Der fettgedruckte Titel zeigt Folgendes an:

![Unternehmen bearbeiten](assets/group-admin-add-company.png)

Informationen dazu, wie Benutzer administrativen Zugriff auf Unternehmen in ihrer Zugriffsebene erhalten, finden Sie unter [Gewähren von Benutzern administrativen Zugriff auf bestimmte Bereiche](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

Informationen zum Verwalten eines Unternehmens im Bereich [!UICONTROL Einrichten] finden Sie unter [Erstellen oder Bearbeiten eines Unternehmens in  [!DNL Workfront]](#create-or-edit-a-company-in-workfront) in diesem Artikel.
