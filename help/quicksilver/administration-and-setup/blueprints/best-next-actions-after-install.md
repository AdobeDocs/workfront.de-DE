---
user-type: administrator
content-type: reference
product-area: system-administration;workfront-integrations
navigation-topic: best-practices-catalog
title: Aktionen, die nach der Installation eines Blueprints ausgeführt werden sollen
description: In diesem Artikel wird beschrieben, was Sie nach der Installation eines Blueprints in [!DNL Adobe Workfront] tun sollten, um den Blueprint vollständig für Ihre Systembenutzer bereitzustellen.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 6e5da58f-105a-4edf-8fc1-65e8762d43c6
source-git-commit: 7697327455a7ffdc1a15bfa1676c3a0b091abd04
workflow-type: tm+mt
source-wordcount: '1135'
ht-degree: 0%

---

# Nach der Installation eines Blueprints zu ergreifende Maßnahmen

In diesem Artikel wird beschrieben, was Sie nach der Installation eines Blueprints in [!DNL Adobe Workfront] tun sollten, um den Blueprint vollständig für Ihre Systembenutzer bereitzustellen.

* [Empfehlungen für Projektvorlagen](#project-template-recommendations)
* [Empfehlungen zur Organisationsstruktur](#organizational-structure-recommendations)
* [Dashboard-Empfehlungen](#dashboard-recommendations)

## Empfehlungen für Projektvorlagen {#project-template-recommendations}

Dieser Abschnitt enthält Empfehlungen für die mit Ihren Blueprints installierten Projektvorlagen.

### Benutzer neu erstellten Rollen und Teams zuweisen {#assign-users-to-newly-created-roles-and-teams}

Den Rollen und/oder Teams, die während des Blueprint-Installationsprozesses erstellt wurden, sind keine Benutzer automatisch zugeordnet. Ohne die Zuweisung von Benutzern zu den neu hinzugefügten Rollen oder Teams erstellen Sie Arbeiten für eine Funktion, die von niemandem übernommen wird. In einigen Fällen müssen Sie möglicherweise neue Benutzer erstellen, um diese Rollen und Teams auszufüllen. Informationen zum Erstellen neuer Benutzer finden Sie unter [Benutzer hinzufügen](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

### Anwenden eines benutzerdefinierten Formulars auf die Vorlage und die Vorlagenaufgaben {#apply-a-custom-form-to-the-template-and-the-template-tasks}

Der Installationsprozess verknüpft die Projektvorlage nicht mit benutzerdefinierten Formularen. Wenn Ihre Projekte oder Aufgaben spezifische Formulare oder Felder zum Erstellen der Berichtskonsistenz benötigen oder wenn Ihr digitales Anfrageformular Felder enthält, die auf Projektebene beibehalten werden müssen, empfehlen wir, die Vorlage oder die Vorlagenaufgaben mit diesen Formularen zu verknüpfen. Weitere Informationen finden Sie unter [Hinzufügen eines benutzerdefinierten Formulars zu einem Objekt](../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

### Aktualisierung der Vorlagendauer und -aufwand {#update-template-task-duration-and-effort-estimates}

Jede Aufgabe in der Vorlage enthält eine geplante Dauer und eine geplante Aufwandsschätzung. Diese Schätzungen dienen als Ausgangspunkt für die Dauer und die für diese Aktivitäten verbrachte Zeit. Die Fähigkeiten, Fertigkeiten und Geschwindigkeit Ihres Unternehmens sind jedoch einzigartig. Sie sollten die geschätzte Dauer und den Aufwand jeder Aufgabe überprüfen, um sie an die Bedürfnisse Ihres Unternehmens anzupassen. Weitere Informationen finden Sie unter [Verwalten von Aufgabeninformationen im Bereich [!UICONTROL Übersicht über Aufgabendetails]](../../manage-work/tasks/manage-tasks/task-information-in-overview.md) .

### Meilensteinpfad und Meilensteine verknüpfen {#associate-a-milestone-path-and-milestones}

Der Installationsprozess verknüpft die Projektvorlage nicht mit einem Meilensteinpfad. Wenden Sie einen Meilensteinpfad auf die Vorlage an und wenden Sie Meilensteine auf wichtige Aufgaben in der Vorlage an, um Ihre Meilensteinberichtspflichten zu unterstützen. Weitere Informationen finden Sie unter [Verknüpfen von Meilensteinen mit Aufgaben](../../manage-work/tasks/manage-tasks/associate-milestones-with-tasks.md).

### Rollout der Vorlage für Ihr Team {#roll-out-the-template-to-your-team}

Bereiten Sie Schulungsmaterialien für die Manager vor, die diese Vorlage verwenden, sowie für die einzelnen Mitarbeiter, die die Arbeit in der Projektvorlage ausführen.

### Erstellen oder Aktualisieren von Berichten und Dashboards {#create-or-update-reports-and-dashboards}

Wenn die Lösung eine neue Art von Arbeit darstellt, die Ihr Unternehmen zuvor in [!DNL Workfront] nicht ausgeführt hat, müssen Sie möglicherweise neue Berichte und Dashboards erstellen, um die Arbeit zu unterstützen. Weitere Informationen finden Sie unter [Benutzerspezifischen Bericht erstellen](../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md) und [Dashboard erstellen](../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md).

Wenn die Lösung den bereits in [!DNL Workfront] ausgeführten Arbeiten ähnelt, sollten Sie überprüfen, ob die Arbeit erwartungsgemäß in vorhandene Berichte und Dashboards eingespeist wird. Wenn die Filter nicht in Ihre vorhandenen Berichte einfließen, sollten Sie Maßnahmen ergreifen, um Filter zu aktualisieren oder neue Berichte zu erstellen.

## Empfehlungen zur Organisationsstruktur {#organizational-structure-recommendations}

Dieser Abschnitt enthält Empfehlungen für die mit Ihren Blueprints installierten Elemente der Organisationsstruktur.

### Firmen

Nach der Installation eines Blueprints, der ein Unternehmen enthält:

* Fügen Sie ein benutzerdefiniertes Formular hinzu, um den Firmendatensatz mit nützlichen Details zu ergänzen (das Formular und seine Details sind für Sie eindeutig). Weitere Informationen finden Sie unter [Hinzufügen eines benutzerdefinierten Formulars zu einem Objekt](../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).
* Wenn das Unternehmen einen Kunden repräsentiert, überprüfen Sie die mit dem Unternehmen verbundenen Überschreibungsraten. Weitere Informationen finden Sie unter [Außerkraftsetzen der Abrechnungsraten für Auftragsrollen auf Unternehmensebene](../../administration-and-setup/set-up-workfront/organizational-setup/override-job-role-billing-rates-company-level.md).
* Wenn das Unternehmen einen Kunden repräsentiert und es andere Projektvorlagen gibt, die für diese Organisation eindeutig sind, verknüpfen Sie die Projektvorlagen zunächst mit dem neu hinzugefügten Unternehmen. Weitere Informationen finden Sie unter [Bearbeiten von Projektvorlagen](../../manage-work/projects/create-and-manage-templates/edit-templates.md).
* Wenn das Unternehmen einen Kunden oder einen Anbieter repräsentiert, verknüpfen Sie vorhandene Benutzer aus der externen Organisation, die sich möglicherweise bereits in Ihrer Umgebung befinden. Weitere Informationen finden Sie unter [Erstellen und Bearbeiten von Unternehmen](../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).
* Wenn das Unternehmen einen Kunden oder einen Anbieter repräsentiert, erstellen Sie zusätzliche Mitarbeiter-Benutzer für die externe Organisation, die Sie möglicherweise in Ihrer Umgebung benötigen, um die Kommunikation, die Arbeitsausführung und die Genehmigungen zu optimieren. Informationen zum Erstellen neuer Benutzer finden Sie unter [Benutzer hinzufügen](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).
* Aktualisieren Sie die Beziehungen der Organigramme für alle Benutzer, die jetzt mit dem neu hinzugefügten Unternehmen verknüpft sind. Weitere Informationen finden Sie unter [Erstellen von direkten Berichten](../../administration-and-setup/add-users/create-and-manage-users/create-direct-reports.md) und [Anzeigen des Organigrafts](../../people-teams-and-groups/work-directly-with-others/view-the-org-chart.md).

Weitere Informationen zu Unternehmen finden Sie unter [Erstellen und Bearbeiten von Unternehmen](../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

## Dashboard-Empfehlungen {#dashboard-recommendations}

Dieser Abschnitt enthält Empfehlungen für die Dashboards und Berichte, die mit einem Blueprint installiert werden.

### Neu erstellte Dashboards aktualisieren, um Berichte hinzuzufügen/zu entfernen

Die über einen Blueprint hinzugefügten Dashboards verfügen über einen oder mehrere Berichte, externe Seiten oder Kalender. Sie benötigen wahrscheinlich nicht alle Berichte und anderen Dashboard-Elemente oder müssen das Dashboard mit vorhandenen Berichten, externen Seiten und Kalendern erweitern, bevor es für andere Personen freigegeben werden kann. Weitere Informationen finden Sie unter [Einen Bericht zu einem Dashboard hinzufügen](/help/quicksilver/reports-and-dashboards/dashboards/creating-and-managing-dashboards/add-report-dashboard.md).

### Aktualisieren Sie die neu erstellten Berichte, um Spalten hinzuzufügen/zu entfernen oder Kriterien zu filtern

Die über einen Dashboard-Blueprint verteilten Berichte verfügen nicht über alle Spalten oder Filterkriterien, die Ihre Konfiguration von [!DNL Workfront] unterstützen. Es wird erwartet, dass Sie einige Anpassungen an den Berichten vornehmen, um sie an Ihre Standards anzupassen. Um die Konsistenz mit anderen Berichten in Ihrer Umgebung zu gewährleisten, können Sie eine Spalte hinzufügen, die Sie in alle Berichte für das aufgelistete Objekt aufnehmen, oder Filterkriterien hinzufügen, die die Ergebnisse auf einen bestimmten Projekttyp oder eine bestimmte Benutzergruppe beschränken. Weitere Informationen finden Sie unter [Erstellen oder Bearbeiten von Ansichten](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-edit-views.md) und [Erstellen oder Bearbeiten von Filtern](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-filters.md).

### Dashboards oder Berichte für Benutzer freigeben

Wenn Sie das Dashboard nicht auf einer Layoutvorlage platzieren möchten, sollten Sie das Dashboard für die Personen freigeben, die es für nützlich halten. Weitere Informationen finden Sie unter [Dashboard freigeben](/help/quicksilver/reports-and-dashboards/dashboards/creating-and-managing-dashboards/share-dashboard.md) und [Bericht freigeben](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/share-report.md).

### Hinzufügen von Dashboards zu Layoutvorlagen

Die beste Möglichkeit, Informationen für andere Benutzer verfügbar zu machen, besteht darin, Dashboards zu Layout-Vorlagen hinzuzufügen. Bestimmen Sie die Layoutvorlagen der Personen, die am meisten von einer regelmäßigen Überprüfung des Dashboards profitieren würden, und fügen Sie diesen Layoutvorlagen das neu erstellte Dashboard hinzu. Weitere Informationen finden Sie unter [Erstellen und Verwalten von Layoutvorlagen](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

### Andere Dashboards und Berichte aktualisieren

Die Einführung eines neuen Dashboards und seiner Berichte kann es ermöglichen, andere vorhandene Dashboards und Berichte einzustellen und anzupassen. Nehmen Sie sich die Zeit, Ihre vorhandenen Berichte zu überprüfen, um redundante und widersprüchliche Berichte zu identifizieren.

### Verteilen benutzerdefinierter Daten in relevante Formulare

Einige Berichte, die in einem Dashboard-Blueprint enthalten sind, verfügen entweder über benutzerdefinierte Datenfelder in der Ansicht, im Filter oder in der Gruppierung des Berichts. In einigen Fällen enthält der Blueprint auch ein Formular, mit dem diese Felder verknüpft sind. In den meisten Fällen werden die benutzerdefinierten Felder jedoch nicht auf ein benutzerdefiniertes Formular angewendet. Damit die Spalten, Filter oder Gruppierungen ordnungsgemäß funktionieren, müssen diese Felder mit Formularen verknüpft sein, die mit einem Benutzer, Projekt, einer Aufgabe oder einem anderen Objektdatensatz verbunden sind. Weitere Informationen finden Sie unter [Erstellen eines benutzerdefinierten Formulars](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).
