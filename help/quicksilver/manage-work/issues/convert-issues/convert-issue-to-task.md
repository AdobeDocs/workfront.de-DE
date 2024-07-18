---
product-area: projects
navigation-topic: convert-issues
title: Konvertieren eines Problems in eine Aufgabe in Adobe Workfront
description: Wenn nach dem Absenden des Problems noch mehr Arbeit erforderlich ist, können Sie das Problem in eine Aufgabe konvertieren.
author: Alina
feature: Work Management
exl-id: 9d8e50ab-9fed-4ded-83e1-29dc92c37171
source-git-commit: 1ae65d18419bf4235a7c97614b539811643110cc
workflow-type: tm+mt
source-wordcount: '1041'
ht-degree: 0%

---

# Konvertieren eines Problems in eine Aufgabe in Adobe Workfront

Wenn nach dem Absenden des Problems noch mehr Arbeit erforderlich ist, können Sie das Problem in eine Aufgabe konvertieren.

Allgemeine Informationen zu Konvertierungsproblemen finden Sie unter [Überblick über Konvertierungsprobleme in Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md).

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Arbeit oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf Probleme, Aufgaben und Projekte bearbeiten</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Berechtigungen für das Problem anzeigen</p> <p>Contribute-Berechtigungen für das Projekt</p> <p>Sie erhalten nach der Konvertierung des Problems Verwaltungsberechtigungen für die Aufgabe</p> <p>Weitere Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Anfordern des Zugriffs auf Objekte </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Konvertieren eines Problems in eine Aufgabe

1. Wechseln Sie zu einem Projekt und klicken Sie im linken Bereich auf [!UICONTROL **Probleme**] .
1. Klicken Sie auf das Problem, das Sie konvertieren möchten, um zur Landingpage des Problems zu gelangen.
1. Klicken Sie auf das Menü [!UICONTROL **Mehr**] zum Problem und dann auf [!UICONTROL **In Aufgabe konvertieren**].

   ![](assets/qs-issue-more-menu-highlighted-350x469.png)

   >[!TIP]
   >
   >Wenn das Problem mit einem Genehmigungsprozess verknüpft ist oder bereits mit einem aufgelösten Objekt verknüpft ist, zeigt Workfront oben im Feld [!UICONTROL In Projekt konvertieren] eine Warnung an, um Sie darüber zu informieren, dass die Genehmigung entfernt wurde oder das aufgelöste Objekt während der Konvertierung überschrieben wurde. Weitere Informationen finden Sie unter [Übersicht über Konvertierungsprobleme in Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md).

1. Aktualisieren Sie den Aufgabennamen im Abschnitt [!UICONTROL Aufgabenname] . Standardmäßig entspricht der Name der Aufgabe dem des ursprünglichen Problems.

   ![](assets/convert-to-task-box-nwe.png)

1. Klicken Sie auf [!UICONTROL **Zielprojekt**], geben Sie dann den Namen des Projekts ein, in das Sie die neue Aufgabe im Feld [!UICONTROL **Zielprojekt**] einfügen möchten, und wählen Sie es aus, wenn es in der Liste angezeigt wird. Das Projekt des Problems ist standardmäßig ausgewählt.

1. Klicken Sie auf [!UICONTROL **Überblick**] und geben Sie eine [!UICONTROL **Beschreibung**] für die Aufgabe ein.

   >[!TIP]
   >
   >   Ein System- oder Gruppenadministrator kann die Reihenfolge der Abschnitte im linken Bereich des Konvertierungsfelds ändern, indem er Ihre Layoutvorlage ändert.

1. (Optional und bedingt) Klicken Sie auf [!UICONTROL **Optionen**] und wählen Sie eine der folgenden Optionen aus.

   Der Workfront-Administrator oder -Gruppenadministrator muss diese Voreinstellungen aktivieren, bevor sie während der Konvertierung von Problemen angezeigt werden:

   * [!UICONTROL **Behalten Sie das ursprüngliche Problem bei und binden Sie seine Lösung mit dieser Aufgabe**]

     Wenn diese Option deaktiviert ist, wird das ursprüngliche Problem gelöscht.

     >[!NOTE]
     >
     >Benutzer ohne Zugriff oder Berechtigung zum Löschen von Problemen können das Problem beim Konvertieren nicht löschen, unabhängig vom Status dieser Einstellung. Informationen zum Zugriff auf und zu Berechtigungen für Probleme finden Sie unter:
     >   
     >   * [Gewähren des Zugriffs auf Probleme](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md)
     >   * [Ein Problem freigeben](../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md)
     >   
     >

   * [!UICONTROL **Erlauben (Benutzername), Zugriff auf diese Aufgabe zu erhalten**]

     Wenn diese Option deaktiviert ist, hat der Primäre Kontakt des Problems keinen Zugriff auf die neue Aufgabe.

   * [!UICONTROL **Behalten Sie das geplante Abschlussdatum des Problems bei**]

     Wenn diese Option deaktiviert ist, wird das [!UICONTROL geplante Abschlussdatum] der neuen Aufgabe aus dem [!UICONTROL geplanten Startdatum] der Aufgabe berechnet. Das [!UICONTROL geplante Startdatum] der neuen Aufgabe wird entsprechend den Systemeinstellungen für neue Aufgaben festgelegt.

     >[!NOTE]
     >
     >
     >Die Optionen, die hier angezeigt werden, hängen davon ab, wie der Workfront-Administrator sie für alle Benutzer im System konfiguriert hat. Weitere Informationen finden Sie unter [Konfigurieren von systemweiten Aufgaben- und Problemeinstellungen](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).
     >
     >Oder wenn die Gruppen der obersten Ebene in Ihrer Organisation sie separat konfiguriert haben, hängen die hier angezeigten Optionen davon ab, welche Gruppe mit dem in Schritt 6 ausgewählten Projekt verknüpft ist. Weitere Informationen finden Sie unter [Konfigurieren der Voreinstellungen für Aufgaben und Ausgaben für eine Gruppe](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

1. (Optional) Klicken Sie auf [!UICONTROL **Benutzerdefinierter Forms**] und fügen Sie ein benutzerdefiniertes Formular für die neue Aufgabe hinzu.

   >[!TIP]
   >
   >* Wenn ein benutzerdefiniertes Formular mit mehreren Objekten, das an das Problem angehängt ist, für die Verwendung sowohl mit Problemen als auch mit Aufgaben konfiguriert ist, werden alle im Formular gespeicherten Informationen bei der Konvertierung beibehalten, wenn sowohl die Felder für das Problem als auch die benutzerdefinierten Formulare der Aufgabe vorhanden sind.
   >* Wenn ein benutzerdefiniertes Formular mit mehreren Objekten und einem berechneten Feld an das Problem sowie an die Aufgabe angehängt ist, müssen das Problem und die Aufgabe mit allen Feldern kompatibel sein, auf die in den berechneten benutzerdefinierten Feldern des Formulars verwiesen wird. Wenn eine Inkompatibilität vorliegt, werden Sie durch eine Meldung darauf hingewiesen, dass Sie Anpassungen vornehmen müssen. Weitere Informationen finden Sie unter [Berechnete Felder zu einem Formular hinzufügen](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md).
   >* Wenn beim Bearbeiten des Projekts im Feld &quot;Task Default Custom Forms&quot;Standardformulare für das Zielprojekt definiert sind, werden diese Aufgabenformulare auch der neuen Aufgabe hinzugefügt. Alle benutzerdefinierten Felder, die zwischen dem ursprünglichen Problem und den Feldern in den Standardformularen für Aufgaben vorhanden sind, werden mit Informationen aus den Problemfeldern vorausgefüllt.


1. Klicken Sie auf [!UICONTROL **In Aufgabe konvertieren**].

   Das Problem ist jetzt eine Aufgabe für das vorgesehene Projekt, wenn Sie sich entschieden haben, das ursprüngliche Problem zu löschen.

   Oder

   Das Problem ist jetzt mit der neuen Aufgabe des ausgewählten Projekts verknüpft und wird nach Abschluss der Aufgabe abgeschlossen, wenn Sie beschlossen haben, das ursprüngliche Problem beizubehalten.

   Einige Problemfelder werden an die Aufgabe übertragen. Weitere Informationen finden Sie im Abschnitt [Original-Probleminformationen zu Projekten und Aufgaben anzeigen](#view-original-issue-information-on-projects-and-tasks) in diesem Artikel.

1. (Optional) Fahren Sie mit der Bearbeitung der Aufgabe fort.

## Originalinformationen zu Problemen in Projekten und Aufgaben anzeigen {#view-original-issue-information-on-projects-and-tasks}

Sie können die ursprünglichen Probleminformationen in Projekt- und Aufgabenlisten und Berichten oder im Bereich Projektdetails anzeigen. Informationen zum Erstellen von Berichten finden Sie unter [Benutzerspezifischen Bericht erstellen](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

Die folgende Tabelle zeigt, welche Problemfelder in den konvertierten Projekten und Aufgaben sichtbar sind.

| Problemfelder | Projekt- oder Aufgabenfeld | Projektliste oder Bericht | Bereich &quot;Projektdetails&quot; | Aufgabenliste oder Bericht | Bereich &quot;Aufgabendetails&quot; |
|---|---|---|---|---|---|
| [!UICONTROL Name des Problems] | [!UICONTROL Name des konvertierten Problems] | ms | ms | ms | ms |
| [!UICONTROL Primärer Kontakt] | [!UICONTROL Konvertierter Name des Ausgabeherstellers] | ms | ms | ms |
| [!UICONTROL Einstiegsdatum] | [!UICONTROL Problem-Eingabedatum konvertiert] | ms |  | ms |


>[!CAUTION]
>
>Wenn sich der [!UICONTROL Primäre Kontakt] eines Problems ändert oder wenn die Verknüpfung des Problems mit dem Projekt oder der Aufgabe aufgehoben wird, nachdem das Problem konvertiert wurde, wird der [!UICONTROL Name des konvertierten Ausgabe-Originators]nicht aktualisiert und der ursprüngliche [!UICONTROL Primäre Kontakt] des Problems wird zum Zeitpunkt der Konvertierung des Problems angezeigt.
