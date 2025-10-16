---
product-area: projects
navigation-topic: use-the-gantt-chart
title: Informationen im Gantt-Diagramm der Aufgabenliste aktualisieren
description: Das Gantt-Diagramm einer Adobe Workfront-Aufgabenliste zeigt Details zu Aufgaben an, die sich in einem Projekt oder einer Vorlage befinden.
author: Alina
feature: Work Management
exl-id: 0a8e6fd5-985c-49e5-842d-67ade29ee1c9
source-git-commit: c8987d036e1c1324618cb53ebcbb8fd7e4bcc6a4
workflow-type: tm+mt
source-wordcount: '1006'
ht-degree: 1%

---

# Informationen in der Aufgabenliste aktualisieren [!UICONTROL Gantt-Diagramm]

<!--Audited: 08/2025-->

Das [!UICONTROL Gantt-] einer Adobe Workfront-Aufgabenliste zeigt Details zu Aufgaben an, die sich in einem Projekt oder einer Vorlage befinden.

In einer Vorlage spiegelt die Aufgabenliste [!UICONTROL Gantt-Diagramm] Aktualisierungen wider, die in der Aufgabenliste der Vorlage auf Vorlagenaufgabenebene vorgenommen wurden. Das mit einer Vorlage verknüpfte [!UICONTROL Gantt-]&quot; kann nicht bearbeitet werden.

In einem Projekt können Sie Aufgabeninformationen direkt in der Aufgabenliste (Gantt[!UICONTROL Diagramm) ].

In diesem Artikel werden die folgenden Aktionen beschrieben, die Sie direkt in der Aufgabenliste ausführen können [!UICONTROL Gantt-Diagramm]:

* Aufgabendauer ändern
* Erstellen oder Entfernen von Vorgängerbeziehungen
* Start- und Enddatum der Aufgabe ändern
* Prozent abgeschlossen aktualisieren
* Projektressourcen abgleichen

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Packstück</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Lizenz</td> 
   <td> <p>[!UICONTROL Standard]</p>
   <p>[!UICONTROL-Plan]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>[!UICONTROL Bearbeiten] Zugriff auf Projekte und Aufgaben</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>[!UICONTROL Manage] Zugriff auf das Projekt und die Aufgaben</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++ 

<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td> <p>[!UICONTROL Plan] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>[!UICONTROL Edit] access to Projects and Tasks</p> <p>Note: If you still don't have access, ask your [!DNL Workfront] administrator if they set additional restrictions in your access level. For information on how a [!DNL Workfront] administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>[!UICONTROL Manage] access to the project and tasks </p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Aufgabendauer ändern

1. Wechseln Sie zu dem Projekt, das Sie ändern möchten.
1. Klicken Sie **[!UICONTROL linken]** auf „Aufgaben“.

   ![Aufgabenbereich](assets/qs-tasks-area-highlighted-in-the-secondary-nav-350x206.png)

1. Klicken Sie auf **[!UICONTROL Symbol]** Gantt-Diagramm“.

   ![Klicken Sie auf das Symbol Gantt-Diagramm ](assets/click-gantt-chart-icon.png)

   Alle Änderungen werden automatisch gespeichert, wenn die Option **[!UICONTROL Automatisches Speichern]** aktiviert ist. Diese ist standardmäßig aktiviert.

1. (Optional) Klicken Sie auf das Symbol **[!UICONTROL Planungsmodus]** und wählen Sie **[!UICONTROL Manuelles Speichern von Standard]** oder **[!UICONTROL Timeline Planning]**, um Ihre Änderungen manuell zu speichern.

   ![Manuelle Einstellung aktiviert](assets/manual-standard-setting-enabled-quicksilver-task-list-350x493.png)

1. Bewegen Sie den Mauszeiger über die Zeitleiste einer Aufgabe und ziehen Sie die Zeitleisten-Anzeige auf ein anderes Datum.
1. Anzeige ignorieren, wenn das richtige neue Abschlussdatum für die Aufgabe erreicht ist.
1. (Optional und bedingt) Wenn Sie ausgewählt haben, dass Ihre Änderungen manuell gespeichert werden sollen, klicken Sie auf die Symbole **[!UICONTROL Rückgängig]** oder&#x200B;**[!UICONTROL Wiederholen]**, wenn Sie Änderungen rückgängig machen oder duplizieren möchten.

   >[!TIP]
   >
   >Mit den folgenden Tastaturbefehlen können Sie Änderungen im Gantt-Diagramm rückgängig machen oder wiederherstellen:
   >
   >   
   >   
   >   * [!DNL Mac]: Verwenden Sie [!UICONTROL Befehl + Z], um den Vorgang rückgängig zu machen, und [!UICONTROL Befehl + Umschalt + Z], um ihn wiederherzustellen.
   >   * [!DNL Windows]: Verwenden Sie [!UICONTROL Strg + Z], um dies rückgängig zu machen, und [!UICONTROL Strg + Y], um es wiederherzustellen.
   >   
   >

1. Klicken **[!UICONTROL oben rechts]** &quot;[!UICONTROL &quot; auf „Speichern].

## Erstellen oder Entfernen von Vorgängerbeziehungen

1. Wechseln Sie zu dem Projekt, das Sie ändern möchten.
1. Klicken Sie im Bereich **[!UICONTROL Aufgaben]** auf das Symbol **[!UICONTROL Gantt-Diagramm]**.

   Die **[!UICONTROL AutoSpeichern]**-Option ist standardmäßig ausgewählt. In diesem Fall werden alle Änderungen automatisch gespeichert.

   ![Klicken Sie auf das Symbol Gantt-Diagramm ](assets/click-gantt-chart-icon.png)

1. (Optional) Klicken Sie auf das Symbol **[!UICONTROL Planungsmodus]** und wählen Sie **[!UICONTROL Manuelles Speichern von Standard]** oder **[!UICONTROL Timeline Planning]**, um Ihre Änderungen manuell zu speichern.

   ![Manuelle Einstellung aktiviert](assets/manual-standard-setting-enabled-quicksilver-task-list-350x493.png)

1. Um eine Vorgängerbeziehung zu erstellen, klicken Sie auf den Startpunkt einer Aufgabe und ziehen Sie sie an den Endpunkt der Aufgabe.
1. Um eine Vorgängerbeziehung zu löschen, klicken Sie auf eine Vorgängerzeile, die zwei Aufgaben verbindet, um sie auszuwählen, und drücken Sie dann **[!UICONTROL Löschen]** auf Ihrer Tastatur.\
   ![delete_precessor.png](assets/delete-predecessor-350x152.png)

1. (Optional und bedingt) Wenn Sie ausgewählt haben, dass die Änderungen manuell gespeichert werden sollen, klicken Sie auf **[!UICONTROL Rückgängig]** oder&#x200B;**[!UICONTROL Wiederholen]**, um Änderungen rückgängig zu machen oder zu duplizieren.

   >[!TIP]
   >
   >Mit den folgenden Tastaturbefehlen können Sie Änderungen im Gantt-Diagramm rückgängig machen oder wiederherstellen:
   >
   >   
   >   
   >   * [!DNL Mac]: Verwenden Sie [!UICONTROL Befehl + Z], um den Vorgang rückgängig zu machen, und [!UICONTROL Befehl + Umschalt + Z], um ihn wiederherzustellen.
   >   * [!DNL Windows]: [!UICONTROL Verwenden Sie Strg+Z], um dies rückgängig zu machen, und [!UICONTROL Strg+Y], um es wiederherzustellen.
   >   
   >

1. Klicken Sie **[!UICONTROL Speichern]** .

## Start- und Enddatum der Aufgabe ändern

1. Wechseln Sie zu dem Projekt, das Sie ändern möchten.
1. Klicken Sie im Bereich **[!UICONTROL Aufgaben]** auf das Symbol **[!UICONTROL Gantt-Diagramm]**.

   Alle Änderungen werden automatisch gespeichert, wenn die Option **[!UICONTROL Automatisches Speichern]** aktiviert ist. Diese ist standardmäßig aktiviert.

   ![Klicken Sie auf das Symbol Gantt-Diagramm ](assets/click-gantt-chart-icon.png)

1. (Optional) Klicken Sie auf das Symbol **[!UICONTROL Planungsmodus]** und wählen Sie **[!UICONTROL Manuelles Speichern von Standard]** oder **[!UICONTROL Timeline Planning]**, um Ihre Änderungen manuell zu speichern.

   ![Manuelle Einstellung aktiviert](assets/manual-standard-setting-enabled-quicksilver-task-list-350x493.png)

1. Bewegen Sie den Mauszeiger über die Mitte der Aufgabe und suchen Sie den multidirektionalen Pfeil.
1. Klicken und ziehen Sie die Aufgabe auf das gewünschte Datum.

   ![change_start_end_date.png](assets/change-start-end-date.png)

1. Wenn Sie das Aufgabendatum in einer Weise ändern, die sich auf die Aufgabenbeschränkung auswirkt, klicken Sie auf **[!UICONTROL Akzeptieren]**, um die Änderung der Aufgabenbeschränkung zu bestätigen.

   >[!NOTE]
   >
   >Wenn die Aufgabe eine der folgenden Einschränkungen aufweist, aktualisiert das System die [!UICONTROL Aufgabenbeschränkung] auf [!UICONTROL Start nicht früher] als, wenn das Projekt ab dem [!UICONTROL Startdatum] oder [!UICONTROL Ende nicht später als] geplant ist, wenn das Projekt am [!UICONTROL Abschlussdatum]:
   >
   >   
   >   
   >   * [!UICONTROL So bald wie möglich]
   >   * [!UICONTROL So spät wie möglich]
   >   * [!UICONTROL Früheste verfügbare Zeit]
   >   * [!UICONTROL Letzte verfügbare Zeit]
   >   
   >   
   >In einigen Fällen verhindern die Vorgängerbeziehungen möglicherweise, dass die Aufgaben früher beginnen, und das Verschieben der Aufgabe ist nicht zulässig.

1. (Optional und bedingt) Wenn Sie ausgewählt haben, dass die Änderungen manuell gespeichert werden sollen, klicken Sie auf die Symbole **[!UICONTROL Rückgängig]** oder&#x200B;**[!UICONTROL Wiederholen]**, um Änderungen rückgängig zu machen oder zu duplizieren.

   >[!TIP]
   >
   >Sie können die folgenden Tastaturbefehle verwenden, um Änderungen im [!UICONTROL Gantt-Diagramm“ rückgängig zu machen oder ]:
   >
   >   
   >   
   >   * [!DNL Mac]: Verwenden Sie [!UICONTROL Befehl + Z], um den Vorgang rückgängig zu machen, und [!UICONTROL Befehl + Umschalt + Z], um ihn wiederherzustellen.
   >   * [!DNL Windows]: Verwenden Sie [!UICONTROL Strg + Z], um dies rückgängig zu machen, und [!UICONTROL Strg + Y], um es wiederherzustellen.
   >   
   >

1. Klicken Sie auf **[!UICONTROL Speichern]**.

## Prozent abgeschlossen aktualisieren

1. Wechseln Sie zu dem Projekt, das Sie ändern möchten.
1. Klicken Sie im Bereich **[!UICONTROL Aufgaben]** auf das Symbol **[!UICONTROL Gantt-Diagramm]**.

   ![Klicken Sie auf das Symbol Gantt-Diagramm ](assets/click-gantt-chart-icon.png)

   Alle Änderungen werden automatisch gespeichert, wenn die Option **[!UICONTROL Automatisches Speichern]** aktiviert ist. Diese ist standardmäßig aktiviert.

1. (Optional) Klicken Sie auf das Symbol **[!UICONTROL Planungsmodus]** und wählen Sie **[!UICONTROL Manuelles Speichern von Standard]** oder **[!UICONTROL Timeline Planning]**, um Ihre Änderungen manuell zu speichern.
1. Doppelklicken Sie in der Aufgabe auf die Prozentzahl und geben Sie die Zahl ein.

   >[!IMPORTANT]
   >
   >Sie müssen [!UICONTROL % abgeschlossen] im Dialogfeld [!UICONTROL Optionen] ausgewählt haben, um den Prozentsatz der Fertigstellung zu aktualisieren. Klicken Sie dazu auf das Symbol **[!UICONTROL Optionen]** und wählen Sie **[!UICONTROL % Abgeschlossen]**.
   >
   >
   >![update_percent_complete.png](assets/update-percent-complete-350x175.png)   >
   >

1. (Optional und bedingt) Wenn Sie ausgewählt haben, dass die Änderungen manuell gespeichert werden sollen, klicken Sie auf **[!UICONTROL Rückgängig]** oder&#x200B;**[!UICONTROL Wiederholen]**, um Änderungen rückgängig zu machen oder zu duplizieren.

   >[!TIP]
   >
   >Sie können die folgenden Tastaturbefehle verwenden, um Änderungen im [!UICONTROL Gantt-Diagramm“ rückgängig zu machen oder ]:
   >
   >   
   >   
   >   * [!DNL Mac]: Verwenden Sie [!UICONTROL Befehl + Z], um den Vorgang rückgängig zu machen, und [!UICONTROL Befehl + Umschalt + Z], um ihn wiederherzustellen.
   >   * [!DNL Windows]: Verwenden Sie [!UICONTROL Strg + Z], um dies rückgängig zu machen, und [!UICONTROL Strg + Y], um es wiederherzustellen.
   >   
   >

1. Klicken **[!UICONTROL oben rechts]** &quot;[!UICONTROL &quot; auf „Speichern].

## Projektressourcen abgleichen

Sie können die Aufgabenliste (Gantt[!UICONTROL Diagramm) verwenden] um Ihre Ressourcen abzugleichen.

Informationen zu Abgleichressourcen im [!UICONTROL Gantt-Diagramm] finden Sie unter [Abgleichressourcen im [!UICONTROL Gantt-Diagramm]](../../../manage-work/gantt-chart/use-the-gantt-chart/level-resources-in-gantt.md).

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
