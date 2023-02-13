---
content-type: reference
product-area: documents
navigation-topic: workfront-dam-within-workfront
title: Adobe Workfront-Lizenzierungs-Rollentypen im Vergleich zu Adobe Workfront DAM-Rollentypen
description: Adobe Workfront-Administratoren legen mithilfe von Zugriffsebenen fest, was Benutzer in einer Anwendung tun können.
author: Courtney
feature: Digital Content and Documents
exl-id: dcca0158-dc31-4aba-bd87-90ccc64e77cb
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '472'
ht-degree: 2%

---

# Adobe Workfront-Lizenzierungs-Rollentypen im Vergleich zu Adobe Workfront DAM-Rollentypen

Adobe Workfront-Administratoren legen mithilfe von Zugriffsebenen fest, was Benutzer in einer Anwendung tun können.

* In Workfront bestimmt die Lizenzierung die Zugriffsstufe eines Benutzers.
* In Workfront DAM definieren Rollentypen den Zugriff von Benutzern auf Assets im DAM.

Da Lizenztypen und Rollentypen nicht austauschbar sind, bedeutet der Zugriff auf eine der Anwendungen nicht, dass sie in der anderen Anwendung verfügbar sind. Beispielsweise wird einem Benutzer mit einer Work-Lizenz in Workfront nicht automatisch eine Mitarbeiter-Rolle innerhalb von Workfront DAM zugewiesen.

## Workfront Lizenzarten

Als Workfront-Administrator definieren Sie die Zugriffsstufe, die Benutzer haben, indem Sie Lizenztypen zuweisen. Jede Lizenz enthält eine Reihe von Standardzugriffsfunktionen, die Sie ändern können, bevor Sie die Lizenz dem Benutzer zuweisen. 

Sie verwenden die Lizenzierung, um zu bestimmen, was ein Benutzer in Workfront sehen und tun kann. In Workfront stehen fünf Lizenztypen zur Verfügung:

* Plan
* Arbeit
* Überarbeitung
* Anfrage
* Extern

Siehe [Übersicht über Adobe Workfront-Lizenzen](../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md) für eine Beschreibung der verschiedenen Lizenztypen in Workfront.

## Workfront DAM-Rollentypen

Als Workfront DAM Workfront-Administrator weisen Sie Benutzern Rollentypen zu, um den Zugriff auf Assets zu definieren. Darüber hinaus geben Rollentypen die Bereiche im DAM an, in denen Benutzer arbeiten können.

Rollentypen funktionieren bei der Festlegung von Benutzerzugriffsrechten zusammen mit Gruppen. Gruppen steuern den Zugriff der Benutzer auf Ordner und die Assets selbst. Rollentypen bestimmen, welche Aktionen Benutzer mit Assets ausführen können. Alle DAM-Benutzer müssen mindestens einer Gruppe zugeordnet sein. Weitere Informationen zu Rollentypen und zur Zugriffskonfiguration finden Sie in der Hilfe zu Workfront DAM.

In Workfront DAM stehen vier verschiedene Rollentypen zur Verfügung:

### Brand Portal

Benutzer mit diesem Rollentyp haben nur Zugriff auf das Brand Connect-Portal in DAM. Innerhalb des Portals können Benutzer Assets anzeigen und herunterladen, für die sie berechtigt sind.

Brand Portal-Benutzer können mit anderen zusammenarbeiten, indem sie Lightboxes erstellen und teilen.

### Regulärer Benutzer

Benutzer mit diesem Rollentyp können Assets aus Workfront DAM und dem Brand Connect-Portal anzeigen und herunterladen.

Normale Benutzer können auch mit anderen zusammenarbeiten, indem sie Lightboxes erstellen und teilen.

### Mitwirkender oder Mitwirkende

Benutzer mit diesem Rollentyp haben Zugriff auf Workfront DAM und das Brand Connect-Portal.

Mitarbeiter können Assets und Ordner, auf die sie Zugriff haben, anzeigen, herunterladen, hochladen, bearbeiten, verschieben und löschen. Darüber hinaus können Mitarbeiter mit anderen zusammenarbeiten, indem sie Lightboxes erstellen und teilen. 

### Administrator

Workfront-Administratoren haben Zugriff auf alles im Brand Connect-Portal und Workfront DAM, einschließlich Assets, die abgelaufen sind oder einen inaktiven Status haben.

Um Administratorzugriff zu erhalten, müssen sich Benutzer mit dem Rollentyp &quot;Administrator&quot;in der Administratorgruppe befinden.
