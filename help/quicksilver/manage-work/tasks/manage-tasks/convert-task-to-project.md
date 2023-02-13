---
product-area: projects
navigation-topic: manage-tasks
title: Konvertieren einer Aufgabe in ein Projekt
description: Wenn eine Aufgabe in einem Projekt einen größeren Aufwand erfordert, als Sie ursprünglich geplant haben, können Sie sie in ein Projekt konvertieren.
author: Alina
feature: Work Management
exl-id: a45f0af4-1768-4f20-80d4-912e6fe0fc03
source-git-commit: dd7f61fcd92a43303be356dd3209ec6da6a063dd
workflow-type: tm+mt
source-wordcount: '602'
ht-degree: 0%

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

* Die ursprüngliche Aufgabe wird gelöscht.
* Aufgabengenehmigungen werden gelöscht.
* Alle Unteraufgaben, Probleme und Hinweise werden in das neue Projekt übernommen.
* Dokumente, Dokumentversionen und Testsendungen werden in das neue Projekt verschoben.
* Status und prozentualer Abschluss aller Unteraufgaben und Probleme bleiben erhalten.
* Freigegebene Benutzer der Aufgabe werden zu freigegebenen Benutzern im Projekt.
* Das Projektstartdatum wird auf das Anfangsdatum der Aufgabe festgelegt.
* Wenn der Aufgabenstatus &quot;Neu&quot;lautet, wird der Projektstatus auf &quot;Planung&quot;festgelegt.
* Wenn die Aufgabe den Status &quot;Wird ausgeführt&quot;hat, wird der Projektstatus auf &quot;Aktuell&quot;gesetzt.
* Wenn der Aufgabenstatus &quot;Abgeschlossen&quot;lautet, wird der Projektstatus auf &quot;Abgeschlossen&quot;gesetzt.

## Konvertieren einer Aufgabe in ein Projekt

1. Wechseln Sie zu der Aufgabe, die Sie in ein Projekt konvertieren möchten.
1. Klicken Sie auf **Mehr** icon ![](assets/more-icon.png), dann **In Projekt konvertieren**.
1. Wählen Sie eine der folgenden Optionen aus:

   * **Neues Projekt**
   * Eine Vorlage im **Aus Vorlagen auswählen** Abschnitt

      ![](assets/convert-task-to-project-template-option-dropdown-nwe-350x209.png)

1. Klicken **Weiter** auf der angezeigten Benachrichtigung.
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
      Wenn ein benutzerdefiniertes Formular mit mehreren Objekten, das an die Aufgabe angehängt ist, für die Verwendung mit Aufgaben und Projekten konfiguriert ist, werden alle im Formular gespeicherten Informationen bei der Konvertierung beibehalten.
      Wenn Sie eine Vorlage für die Konvertierung verwenden und ein benutzerdefiniertes Formular, das an die Vorlage angehängt ist, ein benutzerdefiniertes Feld enthält, das auch in einem benutzerdefinierten Formular enthalten ist, das an die Aufgabe angehängt ist, wird der Feldwert der Aufgabe für das neue Projekt verwendet. Wenn das benutzerdefinierte Feld jedoch für die Aufgabe leer ist, wird der Wert aus der Vorlage verwendet.

1. Klicken **Änderungen speichern**.
