---
product-area: projects
navigation-topic: use-the-gantt-chart
title: Aktualisieren von Informationen in der Aufgabenliste Gantt-Diagramm
description: Das Gantt-Diagramm der Aufgabenliste zeigt Details zu Aufgaben an, die sich auf ein Projekt oder eine Vorlage beziehen.
author: Alina
feature: Work Management
exl-id: 0a8e6fd5-985c-49e5-842d-67ade29ee1c9
source-git-commit: 7c373707f6e5ec1431e38cc0e103e25cd8cf2309
workflow-type: tm+mt
source-wordcount: '1021'
ht-degree: 1%

---

# Informationen in der Aufgabenliste aktualisieren [!UICONTROL Gantt-Diagramm]

Aufgabenliste [!UICONTROL Gantt-Diagramm] zeigt Details zu Aufgaben an, die sich auf ein Projekt oder eine Vorlage beziehen.

In einer Vorlage die Aufgabenliste [!UICONTROL Gantt-Diagramm] spiegelt Aktualisierungen wider, die auf Aufgabenebene in der Aufgabenliste der Vorlage vorgenommen wurden. Sie können die [!UICONTROL Gantt-Diagramm] mit einer Vorlage verknüpft ist.

In einem Projekt können Sie Aufgabeninformationen direkt in der Aufgabenliste aktualisieren [!UICONTROL Gantt-Diagramm].

In diesem Artikel werden die folgenden Aktionen beschrieben, die Sie direkt in der Aufgabenliste ausführen können [!UICONTROL Gantt-Diagramm]:

* Ändern der Aufgabendauer
* Erstellen oder Entfernen von Vorgängerbeziehungen
* Beginn und Ende von Aufgaben ändern
* Prozentsatz aktualisieren abgeschlossen
* Level-Projektressourcen

## Zugriffsanforderungen

Sie müssen über Folgendes verfügen, um die Schritte in diesem Artikel zu befolgen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Plan*</td> 
   <td> <p>Beliebig </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td> <p>[!UICONTROL Plan] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>[!UICONTROL Zugriff auf Projekte und Aufgaben bearbeiten</p> <p>Hinweis: Wenn Sie noch keinen Zugriff haben, fragen Sie Ihren [!DNL Workfront] Administrator , wenn sie zusätzliche Einschränkungen für Ihre Zugriffsebene festlegen. Für Informationen zur [!DNL Workfront] Administrator kann Ihre Zugriffsebene ändern, siehe <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>[!UICONTROL] Zugriff auf das Projekt und die Aufgaben verwalten </p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren [!DNL Workfront] Administrator.

## Ändern der Aufgabendauer

1. Wechseln Sie zu dem Projekt, das Sie ändern möchten.
1. Klicken **[!UICONTROL Aufgaben]** im linken Bereich.

   ![](assets/qs-tasks-area-highlighted-in-the-secondary-nav-350x206.png)

1. Klicken Sie auf **[!UICONTROL Gantt-Diagramm]** Symbol.

   ![Klicken Sie auf das Symbol &quot;Gantt-Diagramm&quot;](assets/click-gantt-chart-icon.png)

   Alle Änderungen werden automatisch gespeichert, wenn die Variable **[!UICONTROL Automatische Speicherung]** aktiviert ist. Sie ist standardmäßig aktiviert.

1. (Optional) Klicken Sie auf die **[!UICONTROL Planmodus]** Symbol und wählen Sie **[!UICONTROL Manuelles Speichern Standard]** oder **[!UICONTROL Timeline-Planung]** , um Ihre Änderungen manuell zu speichern.

   ![](assets/manual-standard-setting-enabled-quicksilver-task-list-350x493.png)

1. Bewegen Sie den Mauszeiger über die Zeitleiste einer Aufgabe und ziehen Sie die Zeitleistenanzeige an ein anderes Datum.
1. Legen Sie den Indikator ab, wenn Sie das richtige neue Abschlussdatum für die Aufgabe erreicht haben.
1. (Optional und bedingt) Wenn Sie ausgewählt haben, Ihre Änderungen manuell zu speichern, klicken Sie auf die Schaltfläche **[!UICONTROL Rückgängig]** oder &#x200B;**[!UICONTROL Wiederholen]** -Symbole, wenn Sie eine der Änderungen abbrechen oder duplizieren möchten.

   >[!TIP]
   >
   >Sie können die folgenden Tastaturbefehle verwenden, um Änderungen am Gantt-Diagramm rückgängig zu machen oder wiederherzustellen:
   >
   >   
   >   
   >   * [!DNL Mac]: Verwendung [!UICONTROL Befehl + Z] zum Rückgängigmachen und [!UICONTROL Befehl + Umschalt + Z] zurück.
   >   * [!DNL Windows]: Verwendung [!UICONTROL Strg + Z] zum Rückgängigmachen und [!UICONTROL Strg + Y] zurück.
   >   
   >

1. Klicken **[!UICONTROL Speichern]** in der oberen rechten Ecke des [!UICONTROL Gantt-Diagramm].

## Erstellen oder Entfernen von Vorgängerbeziehungen

1. Wechseln Sie zu dem Projekt, das Sie ändern möchten.
1. Im **[!UICONTROL Aufgaben]** Bereich, klicken Sie auf **[!UICONTROL Gantt-Diagramm]** Symbol.

   Die **[!UICONTROL Automatische Speicherung]** standardmäßig aktiviert ist, werden alle Änderungen automatisch gespeichert.

   ![](assets/qs-gantt-icon-on-task-list-highlighted-350x199.png)

1. (Optional) Klicken Sie auf die **[!UICONTROL Planmodus]** Symbol und wählen Sie **[!UICONTROL Manuelles Speichern Standard]** oder **[!UICONTROL Timeline-Planung]** , um Ihre Änderungen manuell zu speichern.

   ![](assets/manual-standard-setting-enabled-quicksilver-task-list-350x493.png)

1. Um eine Vorgängerbeziehung zu erstellen, klicken Sie auf den Startpunkt einer Aufgabe und ziehen Sie sie an den Endpunkt der Aufgabe.
1. Um eine Vorgängerbeziehung zu löschen, klicken Sie auf eine Vorgängerzeile, die zwei Aufgaben miteinander verbindet, um sie auszuwählen, und drücken Sie dann die Eingabetaste **[!UICONTROL Löschen]** auf Ihrer Tastatur.\
   ![Delete_predecessor.png](assets/delete-predecessor-350x152.png)

1. (Optional und bedingt) Wenn Sie ausgewählt haben, um Ihre Änderungen manuell zu speichern, klicken Sie auf die **[!UICONTROL Rückgängig]** oder &#x200B;**[!UICONTROL Wiederholen]** -Symbole, wenn Sie eine der Änderungen abbrechen oder duplizieren möchten.

   >[!TIP]
   >
   >Sie können die folgenden Tastaturbefehle verwenden, um Änderungen am Gantt-Diagramm rückgängig zu machen oder wiederherzustellen:
   >
   >   
   >   
   >   * [!DNL Mac]: Verwendung [!UICONTROL Befehl + Z] zum Rückgängigmachen und [!UICONTROL Befehl + Umschalt + Z] zurück.
   >   * [!DNL Windows]: [!UICONTROL Strg + Z verwenden] zum Rückgängigmachen und [!UICONTROL Strg + Y] zurück.
   >   
   >

1. Klicken Sie auf **[!UICONTROL Speichern]** .

## Beginn und Ende von Aufgaben ändern

1. Wechseln Sie zu dem Projekt, das Sie ändern möchten.
1. Im **[!UICONTROL Aufgaben]** Bereich, klicken Sie auf **[!UICONTROL Gantt-Diagramm]** Symbol.

   Alle Änderungen werden automatisch gespeichert, wenn die Variable **[!UICONTROL Automatische Speicherung]** aktiviert ist. Sie ist standardmäßig aktiviert.

   ![](assets/qs-gantt-icon-on-task-list-highlighted-350x199.png)

1. (Optional) Klicken Sie auf die **[!UICONTROL Planmodus]** Symbol und wählen Sie **[!UICONTROL Manuelles Speichern Standard]** oder **[!UICONTROL Timeline-Planung]** , um Ihre Änderungen manuell zu speichern.

   ![](assets/manual-standard-setting-enabled-quicksilver-task-list-350x493.png)

1. Bewegen Sie den Mauszeiger über den Mittelpunkt der Aufgabe und suchen Sie den Pfeil mit mehreren Richtungen.
1. Klicken Sie auf die Aufgabe und ziehen Sie sie an das gewünschte Datum.

   ![Change_start_end_date.png](assets/change-start-end-date.png)

1. Wenn Sie das Aufgabendatum in einer Weise ändern, die sich auf die Aufgabenbegrenzung auswirkt, klicken Sie auf **[!UICONTROL Accept]** um die Änderung der Aufgabenbegrenzung zu bestätigen.

   >[!NOTE]
   >
   >Wenn die Aufgabe eine der folgenden Einschränkungen aufweist, aktualisiert das System die [!UICONTROL Aufgabenbegrenzung] nach [!UICONTROL Anfang 2007] Ist der Fall, wenn das Projekt von der [!UICONTROL Startdatum] oder [!UICONTROL Finish No Later Than] , wenn das Projekt über die [!UICONTROL Abschlussdatum]:
   >
   >   
   >   
   >   * [!UICONTROL So bald wie möglich (SBWM)]
   >   * [!UICONTROL So spät wie möglich (SSWM)]
   >   * [!UICONTROL Frühestmögliche Zeit]
   >   * [!UICONTROL Spätestmögliche Zeit]
   >   
   >   
   >In einigen Fällen können die Vorgängerbeziehungen verhindern, dass die Aufgaben früher gestartet werden, und die Verschiebung der Aufgabe ist nicht zulässig.

1. (Optional und bedingt) Wenn Sie ausgewählt haben, Ihre Änderungen manuell zu speichern, klicken Sie auf die Schaltfläche **[!UICONTROL Rückgängig]** oder &#x200B;**[!UICONTROL Wiederholen]** -Symbole, wenn Sie eine der Änderungen abbrechen oder duplizieren möchten.

   >[!TIP]
   >
   >Sie können die folgenden Tastaturbefehle verwenden, um Änderungen an der [!UICONTROL Gantt-Diagramm]:
   >
   >   
   >   
   >   * [!DNL Mac]: Verwendung [!UICONTROL Befehl + Z] zum Rückgängigmachen und [!UICONTROL Befehl + Umschalt + Z] zurück.
   >   * [!DNL Windows]: Verwendung [!UICONTROL Strg + Z] zum Rückgängigmachen und [!UICONTROL Strg + Y] zurück.
   >   
   >

1. Klicken Sie auf **[!UICONTROL Speichern]**.

## Prozentsatz aktualisieren abgeschlossen

1. Wechseln Sie zu dem Projekt, das Sie ändern möchten.
1. Im **[!UICONTROL Aufgaben]** Bereich, klicken Sie auf **[!UICONTROL Gantt-Diagramm]** Symbol.

   ![](assets/qs-gantt-icon-on-task-list-highlighted-350x199.png)

   Alle Änderungen werden automatisch gespeichert, wenn die Variable **[!UICONTROL Automatische Speicherung]** aktiviert ist. Sie ist standardmäßig aktiviert.

1. (Optional) Klicken Sie auf die **[!UICONTROL Planmodus]** Symbol und wählen Sie **[!UICONTROL Manuelles Speichern Standard]** oder **[!UICONTROL Timeline-Planung]** , um Ihre Änderungen manuell zu speichern.
1. Doppelklicken Sie auf die Prozentzahl innerhalb der Aufgabe und geben Sie die Nummer ein.

   >[!IMPORTANT]
   >
   >Sie müssen [!UICONTROL % Complete] in der [!UICONTROL Optionen] angezeigt, um den Prozentsatz des Abschlusses zu aktualisieren. Klicken Sie dazu auf die Schaltfläche **[!UICONTROL Optionen]** Symbol und wählen Sie **[!UICONTROL % Complete]**.
   >
   >
   >![update_percent_complete.png](assets/update-percent-complete-350x175.png)   >
   >

1. (Optional und bedingt) Wenn Sie ausgewählt haben, um Ihre Änderungen manuell zu speichern, klicken Sie auf die **[!UICONTROL Rückgängig]** oder &#x200B;**[!UICONTROL Wiederholen]** -Symbole, wenn Sie eine der Änderungen abbrechen oder duplizieren möchten.

   >[!TIP]
   >
   >Sie können die folgenden Tastaturbefehle verwenden, um Änderungen an der [!UICONTROL Gantt-Diagramm]:
   >
   >   
   >   
   >   * [!DNL Mac]: Verwendung [!UICONTROL Befehl + Z] zum Rückgängigmachen und [!UICONTROL Befehl + Umschalt + Z] zurück.
   >   * [!DNL Windows]: Verwendung [!UICONTROL Strg + Z] zum Rückgängigmachen und [!UICONTROL Strg + Y] zurück.
   >   
   >

1. Klicken **[!UICONTROL Speichern]** in der oberen rechten Ecke des [!UICONTROL Gantt-Diagramm].

## Level-Projektressourcen

Sie können die Aufgabenliste verwenden [!UICONTROL Gantt-Diagramm] , um Ressourcen zu sammeln.

Informationen zur Ressourcenebene finden Sie im Abschnitt [!UICONTROL Gantt-Diagramm], siehe [Level-Ressourcen in [!UICONTROL Gantt-Diagramm]](../../../manage-work/gantt-chart/use-the-gantt-chart/level-resources-in-gantt.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE:&nbsp;this is drafted because I moved the whole content to the article linked above)</p>
<ol>
<li value="1">Go to the project you want to level.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> In the <strong>Tasks</strong> area, click the <strong>Gantt chart</strong> icon.</p> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">All changes are saved automatically when the <strong>Autosave</strong> option is enabled. It is enabled by default. </p> </li>
<li value="3">
<div>
<p data-mc-conditions="QuicksilverOrClassic.Quicksilver">(Optional) Click the <strong>Plan mode</strong> icon and select <strong>Manual save Standard</strong> or <strong>Timeline Planning</strong> to save your changes manually.</p> <note type="tip">
You cannot level resources in the Gantt chart when the Autosave option is enabled.
</note>
<p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <img src="assets/manual-standard-setting-enabled-quicksilver-task-list-350x493.png" style="width: 350;height: 493;"> </p>
</div> </li>
<li value="4"> <p>Click the <strong>Level Resources</strong> drop-down menu.</p> <p> <img src="assets/level-resouces.png" alt="Level_resouces.png"> </p> </li>
<li value="5">Select one of following options:
<ul>
<li><strong>Level Now</strong>: Applies resource leveling to the selected task.</li>
<li><p><strong>Clear Leveling</strong>: Removes all resource leveling from the selected task.</p></li>
</ul><note type="note">
Your resources might be overallocated if they are assigned to multiple tasks which occur during the same time frame.
</note></li>
<li value="6"> <p>(Optional and conditional) If you have disabled the Autosave option, click the <strong>Undo</strong> or<strong>Redo</strong> icons if you want to cancel or duplicate any of the changes. </p> <note type="tip">
<p>You can use the following keyboard shortcuts to undo or redo changes on the Gantt chart:</p>
<ul>
<li>Mac: Use Command + Z to undo and Command + Shift + Z to redo.</li>
<li>Windows: Use Ctrl + Z to undo and Ctrl + Y to redo.</li>
</ul>
</note> </li>
<li value="7">Click <strong>Save</strong> in the upper-right corner of the Gantt chart.</li>
</ol>
</div>
-->

<!--
<h2 data-mc-conditions="QuicksilverOrClassic.Draft mode"> </h2>
-->
