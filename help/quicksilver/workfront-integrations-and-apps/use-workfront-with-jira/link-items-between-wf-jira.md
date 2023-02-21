---
product-area: workfront-integrations
navigation-topic: workfront-for-jira
title: Elemente verknüpfen zwischen [!DNL Adobe Workfront] und [!DNL Jira]
description: Sie können [!DNL Jira] Probleme [!DNL Adobe Workfront] Aufgaben oder Probleme entweder automatisch oder manuell.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 1c37f361-e866-4ac6-b672-408848a80ed6
source-git-commit: f22a67cd3235a3111f7b874637ec05f8299de271
workflow-type: tm+mt
source-wordcount: '1160'
ht-degree: 0%

---

# Elemente verknüpfen zwischen [!DNL Adobe Workfront] und [!DNL Jira]

Sie können [!DNL Jira] Probleme [!DNL Adobe Workfront] Aufgaben oder Probleme entweder automatisch oder manuell.

Nur ein Element in [!DNL Workfront] kann mit einem Element in [!DNL Jira]. Sie können nie eine [!DNL Workfront] Element zu mehreren [!DNL Jira] Fragen oder [!DNL Jira] Problem bei mehreren [!DNL Workfront] Elemente.

## Zugriffsanforderungen

Sie müssen über Folgendes verfügen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">[!DNL [!DNL Adobe Workfront] Plan]</a>*</td> 
   <td> <p>[!UICONTROL Pro] oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe [!DNL Workfront] Lizenzübersicht</a>*</td> 
   <td> <p>Plan</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Zugriff auf Jira</td> 
   <td> <p>Systemadministratorzugriff</p> <p><b>WICHTIG</b>

Es wird empfohlen, separate Systemadministratorkonten in der [!DNL Jira] und [!DNL Workfront] , um dieser Integration zu widmen, anstatt vorhandene zu verwenden, die möglicherweise mit Benutzern verbunden sind.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Sie müssen [!DNL Workfront] Administrator. Informationen über [!DNL Workfront] Administratoren, siehe <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Gewähren eines vollen Administratorzugriffs</a>.</p> <p><b>NOTIZ</b>

Wenn Sie noch keinen Zugriff haben, fragen Sie Ihren [!DNL Workfront] Administrator , wenn sie zusätzliche Einschränkungen für Ihre Zugriffsebene festlegen. Für Informationen zur [!DNL Workfront] Administrator kann Ihre Zugriffsebene ändern, siehe <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td>
</tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren [!DNL Workfront] Administrator.

## Voraussetzungen

Bevor Sie Elemente verknüpfen können zwischen [!DNL Workfront] und [!DNL Jira], müssen Sie

* Installieren [!DNL Workfront] für [!DNL Jira]

   Anweisungen zur Installation von Workfront für Jira finden Sie unter [Installieren von Adobe Workfront für Jira](../../workfront-integrations-and-apps/use-workfront-with-jira/install-workfront-for-jira.md).

* Konfigurieren [!DNL Workfront] für Jira

   Anweisungen zum Konfigurieren von Workfront für Jira finden Sie unter [Adobe Workfront für Jira konfigurieren](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

## Automatische Verknüpfung [!DNL Workfront] Elemente [!DNL Jira] issues

Als [!DNL Workfront] Administrator können Sie Trigger definieren, die automatisch ein Problem in [!DNL Jira] jedes Mal, wenn bestimmte Bedingungen für eine Aufgabe oder ein Problem in [!DNL Workfront]. Die Workfront und [!DNL Jira] Elemente werden verknüpft.

Nachdem Sie die Konfiguration von [!DNL Workfront] für Jira, wenn ein Element entweder in erstellt oder aktualisiert wird [!DNL Workfront] , um Ihren Triggern zu entsprechen, wird automatisch ein neues Element in [!DNL Jira].\
Workfront-Benutzer, die Workfront-Elemente erstellen und aktualisieren, benötigen keine [!DNL Jira] -Lizenz zum Trigger der Erstellung von Elementen in [!DNL Jira].

Weitere Informationen zum Definieren von Triggern zum automatischen Erstellen von Jira-Problemen finden Sie unter  [Konfigurieren [!DNL Adobe Workfront] für Jira](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

>[!NOTE]
>
>Sie können [!DNL Jira] -Elemente automatisch, indem Sie eine Vorlage an ein Projekt anhängen. Wenn die Vorlage Aufgaben mit Zuweisungen enthält, die der [!DNL Jira] Trigger, die neuen Aufgaben generieren neue [!DNL Jira] Probleme.

Automatisches Verknüpfen eines [!DNL Workfront] ein Problem [!DNL Jira] -Problem mit der automatischen Verknüpfung einer [!DNL Workfront] Aufgabe an eine [!DNL Jira] Problem.

So verknüpfen Sie automatisch [!DNL Workfront] Aufgabe an eine [!DNL Jira] Problem:

1. Stellen Sie sicher, dass [!DNL Jira] Systemadministrator hat Trigger für die automatische Erstellung konfiguriert [!DNL Jira] Probleme beim [!DNL Workfront] -Elemente zugewiesen werden, melden Sie sich dann bei [!DNL Workfront] mit einer Zugriffsebene, die die Erstellung einer Aufgabe ermöglicht.

   Weitere Informationen zum Zugriff auf Aufgaben finden Sie unter [Zugriff auf Aufgaben gewähren](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md).

1. Wechseln Sie zu einem Projekt und wählen Sie **[!UICONTROL Aufgaben]** ![](assets/tasks-icon-in-left-panel-14x14.png) im linken Bereich.

1. Klicken **[!UICONTROL Neue Aufgabe]**

   Oder

   Wählen Sie eine vorhandene Aufgabe aus und klicken Sie auf **Bearbeiten**.

1. Geben Sie eines der für die Aufgabe verfügbaren Felder an oder aktualisieren Sie es.
1. Klicken **[!UICONTROL Zuweisungen]** und weisen die Aufgabe einem Benutzer, einer Rolle oder einem Team zu, das bzw. das als Trigger im [!DNL Jira] Integration.

1. Klicken **Änderungen speichern**.

   In Workfront wird eine neue Aufgabe erstellt.

   Im **[!UICONTROL Updates]** -Bereich der neuen Aufgabe gibt es einen Kommentar, der angibt, dass auch ein neues Problem in erstellt wurde. [!DNL Jira].

1. (Optional) Klicken Sie auf den Link zum Jira-Problem, um es in Jira zu öffnen.

   Oder

   Klicken Sie auf **[!UICONTROL Gehe nach Jira]** im **[!UICONTROL Integrationen]** der **[!UICONTROL Details]** oder der Aufgaben- oder Problemkopfzeile, um die [!DNL Jira] Problem.

   Ihr System- oder Gruppenadministrator muss [!UICONTROL Integrationen] in Ihre Layout-Vorlage ein, um sie in der Aufgaben- oder Problemüberschrift anzuzeigen. Weitere Informationen finden Sie unter [Objektüberschriften mithilfe einer Layoutvorlage anpassen](../../administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md).

   Alle [!DNL Jira] Benutzer können sofort mit der Arbeit an Elementen beginnen, die automatisch aus [!DNL Workfront] und ihre Aktualisierungen werden an [!DNL Workfront] ohne eine Lizenz für [!DNL Workfront] um dies zu tun.

   Nur die Felder, die Sie als [!DNL Workfront] Administrator, der während der Einrichtung der [!DNL Workfront] -Add-on aktualisiert.

   Weitere Informationen zum Synchronisieren von Feldern zwischen Workfront und Jira finden Sie in der [Workfront für Jira konfigurieren](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md#configuring-the-add-on-for-jira) Abschnitt in  [Adobe Workfront für Jira konfigurieren](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

   >[!NOTE]
   >
   >Die [!DNL Jira] Das Problem wird niemandem in [!DNL Jira] wenn sie automatisch aus Workfront erstellt wird.

## Manuelle Verknüpfung [!DNL Jira] Probleme [!DNL Workfront] items

Nachdem Elemente in erstellt wurden [!DNL Jira] und [!DNL Workfront]unabhängig voneinander können Sie eine [!DNL Jira] Problem an bestehende [!DNL Workfront] Aufgabe oder Problem.\
Sie können eine [!DNL Workfront] Element aus [!DNL Workfront] zu [!DNL Jira] Element.

>[!NOTE]
>
>Wenn die Variable [!DNL Jira] Das Problem befindet sich nicht in einem Projekt, das nicht als Trigger im [!DNL Workfront] Integration: Bei Verwendung der Integration mit [!DNL Jira] On-Premise.\
>Weitere Informationen zum Einrichten von Triggern für den Workflow &quot;Workfront to Jira&quot;finden Sie unter [Workfront-Elemente automatisch mit Jira-Problemen verknüpfen](#automatically-link-workfront-items-to-jira-issues).

Wann [!DNL Workfront] und [!DNL Jira] Elemente verknüpft sind, können bestimmte Felder aus einem Element automatisch auf dem anderen aktualisiert werden.\
Weitere Informationen zum Aktualisieren verknüpfter Elemente finden Sie unter [Aktualisieren verknüpfter Elemente zwischen Jira und Adobe Workfront](../../workfront-integrations-and-apps/use-workfront-with-jira/update-linked-items-between-jira-wf.md).

Manuelle Verknüpfung [!DNL Jira] Probleme [!DNL Workfront] items:

1. (Bedingt) Anmelden bei [!DNL Workfront] und suchen Sie nach einem Problem oder einer Aufgabe, mit der Sie eine Verknüpfung herstellen möchten [!DNL Jira] Problem.
1. (Bedingt) Kopieren Sie in der Adressleiste des Elements die **URL** des Elements in Workfront.

   Oder

   Aus dem [!UICONTROL Details] Bereich, kopieren Sie die **[!UICONTROL Referenz Nr.]** des Elements in Workfront.

   >[!NOTE]
   >
   >Sie müssen über eine [!DNL Workfront] -Lizenz für die Anmeldung bei [!DNL Workfront]. Andernfalls wird ein [!DNL Workfront] -Benutzer muss Ihnen diese Informationen zur Verfügung stellen.

1. In [!DNL Jira], navigieren Sie zu einem Problem, das Sie manuell mit dem [!DNL Workfront] Element.
1. Im [!DNL Workfront] den rechten Bereich, fügen Sie die **URL** oder **[!UICONTROL Referenz Nr.]** des [!DNL Workfront] -Element, mit dem Sie ihn verknüpfen möchten.

1. Klicken **[!UICONTROL Link]**.

   Die beiden Elemente werden verknüpft und die [!DNL Workfront] Der rechte Bereich enthält Informationen aus dem [!DNL Workfront] Element.

   Folgendes [!DNL Workfront] -Felder sind sichtbar in [!DNL Jira], standardmäßig in der [!DNL Workfront] rechter Bereich:

   * Die **[!UICONTROL Name]** des Artikels: Sie können auf die [!DNL Workfront] Element durch Klicken auf den Namen im Bedienfeld ein.
   * **[!UICONTROL Projektname]**
   * Die **[!UICONTROL Status]** des Artikels
   * Die **[!UICONTROL Priorität]** des Artikels
   * Das Datum der Erstellung in [!DNL Workfront]
   * Die **[!UICONTROL Geplante Stunden]** des Artikels
   * Die **[!UICONTROL Referenz Nr.]**: Sie können auf die [!DNL Workfront] Element durch Klicken auf [!UICONTROL Referenz Nr.] im Bereich.

Weitere Informationen zum Aktivieren zusätzlicher Felder für die Anzeige im rechten Bereich finden Sie unter [Konfigurieren der Feldsynchronisierung zwischen [!DNL Jira] und [!DNL Workfront] Elemente](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md#setting-up-field-synchronization) Abschnitt in [Konfigurieren [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md). Ein Kommentar von [!DNL Workfront] -Administrator, der mit der Integration verknüpft ist, wird im **[!DNL Workfront]** des [!DNL Jira] Problem zur Bestätigung, dass ein neuer [!DNL Jira] -Element erstellt wurde. Der Kommentar enthält einen Link zum [!DNL Jira] Problem.

## Verknüpfung zwischen Elementen aufheben [!DNL Jira] und [!DNL Workfront]

Verknüpfte Elemente zwischen [!DNL Jira] und [!DNL Workfront] kann die Verknüpfung von [!DNL Jira].\
Die Verknüpfung einer [!DNL Workfront] -Element [!DNL Jira] Gegenstück in [!DNL Workfront].

Sie benötigen den folgenden Zugriff, um die Verknüpfung manuell verknüpfter Elemente aufzuheben:

* Sie sind der Benutzer, der die Elemente manuell verknüpft hat
* Sie sind [!DNL Jira] Systemadministrator

Nur ein [!DNL Workfront] -Administrator kann die Verknüpfung von automatisch verknüpften Elementen aufheben.

Aufheben der Verknüpfung [!DNL Jira] ein Problem aus [!DNL Workfront] item:

1. In [!DNL Jira], navigieren Sie zu einem Problem, das mit einem [!DNL Workfront] Aufgabe oder Problem.
1. Navigieren Sie zu [!DNL Workfront] und klicken Sie auf das **[!UICONTROL Verknüpfung aufheben]** und klicken Sie auf **[!UICONTROL Verknüpfung aufheben]**.

   Die zuvor verknüpfte [!DNL Jira] und [!DNL Workfront] -Elemente sind jetzt nicht mehr verknüpft. Alle Felder, Kommentare oder Dokumente, die später einzeln aktualisiert werden, werden nicht über ihre Vorgängerelemente in der anderen Anwendung aktualisiert.
