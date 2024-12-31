---
product-area: templates
navigation-topic: templates-navigation-topic
title: Projektvorlagen löschen
description: Es wird empfohlen, Vorlagen, die Sie nicht mehr verwenden, zu deaktivieren, anstatt sie zu löschen, damit Sie über einen längeren Zeitraum historische Informationen über Ihre Projekte behalten können.
author: Alina
feature: Work Management
exl-id: 41e0979c-f8ef-4a07-8848-e4ee8cc212c5
source-git-commit: 02d20209b8bf53c84308707a89a5abf399494b64
workflow-type: tm+mt
source-wordcount: '416'
ht-degree: 0%

---

# Projektvorlagen löschen

Es wird empfohlen, Vorlagen, die Sie nicht mehr verwenden, zu deaktivieren, anstatt sie zu löschen, damit Sie über einen längeren Zeitraum historische Informationen über Ihre Projekte behalten können. Informationen zum Deaktivieren einer Vorlage finden Sie unter [Projektvorlagen bearbeiten](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).

>[!IMPORTANT]
>
>Wenn Sie eine Vorlage löschen, werden die Projekte, die diese Vorlage verwenden, in keiner Weise geändert. Der Name der ursprünglichen Vorlage wird jedoch nicht mehr im Feld Vorlage des Projekts angezeigt. Darüber hinaus können Sie die Namen der Vorlagenaufgaben für die Aufgaben im Projekt nicht mehr in einer Aufgabenansicht anzeigen. Das Vorlagenfeld im Projekt und das Vorlagenaufgabenfeld in den Aufgaben bleiben leer, nachdem die ursprünglich mit dem Projekt verknüpfte Vorlage gelöscht wurde.

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
   <td role="rowheader">Konfigurationen der Zugriffsebene*</td> 
   <td> <p>Bearbeiten des Zugriffs auf Vorlagen, der den Zugriff auf „Löschen“ umfasst</p> <p> <img src="assets/template-access-level-with-advanced-settings-350x113.png" style="width: 350;height: 113;"> </p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Einschränkungen in Ihrer Zugriffsebene festgelegt hat. Informationen dazu, wie Workfront-Admins Ihre Zugriffsebene ändern können, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Erstellen oder Ändern benutzerdefinierter Zugriffsebenen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Verwalten Sie Berechtigungen für die Vorlage, die Berechtigungen zum Löschen enthält</p> <p> <img src="assets/template-manage-permissions-with-advanced-settings-350x352.png" style="width: 350;height: 352;"> </p> <p>Informationen zum Anfordern zusätzlicher Zugriffsberechtigungen finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Anfordern von Zugriffsberechtigungen für Objekte </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um herauszufinden, über welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie verfügen.

## Überlegungen zum Löschen von Vorlagen

* Die Aufgaben, die Projekten beim Anhängen der Vorlage hinzugefügt wurden, verbleiben in den Projekten. Die mit den Aufgaben verknüpften Vorlagenaufgabeninformationen werden jedoch gelöscht.
* Der Name der Vorlage wird nicht mehr im Feld **Vorlage** auf der Unterregisterkarte **Übersicht** des Projekts aufgeführt.

* Sie können eine kürzlich gelöschte Vorlage aus dem Papierkorb wiederherstellen. Weitere Informationen zum Wiederherstellen von Elementen aus dem Papierkorb finden Sie unter [Wiederherstellen gelöschter Elemente](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).

## Löschen einer Vorlage

{{step1-to-templates}}

Dadurch wird eine Liste von Vorlagen geöffnet

1. Wählen Sie die zu löschende Vorlage aus, indem Sie das Kontrollkästchen links neben dem Vorlagennamen aktivieren und dann auf **Löschen > Ja, Löschen** klicken, um den Löschvorgang zu bestätigen.

   Oder

   Klicken Sie auf den Namen einer Vorlage, um darauf zuzugreifen, und klicken Sie dann auf das Menü **Mehr** ![](assets/qs-more-icon-on-an-object.png) und dann auf **Vorlage löschen > Ja, löschen**.

   Die Vorlage kann nicht mehr mit einem Projekt verknüpft werden.
