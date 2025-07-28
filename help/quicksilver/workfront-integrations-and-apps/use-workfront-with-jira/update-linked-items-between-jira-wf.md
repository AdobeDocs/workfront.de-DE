---
product-area: workfront-integrations
navigation-topic: workfront-for-jira
title: Aktualisieren von verknüpften Elementen zwischen [!DNL Jira] und [!DNL Adobe Workfront]
description: Wenn Sie Probleme  [!DNL Jira]  Aufgaben oder  [!DNL Adobe Workfront]  verknüpfen, können Ihre Benutzer Elemente in einer Anwendung aktualisieren. Das Gegenstück zu diesem Element wird auch für die Benutzer aktualisiert, die in der zweiten Anwendung arbeiten.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 79ac6ff1-2f7d-4abc-8735-398f6aac5191
source-git-commit: f9af669b023309abc132421f35a2ece974e796b0
workflow-type: tm+mt
source-wordcount: '1700'
ht-degree: 0%

---

# Aktualisieren verknüpfter Elemente zwischen [!DNL Jira] und [!DNL Adobe Workfront]

>[!IMPORTANT]
>
>Um stabilere und skalierbarere Integrationen bereitzustellen, wechseln wir mithilfe von Workfront Automation and Integration (Fusion) zu einem modernen, flexiblen Integrationsansatz. Im Rahmen dieses Übergangsprozesses wird die Integration von Workfront für Jira nach dem 28. **2026 nicht mehr**.
>
>Es wird empfohlen, Workfront-Automatisierung und -Integration für die Integrationsanforderungen Ihres Unternehmens mit Jira zu verwenden.
>
>Acht einsatzbereite Workfront-Automatisierungs- und Integrationsvorlagen für Jira werden bis August verfügbar sein, um gängige Workflows zu replizieren und die Implementierung zu beschleunigen. Vorlagen können vollständig an spezifische Geschäftsanforderungen angepasst und bei sich ändernden Anforderungen erweitert werden.
> 
>Einen Überblick über die Automatisierung und Integration von Workfront finden Sie unter [Übersicht über Adobe Workfront Fusion](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview).
>
>Informationen zu den spezifischen Funktionen der Workfront-Automatisierungs- und Integrationsmodule für Jira finden Sie unter [Jira-Softwaremodule](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/jira-software-modules).

Wenn Sie [!DNL Jira] Probleme mit [!DNL Adobe Workfront] Aufgaben oder Problemen verknüpfen, können Ihre Benutzerinnen und Benutzer Elemente in einer Anwendung aktualisieren. Das Gegenstück zu diesem Element wird auch für die Benutzerinnen und Benutzer aktualisiert, die in der zweiten Anwendung arbeiten.

Weitere Informationen zum Verknüpfen von Elementen zwischen [!DNL Workfront] und [!DNL Jira] finden Sie unter [Verknüpfen von Elementen zwischen Adobe Workfront und Jira](../../workfront-integrations-and-apps/use-workfront-with-jira/link-items-between-wf-jira.md).

Beim Einrichten von [!DNL Workfront] für [!DNL Jira] können Sie als [!DNL Jira]-Systemadministrator bestimmte Felder in einer Anwendung so konfigurieren, dass sie mit Feldern aus verknüpften Elementen in der anderen Anwendung synchronisiert werden.

Weitere Informationen zum Synchronisieren von Feldern zwischen verknüpften [!DNL Jira] und [!DNL Workfront] Elementen finden Sie unter [Konfigurieren [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

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
   <td role="rowheader">[!DNL Jira] Zugriff</td> 
   <td> <p>Systemadministratorzugriff</p> <p>Wichtig: Es wird empfohlen, separate Systemadministratorkonten in [!DNL Jira] und [!DNL Workfront] zu erstellen, um diese Integration zu ermöglichen, anstatt vorhandene Konten zu verwenden, die an Benutzer angehängt sein könnten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Sie müssen [!DNL Workfront] sein.</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Voraussetzungen

Bevor Sie Elemente zwischen [!DNL Workfront] und [!DNL Jira] verknüpfen können, müssen Sie:

* Installieren Sie [!DNL Workfront for Jira].

  Anweisungen zur Installation von [!DNL Workfront for Jira] finden Sie unter [Installieren [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/install-workfront-for-jira.md).

* Konfigurieren Sie [!DNL Workfront for Jira].

  Anweisungen zum Konfigurieren von [!DNL Workfront for Jira] finden Sie unter [Konfigurieren [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

* Elemente zwischen [!DNL Workfront] und [!DNL Jira] verknüpfen.

  Anweisungen finden Sie unter [Verknüpfen von Elementen zwischen [!DNL Adobe Workfront] und [!DNL Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/link-items-between-wf-jira.md).

## Aktualisieren verknüpfter Elemente in [!DNL Workfront]

Wenn Sie hauptsächlich in [!DNL Workfront] arbeiten, können Sie Ihre Arbeitselemente in [!DNL Workfront] aktualisieren und ihre Gegenstücke in [!DNL Jira] ebenfalls aktualisieren. Dieses Update erfolgt durch die Integration von [!DNL Workfront] für [!DNL Jira], für die Sie keine [!DNL Jira] benötigen.

Solange Ihr [!DNL Workfront]-Administrator [!DNL Workfront for Jira] zum Synchronisieren der Felder zwischen verknüpften Elementen konfiguriert hat, werden bestimmte Felder, die Sie in aktualisieren, [!DNL Workfront] auch für das verknüpfte [!DNL Jira] aktualisiert. Weitere Informationen zum Aktualisieren von Elementen in [!DNL Workfront] finden Sie unter [Probleme bearbeiten](../../manage-work/issues/manage-issues/edit-issues.md) und [Aufgaben bearbeiten](../../manage-work/tasks/manage-tasks/edit-tasks.md).

Die folgende Liste zeigt, welche [!DNL Workfront] Felder mit [!DNL Jira] Feldern in verknüpften Elementen synchronisiert werden:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>[!DNL Workfront] Feld wurde aktualisiert</strong> </th> 
   <th><strong>Synchronisiertes [!DNL Jira]/Aktualisierung</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Problem oder Aufgabenname]</td> 
   <td> <p>[!UICONTROL Problemname]</p> <p>Der Registerkarte <strong>[!DNL Workfront]</strong> des [!DNL Jira] Problems wird ein Kommentar zur Namensänderung hinzugefügt. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Problem oder Aufgabenbeschreibung]</td> 
   <td> <p> [!UICONTROL Problembeschreibung]</p> <p>Auf der Registerkarte <strong>[!DNL Workfront]</strong> des [!DNL Jira] Problems wird ein Kommentar zur aktualisierten Beschreibung hinzugefügt.<br></p> </td> 
  </tr> 
  <tr> 
   <td> <p> [!UICONTROL hat Dokumente hochgeladen]</p> <p>Hinweis: Dokumente, die mit [!DNL Workfront] Elementen von einem externen Server verknüpft sind, werden nicht an [!DNL Jira] übertragen. Nur Dokumente, die direkt in [!DNL Workfront] Elemente hochgeladen werden, werden auch auf die verknüpften [!DNL Jira] aktualisiert. </p> </td> 
   <td> <p>[!UICONTROL Anlagen]</p> <p>Auf der Registerkarte <strong>[!DNL Workfront]</strong> des [!DNL Jira] Problems wird ein Kommentar zu den hochgeladenen Anhängen hinzugefügt.<br></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Geplantes Abschlussdatum]</td> 
   <td> <p>[!UICONTROL Fälligkeitsdatum]</p> <p>Ein Kommentar zur Änderung des [!UICONTROL Due Date] wird der Registerkarte [!DNL Workfront] des [!DNL Jira] hinzugefügt. </p> <p>Hinweis: Sie müssen <strong>[!UICONTROL Due Date]</strong> aktivieren, damit Ihre [!DNL Jira] Probleme dieses Feld in [!UICONTROL Jira] aktualisiert sehen können. </p> </td> 
  </tr> 
  <tr> 
   <td>Benutzerdefinierte Forms und benutzerdefinierte Felder</td> 
   <td> <p> Wird im [!DNL Workfront] rechten Bedienfeld des [!DNL Jira] Problems angezeigt. <br>Im Bedienfeld werden nur die benutzerdefinierten Felder angezeigt, die über einen tatsächlichen Wert verfügen.<br></p> <p>Hinweis: Benutzerdefinierte Formularabschnitte werden mit der Zugriffsebene des [!DNL Workfront]-Administrators angezeigt. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Problem oder Aufgabenpriorität]</td> 
   <td>Wird im [!DNL Workfront] rechten Bedienfeld des [!DNL Jira] Problems angezeigt. <br>Das Feld <strong>[!UICONTROL Priority]</strong> in [!DNL Jira] wird nicht aktualisiert. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Protokollzeit] </td> 
   <td> <p>Auf der Registerkarte <strong>[!DNL Workfront]</strong> des [!DNL Jira] Problems wird ein Kommentar zur protokollierten Zeit hinzugefügt. Dazu gehören der Name des Benutzers, der die Zeit protokolliert, sowie der Benutzer, für den die Zeit protokolliert wird, falls sie nicht identisch sind. Auf der Registerkarte <strong>[!UICONTROL Work Log]</strong> in [!DNL Jira] wird keine Zeit protokolliert.<br></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Kommentare]</td> 
   <td> <p>Der Kommentar wird der Registerkarte "<strong>[!DNL Workfront]</strong>" des [!DNL Jira] hinzugefügt. Er wird nicht zur Registerkarte <strong>[!UICONTROL Kommentare]</strong> des [!DNL Jira] hinzugefügt</p> <p>Hinweis: Wenn Sie zwei vorhandene Elemente manuell verknüpfen, werden die Kommentare, die dem [!DNL Workfront] Element vor dem Verknüpfen mit hinzugefügt wurden, [!DNL Jira] mit dem [!DNL Jira] Problem synchronisiert. </p> <p>Jira-Kommentare werden mit Workfront synchronisiert.</td> 
  </tr> 
 </tbody> 
</table>

## Aktualisieren verknüpfter Elemente in [!DNL Jira]

Wenn Sie hauptsächlich in [!DNL Jira] arbeiten, können Sie Ihre Arbeitselemente in [!DNL Jira] aktualisieren und ihre Gegenstücke in [!DNL Workfront] ebenfalls aktualisieren. Sie benötigen keine [!DNL Workfront]-Lizenz für die [!DNL Workfront] Elemente, die mit Ihren [!DNL Jira] Problemen verknüpft sind, um die Aktualisierungen zu erhalten, die Sie in [!DNL Jira] vornehmen.

Sofern Ihr [!DNL Workfront]-Administrator [!DNL Workfront] für [!DNL Jira] konfiguriert hat, um die Felder zwischen verknüpften Elementen zu synchronisieren, werden bestimmte Felder, die Sie in aktualisieren, [!DNL Jira] auch für das verknüpfte [!DNL Workfront]-Element aktualisiert.

Die folgende Liste zeigt, welche [!DNL Jira] Felder mit [!DNL Workfront] Feldern in verknüpften Elementen synchronisiert werden:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>[!DNL Jira] Feld wurde aktualisiert</strong> </th> 
   <th><strong>Synchronisiertes [!DNL Workfront]/Feld aktualisieren</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Problemstatus]</td> 
   <td> <p> [!UICONTROL Problem- oder Aufgabenstatus]</p> <p>Problemstatus in [!DNL Jira] synchronisiert mit den folgenden Status oder Status, die den folgenden Status entsprechen, in Workfront:</p> 
    <ul> 
     <li> <p>[!UICONTROL NEU] ([!UICONTROL NEU])</p> </li> 
     <li> <p>[!UICONTROL IN BEARBEITUNG] ([!UICONTROL INP])</p> </li> 
     <li> <p>[!UICONTROL geschlossen]/[!UICONTROL abgeschlossen] ([!UICONTROL CLS]/[!UICONTROL CPL])</p> </li> 
    </ul> <p>Hinweis: Der [!DNL Jira] synchronisiert den ersten [!DNL Workfront], der dem entsprechenden Status entspricht.</p> <p>Weitere Informationen zum Status von Elementen in [!DNL Workfront] finden Sie unter <a href="../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md" class="MCXref xref">Erstellen oder Bearbeiten eines Status</a>.</p> </td> 
  </tr>
  <tr> 
   <td>[!UICONTROL Problemanhänge]</td> 
   <td> [!UICONTROL Problem- oder Aufgabendokumente]<br>Ein Kommentar zum Hochladen eines neuen Dokuments in [!DNL Jira] wird der Registerkarte [!UICONTROL-Aktualisierungen] des [!DNL Workfront] Problems oder der Aufgabe hinzugefügt.  </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Fälligkeitsdatum]</td> 
   <td> <p> Ein Kommentar zur Änderung des [!UICONTROL Due Date] in [!DNL Jira] wird der Registerkarte [!UICONTROL Updates] des [!DNL Workfront] Problems oder der Aufgabe hinzugefügt. </p> <p>Hinweis: Für das [!DNL Workfront] Problem oder die Aufgabe ändern sich keine Daten. </p> </td> 
  </tr> 
  <tr> 
   <td> Zeit im rechten [!DNL Workfront]-Bedienfeld oder über das Menü [!UICONTROL Mehr] zum [!DNL Jira] Problem protokollieren<br></td> 
   <td> <p>Stunden<br>Zusätzlich zum Hinzufügen der in Jira protokollierten Stunden zum verknüpften [!DNL Workfront] wird auf der Registerkarte [!UICONTROL Updates] des [!DNL Workfront]-Elements ein Kommentar zur Protokollierungszeit hinzugefügt.</p> <p>Weitere Informationen zur Zeitprotokollierung bei Problemen mit verknüpften [!DNL Jira], einschließlich der Aktualisierung des [!DNL Jira] Benutzers, der die Zeit in [!DNL Workfront] protokolliert, finden Sie unter <a href="#log-time-for-linked-jira-and-workfront-items" class="MCXref xref">Zeit für verknüpfte [!DNL Jira] und [!DNL Workfront] Elemente protokollieren</a>.</p> </td> 
  </tr> 
  <tr> 
   <td> Kommentare <br><br></td> 
   <td> <p>Kommentare werden zur Registerkarte [!UICONTROL Updates] des [!DNL Workfront] Problems oder der Aufgabe hinzugefügt, wenn die Einstellung <strong>[!UICONTROL Comments]</strong> im Abschnitt [!UICONTROL SYNCHRONIZE FROM JIRA TO WORKFRONT] der Registerkarte [!UICONTROL Setup] auf <strong>[!UICONTROL Always]</strong>.</p> <p>Informationen zum Konfigurieren der Workfront-Einstellungen in [!DNL Jira] finden Sie unter <a href="../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md">Konfigurieren von [!DNL Workfront for Jira]</a>.</p> <p>Informationen zum Kommentieren von Elementen aus verknüpften [!DNL Jira] finden Sie unter <a href="#comment-from-a-linked-jira-issue" class="MCXref xref">Kommentar aus einem verknüpften [!DNL Jira]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Zeit aus verknüpften [!DNL Jira]-Problemen protokollieren

Die Zeit, die Sie für ein [!DNL Jira] Element in [!DNL Jira] aufzeichnen, wird auch auf das verknüpfte [!DNL Workfront] Element übertragen, unabhängig davon, wo in [!DNL Jira] Sie die Zeit erfassen.\
Wenn Sie die Zeit in Jira im [!DNL Workfront] Panel protokollieren, wird die Zeit nur in [!DNL Workfront] aufgezeichnet.\
Die Zeit, die Sie in [!DNL Workfront] aufzeichnen, wirkt sich nicht auf die Zeit des verknüpften Problems in [!DNL Jira] aus.

>[!NOTE]
>
>Wenn die Zeit zu einem [!DNL Jira] Element hinzugefügt wird, das mit einer [!DNL Workfront] Aufgabe verknüpft ist, lautet [!UICONTROL Stundentyp] für die Zeit in [!DNL Workfront] &quot;[!UICONTROL -Aufgabe]. Wenn die Zeit zu einem [!DNL Jira] Element hinzugefügt wird, das mit einem [!DNL Workfront] Problem verknüpft ist, lautet [!UICONTROL Stundentyp] für die Zeit in [!DNL Workfront] [!UICONTROL Problemzeit].

Um die Protokollierungszeit zu erfassen, wird der Registerkarte **[!DNL Workfront]** in [!DNL Jira] und der Registerkarte **[!UICONTROL Aktualisierungen]** des Elements in [!DNL Workfront] ein Kommentar hinzugefügt.\
Die Uhrzeit wird auch auf der Registerkarte **[!UICONTROL Stunden]** des [!DNL Workfront] Elements angezeigt.

* [Zeit für verknüpfte  [!DNL Jira] / [!DNL Workfront]  protokollieren](#log-time-for-linked-jira-and-workfront-items)
* [Zeit von/ [!DNL Jira]  einem/ [!DNL Workfront]  protokollieren](#log-time-from-jira-to-a-workfront-item)

### Zeit für verknüpfte [!DNL Jira] und [!DNL Workfront] Elemente protokollieren

Sie können die Zeit aus einem [!DNL Jira] Problem protokollieren, das mit einem [!DNL Workfront] Element verknüpft ist, und die Zeit wird sowohl für das [!DNL Jira] Problem als auch für das [!DNL Workfront] Element aufgezeichnet.

>[!IMPORTANT]
>
>Wenn der Benutzer, der die Zeit in [!DNL Jira] protokolliert, in [!DNL Workfront] nicht vorhanden ist, erstellt die Integration einen neuen aktiven Benutzer in Workfront, wenn **[!UICONTROL Automatisch einen Benutzer in [!DNL Workfront] erstellen&#x200B;wenn der [!DNL Jira] *Benutzer kein[!DNL Workfront]&#x200B;Konto]** auf**[!UICONTROL  Immer ]**gesetzt ist. Dieser Benutzer ist nicht im Besitz einer [!DNL Workfront]. Sie können aktive Benutzer Arbeitselementen in [!DNL Workfront] zuweisen, sie jedoch nicht in Aktualisierungen einbeziehen. Informationen zum Konfigurieren der automatischen Erstellung [!DNL Workfront] Benutzer aus [!DNL Jira] finden Sie unter [Konfigurieren [!DNL Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

So protokollieren Sie die Zeit für ein Element in [!DNL Jira] und lassen es sowohl in [!DNL Jira] als auch [!DNL Workfront] aufzeichnen:

1. Anmelden bei [!DNL Jira].
1. Navigieren Sie zum [!DNL Jira] Problem, das mit dem [!DNL Workfront] Element verknüpft ist.
1. Erweitern Sie das Menü **[!UICONTROL Mehr]** und klicken Sie auf **[!UICONTROL Arbeit protokollieren]**.

1. Geben Sie **[!UICONTROL Feld „Aufgewendete]**&quot; die Zeit an, die mit der Bearbeitung dieses Problems verbracht wurde. Sie müssen die Zeit in den folgenden Zeiträumen angeben:

   * [!UICONTROL Wochen] (w)
   * [!UICONTROL Tage] (d)
   * [!UICONTROL Stunden] (h)

1. Fügen Sie Ihrem Zeiteintrag weitere Informationen hinzu, einschließlich einer **[!UICONTROL Arbeitsbeschreibung]**, und klicken Sie dann auf **[!UICONTROL Protokoll]**.\
   Die Zeit wird der Registerkarte **[!UICONTROL Arbeitsprotokoll]** des [!DNL Jira] Elements sowie dem damit verknüpften [!DNL Workfront] Element hinzugefügt.\
   Die Arbeitsbeschreibung des Zeiteintrags wird als Notiz auf dem Stundeneintrag in [!DNL Workfront] aufgezeichnet.

### Zeit von [!DNL Jira] in ein [!DNL Workfront] Element protokollieren

Sie können die Zeit aus dem [!DNL Workfront] Problem nur für das verknüpfte [!DNL Jira]-Element protokollieren, ohne diese Zeit für das [!DNL Jira] Problem aufzuzeichnen.

1. Anmelden bei [!DNL Jira].
1. Navigieren Sie zu einem [!DNL Jira] Problem, das mit einem [!DNL Workfront] Element verknüpft ist.

   Die Details des [!DNL Workfront] Elements sollten im [!DNL Workfront] rechten Bedienfeld des Problems angezeigt werden.

1. Klicken Sie auf **[!UICONTROL Symbol]** Zeit protokollieren“.

1. Geben Sie die Anzahl von **[!UICONTROL Stunden]** und **[!UICONTROL Minuten]** an, die Sie für das Problem protokollieren möchten.

1. Klicken Sie **[!UICONTROL Zeit protokollieren]**.

   Die Zeit wird dem [!DNL Workfront] hinzugefügt.

   Diese Zeit wird nicht zur Registerkarte [!UICONTROL Arbeitsprotokoll] des [!DNL Jira] hinzugefügt.

## Kommentar aus einem verknüpften [!DNL Jira] {#comment-from-a-linked-jira-issue}

Wenn Sie einen Kommentar zu einem [!DNL Jira] Element im [!DNL Workfront] rechten Bereich in [!DNL Jira] abgeben, wird der Kommentar auch zur Registerkarte [!UICONTROL Aktualisierungen] des verknüpften Elements in Workfront hinzugefügt.

So fügen Sie einen Kommentar von [!DNL Jira] zu einem [!DNL Workfront] ein:

1. Anmelden bei [!DNL Jira].
1. Navigieren Sie zu einem [!DNL Jira] Problem, das mit einem [!DNL Workfront] Element verknüpft ist.

   Die Details des [!DNL Workfront] Elements sollten im [!DNL Workfront] rechten Bedienfeld des Problems angezeigt werden.

1. Klicken Sie auf **[!UICONTROL Symbol]** Kommentare[!DNL Workfront] im Bedienfeld oder auf der Registerkarte **[!UICONTROL Kommentare]**.

1. Geben Sie einen Kommentar ein und klicken Sie dann auf **[!UICONTROL Senden]**.

   Der Kommentar wird wie folgt hinzugefügt:

   * Die Registerkarte &quot;**[!DNL Workfront]**&quot; des [!DNL Jira] Problems.
   * Die **[!UICONTROL Kommentare]** des [!DNL Jira] Problems.
   * Die **[!UICONTROL Aktualisierungen]** des verknüpften Elements in Workfront.
