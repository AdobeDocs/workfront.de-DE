---
title: Benutzerdefinierte Zugriffsebenen erstellen und ändern
user-type: administrator
product-area: system-administration;user-management
navigation-topic: configure-access-to-workfront
description: Als Adobe Workfront-Administrator können Sie benutzerdefinierte Zugriffsebenen erstellen und diese auf Benutzer anwenden.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: d2a73d24-51d3-42e2-9c09-7f4bc30b2caa
source-git-commit: 4cab7bed6cb4c25d96e70ccce2ece7f6d156f435
workflow-type: tm+mt
source-wordcount: '1463'
ht-degree: 6%

---

# Benutzerdefinierte Zugriffsebenen erstellen und ändern

<!--Audited: 12/2023-->

<!--Don't delete, draft, or change the title of this article. The UI links to it via context-sensitive help. -->

Als Adobe Workfront-Administrator können Sie benutzerdefinierte Zugriffsebenen erstellen und diese auf Benutzer anwenden. Bei der Arbeit mit Zugriffsebenen ist es wichtig zu verstehen, wie sie mit den Objektberechtigungen zusammenarbeiten, die Benutzer gewähren, wenn sie Objekte miteinander teilen. Weitere Informationen zu Zugriffsebenen finden Sie unter:

* [Übersicht über die neuen Zugriffsebenen](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/access-level-overview.md)
* [Übersicht über Zugriffsebenen](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md)

>[!IMPORTANT]
>
>Wir empfehlen dringend, die integrierten Zugriffsebenen unverändert zu lassen, damit Sie nach der Einrichtung Ihrer Benutzer darauf verweisen können. Um eine Zugriffsebene anzupassen, kopieren Sie die standardmäßige Zugriffsebene und ändern Sie die Kopie. Sie können dies für jede Zugriffsstufe mit Ausnahme von &quot;Systemadministrator&quot;und &quot;Externer Benutzer&quot;tun.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Abo</td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td>Neu: Standard
   <p>oder</p>
   <p>Aktuell: Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Sie müssen Workfront-Administrator sein.</p></td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Benutzerdefinierte Zugriffsebene erstellen oder bearbeiten

{{step-1-to-setup}}

1. Klicks **Zugriffsebenen** im linken Bereich.
1. Wählen Sie die Zugriffsebene aus, die Sie kopieren und anpassen möchten, und klicken Sie auf **Kopieren**.

   Oder

   Wenn Sie eine vorhandene Zugriffsebene bearbeiten (die Sie zuvor kopiert haben), klicken Sie auf deren Namen.

1. Führen Sie im angezeigten Feld einen der folgenden Schritte aus, um die benutzerdefinierte Zugriffsebene zu konfigurieren:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Name</td> 
      <td> <p>Geben Sie einen Namen für Ihre Zugriffsebene ein. </p> <p>Wenn Sie gerade eine Zugriffsebene kopiert haben, um eine neue zu erstellen, lautet der Standardname Zugriffsstufenname (Kopie), wobei Zugriffsstufenname die von Ihnen kopierte Zugriffsebene ist.</p> <p><strong>Tipp</strong>: Es wird empfohlen, den ursprünglichen Namen der Zugriffsebene in den Namen der Kopie einzufügen. Im ACME-Unternehmen kann beispielsweise eine Kopie der Standardzugriffsstufe ACME Standard heißen.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Beschreibung </td> 
      <td>Geben Sie eine Beschreibung für die Zugriffsebene ein. Es ist hilfreich, hier aufzulisten, was ein Benutzer mit dieser Zugriffsstufe erreichen kann.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Lizenztyp</td> 
      <td>Stellen Sie sicher, dass die hier ausgewählte Lizenz die am ehesten mit der Art der Zugriffsebene in Verbindung stehende Lizenz ist, die Sie erstellen oder bearbeiten. Die ausgewählte Lizenz bestimmt, welche Einstellungen für die Zugriffsebene verfügbar sind. Weitere Informationen finden Sie unter <a href="/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/licenses-overview.md" class="MCXref xref">Übersicht über neue Lizenzen</a> oder <a href="/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md">Überblick über Lizenzen</a>.</td> 
     </tr> 
    </tbody> 
   </table>

1. (Bedingt) Wenn **Standard** oder **Plan** wird im Feld **Lizenztyp** zum Bereich **Administratorzugriff zulassen für** und wählen Sie die administrativen Zugriffsberechtigungen für diejenigen aus, die diese Zugriffsebene haben werden.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Genehmigungsprozesse</td> 
      <td>Erstellen und verwalten Sie Validierungsprozesse für die Verwendung im gesamten System und für bestimmte Gruppen.<p>Ohne diesen Zugriff können Benutzer nur Ad-hoc-Genehmigungsprozesse für Elemente erstellen, auf die sie Zugriff haben.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Firmen</td> 
      <td>Fügen Sie neue hinzu und bearbeiten Sie bestehende Unternehmen in Workfront.<br><p>Ohne diesen Zugriff können Benutzer nur bestehende Unternehmen anzeigen.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Benutzerdefinierte Formulare</td> 
      <td>Erstellen und verwalten Sie alle benutzerdefinierten Formulare in ihrer Gruppe. <br><p>Ohne diesen Zugriff können Benutzer nur vorhandene Formulare an Objekte anhängen, auf die sie Zugriff haben, um sie beizutragen oder zu verwalten.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Wechselkurse</td> 
      <td> Neue Währung in Workfront hinzufügen. <p>Ohne diesen Zugriff kann der Benutzer eine vorhandene Währung nur zu einem von ihm erstellten Projekt hinzufügen.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ausgaben</td> 
      <td>Zeigen Sie alle Ausgaben für Objekte in Workfront an.<p>Ohne diesen Zugriff kann der Benutzer nur Folgendes anzeigen:</p>
       <ul>
        <li>Ausgaben für von ihnen verwaltete Projekte, Aufgaben oder Probleme</li>
        <li>Ihre eigenen Ausgaben</li>
        <li>Die Kosten für ihre Untergebenen</li>
       </ul><p><b>NOTE</b>: Benutzer können hierdurch keine neuen Ausgabetypen erstellen.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Aufgabengebiete</td> 
      <td> Mit diesem Zugriff kann der Benutzer Folgendes tun: 
       <ul> 
        <li>Vorhandene Auftrags-Rollen anzeigen und bearbeiten</li> 
        <li>Hinzufügen neuer Vorgangsrollen</li> 
        <li>Bearbeiten der Rollenabrechnung und der Kostensätze</li> 
       </ul> 
       <p>Wichtige Informationen zum Zugriff auf Finanzdaten, die einem Standard- oder Planer-Benutzer mit Administratorzugriff auf Stellenrollen zur Verfügung stehen, finden Sie unter <a href="#standard-or-planner-users-with-administrative-access-to-job-roles">Standard- oder Planer-Benutzer mit Administratorzugriff auf Stellenrollen</a>.</p>
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Meilensteine in meiner Gruppe</td> 
      <td>Zeigen Sie alle Meilensteinpfade im System unter dem Menü Meilensteinpfade im Setup an. Benutzer können auch alle Meilensteinpfade bearbeiten oder löschen, die zu einer ihrer Gruppen gehören. Benutzer können keine Meilensteinpfade verwalten (bearbeiten oder löschen), die ihren Gruppen nicht zugewiesen sind.<p>Ohne diesen Zugriff können Benutzer nur vorhandene Meilensteinpfade anzeigen und auf Projekte anwenden, auf die sie Zugriff haben.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Erinnerungsbenachrichtigungen</td> 
      <td>Erstellen und verwalten Sie Erinnerungsbenachrichtigungen in Workfront.<p>Ohne diesen Zugriff sind Benutzer auf den Empfang und die Anzeige von Benachrichtigungen beschränkt.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Arbeitszeittabellen und Stunden</td> 
      <td> Gruppenadministratoren können Benutzern in den von ihnen verwalteten Gruppen und Untergruppen Timesheet-Profile zuweisen. <p>Wenn diese Option nicht aktiviert ist, können Gruppenadministratoren anderen Benutzern in den von ihnen verwalteten Gruppen und Untergruppen keine Zeitleistenprofile zuweisen, obwohl sie diese erstellen können.</p> <p>Alle anderen Benutzer mit einer Standard- oder Planungslizenz können alle Stunden und Zeitpläne in Workfront anzeigen.</p> <p>Wenn diese Option nicht aktiviert ist, können Benutzer Stunden nur in folgenden Bereichen anzeigen:</p> 
       <ul> 
        <li>Von ihnen verwaltete Projekte, Aufgaben oder Probleme</li> 
        <li>Ihre eigenen Zeitpläne</li> 
        <li>Ein Timesheet für einen Benutzer, der ihm Berichte übermittelt</li> 
        <li>Von ihnen genehmigte Zeitpläne</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. Klicks **Weitere Einschränkungen festlegen** und legen Sie dann eine der folgenden Einschränkungen für die Zugriffsebene fest.

   >[!IMPORTANT]
   >
   >Für externe Benutzer wie Anbieter (alle Personen, die nicht in Ihrer Organisation arbeiten) empfehlen wir, den Zugriff auf Aufgaben, Projekte, Updates, Mitteilungen, andere Unternehmen, Teams und Gruppen zu beschränken.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Nie Zugriff auf das gesamte Projekt geben, wenn einer Aufgabe oder einem Problem zugeordnet</td> 
      <td> Verhindert, dass Benutzern, die Aufgaben oder Problemen zugewiesen sind, auch Berechtigungen für das übergeordnete Projekt erhalten, selbst wenn die Projektberechtigungen dies zulassen.<p>Weitere Informationen zum Konfigurieren der Berechtigungen für ein Projekt finden Sie im Abschnitt <a href="../../../manage-work/projects/manage-projects/edit-projects.md#access" class="MCXref xref"></a> im Artikel <a href="../../../manage-work/projects/manage-projects/edit-projects.md" class="MCXref xref">Projekte bearbeiten</a>.</p></td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Nie den Dokumentzugriff aus Projekten, Aufgaben, Problemen etc. erben</td> 
      <td>Verhindert, dass Dokumente die für ihr übergeordnetes Objekt festgelegten Berechtigungen übernehmen.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Nur Aktualisierungen anzeigen, in denen Sie an der Konversation beteiligt waren</td> 
      <td> Ermöglicht Benutzern, nur Kommentare anzuzeigen, in denen ihr Name oder der Name ihres Teams enthalten war. <p> <p><b>NOTE</b>: Dadurch wird verhindert, dass Benutzer Artikel in Workfront abonnieren. Weitere Informationen zum Abonnieren von Elementen finden Sie unter <a href="../../../workfront-basics/using-notifications/subscribe-to-items-in-workfront.md" class="MCXref xref">Abonnieren von Elementen in Adobe Workfront</a>.</p> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Nicht zulassen, dass Benutzer Kommentare löschen </td> 
      <td> Verhindert, dass Benutzer Kommentare zu Elementen löschen.  <p><b>NOTE</b>: Keiner kann die Kommentare anderer Benutzer löschen.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Nur Firmen, Gruppen &amp; Teams anzeigen, der Sie angehören</td> 
      <td>Ermöglicht Benutzern, Elemente nur für Unternehmen, Gruppen und Teams anzuzeigen und freizugeben, denen sie angehören.<p><strong>NOTE</strong>: Benutzer mit Anfragenlizenzen können keine Unternehmen anzeigen, zu denen sie nicht gehören, selbst wenn diese Option aktiviert ist.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Anzeige von "Geplante Stunden" oder "Tatsächliche Stunden" nicht zulassen</td> 
      <td>Verhindert, dass Benutzer die geplanten und tatsächlichen Stunden der Arbeitselemente sehen, auf die sie Zugriff haben. Sie können jedoch die tatsächlichen Stunden sehen, die sie selbst melden, oder Stunden, die von einem Benutzer protokolliert werden, der sie meldet.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Nie zulassen, dass Benutzer Ankündigungen löschen</td> 
      <td>Verhindert, dass Benutzer Ankündigungen im Ankündigungs-Center löschen. Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/get-started-wf-administration/view-send-announcements.md" class="MCXref xref">Mitteilungen senden</a>.</td> 
     </tr> 
    </tbody> 
   </table>

1. (Bedingt und optional) Wenn Ihr Workfront-System für Benutzer eingerichtet ist, die mehreren Unternehmen angehören, beschränken Sie die Sichtbarkeit auf andere Benutzer, basierend darauf, zu welchem Unternehmen sie gehören. **Personen in anderen Unternehmen sollten nur Benutzer von**.

   Sie können die Benutzer so einschränken, dass sie nur Benutzer aus ihrem eigenen Unternehmen oder aus dem Unternehmen sehen, das Sie als Hauptunternehmen benannt haben. Das primäre Unternehmen stellt normalerweise Ihr Workfront-Konto dar, in dem die meisten Ihrer Benutzer arbeiten. Weitere Informationen zum primären Unternehmen finden Sie unter [Erstellen und Bearbeiten von Unternehmen](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

   >[!NOTE]
   >
   >Wenn zwei Benutzer zu zwei verschiedenen Unternehmen gehören, aber beide Benutzer vom primären Unternehmen sehen können, können sie den Bereich Updates sehen, der mit dem primären Unternehmen verknüpft ist.

1. (Optional) Um die Zugriffseinstellungen für andere Objekte und Bereiche in der Zugriffsebene zu konfigurieren, mit einem der Artikel fortzufahren, die unter [Zugriff auf Adobe Workfront konfigurieren](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md), beispielsweise [Zugriff auf Aufgaben gewähren](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md) und [Zugriff auf Finanzdaten gewähren](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
1. Klicken Sie auf **Speichern**.

   Nachdem die Zugriffsebene erstellt wurde, können Sie sie einem Benutzer zuweisen (es sei denn, es handelt sich um eine Zugriffsstufe für Systemadministratoren).

   Weitere Informationen finden Sie unter [Profil eines Benutzers bearbeiten](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

   Informationen dazu, wie ein Adobe-Administrator einem Benutzer eine Systemadministratorzugriffsstufe zuweist, finden Sie unter [Gewähren eines vollen Administratorzugriffs](../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md).

## Standard- oder Planer-Benutzer mit Administratorzugriff auf Stellenrollen {#planner-users}

Wenn Sie einem Standard- oder Planer-Benutzer Administratorzugriff auf Stellenrollen gewähren, wird die Einstellung Rollenabrechnung und -kosten bearbeiten automatisch für den Benutzer aktiviert.

Wenn Sie später den administrativen Zugriff auf Stellenrollen für den Benutzer deaktivieren, sind die Arbeitsplatzrollen für den Benutzer weiterhin sichtbar, da die Einstellung Rollenabrechnung und -kosten bearbeiten weiterhin aktiviert ist.

Wenn dies eintritt und Sie den Zugriff des Benutzers entfernen müssen, um Vorgangsrollen anzuzeigen, müssen Sie die Berechtigungseinstellung &quot;Rollenabrechnung und -kosten bearbeiten&quot;des Benutzers deaktivieren. Anweisungen finden Sie unter [Zugriff auf Finanzdaten gewähren](grant-access-financial.md).
