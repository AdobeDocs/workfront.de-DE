---
product-area: workfront-integrations
navigation-topic: workfront-for-jira
title: Aktualisieren verknüpfter Elemente zwischen [!DNL Jira] und [!DNL Adobe Workfront]
description: Wenn Sie [!DNL Jira] Probleme mit [!DNL Adobe Workfront] Aufgaben oder Problemen verknüpfen, können Ihre Benutzer Elemente in einer Anwendung aktualisieren und das Gegenstück zu diesem Element wird auch für die Benutzer aktualisiert, die in der zweiten Anwendung arbeiten.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 79ac6ff1-2f7d-4abc-8735-398f6aac5191
source-git-commit: 99924f690c53584c090d19fff90d23d84ec306d4
workflow-type: tm+mt
source-wordcount: '1576'
ht-degree: 0%

---

# Aktualisieren der verknüpften Elemente zwischen [!DNL Jira] und [!DNL Adobe Workfront]

Wenn Sie [!DNL Jira]-Probleme mit [!DNL Adobe Workfront] -Aufgaben oder -Problemen verknüpfen, können Ihre Benutzer Elemente in einer Anwendung aktualisieren und das Gegenstück zu diesem Element wird auch für die Benutzer aktualisiert, die in der zweiten Anwendung arbeiten.

Weitere Informationen zum Verknüpfen von Elementen zwischen [!DNL Workfront] und [!DNL Jira] finden Sie unter [Verknüpfen von Elementen zwischen Adobe Workfront und Jira](../../workfront-integrations-and-apps/use-workfront-with-jira/link-items-between-wf-jira.md).

Wenn Sie [!DNL Workfront] für [!DNL Jira] einrichten, können Sie als Systemadministrator von [!DNL Jira] bestimmte Felder aus einer Anwendung so konfigurieren, dass sie mit Feldern aus verknüpften Elementen in der anderen Anwendung synchronisiert werden.

Weitere Informationen zum Synchronisieren von Feldern zwischen verknüpften [!DNL Jira]- und [!DNL Workfront]-Elementen finden Sie unter [Konfigurieren [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

## Zugriffsanforderungen

Sie müssen über Folgendes verfügen:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Plan</td> 
   <td><p>Neu: Beliebig</p>
       <p>oder</p>
       <p>Aktuell: [!UICONTROL Pro] oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Lizenz</td> 
   <td><p>Neu: [!UICONTROL Standard]</p>
       <p>oder</p>
       <p>Aktuell: [!UICONTROL Plan]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Jira] access</td> 
   <td> <p>Systemadministratorzugriff</p> <p>Wichtig: Es wird empfohlen, separate Systemadministratorkonten in [!DNL Jira] und [!DNL Workfront] zu erstellen, um diese Integration zu widmen, anstatt vorhandene zu Benutzern gehörende Konten zu verwenden.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Sie müssen ein [!DNL Workfront] -Administrator sein.</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Voraussetzungen

Bevor Sie Elemente zwischen [!DNL Workfront] und [!DNL Jira] verknüpfen können, müssen Sie:

* Installieren Sie [!DNL Workfront for Jira].

  Anweisungen zum Installieren von [!DNL Workfront for Jira] finden Sie unter [Installieren [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/install-workfront-for-jira.md).

* Konfigurieren Sie [!DNL Workfront for Jira].

  Anweisungen zum Konfigurieren von [!DNL Workfront for Jira] finden Sie unter [Konfigurieren [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

* Verknüpfen Sie Elemente zwischen [!DNL Workfront] und [!DNL Jira].

  Anweisungen finden Sie unter [Verknüpfen von Elementen zwischen [!DNL Adobe Workfront] und [!DNL Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/link-items-between-wf-jira.md).

## Verknüpfte Elemente in [!DNL Workfront] aktualisieren

Wenn Sie primär in [!DNL Workfront] arbeiten, können Sie Ihre Arbeitselemente in [!DNL Workfront] aktualisieren und ihre Gegenstücke in [!DNL Jira] ebenfalls aktualisieren. Dieses Update erfolgt durch die Integration von [!DNL Workfront] für [!DNL Jira], für die Sie keine [!DNL Jira] -Lizenz benötigen.

Solange Ihr [!DNL Workfront] -Administrator [!DNL Workfront for Jira] so konfiguriert hat, dass die Felder zwischen verknüpften Elementen synchronisiert werden, werden bestimmte Felder, die Sie in [!DNL Workfront] aktualisieren, auch für das verknüpfte [!DNL Jira]-Problem aktualisiert. Weitere Informationen zum Aktualisieren von Elementen in [!DNL Workfront] finden Sie unter [Probleme bearbeiten](../../manage-work/issues/manage-issues/edit-issues.md) und [Aufgaben bearbeiten](../../manage-work/tasks/manage-tasks/edit-tasks.md).

Die folgende Liste zeigt, welche [!DNL Workfront] -Felder mit [!DNL Jira] -Feldern für verknüpfte Elemente synchronisiert werden:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Aktualisiertes [!DNL Workfront] -Feld</strong> </th> 
   <th><strong>Synchronisiertes [!DNL Jira] Feld/ Update</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Problem oder Aufgabenname]</td> 
   <td> <p>[!UICONTROL Problemname]</p> <p>Der Registerkarte <strong>[!DNL Workfront]</strong> des [!DNL Jira]-Problems wird ein Kommentar zur Namensänderung hinzugefügt. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Problem oder Aufgabenbeschreibung]</td> 
   <td> <p> [!UICONTROL Problembeschreibung]</p> <p>Der Registerkarte <strong>[!DNL Workfront]</strong> des [!DNL Jira]-Problems wird ein Kommentar zur aktualisierten Beschreibung hinzugefügt.<br></p> </td> 
  </tr> 
  <tr> 
   <td> <p> [!UICONTROL Hochgeladene Dokumente]</p> <p>Hinweis: Dokumente, die mit [!DNL Workfront] -Elementen von einem externen Server verknüpft sind, werden nicht in [!DNL Jira] -Probleme übertragen. Nur Dokumente, die direkt in [!DNL Workfront] -Elemente hochgeladen wurden, werden ebenfalls auf die verknüpften [!DNL Jira] -Probleme aktualisiert. </p> </td> 
   <td> <p>[!UICONTROL Attachments]</p> <p>Auf der Registerkarte <strong>[!DNL Workfront]</strong> des [!DNL Jira]-Problems wird ein Kommentar zu den hochgeladenen Anlagen hinzugefügt.<br></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Geplantes Abschlussdatum]</td> 
   <td> <p>[!UICONTROL Fälligkeitsdatum]</p> <p>Auf der Registerkarte [!DNL Workfront] des [!DNL Jira]-Problems wird ein Kommentar zum geänderten [!UICONTROL Fälligkeitsdatum] hinzugefügt. </p> <p>Hinweis: Sie müssen <strong>[!UICONTROL Fälligkeitsdatum]</strong> aktivieren, damit Ihre [!DNL Jira] Probleme dieses Feld in [!UICONTROL Jira] aktualisiert sehen können. </p> </td> 
  </tr> 
  <tr> 
   <td>Benutzerdefinierte Forms- und benutzerdefinierte Felder</td> 
   <td> <p> Anzeige im rechten Bereich von [!DNL Workfront] des Problems [!DNL Jira]. <br>Im Bedienfeld werden nur die benutzerdefinierten Felder mit einem tatsächlichen Wert angezeigt.<br></p> <p>Hinweis: Die Abschnitte Benutzerdefiniertes Formular werden mit der Zugriffsebene des [!DNL Workfront] -Administrators angezeigt. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Problem oder Aufgabenpriorität]</td> 
   <td>Wird im rechten Bereich von [!DNL Jira] angezeigt. [!DNL Workfront] <br>Das Feld <strong>[!UICONTROL Priority]</strong> in [!DNL Jira] wird nicht aktualisiert. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Protokollzeit] </td> 
   <td> <p>Auf der Registerkarte <strong>[!DNL Workfront]</strong> des [!DNL Jira]-Problems wird ein Kommentar zur protokollierten Zeit hinzugefügt. Dazu gehören der Name des Benutzers, der die Zeit protokolliert, sowie der Benutzer, für den die Zeit protokolliert wird, falls er anders ist. Auf der Registerkarte <strong>[!UICONTROL Arbeitsprotokoll]</strong> in [!DNL Jira] wird keine Zeit protokolliert.<br></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Kommentare]</td> 
   <td> <p>Der Kommentar wird der Registerkarte <strong>[!DNL Workfront]</strong> des [!DNL Jira]-Problems hinzugefügt. Sie wird nicht zur Registerkarte <strong>[!UICONTROL Kommentare]</strong> des [!DNL Jira]-Problems hinzugefügt.</p> <p>Hinweis: Wenn Sie zwei vorhandene Elemente manuell verknüpfen, werden die Kommentare, die zum Element [!DNL Workfront] hinzugefügt wurden, bevor Sie es mit [!DNL Jira] verknüpfen, nicht mit dem Problem [!DNL Jira] synchronisiert. </p> <p>Jira-Kommentare werden mit Workfront synchronisiert.</td> 
  </tr> 
 </tbody> 
</table>

## Verknüpfte Elemente in [!DNL Jira] aktualisieren

Wenn Sie primär in [!DNL Jira] arbeiten, können Sie Ihre Arbeitselemente in [!DNL Jira] aktualisieren und ihre Gegenstücke in [!DNL Workfront] ebenfalls aktualisieren. Sie benötigen keine [!DNL Workfront] Lizenz für die [!DNL Workfront] Elemente, die mit Ihren [!DNL Jira] -Problemen verknüpft sind, um die Aktualisierungen zu erhalten, die Sie in [!DNL Jira] vornehmen.

Unter der Bedingung, dass Ihr [!DNL Workfront] -Administrator [!DNL Workfront] für [!DNL Jira] konfiguriert hat, die Felder zwischen verknüpften Elementen zu synchronisieren, werden bestimmte Felder, die Sie in [!DNL Jira] aktualisieren, auch für das verknüpfte [!DNL Workfront] -Element aktualisiert.

Die folgende Liste zeigt, welche [!DNL Jira] -Felder mit [!DNL Workfront] -Feldern für verknüpfte Elemente synchronisiert werden:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Aktualisiertes [!DNL Jira] Feld</strong> </th> 
   <th><strong>Synchronisiertes [!DNL Workfront] Feld/ Update</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Problemstatus]</td> 
   <td> <p> [!UICONTROL Problem oder Aufgabenstatus]</p> <p>Der Problemstatus in [!DNL Jira] wird in Workfront mit den folgenden Status oder Status synchronisiert, die mit den folgenden Status übereinstimmen:</p> 
    <ul> 
     <li> <p>[!UICONTROL Neu] ([!UICONTROL NEW])</p> </li> 
     <li> <p>[!UICONTROL In Bearbeitung] ([!UICONTROL INP])</p> </li> 
     <li> <p>[!UICONTROL Closed]/[!UICONTROL Complete] ([!UICONTROL CLS]/[!UICONTROL CPL])</p> </li> 
    </ul> <p>Hinweis: Der Status [!DNL Jira] wird mit dem ersten [!DNL Workfront] -Status synchronisiert, der dem entsprechenden Status entspricht.</p> <p>Weitere Informationen zum Status von Elementen in [!DNL Workfront] finden Sie unter <a href="../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md" class="MCXref xref">Erstellen oder Bearbeiten eines Status</a>.</p> </td> 
  </tr>
  <tr> 
   <td>[!UICONTROL Problemanlagen]</td> 
   <td> [!UICONTROL Problem oder Aufgabendokumente]<br>Der Registerkarte [!UICONTROL Aktualisierungen] des [!DNL Workfront] -Problems oder der Aufgabe wird ein Kommentar zum Hochladen eines neuen Dokuments in [!DNL Jira] hinzugefügt.  </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Fälligkeitsdatum]</td> 
   <td> <p> Ein Kommentar zur Änderung des [!UICONTROL Fälligkeitsdatums] in [!DNL Jira] wird der Registerkarte [!UICONTROL Updates] der [!DNL Workfront] Ausgabe oder Aufgabe hinzugefügt. </p> <p>Hinweis: Beim [!DNL Workfront]-Problem oder der Aufgabe werden keine Datumsänderungen vorgenommen. </p> </td> 
  </tr> 
  <tr> 
   <td> Protokollzeit im rechten Bereich [!DNL Workfront] oder im Menü [!UICONTROL Mehr] im Problem [!DNL Jira]<br></td> 
   <td> <p>Stunden<br>Zusätzlich zum Hinzufügen der im Jira angemeldeten Stunden zum verknüpften [!DNL Workfront]-Element wird der Registerkarte [!UICONTROL Updates] des Elements [!DNL Workfront] ein Kommentar zur Protokollierungszeit hinzugefügt.</p> <p>Weitere Informationen zur Protokollierungszeit bei verknüpften [!DNL Jira]-Problemen, einschließlich der Aktualisierung des [!DNL Jira]-Benutzers, der die Zeit in [!DNL Workfront] protokolliert, finden Sie unter <a href="#log-time-for-linked-jira-and-workfront-items" class="MCXref xref">Protokollzeit für verknüpfte [!DNL Jira] und [!DNL Workfront] Elemente</a>.</p> </td> 
  </tr> 
  <tr> 
   <td> Kommentare <br><br></td> 
   <td> <p>Kommentare werden auf der Registerkarte [!UICONTROL Updates] des [!DNL Workfront]-Problems oder der Aufgabe hinzugefügt, wenn die Einstellung <strong>[!UICONTROL Kommentare]</strong> im Abschnitt [!UICONTROL SYNCHRONISIEREN VON JIRA ZU WORKFRONT] auf der Registerkarte [!UICONTROL Setup] auf <strong>[!UICONTROL Always]</strong> gesetzt ist.</p> <p>Informationen zum Konfigurieren von Workfront-Einstellungen in [!DNL Jira] finden Sie unter <a href="../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md">Konfigurieren von [!DNL Workfront for Jira]</a>.</p> <p>Informationen zur Kommentar zu Elementen aus verknüpften [!DNL Jira]-Problemen finden Sie unter <a href="#comment-from-a-linked-jira-issue" class="MCXref xref">Kommentar aus einem verknüpften [!DNL Jira] Problem</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Protokollzeit von verknüpften [!DNL Jira] -Problemen

Die Zeit, die Sie für ein [!DNL Jira] Element in [!DNL Jira] aufzeichnen, wird auch auf das verknüpfte [!DNL Workfront] Element übertragen, unabhängig davon, wo in [!DNL Jira] Sie die Zeit protokollieren.\
Wenn Sie die Zeit in Jira im Bedienfeld [!DNL Workfront] protokollieren, wird die Zeit nur in [!DNL Workfront] aufgezeichnet.\
Die Zeit, die Sie in [!DNL Workfront] aufzeichnen, wirkt sich nicht auf die Zeit des verknüpften Problems in [!DNL Jira] aus.

>[!NOTE]
>
>Wenn die Zeit einem [!DNL Jira] -Element hinzugefügt wird, das mit einer [!DNL Workfront] -Aufgabe verknüpft ist, lautet der [!UICONTROL Stündungstyp] für die Zeit in [!DNL Workfront] [!UICONTROL Task Time]. Wenn die Zeit einem [!DNL Jira] -Element hinzugefügt wird, das mit einem [!DNL Workfront] -Problem verknüpft ist, lautet der [!UICONTROL Stündungstyp] für die Zeit in [!DNL Workfront] [!UICONTROL Problemzeit].

Der Registerkarte **[!DNL Workfront]** in [!DNL Jira] und der Registerkarte **[!UICONTROL Aktualisierungen]** des Elements in [!DNL Workfront] wird ein Kommentar hinzugefügt, um die Protokollierung der Zeit aufzuzeichnen.\
Die Zeit wird auch auf der Registerkarte **[!UICONTROL Stunden]** des Elements [!DNL Workfront] angezeigt.

* [Protokollzeit für verknüpfte [!DNL Jira] und  [!DNL Workfront] Elemente](#log-time-for-linked-jira-and-workfront-items)
* [Protokollzeit von  [!DNL Jira]  zu einem  [!DNL Workfront]  Element](#log-time-from-jira-to-a-workfront-item)

### Protokollzeit für verknüpfte Elemente [!DNL Jira] und [!DNL Workfront]

Sie können die Zeit aus einem [!DNL Jira] -Problem protokollieren, das mit einem [!DNL Workfront] -Element verknüpft ist, und die Zeit wird sowohl beim [!DNL Jira] -Problem als auch beim [!DNL Workfront] -Element aufgezeichnet.

>[!IMPORTANT]
>
>Wenn der Benutzer, der die Zeit in [!DNL Jira] protokolliert, nicht in [!DNL Workfront] vorhanden ist, erstellt die Integration einen neuen aktiven Benutzer in Workfront, wenn der Benutzer **[!UICONTROL automatisch einen Benutzer in [!DNL Workfront] erstellt, &#x200B; der Benutzer [!DNL Jira] nicht über ein *[!DNL Workfront] &#x200B; Konto]** auf**[!UICONTROL  Always ]**verfügt. Dieser Benutzer besitzt keine [!DNL Workfront] -Lizenz. Sie können aktive Benutzer Arbeitselementen in [!DNL Workfront] zuweisen, sie können sie jedoch nicht in Aktualisierungen einbeziehen. Informationen zum Konfigurieren der automatischen Erstellung von [!DNL Workfront] Benutzern von [!DNL Jira] finden Sie unter [Konfigurieren [!DNL Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

So protokollieren Sie die Zeit für ein Element in [!DNL Jira] und lassen es sowohl in [!DNL Jira] als auch in [!DNL Workfront] aufgezeichnet werden:

1. Melden Sie sich bei [!DNL Jira] an.
1. Gehen Sie zum Problem [!DNL Jira] , das mit dem Element [!DNL Workfront] verknüpft ist.
1. Erweitern Sie das Menü **[!UICONTROL Mehr]** und klicken Sie auf **[!UICONTROL Protokoll funktioniert]**.

1. Geben Sie im Feld **[!UICONTROL Besuchszeit]** die Zeit an, die mit der Bearbeitung dieses Problems verbracht wurde. Sie müssen die Zeit mithilfe der folgenden Zeiträume angeben:

   * [!UICONTROL Wochen] (w)
   * [!UICONTROL Days] (d)
   * [!UICONTROL Stunden] (h)

1. Fügen Sie Ihrem Zeiteintrag weitere Informationen hinzu, einschließlich einer **[!UICONTROL Arbeitsbeschreibung]**, und klicken Sie dann auf **[!UICONTROL Protokoll]**.\
   Die Zeit wird der Registerkarte **[!UICONTROL Arbeitsprotokoll]** des Elements [!DNL Jira] sowie dem damit verknüpften Element [!DNL Workfront] hinzugefügt.\
   Die Arbeitsbeschreibung des Zeiteintrags wird als Hinweis beim Stundeneintrag in [!DNL Workfront] aufgezeichnet.

### Protokollzeit von [!DNL Jira] zu einem [!DNL Workfront] Element

Sie können die Zeit vom [!DNL Jira] -Problem nur auf das verknüpfte [!DNL Workfront] -Element protokollieren, ohne dieses Mal das [!DNL Jira] -Problem aufzuzeichnen.

1. Melden Sie sich bei [!DNL Jira] an.
1. Navigieren Sie zu einem [!DNL Jira] -Problem, das mit einem [!DNL Workfront] -Element verknüpft ist.

   Die Details des Elements [!DNL Workfront] sollten im rechten Bereich [!DNL Workfront] des Problems angezeigt werden.

1. Klicken Sie auf das Symbol **[!UICONTROL Protokollzeit]**.

1. Geben Sie den Betrag von **[!UICONTROL Stunden]** und **[!UICONTROL Minuten]** an, den Sie für das Problem protokollieren möchten.

1. Klicken Sie auf **[!UICONTROL Protokollzeit]**.

   Die Zeit wird dem Element [!DNL Workfront] hinzugefügt.

   Diese Zeit wird der Registerkarte [!UICONTROL Arbeitsprotokoll] des [!DNL Jira]-Problems nicht hinzugefügt.

## Kommentar zu einem verknüpften [!DNL Jira]-Problem {#comment-from-a-linked-jira-issue}

Wenn Sie ein [!DNL Jira] -Element aus dem rechten Bereich [!DNL Workfront] in [!DNL Jira] kommentieren, wird der Kommentar auch zur Registerkarte [!UICONTROL Aktualisierungen] des verknüpften Elements in Workfront hinzugefügt.

So kommentieren Sie von [!DNL Jira] zu einem [!DNL Workfront] -Element:

1. Melden Sie sich bei [!DNL Jira] an.
1. Navigieren Sie zu einem [!DNL Jira] -Problem, das mit einem [!DNL Workfront] -Element verknüpft ist.

   Die Details des Elements [!DNL Workfront] sollten im rechten Bereich [!DNL Workfront] des Problems angezeigt werden.

1. Klicken Sie auf das Symbol **[!UICONTROL Kommentare]** im Bedienfeld [!DNL Workfront] oder auf der Registerkarte **[!UICONTROL Kommentare]**.

1. Beginnen Sie mit der Eingabe eines Kommentars und klicken Sie dann auf **[!UICONTROL Senden]**.

   Der Kommentar wird wie folgt hinzugefügt:

   * Die Registerkarte **[!DNL Workfront]** des [!DNL Jira]-Problems.
   * Die Registerkarte **[!UICONTROL Kommentare]** des [!DNL Jira]-Problems.
   * Die Registerkarte **[!UICONTROL Aktualisierungen]** des verknüpften Elements in Workfront.
