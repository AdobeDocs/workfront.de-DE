---
product-area: workfront-integrations
navigation-topic: workfront-for-jira
title: Verknüpfen von Elementen zwischen [!DNL Adobe Workfront] und [!DNL Jira]
description: Sie können [!DNL Jira] Probleme mit [!DNL Adobe Workfront] Aufgaben oder Problemen entweder automatisch oder manuell verknüpfen.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 1c37f361-e866-4ac6-b672-408848a80ed6
source-git-commit: f22a67cd3235a3111f7b874637ec05f8299de271
workflow-type: tm+mt
source-wordcount: '1158'
ht-degree: 0%

---

# Verknüpfen von Elementen zwischen [!DNL Adobe Workfront] und [!DNL Jira]

Sie können [!DNL Jira]-Probleme mit [!DNL Adobe Workfront] Aufgaben oder Problemen entweder automatisch oder manuell verknüpfen.

Nur ein Element in [!DNL Workfront] kann mit einem Element in [!DNL Jira] verknüpft werden. Sie können nie ein [!DNL Workfront] Element mit mehreren [!DNL Jira] Problemen verknüpfen oder ein [!DNL Jira] Problem mit mehreren [!DNL Workfront] Elementen.

## Zugriffsanforderungen

Sie müssen über Folgendes verfügen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">[!DNL [!DNL Adobe Workfront] plan]</a>*</td> 
   <td> <p>[!UICONTROL Pro] oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe [!DNL Workfront] Lizenzübersicht</a>*</td> 
   <td> <p>Plan</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Zugriff auf Jira</td> 
   <td> <p>Systemadministratorzugriff</p> <p><b>WICHTIG</b>

Es wird empfohlen, separate Systemadministratorkonten in [!DNL Jira] und [!DNL Workfront] zu erstellen, um diese Integration zu widmen, anstatt vorhandene Konten zu verwenden, die möglicherweise an Benutzer angehängt sind.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Sie müssen ein [!DNL Workfront] -Administrator sein. Weitere Informationen zu [!DNL Workfront] -Administratoren finden Sie unter <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Gewähren eines vollen Administratorzugriffs für einen Benutzer</a>.</p> <p><b>NOTIZ</b>

Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren [!DNL Workfront] -Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein [!DNL Workfront] -Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td>
</tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren [!DNL Workfront] -Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Voraussetzungen

Bevor Sie Elemente zwischen [!DNL Workfront] und [!DNL Jira] verknüpfen können, müssen Sie

* Installieren Sie [!DNL Workfront] für [!DNL Jira]

  Anweisungen zum Installieren von Workfront für Jira finden Sie unter [Installieren von Adobe Workfront für Jira](../../workfront-integrations-and-apps/use-workfront-with-jira/install-workfront-for-jira.md).

* Konfigurieren von [!DNL Workfront] für Jira

  Anweisungen zum Konfigurieren von Workfront für Jira finden Sie unter [Adobe Workfront für Jira konfigurieren](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

## Automatisch [!DNL Workfront] Elemente mit [!DNL Jira] Problemen verknüpfen

Als [!DNL Workfront] -Administrator können Sie Trigger definieren, die automatisch ein Problem in [!DNL Jira] erstellen können, sobald bestimmte Bedingungen für eine Aufgabe oder ein Problem in [!DNL Workfront] erfüllt sind. Die Elemente Workfront und [!DNL Jira] werden verknüpft.

Wenn Sie die Konfiguration von [!DNL Workfront] für Jira abgeschlossen haben und ein Element entweder in [!DNL Workfront] erstellt oder aktualisiert wird, um Ihren Triggern zu entsprechen, wird automatisch ein neues Element in [!DNL Jira] erstellt.\
Workfront-Benutzer, die Workfront-Elemente erstellen und aktualisieren, benötigen keine [!DNL Jira] -Lizenz, um die Erstellung von Elementen in [!DNL Jira] Trigger.

Weitere Informationen zum Definieren von Triggern zum automatischen Erstellen von Jira-Problemen finden Sie unter [Konfigurieren von  [!DNL Adobe Workfront] für Jira](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

>[!NOTE]
>
>Sie können [!DNL Jira] -Elemente automatisch erstellen, indem Sie eine Vorlage an ein Projekt anhängen. Wenn die Vorlage Aufgaben mit Zuweisungen enthält, die den [!DNL Jira] -Triggern entsprechen, verursachen die neuen Aufgaben neue [!DNL Jira]-Probleme.

Die automatische Verknüpfung eines [!DNL Workfront] -Problems mit einem [!DNL Jira] -Problem ist identisch mit der automatischen Verknüpfung einer [!DNL Workfront] -Aufgabe mit einem [!DNL Jira] -Problem.

So verknüpfen Sie eine [!DNL Workfront] -Aufgabe automatisch mit einem [!DNL Jira] -Problem:

1. Stellen Sie sicher, dass Ihr [!DNL Jira] -Systemadministrator Trigger für die automatische Erstellung von [!DNL Jira] Problemen bei der Zuweisung von [!DNL Workfront] -Elementen konfiguriert hat, und melden Sie sich dann bei [!DNL Workfront] mit einer Zugriffsebene an, über die Sie eine Aufgabe erstellen können.

   Weitere Informationen zum Zugriff auf Aufgaben finden Sie unter [Zugriff auf Aufgaben gewähren](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md).

1. Wechseln Sie zu einem Projekt und wählen Sie im linken Bereich **[!UICONTROL Aufgaben]** ![](assets/tasks-icon-in-left-panel-14x14.png) aus.

1. Klicken Sie auf **[!UICONTROL Neue Aufgabe]**

   Oder

   Wählen Sie eine vorhandene Aufgabe aus und klicken Sie dann auf **Bearbeiten**.

1. Geben Sie eines der für die Aufgabe verfügbaren Felder an oder aktualisieren Sie es.
1. Klicken Sie auf **[!UICONTROL Zuweisungen]** und weisen Sie die Aufgabe einem Benutzer, einer Rolle oder einem Team zu, der bzw. das als Trigger in der [!DNL Jira] -Integration angegeben ist.

1. Klicken Sie auf **Änderungen speichern**.

   In Workfront wird eine neue Aufgabe erstellt.

   Im Bereich **[!UICONTROL Aktualisierungen]** der neuen Aufgabe gibt es einen Kommentar, der angibt, dass auch in [!DNL Jira] ein neues Problem erstellt wurde.

1. (Optional) Klicken Sie auf den Link zum Jira-Problem, um es in Jira zu öffnen.

   Oder

   Klicken Sie auf den Link **[!UICONTROL Gehe zu Jira]** im Bereich **[!UICONTROL Integrationen]** des Abschnitts **[!UICONTROL Details]** oder in der Aufgaben- oder Problemkopfzeile, um das Problem [!DNL Jira] zu öffnen.

   Ihr System- oder Gruppenadministrator muss das Feld [!UICONTROL Integrationen] zu Ihrer Layoutvorlage hinzufügen, um es in der Aufgaben- oder Problemkopfzeile anzuzeigen. Weitere Informationen finden Sie unter [Anpassen von Objektüberschriften mithilfe einer Layoutvorlage](../../administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md).

   Jeder [!DNL Jira] -Benutzer kann sofort mit der Arbeit an Artikeln beginnen, die automatisch aus [!DNL Workfront] erstellt wurden, und seine Aktualisierungen werden an [!DNL Workfront] übertragen, ohne dass dafür eine Lizenz für [!DNL Workfront] erforderlich ist.

   Nur die Felder, die Sie als [!DNL Workfront] -Administrator während der Einrichtung des [!DNL Workfront] -Add-ons konfiguriert haben, werden aktualisiert.

   Weitere Informationen zum Synchronisieren von Feldern zwischen Workfront und Jira finden Sie im Abschnitt [Workfront für Jira konfigurieren](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md#configuring-the-add-on-for-jira) in [Adobe Workfront für Jira konfigurieren](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md) .

   >[!NOTE]
   >
   >Das Problem [!DNL Jira] wird in [!DNL Jira] niemandem zugewiesen, wenn es automatisch aus Workfront erstellt wird.

## Manuelles Verknüpfen von [!DNL Jira]-Problemen mit [!DNL Workfront]-Elementen

Nachdem Elemente in [!DNL Jira] und [!DNL Workfront] erstellt wurden, können Sie unabhängig voneinander ein [!DNL Jira] -Problem manuell mit einer vorhandenen [!DNL Workfront] -Aufgabe oder einem vorhandenen Problem verknüpfen.\
Ein [!DNL Workfront] -Element von [!DNL Workfront] kann nicht manuell mit einem vorhandenen [!DNL Jira] -Element verknüpft werden.

>[!NOTE]
>
>Wenn sich das Problem [!DNL Jira] nicht in einem Projekt befindet, das in der [!DNL Workfront] -Integration nicht als Trigger identifiziert wurde, können Sie es nicht manuell mit einem Workfront-Element verknüpfen, wenn Sie die Integration mit [!DNL Jira] On-Premise verwenden.\
>Weitere Informationen zum Einrichten von Triggern für den Workflow &quot;Workfront to Jira&quot;finden Sie unter [Automatisches Verknüpfen von Workfront-Elementen mit Jira-Problemen](#automatically-link-workfront-items-to-jira-issues).

Wenn die Elemente [!DNL Workfront] und [!DNL Jira] verknüpft sind, können bestimmte Felder aus einem Element automatisch auf dem anderen aktualisiert werden.\
Weitere Informationen zum Aktualisieren verknüpfter Elemente finden Sie unter [Aktualisieren verknüpfter Elemente zwischen Jira und Adobe Workfront](../../workfront-integrations-and-apps/use-workfront-with-jira/update-linked-items-between-jira-wf.md).

So verknüpfen Sie [!DNL Jira]-Probleme manuell mit [!DNL Workfront] -Elementen:

1. (Bedingt) Melden Sie sich bei [!DNL Workfront] an und suchen Sie nach einem Problem oder einer Aufgabe, die Sie mit dem Problem [!DNL Jira] verknüpfen möchten.
1. (Bedingt) Kopieren Sie in der Adressleiste des Elements die **URL** des Elements in Workfront.

   Oder

   Kopieren Sie aus dem Bereich [!UICONTROL Details] die **[!UICONTROL Referenznummer]** des Elements in Workfront.

   >[!NOTE]
   >
   >Sie müssen über eine [!DNL Workfront] -Lizenz verfügen, um sich bei [!DNL Workfront] anzumelden. Andernfalls muss Ihnen ein [!DNL Workfront] -Benutzer diese Informationen bereitstellen.

1. Navigieren Sie in [!DNL Jira] zu einem Problem, das Sie manuell mit dem Element [!DNL Workfront] verknüpfen möchten.
1. Fügen Sie im rechten Bereich [!DNL Workfront] die **URL** oder die **[!UICONTROL Referenz-Nummer]** des Elements [!DNL Workfront] ein, mit dem Sie eine Verknüpfung herstellen möchten.

1. Klicken Sie auf **[!UICONTROL Link]**.

   Die beiden Elemente werden verknüpft und das rechte Bedienfeld [!DNL Workfront] wird mit Informationen aus dem Element [!DNL Workfront] gefüllt.

   Die folgenden [!DNL Workfront] -Felder sind in [!DNL Jira] standardmäßig im rechten Bereich [!DNL Workfront] sichtbar:

   * Der **[!UICONTROL Name]** des Elements: Sie können auf das Element [!DNL Workfront] zugreifen, indem Sie auf den Namen im Bedienfeld klicken.
   * **[!UICONTROL Projektname]**
   * Der **[!UICONTROL Status]** des Elements
   * Die **[!UICONTROL Priorität]** des Elements
   * Das Datum, an dem es in [!DNL Workfront] erstellt wurde
   * Die **[!UICONTROL geplanten Stunden]** des Elements
   * Die **[!UICONTROL Referenz-Nummer]**: Sie können auf das Element [!DNL Workfront] zugreifen, indem Sie auf die [!UICONTROL Referenz-Nummer] im Bedienfeld klicken.

Weitere Informationen zum Aktivieren zusätzlicher Felder für die Anzeige im rechten Bereich finden Sie im Abschnitt [Konfigurieren der Feldsynchronisierung zwischen [!DNL Jira] und [!DNL Workfront] Elementen](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md#setting-up-field-synchronization) in [Konfigurieren [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md). Ein Kommentar des mit der Integration verknüpften [!DNL Workfront] -Administrators wird auf der Registerkarte **[!DNL Workfront]** des [!DNL Jira] -Problems veröffentlicht, um zu bestätigen, dass ein neues [!DNL Jira] -Element erstellt wurde. Der Kommentar enthält einen Link zum Problem [!DNL Jira].

## Aufheben der Verknüpfung zwischen [!DNL Jira] und [!DNL Workfront]

Verknüpfte Elemente zwischen [!DNL Jira] und [!DNL Workfront] können manuell von [!DNL Jira] getrennt werden.\
Sie können die Verknüpfung eines [!DNL Workfront] -Elements mit ihrem [!DNL Jira]-Gegenstück in [!DNL Workfront] nicht aufheben.

Sie benötigen den folgenden Zugriff, um die Verknüpfung manuell verknüpfter Elemente aufzuheben:

* Sie sind der Benutzer, der die Elemente manuell verknüpft hat
* Sie sind der [!DNL Jira]-Systemadministrator

Nur ein [!DNL Workfront] -Administrator kann die Verknüpfung von automatisch verknüpften Elementen aufheben.

So stellen Sie die Verknüpfung eines [!DNL Jira] -Problems mit einem [!DNL Workfront] -Element auf:

1. Navigieren Sie in [!DNL Jira] zu einem Problem, das mit einer [!DNL Workfront] -Aufgabe oder einem Problem verknüpft ist.
1. Wechseln Sie zum rechten Bereich [!DNL Workfront], klicken Sie auf das Symbol **[!UICONTROL Verknüpfung aufheben]** und dann auf **[!UICONTROL Verknüpfung aufheben]**.

   Die zuvor verknüpften Elemente [!DNL Jira] und [!DNL Workfront] sind jetzt nicht mehr verknüpft. Alle Felder, Kommentare oder Dokumente, die später einzeln aktualisiert werden, werden nicht über ihre Vorgängerelemente in der anderen Anwendung aktualisiert.
