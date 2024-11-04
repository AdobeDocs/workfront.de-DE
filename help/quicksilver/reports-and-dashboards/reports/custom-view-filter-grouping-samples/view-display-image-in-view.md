---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: "Ansicht: Anzeigen eines Bildes anstelle einer Zeichenfolge in einer Spalte"
description: Sie können den Namen eines Objekts in einer Ansicht mithilfe des Textmodus durch ein Bild ersetzen. Sie können auch einen Link zum Bild hinzufügen, der das von ihm ersetzte Objekt öffnen kann.
author: Nolan
feature: Reports and Dashboards
exl-id: e1e4a993-f05c-4b6e-b00a-e96c9ab4c94f
source-git-commit: ecce7484423419823effa2cb41da892ba3fb207c
workflow-type: tm+mt
source-wordcount: '488'
ht-degree: 0%

---

# Ansicht: Anzeigen eines Bildes anstelle einer Zeichenfolge in einer Spalte

<!--Audited: 11/2024-->

Sie können den Namen eines Objekts in einer Ansicht mithilfe des Textmodus durch ein Bild ersetzen. Sie können auch einen Link zum Bild hinzufügen, der das von ihm ersetzte Objekt öffnen kann.

>[!NOTE]
>
>Bilder werden in ihrer tatsächlichen Auflösung angezeigt, daher versuchen Sie, kleine Bilder zu verwenden.

![](assets/replace-project-name-with-image-and-link-350x125.png)

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

## Beispiel: Ersetzen Sie den Namen eines Projekts in einer Projektansicht durch ein Bild:

1. Laden Sie ein Bild auf eine Website oder einen Server hoch, der außerhalb von Adobe Workfront liegt. Sie müssen über Ihren Webbrowser auf das Bild zugreifen können.

   >[!TIP]
   >
   >* Jeder Browsertyp unterscheidet sich, doch alle sind in der Lage, URLs anzuzeigen.
   >* Vermeiden Sie die Verwendung von Bildern, die in Workfront hochgeladen werden. Da in Workfront gespeicherte Bilder nicht öffentlich verfügbar sind und einen Zugriffsschlüssel haben, der nach einem bestimmten Zeitraum abläuft, werden diese Bilder nicht mehr in der Ansicht angezeigt.
   >* Ein auf Ihrem Computer gespeichertes Bild hat keine inhärente URL. Suchen Sie eine Site, die Bild-Hosting bereitstellt und Ihr Bild dort hosten. Möglicherweise verfügt Ihr Unternehmen bereits über eine solche Website.

1. Rufen Sie mit Ihrem Webbrowser das Bild auf, das Sie gespeichert haben.
1. Rufen Sie die URL des Bildes wie folgt ab:

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: I used this blog post to document what kind of image we need for this: https://www.canto.com/blog/image-url/ (consulting uses this)) </p>
   -->

   1. Klicken Sie mit der rechten Maustaste und wählen Sie je nach Browser **Speicherort des Bildes kopieren** oder **Link abrufen** aus. Sie verfügen nun über die URL für dieses spezifische Bild und können es aus der Zwischenablage einfügen.
   1. Stellen Sie sicher, dass alle Benutzer mit diesem Link berechtigt sind, das Bild anzuzeigen, indem Sie einfach zum Link navigieren, und sie keine Anmeldung benötigen, um darauf zuzugreifen.

1. Wechseln Sie zu einem Projekt, klicken Sie auf das Menü **Mehr** neben dem Namen des Projekts und klicken Sie dann auf **Bearbeiten**.![](assets/more-icon-45x33.png)

1. Fügen Sie im Feld **URL** den Link zum Bild hinzu.
1. Wechseln Sie in einer Projektliste zu einer Projektansicht.
1. Klicken Sie auf das Dropdownmenü **Ansicht** und dann auf **Neue Ansicht**.
1. Klicken Sie auf die Kopfzeile der Spalte für den **Projektnamen** und dann auf **Wechseln zum Textmodus**.

1. Fügen Sie der Spalte den folgenden Code zum vorhandenen Code hinzu:

   ```
   displayname=Link Project
   image.name=Link Project
   image.valuefield=URL
   link.linkproperty.0.name=projectID
   link.linkproperty.0.value=ID
   link.lookup=link.edit
   link.page=/view
   link.valuefield=objCode
   link.valueformat=val
   textmode=true
   type=image
   valueformat=
   ```

1. Klicken Sie auf **Fertig** > **Ansicht speichern**.
Das ausgewählte Bild ersetzt den Projektnamen in der Projektansicht und das Bild ist ein Link zum Projekt.