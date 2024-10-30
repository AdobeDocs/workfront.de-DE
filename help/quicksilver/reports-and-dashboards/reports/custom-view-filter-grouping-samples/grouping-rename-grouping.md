---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: "Gruppierung: Anzeigename in einer Gruppierung bearbeiten"
description: Sie können Gruppierungen in Listen und Berichten so umbenennen, dass sie Ihren Benutzern besser bekannt sind.
author: Nolan
feature: Reports and Dashboards
exl-id: 072d3c2b-9ede-4bb9-9a27-dc77ceb732c4
source-git-commit: a6874c3a2dfda02b8a25f78056767d8c59c888e9
workflow-type: tm+mt
source-wordcount: '350'
ht-degree: 0%

---

# Gruppierung: Anzeige in einer Gruppierung gruppieren

<!--Audited: 01/2024-->

Sie können Gruppierungen so umbenennen, dass sie Ihren Benutzern besser bekannt sind.

Wenn Sie beispielsweise die Standardgruppierung Projektname auf eine Projektliste anwenden, wird der Gruppierungsname als *Portfolio: Portfolio:`<name of portfolio>`* angezeigt.

![](assets/grouping-unedited-name-350x167.png)

Sie können diese Gruppierung mithilfe des Textmodus ändern, um einen leichter lesbaren Namen anzuzeigen.

![](assets/grouping-edited-name-350x160.png)

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Abo</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> 
    <p>Neu:</p>
   <ul><li><p>Mitwirkende bei der Änderung eines Filters </p></li>
   <li><p>Standard zum Ändern eines Berichts</p></li> </ul>

<p>Aktuell:</p>
   <ul><li><p>Filteranforderung </p></li>
   <li><p>Berichtänderung planen</p></li> </ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Zugriff auf Berichte, Dashboards und Kalender bearbeiten, um einen Bericht zu ändern</p> <p>Zugriff auf Filter, Ansichten und Gruppierungen bearbeiten, um einen Filter zu ändern</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Berechtigungen für einen Bericht verwalten</p>  </td> 
  </tr> 
 </tbody> 
</table>

*Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Anzeigenamen in einer Gruppierung bearbeiten

So ändern Sie den Anzeigenamen in einer Projektgruppe:

1. Gehen Sie zu einer Projektliste.
1. Wählen Sie aus dem Dropdownmenü **Gruppierung** die Option **Neue Gruppierung** aus.

1. Klicken Sie auf **Gruppierung hinzufügen**, geben Sie im Feld **Gruppieren nach:** den Wert &quot;Portfolio-Name&quot;ein und wählen Sie ihn aus, wenn er in der Liste angezeigt wird.

1. Klicken Sie auf **Wechseln zum Textmodus**.
1. Führen Sie einen der folgenden Schritte aus:

   * Fügen Sie den folgenden Code zum vorhandenen Text hinzu, der im Feld **Gruppieren Ihres Berichts** verfügbar ist:


     `group.0.displayname=Your Value`


     Fügen Sie beispielsweise den folgenden Code hinzu, um den Anzeigenamen in &quot;Portfolio&quot;zu ändern:

     `group.0.displayname=Portfolio`

   * Entfernen Sie alle Zeilen in der Textmodus-Benutzeroberfläche der Gruppierung, die das Wort &quot;name&quot;enthalten, und fügen Sie dann die Zeile hinzu:

     `group.0.name=Your Value`

     Fügen Sie beispielsweise den folgenden Code hinzu, um den Anzeigenamen in &quot;Portfolio&quot;zu ändern:

     `group.0.name=Portfolio`

     >[!TIP]
     >
     >Sie können auch die Zeilen `group.0.name=` und `group.0.displayname=` leer lassen. In diesem Fall zeigt die Gruppierung den Wert an, nach dem Sie gruppieren.


     ![](assets/grouping-edited-name-no-name-350x162.png)

1. Klicken Sie auf **Fertig** und dann auf **Gruppierung speichern**.
1. (Optional) Aktualisieren Sie den Gruppierungsnamen und klicken Sie dann auf **Gruppierung speichern**.

   Der Standardname für die Gruppierung wird entsprechend Ihren Textmodusinformationen geändert.
