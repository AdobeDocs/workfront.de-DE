---
product-area: workfront-integrations
navigation-topic: workfront-for-jira
title: Elemente verknüpfen zwischen [!DNL Adobe Workfront] und [!DNL Jira]
description: Sie können Probleme  [!DNL Jira]  Aufgaben oder  [!DNL Adobe Workfront]  entweder automatisch oder manuell verknüpfen.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 1c37f361-e866-4ac6-b672-408848a80ed6
source-git-commit: 064418302767ad20e176080ba9a12db548750f3c
workflow-type: tm+mt
source-wordcount: '1324'
ht-degree: 0%

---

# Elemente zwischen [!DNL Adobe Workfront] und [!DNL Jira] verknüpfen

<!-- Audited: 5/2025 -->

>[!IMPORTANT]
>
>Um stabilere und skalierbarere Integrationen bereitzustellen, wechseln wir mithilfe von Workfront Automation and Integration (Fusion) zu einem modernen, flexiblen Integrationsansatz. Im Rahmen dieses Übergangsprozesses wird die Integration von Workfront für Jira nach dem 28. **2026 nicht mehr**.
>
>Es wird empfohlen, Workfront-Automatisierung und -Integration für die Integrationsanforderungen Ihres Unternehmens mit Jira zu verwenden.
>
>Einen Überblick über die Automatisierung und Integration von Workfront finden Sie unter [Übersicht über Adobe Workfront Fusion](https://experienceleague.adobe.com/de/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview).
>
>Informationen zu den spezifischen Funktionen der Workfront-Automatisierungs- und Integrationsmodule für Jira finden Sie unter [Jira-Softwaremodule](https://experienceleague.adobe.com/de/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/jira-software-modules).

<!--

>[!IMPORTANT]
>
>To deliver more stable and scalable integrations, we're shifting to a modern, flexible integration approach using Workfront Automation and Integration (Fusion). As part of this transition process, the Workfront for Jira integration will not be available after **February 28, 2026**. 
>
>We recommend using Workfront Automation and Integration for your organization's integration needs with Jira. 
>
>Eight ready-to-use Workfront Automation and Integration templates for Jira will be available by August to help replicate common workflows and accelerate implementation. Templates are fully customizable to meet specific business needs and can be extended as requirements evolve. 
> 
>For an overview of Workfront Automation and Integration, see [Adobe Workfront Fusion overview](https://experienceleague.adobe.com/de/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview). 
>
>For information about the specific capabilities of the Workfront Automation and Integration modules for Jira, see [Jira Software modules](https://experienceleague.adobe.com/de/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/jira-software-modules). 

-->

Sie können [!DNL Jira] Probleme entweder automatisch oder manuell mit [!DNL Adobe Workfront] Aufgaben oder Problemen verknüpfen.

Nur ein Element in [!DNL Workfront] kann mit einem Element in [!DNL Jira] verknüpft werden. Sie können niemals ein [!DNL Workfront] mit mehreren [!DNL Jira] oder ein [!DNL Jira] mit mehreren [!DNL Workfront] verknüpfen.

## Zugriffsanforderungen

Sie müssen über Folgendes verfügen:

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://business.adobe.com/products/workfront/pricing.html" target="_blank">[!DNL [!DNL Adobe Workfront] Plan]</a></td> 
   <td> <p>[!UICONTROL Pro] oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Übersicht über Adobe-[!DNL Workfront]</a></td> 
   <td> 
   <p>Neu: Standard<p>
   <p>Oder</p>
   <p>Aktuell: Plan </p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Jira-Zugriff</td> 
   <td> <p>Systemadministratorzugriff</p> <p><b>WICHTIG</b>

Es wird empfohlen, separate Systemadministratorkonten in [!DNL Jira] und [!DNL Workfront] zu erstellen, um diese Integration zu ermöglichen, anstatt vorhandene Konten zu verwenden, die an Benutzer angehängt sein könnten.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Sie müssen [!DNL Workfront] sein. Informationen zu [!DNL Workfront] finden Sie unter <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Gewähren des vollständigen Administratorzugriffs für einen Benutzer</a>.</p> <p><b>NOTIZ</b>

Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren [!DNL Workfront], ob er zusätzliche Einschränkungen in Ihrer Zugriffsebene festlegt. Informationen dazu, wie [!DNL Workfront]-Admins Ihre Zugriffsebene ändern können, finden Sie unter <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Erstellen oder Ändern benutzerdefinierter Zugriffsebenen</a>.</p> </td>
</tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Voraussetzungen

Bevor Sie Elemente zwischen [!DNL Workfront] und [!DNL Jira] verknüpfen können, müssen Sie Folgendes tun:

* Installieren Sie [!DNL Workfront] für [!DNL Jira].

  Anweisungen finden Sie unter [Installieren von Adobe Workfront für Jira](../../workfront-integrations-and-apps/use-workfront-with-jira/install-workfront-for-jira.md).

* Konfigurieren Sie [!DNL Workfront] für Jira.

  Anweisungen finden Sie unter [Konfigurieren von Adobe Workfront für Jira](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

## [!DNL Workfront] Elemente automatisch mit [!DNL Jira] Problemen verknüpfen

Als [!DNL Workfront] können Sie Trigger definieren, die automatisch ein Problem in [!DNL Jira] erstellen, wenn bestimmte Bedingungen für eine Aufgabe oder ein Problem in [!DNL Workfront] erfüllt sind. Die Workfront- und [!DNL Jira]-Elemente werden verknüpft.

Nachdem Sie die Konfiguration von [!DNL Workfront] für Jira abgeschlossen haben und ein Element entweder erstellt oder aktualisiert wird, [!DNL Workfront] es Ihren Triggern entspricht, wird automatisch ein neues Element in [!DNL Jira] erstellt.

Workfront-Benutzende, die Workfront-Elemente erstellen und aktualisieren, benötigen keine [!DNL Jira], um die Erstellung von Elementen in [!DNL Jira] mit Triggern zu versehen.

Weitere Informationen finden Sie unter [Konfigurieren [!DNL Adobe Workfront]  für Jira](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

>[!NOTE]
>
>Sie können [!DNL Jira] Elemente automatisch erstellen, indem Sie eine Vorlage an ein Projekt anhängen. Wenn die Vorlage Aufgaben mit Arbeitsaufträgen enthält, die den [!DNL Jira] Trigger entsprechen, führen die neuen Aufgaben zu neuen [!DNL Jira].

Die automatische Verknüpfung eines [!DNL Workfront] Problems mit einem [!DNL Jira] Problem entspricht der automatischen Verknüpfung einer [!DNL Workfront] Aufgabe mit einem [!DNL Jira] Problem.

So verknüpfen Sie eine [!DNL Workfront] Aufgabe automatisch mit einem [!DNL Jira] Problem:

1. Vergewissern Sie sich, dass Ihr [!DNL Jira]-Systemadministrator Trigger konfiguriert hat, mit denen automatisch [!DNL Jira] Probleme erstellt werden, wenn [!DNL Workfront] Elemente zugewiesen werden. Melden Sie sich dann bei [!DNL Workfront] mit einer Zugriffsebene an, mit der Sie eine Aufgabe erstellen können.

   Weitere Informationen zum Zugriff auf Aufgaben finden Sie unter [Zugriff auf Aufgaben gewähren](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md).

{{step1-to-projects}}

1. Wählen Sie auf **Seite** ein Projekt aus.

1. Wählen Sie im linken Projektbedienfeld die Option **[!UICONTROL Aufgaben]** aus.

1. Klicken Sie auf **+ Neue Aufgabe**.

   >[!NOTE]
   >
   >Um ein vorhandenes Workfront-Element mit einem Jira-Problem zu verknüpfen, wählen Sie **Bearbeiten** aus dem Menü **Mehr** Mehr![Symbol &#x200B;](assets/more-icon.png) des Elements aus.

1. Geben Sie die für die Aufgabe verfügbaren Felder an oder aktualisieren Sie sie.
1. Suchen Sie im **[!UICONTROL Arbeitsaufträge]** nach dem Benutzer, der Rolle oder dem Team, der bzw. das als Trigger(in) in der [!DNL Jira]-Integration angegeben ist, und wählen Sie diese aus.

1. Klicken Sie **Aufgabe erstellen**. Die Aufgabe wird in Workfront erstellt, und auf der Registerkarte **Updates“ der Aufgabe wird ein neuer** angezeigt, um anzugeben, dass auch in [!DNL Jira] ein neues Problem erstellt wurde.

1. (Optional) Klicken Sie im Bereich **[!UICONTROL Integrationen]** des Abschnitts **[!UICONTROL Details]** der Aufgaben- oder Problem-Kopfzeile auf den Link **[!UICONTROL Zu Jira wechseln]**, um das Problem in Jira zu öffnen.

   Ihr System- oder Gruppenadministrator muss das Feld [!UICONTROL Integrationen] zu Ihrer Layout-Vorlage hinzufügen, um es in der Aufgaben- oder Problem-Kopfzeile anzuzeigen. Weitere Informationen finden Sie unter [Anpassen von Objektkopfzeilen mithilfe einer Layout-Vorlage](../../administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md).

   Jeder [!DNL Jira] Benutzer kann sofort mit der Arbeit an Elementen beginnen, die automatisch aus [!DNL Workfront] erstellt wurden, und ihre Aktualisierungen werden auf [!DNL Workfront] übertragen, ohne dass eine Lizenz für [!DNL Workfront] erforderlich ist.

   Es werden nur die Felder aktualisiert, die Sie als [!DNL Workfront] während der Einrichtung des [!DNL Workfront]-Add-ons konfiguriert haben.

   Weitere Informationen zum Synchronisieren von Feldern zwischen Workfront und Jira finden Sie im Abschnitt Konfigurieren von Workfront für Jira unter [Konfigurieren von Adobe Workfront für Jira](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

   >[!NOTE]
   >
   >Das [!DNL Jira] Problem wird in [!DNL Jira] niemandem zugewiesen, wenn es automatisch in Workfront erstellt wird.

## [!DNL Jira] Probleme manuell mit [!DNL Workfront] Elementen verknüpfen

Nachdem Elemente in [!DNL Jira] und unabhängig voneinander erstellt [!DNL Workfront], können Sie ein [!DNL Jira] Problem manuell mit einer vorhandenen [!DNL Workfront] Aufgabe oder einem vorhandenen Problem verknüpfen.

Sie können ein [!DNL Workfront] Element nicht manuell von [!DNL Workfront] mit einem vorhandenen [!DNL Jira] verknüpfen.

>[!NOTE]
>
>Wenn sich das [!DNL Jira] Problem nicht auf einem Projekt befindet, das nicht als Trigger in der [!DNL Workfront]-Integration identifiziert wird, können Sie es bei Verwendung der Integration mit [!DNL Jira] On-Premise nicht manuell mit einem Workfront-Element verknüpfen.\
>Weitere Informationen zum Einrichten von Triggern für den Workflow &quot;Workfront zu Jira“ finden Sie unter [Workfront-Elemente automatisch mit Jira-Problemen verknüpfen](#automatically-link-workfront-items-to-jira-issues).

Wenn [!DNL Workfront] und [!DNL Jira] Elemente verknüpft sind, können bestimmte Felder eines Elements beim anderen automatisch aktualisiert werden.\
Weitere Informationen zum Aktualisieren verknüpfter Elemente finden Sie unter [Aktualisieren verknüpfter Elemente zwischen Jira und Adobe Workfront](../../workfront-integrations-and-apps/use-workfront-with-jira/update-linked-items-between-jira-wf.md).

So verknüpfen Sie [!DNL Jira] Probleme manuell mit [!DNL Workfront]:

1. (Bedingt) Melden Sie sich bei [!DNL Workfront] an und finden Sie ein Problem oder eine Aufgabe, die Sie mit einem [!DNL Jira] Problem verknüpfen möchten.
1. (Bedingt) Kopieren Sie im Abschnitt **Grundlegende Informationen** auf der Registerkarte **Aufgabendetails** oder **Problemdetails** die **[!UICONTROL Referenznummer]** des Elements in Workfront.

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
1. Fügen Sie im rechten Bedienfeld [!DNL Workfront] die **[!UICONTROL Referenznummer]** oder die **URL** des [!DNL Workfront] ein, mit dem Sie es verknüpfen möchten.

1. Klicken Sie auf **[!UICONTROL Link]**. Die beiden Elemente werden verknüpft und der [!DNL Workfront] rechte Bereich wird mit Informationen aus dem [!DNL Workfront] Element gefüllt.

   Standardmäßig sind die folgenden [!DNL Workfront] in [!DNL Jira] im rechten [!DNL Workfront] sichtbar:

   * Der **[!UICONTROL Name]** des Elements. Sie können auf das [!DNL Workfront] Element zugreifen, indem Sie auf den Namen im Bedienfeld klicken.
   * Der **[!UICONTROL Projektname]**.
   * Der **[!UICONTROL Status]** des Elements.
   * Die **[!UICONTROL Priorität]** des Elements.
   * Das Datum, an dem es in [!DNL Workfront] erstellt wurde.
   * Die **[!UICONTROL Geplanten Stunden]** des Elements.
   * Die **[!UICONTROL Referenznummer]**. Sie können auf das [!DNL Workfront] Element zugreifen, indem Sie auf **Referenznummer** im Bedienfeld klicken.

   Weitere Informationen zum Aktivieren zusätzlicher Felder, die im rechten Bereich angezeigt werden, finden Sie im Abschnitt Konfigurieren der Feldsynchronisierung zwischen [!DNL Jira] und [!DNL Workfront] Elementen in [Konfigurieren [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md). Auf der Registerkarte [!DNL Workfront] des **[!DNL Workfront]** Problems wird ein Kommentar des [!DNL Jira]-Administrators, der mit der Integration verknüpft ist, veröffentlicht, um zu bestätigen, dass ein neues [!DNL Jira] erstellt wurde. Der Kommentar enthält einen Link zum [!DNL Jira].

## Verknüpfung von Elementen zwischen [!DNL Jira] und [!DNL Workfront] aufheben

Verknüpfte Elemente zwischen [!DNL Jira] und [!DNL Workfront] können in [!DNL Jira] manuell aufgehoben werden. Sie können die Verknüpfung eines [!DNL Workfront] Elements mit seinem [!DNL Jira] Gegenstück in [!DNL Workfront] nicht aufheben.

Sie benötigen den folgenden Zugriff, um die Verknüpfung mit manuell verknüpften Elementen aufzuheben:

* Sie sind der Benutzer, der die Elemente manuell verknüpft hat.
* Sie sind der [!DNL Jira] Systemadministrator.

>[!NOTE]
>
>Nur ein [!DNL Workfront] Administrator kann die Verknüpfung von automatisch verknüpften Elementen aufheben.

So heben Sie die Verknüpfung eines [!DNL Jira] Problems mit einem [!DNL Workfront] auf:

1. Anmelden bei Jira.
1. Navigieren Sie zu dem Problem, das mit einer [!DNL Workfront] Aufgabe oder einem Problem verknüpft ist.
1. Wechseln Sie zum rechten Bedienfeld von **0&rbrace;Workfront.**
1. Klicken Sie auf das Symbol **[!UICONTROL Verknüpfung aufheben]** und dann auf **[!UICONTROL Verknüpfung aufheben]**. Die zuvor verknüpften [!DNL Jira] und [!DNL Workfront] Elemente werden aufgehoben.

   Felder, Kommentare oder Dokumente, die in Zukunft aktualisiert werden, werden nicht im vorherigen Gegenstück in der anderen Anwendung aktualisiert.
