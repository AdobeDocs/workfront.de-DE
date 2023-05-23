---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '"Ansicht: Anzeigen eines Bildes anstelle einer Zeichenfolge in einer Spalte'
description: Sie können den Namen eines Objekts in einer Ansicht mithilfe des Textmodus durch ein Bild ersetzen. Sie können auch einen Link zum Bild hinzufügen, der das von ihm ersetzte Objekt öffnen kann.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: e1e4a993-f05c-4b6e-b00a-e96c9ab4c94f
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '516'
ht-degree: 0%

---

# Ansicht: Anzeigen eines Bildes anstelle einer Zeichenfolge in einer Spalte

Sie können den Namen eines Objekts in einer Ansicht mithilfe des Textmodus durch ein Bild ersetzen. Sie können auch einen Link zum Bild hinzufügen, der das von ihm ersetzte Objekt öffnen kann.

>[!NOTE]
>
>Bilder werden in ihrer tatsächlichen Auflösung angezeigt, daher versuchen Sie, kleine Bilder zu verwenden.

![](assets/replace-project-name-with-image-and-link-350x125.png)

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
   <td> <p>Anforderung zum Ändern einer Ansicht </p>
   <p>Berichtänderung planen</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf Berichte, Dashboards und Kalender bearbeiten, um einen Bericht zu ändern</p> <p>Zugriff auf Filter, Ansichten und Gruppierungen bearbeiten, um eine Ansicht zu ändern</p> <p><b>NOTIZ</b>

Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Berechtigungen für einen Bericht verwalten</p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

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

   1. Klicken Sie mit der rechten Maustaste und wählen Sie **Speicherort des Bildes kopieren** oder **Link abrufen**- abhängig von Ihrem Browser. Sie verfügen nun über die URL für dieses spezifische Bild und können es aus der Zwischenablage einfügen.
   1. Stellen Sie sicher, dass alle Benutzer mit diesem Link berechtigt sind, das Bild anzuzeigen, indem Sie einfach zum Link navigieren, und sie keine Anmeldung benötigen, um darauf zuzugreifen.

1. Wechseln Sie zu einem Projekt, klicken Sie auf die **Mehr** Menü ![](assets/more-icon-45x33.png) neben dem Namen des Projekts klicken Sie auf **Bearbeiten**.

1. Im **URL** -Feld den Link zum Bild hinzufügen.
1. Navigieren Sie zu einer Projektansicht in einer Liste oder einem Bericht und passen Sie die Ansicht an.
1. Klicken Sie auf die Kopfzeile der Spalte für die **Projektname** Klicken Sie auf **In den Textmodus wechseln**.

1. Fügen Sie der Spalte den folgenden Code zum vorhandenen Code hinzu:

   ```
   displayname=Link Project
   ```

   ```
   image.name=Link Project
   ```

   ```
   image.valuefield=URL
   ```

   ```
   link.linkproperty.0.name=projectID
   ```

   ```
   link.linkproperty.0.value=ID
   ```

   ```
   link.lookup=link.edit
   ```

   ```
   link.page=/view
   ```

   ```
   link.valuefield=objCode
   ```

   ```
   link.valueformat=val
   ```

   ```
   textmode=true
   ```

   ```
   type=image
   ```

   ```
   valueformat=
   ```

   Das ausgewählte Bild ersetzt den Projektnamen in der Projektansicht und das Bild ist ein Link zum Projekt.

1. Klicken **Ansicht speichern**.
