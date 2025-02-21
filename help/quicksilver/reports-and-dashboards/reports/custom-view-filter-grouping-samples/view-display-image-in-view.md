---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Ansicht: Anzeigen eines Bildes anstelle einer Zeichenfolge in einer Spalte'
description: Sie können den Namen eines Objekts in einer Ansicht mit einem Bild im Textmodus ersetzen. Sie können dem Bild auch einen Link hinzufügen, mit dem das ersetzte Objekt geöffnet werden kann.
author: Nolan
feature: Reports and Dashboards
exl-id: e1e4a993-f05c-4b6e-b00a-e96c9ab4c94f
source-git-commit: 70bda5a7186abfa7e8cbd26e25a4c58583a322b4
workflow-type: tm+mt
source-wordcount: '497'
ht-degree: 0%

---

# Anzeigen : Ein Bild anstelle einer Zeichenfolge in einer Spalte anzeigen

<!--Audited: 11/2024-->

Sie können den Namen eines Objekts in einer Ansicht mit einem Bild im Textmodus ersetzen. Sie können dem Bild auch einen Link hinzufügen, mit dem das ersetzte Objekt geöffnet werden kann.

>[!NOTE]
>
>Bilder erscheinen in der tatsächlichen Auflösung. Versuchen Sie daher, kleine Bilder zu verwenden.

![Projektname durch Bild und Link ersetzen](assets/replace-project-name-with-image-and-link-350x125.png)

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

## Beispiel: Ersetzen Sie den Namen eines Projekts in einer Projektansicht durch ein Bild:

1. Laden Sie ein Bild auf eine Website oder einen externen Server von Adobe Workfront hoch. Sie müssen in der Lage sein, über Ihren Webbrowser auf das Bild zuzugreifen.

   >[!TIP]
   >
   >* Jeder Browser-Typ ist anders, aber alle Browser können URLs anzeigen.
   >* Vermeiden Sie die Verwendung von Bildern, die in Workfront hochgeladen werden. Da in Workfront gespeicherte Bilder nicht öffentlich verfügbar sind und über einen Zugriffsschlüssel verfügen, der nach einem bestimmten Zeitraum abläuft, werden sie im Laufe der Zeit nicht mehr in der Ansicht angezeigt.
   >* Ein auf Ihrem Computer gespeichertes Bild verfügt nicht über eine inhärente URL. Suchen Sie eine Website, die Bild-Hosting bietet und hosten Sie Ihr Bild dort. Möglicherweise verfügt Ihr Unternehmen bereits über eine solche Website.

1. Wechseln Sie mithilfe Ihres Webbrowsers zu dem Bild, das Sie gespeichert haben.
1. Rufen Sie die URL des Bildes wie folgt ab:

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: I used this blog post to document what kind of image we need for this: https://www.canto.com/blog/image-url/ (consulting uses this)) </p>
   -->

   1. Klicken Sie mit der rechten Maustaste und wählen **Bildspeicherort kopieren** oder **Link abrufen** je nach Browser. Jetzt haben Sie die URL für dieses bestimmte Bild und können es aus Ihrer Zwischenablage einfügen.
   1. Stellen Sie sicher, dass alle Personen mit diesem Link die Berechtigung zum Anzeigen des Bildes haben, indem sie einfach zu dem Link gehen, und sie benötigen keine Anmeldung, um darauf zuzugreifen.

1. Gehen Sie zu einem Projekt, klicken Sie auf das **Mehr** Menü ![Mehr](assets/more-icon-45x33.png) neben dem Namen des Projekts und klicken Sie dann auf **Bearbeiten**.

1. Fügen Sie im Feld **URL** den Link zum Bild hinzu.
1. Gehe zu einer Projektansicht in einer Projektliste.
1. Klicken Sie auf **Dropdown** Menü Ansicht und dann auf **Neue Ansicht**.
1. Klicken Sie auf die Kopfzeile der Spalte für den **Projektnamen** und dann auf **In Textmodus wechseln**.

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

1. Klicken Sie **Fertig** > **Ansicht speichern**.
Das ausgewählte Bild ersetzt den Projektnamen in der Projektansicht, und das Bild ist ein Link zum Projekt.