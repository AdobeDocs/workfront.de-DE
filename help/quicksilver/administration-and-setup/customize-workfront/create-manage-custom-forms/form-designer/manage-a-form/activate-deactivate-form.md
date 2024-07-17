---
title: Deaktivieren oder reaktivieren Sie ein benutzerdefiniertes Formular
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: Sie können ein benutzerdefiniertes Formular reaktivieren oder deaktivieren. Es wird empfohlen, benutzerdefinierte Formulare zu deaktivieren, anstatt Formulare zu löschen, die Sie nicht mehr verwenden, um historische Daten beizubehalten.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 6d9a409d-8d16-4c58-ad02-f60aa1ac1714
source-git-commit: 35de4535970d5cd15fcd68f79bf849803f94a77e
workflow-type: tm+mt
source-wordcount: '356'
ht-degree: 0%

---

# Deaktivieren oder reaktivieren Sie ein benutzerdefiniertes Formular

Sie können ein benutzerdefiniertes Formular reaktivieren oder deaktivieren. Es wird empfohlen, benutzerdefinierte Formulare zu deaktivieren, anstatt Formulare zu löschen, die Sie nicht mehr verwenden, um historische Daten beizubehalten.

>[!NOTE]
>
>Wenn ein benutzerdefiniertes Formular deaktiviert ist, aber weiterhin Teil eines Warteschlangenthemas oder einer Anforderungswarteschlangendefinition ist, wird es an neue Anforderungen angehängt. Wenn das Formular nicht in den Anforderungen enthalten sein soll, müssen Sie es manuell aus der Anforderungswarteschlange entfernen.

## Zugriffsanforderungen

Sie müssen über Folgendes verfügen, um die Schritte in diesem Artikel durchzuführen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Adobe Workfront-Abo</p> </td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td>
   <p>Neu: Standard</p>
   <p>oder</p>
   <p>Aktuell: Plan</p></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Administratorzugriff auf benutzerdefinierte Formulare</p></td> 
  </tr>  
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Deaktivieren eines benutzerdefinierten Formulars

Sie können nicht mehr verwendete benutzerdefinierte Formulare deaktivieren, ohne die zugehörigen historischen Daten zu verlieren. Benutzer können Objekten zwar kein inaktives benutzerdefiniertes Formular hinzufügen, sie können jedoch trotzdem Daten zu Objekten, an denen es bereits angehängt war, anzeigen und zu ihren Feldern hinzufügen.

Felder in einem inaktiven benutzerdefinierten Formular können auch in einer Ansicht inline bearbeitet werden. Wenn ein Benutzer während einer Inline-Bearbeitung ein Feld aus einem inaktiven benutzerdefinierten Formular hinzufügt, wird das Formular automatisch an das Objekt angehängt, auch wenn das benutzerdefinierte Formular deaktiviert ist.

So deaktivieren Sie ein benutzerdefiniertes Formular:

{{step-1-to-setup}}

1. Wählen Sie im linken Bereich **Benutzerdefinierter Forms** aus.
1. Wählen Sie im Bereich **Forms** das benutzerdefinierte Formular aus, das Sie deaktivieren möchten.
1. Wählen Sie in der Spalte Ist aktiv die Option **False** aus und klicken Sie aus der Spalte. Das Formular ist nicht mehr aktiv.

## Benutzerdefiniertes Formular erneut aktivieren

Wenn Sie ein benutzerdefiniertes Formular reaktivieren, werden die zuvor vorhandenen Einstellungen beibehalten und die Benutzer können mit dem Formular so interagieren, als wäre es nie deaktiviert.

{{step-1-to-setup}}

1. Wählen Sie im linken Bereich **Benutzerdefinierter Forms** aus.
1. Wählen Sie im Bereich **Forms** das benutzerdefinierte Formular aus, das Sie reaktivieren möchten.
1. Wählen Sie in der Spalte Ist aktiv die Option **True** aus und klicken Sie aus der Spalte. Das Formular ist jetzt aktiv.
