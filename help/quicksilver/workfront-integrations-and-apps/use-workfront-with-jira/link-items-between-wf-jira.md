---
product-area: workfront-integrations
navigation-topic: workfront-for-jira
title: Elemente verknüpfen zwischen [!DNL Adobe Workfront] und [!DNL Jira]
description: Sie können Probleme  [!DNL Jira]  Aufgaben oder  [!DNL Adobe Workfront]  entweder automatisch oder manuell verknüpfen.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 1c37f361-e866-4ac6-b672-408848a80ed6
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '1231'
ht-degree: 0%

---

# Elemente zwischen [!DNL Adobe Workfront] und [!DNL Jira] verknüpfen

Sie können [!DNL Jira] Probleme entweder automatisch oder manuell mit [!DNL Adobe Workfront] Aufgaben oder Problemen verknüpfen.

Nur ein Element in [!DNL Workfront] kann mit einem Element in [!DNL Jira] verknüpft werden. Sie können niemals ein [!DNL Workfront] mit mehreren [!DNL Jira] oder ein [!DNL Jira] mit mehreren [!DNL Workfront] verknüpfen.

## Zugriffsanforderungen

Sie müssen über Folgendes verfügen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://business.adobe.com/products/workfront/pricing.html" target="_blank">[!DNL [!DNL Adobe Workfront]]</a>*</td> 
   <td> <p>[!UICONTROL Pro] oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Übersicht über Adobe [!DNL Workfront]-Lizenzen</a>*</td> 
   <td> <p>Plan</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Jira-Zugriff</td> 
   <td> <p>Systemadministratorzugriff</p> <p><b>WICHTIG</b>

Es wird empfohlen, separate Systemadministratorkonten in [!DNL Jira] und [!DNL Workfront] zu erstellen, um diese Integration zu ermöglichen, anstatt vorhandene Konten zu verwenden, die an Benutzer angehängt sein könnten.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene*</td> 
   <td> <p>Sie müssen [!DNL Workfront] sein. Informationen zu [!DNL Workfront] finden Sie unter <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Gewähren des vollständigen Administratorzugriffs für einen Benutzer</a>.</p> <p><b>NOTIZ</b>

Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren [!DNL Workfront], ob er zusätzliche Einschränkungen in Ihrer Zugriffsebene festlegt. Informationen dazu, wie [!DNL Workfront]-Admins Ihre Zugriffsebene ändern können, finden Sie unter <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Erstellen oder Ändern benutzerdefinierter Zugriffsebenen</a>.</p> </td>
</tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren [!DNL Workfront], um herauszufinden, über welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie verfügen.

## Voraussetzungen

Bevor Sie Elemente zwischen [!DNL Workfront] und [!DNL Jira] verknüpfen können, müssen Sie

* Installieren von [!DNL Workfront] für [!DNL Jira]

  Anweisungen zur Installation von Workfront für Jira finden Sie unter [Installieren von Adobe Workfront für Jira](../../workfront-integrations-and-apps/use-workfront-with-jira/install-workfront-for-jira.md).

* Konfigurieren von [!DNL Workfront] für Jira

  Anweisungen zum Konfigurieren von Workfront für Jira finden Sie unter [Konfigurieren von Adobe Workfront für Jira](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

## [!DNL Workfront] Elemente automatisch mit [!DNL Jira] Problemen verknüpfen

Als [!DNL Workfront] können Sie Trigger definieren, die automatisch ein Problem in [!DNL Jira] erstellen, sobald bestimmte Bedingungen für eine Aufgabe oder ein Problem in [!DNL Workfront] erfüllt werden. Die Workfront- und [!DNL Jira]-Elemente werden verknüpft.

Nachdem Sie die Konfiguration von [!DNL Workfront] für Jira abgeschlossen haben und ein Element entweder erstellt oder aktualisiert wird, [!DNL Workfront] es Ihren Triggern entspricht, wird automatisch ein neues Element in [!DNL Jira] erstellt.\
Workfront-Benutzende, die Workfront-Elemente erstellen und aktualisieren, benötigen keine [!DNL Jira], um die Erstellung von Elementen in [!DNL Jira] mit Triggern zu versehen.

Weitere Informationen zum automatischen Erstellen von Jira-Problemen mithilfe von Triggern finden Sie unter [Konfigurieren [!DNL Adobe Workfront]  für Jira](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

>[!NOTE]
>
>Sie können [!DNL Jira] Elemente automatisch erstellen, indem Sie eine Vorlage an ein Projekt anhängen. Wenn die Vorlage Aufgaben mit Arbeitsaufträgen enthält, die den [!DNL Jira] Trigger entsprechen, führen die neuen Aufgaben zu neuen [!DNL Jira].

Die automatische Verknüpfung eines [!DNL Workfront] Problems mit einem [!DNL Jira] Problem entspricht der automatischen Verknüpfung einer [!DNL Workfront] Aufgabe mit einem [!DNL Jira] Problem.

So verknüpfen Sie eine [!DNL Workfront] Aufgabe automatisch mit einem [!DNL Jira] Problem:

1. Vergewissern Sie sich, dass Ihr [!DNL Jira]-Systemadministrator Trigger konfiguriert hat, mit denen automatisch [!DNL Jira] Probleme erstellt werden, wenn [!DNL Workfront] Elemente zugewiesen werden. Melden Sie sich dann bei [!DNL Workfront] mit einer Zugriffsebene an, mit der Sie eine Aufgabe erstellen können.

   Weitere Informationen zum Zugriff auf Aufgaben finden Sie unter [Zugriff auf Aufgaben gewähren](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md).

1. Gehen Sie zu einem Projekt und wählen Sie **[!UICONTROL Aufgaben]** ![Symbol ](assets/tasks-icon-in-left-panel-14x14.png) im linken Bereich aus.

1. Klicken Sie auf **[!UICONTROL Neue Aufgabe]**

   Oder

   Wählen Sie eine vorhandene Aufgabe aus und klicken Sie dann auf **Bearbeiten**.

1. Geben Sie die für die Aufgabe verfügbaren Felder an oder aktualisieren Sie sie.
1. Klicken Sie **[!UICONTROL Arbeitsaufträge]** und weisen Sie die Aufgabe einem Benutzer, einer Rolle oder einem Team zu, der bzw. das in der [!DNL Jira] als Trigger angegeben ist.

1. Klicken Sie auf **Änderungen speichern**.

   In Workfront wird eine neue Aufgabe erstellt.

   Im Bereich **[!UICONTROL Updates]** der neuen Aufgabe gibt es einen Kommentar, der angibt, dass auch in [!DNL Jira] ein neues Problem erstellt wurde.

1. (Optional) Klicken Sie auf den Link zum Jira-Problem, um es in Jira zu öffnen.

   Oder

   Klicken Sie auf den **[!UICONTROL Zu Jira wechseln]** im Bereich **[!UICONTROL Integrationen]** des Abschnitts **[!UICONTROL Details]** oder in der Kopfzeile der Aufgabe oder des Problems, um das [!DNL Jira] Problem zu öffnen.

   Ihr System- oder Gruppenadministrator muss das Feld [!UICONTROL Integrationen] zu Ihrer Layout-Vorlage hinzufügen, um es in der Aufgaben- oder Problem-Kopfzeile anzuzeigen. Weitere Informationen finden Sie unter [Anpassen von Objektkopfzeilen mithilfe einer Layout-Vorlage](../../administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md).

   Jeder [!DNL Jira] Benutzer kann sofort mit der Arbeit an Elementen beginnen, die automatisch aus [!DNL Workfront] erstellt wurden, und ihre Aktualisierungen werden auf [!DNL Workfront] übertragen, ohne dass eine Lizenz für [!DNL Workfront] erforderlich ist.

   Es werden nur die Felder aktualisiert, die Sie als [!DNL Workfront] während der Einrichtung des [!DNL Workfront]-Add-ons konfiguriert haben.

   Weitere Informationen zum Synchronisieren von Feldern zwischen Workfront und Jira finden Sie im Abschnitt [Konfigurieren von Workfront für Jira](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md#configuring-the-add-on-for-jira) in [Konfigurieren von Adobe Workfront für Jira](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

   >[!NOTE]
   >
   >Das [!DNL Jira] Problem wird niemandem in [!DNL Jira] zugewiesen, wenn es automatisch in Workfront erstellt wird.

## [!DNL Jira] Probleme manuell mit [!DNL Workfront] Elementen verknüpfen

Nachdem Elemente in [!DNL Jira] und [!DNL Workfront] unabhängig voneinander erstellt wurden, können Sie ein [!DNL Jira] Problem manuell mit einer vorhandenen [!DNL Workfront] Aufgabe oder einem vorhandenen Problem verknüpfen.\
Sie können ein [!DNL Workfront] Element nicht manuell von [!DNL Workfront] mit einem vorhandenen [!DNL Jira] verknüpfen.

>[!NOTE]
>
>Wenn sich das [!DNL Jira] Problem nicht auf einem Projekt befindet, das nicht als Trigger in der [!DNL Workfront]-Integration identifiziert wird, können Sie es bei Verwendung der Integration mit [!DNL Jira] On-Premise nicht manuell mit einem Workfront-Element verknüpfen.\
>Weitere Informationen zum Einrichten von Triggern für den Workflow &quot;Workfront zu Jira“ finden Sie unter [Workfront-Elemente automatisch mit Jira-Problemen verknüpfen](#automatically-link-workfront-items-to-jira-issues).

Wenn [!DNL Workfront] und [!DNL Jira] Elemente verknüpft sind, können bestimmte Felder eines Elements beim anderen automatisch aktualisiert werden.\
Weitere Informationen zum Aktualisieren verknüpfter Elemente finden Sie unter [Aktualisieren verknüpfter Elemente zwischen Jira und Adobe Workfront](../../workfront-integrations-and-apps/use-workfront-with-jira/update-linked-items-between-jira-wf.md).

So verknüpfen Sie [!DNL Jira] Probleme manuell mit [!DNL Workfront]:

1. (Bedingt) Melden Sie sich bei [!DNL Workfront] an und finden Sie ein Problem oder eine Aufgabe, die Sie mit [!DNL Jira] Problem verknüpfen möchten.
1. (Bedingt) Kopieren Sie im [!UICONTROL Details] die **[!UICONTROL Referenznummer]** des Elements in Workfront.

   Oder

   Kopieren Sie in der Adressleiste des Elements die **URL** des Elements in Workfront.

   >[!IMPORTANT]
   >
   >Wenn Ihr Unternehmen in das einheitliche Adobe-Erlebnis integriert wurde, müssen Sie die **Referenznummer** zum Verknüpfen von Workfront-Elementen mit Jira verwenden. (Die URL-Option ist verfügbar, gibt aber einen Fehler zurück, wenn Sie sie verwenden.) Informationen zum einheitlichen Erlebnis finden Sie unter [Einheitliches Adobe-Erlebnis für Workfront](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md).
   >
   >Für Unternehmen, die nicht am einheitlichen Adobe-Erlebnis teilnehmen, wird die Verwendung der URL-Option nicht empfohlen, da sich die URLs ändern können.

   >[!NOTE]
   >
   >Sie müssen über eine [!DNL Workfront]-Lizenz verfügen, um sich bei [!DNL Workfront] anzumelden. Andernfalls muss Ihnen ein [!DNL Workfront] Benutzer diese Informationen bereitstellen.

1. Navigieren Sie in [!DNL Jira] zu einem Problem, das Sie manuell mit dem [!DNL Workfront] verknüpfen möchten.
1. Fügen Sie im rechten Bedienfeld [!DNL Workfront] die **[!UICONTROL Referenznummer]** oder die **URL** des [!DNL Workfront] ein, mit dem Sie eine Verknüpfung herstellen möchten.

1. Klicken Sie auf **[!UICONTROL Link]**.

   Die beiden Elemente werden verknüpft und der [!DNL Workfront] rechte Bereich wird mit Informationen aus dem [!DNL Workfront] Element gefüllt.

   Die folgenden [!DNL Workfront] sind standardmäßig in [!DNL Jira] im [!DNL Workfront] rechten Bereich sichtbar:

   * Der **[!UICONTROL Name]** des Elements: Sie können auf das [!DNL Workfront] Element zugreifen, indem Sie auf den Namen im Bedienfeld klicken.
   * **[!UICONTROL Projektname]**
   * Der **[!UICONTROL Status]** des Elements
   * Die **[!UICONTROL Priorität]** des Elements
   * Das Datum, an dem es in [!DNL Workfront] erstellt wurde
   * Die **[!UICONTROL Geplanten Stunden]** des Elements
   * Die **[!UICONTROL Referenznummer]**: Sie können auf das [!DNL Workfront] Element zugreifen, indem Sie auf die [!UICONTROL Referenznummer] im Bedienfeld klicken.

Weitere Informationen dazu, wie Sie zusätzliche Felder für die Anzeige im rechten Bereich aktivieren, finden Sie [ Abschnitt „Konfigurieren der Feldsynchronisierung zwischen  [!DNL Jira]  und  [!DNL Workfront]  Elementen](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md#setting-up-field-synchronization) in [Konfigurieren [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md). Auf der Registerkarte **[!DNL Workfront]** des [!DNL Jira] Problems wird ein Kommentar des [!DNL Workfront]-Administrators, der mit der Integration verknüpft ist, veröffentlicht, um zu bestätigen, dass ein neues [!DNL Jira] erstellt wurde. Der Kommentar enthält einen Link zum [!DNL Jira].

## Verknüpfung von Elementen zwischen [!DNL Jira] und [!DNL Workfront] aufheben

Verknüpfte Elemente zwischen [!DNL Jira] und [!DNL Workfront] können manuell aus [!DNL Jira] entfernt werden.\
Sie können die Verknüpfung eines [!DNL Workfront] Elements mit seinem [!DNL Jira] Gegenstück in [!DNL Workfront] nicht aufheben.

Sie benötigen den folgenden Zugriff, um die Verknüpfung mit manuell verknüpften Elementen aufzuheben:

* Sie sind der Benutzer, der die Elemente manuell verknüpft hat
* Sie sind der [!DNL Jira] Systemadministrator

Nur ein [!DNL Workfront] Administrator kann die Verknüpfung von automatisch verknüpften Elementen aufheben.

So heben Sie die Verknüpfung eines [!DNL Jira] Problems mit einem [!DNL Workfront] auf:

1. Navigieren Sie [!DNL Jira] zu einem Problem, das mit einer [!DNL Workfront] Aufgabe oder einem Problem verknüpft ist.
1. Klicken Sie im rechten [!DNL Workfront] auf das Symbol **[!UICONTROL Verknüpfung aufheben]** und dann auf **[!UICONTROL Verknüpfung aufheben]**.

   Die zuvor verknüpften [!DNL Jira]- und [!DNL Workfront]-Elemente sind jetzt unverknüpft. Felder, Kommentare oder Dokumente, die in Zukunft einzeln aktualisiert werden könnten, werden in der anderen Anwendung nicht im Vergleich zu ihrem vorherigen Gegenstück aktualisiert.
