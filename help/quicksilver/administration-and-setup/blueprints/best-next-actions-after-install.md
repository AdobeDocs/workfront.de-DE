---
user-type: administrator
content-type: reference
product-area: system-administration;workfront-integrations
navigation-topic: best-practices-catalog
title: Nach der Installation eines Blueprints auszuführende Aktionen
description: In diesem Artikel wird beschrieben, was Sie nach der Installation eines Blueprints tun sollten [!DNL Adobe Workfront]  um den Blueprint für Ihre Systembenutzer vollständig bereitzustellen.
author: Jenny
feature: System Setup and Administration
role: Admin
exl-id: 6e5da58f-105a-4edf-8fc1-65e8762d43c6
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '1135'
ht-degree: 0%

---

# Nach der Installation eines Blueprints auszuführende Aktionen

In diesem Artikel wird beschrieben, was Sie nach der Installation eines Blueprints tun sollten, [!DNL Adobe Workfront] den Blueprint den Systembenutzern vollständig bereitzustellen.

* [Empfehlungen für Projektvorlagen](#project-template-recommendations)
* [Empfehlungen zur Organisationsstruktur](#organizational-structure-recommendations)
* [Dashboard-Empfehlungen](#dashboard-recommendations)

## Empfehlungen für Projektvorlagen {#project-template-recommendations}

Dieser Abschnitt enthält Empfehlungen für die mit Ihren Blueprints installierten Projektvorlagen.

### Zuweisen von Benutzern zu neu erstellten Rollen und Teams {#assign-users-to-newly-created-roles-and-teams}

Den Rollen und/oder Teams, die während des Blueprint-Installationsprozesses erstellt wurden, sind nicht automatisch Benutzer zugeordnet. Ohne die Zuweisung von Benutzern zu den neu hinzugefügten Rollen oder Teams erstellen Sie Arbeit für eine Funktion, die niemand aufnimmt. In einigen Fällen müssen Sie möglicherweise neue Benutzer erstellen, um diese Rollen und Teams auszufüllen. Informationen zum Erstellen neuer Benutzer finden Sie unter [Benutzer hinzufügen](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

### Anwenden eines benutzerdefinierten Formulars auf die Vorlage und die Vorlagenaufgaben {#apply-a-custom-form-to-the-template-and-the-template-tasks}

Im Installationsprozess wird die Projektvorlage mit keinen benutzerdefinierten Formularen verknüpft. Wenn Ihre Projekte oder Aufgaben bestimmte Formulare oder Felder ausfüllen müssen, um Konsistenz in der Berichterstellung zu gewährleisten, oder wenn Ihr digitales Anfrageformular Felder enthält, die auf Projektebene beibehalten werden müssen, empfehlen wir, die Vorlage oder die Vorlagenaufgaben mit diesen Formularen zu verknüpfen. Weitere Informationen finden Sie unter [Hinzufügen eines benutzerdefinierten Formulars zu einem Objekt](../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

### Vorlagenaufgabe - Dauer und Aufwandsschätzungen aktualisieren {#update-template-task-duration-and-effort-estimates}

Jede Aufgabe in der Vorlage enthält eine geplante Dauer und eine geplante Aufwandsschätzung. Diese Schätzungen dienen als Ausgangspunkt für die Dauer und die für diese Aktivitäten aufgewendete Zeit. Die Fähigkeiten, Fähigkeiten und das Tempo Ihres Unternehmens sind jedoch einzigartig. Sie sollten die geschätzte Dauer und den geschätzten Aufwand jeder Aufgabe überprüfen, um sie an die Anforderungen Ihres Unternehmens anzupassen. Weitere Informationen finden Sie unter [Verwalten von Aufgabeninformationen im Bereich [!UICONTROL Übersicht über ] Aufgabendetails](../../manage-work/tasks/manage-tasks/task-information-in-overview.md).

### Meilensteinpfad und Meilensteine verknüpfen {#associate-a-milestone-path-and-milestones}

Im Installationsprozess wird die Projektvorlage nicht mit einem Meilensteinpfad verknüpft. Wenden Sie einen Meilensteinpfad auf die Vorlage an und wenden Sie Meilensteine auf wichtige Aufgaben in der Vorlage an, um Ihre Meilensteinberichte zu unterstützen. Weitere Informationen finden Sie unter [Zuordnen von Meilensteinen zu Aufgaben](../../manage-work/tasks/manage-tasks/associate-milestones-with-tasks.md).

### Rollout der Vorlage an Ihr Team {#roll-out-the-template-to-your-team}

Bereiten Sie Schulungsmaterialien für die beiden Arbeitsverantwortlichen vor, die diese Vorlage verwenden werden, sowie für die einzelnen Mitwirkenden, die die Arbeit innerhalb der Projektvorlage ausführen.

### Erstellen oder Aktualisieren von Berichten und Dashboards {#create-or-update-reports-and-dashboards}

Wenn es sich bei der Lösung um eine neue Art von Arbeit handelt, die Ihr Unternehmen zuvor noch nicht in [!DNL Workfront] ausgeführt hat, müssen Sie möglicherweise neue Berichte und Dashboards erstellen, um die Arbeit zu unterstützen. Weitere Informationen finden Sie unter [Erstellen eines benutzerdefinierten ](../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md) und [Erstellen eines Dashboards](../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md).

Wenn die Lösung der Arbeit ähnelt, die Sie bereits in [!DNL Workfront] ausgeführt haben, sollten Sie überprüfen, ob die Arbeit erwartungsgemäß in vorhandene Berichte und Dashboards einfließt. Wenn er nicht in Ihr vorhandenes Reporting einfließt, ergreifen Sie Maßnahmen, um Filter zu aktualisieren oder neue Berichte zu erstellen.

## Empfehlungen zur Organisationsstruktur {#organizational-structure-recommendations}

Dieser Abschnitt enthält Empfehlungen für die mit Ihren Blueprints installierten Organisationselemente.

### Firmen

Nach der Installation eines Blueprints, der ein Unternehmen enthält:

* Fügen Sie ein benutzerdefiniertes Formular hinzu, um den Firmendatensatz um nützliche Details zu ergänzen (das Formular und die zugehörigen Details sind für Sie eindeutig). Weitere Informationen finden Sie unter [Hinzufügen eines benutzerdefinierten Formulars zu einem Objekt](../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).
* Wenn die Firma einen Kunden repräsentiert, überprüfen Sie die Überschreibungsraten, die mit der Firma verbunden sind. Weitere Informationen finden Sie unter [Überschreiben von Abrechnungssätzen für Aufgabengebiete auf Unternehmensebene](../../administration-and-setup/set-up-workfront/organizational-setup/override-job-role-billing-rates-company-level.md).
* Wenn das Unternehmen einen Kunden repräsentiert und es andere Projektvorlagen gibt, die eindeutig für diese Organisation sind, verknüpfen Sie die Projektvorlagen zunächst mit dem neu hinzugefügten Unternehmen. Weitere Informationen finden Sie unter [Projektvorlagen bearbeiten](../../manage-work/projects/create-and-manage-templates/edit-templates.md).
* Wenn das Unternehmen einen Kunden oder einen Anbieter vertritt, verknüpfen Sie bestehende Benutzer der externen Organisation, die sich möglicherweise bereits in Ihrer Umgebung befindet. Weitere Informationen finden Sie unter [Erstellen und Bearbeiten von Unternehmen](../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).
* Wenn das Unternehmen einen Kunden oder Anbieter repräsentiert, erstellen Sie zusätzliche Mitarbeiter-Benutzer für die externe Organisation, die Sie möglicherweise in Ihrer Umgebung benötigen, um Kommunikation, Arbeitsausführung und Genehmigungen zu optimieren. Informationen zum Erstellen neuer Benutzer finden Sie unter [Benutzer hinzufügen](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).
* Aktualisieren Sie die Organigrammbeziehungen für alle Benutzer, die jetzt mit dem neu hinzugefügten Unternehmen verknüpft sind. Weitere Informationen finden Sie unter [Erstellen von ](../../administration-and-setup/add-users/create-and-manage-users/create-direct-reports.md) und [Anzeigen des Organigramms](../../people-teams-and-groups/work-directly-with-others/view-the-org-chart.md).

Weitere Informationen zu Unternehmen finden Sie unter [Erstellen und Bearbeiten von Unternehmen](../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

## Dashboard-Empfehlungen {#dashboard-recommendations}

Dieser Abschnitt enthält Empfehlungen für die Dashboards und Berichte, die mit einer Blueprint installiert wurden.

### Aktualisieren der neu erstellten Dashboards zum Hinzufügen/Entfernen von Berichten

Die aus einer Blueprint hinzugefügten Dashboards verfügen über einen oder mehrere Berichte, externe Seiten oder Kalender. Wahrscheinlich benötigen Sie entweder nicht alle Berichte und anderen Dashboard-Elemente oder Sie müssen das Dashboard um vorhandene Berichte, externe Seiten und Kalender erweitern, bevor es für die Freigabe für andere Personen bereit ist. Weitere Informationen finden Sie unter [Hinzufügen eines Berichts zu einem Dashboard](/help/quicksilver/reports-and-dashboards/dashboards/creating-and-managing-dashboards/add-report-dashboard.md).

### Aktualisieren Sie die neu erstellten Berichte, um Spalten oder Filterkriterien hinzuzufügen/zu entfernen

Die über einen Dashboard-Blueprint verteilten Berichte verfügen nicht über alle Spalten oder Filterkriterien, um Ihre Konfiguration von [!DNL Workfront] zu unterstützen. Es wird erwartet, dass Sie einige Anpassungen an den Berichten vornehmen werden, um sie an Ihre Standards anzupassen. Um die Konsistenz mit anderen Berichten in Ihrer Umgebung zu gewährleisten, empfiehlt es sich, eine Spalte in alle Berichte für das aufgelistete Objekt aufzunehmen oder Filterkriterien hinzuzufügen, die die Ergebnisse auf einen bestimmten Projekttyp oder eine bestimmte Benutzergruppe beschränken. Weitere Informationen finden Sie unter [Erstellen oder Bearbeiten von ](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-edit-views.md) und [Erstellen oder Bearbeiten von Filtern](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-filters.md).

### Freigeben von Dashboards oder Berichten für Benutzer

Wenn Sie nicht planen, das Dashboard auf einer Layout-Vorlage zu platzieren, sollten Sie das Dashboard für die Personen freigeben, die es nützlich finden. Weitere Informationen finden Sie unter [Freigeben eines Dashboards](/help/quicksilver/reports-and-dashboards/dashboards/creating-and-managing-dashboards/share-dashboard.md) und [Freigeben eines Berichts](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/share-report.md).

### Hinzufügen der Dashboards zu Layout-Vorlagen

Um Informationen für andere Personen verfügbar zu machen, fügen Sie Dashboards zu Layout-Vorlagen hinzu. Identifizieren Sie die Layout-Vorlagen der Personen, die am meisten von einer regelmäßigen Überprüfung des Dashboards profitieren würden, und fügen Sie das neu erstellte Dashboard zu diesen Layout-Vorlagen hinzu. Weitere Informationen finden Sie unter [Erstellen und Verwalten von Layout-Vorlagen](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

### Aktualisieren anderer Dashboards und Berichte

Die Einführung eines neuen Dashboards und seiner Berichte kann es ermöglichen, andere vorhandene Dashboards und Berichte außer Kraft zu setzen und anzupassen. Nehmen Sie sich die Zeit, Ihre vorhandenen Berichte zu überprüfen, um redundante und widersprüchliche Berichte zu identifizieren.

### Verteilen benutzerdefinierter Daten an relevante Formulare

Einige in einer Dashboard-Blueprint enthaltene Berichte verfügen über benutzerdefinierte Datenfelder in der Ansicht, im Filter oder in der Gruppierung des Berichts. In einigen Fällen verfügt der Blueprint auch über ein Formular, mit dem diese Felder verknüpft sind. In den meisten Fällen werden die benutzerdefinierten Felder jedoch nicht auf ein benutzerdefiniertes Formular angewendet. Damit Spalten, Filter oder Gruppierungen ordnungsgemäß funktionieren, müssen diese Felder mit Formularen verknüpft werden, die mit einem Benutzer, Projekt, einer Aufgabe oder einem anderen Objektdatensatz verbunden sind. Weitere Informationen finden Sie unter [Erstellen eines benutzerdefinierten Formulars](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).
