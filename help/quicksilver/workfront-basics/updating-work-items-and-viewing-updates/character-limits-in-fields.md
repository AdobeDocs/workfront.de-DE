---
content-type: reference
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: Zeichenbeschränkungen in Feldern
description: Bestimmte Felder in Adobe Workfront beschränken die Anzahl der Zeichen, die in das Feld aufgenommen werden können. Workfront indiziert Inhalte, damit sie zu einem späteren Zeitpunkt durchsucht werden können. Eine Zeichenbeschränkung wird durchgesetzt, um eine hohe Leistung des Workfront-Systems zu gewährleisten.
author: Alina
feature: Get Started with Workfront
exl-id: f09dadf4-24f2-46d9-85ae-6081731d917d
source-git-commit: e2a2a8cfe402c1f9f810ca360db4912d804b0a57
workflow-type: tm+mt
source-wordcount: '250'
ht-degree: 5%

---

# Zeichenbeschränkungen in Feldern

Bestimmte Felder in Adobe Workfront beschränken die Anzahl der Zeichen, die in das Feld aufgenommen werden können. Workfront indiziert Inhalte, damit sie zu einem späteren Zeitpunkt durchsucht werden können. Eine Zeichenbeschränkung wird durchgesetzt, um eine hohe Leistung des Workfront-Systems zu gewährleisten.

Wenn Sie sich dem Limit nähern, wird ein Zähler angezeigt. Wenn Sie das Limit überschreiten, werden überschüssige Zeichen hervorgehoben und Sie können den Text nicht veröffentlichen. Löschen Sie Zeichen, bis Sie das zulässige Limit erreicht haben.

Die Zeichenbeschränkung unterscheidet sich je nach verwendetem Feld. Die unten aufgeführten Beschränkungen gelten für Sprachen, die ein lateinisches Alphabet verwenden (z. B. Englisch). Der Grenzwert kann für Sprachen, die erweiterte Zeichen oder Doppelbyte-Zeichen enthalten, niedriger sein.

Workfront- oder Gruppenadministratoren können die Zeichenbeschränkungen in Feldern nicht ändern.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Feldtyp</strong> </p> </th> 
   <th> <p><strong>Zeichenbeschränkung (</strong><strong> Leerzeichen)</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Textfeld mit Formatierung in einem benutzerdefinierten Formular</td> 
   <td>15.000</td> 
  </tr> 
  <tr> 
   <td> <p>Status-Update</p> </td> 
   <td> <p>15.000</p>
   <p> 4.000 bei Verwendung der API</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aktualisieren</p> </td> 
   <td> <p>15.000</p> 
   <p> 4.000 bei Verwendung der API</p></td> 
  </tr> 
  <tr> 
   <td> <p>Beschreibung (Dokumente, Aufgaben, Probleme, Portfolios, Programme und Projekte)</p> </td> 
   <td> <p>4.000</p> </td> 
  </tr> 
  <tr> 
   <td>Beschreibungsfeld in einem benutzerdefinierten Formular</td> 
   <td>4.000</td> 
  </tr> 
  <tr> 
   <td> <p>Benutzerdefinierter Datenabsatz oder einzeiliger Text </p> </td> 
   <td> <p>2.000</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Beschreibungsfeld im Report Builder</p> </td> 
   <td> <p>512</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Dropdown-Menübezeichnung</p> </td> 
   <td> <p>255</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Objektname</p> </td> 
   <td> <p>255</p> </td> 
  </tr> 
 </tbody> 
</table>
