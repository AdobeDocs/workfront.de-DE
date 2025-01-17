---
product-area: projects;user-management
navigation-topic: assign-tasks
title: Erweiterte Zuweisungen erstellen
description: Mithilfe von „Erweiterte Zuweisungen“ können Sie Aufgaben- oder Problemzuweisungen verwalten.
author: Lisa
feature: Work Management, Resource Management
role: User
exl-id: 09780f78-4eb8-404d-859b-d066d462776d
source-git-commit: 259fd0e3fdaa07bfdb0301d60bf0d9b1090b4ef7
workflow-type: tm+mt
source-wordcount: '1171'
ht-degree: 0%

---

# Erweiterte Zuweisungen erstellen

<!-- Audited: 07/2024-->

<span class="preview">Die hervorgehobenen Informationen auf dieser Seite beziehen sich auf Funktionen, die noch nicht allgemein verfügbar sind. Sie ist nur in der Vorschau -Umgebung für alle Kunden verfügbar oder in der Produktionsumgebung für Kunden, die schnelle Versionen aktiviert haben.</span>

<span class="preview">Informationen zu Schnellversionen finden Sie unter [Aktivieren oder Deaktivieren von Schnellversionen für Ihre Organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>

<span class="preview">Informationen zur aktuellen Version finden Sie unter [Versionsübersicht 4. Quartal 2024](/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-release-overview.md).</span>

Mithilfe von „Erweiterte Zuweisungen“ können Sie Aufgaben- oder Problemzuweisungen verwalten.

Sie können bei erweiterten Zuweisungen die folgenden Zuweisungsinformationen anpassen:

* Weisen Sie der Aufgabe oder dem Problem Benutzer zu (dies kann außerhalb einer erweiterten Zuweisung erfolgen).
* Anpassen und Verteilen der Anzahl der Stunden, die jedem Zugewiesenen zugewiesen werden.
* Legen Sie fest, welcher Benutzer als Eigentümer oder Primärer Bevollmächtigter der Aufgabe oder des Problems bestimmt werden soll.
* Geben Sie an, welche Rolle jeder Benutzer bei der Arbeit an der Aufgabe oder dem Problem erfüllt.
  <!--* <span class="preview">Override the billing rate for a job role.</span>-->

>[!NOTE]
>
>Wenn Sie Benutzende einer Arbeit zuweisen, wirkt sich ihre Verfügbarkeit entsprechend den Zeitplänen auf die geplanten und erwarteten Termine von Aufgaben und Problemen aus. Weitere Informationen zu Zeitplänen finden Sie unter [Erstellen eines Zeitplans](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

## Bereiche von Adobe Workfront, in denen Sie erweiterte Zuweisungen vornehmen können

In diesem Artikel wird beschrieben, wie Sie in der Kopfzeile der Aufgabe oder des Problems auf erweiterte Zuweisungen zugreifen können.

Darüber hinaus können Sie in den folgenden Bereichen von Workfront erweiterte Zuweisungen vornehmen:

* In Listen und Berichten, wenn das Feld „Zuweisungen“ in der Ansicht angezeigt wird.
* Im Abschnitt Arbeitsaufträge beim Bearbeiten einer Aufgabe. Weitere Informationen finden Sie unter [Aufgaben bearbeiten](../../../manage-work/tasks/manage-tasks/edit-tasks.md).
* In der Aufgaben- oder Problem-Kopfzeile im Bereich Zuweisungen .
* Im Workload Balancer. Weitere Informationen finden Sie unter [Arbeiten manuell über den Workload Balancer zuweisen](../../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer-manually.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Neu: Standard</p>
    <p>Aktuell: Arbeit oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriff auf Aufgaben und Probleme bearbeiten</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Contribute oder höhere Berechtigungen für eine Aufgabe oder ein Problem</p>  </td> 
  </tr> 
 </tbody> 
</table>

*Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Erweiterte Zuweisungen vornehmen

1. Wechseln Sie zu dem Projekt, dem Sie eine Aufgabe oder ein Problem zuweisen möchten.
1. Klicken Sie **linken Bereich** Aufgaben“ oder **Probleme** und klicken Sie dann auf den Namen einer Aufgabe oder eines Problems in der Liste.

   >[!TIP]
   >
   >Erweiterte Zuweisungen können direkt in der Aufgaben- oder Problemliste vorgenommen werden, wenn mindestens zwei Personen zugewiesen sind. Klicken Sie in das **Arbeitsaufträge**-Feld in derselben Zeile wie die Aufgabe oder das Problem und klicken Sie dann auf das **Personen-Symbol**, um das Fenster Erweiterte Arbeitsaufträge zu öffnen. Fahren Sie mit Schritt 5 fort, um mit dem Erstellen erweiterter Zuweisungen fortzufahren.\
   >![](assets/nwe-advanced-assignments-350x55.png)
   >

1. Klicken Sie **Zuweisen zu** im Feld **Zuweisungen** in der Kopfzeile der Aufgabe oder des Problems

   Oder

   Klicken Sie auf den Namen der Zuweisungen, wenn die Aufgabe oder das Problem bereits zugewiesen ist.

1. Klicken Sie auf **Erweitert**.

   <span class="preview">![Klicken Sie auf Erweitert](assets/assignments-box-in-task-header.png)</span>

1. Beginnen Sie im Feld **Personen, Rollen und Teams suchen** mit der Eingabe des Namens eines Benutzers, einer Rolle oder eines Teams und klicken Sie dann auf den Namen, wenn er in der Dropdown-Liste angezeigt wird.

   >[!NOTE]
   >
   >Wenn der Name des Benutzers ein Sonderzeichen enthält, müssen Sie das Sonderzeichen in das Suchfeld einschließen.

1. (Optional) Fügen Sie im Feld **Personen, Rollen oder Teams suchen“ weitere Beauftragte**, um der Aufgabe oder dem Problem mehrere Ressourcen hinzuzufügen.

   >[!TIP]
   >
   >* Sie können mehrere Benutzer, Aufgabengebiete oder Teams zuweisen. Sie können nur aktive Benutzer, Aufgabengebiete und Teams zuweisen.
   >
   >
   >* Beachten Sie beim Hinzufügen einer Benutzerzuweisung den Avatar, die Primäre Rolle des Benutzers oder seine E-Mail-Adresse, um zwischen Benutzern mit identischen Namen zu unterscheiden.
   >Benutzende müssen mindestens einem Aufgabengebiet zugeordnet sein, damit sie es beim Hinzufügen anzeigen können.
   >Die Einstellung Kontaktinformationen anzeigen muss in Ihrer Zugriffsebene aktiviert sein, damit Benutzer die E-Mails von Benutzern anzeigen können. Weitere Informationen finden Sie unter [Gewähren des Benutzerzugriffs](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).
   >
   >
   >* Wenn ein(e) Benutzende(r), ein Aufgabengebiet oder ein Team zugewiesen wurde, bevor sie/er deaktiviert wurden, bleiben sie/sie dem Arbeitselement zugewiesen. In diesem Fall empfehlen wir Folgendes:
   >   
   >   * Weisen Sie das Arbeitselement den aktiven Ressourcen neu zu.
   >   * Verknüpfen Sie die Benutzer in einem deaktivierten Team mit einem aktiven Team und weisen Sie das Arbeitselement dem aktiven Team zu.
   >

   <!-- SHOULD BE THIRD BULLET POINT IN TIP TABLE WHEN THIS FEATURE IS RELEASED 
    * <span class="preview">When adding a job role assignment, you can search for the job role or location. Select the System/Default Job Role to use the default billing rate for the assignment, or select a Rate Card Job Role to override the rate at the assignment level. For more information on rate cards, see [Manage rate cards](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/manage-rate-cards.md).</span>
    -->

1. Geben Sie für jeden Benutzer in der Spalte **Verantwortlicher** die folgenden Informationen an:


   * **Verantwortlicher**: Bewegen Sie den Mauszeiger über den Namen des Verantwortlichen und klicken Sie **Primär machen** im Feld „Verantwortlicher“, wenn Sie den Verantwortlichen als Aufgaben- oder Problembesitzer markieren möchten. Ein grünes Kontrollkästchen gibt an, dass der angegebene Benutzer der Primäre Ansprechpartner für die Aufgabe oder das Problem ist. Adobe Workfront markiert den ersten Benutzer oder das erste Aufgabengebiet, das Sie einer Aufgabe oder einem Problem zuweisen, als Inhaber oder Primäre Zuweisung. Ein Team kann nicht zum Primären Eigentümer einer Aufgabe oder eines Problems bestimmt werden.

     >[!IMPORTANT]
     >
     >Je nachdem, wie der Workfront-Administrator oder der Gruppenadministrator Ihre Projektvoreinstellungen eingerichtet hat, kann Workfront den Zeitplan des Aufgabenbesitzers verwenden, um den Zeitplan der Aufgabe zu berechnen, wenn mehrere Benutzende der Aufgabe zugewiesen sind. Informationen zu mehreren Aufgabenzuweisungen finden Sie im Abschnitt „Mehrere Benutzer einer Aufgabe zuweisen“ im Artikel &quot;[ zuweisen](../../../manage-work/tasks/assign-tasks/assign-tasks.md).

   * **Zuteilungen** : Wenn der Dauertyp einer Aufgabe „Einfach“ ist, geben Sie die Anzahl der Stunden an, die jeder Benutzer bzw. jedes Aufgabengebiet der Aufgabe zugewiesen werden soll. Die Summe aller zugewiesenen Stunden für jeden Benutzer ist gleich der Zahl im Feld **Geplante Stunden** am unteren Rand der Spalte „Zuordnungen“. Geben Sie in allen anderen Fällen den Prozentsatz der Zeit (oder Zuordnung) an, die der Beauftragte für die Lösung der Aufgabe oder des Problems aufwenden soll.

     <!--   
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: make sure this is right in the new UI for both classic and QS???)</p>   
     -->

     >[!TIP]
     >   
     >   * Nachdem Sie die Zuweisungen für Aufgaben manuell geändert haben, werden die geplanten Stunden der Aufgaben möglicherweise entsprechend aktualisiert. Weitere Informationen finden Sie im Abschnitt „Geplante Stunden für die Aktualisierung von Aufgaben bei der Verwaltung von Benutzerzuweisungen“ im Artikel &quot;[ Stunden - Übersicht](../../../manage-work/tasks/task-information/planned-hours.md).
     >   * Zuweisungen für Probleme können nicht manuell geändert werden.
     >   * Zuteilungen für Teams, die Aufgaben zugewiesen sind, können nicht manuell geändert werden.

   * **Rolle des Verantwortlichen:** Wählen Sie die Rolle aus, die der Benutzer bei der Erfüllung dieser Zuweisung verwenden soll.  Standardmäßig wird die Primäre Rolle des/r Benutzenden angezeigt. Klicken Sie in das Feld Rolle des Verantwortlichen, um eine andere Rolle auszuwählen.  Wenn Sie die Aufgabe oder das Problem zuerst einer Rolle zuweisen und dann einen Benutzer hinzufügen, der diese Rolle als zweite Zuweisung erfüllen kann, wird die Liste der vorgeschlagenen Benutzer nach den Benutzern gefiltert, die die der Aufgabe und dem Problem bereits zugewiesenen Rollen erfüllen können.

     ![Rolle des Verantwortlichen](assets/advanced-assignments-select-role.png)

   <!--<div class="preview">

   * **Location**: The location comes from the rate card, if a rate card attached to the project uses locations with the job roles. The location can't be changed. 

   * **Billing Rates**: The billing rate for a user comes from the system rate for the user or their associated job role. The billing rate for a job role comes from the system rate or from the rate card, if a rate card is attached to the project. Existing billing rates are not displayed in this field. Click in the field to change the billing rate for this specific task assignment.

   </div>-->

   * **Dauertyp**: Dies ist nur für Aufgaben verfügbar. Klicken Sie auf den Namen des Dauertyps und wählen Sie aus dem Dropdown-Menü einen Dauertyp aus. Weitere Informationen zu den Dauertypen finden Sie unter [Übersicht über die Aufgabendauer und den Dauertyp](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

   * **Dauer:** Sie können dieses Feld für eine Aufgabe aktualisieren, wenn Sie über Verwaltungsberechtigungen für die Aufgabe verfügen.

     Weitere Informationen finden Sie unter [Übersicht über Aufgabendauer und -typ](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md). Bei der Massenbearbeitung von Zuweisungsinformationen wird ein ähnliches Dialogfeld angezeigt, in dem Benutzer, Stunden, Zuordnung und Aufgabenbesitzer zugewiesen werden.

   * **Geplante Stunden**: Wenn der Dauertyp „Berechnete Zuweisung“ oder „Einfach“ ist, aktualisieren Sie die Anzahl der geplanten Stunden. Dadurch werden die Prozentsätze der Zuordnungen bzw. die Stunden für jede Ressource gleichmäßig verteilt. Workfront berechnet die geplanten Stunden, wenn der Dauertyp „Berechnete Arbeit“ oder „Leistungsgesteuert“ ist. Weitere Informationen finden Sie unter [Übersicht über Aufgabendauer und -typ](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).


1. Klicken Sie auf **Speichern**.
