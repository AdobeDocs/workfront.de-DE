---
user-type: administrator
product-area: system-administration
navigation-topic: organization-setup
title: Erstellen und Bearbeiten von Firmen
description: Sie können Firmen zu hinzufügen  [!DNL Adobe Workfront]  diese für Finanzplanung und Berichtszwecke verwenden, um Berechtigungen für Objekte zu definieren und Informationen vertraulich zu behandeln.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: bb597032-3395-4c9a-b622-5c920ba55131
source-git-commit: 15063d937a5ba9b5285c66a0987e8deea6cc6d74
workflow-type: tm+mt
source-wordcount: '1387'
ht-degree: 0%

---

# Unternehmen erstellen und bearbeiten

<!--Audited: 01/2024-->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

Ein Unternehmen ist eine Organisationseinheit in [!DNL Adobe Workfront], die Ihr Unternehmen, eine Abteilung innerhalb des Unternehmens oder einen Kunden, mit dem Sie zusammenarbeiten, repräsentieren kann. Sie können Unternehmen zu [!DNL Workfront] hinzufügen und sie für Finanzplanung und Berichtszwecke verwenden, um Berechtigungen für Objekte zu definieren und Informationen vertraulich zu behandeln.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Workfront] Packstück</p> </td> 
   <td><p>Beliebig</p></td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] Lizenz</p> </td> 
   <td><p>[!UICONTROL -Plan]</p>
   <p>[!UICONTROL Standard]</p>
   </td> 
  </tr> 
  <tr> 
   <td>Konfiguration der Zugriffsebene</td> 
   <td> <p>Sie müssen eine der folgenden Möglichkeiten haben:</p> 
    <ul> 
     <li> <p>Die Zugriffsebene [!UICONTROL Systemadministrator], mit der Sie jede Firma im System bearbeiten können.</p> </li> 
     <li> <p>Administrativer Zugriff auf die Verwaltung von Unternehmen, wodurch Sie jedes Unternehmen im System bearbeiten können.</p> </li> 
    </ul> <p><b>HINWEIS</b>:  
     <ul> 
      <li> <p>Sie können auch Firmen verwalten, die mit einer beliebigen Gruppe verknüpft sind, der Sie als Gruppenadministrator zugewiesen sind.</p> </li> 
      <li> <p>Um Benutzer zum [!DNL Workfront] hinzuzufügen oder daraus zu entfernen, benötigen Sie eine der folgenden Eigenschaften:</p> 
       <ul> 
        <li> <p>Zugriffsebene des [!UICONTROL Systemadministrators]. </p> </li> 
        <li> <p><b>[!UICONTROL Users]</b> Einstellung in der Zugriffsebene konfiguriert, um den[!UICONTROL Edit]<b>-Zugriff zu </b>, wobei <b>[!UICONTROL Create]</b> und mindestens eine der beiden <b>[!UICONTROL User Admin]</b> Optionen unter <b> </b>[!UICONTROL Feinabstimmung der Einstellungen]<img src="assets/gear-icon-in-access-levels.png"> aktiviert ist. </p> <p> <img src="assets/access-req-users.png"> </p> <p>Wenn <b>[!UICONTROL User Admin (Group Users)]</b> aktiviert ist, müssen Sie unter diesen beiden Optionen Gruppenadministrator einer Gruppe sein, in der der Benutzer Mitglied ist.</p> </li> 
       </ul>
       </li> 
     </ul> </p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Vorteile beim Hinzufügen von Benutzern zu einem Unternehmen {#benefits-of-adding-users-to-a-company}

* Sie können das Organigramm eines Unternehmens erstellen, indem Sie Benutzer mit direkt unterstellten Mitarbeitern verknüpfen. Nur Benutzer desselben Unternehmens können als direkt unterstellte Mitarbeiter eines anderen Benutzers dieses Unternehmens hinzugefügt werden.
* Als Projekt-Manager können Sie die verfügbaren Ressourcen innerhalb desselben Unternehmens identifizieren.
* Sie können Informationen zwischen Unternehmen vertraulich halten, indem Sie eine oder alle der folgenden Einstellungen auswählen:

   * Benutzer desselben Unternehmens können die Anfragen des jeweils anderen sehen.

     Weitere Informationen dazu, wie ein [!DNL Workfront]-Administrator ähnlichen Zugriff auf Anfragen gewähren kann, die auf dem Unternehmen des Benutzers basieren, finden Sie im Abschnitt [Konfigurieren von Voreinstellungen für Aufgaben und Probleme für alle in [!DNL Workfront]](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md#changing-task-and-issue-preferences) im Artikel [Konfigurieren von systemweiten Voreinstellungen für Aufgaben und Probleme](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

     Weitere Informationen dazu, wie ein Gruppenadministrator bzw. eine Gruppenadministratorin ähnlichen Zugriff auf Anfragen gewähren kann, die auf dem Unternehmen des Benutzers bzw. der Benutzerin basieren, finden Sie [Konfigurieren von Aufgaben- und Problemeinstellungen für eine Gruppe](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

   * Benutzende können nur Anforderungswarteschlangen sehen, die mit ihren Unternehmen verknüpft sind. Weitere Informationen zur Einschränkung der Sichtbarkeit einer Anfrage-Warteschlange finden Sie unter [Zugriff auf Anfrage-Warteschlangen gewähren](../../../manage-work/requests/create-and-manage-request-queues/provide-access-to-request-queues.md).
   * Sie können Benutzer so einschränken, dass sie nur Benutzer in ihrem Unternehmen oder ihrem Unternehmen und dem primären Unternehmen sehen. Informationen zur primären Unternehmensfunktion für den Datenschutz von Benutzern finden Sie unter [Erstellen oder Ändern benutzerdefinierter Zugriffsebenen](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
   * Benutzer können Aktualisierungen, die sie an Elementen vornehmen, darauf beschränken, dass sie nur für ihre Firmenbenutzer sichtbar sind. Weitere Informationen dazu, wie Sie eine Aktualisierung für eine Firma als privat festlegen, finden Sie unter [Arbeit aktualisieren](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

## Erstellen oder Bearbeiten eines Unternehmens in [!DNL Workfront] {#create-or-edit-a-company-in-workfront}

Die Anzahl der Unternehmen, die Sie hinzufügen können, ist unbegrenzt. Wir empfehlen jedoch, die Anzahl der von Ihnen verwendeten Unternehmen zu begrenzen, da Probleme mit Objektberechtigungen auftreten können. Eine zu starke Fragmentierung kann die Sichtbarkeit der Benutzer für Arbeitselemente beeinträchtigen.

Standardmäßig wird das mit Ihrer Instanz von [!DNL Workfront] verknüpfte Unternehmen bereits in Ihrem [!DNL Workfront] erstellt und ist das Primäre Unternehmen für Ihr Unternehmen. Sie hat denselben Namen wie Ihr Kundenname. Weitere Informationen zu Ihren Kundeninformationen in [!DNL Workfront] finden Sie unter [Konfigurieren grundlegender Informationen für Ihr System](../../../administration-and-setup/get-started-wf-administration/configure-basic-info.md).

So fügen Sie eine Firma hinzu oder bearbeiten sie:

{{step-1-to-setup}}

1. Klicken Sie auf **[!UICONTROL Firmen]**.

   Eine Liste der Unternehmen wird angezeigt.

1. Wenn Sie eine Firma hinzufügen möchten, klicken Sie auf **[!UICONTROL Neue Firma]**.

   Oder

   Wenn Sie eine vorhandene Firma bearbeiten, wählen Sie die Firma aus und klicken Sie dann oben in der Liste der Firmen auf **[!UICONTROL Bearbeiten]** Symbol ![Bearbeiten](assets/edit-icon.png).

1. Aktualisieren Sie die folgenden Informationen:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Abschnitt [!UICONTROL Basic Info]</td> 
      <td> 
       <ul> 
        <li> <p><b>[!UICONTROL Firmenname]</b>: Geben Sie einen Namen für das Unternehmen ein.</p> </li> 
        <li> <p><b>[!UICONTROL Ist Aktiv]</b>: Wenn diese Option aktiviert ist, können Benutzer das Unternehmen finden und es an Projekte anhängen, die sie erstellen und bearbeiten. Eine inaktive Firma kann nicht mit Projekten verknüpft werden. Standardmäßig ist diese Option aktiviert.</p> </li> 
        <li> <p><b>[!UICONTROL Dies ist die Primäre Firma]</b>: Weist die Firma als die primäre Firma Ihrer Organisation zu. Die primäre Firma stellt in der Regel Ihr [!DNL Workfront]-Konto dar, in dem die meisten Ihrer Benutzer arbeiten.</p> <p>Sie können eine Firma oder kein Unternehmen als Primärunternehmen festlegen, aber Sie können nicht mehrere Unternehmen als Primärunternehmen festlegen. Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Erstellen oder Ändern benutzerdefinierter Zugriffsebenen</a>.</p> <p><b>HINWEIS</b>: Durch Ändern ihrer Zugriffsebenen können Sie Benutzer darauf beschränken, andere Benutzer anzuzeigen: nur in ihrer primären Firma oder in ihrem zugehörigen Unternehmen und der primären Firma. Informationen dazu, wie das primäre Unternehmen mit den Zugriffsebenen von Benutzenden arbeitet, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Erstellen oder Ändern benutzerdefinierter Zugriffsebenen</a>.</p> </li> 
        <li> <p><b>[!UICONTROL Group]</b>: Wenn es eine Gruppe gibt, die mit dem Unternehmen Geschäfte macht, können Sie den Namen der Gruppe hier hinzufügen. Dies ist für Gruppenadministratoren nützlich, die Berichte über alle Unternehmen erstellen und diese verwalten müssen, mit denen ihre Gruppen Geschäfte machen.</p> <p><b>WICHTIG</b>: Wenn Sie die Gruppe, die mit dieser Firma arbeiten wird, nicht verknüpfen, können Administratoren für die Gruppe nicht auf die Firma zugreifen, es sei denn, sie haben administrativen Zugriff auf Unternehmen in ihrer Zugriffsebene. Weitere Informationen dazu, wie dieser Zugriff gewährt wird, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Gewähren von administrativem Zugriff für Benutzer auf bestimmte Bereiche</a>.</p> <p data-mc-conditions="SnippetConditions-wf-groups.system-level">Beginnen Sie, den Namen der Gruppe einzugeben, und drücken Sie dann <strong>[!UICONTROL Enter]</strong> wenn er erscheint.</p> <p data-mc-conditions="SnippetConditions-wf-groups.system-level">Wenn Sie einer Firma eine Gruppe zuweisen, erhalten die Gruppenadministratoren für die Gruppe [!UICONTROL Manage] Zugriff auf die Firma. Weitere Informationen finden Sie unter <a href="#group-administrators-and-companies" class="MCXref xref">Gruppenadministratoren und Unternehmen</a> in diesem Artikel.</p> </li> 
        <li> <p><b>[!UICONTROL Firmenmitglieder]</b>: Fügen Sie dem Unternehmen vorhandene Benutzer hinzu. Auf diese Weise verknüpfen Sie diese Benutzer mit dieser Firma.</p> <p>Es gibt keine Begrenzung dafür, wie viele Benutzer Sie mit einer Firma verknüpfen. Ein Benutzer kann jedoch nicht mit mehr als einer Firma verknüpft werden.</p> </li> 
       </ul> </td> 
     </tr>
     <tr> 
      <td role="rowheader">Abschnitt [!UICONTROL Custom Forms]</td> 
      <td> <p>Wenn es Felder gibt, die Sie Ihrer Firma hinzufügen möchten und die in [!DNL Workfront] nicht verfügbar sind, können Sie ein benutzerdefiniertes Formular erstellen und es mit Ihrer Firma verknüpfen. </p> <p>Sie können dieses Formular an Ihr Unternehmen anhängen, indem Sie es aus dem Dropdown-Menü auswählen. Im Menü werden nur aktive benutzerdefinierte Formulare aufgelistet.</p> <p><strong>Hinweis</strong> Erweiterte benutzerdefinierte Formularfunktionen wie externe Suchfelder und native Workfront-Felder sind nur verfügbar, wenn Sie den Firmendatensatz auf der Detailseite öffnen, nicht im Dialogfeld „Unternehmen bearbeiten“. (Klicken Sie in der Liste der Unternehmen auf den Firmennamen, um die Details zu öffnen.)</p> <p> Informationen zum Erstellen benutzerdefinierter Formulare finden Sie unter <a href="/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md">Erstellen eines benutzerdefinierten Formulars</a>. </p> </td>
     </tr> 
    </tbody> 
   </table>

1. (Bedingt) Wenn Sie eine Firma erstellen, klicken Sie auf **[!UICONTROL Firma erstellen]**.

   Oder

   Wenn Sie eine vorhandene Firma bearbeiten, klicken Sie auf **[!UICONTROL Änderungen speichern]**.

## Verwalten von Unternehmensmitgliedschaften

Informationen zum Verwalten von Mitgliedschaften für eine bestehende Firma finden Sie unter [Verwalten von Firmenmitgliedschaften](../../../administration-and-setup/set-up-workfront/organizational-setup/manage-company-memberships.md).

## Abrechnungssätze verwalten

Informationen zum Überschreiben von Abrechnungssätzen auf Firmenebene finden Sie unter [Überschreiben von Abrechnungssätzen für Aufgabengebiete auf Firmenebene](/help/quicksilver/administration-and-setup/set-up-workfront/organizational-setup/override-job-role-billing-rates-company-level.md).

## Übersicht über die Freigabe von Objekten für Unternehmen

Bestimmte Berechtigungen stehen Benutzern zur Verfügung, die mit einem Unternehmen verknüpft sind, wie im Abschnitt [Vorteile beim Hinzufügen von Benutzern zu einem Unternehmen](#benefits-of-adding-users-to-a-company) erläutert. Zusätzlich zu diesen Berechtigungen können Sie Benutzerinnen und Benutzern die Berechtigung erteilen, Objekte in [!DNL Workfront] anzuzeigen, beizutragen oder zu bearbeiten, indem Sie das Objekt für ihr Unternehmen freigeben.

Anstatt ein Objekt jeweils für einen einzelnen Benutzer freizugeben, können Sie es für das gesamte Unternehmen freigeben. Jeder Benutzer im Unternehmen verfügt über dieselben Berechtigungen für dieses Objekt.

Weitere Informationen zum Freigeben von Objekten finden Sie unter [Übersicht über Berechtigungen zum Freigeben von Objekten](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

## Gruppenadministratoren und Unternehmen {#group-administrators-and-companies}

Wenn ein [!DNL Workfront] eine Gruppe einem Unternehmen zuweist, erhalten die Gruppenadministratoren für die Gruppe [!UICONTROL Verwalten] Zugriff auf das Unternehmen in [!UICONTROL Setup]. Dazu gehört der Zugriff auf die [!UICONTROL Firmen] in [!UICONTROL Setup], wo sie das mit ihrer Gruppe verknüpfte Unternehmen sehen und verwalten können.

Mit diesem Zugriff auf die Seite [!UICONTROL Firmen] kann ein Gruppenadministrator eine Gruppe einem Unternehmen zuweisen, es muss jedoch ein Unternehmen sein, das der Gruppenadministrator erstellt hat. Wenn die Zugriffsebene des Gruppenadministrators nicht mit administrativem Zugriff auf Unternehmen konfiguriert ist, ist das Feld [!UICONTROL Gruppe] erforderlich, wenn der Gruppenadministrator die Firma erstellt - der fettgedruckte Titel zeigt dies an:

![Firma bearbeiten](assets/group-admin-add-company.png)

Informationen dazu, wie Benutzer administrativen Zugriff auf Unternehmen in ihrer Zugriffsebene erhalten, finden Sie unter [Gewähren von administrativem Zugriff für Benutzer auf bestimmte Bereiche](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

Informationen zum Verwalten eines Unternehmens im Bereich [!UICONTROL Setup] finden Sie unter [Erstellen oder Bearbeiten eines Unternehmens in [!DNL Workfront]](#create-or-edit-a-company-in-workfront) in diesem Artikel.
