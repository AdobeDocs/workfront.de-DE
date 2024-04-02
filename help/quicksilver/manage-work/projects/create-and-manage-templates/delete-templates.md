---
product-area: templates
navigation-topic: templates-navigation-topic
title: Löschen von Projektvorlagen
description: Es wird empfohlen, Vorlagen, die Sie nicht mehr verwenden, zu deaktivieren, anstatt sie zu löschen, damit Sie historische Informationen über Ihre Projekte im Laufe der Zeit speichern können. Weitere Informationen zum Deaktivieren einer Vorlage finden Sie unter Bearbeiten von Projektvorlagen .
author: Alina
feature: Work Management
exl-id: 41e0979c-f8ef-4a07-8848-e4ee8cc212c5
source-git-commit: 7bef757c24adc7791cb3b258ae6c33f3c0eec818
workflow-type: tm+mt
source-wordcount: '426'
ht-degree: 0%

---

# Löschen von Projektvorlagen

Es wird empfohlen, Vorlagen, die Sie nicht mehr verwenden, zu deaktivieren, anstatt sie zu löschen, damit Sie historische Informationen über Ihre Projekte im Laufe der Zeit speichern können. Informationen zum Deaktivieren einer Vorlage finden Sie unter [Bearbeiten von Projektvorlagen](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).

>[!IMPORTANT]
>
>Wenn Sie eine Vorlage löschen, werden die Projekte, die diese Vorlage verwenden, in keiner Weise geändert. Der Name der ursprünglichen Vorlage wird jedoch nicht mehr im Feld Vorlage des Projekts angezeigt. Darüber hinaus können Sie die Namen der Vorlagenaufgaben für die Aufgaben im Projekt nicht mehr in einer Aufgabenansicht anzeigen. Das Feld Vorlage im Projekt und das Feld Vorlagenaufgabe für die Aufgaben bleiben leer, nachdem die Vorlage, die ursprünglich mit dem Projekt verknüpft war, gelöscht wurde.

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf Vorlagen bearbeiten, die Zugriff auf Löschen enthalten</p> <p> <img src="assets/template-access-level-with-advanced-settings-350x113.png" style="width: 350;height: 113;"> </p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Berechtigungen für die Vorlage verwalten, die Berechtigungen zum Löschen enthält</p> <p> <img src="assets/template-manage-permissions-with-advanced-settings-350x352.png" style="width: 350;height: 352;"> </p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Überlegungen zum Löschen von Vorlagen

* Die Aufgaben, die zu den Projekten hinzugefügt wurden, als die Vorlage angehängt wurde, verbleiben in den Projekten. Die mit den Aufgaben verknüpften Vorlagenaufgabeninformationen werden jedoch gelöscht.
* Der Name der Vorlage wird nicht mehr im **Vorlage** im Feld **Übersicht** Unterregisterkarte des Projekts.

* Sie können eine kürzlich gelöschte Vorlage aus dem Papierkorb wiederherstellen. Informationen zum Wiederherstellen von Elementen aus dem Papierkorb finden Sie unter [Gelöschte Elemente wiederherstellen](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).

## Vorlage löschen

{{step1-to-templates}}

Dadurch wird eine Liste von Vorlagen geöffnet

1. Wählen Sie die zu löschende Vorlage aus, indem Sie das Kontrollkästchen links neben dem Vorlagennamen aktivieren und dann auf **Löschen > Ja, Löschen** , um den Löschvorgang zu bestätigen.

   Oder

   Klicken Sie auf den Namen einer Vorlage, um darauf zuzugreifen, und klicken Sie dann auf das **Mehr** Menü ![](assets/qs-more-icon-on-an-object.png) , dann **Vorlage löschen > Ja, Löschen**.

   Die Vorlage kann nicht mehr mit einem Projekt verknüpft werden.
