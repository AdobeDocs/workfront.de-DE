---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '"Gruppierung: den Anzeigenamen in einer Gruppierung bearbeiten'''
description: Sie können Gruppierungen so umbenennen, dass sie Ihren Benutzern besser bekannt sind.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 072d3c2b-9ede-4bb9-9a27-dc77ceb732c4
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '323'
ht-degree: 0%

---

# Gruppierung: den Anzeigenamen in einer Gruppierung bearbeiten

Sie können Gruppierungen so umbenennen, dass sie Ihren Benutzern besser bekannt sind.

Wenn Sie beispielsweise die Standardgruppierung Projektname auf eine Projektliste anwenden, wird der Portfolio der Gruppierung als *Portfolio: Name:`<name of portfolio>`*.

![](assets/grouping-unedited-name-350x167.png)

Sie können diese Gruppierung mithilfe des Textmodus ändern, um einen leichter lesbaren Namen anzuzeigen.

![](assets/grouping-edited-name-350x160.png)

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
   <td> <p>Zugriff auf Berichte, Dashboards und Kalender bearbeiten</p> <p>Zugriff auf Filter, Ansichten, Gruppierungen bearbeiten</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Berechtigungen für einen Bericht verwalten</p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Anzeigenamen in einer Gruppierung bearbeiten

So ändern Sie den Anzeigenamen in einer Projektgruppe:

1. Gehen Sie zu einer Projektliste.
1. Aus dem **Gruppierung** Dropdown-Menü auswählen **Neue Gruppierung**.

1. Klicken **Gruppierung hinzufügen** und beginnen Sie mit der Eingabe von &quot;Portfolio Name&quot;im **Zuerst durch:** und wählen Sie es aus, wenn es in der Liste angezeigt wird.

1. Klicken **In den Textmodus wechseln**.
1. Führen Sie einen der folgenden Schritte aus:

   * Fügen Sie den folgenden Code zum vorhandenen Text hinzu, der im **Gruppieren Ihres Berichts** Feld:

      ```
      group.0.displayname=Your
      ```

      ```
      Value
      ```

      Oder in diesem Fall:

      ```
      group.0.displayname=Portfolio
      ```

   * Entfernen Sie alle Zeilen in der Textmodus-Benutzeroberfläche der Gruppierung, die das Wort &quot;name&quot;enthalten, und fügen Sie dann die Zeile hinzu:

      ```
      group.0.name=Your Value
      ```

      Oder in diesem Fall:

      ```
      group.0.name=Portfolio
      ```

      Sie können auch die

      ```
      group.0.name
      ```

      leer, wobei die Gruppierung den Namen des Werts angibt, nach dem Sie gruppieren möchten.

      ![](assets/grouping-edited-name-no-name-350x162.png)

1. Klicken **Fertig**, dann **Gruppierung speichern**.
