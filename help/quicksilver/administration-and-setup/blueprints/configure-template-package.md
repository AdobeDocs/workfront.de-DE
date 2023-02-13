---
user-type: administrator
product-area: system-administration;workfront-integrations
navigation-topic: best-practices-catalog
title: Blueprint konfigurieren
description: Sie können Details der Projektvorlage oder der Organisationsstruktur konfigurieren, bevor Sie den Blueprint installieren.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: df10bc8f-b980-4c61-ae6d-bcea03103738
source-git-commit: d46eb98c443a421f340b1021972ddb89eda1966b
workflow-type: tm+mt
source-wordcount: '1824'
ht-degree: 0%

---

# Blueprint konfigurieren

Sie können Details eines Blueprints konfigurieren, bevor Sie ihn installieren. Projektvorlagen und Blueprint-Typen für die Organisationsstruktur erfordern in der Regel, dass einige Voreinstellungen festgelegt und einige Eigenschaften zugeordnet werden. Andere Blueprint-Typen müssen möglicherweise nicht konfiguriert werden, und Sie installieren sie unverändert. Weitere Informationen zur Installation finden Sie unter [Blueprint installieren](/help/quicksilver/administration-and-setup/blueprints/blueprints-install.md).

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] Plan</strong></td>
   <td>Beliebig</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe [!DNL Workfront] Lizenz</strong></td>
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Konfigurationen auf Zugriffsebene</strong></td>
   <td> <p>[!UICONTROL Systemadministrator]</p> </td> 
  </tr> 
 </tbody> 
</table>

## Projektvorlagen-Blueprint konfigurieren

1. Suchen Sie den gewünschten Blueprint.
1. Klicken **[!UICONTROL Installieren]** und wählen Sie dann eine Umgebung aus:

   <table style="table-layout:auto">
        <tr>
        <td><strong>Produktion</strong></td>
        <td>Die Produktion ist Ihre Live-Umgebung.</td>
    </tr>
    <tr>
        <td><strong>Sandbox-Vorschau</strong></td>
        <td>Die Sandbox-Vorschau ist eine Testumgebung, die als Replikation Ihrer Live-Umgebung dient und an jedem Wochenende von Workfront aktualisiert wird.</td>
    </tr>
    <tr>
        <td><strong>Sandbox 1 &amp; 2</strong></td>
        <td>Die Sandbox für benutzerdefinierte Aktualisierungen ist eine separate Testumgebung, die von Ihnen manuell aktualisiert wird. Es fallen zusätzliche Kosten an, um die Sandbox für benutzerdefinierte Aktualisierung zu erhalten.</td>
    </tr>
   </table>

1. Fahren Sie mit den folgenden Abschnitten fort:

   * [[!UICONTROL Vorlagenvoreinstellungen]](#template-preferences)
   * [[!UICONTROL Rollenzuordnung]](#role-mapping)
   * [[!UICONTROL Team-Mapping]](#team-mapping)
   * [[!UICONTROL Firmenzuordnung]g](#company-mapping)
   * [[!UICONTROL Gruppenzuordnung]](#group-mapping)

## [!UICONTROL Vorlagenvoreinstellungen] {#template-preferences}

Wählen Sie aus, wie die Vorlage installiert werden soll.

Sie können vor der Installation des Blueprints auch den Vorlagenbesitz festlegen. Sie können Änderungen an diesen Feldern vornehmen, nachdem die Vorlage installiert wurde. Weitere Informationen finden Sie unter [Bearbeiten von Projektvorlagen](../../manage-work/projects/create-and-manage-templates/edit-templates.md).

![[!UICONTROL Vorlageneinstellungen] Abschnitt](assets/Blueprints_TemplatePreferences.png)

1. Im [!UICONTROL Vorlageneinstellungen] geben Sie einen neuen Vorlagennamen an.
1. Geben Sie Folgendes an:

   <table style="table-layout:auto">
    <tr>
        <td><strong>[!UICONTROL Vorlageneigentümer]<strong></td>
        <td>Diese Person erhält [!UICONTROL Manager] -Berechtigungen für die Vorlage und wird zum Projekteigentümer, wenn die Vorlage zum Erstellen eines Projekts verwendet wird.</td>
    </tr>
    <tr>
        <td><strong>[!UICONTROL Vorlagen-Sponsor]</strong></td>
        <td>Diese Person ist in der Regel ein Manager, Führungskräfte oder Interessenträger, der wissen muss, was mit dem Projekt geschieht. Der Projektsponsor erhält keinen zusätzlichen Zugriff auf das Projekt, wird aber zu den E-Mail-Benachrichtigungen für das Projekt hinzugefügt.</td>
    </tr>
    <tr>
        <td><strong>[!UICONTROL Portfolio]</strong></td>
        <td>Dies ist das Portfolio, zu dem das Projekt bei seiner Erstellung gehören wird.</td>
    </tr>
    <tr>
        <td><strong>[!UICONTROL Programm]</strong></td>
        <td>Dies ist das Programm, zu dem das Projekt bei seiner Erstellung gehören wird.</td>
    </tr>
   </table>

1. Wählen Sie aus, ob die Vorlage als aktiv oder inaktiv installiert ist.
1. Wählen Sie aus, ob Sie definierte neue Ausgabevoreinstellungen verwenden möchten, sofern Voreinstellungen verfügbar sind.

   Klicken **[!UICONTROL Informationen zu den Problemeinstellungen]** , um die spezifischen Voreinstellungen zu überprüfen, die mit dem Blueprint installiert werden. Projekte, die aus der importierten Vorlage erstellt wurden, verwenden diese Voreinstellungen für neue Probleme, die im [!UICONTROL Probleme] Abschnitt.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Warteschlangen-Themen-Gruppen</strong></td> 
      <td> <p>Themengruppen in der Warteschlange definieren die höchste Ebene von Kategorien für die Probleme oder Anforderungen. Benutzer zeigen Themengruppen als Menüoptionen an, wenn sie auswählen, wo Anforderungen gesendet werden sollen. Eine Themengruppe kann mehrere Warteschlangenthemen enthalten. Weitere Informationen finden Sie unter <a href="../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md" class="MCXref xref">Themengruppen erstellen</a>. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Warteschlangen-Themen</strong></td> 
      <td> <p>Warteschlangenthemen funktionieren in Verbindung mit Routing-Regeln, um Probleme oder Anforderungen zuzuweisen. Dies sind die Menüoptionen, die Benutzer nach Auswahl einer Themengruppe auswählen, wenn sie ein Problem oder eine Anfrage eingeben. Weitere Informationen finden Sie unter <a href="../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md" class="MCXref xref">Erstellen von Warteschlangenthemen</a>. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Routing-Regeln</strong></td> 
      <td>Routing-Regeln senden Probleme oder Anforderungen an bestimmte Auftragsrollen , Benutzer oder Teams. Sie können die Anforderungen auch an bestimmte Projekte senden, die nicht mit der Anforderungswarteschlange verbunden sind. Weitere Informationen finden Sie unter <a href="../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md" class="MCXref xref">Erstellen von Routing-Regeln</a>. </td> 
     </tr> 
    </tbody> 
   </table>

   >[!INFO]
   >
   >**Beispiel:** Die neuen Ausgabevoreinstellungen in diesem Blueprint bieten vier Themen für die Warteschlange. Der Benutzer wählt beim Erstellen eines Problems eines dieser Themen aus. (Da nur eine Themengruppe existiert, wird sie automatisch angewendet und der Benutzer muss sie nicht auswählen.) Wenn der Benutzer das Problem abschließt und sendet, bestimmen Routing-Regeln, welcher Auftrags- oder Team-Rolle er zugewiesen ist.
   >![Beispiele für neue Problempräferenzen](assets/Blueprints_IssuePrefsDetails.png)
   >![Warteschlangenthemen für neues Problem](assets/blueprints-newissueqtopicsexample-350x204.png)
   >![Problem, das zur Stellenrolle weitergeleitet wird](assets/Blueprints_ProjectShowsIssueAssignment.png)

   >[!TIP]
   >
   >* Die Verwendung der Problemvoreinstellungen trägt dazu bei, die Konsistenz bei der Erfassung neuer Probleme oder Anforderungen in Ihren Projekten zu gewährleisten.
   >* Durch das Festlegen dieser Voreinstellungen werden die aus der Vorlage erstellten Projekte nicht automatisch in Anfragewarteschlangen umgewandelt. Informationen zum Einrichten einer Anforderungswarteschlange finden Sie unter [Erstellen einer Anforderungswarteschlange](../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).
   >* Nicht alle Blueprints enthalten neue Ausgabevoreinstellungen.



## [!UICONTROL Rollenzuordnung] {#role-mapping}

>[!NOTE]
>
>Dieser Abschnitt wird in einigen Blueprints möglicherweise nicht angezeigt.

Einige Vorlagen enthalten vorgeschriebene Vorgangsrollen. Mithilfe von Vorgangsrollen können Sie die richtigen Personen zuweisen, wenn die Vorlage in ein Projekt konvertiert wird. Sie können anpassen, wie Rollen zugeordnet werden, bevor Sie den Blueprint installieren. Klicken **[!UICONTROL Siehe Rollenbeschreibungen]** , um mehr über die im Blueprint verfügbaren Rollen zu erfahren.

Der Blueprint sucht nach dem Rollennamen, um zu sehen, ob vorhandene Rollen übereinstimmen. Bei der Suche wird zwischen Groß- und Kleinschreibung unterschieden. Daher müssen Namen exakt übereinstimmen. Wenn keine der vorhandenen Rollen übereinstimmt, können Sie sie vom Blueprint erstellen lassen.

![[!UICONTROL Rollenzuordnung] Abschnitt](assets/Blueprints_RoleMapping.png)

1. Wenn eine Rolle vorhanden ist, können Sie eine der folgenden Optionen auswählen:

   1. Erstellen Sie eine neue Rolle mit einem anderen Namen und geben Sie dann den Namen in das Textfeld ein.
   1. Verwenden Sie die vorhandene Rolle und wählen Sie dann im Auswahlfeld eine Rolle aus.
   1. Verwenden Sie keine zugeordnete Rolle. Diese Option wird nicht empfohlen, da einigen Aufgaben keine Rollen zugewiesen sind.

1. Wenn keine Rolle vorhanden ist, können Sie eine der folgenden Optionen auswählen:

   1. Erstellen Sie eine neue Rolle. Diese Option erstellt die Rolle, die der Blueprint empfiehlt.
   1. Erstellen Sie eine neue Rolle mit einem anderen Namen und geben Sie dann den Namen in das Textfeld ein.
   1. Verwenden Sie die vorhandene Rolle und wählen Sie dann im Auswahlfeld eine Rolle aus.
   1. Verwenden Sie keine zugeordnete Rolle. Diese Option wird nicht empfohlen, da einigen Aufgaben keine Rollen zugewiesen sind.

>[!NOTE]
>
>Der Installationsprozess wendet keine Rollen auf bestimmte Personen an. Sie sollten die Personen in diesen Rollen überprüfen, nachdem Sie die Blueprint-Lösung installiert haben, und bei Bedarf Personen zuweisen. Weitere Informationen finden Sie unter [Nach der Installation eines Blueprints zu ergreifende Maßnahmen](../../administration-and-setup/blueprints/best-next-actions-after-install.md).

Weitere Informationen zu den Vorgangsrollen in [!DNL Workfront], siehe [Erstellen und Verwalten von Vorgangsrollen](../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

## [!UICONTROL Team-Mapping] {#team-mapping}

>[!NOTE]
>
>Dieser Abschnitt wird in einigen Blueprints möglicherweise nicht angezeigt.

Einige Vorlagen enthalten vorgeschriebene Teams. Die einem Team zugewiesenen Arbeiten können von jedem beliebigen Team-Mitglied abgeschlossen werden. Sie können anpassen, wie Teams zugeordnet werden, bevor Sie den Blueprint installieren. Klicken **[!UICONTROL Siehe Teambeschreibungen]** um mehr über die im Blueprint verfügbaren Teams zu erfahren.

Der Blueprint sucht nach dem Teamnamen, um zu sehen, ob vorhandene Teams übereinstimmen. Bei der Suche wird zwischen Groß- und Kleinschreibung unterschieden. Daher müssen Namen exakt übereinstimmen. Wenn keine vorhandenen Teams übereinstimmen, können Sie sie mit dem Blueprint für Sie erstellen lassen.

![[!UICONTROL Team-Zuordnung] Abschnitt](assets/Blueprints_TeamMapping.png)

1. Wenn ein Team vorhanden ist, können Sie eine der folgenden Optionen auswählen:

   1. Erstellen Sie ein neues Team mit einem anderen Namen und geben Sie dann den Namen in das Textfeld ein.
   1. Verwendung [!UICONTROL vorhandenes Team]und wählen Sie dann ein Team im Auswahlfeld aus.
   1. Verwenden Sie kein zugeordnetes Team. Diese Option wird nicht empfohlen, da für einige Aufgaben keine Teams zugewiesen sind.

1. Wenn kein Team vorhanden ist, können Sie eine der folgenden Optionen auswählen:

   1. Erstellen Sie ein neues Team. Mit dieser Option wird das Team erstellt, das der Blueprint empfiehlt.
   1. Erstellen Sie ein neues Team mit einem anderen Namen und geben Sie dann den Namen in das Textfeld ein.
   1. Verwendung [!UICONTROL vorhandenes Team]und wählen Sie dann ein Team im Auswahlfeld aus.
   1. Verwenden Sie kein zugeordnetes Team. Diese Option wird nicht empfohlen, da für einige Aufgaben keine Teams zugewiesen sind.

>[!NOTE]
>
>Der Installationsprozess fügt den Teams keine Personen hinzu. Sie sollten die Mitarbeiter der Teams nach der Installation der Blueprint-Lösung überprüfen und bei Bedarf Personen zuweisen. Weitere Informationen finden Sie unter [Nach der Installation eines Blueprints zu ergreifende Maßnahmen](../../administration-and-setup/blueprints/best-next-actions-after-install.md).

Weitere Informationen zur Funktionsweise von Teams finden Sie in [!DNL Workfront], siehe [Erstellen und Verwalten von Teams](../../people-teams-and-groups/create-and-manage-teams/create-and-mange-teams.md).

## Unternehmenszuordnung {#company-mapping}

>[!NOTE]
>
>Dieser Abschnitt wird in einigen Blueprints möglicherweise nicht angezeigt.

Einige Blueprints umfassen verschriebene Unternehmen. Ein Unternehmen ist eine Organisationseinheit, die Ihre Organisation, eine Abteilung innerhalb der Organisation oder einen Kunden, mit dem Sie arbeiten, repräsentieren kann. Sie können anpassen, wie Unternehmen zugeordnet werden, bevor Sie den Blueprint installieren. Klicken **[!UICONTROL Siehe Unternehmensbeschreibungen]** um mehr über die Unternehmen zu erfahren, die im Blueprint verfügbar sind.

Der Blueprint sucht nach dem Unternehmensnamen, um zu sehen, ob vorhandene Unternehmen übereinstimmen. Bei der Suche wird zwischen Groß- und Kleinschreibung unterschieden. Daher müssen Namen exakt übereinstimmen. Wenn keine bestehenden Unternehmen übereinstimmen, können Sie sie mit dem Blueprint für Sie erstellen lassen. Das primäre Unternehmen im Blueprint wird dem primären Unternehmen in Ihrer Umgebung zugeordnet, auch wenn es nicht denselben Namen hat.

![[!UICONTROL Unternehmenszuordnung] Abschnitt](assets/Blueprints_CompanyMapping.png)

1. Wenn ein Unternehmen existiert, können Sie eine der folgenden Optionen auswählen:

   1. Erstellen Sie ein neues Unternehmen mit einem anderen Namen und geben Sie dann den Namen in das Textfeld ein.
   1. Verwenden Sie ein bestehendes Unternehmen und wählen Sie dann im Auswahlfeld ein Unternehmen aus.\

      Das primäre Unternehmen im Blueprint wird dem primären Unternehmen in Ihrer Umgebung zugeordnet, auch wenn es nicht denselben Namen hat.
   1. Verwenden Sie kein zugeordnetes Unternehmen. Diese Option wird nicht empfohlen, da die Unternehmensreferenzen in anderen Objekten leer sind.

1. Wenn kein Unternehmen existiert, können Sie eine der folgenden Optionen auswählen:

   1. Neue Firma erstellen. Mit dieser Option wird das Unternehmen erstellt, das der Blueprint empfiehlt.
   1. Erstellen Sie ein neues Unternehmen mit einem anderen Namen und geben Sie dann den Namen in das Textfeld ein.
   1. Verwenden Sie ein bestehendes Unternehmen und wählen Sie dann im Auswahlfeld ein Unternehmen aus.
   1. Verwenden Sie kein zugeordnetes Unternehmen. Diese Option wird nicht empfohlen, da die Unternehmensreferenzen in anderen Objekten leer sind.

>[!NOTE]
>
>Informationen zum Konfigurieren der Unternehmen nach der Installation des Blueprints finden Sie unter [Nach der Installation eines Blueprints zu ergreifende Maßnahmen](../../administration-and-setup/blueprints/best-next-actions-after-install.md).

Informationen zum Verknüpfen einer Vorlage mit einem Unternehmen finden Sie unter [Bearbeiten von Projektvorlagen](../../manage-work/projects/create-and-manage-templates/edit-templates.md).

Informationen zur Funktionsweise von Unternehmen in [!DNL Workfront], siehe [Erstellen und Bearbeiten von Unternehmen](../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

## [!UICONTROL Gruppenzuordnung] {#group-mapping}

>[!NOTE]
>
>Dieser Abschnitt wird in einigen Blueprints möglicherweise nicht angezeigt.

Einige Blueprints enthalten verschriebene Gruppen. Eine Gruppe ist eine Benutzergruppe, die mit Ihrer Abteilungsstruktur übereinstimmt. Gruppen sind ähnlich, unterscheiden sich aber von Teams und Unternehmen in Workfront. Sie können anpassen, wie Gruppen zugeordnet werden, bevor Sie den Blueprint installieren. Klicken **[!UICONTROL Siehe Gruppenbeschreibungen]** um mehr über die Gruppen zu erfahren, die im Blueprint verfügbar sind.

Der Blueprint sucht nach dem Gruppennamen, um zu sehen, ob vorhandene Gruppen übereinstimmen. Bei der Suche wird zwischen Groß- und Kleinschreibung unterschieden. Daher müssen Namen exakt übereinstimmen. Wenn keine vorhandenen Gruppen übereinstimmen, können Sie sie mit dem Blueprint erstellen lassen.

![[!UICONTROL Gruppenzuordnung] Abschnitt](assets/Blueprints_GroupMapping.png)

1. Wenn eine Gruppe vorhanden ist, können Sie **[!UICONTROL Remap-Gruppe]** und wählen Sie eine der folgenden Optionen:

   1. **[!UICONTROL Neue Gruppe mit einem anderen Namen erstellen]** und geben Sie dann den Namen ein, der dieser Gruppe zugewiesen werden soll. Verweise auf die Gruppe in der Blueprint-Definition werden stattdessen mit dieser neuen Gruppe verknüpft.
   1. **[!UICONTROL Ersetzen durch eine vorhandene Gruppe]**, suchen und wählen Sie dann eine Gruppe im Auswahlfeld aus.

      >[!NOTE]
      >
      >Eine bestehende Gruppe kann nicht umbenannt werden.

1. Wenn keine Gruppe vorhanden ist, können Sie:

   1. Ändern Sie den vorgeschlagenen Gruppennamen, indem Sie ihn in das Textfeld eingeben.
   1. Auswählen **[!UICONTROL Remap-Gruppe]** und wählen Sie [!UICONTROL Ersetzen durch eine vorhandene Gruppe], suchen und wählen Sie dann eine Gruppe im Auswahlfeld aus.
   1. Auswählen **[!UICONTROL Remap-Gruppe]** und wählen Sie **[!UICONTROL Unter einer vorhandenen Gruppe einfügen]**, suchen und wählen Sie dann eine Gruppe im Auswahlfeld aus. Mit dieser Option wird eine neue Untergruppe unter der vorhandenen Gruppe erstellt.

>[!NOTE]
>
>Informationen zum Konfigurieren der Gruppen nach der Installation des Blueprints finden Sie unter [Nach der Installation eines Blueprints zu ergreifende Maßnahmen](../../administration-and-setup/blueprints/best-next-actions-after-install.md).

Informationen zur Verwendung von Gruppen in [!DNL Workfront], siehe [Gruppenübersicht](../../administration-and-setup/manage-groups/groups-overview/groups.md).
