---
product-area: workfront-integrations
navigation-topic: workfront-for-jira
title: Verknüpfte Elemente zwischen [!DNL Jira] und [!DNL Adobe Workfront]
description: Link [!DNL Jira] Probleme [!DNL Adobe Workfront] Aufgaben oder Probleme verwenden, können Ihre Benutzer Elemente in einer Anwendung aktualisieren und das Gegenstück zu diesem Element wird auch für die Benutzer aktualisiert, die in der zweiten Anwendung arbeiten.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 79ac6ff1-2f7d-4abc-8735-398f6aac5191
source-git-commit: f22a67cd3235a3111f7b874637ec05f8299de271
workflow-type: tm+mt
source-wordcount: '1703'
ht-degree: 0%

---

# Verknüpfte Elemente zwischen [!DNL Jira] und [!DNL Adobe Workfront]

Link [!DNL Jira] Probleme [!DNL Adobe Workfront] Aufgaben oder Probleme verwenden, können Ihre Benutzer Elemente in einer Anwendung aktualisieren und das Gegenstück zu diesem Element wird auch für die Benutzer aktualisiert, die in der zweiten Anwendung arbeiten.

Weitere Informationen zum Verknüpfen von Elementen zwischen [!DNL Workfront] und [!DNL Jira], siehe [Verknüpfen von Elementen zwischen Adobe Workfront und Jira](../../workfront-integrations-and-apps/use-workfront-with-jira/link-items-between-wf-jira.md).

Während der Einrichtung [!DNL Workfront] für [!DNL Jira]als [!DNL Jira] Systemadministrator können Sie bestimmte Felder aus einer Anwendung konfigurieren, um sie mit Feldern aus verknüpften Elementen in der anderen Anwendung zu synchronisieren.

Weitere Informationen zum Synchronisieren von Feldern zwischen verknüpften [!DNL Jira] und [!DNL Workfront] Elemente, siehe [Konfigurieren [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

## Zugriffsanforderungen

Sie müssen über Folgendes verfügen:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">[!DNL Adobe Workfront] Plan</a>*</td> 
   <td> <p>[!UICONTROL Pro] oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe [!DNL Workfront] Lizenzübersicht</a>*</td> 
   <td> <p>[!UICONTROL Plan]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Jira] Zugriff</td> 
   <td> <p>Systemadministratorzugriff</p> <p>Wichtig: Es wird empfohlen, separate Systemadministratorkonten in der [!DNL Jira] und [!DNL Workfront] , um dieser Integration zu widmen, anstatt vorhandene zu verwenden, die möglicherweise mit Benutzern verbunden sind.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Sie müssen [!DNL Workfront] Administrator. Informationen über [!DNL Workfront] Administratoren, siehe <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Gewähren eines vollen Administratorzugriffs</a>.</p> <p>Hinweis: Wenn Sie noch keinen Zugriff haben, fragen Sie Ihren [!DNL Workfront] Administrator , wenn sie zusätzliche Einschränkungen für Ihre Zugriffsebene festlegen. Für Informationen zur [!DNL Workfront] Administrator kann Ihre Zugriffsebene ändern, siehe <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren [!DNL Workfront] Administrator.

## Voraussetzungen

Bevor Sie Elemente verknüpfen können zwischen [!DNL Workfront] und [!DNL Jira], müssen Sie

* Installieren [!DNL Workfront for Jira].

   Anweisungen zur Installation [!DNL Workfront for Jira], siehe [Installieren [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/install-workfront-for-jira.md).

* Konfigurieren [!DNL Workfront for Jira].

   Anweisungen zum Konfigurieren von [!DNL Workfront for Jira], siehe [Konfigurieren [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

* Elemente verknüpfen zwischen [!DNL Workfront] und [!DNL Jira].

   Anweisungen finden Sie unter [Elemente verknüpfen zwischen [!DNL Adobe Workfront] und [!DNL Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/link-items-between-wf-jira.md).

## Verknüpfte Elemente in aktualisieren [!DNL Workfront]

Wenn Sie hauptsächlich in [!DNL Workfront], können Sie Ihre Arbeitselemente in [!DNL Workfront] und ihre Kollegen in [!DNL Jira] auch aktualisieren. Diese Aktualisierung erfolgt durch die Integration von [!DNL Workfront] für [!DNL Jira] für die Sie keine [!DNL Jira] Lizenz.

Solange Ihre [!DNL Workfront] Administrator hat [!DNL Workfront for Jira] um die Felder zwischen verknüpften Elementen zu synchronisieren, bestimmte Felder, die Sie aktualisieren in [!DNL Workfront] auch für die verknüpfte [!DNL Jira] Problem. Weitere Informationen zum Aktualisieren von Elementen finden Sie unter [!DNL Workfront], siehe [Probleme bearbeiten](../../manage-work/issues/manage-issues/edit-issues.md) und [Aufgaben bearbeiten](../../manage-work/tasks/manage-tasks/edit-tasks.md).

Die folgende Liste zeigt, welche [!DNL Workfront] synchronisierte Felder mit [!DNL Jira] Felder für verknüpfte Elemente:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Aktualisiert [!DNL Workfront] field</strong> </th> 
   <th><strong>Synchronisiert [!DNL Jira] field/update</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Problem oder Aufgabenname]</td> 
   <td> <p>[!UICONTROL Problemname]</p> <p>Der <strong>[!DNL Workfront]</strong> des [!DNL Jira] Problem. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Problem oder Aufgabenbeschreibung]</td> 
   <td> <p> [!UICONTROL Problembeschreibung]</p> <p>Der <strong>[!DNL Workfront]</strong> des [!DNL Jira] Problem.<br></p> </td> 
  </tr> 
  <tr> 
   <td> <p> [!UICONTROL Hochgeladene Dokumente]</p> <p>Hinweis: Dokumente, die mit [!DNL Workfront] Elemente von einem externen Server werden nicht an [!DNL Jira] Probleme. Nur Dokumente, die direkt in hochgeladen wurden [!DNL Workfront] -Elemente werden auch auf die verknüpften [!DNL Jira] Probleme. </p> </td> 
   <td> <p>[!UICONTROL Attachments]</p> <p>Der <strong>[!DNL Workfront]</strong> des [!DNL Jira] Problem.<br></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Geplantes Abschlussdatum]</td> 
   <td> <p>[!UICONTROL Fälligkeitsdatum]</p> <p>Ein Kommentar zum geänderten [!UICONTROL Fälligkeitsdatum wird zum [!DNL Workfront] des [!DNL Jira] Problem. </p> <p>Hinweis: Sie müssen <strong>[!UICONTROL Fälligkeitsdatum]</strong> für Ihre [!DNL Jira] Probleme, damit dieses Feld in [!UICONTROL Jira] aktualisiert werden kann. </p> </td> 
  </tr> 
  <tr> 
   <td>Benutzerdefinierte Forms- und benutzerdefinierte Felder</td> 
   <td> <p> Anzeige im [!DNL Workfront] rechter Bereich des [!DNL Jira] Problem. <br>Nur die benutzerdefinierten Felder mit einem tatsächlichen Wert werden im Bereich angezeigt.<br></p> <p>Hinweis: Die Abschnitte Benutzerdefiniertes Formular werden mit der Zugriffsebene der [!DNL Workfront] Administrator. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Problem oder Aufgabenpriorität]</td> 
   <td>Anzeigen im [!DNL Workfront] rechter Bereich des [!DNL Jira] Problem. <br>Das Problem wird nicht aktualisiert <strong>[!UICONTROL Priority]</strong> -Feld in [!DNL Jira]. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Protokollzeit] </td> 
   <td> <p>Im Abschnitt <strong>[!DNL Workfront]</strong> des [!DNL Jira] Problem. Dazu gehören der Name des Benutzers, der die Zeit protokolliert, sowie der Benutzer, für den die Zeit protokolliert wird, falls er anders ist. Es wird keine Zeit in der <strong>[!UICONTROL Arbeitsprotokoll]</strong> Registerkarte in [!DNL Jira].<br></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Kommentare]</td> 
   <td> <p>Der Kommentar wird zum <strong>[!DNL Workfront]</strong> des [!DNL Jira] Problem. Sie wird nicht zum <strong>[!UICONTROL Kommentare]</strong> des [!DNL Jira] Problem</p> <p>Hinweis: Wenn Sie zwei vorhandene Elemente manuell verknüpfen, werden die Kommentare, die zum [!DNL Workfront] Element vor Verknüpfung mit [!DNL Jira] nicht mit der [!DNL Jira] Problem. </p> </td> 
  </tr> 
 </tbody> 
</table>

## Verknüpfte Elemente in aktualisieren [!DNL Jira]

Wenn Sie hauptsächlich in [!DNL Jira], können Sie Ihre Arbeitselemente in [!DNL Jira] und ihre Kollegen in [!DNL Workfront] auch aktualisieren. Sie müssen keine [!DNL Workfront] Lizenz für [!DNL Workfront] Elemente, die mit Ihrer [!DNL Jira] Probleme beim Empfang von Aktualisierungen, die Sie in [!DNL Jira].

Unter der Bedingung, dass [!DNL Workfront] Administrator hat [!DNL Workfront] für [!DNL Jira] um die Felder zwischen verknüpften Elementen zu synchronisieren, bestimmte Felder, die Sie aktualisieren in [!DNL Jira] auch für die verknüpfte [!DNL Workfront] Element.

Die folgende Liste zeigt, welche [!DNL Jira] synchronisierte Felder mit [!DNL Workfront] Felder für verknüpfte Elemente:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Aktualisiert [!DNL Jira] Feld</strong> </th> 
   <th><strong>Synchronisiert [!DNL Workfront] Feld/Aktualisierung</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Problemstatus]</td> 
   <td> <p> [!UICONTROL Problem oder Aufgabenstatus]</p> <p>Problemstatus in [!DNL Jira] synchronisiert in Workfront mit den folgenden Status oder Status, die mit den folgenden Status übereinstimmen:</p> 
    <ul> 
     <li> <p>[!UICONTROL Neu] ([!UICONTROL NEW])</p> </li> 
     <li> <p>[!UICONTROL In Bearbeitung] ([!UICONTROL INP])</p> </li> 
     <li> <p>[!UICONTROL Closed]/[!UICONTROL Complete] ([!UICONTROL CLS]/[!UICONTROL CPL])</p> </li> 
    </ul> <p>Hinweis: Die [!DNL Jira] status synchronisiert mit der ersten [!DNL Workfront] -Status, der mit dem entsprechenden Status übereinstimmt.</p> <p>Weitere Informationen zum Status von Elementen finden Sie unter [!DNL Workfront], siehe <a href="../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md" class="MCXref xref">Erstellen oder Bearbeiten eines Status</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Problemverantwortlicher]</td> 
   <td> <p> [!UICONTROL Problem oder Aufgabenverantwortlicher]</p> <p>Wichtig: Wenn Sie ein Element in [!DNL Jira] für einen Benutzer, der keine [!DNL Workfront] -Konto, erstellt die Integration einen neuen aktiven Benutzer in [!DNL Workfront] nur bei der Option "[!UICONTROL Benutzer automatisch erstellen in [!DNL Workfront] wenn die [!DNL Jira] Der Benutzer verfügt nicht über eine [!DNL Workfront] account]"auf [!UICONTROL Immer] gesetzt ist. Dieser Benutzer belegt keine [!DNL Workfront] Lizenz. Aktive Benutzer können Arbeitselementen in [!DNL Workfront], können jedoch nicht in Aktualisierungen einbezogen werden. Weitere Informationen zum Konfigurieren der automatischen Erstellung von [!DNL Workfront] Benutzer von [!DNL Jira], siehe <a href="../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md">Konfiguration [!DNL Workfront for Jira]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Problemanlagen]</td> 
   <td> [!UICONTROL Problem oder Aufgabendokumente]<br>Ein Kommentar zum Hochladen eines neuen Dokuments in [!DNL Jira] wird der Registerkarte [!UICONTROL Updates] im Abschnitt [!DNL Workfront] Problem oder Aufgabe.  </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Fälligkeitsdatum]</td> 
   <td> <p> Ein Kommentar zur Änderung des [!UICONTROL Fälligkeitsdatums] in [!DNL Jira] wird der Registerkarte [!UICONTROL Updates] im Abschnitt [!DNL Workfront] Problem oder Aufgabe. </p> <p>Hinweis: Keine Datumsänderungen am [!DNL Workfront] Problem oder Aufgabe. </p> </td> 
  </tr> 
  <tr> 
   <td> Protokollzeit in [!DNL Workfront] rechts oder über das Menü [!UICONTROL Mehr] im [!DNL Jira] Problem<br></td> 
   <td> <p>Stunden<br>Zusätzlich dazu werden die in Jira angemeldeten Stunden zum verknüpften [!DNL Workfront] -Element ein Kommentar zur Protokollierungszeit auf der Registerkarte [!UICONTROL Updates] im [!DNL Workfront] Element.</p> <p>Weitere Informationen zur Protokollierungszeit in verknüpften [!DNL Jira] Probleme, einschließlich der Aktualisierung der [!DNL Jira] Benutzer, der die Zeit in [!DNL Workfront], siehe <a href="#log-time-for-linked-jira-and-workfront-items" class="MCXref xref">Protokollzeit für verknüpfte Elemente [!DNL Jira] und [!DNL Workfront] items</a>.</p> </td> 
  </tr> 
  <tr> 
   <td> Kommentare <br><br></td> 
   <td> <p>Kommentare werden zur Registerkarte [!UICONTROL Updates] im [!DNL Workfront] Problem oder Aufgabe, wenn die <strong>[!UICONTROL Kommentare]</strong> im Bereich [!UICONTROL SYNCHRONISIEREN VON JIRA ZU WORKFRONT] der Registerkarte [!UICONTROL Setup] auf <strong>[!UICONTROL Immer]</strong>.</p> <p>Informationen zum Konfigurieren von Workfront-Einstellungen finden Sie unter [!DNL Jira], siehe <a href="../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md">Konfiguration [!DNL Workfront for Jira]</a>.</p> <p>Informationen zur Kommentierung von Elementen aus verknüpften [!DNL Jira] Probleme, siehe <a href="#comment-from-a-linked-jira-issue" class="MCXref xref">Kommentar aus einem Link [!DNL Jira] Problem</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Protokollzeit aus verknüpften [!DNL Jira] issues

Die Zeit, die Sie für einen [!DNL Jira] -Element [!DNL Jira] wird auch auf die verknüpfte [!DNL Workfront] Element, unabhängig davon, wo in [!DNL Jira] Sie protokollieren die Zeit.\
Wenn Sie die Zeit in Jira in der [!DNL Workfront] -Bedienfeld, wird die Zeit nur in aufgezeichnet. [!DNL Workfront].\
Die aufgezeichnete Zeit in [!DNL Workfront] hat keinen Einfluss auf den Zeitpunkt des verknüpften Problems in [!DNL Jira].

>[!NOTE]
>
>Wenn die Zeit zu einem [!DNL Jira] Element, das mit einem [!DNL Workfront] Aufgabe, die [!UICONTROL Stündentyp] für die Zeit in [!DNL Workfront] is [!UICONTROL Task Time]. Wenn die Zeit zu einem [!DNL Jira] Element, das mit einem [!DNL Workfront] -Problem, [!UICONTROL Stündentyp] für die Zeit in [!DNL Workfront] is [!UICONTROL Problemzeit].

Der **[!DNL Workfront]** Registerkarte in [!DNL Jira] und **[!UICONTROL Updates]** Registerkarte des Elements in [!DNL Workfront] , um die Protokollierung der Zeit aufzuzeichnen.\
Die Zeit wird auch im **[!UICONTROL Stunden]** des [!DNL Workfront] Element.

* [Protokollzeit für verknüpfte Elemente [!DNL Jira] und [!DNL Workfront] items](#log-time-for-linked-jira-and-workfront-items)
* [Protokollzeit von [!DNL Jira] zu [!DNL Workfront] item](#log-time-from-jira-to-a-workfront-item)

### Protokollzeit für verknüpfte Elemente [!DNL Jira] und [!DNL Workfront] items

Sie können die Zeit von [!DNL Jira] Problem in Zusammenhang mit einem [!DNL Workfront] -Element, und die Zeit wird sowohl auf der [!DNL Jira] sowie [!DNL Workfront] Element.

>[!IMPORTANT]
>
>Wenn der Benutzer sich anmeldet [!DNL Jira] ist nicht in vorhanden [!DNL Workfront], erstellt die Integration einen neuen aktiven Benutzer in Workfront, wenn die **[!UICONTROL Benutzer automatisch erstellen in [!DNL Workfront]&#x200B;, wenn die [!DNL Jira] Der Benutzer verfügt nicht über eine *[!DNL Workfront]&#x200B;]** festgelegt ist auf**[!UICONTROL  Immer ]**. Dieser Benutzer belegt keine [!DNL Workfront] Lizenz. Sie können aktive Benutzer Arbeitselementen in [!DNL Workfront], Sie können sie jedoch nicht in Aktualisierungen einbeziehen. Informationen zum Konfigurieren der automatischen Erstellung von [!DNL Workfront] Benutzer von [!DNL Jira], siehe [Konfiguration [!DNL Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

So protokollieren Sie die Zeit für ein Element in [!DNL Jira] und lassen Sie sie sowohl in [!DNL Jira] und [!DNL Workfront]:

1. Anmelden [!DNL Jira].
1. Navigieren Sie zu [!DNL Jira] -Problem, das mit dem [!DNL Workfront] Element.
1. Erweitern Sie die **[!UICONTROL Mehr]** Menü und klicken Sie auf **[!UICONTROL Protokollarbeit]**.

1. Im **[!UICONTROL Besuchszeit]** geben Sie die Zeit an, die mit der Bearbeitung dieses Problems verbracht wurde. Sie müssen die Zeit mithilfe der folgenden Zeiträume angeben:

   * [!UICONTROL Wochen] w)
   * [!UICONTROL Tage] d)
   * [!UICONTROL Stunden] h)

1. Fügen Sie Ihrem Zeiteintrag weiterhin Informationen hinzu, einschließlich einer **[!UICONTROL Arbeitsbeschreibung]** Klicken Sie auf **[!UICONTROL Protokoll]**.\
   Die Zeit wird zum **[!UICONTROL Arbeitsprotokoll]** des [!DNL Jira] sowie auf die [!DNL Workfront] -Element.\
   Die Arbeitsbeschreibung des Zeiteintrags wird als Hinweis beim Stundeneintrag in [!DNL Workfront].

### Protokollzeit von [!DNL Jira] zu [!DNL Workfront] item

Sie können die Zeit nur auf die verknüpfte [!DNL Workfront] -Element [!DNL Jira] -Problem, ohne dieses Mal auf [!DNL Jira] Problem.

1. Anmelden [!DNL Jira].
1. Navigieren zu einer [!DNL Jira] -Problem, das mit einer [!DNL Workfront] Element.

   Die Einzelheiten der [!DNL Workfront] -Element im [!DNL Workfront] rechter Bereich des Problems.

1. Klicken Sie auf **[!UICONTROL Protokollzeit]** Symbol.

1. Geben Sie den Betrag von **[!UICONTROL Stunden]** und **[!UICONTROL Minuten]** Sie möchten sich für das Problem anmelden.

1. Klicken **[!UICONTROL Protokollzeit]**.

   Die Zeit wird zum [!DNL Workfront] Element.

   Diese Zeit wird nicht zum [!UICONTROL Arbeitsprotokoll] des [!DNL Jira] Problem.

## Kommentar aus einem Link [!DNL Jira] Problem {#comment-from-a-linked-jira-issue}

Wenn Sie einen Kommentar zu einer [!DNL Jira] -Element [!DNL Workfront] rechter Bereich in [!DNL Jira], wird der Kommentar auch zum [!UICONTROL Updates] des verknüpften Elements in Workfront.

So kommentieren Sie [!DNL Jira] zu [!DNL Workfront] item:

1. Anmelden [!DNL Jira].
1. Navigieren zu einer [!DNL Jira] -Problem, das mit einer [!DNL Workfront] Element.

   Die Einzelheiten der [!DNL Workfront] -Element im [!DNL Workfront] rechter Bereich des Problems.

1. Klicken Sie auf **[!UICONTROL Kommentare]** im [!DNL Workfront] oder auf **[!UICONTROL Kommentare]** Registerkarte.

1. Beginnen Sie mit der Eingabe eines Kommentars und klicken Sie dann auf **[!UICONTROL Senden]**.

   Der Kommentar wird wie folgt hinzugefügt:

   * Die **[!DNL Workfront]** des [!DNL Jira] Problem.
   * Die **[!UICONTROL Kommentare]** des [!DNL Jira] Problem.
   * Die **[!UICONTROL Updates]** des verknüpften Elements in Workfront.
