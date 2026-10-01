---
title: Verbesserungen bei Dokumenten für das vierte Quartal 2026
description: Verbesserungen bei Dokumenten für das vierte Quartal 2026
author: Becky
feature: Product Announcements
recommendations: noDisplay, noCatalog
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
subfeature_v2:
  - id: a29813d3-f0cc-4b60-9396-13b558370803
    internal-label: Product announcements
source-git-commit: deeb63ceccc28b8f376713d4a6fb6c103ab4e06b
workflow-type: tm+mt
source-wordcount: '1617'
ht-degree: 2%
---
# Verbesserungen bei Dokumenten für das vierte Quartal 2026

Auf dieser Seite werden die Verbesserungen beschrieben, die mit der Version vom vierten Quartal 2026 in der Vorschau-Umgebung vorgenommen wurden. Diese Verbesserungen werden wie angegeben in der Produktionsumgebung verfügbar gemacht.

Eine Liste aller Änderungen, die zu diesem Zeitpunkt im vierten Quartal 2026 des Versionszyklus verfügbar sind, finden Sie unter [Versionsübersicht für das vierte Quartal 2026](/help/quicksilver/product-announcements/product-releases/26-q4-release-activity/26-q4-release-overview.md).

## Zugreifen auf Workfront-Projekte über Creative Cloud Apps

>[!NOTE]
>  
>Vorschau: Nicht zutreffend\
>Produktions-Schnellveröffentlichung: 1. Oktober 2026\
>Produktion für alle: 1. Oktober 2026

Sie können jetzt direkt über Adobe Photoshop, Illustrator und InDesign auf Ihre Workfront-Projekte zugreifen. Workfront-Projekte, die den Adobe-Cloud-Speicher verwenden, werden im Bedienfeld Projekte auf der linken Seite des Programmfensters neben Ihren anderen Creative Cloud-Projekten angezeigt.

Sie können ein Dokument in einem Projektordner öffnen, bearbeiten und speichern. Ihre Änderungen werden wieder in Workfront gespeichert. Sie können neue Dateien auch direkt in einem Workfront-Projekt speichern.

Wenn Sie ein Dokument mit einem Genehmigungs-Workflow speichern, erstellt Workfront eine neue Version und behält den Genehmigungsverlauf bei. Wenn Sie ein Dokument speichern, das keinen Genehmigungs-Workflow hat, aktualisiert Workfront die neueste Version.

So verwenden Sie diese Integration:

* Ihr Unternehmen muss über eine Version von Workfront verfügen, die die Adobe-Cloud-Datenspeicherung unterstützt.
* Workfront und Photoshop, Illustrator oder InDesign müssen Berechtigungen in derselben Adobe Identity Management System (IMS)-Organisation haben.

Weitere Informationen finden Sie unter:

* [Übersicht über Adobe Creative Cloud-Projekte](/help/quicksilver/documents/adobe-creative-cloud-projects/adobe-creative-cloud-projects-overview.md)
* [Verwenden von Workfront-Dokumenten in Creative Cloud-Apps](/help/quicksilver/documents/adobe-creative-cloud-projects/use-wf-documents-in-cc-apps.md)

## Mehrere Dokumente in einem einzigen Genehmigungs-Workflow gruppieren

>[!NOTE]
>
>Vorschau: Diese Funktion ist in der Sandbox-Vorschau-Umgebung nicht verfügbar, da die Integration von Frame.io dort nicht verfügbar ist.
>Produktions-Schnellveröffentlichung: 14. Oktober 2026
>Produktion für alle: 15. Oktober 2026

Sie können jetzt mehrere Dokumente unter einem einzigen Genehmigungs-Workflow gruppieren, sodass sie dieselben Phasen gemeinsam durchlaufen.

Gruppierte Validierungen unterstützen den einfachen und erweiterten Modus, mehrere Phasen und parallele Pfade.

Gruppierte Validierungen sind nur im Bereich Neue Dokumente verfügbar, der angezeigt wird, wenn Ihr Unternehmen eine Version von Workfront verwendet, die Adobe Cloud Storage unterstützt.

Weitere Informationen finden Sie unter [Erstellen einer gruppierten Genehmigung](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-grouped-approval.md).

<!--

## Add a web link as a document

>[!NOTE]
>
> Preview: This feature isn't available in preview because Frame.io doesn't currently offer a preview environment.
> Production fast release: October 14, 2026
> Production for everyone: October 15, 2026

You can now add a website to Adobe Workfront as a web link in the new Documents area. After you add it, you can request approval on the live web page the same way you request approval on an uploaded file.

For more information, see [Add a web link as a document](/help/quicksilver/documents/adding-documents-to-workfront/add-live-url.md) and [Create a document approval workflow](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md).

-->

## Kontrollieren, wer Validierungsvorlagen sehen und verwenden kann

>[!NOTE]
>
>Vorschau: 30. Juli 2026
>Produktions-Schnellveröffentlichung: 13. August 2026
>Produktion für alle: 15. Oktober 2026

Genehmigungsvorlagen sind jetzt standardmäßig privat. Zuvor konnte jeder Validierungsanforderer jede Vorlage im System sehen, wodurch die Vorlagenlisten lang und schwer zu navigieren waren. Jetzt ist eine Vorlage nur noch für den Benutzer sichtbar, der sie erstellt hat, es sei denn, der Ersteller gibt sie frei.

Vorlagenersteller können eine Vorlage für bestimmte Benutzende oder für alle Personen in ihrem Unternehmen über die Liste der Genehmigungsvorlagen im Workfront-Setup freigeben. Bei der Anforderung einer Genehmigung sehen Benutzerinnen und Benutzer nur Vorlagen, die sie erstellt haben oder die für sie freigegeben wurden.

Diese Änderung gilt sowohl für neue als auch vorhandene Vorlagen, und der Zugriff wird konsistent erzwungen, unabhängig davon, wie eine Vorlage angefordert wird.

Weitere Informationen finden Sie unter:

* [Freigeben einer Vorlage](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md#share-a-template) in Erstellen einer Workflow-Vorlage für die Genehmigung von Dokumenten
* [Erstellen eines Workflows für die Dokumentvalidierung](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md)

## Systemadministratoren haben vollen Zugriff auf Genehmigungsvorlagen

>[!NOTE]
>
>Vorschau: 8. September 2026
>Produktions-Schnellveröffentlichung: 8. September 2026
>Produktion für alle: 8. September 2026
>[!BADGE Außerplanmäßig]{type=Neutral}

Systemadministratoren können jetzt jede Genehmigungsvorlage im Konto anzeigen, bearbeiten, löschen und stapelweise löschen, unabhängig davon, wer sie erstellt oder freigegeben hat. Zuvor unterlagen Systemadministratoren denselben Freigaberegeln wie andere Benutzer, und sie konnten nur von ihnen erstellte oder für sie freigegebene Vorlagen anzeigen oder verwalten.

Weitere Informationen finden Sie unter [Verwalten von ](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/manage-approval-templates.md).

## Sichtbarkeit von Frame.io-Kommentaren in Workfront

>[!NOTE]
>
>Vorschau: Nicht zutreffend
>Produktions-Schnellveröffentlichung: 17. September 2026
>Produktion für alle: 15. Oktober 2026

Wenn ein Genehmigungs-Workflow für ein Dokument erstellt wird, können Benutzer im Frame.io-Viewer Kommentare hinterlassen und Anmerkungen vornehmen. Diese Kommentare werden nicht im Workfront-Kommentarbedienfeld angezeigt, Sie können sie jedoch im Frame.io-Viewer anzeigen.

Jetzt zeigt das Bedienfeld „Kommentare“ in Workfront eine Meldung an, die Sie darüber informiert, wenn neue Kommentare in Frame.io verfügbar sind.

Weitere Informationen finden Sie unter [Hinzufügen einer Aktualisierung zu einem Dokument](/help/quicksilver/documents/managing-documents/add-update-documents.md).

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

Weitere Informationen finden Sie unter [Verknüpfen von Inhalten aus Experience Manager Assets mit Adobe Cloud-Speicher](/help/quicksilver/review-and-approve-work/native-integrations/frame-io/use-aem-with-frame.md#link-content-from-experience-manager-assets).

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

