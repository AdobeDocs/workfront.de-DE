---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Gruppierung: Anzeigenamen in einer Gruppierung bearbeiten'
description: Sie können Gruppierungen in Listen und Berichten umbenennen, um sie Ihren Benutzern bekannter zu machen.
author: Nolan
feature: Reports and Dashboards
exl-id: 072d3c2b-9ede-4bb9-9a27-dc77ceb732c4
source-git-commit: 70bda5a7186abfa7e8cbd26e25a4c58583a322b4
workflow-type: tm+mt
source-wordcount: '365'
ht-degree: 0%

---

# Gruppierung: Anzeigenamen in einer Gruppierung bearbeiten

<!--Audited: 01/2024-->

Sie können Gruppierungen umbenennen, damit sie Ihren Benutzern vertrauter sind.

Wenn Sie beispielsweise die standardmäßige Gruppierung Portfolio-Name auf eine Liste von Projekten anwenden, wird der Name der Gruppierung als *Portfolio: Name:`<name of portfolio>`* angezeigt.

![Gruppierung nach nicht bearbeitetem Namen](assets/grouping-unedited-name-350x167.png)

Sie können diese Gruppierung im Textmodus ändern, um einen leichter lesbaren Namen anzuzeigen.

![Gruppieren nach bearbeitetem Namen](assets/grouping-edited-name-350x160.png)

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

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
   <td> 
    <p>Neu:</p>
   <ul><li><p>Mitwirkender zum Ändern eines Filters </p></li>
   <li><p>Standard zum Ändern eines Berichts</p></li> </ul>

<p>Aktuell:</p>
   <ul><li><p>Filter ändern </p></li>
   <li><p>Planen der Änderung eines Berichts</p></li> </ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriff auf Berichte, Dashboards und Kalender bearbeiten, um einen Bericht zu ändern</p> <p>Zugriff auf Filter, Ansichten, Gruppierungen bearbeiten, um einen Filter zu ändern</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Verwalten von Berechtigungen für einen Bericht</p>  </td> 
  </tr> 
 </tbody> 
</table>

*Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Anzeigenamen in einer Gruppierung bearbeiten

So ändern Sie den Anzeigenamen in einer Projektgruppierung:

1. Zu einer Projektliste gehen.
1. Wählen Sie **Dropdown-Menü** Gruppierung“ **Neue Gruppierung** aus.

1. Klicken Sie auf **Gruppierung hinzufügen** und geben Sie &quot;Portfolio-Name“ in das Feld **Gruppieren nach:** ein. Wählen Sie es aus, wenn es in der Liste angezeigt wird.

1. Klicken Sie **In Textmodus wechseln**.
1. Führen Sie einen der folgenden Schritte aus:

   * Fügen Sie den folgenden Code zum vorhandenen Text hinzu, der im Feld **Bericht gruppieren** verfügbar ist:


     `group.0.displayname=Your Value`


     Fügen Sie beispielsweise den folgenden Code hinzu, um den Anzeigenamen in &quot;Portfolio&quot; zu ändern:

     `group.0.displayname=Portfolio`

   * Entfernen Sie alle Zeilen in der Textmodusschnittstelle der Gruppierung, die das Wort „Name“ enthalten, und fügen Sie dann die Zeile hinzu:

     `group.0.name=Your Value`

     Fügen Sie beispielsweise den folgenden Code hinzu, um den Anzeigenamen in &quot;Portfolio&quot; zu ändern:

     `group.0.name=Portfolio`

     >[!TIP]
     >
     >Sie können die `group.0.name=` und die `group.0.displayname=` auch leer lassen. In diesem Fall zeigt die Gruppierung den Wert an, nach dem gruppiert werden soll.


     ![Gruppierung nach bearbeitetem Namen ohne Namen](assets/grouping-edited-name-no-name-350x162.png)

1. Klicken Sie **Fertig** und dann **Gruppierung speichern**.
1. (Optional) Aktualisieren Sie den Gruppierungsnamen und klicken Sie dann auf **Gruppierung speichern**.

   Der Standardname für die Gruppierung wird entsprechend Ihren Textmodusinformationen geändert.
