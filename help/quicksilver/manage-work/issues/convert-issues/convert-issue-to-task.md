---
product-area: projects
navigation-topic: convert-issues
title: Konvertieren eines Problems in eine Aufgabe in Adobe Workfront
description: Wenn nach dem Senden des Problems noch mehr Arbeit zum Abschließen des Problems erforderlich ist, können Sie das Problem in eine Aufgabe konvertieren.
author: Alina
feature: Work Management
exl-id: 9d8e50ab-9fed-4ded-83e1-29dc92c37171
source-git-commit: 55c714436fe59c84251c7f4e2a46614feae92cd6
workflow-type: tm+mt
source-wordcount: '1081'
ht-degree: 0%

---

# Konvertieren eines Problems in eine Aufgabe in Adobe Workfront

Wenn nach dem Senden des Problems noch mehr Arbeit zum Abschließen des Problems erforderlich ist, können Sie das Problem in eine Aufgabe konvertieren.

Allgemeine Informationen zum Konvertieren von Problemen finden Sie unter [Übersicht über das Konvertieren von Problemen in Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md).

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

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
   <td> <p>Arbeit oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene*</td> 
   <td> <p>Zugriff auf Probleme, Aufgaben und Projekte bearbeiten</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Einschränkungen in Ihrer Zugriffsebene festgelegt hat. Informationen dazu, wie Workfront-Admins Ihre Zugriffsebene ändern können, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Erstellen oder Ändern benutzerdefinierter Zugriffsebenen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Anzeigen der Berechtigungen für das Problem</p> <p>Beitragen von Berechtigungen zum Projekt</p> <p>Sie erhalten Verwaltungsberechtigungen für die Aufgabe, nachdem das Problem konvertiert wurde</p> <p>Informationen zum Anfordern zusätzlicher Zugriffsberechtigungen finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Anfordern von Zugriffsberechtigungen für Objekte </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Wenden Sie sich an Ihren Workfront-Administrator, um herauszufinden, über welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie verfügen.

## Aspekte

* Beim Konvertieren eines Problems in eine Aufgabe gibt es ein Verarbeitungslimit von 5 Minuten. Wenn an das Problem eine große Anzahl von Dokumenten angehängt ist und es nicht konvertiert werden kann, müssen Sie möglicherweise einige der Dokumente entfernen und erneut versuchen.

## Anfrage in eine Aufgabe konvertieren

1. Gehen Sie zu einem Projekt und klicken Sie [!UICONTROL **linken Bereich**] Probleme“.
1. Klicken Sie auf das Problem, das Sie konvertieren möchten, um zur Landingpage des Problems zu gelangen.
1. Klicken Sie auf das [!UICONTROL **Mehr**]-Menü des Problems und dann auf [!UICONTROL **In Aufgabe konvertieren**].

   ![Menü „Problem Mehr“](assets/qs-issue-more-menu-highlighted-350x469.png)

   >[!TIP]
   >
   >Wenn das Problem mit einem Genehmigungsprozess verknüpft ist oder bereits mit einem Lösungsobjekt verknüpft ist, zeigt Workfront oben im Feld [!UICONTROL In Projekt konvertieren] eine Warnung an, die Sie darüber informiert, dass die Genehmigung entfernt oder das Lösungsobjekt während der Konvertierung überschrieben wird. Weitere Informationen finden Sie unter [Übersicht über Konvertierungsprobleme in Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md).

1. Aktualisieren Sie den Aufgabennamen im Abschnitt [!UICONTROL Aufgabenname]. Standardmäßig entspricht der Name der Aufgabe dem Namen des ursprünglichen Problems.

   ![In Aufgabenfeld konvertieren](assets/convert-to-task-box-nwe.png)

1. Klicken Sie [!UICONTROL **Zielprojekt**], geben Sie dann den Namen des Projekts, in dem Sie die neue Aufgabe platzieren möchten, in das Feld [!UICONTROL **Zielprojekt**] ein und wählen Sie es aus, wenn es in der Liste angezeigt wird. Das Projekt des Problems ist standardmäßig ausgewählt.

1. Klicken Sie auf [!UICONTROL **Übersicht**] und geben Sie dann eine [!UICONTROL **Beschreibung**] für die Aufgabe ein.

   >[!TIP]
   >
   >   System- oder Gruppenadmins können die Reihenfolge der Abschnitte im linken Bereich des Konvertierungsfelds ändern, indem sie die Layout-Vorlage ändern.

1. (Optional und bedingt) Klicken Sie [!UICONTROL **Optionen**] und wählen Sie eine der folgenden Optionen aus.

   Der Workfront-Administrator oder Gruppenadministrator muss diese Voreinstellungen aktivieren, bevor sie während der Konvertierung von Problemen angezeigt werden:

   * [!UICONTROL **Ursprüngliches Problem beibehalten und seine Lösung mit dieser Aufgabe verknüpfen**]

     Wenn die Auswahl aufgehoben wird, wird das ursprüngliche Problem gelöscht.

     >[!NOTE]
     >
     >Benutzende ohne Zugriff oder Berechtigung zum Löschen von Problemen können das Problem während der Konvertierung nicht löschen, unabhängig vom Status dieser Einstellung. Informationen zu Zugriff und Berechtigungen für Probleme finden Sie unter:
     >   
     >   * [Zugriff auf Anfragen gewähren](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md)
     >   * [Freigeben eines Problems](../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md)
     >   
     >

   * [!UICONTROL **Erlauben Sie (Benutzername), Zugriff auf diese Aufgabe zu erhalten**]

     Wenn diese Option deaktiviert ist, hat der Primäre Ansprechpartner des Problems keinen Zugriff auf die neue Aufgabe.

   * [!UICONTROL **Das geplante Abschlussdatum der Anfrage beibehalten**]

     Wenn diese Option deaktiviert ist[!UICONTROL &#x200B; wird das geplante Abschlussdatum &#x200B;] neuen Aufgabe anhand des [!UICONTROL geplanten Startdatums] berechnet. Das [!UICONTROL geplante Startdatum] der neuen Aufgabe wird entsprechend den Systemeinstellungen für neue Aufgaben festgelegt.

     >[!NOTE]
     >
     >
     >Welche Optionen hier angezeigt werden, hängt davon ab, wie der Workfront-Administrator sie für alle Personen im System konfiguriert hat. Weitere Informationen finden Sie unter [Systemweite Aufgaben- und Problemeinstellungen konfigurieren](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).
     >
     >Oder, falls die Gruppen der obersten Ebene in Ihrer Organisation sie separat konfiguriert haben, hängen die hier angezeigten Optionen davon ab, welche Gruppe mit dem Projekt verknüpft ist, das Sie in Schritt 6 ausgewählt haben. Weitere Informationen finden Sie unter [Konfigurieren von Aufgaben- und Problemeinstellungen für eine Gruppe](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

1. (Optional) Klicken Sie auf [!UICONTROL **Benutzerdefinierte Forms**] und fügen Sie ein benutzerdefiniertes Formular für die neue Aufgabe hinzu.

   >[!TIP]
   >
   >* Wenn ein benutzerdefiniertes Formular mit mehreren Objekten, das an das Problem angehängt ist, für die Verwendung mit sowohl Problemen als auch Aufgaben konfiguriert ist, werden alle im Formular gespeicherten Informationen beibehalten, wenn Sie die Konvertierung durchführen, wenn die Felder sowohl für das Problem als auch für die benutzerdefinierten Formulare der Aufgabe vorhanden sind.
   >* Wenn ein benutzerdefiniertes Formular mit mehreren Objekten und einem berechneten Feld sowohl an das Problem als auch an die Aufgabe angehängt ist, müssen das Problem und die Aufgabe mit allen Feldern kompatibel sein, auf die in den berechneten benutzerdefinierten Feldern des Formulars verwiesen wird. Bei einer Inkompatibilität werden Sie durch eine Meldung darauf hingewiesen, dass Sie Anpassungen vornehmen müssen. Weitere Informationen finden Sie unter [Hinzufügen berechneter Felder zu einem Formular](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md).
   >* Wenn im Zielprojekt beim Bearbeiten des Projekts im Feld „Aufgabe - Standard - Benutzerdefiniertes Forms&quot; Standardformulare definiert sind, werden diese Aufgabenformulare auch der neuen Aufgabe hinzugefügt. Alle benutzerdefinierten Felder, die zwischen dem ursprünglichen Problem und den Feldern in den Standardaufgabenformularen vorhanden sind, werden vorab mit Informationen aus den Problemfeldern ausgefüllt.


1. Klicken Sie [!UICONTROL **In Aufgabe umwandeln**].

   Das Problem ist jetzt eine Aufgabe im angegebenen Projekt, wenn Sie entschieden haben, das ursprüngliche Problem zu löschen.

   Oder

   Das Problem ist nun mit der neuen Aufgabe für das ausgewählte Projekt verknüpft und wird abgeschlossen, sobald die Aufgabe abgeschlossen ist, falls Sie die ursprüngliche Anfrage beibehalten möchten.

   Einige Problemfelder werden auf die Aufgabe übertragen. Weitere Informationen finden Sie [ Abschnitt „Anzeigen der ursprünglichen Anfrageinformationen zu Projekten und Aufgaben](#view-original-issue-information-on-projects-and-tasks) in diesem Artikel.

1. (Optional) Fahren Sie mit der Bearbeitung der Aufgabe nach Bedarf fort.

## Anzeigen der ursprünglichen Anfrageinformationen zu Projekten und Aufgaben {#view-original-issue-information-on-projects-and-tasks}

Sie können die ursprünglichen Anfrageinformationen in Projekt- und Aufgabenlisten und Berichten oder im Bereich Projektdetails anzeigen. Informationen zum Erstellen von Berichten finden Sie [Erstellen eines benutzerdefinierten Berichts](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

Die folgende Tabelle zeigt, welche Problemfelder in den konvertierten Projekten und Aufgaben sichtbar sind.

| Problemfelder | Projekt- oder Aufgabenfeld | Projektliste oder Bericht | Bereich „Projektdetails“ | Aufgabenliste oder Bericht | Aufgabendetailbereich |
|---|---|---|---|---|---|
| [!UICONTROL Anfragename] | [!UICONTROL Name des konvertierten Problems] | ✔ | ✔ | ✔ | ✔ |
| [!UICONTROL Primärer Kontakt] | [!UICONTROL Name des Urhebers des konvertierten Problems] | ✔ | ✔ | ✔ |
| [!UICONTROL Eingabedatum] | [!UICONTROL Problem-Eingabedatum konvertiert] | ✔ |  | ✔ |


>[!CAUTION]
>
>Wenn sich der [!UICONTROL Primäre &#x200B;] eines Problems ändert oder die Verknüpfung des Problems mit dem Projekt oder der Aufgabe nach der Konvertierung des Problems aufgehoben wird, wird der [!UICONTROL Name des konvertierten Problemurhebers] nicht aktualisiert und der ursprüngliche [!UICONTROL Primäre &#x200B;] des Problems zum Zeitpunkt der Konvertierung wird angezeigt.
