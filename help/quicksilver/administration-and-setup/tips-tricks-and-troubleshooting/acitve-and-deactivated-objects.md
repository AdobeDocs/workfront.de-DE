---
user-type: administrator
content-type: reference
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: Aktive und deaktivierte Objekte
description: Als [!DNL Adobe Workfront] Administrator können Sie Objekte im System aktivieren oder deaktivieren. Es wird empfohlen, die Objekte, die Sie deaktivieren können, niemals zu löschen. Sie sollten das Objekt einfach deaktivieren, um eine zukünftige Verwendung zu verhindern und es aus den Dropdown-Menüs anderer Objekte zu entfernen.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: a0617270-e233-4ebe-a5ee-8df7a8a85823
source-git-commit: 307bfb397555c7f9d424e429785dae36c639756a
workflow-type: tm+mt
source-wordcount: '750'
ht-degree: 2%

---

# Aktive und deaktivierte Objekte

Als [!DNL Adobe Workfront] -Administrator können Sie Objekte im System aktivieren oder deaktivieren. Es wird empfohlen, die Objekte, die Sie deaktivieren können, niemals zu löschen. Sie sollten das Objekt einfach deaktivieren, um eine zukünftige Verwendung zu verhindern und es aus den Dropdown-Menüs anderer Objekte zu entfernen.

Um beispielsweise einen bestimmten [!UICONTROL Stunden-Typ] anzuzeigen, muss der [!UICONTROL Stunden-Typ] aktiv sein. Ein inaktiver oder deaktivierter [!UICONTROL Stunden-Typ] wird nicht im Dropdown-Menü [!UICONTROL Stündentyp] angezeigt, bleibt jedoch im System, um den historischen Datensatz beizubehalten, in dem dieser [!UICONTROL Stündentyp] in der Vergangenheit verwendet wurde.

Der Begriff &quot;Aktiv&quot;wird verwendet, um zu ermitteln, ob bestimmte Objekte im System aktiviert sind. In diesem Zusammenhang wird &quot;Aktiv&quot;für die folgenden Objekte verwendet:

## E-Mail-Benachrichtigungen

Sie können E-Mail-Benachrichtigungen aktivieren, um bestimmte Aktionen zum Trigger von E-Mail-Benachrichtigungen für alle Benutzer zu ermöglichen.

Informationen zum Aktivieren oder Deaktivieren von E-Mail-Benachrichtigungen finden Sie unter [Ereignisbenachrichtigungen für alle Benutzer im System konfigurieren](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

## Stundentypen

Sie können Stundentypen aktivieren, damit sie von Benutzern bei der Protokollierung ausgewählt werden können.

Informationen zum Aktivieren oder Deaktivieren von Stundentypen finden Sie unter [Verwalten von Stundentypen](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/hour-types.md).

## Portfolios

Ein Portfolio muss aktiv sein, damit es im Formular [!UICONTROL Neues Projekt (Geschäftsszenario)] angezeigt wird.

Sie können ein Portfolio beim Bearbeiten des Portfolios aktivieren.

Informationen zum Bearbeiten von Portfolios finden Sie unter [Erstellen eines Portfolios](../../manage-work/portfolios/create-and-manage-portfolios/create-portfolios.md).

## Programme

Ein Programm muss aktiv sein, damit es für ein Projekt im Feld [!UICONTROL Programm] angezeigt wird.

Sie können ein Programm während der Bearbeitung des Programms aktivieren.

Weitere Informationen zum Bearbeiten von Programmen finden Sie unter [Programm erstellen](../../manage-work/portfolios/create-and-manage-programs/create-program.md).

## Vorlagen

Eine Vorlage muss aktiv sein, damit sie im Feld Vorlage für ein Projekt angezeigt wird.

Sie können eine Vorlage beim Bearbeiten der Vorlage aktivieren.

Weitere Informationen zum Bearbeiten von Vorlagen finden Sie unter [Bearbeiten von Projektvorlagen](../../manage-work/projects/create-and-manage-templates/edit-templates.md).

## Genehmigungsprozesse

Ein Genehmigungsprozess muss aktiv sein, damit im Feld [!UICONTROL Validierungsprozess] für ein Projekt, eine Aufgabe oder ein Problem angezeigt wird.

Sie können einen Genehmigungsprozess während der Bearbeitung des Genehmigungsprozesses aktivieren.

Informationen zum Bearbeiten von Genehmigungsprozessen finden Sie unter [Erstellen eines Genehmigungsprozesses für Arbeitselemente](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

## Milestone-Pfade

Ein Meilensteinpfad muss aktiv sein, damit er im Feld [!UICONTROL Meilensteinpfad] für ein Projekt angezeigt wird.

Sie können einen Meilensteinpfad beim Bearbeiten des Meilensteinpfads aktivieren.

Weitere Informationen zum Bearbeiten von Meilensteinpfaden finden Sie unter [Erstellen eines Meilensteinpfads](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md).

## Benutzerdefinierte Formulare

Ein benutzerdefiniertes Formular muss aktiv sein, damit es im Feld [!UICONTROL Benutzerdefiniertes Formular] für ein anderes Objekt angezeigt wird.

Sie können ein benutzerdefiniertes Formular beim Bearbeiten des benutzerdefinierten Formulars aktivieren.

Informationen zum Bearbeiten benutzerdefinierter Formulare und eine Liste von Objekten, mit denen Sie sie verknüpfen können, finden Sie unter [Entwerfen eines Formulars mit dem Formularentwickler](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

## Firmen

Ein Unternehmen muss aktiv sein, damit es für ein Projekt, einen Benutzer oder eine Vorlage im Feld [!UICONTROL Firma] angezeigt wird.

Sie können ein Unternehmen während der Bearbeitung des Unternehmens aktivieren lassen.

Weitere Informationen finden Sie unter [Erstellen und Bearbeiten von Unternehmen](../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

## Benutzende

Ein Benutzer muss aktiv sein, damit er bei der Zuweisung oder Freigabe in allen Typvorlagenfeldern aller anderen Objekte angezeigt wird.

Sie können Benutzer von der Benutzerseite aus oder während der Bearbeitung eines Benutzers deaktivieren.

Informationen zum Deaktivieren von Benutzern finden Sie unter [Deaktivieren oder Reaktivieren eines Benutzers](../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md).

>[!IMPORTANT]
>
>Wenn Ihr Unternehmen in den [!DNL Adobe Business Platform] integriert wurde, müssen Sie Benutzer über den [!UICONTROL Adobe Admin Console] deaktivieren.
>
>Anweisungen zum Deaktivieren eines Benutzers in der [!UICONTROL Adobe Admin Console] finden Sie im Abschnitt &quot;Benutzer entfernen&quot;im Artikel [Benutzer einzeln verwalten](https://helpx.adobe.com/enterprise/using/manage-users-individually.html) oder wenden Sie sich an Ihren [!UICONTROL Adobe Admin Console]-Administrator.
>
>Eine Liste der Vorgehensweisen, die sich je nachdem, ob Ihr Unternehmen in den [!DNL Adobe Business Platform] integriert wurde, unterscheiden, finden Sie unter [Plattformbasierte Verwaltungsunterschiede (Adobe Workfront/Adobe Business Platform)](../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

## Teams

Ein Team muss aktiv sein, damit es bei der Zuweisung oder Freigabe in allen anderen Objekten in allen Typ-Ahead-Feldern angezeigt wird.

Sie können Teams deaktivieren, wenn Sie ein Team bearbeiten.

Weitere Informationen zum Deaktivieren von Teams finden Sie unter [Deaktivieren eines Teams](../../people-teams-and-groups/create-and-manage-teams/deactivate-a-team.md).

## Aufgabengebiete

Eine Auftragsrolle muss aktiv sein, damit sie bei der Zuweisung oder Freigabe in allen Typvorlagenfeldern aller anderen Objekte angezeigt wird.

Sie können Auftragsrollen deaktivieren, wenn Sie sie bearbeiten.

Weitere Informationen zum Deaktivieren von Vorgangsrollen finden Sie unter [Deaktivieren von Vorgangsrollen](../../administration-and-setup/set-up-workfront/organizational-setup/deactivate-job-roles.md).

