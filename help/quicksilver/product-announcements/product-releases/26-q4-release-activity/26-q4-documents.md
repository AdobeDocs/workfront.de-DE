---
title: Verbesserungen bei Dokumenten für das vierte Quartal 2026
description: Verbesserungen bei Dokumenten für das vierte Quartal 2026
author: Becky
feature: Product Announcements
recommendations: noDisplay, noCatalog
source-git-commit: 1b37b57f764d1579629e019c2025c809530124ea
workflow-type: tm+mt
source-wordcount: '1012'
ht-degree: 2%

---

# Verbesserungen bei Dokumenten für das vierte Quartal 2026

Auf dieser Seite werden die Verbesserungen beschrieben, die mit der Version vom vierten Quartal 2026 in der Vorschau-Umgebung vorgenommen wurden. Diese Verbesserungen werden wie angegeben in der Produktionsumgebung verfügbar gemacht.

Eine Liste aller Änderungen, die zu diesem Zeitpunkt im vierten Quartal 2026 des Versionszyklus verfügbar sind, finden Sie unter [Versionsübersicht für das vierte Quartal 2026](/help/quicksilver/product-announcements/product-releases/26-q4-release-activity/26-q4-release-overview.md).

<!--

## System Administrators full access to approval templates

>[!NOTE]
>
>Preview: September 4, 2026
>Production fast release: September 4, 2026
>Production for everyone: September 4, 2026
>[!BADGE Off schedule]{type=Neutral}

System Administrators can now view, edit, delete, and bulk-delete every approval template in the account, regardless of who created or shared it. Previously, System Administrators were subject to the same sharing rules as other users, and could only see or manage templates they created or that were shared with them.

For more information, see [Manage approval templates](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/manage-approval-templates.md).

-->

<!--

## Frame comment visibility in Workfront

>[!NOTE]
>
>Preview: September 3, 2026
>Production fast release: September 17, 2026
>Production for everyone: October 15, 2026

When an approval workflow is created for a document, users can leave comments and make annotations in the Frame.io viewer. These comments are not displayed in the Workfront Comments panel, but you can view them in the Frame.io viewer.

Now, the Comments panel in Workfront displays a message letting you know when new comments are available in Frame.io.

For more information, see [Add an update to a document](/help/quicksilver/documents/managing-documents/add-update-documents.md).

-->

## Direkter Zugriff auf Korrekturabzüge über Genehmigungs-E-Mail-Links

>[!NOTE]
>
>Vorschau: Nicht zutreffend
>Produktions-Schnellveröffentlichung: 17. September 2026
>Produktion für alle: 15. Oktober 2026

Wenn an ein Dokument ein Korrekturabzug angehängt wird, wird der Link „Zur Überprüfung gehen“ in den Genehmigungs-E-Mails jetzt direkt in der Korrekturabzugsansicht geöffnet, sodass Prüfende und genehmigende Personen sofort mit ihrer Überprüfung beginnen können. Wenn für ein Dokument kein Korrekturabzug vorhanden ist, wird durch den Link weiterhin der Abschnitt Genehmigungen des Dokuments geöffnet, wie zuvor.

## Hinzufügen von Teams zu Genehmigungen für Objekte mithilfe von Adobe Cloud Storage

>[!NOTE]
>
>Vorschau: 3. September 2026
>Produktions-Schnellveröffentlichung: 17. September 2026
>Produktion für alle: 15. Oktober 2026

Sie können jetzt ein Workfront-Team als genehmigende Person oder Prüfende Person zu einer Dokumentgenehmigungs- oder Genehmigungsvorlage hinzufügen, anstatt jede Person einzeln hinzuzufügen:

* Objekte im Adobe-Cloud-Speicher: Workfront fügt jedes aktive Teammitglied einzeln hinzu, sodass die Liste der genehmigenden Personen immer widerspiegelt, wer sich derzeit im Team befindet.
* Objekte, die Legacy-Workfront-Speicher verwenden: Das Team wird standardmäßig als Einzelteilnehmer hinzugefügt, Sie können jetzt jedoch jedes Teammitglied als Einzelteilnehmer hinzufügen.
* In Genehmigungsvorlagen speichert Workfront einen Verweis auf das Team und erweitert es in aktive Mitglieder, wenn Sie die Vorlage auf ein Dokument anwenden, und nicht beim Speichern der Vorlage.

Weitere Informationen finden Sie unter:

* [Erstellen eines Validierungs-Workflows im Bereich „Neue Dokumente“](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md#create-an-approval-workflow-in-the-new-documents-area)
* [Erstellen eines Validierungs-Workflows im Bereich „Alte Dokumente“](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md#create-an-approval-workflow-in-the-legacy-documents-area)
* [Erstellen einer Validierungs-Workflow-Vorlage für Dokumente](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md)

## Festlegen eines Frame.io-Arbeitsbereichs in Projektvorlagen

>[!NOTE]
>
>Vorschau: 3. September 2026
>Produktions-Schnellveröffentlichung: 17. September 2026
>Produktion für alle: 15. Oktober 2026

Wenn Ihr Unternehmen Adobe Cloud Storage verwendet und Sie über eine Frame.io Enterprise-Lizenz verfügen, können Sie jetzt in den Projektdetails einer Projektvorlage einen Frame.io-Arbeitsbereich auswählen. Über die Vorlage erstellte Projekte verwenden automatisch den in der Vorlage festgelegten Arbeitsbereich, sodass Projekte an den gewünschten Frame.io-Arbeitsbereich weitergeleitet werden, ohne dass bei der Projekterstellung eine zusätzliche Aktion erforderlich ist.

Im neuen Feld werden die Frame.io-Arbeitsbereiche aufgelistet, denen Sie Projekte zuweisen können. Das Feld kann jederzeit in der Vorlage bearbeitet werden. Änderungen gelten nur für Projekte, die nach der Aktualisierung erstellt wurden, sodass vorhandene Projekte ihren ursprünglichen Arbeitsbereich behalten.

Nachdem ein Projekt über die Vorlage erstellt wurde, ist sein Arbeitsbereichsfeld Frame.io schreibgeschützt und enthält Links zum Arbeitsbereich in Frame.io.

Wenn Sie keine Enterprise-Lizenz für Frame.io haben, werden die Projekte weiterhin in den Standardarbeitsbereich für Workfront verschoben.

Weitere Informationen finden Sie unter [Projektvorlagen bearbeiten](/help/quicksilver/manage-work/projects/create-and-manage-templates/edit-templates.md) und [Informationen verwalten im Bereich Projektübersicht](/help/quicksilver/manage-work/projects/manage-projects/understand-project-overview-area.md).

<!--

## Consistent review and approval buttons across documents

>[!NOTE]
>
>Preview: September 3, 2026
>Production fast release: September 17, 2026
>Production for everyone: October 15, 2026

Review and approval buttons now look and work the same everywhere you review documents: My approvals widget in Home, Document summary panel, the Document Details page, and the document preview page.

In addition to a new look and feel, some buttons have new names:

| Previous name | New name |
| --- | --- |
| Open proof | Open viewer |
| Review and approve | Make decision |
| Complete my review | Complete review |
| Open in Frame.io | Open viewer |

For more information, see [Review and approve documents](/help/quicksilver/documents/review-and-approve-documents.md).

-->

## Benutzerdefinierte Nachricht in E-Mail-Betreffzeile

>[!NOTE]
>
>Vorschau: Nicht zutreffend
>Produktions-Schnellveröffentlichung: 17. September 2026
>Produktion für alle: 15. Oktober 2026

Wenn Sie eine benutzerdefinierte Nachricht für eine Dokumentgenehmigung festlegen, wird diese Nachricht jetzt auch in der Betreffzeile der E-Mail mit der Genehmigungsanfrage angezeigt, wobei das Fälligkeitsdatum im Feld festgelegt wird. Auf diese Weise können Validierungsverantwortliche sehen, was Aufmerksamkeit erfordert, und sie können sehen, wann dies direkt in ihrem Posteingang geschieht, ohne die E-Mail zu öffnen.

Weitere Informationen finden Sie unter [Erstellen eines Dokumentgenehmigungs-Workflows](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md).

## Bedienfeld für neu gestaltete Versionen im Bereich Neue Dokumente

>[!NOTE]
>
>Vorschau: 3. September 2026
>Produktions-Schnellveröffentlichung: 17. September 2026
>Produktion für alle: 15. Oktober 2026

Wenn Ihr Unternehmen Adobe Cloud Storage verwendet, hat das Bedienfeld „Versionen“ im Bereich „Neue Dokumente“ ein neues Design:

* Versionen sind mit V1, V2 usw. gekennzeichnet, um die Konsistenz mit Frame.io zu gewährleisten.
* Jede Version zeigt ihren Genehmigungsstatus, wie „Genehmigt“ oder „Zurückgenommen“, direkt in der Liste an.
* Das Bedienfeld listet jetzt nur noch den Versionsverlauf auf - oben gibt es keinen separaten Eintrag für die „neueste Datei“ mehr.

Zuvor waren Versionen mit einem Zeitstempel versehen anstatt nummeriert.

Weitere Informationen finden Sie unter [Verwalten von Dokumentversionen](/help/quicksilver/documents/managing-documents/manage-document-versions.md).

## Neu gestaltetes Genehmigungsbedienfeld im Bereich „Neue Dokumente“

>[!NOTE]
>
>Vorschau: 3. September 2026
>Produktions-Schnellveröffentlichung: 17. September 2026
>Produktion für alle: 15. Oktober 2026

Wenn Ihr Unternehmen Adobe Cloud-Speicher verwendet, zeigt das Bedienfeld Genehmigungen im Bereich Neue Dokumente jetzt einen versionsübergreifenden Genehmigungsverlauf an:

* Im Bedienfeld wird der Genehmigungs-Workflow für jede Version aufgelistet, die über eine verfügt, nicht nur für die aktuelle Version.
* Zurückgenommene Workflows bleiben in der Liste, sodass Sie ihre vorherigen Entscheidungen weiterhin überprüfen können.
* Erweitern Sie eine beliebige Version, um die Phasen, Entscheidungen der genehmigenden Person, Entscheidungsregeln und Fälligkeitsdaten anzuzeigen, ohne das Bedienfeld zu verlassen.

Zuvor wurde im Bedienfeld Genehmigungen nur der Workflow der aktuellen Version angezeigt.

Weitere Informationen finden Sie unter [Erstellen eines Dokumentgenehmigungs-Workflows](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md).

## Bilder an Kommentare zu Adobe-Cloud-Speicherobjekten anhängen

>[!NOTE]
>
>Vorschau: 30. Juli 2026
>Produktions-Schnellveröffentlichung: 30. Juli 2026
>Produktion für alle: 30. Juli 2026
>[!BADGE Außerplanmäßig]{type=Neutral}

Unternehmen, die Adobe Cloud Storage im Rahmen der einheitlichen Überprüfung und Genehmigung verwenden, können jetzt Bilddateien direkt an Kommentare anhängen und Feedback, Kontext und unterstützende Visualisierungen in einem einzigen, nachvollziehbaren Kommentar-Thread zusammenführen. Dadurch wird eine frühere Lücke geschlossen, in der nur Organisationen, die noch über alten Workfront-Speicher verfügen, Bilder an Kommentare anhängen konnten.

Alle Bildformate vom Typ Medien werden jetzt für Adobe Cloud-Speicherorganisationen unterstützt. (Ältere Objektkommentare unterstützen weiterhin nur .jpg-, .gif- und .png-Dateien.) Nicht-Bilddateien werden nicht für Kommentare für veraltete oder Adobe Cloud-Speicherobjekte unterstützt.

Weitere Informationen finden Sie unter [Arbeit aktualisieren](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

## Verknüpfen von Assets aus Experience Manager Assets mit dem Adobe-Cloud-Speicher

>[!NOTE]
>
>Vorschau: 30. Juli 2026
>Produktions-Schnellveröffentlichung: 13. August 2026
>Produktion für alle: 15. Oktober 2026

Wenn Ihr Unternehmen Adobe Cloud Storage verwendet, können Sie einzelne Assets aus Experience Manager Assets mit jedem Workfront-Objekt verknüpfen, das Dokumente unterstützt. Verknüpfte Inhalte bleiben automatisch synchronisiert: In Experience Manager Assets vorgenommene Änderungen werden in Workfront angezeigt und Sie können neue Asset-Versionen abrufen, ohne Workfront verlassen zu müssen.

Die Verknüpfung wird von Content Advisor unterstützt, sodass Sie auch KI-Suchen, intelligente Vorschläge, Kampagnenkurzanalysen und mehr erhalten, während Sie Inhalte auswählen.

Weitere Informationen finden Sie unter [Verknüpfen von Inhalten aus Experience Manager Assets mit Adobe Cloud-Speicher](/help/quicksilver/review-and-approve-work/native-integrations/link-aem-assets-cloud-storage.md).

<!--

## Approval workflow templates are private by default

>[!NOTE]
>
>Preview: July 30, 2026
>Production fast release: August 13, 2026
>Production for everyone: October 15, 2026

Approval templates are now private by default. Previously, every approval requester could see every template in the system, which made template lists long and hard to navigate. Now, a template is visible only to the user who created it, unless the creator shares it.

For more information, see:

* [Share a template](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/manage-approval-templates.md#share-a-template) in Manage approval templates
* [Create a document approval workflow](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md)

-->

