---
user-type: administrator
product-area: system-administration;projects
keywords: kickstart,kick-start,kickstarts,kick-starts
navigation-topic: use-kick-starts
title: Kick-Starts - einfache Projekt- und Aufgabenimportvorbereitung
description: Beschreibt ausführlich die verfügbaren Einstellungen und Steuerelemente für ein einfaches Projekt und den Import von Aufgaben mithilfe der Kick Start-Methode.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: c095ce9d-b189-449b-bd13-2633837697ed
source-git-commit: a849ecaf6097dcdc924aaab2867f37bf57d5bc09
workflow-type: tm+mt
source-wordcount: '1477'
ht-degree: 9%

---

# Kick-Starts-Szenario: einfache Vorbereitung des Projekt- und Aufgabenimports

Beschreibt ausführlich die verfügbaren Einstellungen und Steuerelemente für ein einfaches Projekt und den Import von Aufgaben mithilfe der Kick Start-Methode.

## Szenario

Das Implementierungsteam würde lieber Projekt- und Aufgabeninformationen für aktive Projekte importieren, anstatt diese Daten manuell in das System einzugeben.

* [Projekte](#projects)
* [Aufgabenliste](#task-list)

### Projekte {#projects}

In der folgenden Tabelle sind vier Projekte und ihre grundlegenden Details aufgeführt, die den Kick Start-Dateiformaten zugeordnet werden müssen.

Dies setzt voraus, dass Benutzer bereits in Adobe Workfront importiert wurden. Wenn Benutzer noch nicht in Workfront sind, müssen Sie andere Namen eingeben oder das Kick Start-Szenario mit Benutzern vor diesem Szenario durchführen.

1. Implementieren Sie Workfront.

   | Geplantes Startdatum | Heute |
   |---|---|
   | Projektleiter | Jennifer Campbell |
   | Projektsponsor | Marc Lewis |
   | Gruppe | Marketing |
   | Firma | *YourCompany* |

   {style=&quot;table-layout:auto&quot;}

1. Implementieren des HR-Systems.

   | Geplantes Startdatum | 14. Juli 2020 |
   |---|---|
   | Projektleiter | Pam Reynolds |
   | Projektsponsor | Marc Lewis |
   | Gruppe | Marketing |
   | Firma | *YourCompany* |

   {style=&quot;table-layout:auto&quot;}

1. Implementieren Sie Document Management System.

   | Geplantes Startdatum | 22. August 2020 |
   |---|---|
   | Projektleiter | Jennifer Campbell |
   | Projektsponsor | Ray Andrews |
   | Gruppe | IT |
   | Firma | *YourCompany* |

   {style=&quot;table-layout:auto&quot;}

1. Implementieren Sie das neue Kalendersystem.

   | Geplantes Startdatum | 6. September 2020 |
   |---|---|
   | Projektleiter | Pam Reynolds |
   | Projektsponsor | Ray Andrews |
   | Gruppe | IT |
   | Firma | *YourCompany* |

   {style=&quot;table-layout:auto&quot;}

### Aufgabenliste {#task-list}

In der folgenden Aufgabenliste werden zu vereinfachte Aufgabenlisten für die Projekte angezeigt. Der einzige Unterschied zwischen den Projekten besteht darin, wann die Projekte beginnen und wie weit sie voranschreiten.

Übergeordnete Aufgaben übernehmen die Aufgaben &quot;Dauer&quot;, &quot;Arbeit&quot;und &quot;Prozent abgeschlossen&quot;für untergeordnete Aufgaben. Es ist nicht erforderlich, diese Werte festzulegen, damit diese zu Zusammenfassungsaufgaben werden.

>[!NOTE]
>
>Die in diesem Szenario bereitgestellten Anweisungen sind nicht so explizit wie die in [Szenario für Kick-Starts: Vorbereitung von Unternehmens-, Gruppen-, Rollen- und Benutzerkick-Starts](../../../administration-and-setup/manage-workfront/using-kick-starts/kick-starts-scenario-company-group-role-user-prep.md). Es wird davon ausgegangen, dass Sie bereits gelernt haben, wie Sie Werte aus den Tabellen &quot;Unternehmen&quot;und &quot;Gruppe&quot;nachschlagen und kopieren können. Daher werden diese Schritte zwar erwähnt, aber nicht spezifisch umrissen.

1. Konfigurieren.
1. Importieren Sie Benutzer.

   <table style="table-layout:auto"> 
    <col width="50%"> 
    <col width="50%"> 
    <tbody> 
     <tr> 
      <td role="rowheader">Zugewiesen an</td> 
      <td>Ray Andrews</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Übergeordnete Aufgabe</td> 
      <td>1</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Dauer</td> 
      <td>1 Stunde</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Arbeit</td> 
      <td>1 Stunde</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Prozent abgeschlossen</td> 
      <td> <p>Workfront: 0 %</p> <p>HR: 100 %</p> <p>Dokumente: 100 %</p> <p>Kalender: 100 %</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Legen Sie Berechtigungen fest.

   <table style="table-layout:auto"> 
    <col width="50%"> 
    <col width="50%"> 
    <tbody> 
     <tr> 
      <td role="rowheader">Zugewiesen an</td> 
      <td>Ray Andrews</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Übergeordnete Aufgabe</td> 
      <td>1</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Vor</td> 
      <td>2</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Dauer</td> 
      <td>1 Stunde</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Arbeit</td> 
      <td>1 Stunde</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Prozent abgeschlossen</td> 
      <td> <p>Workfront: 0 %</p> <p>HR: 100 %</p> <p>Dokumente: 100 %</p> <p>Kalender: 100 %</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Gruppen erstellen.

   <table style="table-layout:auto"> 
    <col width="50%"> 
    <col width="50%"> 
    <tbody> 
     <tr> 
      <td role="rowheader">Zugewiesen an</td> 
      <td>Ray Andrews</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Übergeordnete Aufgabe</td> 
      <td>1</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Vor</td> 
      <td>4</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Dauer</td> 
      <td>2 Tage</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Arbeit</td> 
      <td>4 Stunden</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Prozent abgeschlossen</td> 
      <td> <p>Workfront: 0 %</p> <p>HR: 100 %</p> <p>Dokumente: 100 %</p> <p>Kalender: 25 %</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Vorbereitung von Schulungen.

   <table style="table-layout:auto"> 
    <col width="50%"> 
    <col width="50%"> 
    <tbody> 
     <tr> 
      <td role="rowheader">Zugewiesen an</td> 
      <td>Chris Manning</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Dauer</td> 
      <td>2 Tage</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Arbeit</td> 
      <td>4 Stunden</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Prozent abgeschlossen</td> 
      <td> <p>Workfront: 0 %</p> <p>HR: 100 %</p> <p>Dokumente: 50 %</p> <p>Kalender: 100 %</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Erstellen Sie fortlaufende Support-Richtlinien.

   <table style="table-layout:auto"> 
    <col width="50%"> 
    <col width="50%"> 
    <tbody> 
     <tr> 
      <td role="rowheader">Zugewiesen an</td> 
      <td>Chris Manning</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Dauer</td> 
      <td>2 Tage</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Arbeit</td> 
      <td>4 Stunden</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Prozent abgeschlossen</td> 
      <td> <p>Workfront: 0 %</p> <p>HR: 100 %</p> <p>Dokumente: 50 %</p> <p>Kalender: 0 %</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Rollout.

   | Vor | 1, 6, 7 |
   |---|---|

   {style=&quot;table-layout:auto&quot;}

1. Trainieren Sie Benutzer.

   <table style="table-layout:auto"> 
    <col width="50%"> 
    <col width="50%"> 
    <tbody> 
     <tr> 
      <td role="rowheader">Zugewiesen an</td> 
      <td>Chris Manning</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Übergeordnete Aufgabe</td> 
      <td>8</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Dauer</td> 
      <td>1 Tag</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Arbeit</td> 
      <td>2 Stunden</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Prozent abgeschlossen</td> 
      <td> <p>Workfront: 0 %</p> <p>HR: 0 %</p> <p>Dokumente: 0 %</p> <p>Kalender: 0 %</p> </td> 
     </tr> 
    </tbody> 
   </table>

## Vorlage herunterladen

Gehen Sie zur Seite Kick-Starts . Wählen Sie die Objekte Firma, Gruppe, Projekt, Aufgabe und Benutzer aus. Aktivieren Sie das Kontrollkästchen Vorhandene Daten einschließen (führen Sie dies aus, um schnell auf Unternehmens-, Gruppen- und Benutzer-IDs zu verweisen). Klicken Sie auf die Schaltfläche Herunterladen .

## Input Project Details

Öffnen Sie die soeben heruntergeladene Datei Workfront.xlsx . Gehen Sie zum PROJ-Projektblatt.

![](assets/im2-350x14.png)\
Sofern Sie keine Projekte in Workfront bereits erstellt haben, sollte diese leer sein.\
![](assets/im3-350x37.png)

>[!NOTE]
>
>Erwägen Sie die Verwendung des Tools zum Einfrieren von Bereichen des Arbeitsblatts und/oder das Ausblenden oder Entfernen nicht benötigter Spalten, um die Arbeit mit dem Arbeitsblatt zu vereinfachen. Achten Sie jedoch darauf, keine erforderlichen Spalten oder Spalten zu entfernen, die später verwendet werden sollen.

![](assets/im10-350x42.png)

Legen Sie die Werte für die folgenden Projektfelder fest:

* **isNew column festlegen**
Geben Sie TRUE in die Zeilen 3 bis 6 für die Spalte isNew ein.
* **Festlegen eindeutiger IDs**
Geben Sie in jeder Zeile eine eindeutige ID für die ID-Spalte ein. In der Regel funktionieren Ganzzahlen ab 1 bei der Erstellung neuer Datensätze gut.
* **Festlegen von Projektnamen**
Geben Sie die Namen der einzelnen Projekte in die Spalte setName ein.
* **Festlegen des Projektzeitplans**

   Geben Sie die Kennung des Zeitplans ein, den das Projekt im Feld setScheduleID verwenden soll

* **Festlegen des geplanten Projektstartdatums**

   Geben Sie Datum und Uhrzeit in die Spalte setPlannedStartDate mit der Uhrzeit und dem Datum ein, an dem das Projekt beginnen soll. Wenn dies leer gelassen wird, importiert Workfront das Projekt mit dem aktuellen Tagesdatum und einem Zeitstempel für Mitternacht dieses Tages gemäß der Zeitzone des Browsers.

* **Festlegen von Aufgabenzahlen**
Geben Sie Werte in die Spalte setTaskNumber ein, um die Reihenfolge zu steuern, in der die Aufgaben im Projektplan angezeigt werden.
* **Geben Sie Projektdaten an.**
Geben Sie das geplante Startdatum für jedes Projekt in die Spalte setPlannedStartDate ein.
* **Legen Sie weitere erforderliche Details fest.**
Geben Sie bei Bedarf weitere Details ein, z. B. eine Beschreibung oder den aktuellen Status. Suchen Sie die Gruppen-IDs für jedes Projekt auf der Seite &quot;GRUPPENgruppe&quot;und geben Sie sie in die Spalte &quot;setGroupID&quot;für die jeweiligen Projekte ein. Suchen Sie im Arbeitsblatt CMPY Company nach der Firmen-ID für die Projekte und geben Sie sie in die Spalte setCompanyID ein. Suchen Sie die Benutzer-ID für jeden Projekteigentümer auf dem USER User-Blatt und geben Sie sie in die Spalte setOwnerID ein. Suchen Sie die Benutzer-ID für jeden Projektsponsor auf dem USER User-Blatt und geben Sie sie in die Spalte setSponsorID ein.

![](assets/im9-350x24.png)

>[!NOTE]
>
>Zulässige Werte für die Felder Status und Priorität können Sie ermitteln, indem Sie die Status- und Prioritätseinstellungen für jedes Objekt im Bereich Workflow-Einrichtung von Workfront überprüfen.

## Details zur Eingabeaufgabe

Sie können Informationen zu den Aufgaben im Projekt hinzufügen, während Sie das Projekt mit Kick-Start importieren.

Öffnen Sie die soeben heruntergeladene Datei Workfront.xlsx . **Gehen Sie zum TASK Task-Blatt.**

Sofern Sie keine Aufgaben in Workfront bereits erstellt haben, sollte dieses Blatt leer sein.

![](assets/im8-350x14.png)

![](assets/im7-350x43.png)

![](assets/im6-350x16.png)

Die einfachste Möglichkeit, Aufgaben zuzuordnen, besteht darin, jeweils nur ein Projekt zuzuordnen (insbesondere dann, wenn die Aufgaben in jedem Projekt gleich sind). Anschließend können Sie den Aufgabenplan für das erste Projekt kopieren und kleine Anpassungen am Aufgabenplan für die nachfolgenden Projekte vornehmen. Bei den verbleibenden Schritten wird davon ausgegangen, dass Sie Aufgaben nur für das Projekt &quot;Implementieren von Workfront&quot;erstellen. Gemäß dem Szenario importieren Sie 9 Aufgaben pro Projekt. Geben Sie daher TRUE in die Zeilen 3 bis 11 für die Spalte isNew ein.

Legen Sie die Werte für die folgenden Aufgabenfelder fest:

* **Festlegen von IDs**
Geben Sie in jeder Zeile eine eindeutige ID für die ID-Spalte ein.
* **Namen festlegen**
Geben Sie die Aufgabennamen in die Spalte setName ein.
* **Projekt-ID bestätigen**
Geben Sie die ID ein, die Sie für das Projekt &quot;Implementieren von Workfront&quot;festgelegt haben. Überprüfen Sie das PROJ-Projektblatt, um sicherzustellen, dass es die richtige ID ist.
* **Benutzer festlegen**
Wechseln Sie zum Blatt &quot;USER User&quot;, um die ID für den Benutzer zu suchen, der jeder Aufgabe zugewiesen ist, und geben Sie diese Werte in die entsprechenden Zellen in der Spalte setAssignedToID ein.
* **Identifizieren von Aufgabenbeziehungen**
Geben Sie für die Aufgaben 2 bis 5 in die Spalte setParentID den Wert 1 ein. Geben Sie für Aufgabe 9 in die Spalte setParentID den Wert 8 ein. Geben Sie in der Spalte setPredecessorString die Aufgabennummer für jede Vorgängeraufgabe ein. In Fällen, in denen eine Aufgabe mehrere Vorgänger hat, wie in diesem Szenario Aufgabe 8, müssen Sie ein Komma verwenden, um jede Vorgänger-Aufgaben-ID zu trennen. Vorgänger können mit Verzögerungen bei Nicht-Finish-Start-Beziehungen definiert werden, indem Sie die Kurzbeschreibung verwenden, die im Artikel Erstellen von Vorgängerbeziehungen beschrieben wird.
* **Dauer festlegen**
Legen Sie die Dauer für jede Aufgabe fest, indem Sie im Feld setDuration die Anzahl der Stunden, Tage, Wochen oder Monate für die Aufgabe eingeben. Geben Sie dann die Zeiteinheit in das Feld setDurationUnit ein.

   |  | Zulässiger Wert |
   |---|---|
   | Minuten | M |
   | Stunden | H |
   | Tage | D |
   | Wochen | M |
   | Monate | D |

   Minuten können auch als Bruchteil einer Stunde dargestellt werden (z. B. Minuten = 5 Stunden)

* Legen Sie den Aufwand für jede Aufgabe im Feld setWorkRequired fest. Geben Sie dann die Arbeitseinheit in das Feld setWorkUnit ein. Wenn der Wert für &quot;Arbeit erforderlich&quot;sich von der Dauer unterscheidet, müssen Sie auch ein A in das Feld setDurationType eingeben.

   | Dauertyp | Akzeptierbarer Wert |
   |---|---|
   | Berechnete Zuweisung | A |
   | Berechnete Arbeit | M |
   | Leistungsgesteuert | D |
   | Einfach | S |

* Geben Sie für jede Aufgabe im Feld setPercentComplete die gesamte Zahlendarstellung des vollständigen Prozentsatzes ein. Dieser Wert sollte nicht das Prozentsymbol (%) enthalten.
* Fügen Sie bei Bedarf eine Beschreibung und weitere Details für jede Aufgabe ein, die Sie erstellen.

   ![](assets/im5-350x35.png)

* Die Spalten setPlannedStartDate und setTaskConstraint werden nicht zum Erstellen der Timeline dieses Projekts verwendet, da wir auf Vorgängerbeziehungen angewiesen sind. Stattdessen können Sie für jede Aufgabe ein Datum eingeben. Stellen Sie in diesem Fall sicher, dass Sie auch eine gültige Aufgabenbegrenzung in der Spalte setTaskConstraint angeben. Weitere Informationen zu gültigen Werten für dieses Feld finden Sie in den Artikeln zur Aufgabenbegrenzung und den zugehörigen .

   In diesem Fall können Sie die Aufgaben für die anderen Projekte, die Sie importieren, am einfachsten erstellen, indem Sie die soeben definierten Aufgaben kopieren und unten einfügen, beginnend mit Zeile 12. Anschließend werden Sie:

   1. Nummerieren Sie die Werte in der ID-Spalte um.
   1. Aktualisieren Sie die Spalte setProjectID auf den Wert, den Sie für das nächste Projekt festgelegt haben.
   1. Aktualisieren Sie die Werte setParentID und setPredecessorString , um die neuen IDs widerzuspiegeln, die den Aufgaben dieses Projekts zugewiesen sind.
   1. Aktualisieren Sie die Aufgabenzuweisungen und den Prozentsatz der Abschlüsse.
   1. Wiederholen Sie diese Schritte für die Aufgaben des nächsten Projekts.

* **Excel-Datei importieren**

   Befolgen Sie die Anweisungen unter [Daten mithilfe einer Kick-Start-Vorlage in Adobe Workfront importieren](../../../administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md).
