---
title: Erstellen und Ändern benutzerdefinierter Zugriffsebenen
user-type: administrator
product-area: system-administration;user-management
navigation-topic: configure-access-to-workfront
description: Als Adobe Workfront-Administrator können Sie benutzerdefinierte Zugriffsebenen erstellen und sie auf Benutzende anwenden.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: d2a73d24-51d3-42e2-9c09-7f4bc30b2caa
source-git-commit: f9bf60fc39cc7cd26e242e7cc782ece060cc5471
workflow-type: tm+mt
source-wordcount: '1465'
ht-degree: 6%

---

# Benutzerdefinierte Zugriffsebenen erstellen und ändern

<!--Audited: 12/2023-->

<!--Don't delete, draft, or change the title of this article. The UI links to it via context-sensitive help. -->

Als Adobe Workfront-Administrator können Sie benutzerdefinierte Zugriffsebenen erstellen und sie auf Benutzende anwenden. Bei der Arbeit mit Zugriffsebenen ist es wichtig zu verstehen, wie diese mit den Objektberechtigungen zusammenarbeiten, die Benutzende erteilen, wenn sie Objekte miteinander teilen. Weitere Informationen zu Zugriffsebenen finden Sie unter:

* [Übersicht über neue Zugriffsebenen](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/access-level-overview.md)
* [Übersicht über Zugriffsebenen](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md)

>[!IMPORTANT]
>
>Es wird dringend empfohlen, die integrierten Zugriffsebenen unverändert zu lassen, damit Sie nach der Einrichtung Ihrer Benutzer darauf verweisen können. Um eine Zugriffsebene anzupassen, kopieren Sie die standardmäßige Zugriffsebene und ändern Sie die Kopie. Dies ist für jede Zugriffsebene möglich, mit Ausnahme von Systemadministrator und externem Benutzer.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan</td> 
   <td>Beliebig</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td>Neu: Standard
   <p>oder</p>
   <p>Aktuell: Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Sie müssen ein Workfront-Administrator sein.</p></td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Erstellen oder Bearbeiten einer benutzerdefinierten Zugriffsebene

{{step-1-to-setup}}

1. Klicken **im linken** auf „Zugriffsebenen“.
1. Wählen Sie die Zugriffsebene aus, die Sie kopieren und anpassen möchten, und klicken Sie dann auf **Kopieren**.

   Oder

   Wenn Sie eine vorhandene Zugriffsebene bearbeiten (die Sie zuvor kopiert haben), klicken Sie auf ihren Namen.

1. Führen Sie im angezeigten Feld einen der folgenden Schritte aus, um mit der Konfiguration der benutzerdefinierten Zugriffsebene zu beginnen:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Name</td> 
      <td> <p>Geben Sie einen Namen für Ihre Zugriffsebene ein. </p> <p>Wenn Sie gerade eine Zugriffsebene kopiert haben, um eine neue zu erstellen, lautet der Standardname Access Level Name (Kopieren) , wobei Access Level Name die Zugriffsebene ist, die Sie kopiert haben.</p> <p><strong>Tipp</strong>: Es wird empfohlen, im Namen der Kopie den ursprünglichen Namen der Zugriffsebene anzugeben. Bei der Firma ACME kann beispielsweise eine Kopie der standardmäßigen Zugriffsebene ACME Standard genannt werden.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Beschreibung </td> 
      <td>Geben Sie eine Beschreibung für die Zugriffsebene ein. Es ist hilfreich, hier aufzulisten, auf was ein Benutzer mit dieser Zugriffsebene zugreifen kann.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Lizenztyp</td> 
      <td>Stellen Sie sicher, dass die hier ausgewählte Lizenz diejenige ist, die am engsten mit der Art der Zugriffsebene verbunden ist, die Sie erstellen oder bearbeiten. Die ausgewählte Lizenz bestimmt, welche Einstellungen für die Zugriffsebene verfügbar sind. Weitere Informationen finden Sie unter <a href="/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/licenses-overview.md" class="MCXref xref">Übersicht über neue Lizenzen</a> oder <a href="/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md">Überblick über Lizenzen</a>.</td> 
     </tr> 
    </tbody> 
   </table>

1. (Bedingt) Wenn **Standard** oder **Plan** im Feld **Lizenztyp** ausgewählt ist, scrollen Sie zum Abschnitt **Administratorzugriff für zulassen** und wählen Sie Administratorzugriffsberechtigungen für diejenigen aus, die diese Zugriffsebene haben werden.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Genehmigungsprozesse</td> 
      <td>Genehmigungsprozesse zur Verwendung im gesamten System und für bestimmte Gruppen erstellen und verwalten<p>Ohne diesen Zugriff können Benutzende nur Ad-hoc-Genehmigungsprozesse für Elemente erstellen, auf die sie Zugriff haben und die sie verwalten können.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Firmen</td> 
      <td>Fügen Sie neue hinzu und bearbeiten Sie bestehende Unternehmen in Workfront.<br><p>Ohne diesen Zugriff können Benutzer nur vorhandene Unternehmen anzeigen.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Benutzerdefinierte Formulare</td> 
      <td>Erstellen und verwalten Sie alle benutzerdefinierten Formulare in ihrer Gruppe. <br><p>Ohne diesen Zugriff können Benutzende nur vorhandene Formulare an die Objekte anhängen, zu denen sie beitragen oder die sie verwalten können.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Wechselkurse</td> 
      <td> Neue Währung in Workfront hinzufügen. <p>Ohne diesen Zugriff kann der Benutzer eine vorhandene Währung nur zu einem Projekt hinzufügen, das er erstellt.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ausgaben</td> 
      <td>Alle Ausgaben für Objekte in Workfront anzeigen.<p>Ohne diesen Zugriff kann der Benutzer nur Folgendes anzeigen:</p>
       <ul>
        <li>Ausgaben für von ihnen verwaltete Projekte, Aufgaben oder Probleme</li>
        <li>Ihre eigenen Kosten</li>
        <li>Die Ausgaben ihrer Untergebenen</li>
       </ul><p><b>HINWEIS</b>: Dies ermöglicht es dem Benutzer nicht, neue Ausgabentypen zu erstellen.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Aufgabengebiete</td> 
      <td> Mit diesem Zugriff kann der Benutzer Folgendes tun: 
       <ul> 
        <li>Anzeigen und Bearbeiten vorhandener Aufgabengebiete</li> 
        <li>Neue Aufgabengebiete hinzufügen</li> 
        <li>Funktionsbezogene Abrechnung und Kostensätze bearbeiten</li> 
       </ul> 
       <p>Wichtige Informationen zum Zugriff auf Finanzdaten, die einem Standard- oder Planer-Benutzer mit administrativem Zugriff auf Aufgabengebiete zur Verfügung stehen, finden Sie unter <a href="#standard-or-planner-users-with-administrative-access-to-job-roles">Standard- oder Planer-Benutzer mit administrativem Zugriff auf Aufgabengebiete</a>.</p>
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Meilensteine in meiner Gruppe</td> 
      <td>Zeigen Sie alle Meilensteinpfade im System unter dem Menü Meilensteinpfade im Setup an. Benutzer können auch alle Meilensteinpfade bearbeiten oder löschen, die zu einer ihrer Gruppen gehören. Benutzende können keine Meilensteinpfade verwalten (bearbeiten oder löschen), die nicht ihren Gruppen zugewiesen sind.<p>Ohne diesen Zugriff können Benutzende nur vorhandene Meilensteinpfade anzeigen und auf Projekte anwenden, auf die sie Zugriff haben.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Erinnerungsbenachrichtigungen</td> 
      <td>Erstellen und Verwalten von Erinnerungsnachrichten in Workfront.<p>Ohne diesen Zugriff sind die Benutzenden darauf beschränkt, Benachrichtigungen zu empfangen und anzuzeigen.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Arbeitszeittabellen und Stunden</td> 
      <td> Gruppenadministratoren können Benutzern in den von ihnen verwalteten Gruppen und Untergruppen Arbeitszeittabellen-Profile zuweisen. <p>Ohne diese Option können Gruppenadministratoren anderen Benutzern in den von ihnen verwalteten Gruppen und Untergruppen keine Arbeitszeittabellen-Profile zuweisen, sie können sie jedoch erstellen.</p> <p>Alle anderen Benutzer mit einer Standard- oder Planlizenz können alle Stunden und Arbeitszeittabellen in Workfront anzeigen.</p> <p>Ohne diese Option können Benutzende Stunden nur in folgenden Bereichen anzeigen:</p> 
       <ul> 
        <li>Von ihnen verwaltete Projekte, Aufgaben oder Probleme</li> 
        <li>Ihre eigene Arbeitszeittabelle</li> 
        <li>Arbeitszeittabelle einer Person, die ihnen unterstellt ist</li> 
        <li>Eine von ihnen genehmigte Arbeitszeittabelle</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. Klicken Sie **Zusätzliche Einschränkungen festlegen** und legen Sie dann eine der folgenden Einschränkungen für die Zugriffsebene fest.

   >[!IMPORTANT]
   >
   >Für externe Benutzer wie z. B. Anbieter (alle Personen, die nicht zu Ihrer Organisation gehören) empfehlen wir, den Zugriff auf Aufgaben, Projekte, Aktualisierungen, Ankündigungen, andere Unternehmen, Teams und Gruppen zu beschränken.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Nie Zugriff auf das gesamte Projekt geben, wenn einer Aufgabe oder einem Problem zugeordnet</td> 
      <td> Verhindert, dass Benutzende, die Aufgaben oder Problemen zugewiesen sind, auch Berechtigungen für das übergeordnete Projekt erhalten, selbst wenn die Projektberechtigungen dies zulassen.<p>Weitere Informationen zum Konfigurieren der Berechtigungen für ein Projekt finden Sie im Abschnitt <a href="../../../manage-work/projects/manage-projects/edit-projects.md#access" class="MCXref xref"></a> im Artikel <a href="../../../manage-work/projects/manage-projects/edit-projects.md" class="MCXref xref">Projekte bearbeiten</a>.</p></td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Nie den Dokumentzugriff aus Projekten, Aufgaben, Problemen etc. erben</td> 
      <td>Verhindert, dass Dokumente die für ihr übergeordnetes Objekt festgelegten Berechtigungen erben.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Nur Aktualisierungen anzeigen, in denen Sie an der Konversation beteiligt waren</td> 
      <td> Ermöglicht es Benutzern, nur Kommentare anzuzeigen, in denen ihr Name oder der Name ihres Teams enthalten ist. <p> <p><b>HINWEIS</b>: Dies verhindert, dass Benutzende Elemente in Workfront abonnieren. Weitere Informationen zum Abonnieren von Elementen finden Sie unter <a href="../../../workfront-basics/using-notifications/subscribe-to-items-in-workfront.md" class="MCXref xref">Abonnieren von Elementen in Adobe Workfront</a>.</p> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Nicht zulassen, dass Benutzer Kommentare löschen </td> 
      <td> Verhindert, dass Benutzer Kommentare zu Elementen löschen.  <p><b>HINWEIS</b>: Niemand kann die Kommentare anderer Benutzer löschen.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Nur Firmen, Gruppen &amp; Teams anzeigen, der Sie angehören</td> 
      <td>Ermöglicht Benutzenden, Elemente nur für Unternehmen, Gruppen und Teams anzuzeigen und freizugeben, denen sie angehören.<p><strong>HINWEIS</strong>: Benutzer mit Anforderer- oder Mitwirkerlizenzen können keine Unternehmen anzeigen, denen sie nicht angehören, selbst wenn diese Option aktiviert ist.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Anzeige von "Geplante Stunden" oder "Tatsächliche Stunden" nicht zulassen</td> 
      <td>Verhindert, dass Benutzende die geplanten und tatsächlichen Stunden von Arbeitselementen sehen, auf die sie Zugriff haben. Sie können jedoch tatsächliche Stunden sehen, die sie selbst protokollieren, oder Stunden, die von einer an sie berichtenden Person protokolliert werden.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Nie zulassen, dass Benutzer Ankündigungen löschen</td> 
      <td>Verhindert, dass Benutzer Ankündigungen im Ankündigungscenter löschen. Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/get-started-wf-administration/view-send-announcements.md" class="MCXref xref">Ankündigungen senden</a>.</td> 
     </tr> 
    </tbody> 
   </table>

1. (Bedingt und optional) Wenn Ihr Workfront-System für Benutzende eingerichtet ist, die mehreren Unternehmen angehören, sollten Sie die Sichtbarkeit für andere Benutzende auf Grundlage dessen einschränken, zu welchem Unternehmen sie gehören (**Personen in anderen Unternehmen sollten nur Benutzer von anzeigen**.

   Sie können die Benutzer darauf beschränken, nur Benutzer aus ihrer eigenen Firma oder aus der Firma anzuzeigen, die Sie als primäre Firma angegeben haben. Die Primärfirma stellt in der Regel Ihr Workfront-Konto dar, in dem die meisten Ihrer Benutzenden arbeiten. Weitere Informationen zur primären Firma finden Sie unter [Firmen erstellen und bearbeiten](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

   >[!NOTE]
   >
   >Wenn zwei Benutzer zu zwei verschiedenen Unternehmen gehören, aber beide Benutzer der primären Firma sehen können, können sie den Bereich Aktualisierungen sehen, der mit der primären Firma verknüpft ist.

1. (Optional) Um Zugriffseinstellungen für andere Objekte und Bereiche in der Zugriffsebene, an der Sie arbeiten, zu konfigurieren, fahren Sie mit einem der in [Zugriff auf Adobe Workfront konfigurieren](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md) aufgelisteten Artikel fort, z. B. [Zugriff auf Aufgaben gewähren](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md) und [Zugriff auf Finanzdaten gewähren](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
1. Klicken Sie auf **Speichern**.

   Nachdem die Zugriffsebene erstellt wurde, können Sie sie einem Benutzer zuweisen (es sei denn, es handelt sich um eine Systemadministrator-Zugriffsebene).

   Weitere Informationen finden Sie [Bearbeiten des Benutzerprofils](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

   Informationen dazu, wie ein Adobe-Administrator einem Benutzer eine Systemadministrator-Zugriffsebene zuweist, finden Sie unter [Gewähren des vollständigen Administratorzugriffs für einen Benutzer](../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md).

## Standard- oder Planer-Benutzer mit administrativem Zugriff auf Aufgabengebiete {#planner-users}

Wenn Sie einem Standard- oder Planer-Benutzer administrativen Zugriff auf Aufgabengebiete gewähren, wird die Einstellung „Funktion bearbeiten - Abrechnung und Kostensätze“ automatisch für den Benutzer aktiviert.

Wenn Sie später den administrativen Zugriff auf Aufgabengebiete für den Benutzer deaktivieren, sind Aufgabengebiete für den Benutzer weiterhin sichtbar, da die Einstellung „Aufgabengebiet bearbeiten - Abrechnung und Kostensätze“ weiterhin aktiviert ist.

Wenn dies eintritt und Sie den Zugriff des Benutzers auf die Anzeige von Aufgabengebieten entfernen müssen, müssen Sie die Berechtigungseinstellung „Rolle bearbeiten - Abrechnung und Kostensätze“ des Benutzers deaktivieren. Anweisungen finden Sie unter [Zugriff auf Finanzdaten gewähren](grant-access-financial.md).
