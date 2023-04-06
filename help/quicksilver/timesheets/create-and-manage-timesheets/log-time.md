---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: Protokollzeit
description: Sie können die Zeit für Arbeitselemente in&nbsp;Adobe Workfront protokollieren, um die Anzahl der Arbeitsstunden anzugeben, die Sie damit verbringen. Sie können auch Zeit protokollieren, die nicht mit der Arbeit in Zusammenhang steht, wie Urlaub, Krankheitszeit oder Zeit, die Sie in Meetings verbringen. Die Login-Zeit wird in Ihrem Timesheet angezeigt.
author: Alina
feature: Timesheets
exl-id: 120173a8-95f1-4233-ab40-d3bcfe38c977
source-git-commit: 27e9cfff363ab38c6469b99a8cbb04439f2df61c
workflow-type: tm+mt
source-wordcount: '2979'
ht-degree: 0%

---

# Protokollzeit

Sie können die Arbeitszeit für Arbeitselemente in Adobe Workfront protokollieren, um die Anzahl der Arbeitsstunden anzugeben, die Sie damit verbringen. Sie können auch Zeit protokollieren, die nicht mit der Arbeit in Zusammenhang steht, wie Urlaub, Krankheitszeit oder Zeit, die Sie in Meetings verbringen. Die Login-Zeit wird in Ihrem Timesheet angezeigt.

Weitere Informationen zu den Stunden, die Sie in Workfront anmelden können, finden Sie unter [Stundentypen verwalten](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/hour-types.md).

## Zugriffsanforderungen

<!--drafted for P&P - replace the table:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Light or higher</p>
   <p>Legacy license: 
   <ul><li>Review or higher to log General Hours in a timesheet</li>
   <li>Work or higher to log hours on a project, task, or issue</li></ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to the type of work item you log time for </p> <p>For example, you need Edit access to Issues, to log time for issues</p> <p>If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Contribute or higher permissions on the work item you log time for that includes permissions to Log Hours</p> <p>For information on requesting additional access, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel auszuführen und projektspezifische Stunden zu protokollieren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <ul><li>Überprüfen oder höher zur Protokollierung der allgemeinen Stunden in einem Zeitblatt</li>
   <li> Arbeiten oder höher zur Protokollierung von Stunden in einem Projekt, einer Aufgabe oder einem Problem</li></ul>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Bearbeiten Sie den Zugriff auf den Typ des Arbeitselements, für den Sie die Zeit protokollieren </p> <p>Beispielsweise benötigen Sie Zugriff auf Probleme bearbeiten, um die Zeit für Probleme zu protokollieren.</p> <p>Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Tragen Sie die Berechtigungen für das Arbeitselement, für das Sie die Zeit protokollieren, bei oder höher ein, einschließlich der Berechtigungen für "Log Hours".</p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Überlegungen zur Protokollierung in Workfront

* Sie können die Zeit für Projekte, Aufgaben oder Probleme protokollieren oder die Zeit direkt in Ihrem Timesheet protokollieren.

   Informationen zum Erstellen von Timesheets finden Sie unter [Erstellen eines Datenblatts für die einmalige Verwendung](../../timesheets/create-and-manage-timesheets/create-tmshts.md).

* Alle Zeitangaben, die mit anderen Werkzeugen als dem Timesheet protokolliert werden, werden im Zeitblatt für den entsprechenden Zeitraum angezeigt.
* Aufgaben und Probleme in einem nicht aktuellen Projekt werden nicht vorab in ein Timesheet eingefügt.
* Die im Timesheet protokollierte Zeit wird sofort auf die Aufgabe, das Problem oder das Projekt angewendet.
* Timesheets enthalten die Gesamtdauer für alle protokollierten Daten. Wochenenden sind immer enthalten, auch wenn Zeitleistenberechnungen so konfiguriert wurden, dass sie sie ausschließen (wie beschrieben in [Systemweite Projektvoreinstellungen konfigurieren](../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)).
* Die maximale Anzahl der in einem Zeitblatt angezeigten Elemente beträgt 45. Wenn mehr als 45 Elemente vorhanden sind, deren Daten mit dem Zeitrahmen des Zeitblatts übereinstimmen, werden nur die zuletzt aktualisierten Elemente angezeigt.
* Stündliche Einträge, die in abgerechneten Rechnungsdatensätzen enthalten sind, werden abgeblendet dargestellt und können nicht im Timesheet bearbeitet werden. Weitere Informationen finden Sie unter [Rechnungsdatensätze erstellen](../../manage-work/projects/project-finances/create-billing-records.md).

## Protokollzeit

Sie können die Zeit in den folgenden Bereichen in Workfront protokollieren:

* [Arbeitszeittabelle](#timesheet)
* [Startseite](#home)
* [Projekt, Aufgabe oder Problem](#project-task-or-issue)
* [Zusammenfassungsbereich](#summary-panel)
* [Pinnwände](#boards)
* [Mobile App](#mobile-app)

### Arbeitszeittabelle {#timesheet}

Sie können allgemeine Stunden oder projektspezifische Stunden auf einem Timesheet protokollieren.

>[!NOTE]
>
>Überprüfungsbenutzer, die einem Timesheet-Profil zugewiesen sind, können die Registerkarte &quot;Timesheets&quot;sehen und allgemeine Stunden protokollieren. Sie können jedoch keine Stunden für Aufgaben oder Probleme protokollieren, die ihnen auf dem Timesheet zugewiesen werden.

1. Klicken Sie auf [!UICONTROL **Hauptmenü**] icon ![](assets/main-menu-icon.png) in der rechten oberen Ecke von Adobe Workfront.

1. Klicken [!UICONTROL **Timesheets**]. Ihr aktuelles Timesheet wird standardmäßig angezeigt.
   ![Arbeitszeittabelle](assets/timesheet-redesigned-nwe.png)

   Das Timesheet wird vorab mit Elementen ausgefüllt, die Ihnen während des Zeitrahmens des Zeitblatts zugewiesen wurden. Informationen dazu, wie Timesheets vorausgefüllt werden, finden Sie unter [Zeitblatt- und Stundenvoreinstellungen konfigurieren](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md). Wenn Sie kein Element auf dem Timesheet sehen, können Sie es hinzufügen.

   >[!NOTE]
   >
   >Das Timesheet wird nur mit den Ihnen zugewiesenen Elementen vorausgefüllt. Es werden keine Elemente eingefügt, die Ihren Teams oder Ihren Jobrollen zugewiesen sind.
   >
   >Wenn Sie auf Bearbeiten für ein Ihrer Teams zugewiesenes Element klicken, wird das Element Ihnen zugewiesen und das Element wird in Ihrem Zeitblatt angezeigt.


1. (Optional) Klicken Sie auf die **Vollbild** icon ![](assets/full-screen.png) um das Timesheet im Vollbildmodus anzuzeigen, klicken Sie auf **exit-full-screen** ![](assets/exit-full-screen.png) -Symbol, um zum Timesheet zurückzukehren.

   <!-- drafted for the resize columns in timesheet story: 1. (optional) Click on the separator lines between weeks or between the time frame area and the work item area to resize the columns of the timesheet.-->

1. (Optional) Klicken Sie auf das Symbol **Element hinzufügen** Dropdown-Menü in der oberen linken Ecke des Zeitplans und klicken Sie auf **Projekte hinzufügen**, **Aufgaben hinzufügen** oder **Hinzufügen von Problemen**.

   Eine Liste mit Projekten, Aufgaben oder Problemen wird angezeigt.

   <!--drafted for full screen mode for add projects story - align it with the rest of the steps when you enable this:: 1. (Optional) Click the **full-screen** icon ![](assets/full-screen.png) to display the list of objects in full-screen mode.-->

1. (Optional) Klicken Sie auf das Suchsymbol ![Nach einem Element suchen](assets/search-icon.png) , um mithilfe eines Suchbegriffs, der zum Datenblatt hinzugefügt wird, nach einem bestimmten Element zu suchen.

1. (Optional) Erweitern Sie die Dropdown-Menüs Filter, Ansicht oder Gruppierung, um sie anzuwenden oder anzupassen und um die gewünschten Elementinformationen anzuzeigen.

1. Wählen Sie ein oder mehrere Elemente in der Liste aus und klicken Sie auf **Hinzufügen**.

   >[!NOTE]
   >
   >Wenn Sie Aufgaben oder Probleme zum Timesheet hinzufügen, wird das Projekt ebenfalls hinzugefügt.


1. (Bedingt) Wenn Sie 50 oder mehr Elemente gleichzeitig hinzufügen, wird eine Bestätigungsmeldung angezeigt, die die Anzahl der zu Ihrem Zeitblatt hinzugefügten Elemente anzeigt.

   Klicken **Alle hinzufügen** um alle Elemente hinzuzufügen, oder klicken Sie auf **Abbrechen** , um das Hinzufügen der ausgewählten Elemente zu beenden, und **Abbrechen** , um die Liste der Elemente zu schließen.

   Aufgaben und Probleme werden unter dem Namen des Projekts aufgelistet.

   >[!NOTE]
   >
   >Die Elemente, die Sie manuell zum Timesheet hinzufügen, werden fixiert und bleiben auf den aktuellen und zukünftigen Timesheets erhalten, bis Sie sie manuell entschlüsseln, um sie zu entfernen. Informationen zum Entschlüsseln von Elementen, um sie aus dem Timesheet zu entfernen, finden Sie in Schritt 10.

   <!--(ensure this stays accurate)-->

1. (Optional) Klicken Sie auf die **Reduzieren** ![](assets/collapse-icon.png) oder **Erweitern** ![](assets/expand-icon.png) Symbole neben dem Projektnamen zum Anzeigen oder Ausblenden der Liste der Aufgaben und Probleme für das Projekt.


   >[!TIP]
   >
   >   Drücken Sie bei Verwendung einer standardmäßigen QWERTY-Tastatur und nach dem Klicken auf den Namen eines Projekts im Timesheet die folgenden Tasten, um das Projekt zu reduzieren oder zu erweitern:
   >   * So erweitern Sie das Projekt und zeigen seine Arbeitselemente an:
      >     * Umschalttaste + Alt + Nach-oben-Taste für Windows-Computer
      >     * Umschalttaste + Wahltaste + Nach-oben-Taste für Mac-Computer
   >   * So reduzieren Sie das Projekt und blenden seine Arbeitselemente aus:
      >     * Umschalt + Alt + Abwärtspfeil für Windows-Computer
      >     * Umschalttaste + Wahltaste + Abwärtspfeil für Mac-Computer.



1. (Optional) Wenn Sie ein Element, das automatisch auf dem Timesheet angezeigt wird, manuell veröffentlichen möchten, halten Sie den Mauszeiger über den Namen des Elements und klicken Sie auf **pin** icon ![](assets/empty-pin-icon.png).

   >[!TIP]
   >
   >   Drücken Sie bei Verwendung einer standardmäßigen QWERTY-Tastatur nach dem Klicken auf ein Element im Zeitblatt den folgenden Tastensatz, um ein Element anzuheften:
   >   * Option + P für Windows- und Mac-Computer.



1. (Optional) Klicken Sie auf das Suchsymbol ![](assets/search-icon.png) und beginnen Sie mit der Eingabe eines Suchbegriffs, um ein Projekt, eine Aufgabe oder ein Problem auf dem Timesheet zu finden.

1. (Optional) Sie können ein Element (Projekt, Aufgabe oder Problem) aus dem Timesheet entfernen, wenn Sie das Element manuell hinzugefügt haben (wie in den Schritten 3-6 beschrieben) und wenn Sie die Zeit noch nicht damit verrechnet haben, indem Sie es entsperrt haben. <!--ensure this stays accurate-->

   Es ist nicht möglich, im Timesheet enthaltene Elemente automatisch entsprechend den Timesheet-Voreinstellungen in Ihrem Workfront-System oder Ihrer-Gruppe zu entfernen, die für das Vorausfüllen der Timesheets konfiguriert sind (siehe [Zeitblatt- und Stundenvoreinstellungen konfigurieren](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

   So entfernen Sie ein manuell hinzugefügtes Element aus dem Timesheet:

   1. Stellen Sie sicher, dass keine Zeit für das Element protokolliert wird.
   1. Klicken Sie auf **unpin** icon ![Element fixieren](assets/pin-icon.png) neben dem Element, um die Bindung des Elements aus dem Datenblatt aufzuheben.

   >[!TIP]
   >
   >   Drücken Sie bei Verwendung einer standardmäßigen QWERTY-Tastatur nach dem Klicken auf ein Element im Timesheet die folgenden Tasten, um die Bindung eines Elements aufzuheben:
   >   * Option + P für Windows- und Mac-Computer.



   Das Element wird aus dem Timesheet entfernt, nachdem Sie die Seite aktualisiert haben.

1. (Bedingt) Wenn Ihr Workfront- oder Gruppenadministrator die Funktion **Manuelles Zuweisen von Auftragsrollen zu Stundeneinträgen** festlegen, wählen Sie im Dropdown-Menü eine Auftragsrolle aus. Die Rolle, die beim Zuweisen zum Arbeitselement angegeben wird, wird standardmäßig angezeigt. Wenn Ihnen keine Rolle für das Objekt zugewiesen wurde, wird Ihre Primäre Rolle als Standard angezeigt. Weitere Informationen zu dieser Einstellung finden Sie im Artikel [Zeitblatt- und Stundenvoreinstellungen konfigurieren](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

   ![Protokollzeit für mehrere Rollen im Timesheet](assets/job-role-plus-sign-and-boxes-in-redesigned-timesheet.png)


1. (Optional) Klicken Sie auf die **+** Symbol, um eine weitere Zeile hinzuzufügen, und wählen Sie dann aus dem Dropdown-Menü im [!UICONTROL Stündentyp] Spalte, um die Zeit für einen anderen Stundentyp zu protokollieren.

   ![Dropdown-Menü &quot;Stündentyp&quot;](assets/hour-type-drop-down-expanded-redesigned-timesheet.png)

   >[!TIP]
   >
   >   Drücken Sie je nach Betriebssystem oder Browser und bei Verwendung einer standardmäßigen QWERTY-Tastatur den folgenden Tastensatz, um eine weitere Zeile hinzuzufügen:
   >   * Strg + Wahltaste + + + für Windows-Computer
   >   * Befehl + Wahltaste + + für Mac-Computer


   Je nachdem, was auf System-, Projekt- und Benutzerebene definiert wurde, sind die Stunden-Typen verfügbar, wie unter [Festlegen von Stundentypen und Verfügbarkeit für Timesheets](define-hour-types-and-availability.md).

   Der Stundentyp kann nach dem Schließen eines Zeitblatts nicht mehr geändert werden.

   >[!TIP]
   >
   >Wenn Sie zuvor die Zeit protokolliert haben und der von Ihnen ausgewählte Stundentyp jetzt deaktiviert ist, wird die gesamte Zeile für die protokollierte Zeit abgeblendet angezeigt. Wenn Sie einen anderen Stundentyp auswählen und die Seite aktualisieren, wird die Option für den deaktivierten Stundentyp aus der Dropdownliste entfernt, sodass Sie diesem Stundentyp keine zusätzlichen Stunden hinzufügen können.
   >
   >Erwägen Sie, eine neue Zeile für das Arbeitselement hinzuzufügen, für das Sie zusätzliche Zeit protokollieren möchten, und einen neuen Stundentyp auszuwählen, wenn Sie den deaktivierten Stundentyp beibehalten möchten, der mit der letzten protokollierten Zeit verknüpft ist.

1. Klicken Sie auf **delete** icon  ![](assets/delete.png) neben der Rolle &quot;Job&quot;klicken, um sie zu entfernen. Jede für die Rolle protokollierte Zeit wird ebenfalls entfernt.

   >[!TIP]
   >
   >   Drücken Sie je nach Betriebssystem oder Browser und bei Verwendung einer standardmäßigen QWERTY-Tastatur den folgenden Tastensatz, um eine Zeile zu löschen:
   >   * Strg + Wahltaste + - für Windows-Computer
   >   * Befehl + Wahltaste + - für Mac-Computer



1. Geben Sie im Zeitleistensegment-Bereich des Zeitplans an, wie lange Sie sich an einem bestimmten Tag anmelden möchten, und klicken Sie dann außerhalb des Stundenfelds, um den Stundeneintrag zu speichern. Die Stunden werden automatisch gespeichert. Die Zeile, für die Sie die Protokollzeit festlegen, wird hellblau hervorgehoben und das Feld für die Stundeneingabe ist dunkelblau dargestellt.

   ![Zeitfeld des Protokolls in einem Zeitblatt](assets/log-time-with-blue-hightlight-redesigned-timesheet.png)

   Sie melden die Zeit entweder in Stunden oder Tagen an. Diese Einstellung wird von Benutzern mit einer Planungslizenz oder vom Systemadministrator konfiguriert, wie unter [Konfigurieren, ob die Zeit in Stunden oder Tagen protokolliert wird](../../timesheets/config-timesheet-prefs/config-time-logged-hrs-days.md).

   >[!IMPORTANT]
   >
   >Wenn sich die Rolle des Auftrags, für den Sie die Zeit protokolliert haben, geändert hat und die **Manuelles Zuweisen von Auftragsrollen zu Stundeneinträgen** deaktiviert wurde, müssen Sie Ihre Zeiteinträge manuell speichern. Das Timesheet speichert Ihre Zeit nur dann automatisch, wenn keine Zeit mehr für die geänderte Auftragsrolle protokolliert wird.
   >
   >Wenn sich die Rolle geändert hat und die **Manuelles Zuweisen von Auftragsrollen zu Stundeneinträgen** aktiviert ist, können Sie die Zeit protokollieren oder die Rolle aktualisieren. Ihre Änderungen werden automatisch gespeichert.

1. (Optional) Geben Sie die Zeitdauer im Feld Überstunden in der Kopfzeile des Zeitblatts an.

   >[!TIP]
   >
   >Es ist nicht möglich, eine größere Anzahl von Überstunden als die aktuellen Gesamtstunden auf dem Zeitblatt zu protokollieren. Wenn Sie beispielsweise bisher 7 Stunden auf dem Timesheet angemeldet haben, können Sie keine 8 Stunden Überstunden protokollieren.

1. (Optional) Klicken Sie auf **Kommentar** , um einen Kommentar für Ihren Stundeneintrag hinzuzufügen.

   ![](assets/commment-button-on-hour-log-redesigned-timesheet.png)

   >[!TIP]
   >
   >   Wenn Sie eine standardmäßige QWERTY-Tastatur verwenden, nachdem Sie auf das Stundeneingabefeld geklickt haben, drücken Sie die folgenden Tasten, um das Kommentarfeld zu öffnen:
   >   * Umschalt + F2 für Windows- und Mac-Computer.


1. Klicken **Fertig** , um den Kommentar zu speichern.

   >[!TIP]
   >
   >   Wenn Sie eine standardmäßige QWERTY-Tastatur verwenden, drücken Sie innerhalb des Kommentarfelds die folgenden Tasten, um den Kommentar zu speichern:
   >   * Strg + Eingabetaste für Windows-Computer.
   >   * Befehl + Rückgabe für Mac-Computer.



1. (Optional) Klicken Sie auf **Kommentare anzeigen** in der Symbolleiste, um Kommentare zu Stundeneinträgen unter dem Arbeitselement anzuzeigen.

   ![Anmerkungen, die unter dem Punkt &quot;Zeitblatt&quot;aufgeführt sind](assets/comments-expanded-under-tasks-redesigned-timesheet.png)

   >[!TIP]
   >
   >   Alle Änderungen, die Sie am Timesheet vornehmen, werden automatisch gespeichert.

1. (Optional) Klicken Sie auf die Zeile einer Aufgabe oder eines Problems und dann auf **Zusammenfassung öffnen** in der oberen rechten Ecke des Zeitblatts, um ein Update hinzuzufügen oder Informationen über die Aufgabe oder das Problem zu aktualisieren. Das Bedienfeld &quot;Zusammenfassung&quot;wird rechts geöffnet.

   ![summary-panel-for-task-opened-in-timesheet](assets/summary-panel-for-task-opened-in-timesheet-redesigned-timesheet.png)

   Ihre Aktualisierung wird im Bereich Updates des Arbeitselements angezeigt, das der protokollierten Zeit zugeordnet ist.

   >[!TIP]
   >
   >Sie können keine Kommentare zu Projekten oder Einträgen zur allgemeinen Zeit erstellen.

1. Klicken [!UICONTROL **Zusammenfassung schließen**] , um das Bedienfeld Zusammenfassung zu schließen und zum Timesheet zurückzukehren.

1. (Optional) Klicken Sie auf [!UICONTROL **Updates**] Fügen Sie im linken Bereich ein Update zum Timesheet hinzu. Weitere Informationen zu Workfront-Aktualisierungen finden Sie unter [Update der Arbeit](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

   ![enter-an-update-in-redesign-timesheet-left-panel](assets/enter-an-update-in-redesigned-timesheet-left-panel.png)

   * **Schließen**: Schließen Sie das Timesheet nach der Aktualisierung. Diese Option ist nur verfügbar, wenn Ihr Timesheet keinem Genehmiger zugeordnet ist.

   * **Zur Genehmigung einreichen:** Diese Option ist nur verfügbar, wenn ein Genehmiger auf dem Timesheet vorhanden ist. Speichern Sie Ihre Änderungen und übermitteln Sie sie zur Genehmigung. Sie können das Timesheet öffnen, nachdem Sie es geschlossen haben, indem Sie auf **Rückruf**, wenn noch keine Genehmigung erteilt wurde. Weitere Informationen finden Sie unter [Zeitblatt zur Genehmigung einreichen](../../timesheets/create-and-manage-timesheets/submit-timesheet-for-approval.md).

   * **Ablehnen**: Diese Option wird angezeigt, wenn Sie Timesheet-Genehmiger sind und das Timesheet zur Genehmigung übermittelt wurde. Wenn Sie darauf klicken, wird der Status des Zeitblatts in Abgelehnt geändert und das Zeitblatt bleibt geöffnet.

   * **Genehmigen**: Diese Option wird angezeigt, wenn Sie Timesheet-Genehmiger sind und das Timesheet zur Genehmigung übermittelt wurde. Wenn Sie darauf klicken, ändert sich der Status des Timesheets in Genehmigt und das Timesheet wird geschlossen.
   >[!TIP]
   >
   >Die Optionen Ablehnen und Genehmigen werden auch dann auf Ihrem Timesheet angezeigt, wenn Sie Systemadministrator sind und das Timesheet mit einem Genehmiger verknüpft ist.

1. (Bedingt) Wenn Sie das Datenblatt geschlossen oder zur Genehmigung eingereicht haben, wählen Sie eine der folgenden Optionen aus:

   * **Neu öffnen**: Diese Option ist für Timesheets verfügbar, die Sie bereits geschlossen haben und die keine Genehmiger oder Timesheets haben, die bereits genehmigt wurden. Öffnen Sie das Timesheet erneut, um die Stundeneinträge zu ändern.
   * **Rückruf**: Diese Option steht für Timesheets zur Verfügung, die zur Genehmigung eingereicht, aber noch nicht genehmigt oder abgelehnt wurden. Klicken **Rückruf** , um das Timesheet erneut zu öffnen und die Stundeneinträge zu ändern.

### Startseite {#home}

Sie können projektspezifische Zeit auf der Startseite protokollieren.

Allgemeine Informationen zur Verwendung des Startbereichs finden Sie unter [Verwenden des Startbereichs](../../workfront-basics/using-home/using-the-home-area/use-the-home-area.md).

So protokollieren Sie die Zeit eines Arbeitselements im Bereich &quot;Startseite&quot;:

1. Im **Arbeitsliste** Bereich, wählen Sie das Element aus, in dem Sie die Zeit protokollieren möchten.
1. Klicken Sie im rechten Bereich auf **Protokollzeit**.

   ![](assets/log-time-home-350x181.png)

1. Im **Stunden eingeben** aus dem Dropdown-Menü den entsprechenden Stundentyp auswählen.\
   Je nachdem, was auf System-, Projekt- und Benutzerebene definiert wurde, sind die Stunden-Typen verfügbar, wie unter [Festlegen von Stundentypen und Verfügbarkeit für Timesheets](../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md).
1. (Bedingt) Wenn Ihr Workfront- oder Gruppenadministrator die Funktion **Manuelles Zuweisen von Auftragsrollen zu Stundeneinträgen** festlegen, wählen Sie im Dropdown-Menü eine Auftragsrolle aus. Die Rolle, die beim Zuweisen zum Arbeitselement angegeben wird, wird standardmäßig angezeigt. Wenn Ihnen keine Rolle für das Objekt zugewiesen wurde, wird Ihre Primäre Rolle als Standard angezeigt. Weitere Informationen zu dieser Einstellung finden Sie im Artikel [Zeitblatt- und Stundenvoreinstellungen konfigurieren](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).
1. Geben Sie die Zeit für die Protokollierung an und klicken Sie auf **Protokollzeit**.

### Projekt, Aufgabe oder Problem {#project-task-or-issue}

Sie können projektspezifische Zeit für ein Projekt, eine Aufgabe oder ein Problem protokollieren.

#### Für die Protokollierungszeit erforderliche Berechtigungen

Um Stunden für ein Projekt, eine Aufgabe oder ein Problem protokollieren zu können, benötigen Sie bestimmte Berechtigungen. Sie können die Zeit an zwei Stellen in einem Projekt, einer Aufgabe oder einem Problem protokollieren:

* [Registerkarte Updates](#updates-tab)
* [Registerkarte &quot;Stunden&quot;](#hours-tab)

##### Registerkarte Updates{#updates-tab}

Die folgenden Voraussetzungen müssen erfüllt sein, bevor Sie Stunden auf der Registerkarte Aktualisierungen eines Projekts, einer Aufgabe oder eines Problems protokollieren können:

* Sie müssen über eine Arbeits- oder Planungslizenz verfügen.
* Sie müssen mindestens über Beitragsberechtigungen für das Projekt, die Aufgabe oder das Problem mit Zugriff auf Protokollzeiten verfügen.\
   Weitere Informationen zum Gewähren von Berechtigungen für Projekte finden Sie unter [Freigeben eines Projekts in Adobe Workfront](../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).

* Wenn Sie die Zeit direkt in einem Projekt protokollieren möchten, muss Ihr Workfront-Administrator die Protokollzeit direkt für Projekte aktivieren, die unter [!UICONTROL **Datenblatt und Stunden** ]> [!UICONTROL **Voreinstellungen**].\
   Weitere Informationen dazu, wie Sie Benutzern erlauben, Stunden direkt in Projekten zu protokollieren, finden Sie unter [Zeitblatt- und Stundenvoreinstellungen konfigurieren](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

##### Registerkarte &quot;Stunden&quot;{#hours-tab}

Die folgenden Voraussetzungen müssen erfüllt sein, bevor Sie Stunden auf der Registerkarte Stunden eines Projekts, einer Aufgabe oder eines Problems protokollieren können:

* Sie müssen Systemadministrator sein.

Oder Sie müssen über Folgendes verfügen:

* Sie müssen über eine Planungslizenz mit Administratorzugriff auf Timesheets und Stunden verfügen. Weitere Informationen zum Gewähren des administrativen Zugriffs auf Timesheets und Stunden finden Sie unter [Benutzern administrativen Zugriff auf bestimmte Bereiche gewähren](../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).
* Sie müssen mindestens über Beitragsberechtigungen für das Projekt mit Zugriff auf &quot;Log Hours&quot;verfügen. Weitere Informationen zum Gewähren von Berechtigungen für Projekte finden Sie unter [Freigeben eines Projekts in Adobe Workfront](../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).
* Wenn Sie die Zeit direkt in einem Projekt protokollieren möchten, muss Ihr Workfront-Administrator die Einstellung Zeitpunkt der Projektprotokollierung unter &quot;Timesheet &amp; Hours > Voreinstellungen&quot;aktivieren. Weitere Informationen dazu, wie Sie Benutzern erlauben, Stunden direkt in Projekten zu protokollieren, finden Sie unter [Zeitblatt- und Stundenvoreinstellungen konfigurieren](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

So protokollieren Sie die Zeit eines Projekts, einer Aufgabe oder eines Problems:

1. Navigieren Sie zu einem Projekt, einer Aufgabe oder einem Problem.
1. Wählen Sie im linken Bereich die Option **Stunden**.
1. Klicken **Protokollzeit**.

   Das Dialogfeld Protokollzeiten wird angezeigt.

1. Geben Sie die folgenden Informationen an:

   * **Inhaber:** Ihr Name wird standardmäßig in diesem Feld angezeigt.\
      Wenn Sie die Stunden für einen anderen Benutzer protokollieren, geben Sie dessen Namen an.

   * **Stunden**: Geben Sie die Anzahl der Stunden für das Projekt, die Aufgabe oder das Problem ein.
   * **Stündentyp**: Wählen Sie im Dropdown-Menü einen Stündentyp aus, wenn dieser von dem standardmäßig angezeigten unterscheidet.

      Je nachdem, welche Stundentypen in Ihrem System konfiguriert sind, können die Optionen hier variieren. Weitere Informationen zum Konfigurieren von Stundentypen finden Sie unter [Festlegen von Stundentypen und Verfügbarkeit für Timesheets](../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md).

   * **Auftragsrolle**: (Bedingt) Wenn Ihr Workfront- oder Gruppenadministrator die Funktion **Manuelles Zuweisen von Auftragsrollen zu Stundeneinträgen** -Einstellung festlegen, wählen Sie eine **Auftragsrolle** aus dem Dropdown-Menü. Die Rolle, die beim Zuweisen zum Objekt angegeben wird, wird standardmäßig angezeigt. Wenn Ihnen keine Rolle für das Objekt zugewiesen wurde, wird Ihre Primäre Rolle als Standard angezeigt. Weitere Informationen zu dieser Einstellung finden Sie im Artikel [Zeitblatt- und Stundenvoreinstellungen konfigurieren](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

      ![screen_shot_2017-05-03_at_10.16.52_AM.png](assets/screen-shot-2017-05-03-at-10.16.52-am-350x346.png)

1. Klicken **Protokollzeiten**.

### Zusammenfassungsbereich

Sie können die Zeit für Aufgaben und Probleme im Bereich &quot;Zusammenfassung&quot;protokollieren.
Weitere Informationen finden Sie unter [Zusammenfassungsübersicht](../../workfront-basics/the-new-workfront-experience/summary-overview.md).

![](assets/summary-hour-log.png)

### Pinnwände {#boards}

Sie können die Zeit auf verbundenen Karten auf einer Workfront-Pinnwand protokollieren. Dies entspricht dem Protokollierungszeitpunkt für eine Aufgabe oder ein Problem und die auf der Karte protokollierten Stunden werden für die verbundene Aufgabe oder das Problem gespeichert.
Weitere Informationen finden Sie unter [Angeschlossene Karten auf Pinnwänden verwenden](/help/quicksilver/agile/get-started-with-boards/connected-cards.md).

### Mobile App {#mobile-app}

Sie können die Zeit über die mobile Workfront-App protokollieren.
Weitere Informationen finden Sie unter [Adobe Workfront für Android](/help/quicksilver/workfront-basics/mobile-apps/using-the-workfront-mobile-app/workfront-for-android.md) oder [Adobe Workfront für iOS](/help/quicksilver/workfront-basics/mobile-apps/using-the-workfront-mobile-app/workfront-for-ios.md).
