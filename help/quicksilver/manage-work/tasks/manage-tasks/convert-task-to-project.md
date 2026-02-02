---
product-area: projects
navigation-topic: manage-tasks
title: Konvertieren einer Aufgabe in ein Projekt
description: Wenn für eine Aufgabe in einem Projekt ein größerer Aufwand erforderlich ist als ursprünglich geplant, können Sie sie in ein Projekt konvertieren.
author: Alina
feature: Work Management
exl-id: a45f0af4-1768-4f20-80d4-912e6fe0fc03
source-git-commit: ef64e5c8169fd0a12d303c17649a20400ccbeb58
workflow-type: tm+mt
source-wordcount: '1152'
ht-degree: 4%

---

# Konvertieren einer Aufgabe in ein Projekt

<!--<div class="preview"> 

The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. The same features will also be available in the Production environment for all customers after a week from the Preview release.      

For more information, see [Interface modernization](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md).  

</div>-->

Wenn für eine Aufgabe in einem Projekt ein größerer Aufwand erforderlich ist als ursprünglich geplant, können Sie sie in ein Projekt konvertieren.

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Paket</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td> <p>Standard</p>
   <p>Plan</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriff auf Aufgaben und Projekte bearbeiten</p> <p>Anzeigen oder höherer Zugriff auf Vorlagen beim Konvertieren in ein Projekt mithilfe einer Vorlage</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Verwalten der Berechtigungen für eine Aufgabe</p> <p>Anzeigen von Berechtigungen für eine Vorlage beim Konvertieren in ein Projekt mithilfe einer Vorlage</p> <p>Nach dem Erstellen des Projekts verfügen Sie über Verwaltungsberechtigungen für das Projekt</p></td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:

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
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Tasks and Projects</p> <p>View or higher access to Templates, when converting to a project using a template</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to a task</p> <p>View permissions on a template, if converting to a project using a template</p> <p>After creating the project, you have Manage permissions to the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Überlegungen zum Konvertieren von Aufgaben in Projekte

* Sie können eine Aufgabe mithilfe einer Vorlage in ein leeres Projekt oder in ein Projekt konvertieren.
* Die ursprüngliche Aufgabe wird gelöscht.
* Alle Teilaufgaben, Probleme und Notizen werden dem neuen Projekt zugeordnet.
* Dokumente, Dokumentversionen und Testsendungen werden in das neue Projekt verschoben.
* Beim Konvertieren einer Aufgabe in ein Projekt gibt es ein Verarbeitungslimit von 5 Minuten. Wenn an die Aufgabe eine große Anzahl von Dokumenten angehängt ist und sie nicht konvertiert werden kann, müssen Sie möglicherweise einige der Dokumente entfernen und erneut versuchen.
* Der Status und der abgeschlossene Prozentsatz aller Teilaufgaben und Probleme werden beibehalten.
* Aufgabenzugewiesene und der Benutzer, der die Aufgabe in das Projekt konvertiert, werden zu freigegebenen Benutzern im Projekt.
* Das Startdatum des Projekts ist auf das Startdatum der Aufgabe festgelegt.
* In der folgenden Tabelle sind die Projektinformationen aufgeführt und es wird angegeben, ob sie von der Vorlage oder von der Aufgabe übertragen werden:

  <table style="table-layout:auto"> 
  <col> 
  <col> 
  <tbody> 
    <tr> 
    <td>Beschreibung</td> 
    <td> <p>Die Beschreibung der Aufgabe wird auf das neue Projekt übertragen. </p> <p> Wenn keine Beschreibung für die Aufgabe vorhanden ist, wird die Beschreibung aus der Vorlage in das Projekt übertragen. </p> <p>Wenn das Feld Beschreibung sowohl für die Aufgabe als auch für die Vorlage leer ist, ist das Feld im Projekt leer. </p> </td> 
    </tr> 
    <tr> 
    <td>Status</td> 
    <td> Für die Gruppe in der Vorlage ausgewählter Standardstatus. Wenn die Vorlage nicht mit der Gruppe verknüpft ist, wird der Projektstatus auf den Standardstatus gesetzt, den der Workfront-Administrator im Bereich Projektvoreinstellungen von Setup festgelegt hat. Weitere Informationen finden Sie <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md">Konfigurieren von systemweiten Projektvoreinstellungen</a>

  Die folgenden Szenarien sind für die Aktualisierung des Projektstatus vorhanden:
  <ul>
    <li> Wenn der Aufgabenstatus „Neu“ ist, wird der Projektstatus auf „Planung“ gesetzt.</li>
    <li> Wenn der Aufgabenstatus „In Bearbeitung“ ist, wird der Projektstatus auf „Aktuell“ gesetzt.</li>
    <li> Wenn der Aufgabenstatus „Abgeschlossen“ ist, wird der Projektstatus auf „Abgeschlossen“ gesetzt.</li></ul>

  </td> 
    </tr> 
    <tr> 
    <td>Priorität</td> 
    <td>Überträgt von der Aufgabe an das Projekt oder von der Vorlage, wenn Sie bei der Konvertierung eine verwenden. </td> 
    </tr> 
    <tr> 
    <td>URL</td> 
    <td> <p>Die URL der Aufgabe wird an das neue Projekt übertragen. </p> <p> Wenn für die Aufgabe keine URL angegeben ist, wird die URL von der Vorlage an das Projekt übertragen. </p> <p>Wenn das URL-Feld sowohl für das Problem als auch für die Vorlage leer ist, ist das Feld im Projekt leer. </p> </td> 
    </tr> 
    <tr> 
    <td>Projektbedingungstyp</td> 
    <td>Übertragungen aus der Vorlage.</td> 
    </tr> 
    <tr> 
    <td>Projektbedingung</td> 
    <td>Entspricht der vom Workfront-Administrator im Bereich Setup festgelegten Standardeinstellung auf Systemebene. Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-projects.md">Festlegen einer benutzerdefinierten Bedingung als Standard für Projekte</a>
    </td> 
    </tr> 
    <tr> 
    <td>Planen ab</td> 
    <td>Übertragungen aus der Vorlage.</td> 
    </tr> 
    <tr> 
    <td>Projekttermine</td> 
    <td> 
      <ul> 
      <li> <p><b>Geplantes Startdatum</b>: Die auf der Arbeitszeit des Vorlagenplans basierende nächstgelegene Arbeitszeit sollte entsprechend der Zeitzone des Vorlagenplans vorab ausgewählt werden. Dieses Feld ist deaktiviert, wenn das Feld Zeitplan ab auf „Von Fertigstellung“ gesetzt ist. </p> </li> 
      <li> <p><b>Geplantes Abschlussdatum</b>: Die auf der Arbeitszeit des Vorlagenplans basierende nächstgelegene Arbeitszeit sollte entsprechend der Zeitzone des Vorlagenplans vorausgewählt werden. Dieses Feld ist deaktiviert, wenn das Feld „Zeitplan ab“ auf „Von Start“ gesetzt ist. </p> </li> 
      </ul> </td> 
    </tr> 
    <tr> 
    <td>Portfolio</td> 
    <td>Übertragungen aus der Vorlage. Andernfalls ist dieses Feld leer.</td> 
    </tr> 
    <tr> 
    <td>Programm</td> 
    <td>Übertragungen aus der Vorlage. Andernfalls ist dieses Feld leer.</td> 
    </tr> 
    <tr> 
    <td>Gruppe</td> 
    <td><p> Die folgenden Szenarien sind vorhanden:</p>
      <ul><li>Wenn während der Konvertierung eine Gruppe angegeben wird, wird diese zur Gruppe des Projekts</li>
      <li>Wenn Sie mithilfe einer Vorlage in ein Projekt konvertieren und die Vorlage eine Gruppe enthält und Sie während der Konvertierung keine Gruppe angeben, wird die Gruppe der Vorlage zur Gruppe des neuen Projekts</li>
      <li> Wenn in der Vorlage keine Gruppe vorhanden ist und Sie während der Konvertierung keine Gruppe angeben, wird die Gruppe des Projekts der ursprünglichen Anfrage zur Gruppe des neuen Projekts</li> </ul>
        </td> 
    </tr> 
    <tr> 
    <td>Firma</td>    
    <td>  Übertragungen aus der Vorlage. Andernfalls ist dieses Feld leer.</td>

  </tr> 
    <tr> 
    <td>Projektbesitzer</td> 
    <td>Übertragungen aus dem Feld Vorlagenbesitzer in der Vorlage. Andernfalls wird sie auf den angemeldeten Benutzer festgelegt, der die Konvertierung durchführt. </td> 
    </tr> 
    <tr> 
    <td>Projektsponsor</td> 
    <td>Übertragungen aus dem Feld Vorlagen-Sponsor auf der Vorlage. Andernfalls ist dieses Feld leer.</td> 
    </tr> 
    <tr> 
    <td>Ressourcenmanager</td> 
    <td>Übertragungen aus der Vorlage. Andernfalls ist dieses Feld leer.</td> 
    </tr> 
    <tr> 
    <td>Einstellungen für die Aufgabe</td> 
    <td>Übertragung aus der Vorlage.</td> 
    </tr> 
    <tr> 
    <td>Problemeinstellungen</td> 
    <td>Übertragung aus der Vorlage. </td> 
    </tr> 
    <tr> 
    <td>Zugriff</td> 
    <td> <p>Übertragungen aus dem Abschnitt Zugriff auf die Vorlage. </p> </td> 
    </tr> 
    <tr> 
    <td>Genehmigungen</td> 
    <td>Übertragung aus der Vorlage. Die mit der Aufgabe verbundenen Genehmigungen werden während der Konvertierung entfernt. </td> 
    </tr> 
  </tbody> 
  </table>


## Konvertieren einer Aufgabe in ein Projekt

1. Wechseln Sie zu der Aufgabe, die Sie in ein Projekt konvertieren möchten.
1. Klicken Sie auf das **Mehr**-Symbol ![Mehr-Symbol](assets/more-icon.png) und dann **In Projekt konvertieren**.
1. Wählen Sie eine der folgenden Optionen aus:

   * **Neues Projekt**, um ein Projekt ohne Vorlage zu erstellen
   * Eine Vorlage im Abschnitt **Aus Vorlagen auswählen**

     ![Dropdown-Menü mit der Option „Aufgabe in Projektvorlage konvertieren“](assets/convert-task-to-project-template-option-dropdown-nwe-350x209.png)

1. Klicken **in** eingeblendeten Benachrichtigung auf „Weiter“.
1. Geben **im Feld „In Projekt**&quot; Folgendes an:

   * **Name**: Benennen Sie Ihr Projekt. Der Standardname ist der Name der Aufgabe. Dies ist ein Pflichtfeld.
   * **Beschreibung**: Beschreiben Sie den Zweck dieses Projekts.
   * (Bedingt) Wenn Sie ausgewählt haben, ein Projekt aus einer Vorlage zu erstellen, aktualisieren Sie die verfügbaren Felder im Feld **In Projekt konvertieren**.

     Weitere Informationen zum Bearbeiten von Feldern in Projekten finden Sie unter [Projekte bearbeiten](../../../manage-work/projects/manage-projects/edit-projects.md).

     >[!TIP]
     >
     >Um Felder im Abschnitt Finanzen im Feld In Projekt konvertieren zu aktualisieren, benötigen Sie Bearbeitungszugriff auf Finanzdaten in Ihrer Zugriffsebene. Wenn Sie auf Ihrer Zugriffsebene Ansichtszugriff auf Finanzdaten haben, werden alle Finanzinformationen aus der Vorlage an das neue Projekt übertragen und können nicht bearbeitet werden, während Sie das Problem konvertieren. Weitere Informationen finden Sie unter [Zugriff auf Finanzdaten gewähren](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md) und [Vorlage freigeben](../../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md).

   * (Optional) Fügen Sie **Benutzerdefinierte Forms** zum neuen Projekt hinzu.

     >[!TIP]
     >
     >Wenn ein benutzerdefiniertes Formular mit mehreren Objekten, das an die Aufgabe angehängt ist, für die Verwendung sowohl mit Aufgaben als auch mit Projekten konfiguriert ist, werden alle im Formular gespeicherten Informationen beibehalten, wenn Sie die Konvertierung durchführen.
     >
     >
     >Wenn Sie eine Vorlage für die Konvertierung verwenden und ein benutzerdefiniertes Formular, das an die Vorlage angehängt ist, ein benutzerdefiniertes Feld enthält, das auch in einem benutzerdefinierten Formular zu finden ist, das an die Aufgabe angehängt ist, wird der Feldwert aus der Aufgabe für das neue Projekt verwendet. Wenn das benutzerdefinierte Feld bei der Aufgabe jedoch leer ist, wird der Wert aus der Vorlage verwendet.

1. Klicken Sie **In Projekt konvertieren**.
