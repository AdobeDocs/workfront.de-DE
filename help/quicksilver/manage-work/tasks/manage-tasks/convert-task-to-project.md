---
product-area: projects
navigation-topic: manage-tasks
title: Konvertieren einer Aufgabe in ein Projekt
description: Wenn eine Aufgabe in einem Projekt einen größeren Aufwand erfordert, als Sie ursprünglich geplant haben, können Sie sie in ein Projekt konvertieren.
author: Alina
feature: Work Management
exl-id: a45f0af4-1768-4f20-80d4-912e6fe0fc03
source-git-commit: b781687b175167784367a2fdec158d97fb3fd6a4
workflow-type: tm+mt
source-wordcount: '1142'
ht-degree: 2%

---

# Konvertieren einer Aufgabe in ein Projekt

Wenn eine Aufgabe in einem Projekt einen größeren Aufwand erfordert, als Sie ursprünglich geplant haben, können Sie sie in ein Projekt konvertieren.

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
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf Aufgaben und Projekte bearbeiten</p> <p>Beim Konvertieren in ein Projekt mithilfe einer Vorlage Zugriff auf Vorlagen anzeigen oder höher</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Berechtigungen für eine Aufgabe verwalten</p> <p>Anzeigen von Berechtigungen für eine Vorlage beim Konvertieren in ein Projekt mithilfe einer Vorlage</p> <p>Nach dem Erstellen des Projekts verfügen Sie über Verwaltungsberechtigungen für das Projekt</p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Überlegungen zum Konvertieren von Aufgaben in Projekte

* Sie können eine Aufgabe mithilfe einer Vorlage in ein leeres Projekt oder in ein Projekt konvertieren.
* Die ursprüngliche Aufgabe wird gelöscht.
* Alle Unteraufgaben, Probleme und Hinweise werden in das neue Projekt übernommen.
* Dokumente, Dokumentversionen und Testsendungen werden in das neue Projekt verschoben.
* Status und prozentualer Abschluss aller Unteraufgaben und Probleme bleiben erhalten.
* Freigegebene Benutzer der Aufgabe werden zu freigegebenen Benutzern im Projekt.
* Das Projektstartdatum wird auf das Anfangsdatum der Aufgabe festgelegt.
* In der folgenden Tabelle sind die Projektinformationen aufgeführt und es wird angegeben, ob sie von der Vorlage oder von der Aufgabe übertragen werden:

  <table style="table-layout:auto"> 
  <col> 
  <col> 
  <tbody> 
    <tr> 
    <td>Beschreibung</td> 
    <td> <p>Die Beschreibung der Aufgabe wird an das neue Projekt übertragen. </p> <p> Wenn es keine Beschreibung für die Aufgabe gibt, wird die Beschreibung aus der Vorlage an das Projekt übertragen. </p> <p>Wenn das Feld Beschreibung sowohl für die Aufgabe als auch für die Vorlage leer ist, ist das Feld im Projekt leer. </p> </td> 
    </tr> 
    <tr> 
    <td>Status</td> 
    <td> Standardstatus, der für die Gruppe in der Vorlage ausgewählt wird. Wenn die Vorlage nicht mit der Gruppe verknüpft ist, wird der Projektstatus vom Workfront-Administrator im Bereich "Projekteinstellungen"des Setups auf den Standardstatus festgelegt. Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md">Systemweite Projektvoreinstellungen konfigurieren</a>

  Es gibt die folgenden Szenarien, um den Status des Projekts zu aktualisieren:
  <ul>
    <li> Wenn der Aufgabenstatus "Neu"lautet, wird der Projektstatus auf "Planung"festgelegt.</li>
    <li> Wenn die Aufgabe den Status "Wird ausgeführt"hat, wird der Projektstatus auf "Aktuell"gesetzt.</li>
    <li> Wenn der Aufgabenstatus "Abgeschlossen"lautet, wird der Projektstatus auf "Abgeschlossen"gesetzt.</li></ul>

  </td> 
    </tr> 
    <tr> 
    <td>Priorität</td> 
    <td>Überträgt von der Aufgabe zum Projekt oder von der Vorlage, wenn Sie eine in der Konvertierung verwenden. </td> 
    </tr> 
    <tr> 
    <td>URL</td> 
    <td> <p>Die URL der Aufgabe wird an das neue Projekt übertragen. </p> <p> Wenn für die Aufgabe keine URL angegeben ist, wird die URL aus der Vorlage an das Projekt übertragen. </p> <p>Wenn das Feld URL sowohl für das Problem als auch für die Vorlage leer ist, ist das Feld im Projekt leer. </p> </td> 
    </tr> 
    <tr> 
    <td>Projektbedingungstyp</td> 
    <td>Übertragungen aus der Vorlage.</td> 
    </tr> 
    <tr> 
    <td>Projektbedingung</td> 
    <td>Entspricht den Standardeinstellungen auf Systemebene, die vom Workfront-Administrator im Bereich "Setup"festgelegt wurden. Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-projects.md">Festlegen einer benutzerdefinierten Bedingung als Standard für Projekte</a>
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
      <li> <p><b>Geplantes Startdatum</b>: Die nächstgelegene Arbeitszeit, die auf der Arbeitszeit des Vorlagenzeitplans basiert, sollte entsprechend der Zeitzone des Zeitplans der Vorlage vorausgewählt werden. Dieses Feld ist deaktiviert, wenn im Feld Planen von die Option Aus Abschluss ausgewählt ist. </p> </li> 
      <li> <p><b>Geplantes Abschlussdatum</b>: Die nächstgelegene Arbeitszeit, die auf der Arbeitszeit des Vorlagenzeitplans basiert, sollte entsprechend der Zeitzone des Zeitplans der Vorlage vorausgewählt werden. Dieses Feld ist deaktiviert, wenn im Feld Planung von die Option Von Start ausgewählt ist. </p> </li> 
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
    <td><p> Die folgenden Szenarien existieren:</p>
      <ul><li>Wenn während der Konvertierung eine Gruppe angegeben wird, wird dies zur Gruppe des Projekts</li>
      <li>Wenn Sie mithilfe einer Vorlage in ein Projekt konvertieren und sich in der Vorlage eine Gruppe befindet und während der Konvertierung keine Gruppe angegeben wird, wird die Gruppe der Vorlage zur Gruppe des neuen Projekts</li>
      <li> Wenn keine Gruppe in der Vorlage vorhanden ist und Sie während der Konvertierung keine Gruppe angeben, wird die Gruppe des Projekts des ursprünglichen Problems zur Gruppe des neuen Projekts</li> </ul>
        </td> 
    </tr> 
    <tr> 
    <td>Firma</td>    
    <td>  Übertragungen aus der Vorlage. Andernfalls ist dieses Feld leer.</td>

  </tr> 
    <tr> 
    <td>Projektbesitzer</td> 
    <td>Übertragungen aus dem Feld Vorlageneigentümer in der Vorlage. Andernfalls wird er auf den angemeldeten Benutzer festgelegt, der die Konvertierung durchführt. </td> 
    </tr> 
    <tr> 
    <td>Projektsponsor</td> 
    <td>Übertragungen aus dem Feld "Vorlagen-Sponsor"auf der Vorlage. Andernfalls ist dieses Feld leer.</td> 
    </tr> 
    <tr> 
    <td>Ressourcenmanager</td> 
    <td>Übertragungen aus der Vorlage. Andernfalls ist dieses Feld leer.</td> 
    </tr> 
    <tr> 
    <td>Einstellungen für die Aufgabe</td> 
    <td>Aus der Vorlage übertragen.</td> 
    </tr> 
    <tr> 
    <td>Problemeinstellungen</td> 
    <td>Aus der Vorlage übertragen. </td> 
    </tr> 
    <tr> 
    <td>Zugriff</td> 
    <td> <p>Übertragungen aus dem Bereich Zugriff auf der Vorlage. </p> </td> 
    </tr> 
    <tr> 
    <td>Genehmigungen</td> 
    <td>Aus der Vorlage übertragen. Die mit der Aufgabe verknüpften Genehmigungen werden während der Konvertierung entfernt. </td> 
    </tr> 
  </tbody> 
  </table>


## Konvertieren einer Aufgabe in ein Projekt

1. Wechseln Sie zu der Aufgabe, die Sie in ein Projekt konvertieren möchten.
1. Klicken Sie auf **Mehr** icon ![](assets/more-icon.png), dann **In Projekt konvertieren**.
1. Wählen Sie eine der folgenden Optionen aus:

   * **Neues Projekt**
   * Eine Vorlage im **Aus Vorlagen auswählen** Abschnitt

     ![](assets/convert-task-to-project-template-option-dropdown-nwe-350x209.png)

1. Klicks **Weiter** auf der angezeigten Benachrichtigung.
1. Im **In Projekt konvertieren** Geben Sie Folgendes an:

   * **Name**: Benennen Sie Ihr Projekt. Der Standardname ist der Name der Aufgabe.
   * (Optional) **Beschreibung**: Beschreiben Sie den Zweck dieses Projekts.
   * (Optional und bedingt) Wenn Sie ein Projekt aus einer Vorlage erstellen möchten, aktualisieren Sie die verfügbaren Felder im **In Projekt konvertieren** Dialogfeld.

     Weitere Informationen zum Bearbeiten von Feldern in Projekten finden Sie unter [Projekte bearbeiten](../../../manage-work/projects/manage-projects/edit-projects.md).

     >[!TIP]
     >
     >Um die Felder im Abschnitt Finanzen im Feld In Projekt konvertieren zu aktualisieren, müssen Sie in Ihrer Zugriffsebene Zugriff auf Finanzdaten bearbeiten haben. Wenn Sie auf Ihrer Zugriffsebene Zugriff auf Finanzdaten anzeigen haben, werden alle Finanzinformationen aus der Vorlage an das neue Projekt übertragen und Sie können sie nicht bearbeiten, während Sie das Problem konvertieren. Weitere Informationen finden Sie unter [Zugriff auf Finanzdaten gewähren](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md) und [Vorlage freigeben](../../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md).

   * (Optional) Hinzufügen **Benutzerdefinierte Forms** zum neuen Projekt.

     >[!TIP]
     >
     Wenn ein benutzerdefiniertes Formular mit mehreren Objekten, das an die Aufgabe angehängt ist, für die Verwendung mit Aufgaben und Projekten konfiguriert ist, werden alle im Formular gespeicherten Informationen bei der Konvertierung beibehalten.
     >
     >
     Wenn Sie eine Vorlage für die Konvertierung verwenden und ein benutzerdefiniertes Formular, das an die Vorlage angehängt ist, ein benutzerdefiniertes Feld enthält, das auch in einem benutzerdefinierten Formular enthalten ist, das an die Aufgabe angehängt ist, wird der Feldwert der Aufgabe für das neue Projekt verwendet. Wenn das benutzerdefinierte Feld jedoch für die Aufgabe leer ist, wird der Wert aus der Vorlage verwendet.

1. Klicks **Änderungen speichern**.
