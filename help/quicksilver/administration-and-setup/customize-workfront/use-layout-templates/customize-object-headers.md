---
title: Anpassen von Objektkopfzeilen mithilfe einer Layout-Vorlage
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: Als Adobe Workfront-Administrator oder Gruppenadministrator können Sie eine Layout-Vorlage verwenden, um die Felder zu konfigurieren, die Benutzende in der Kopfzeile des Objekts sehen, wenn sie die Seite eines Objekts öffnen.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: cbeaa0d7-a61a-4806-a871-96663d9ce124
source-git-commit: dc71072107ce80f6cb9033fcb17fe4ac74d5af18
workflow-type: tm+mt
source-wordcount: '547'
ht-degree: 7%

---

# Anpassen von Objekt-Headern mithilfe einer Layout-Vorlage

Als Adobe Workfront-Administrator oder Gruppenadministrator können Sie eine Layout-Vorlage verwenden, um die Felder zu konfigurieren, die Benutzende in der Kopfzeile des Objekts sehen, wenn sie die Seite eines Objekts öffnen.

>[!IMPORTANT]
>
>Die Anpassung von Objektkopfzeilen ist derzeit für Projekte, Aufgaben, Probleme, Portfolios, Programme, Vorlagen, Rechnungsnachweise, Teams, Benutzer, Unternehmen, Gruppen und Tarifkarten verfügbar.

![Objekt-Header-Felder](assets/object-header-fields.png)

Informationen zum Erstellen von Layout-Vorlagen finden Sie unter [Erstellen und Verwalten von Layout-Vorlagen](../use-layout-templates/create-and-manage-layout-templates.md).

Weitere Informationen zu Layout-Vorlagen für Gruppen finden [&#x200B; unter „Erstellen und Ändern der Layout-Vorlagen einer Gruppe](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

Nachdem Sie eine Layout-Vorlage konfiguriert haben, müssen Sie sie Benutzern zuweisen, damit die von Ihnen vorgenommenen Änderungen für andere sichtbar sind. Informationen zum Zuweisen einer Layout-Vorlage an Benutzer finden Sie unter [Zuweisen von Benutzern zu einer Layout-Vorlage](../use-layout-templates/assign-users-to-layout-template.md).

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront-Paket</td> 
   <td><p>Beliebig</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront-Lizenz</td> 
   <td><p>Standard</p>
       <p>Abo</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td>Konfigurationen der Zugriffsebene</td> 
   <td> <p>Um diese Schritte auf Systemebene durchzuführen, benötigen Sie die Zugriffsebene „Systemadministrator“.</p>
        <p>Um sie für eine Gruppe auszuführen, müssen Sie ein Manager dieser Gruppe sein.</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) in der Dokumentation zu Workfront.

+++

## Anpassen von Objektkopfzeilen

1. Beginnen Sie mit der Arbeit an einer Layout-Vorlage, wie unter [Erstellen und Verwalten von Layout-Vorlagen](../../customize-workfront/use-layout-templates/create-and-manage-layout-templates.md) beschrieben.
1. Wählen Sie **Dropdown-Menü „Anpassen** was Benutzer sehen“ ein Objekt aus, dessen Kopfzeile Sie anpassen möchten.
1. Bewegen Sie [!UICONTROL &#x200B; Abschnitt &#x200B;]Kopfzeilenfelder“ den Mauszeiger über die aktuellen Felder und führen Sie einen der folgenden Schritte aus:
   * Klicken Sie auf das **x**-Symbol, um ein Feld zu entfernen

     ODER

   * Klicken Sie auf das **grab**-Symbol und halten Sie es gedrückt, um das Feld per Drag-and-Drop an eine neue Position zu ziehen.

   ![Objektkopfzeilenfelder - Symbole zum Ausblenden und Verschieben](assets/object-header-field-x-and-grab-icons-in-lt.png)

1. Die Kopfzeile eines Objekts kann bis zu fünf Felder enthalten.

   Wenn Sie bereits fünf Felder ausgewählt haben, müssen Sie ein Feld entfernen, bevor Sie ein neues hinzufügen können.

1. Beginnen Sie **Feld &quot;** hinzufügen“ mit der Eingabe des Namens eines benutzerdefinierten Felds oder nativen Workfront-Felds, das Sie hinzufügen möchten, und wählen Sie es aus, wenn es in der Liste angezeigt wird. Das Feld wird direkt rechts neben dem Feld Feld Feld hinzufügen hinzugefügt und als erstes Feld in der oberen rechten Ecke der Kopfzeile des -Objekts angezeigt.

   >[!TIP]
   >
   >* Sie können jedes benutzerdefinierte Feld oder jedes native Feld hinzufügen, das im Bereich Übersicht des Abschnitts Details eines Objekts verfügbar ist. Beispielsweise verfügen nur Probleme über das Feld Schweregrad , und dieses Feld kann nicht zu Projekten oder Aufgaben hinzugefügt werden.
   >
   >* Wenn ein(e) Benutzende(r) ein benutzerdefiniertes Feld in der Kopfzeile bearbeitet und es in einem benutzerdefinierten Formular enthalten ist, das nicht an das Objekt angehängt ist, wird das benutzerdefinierte Formular automatisch zum Objekt hinzugefügt.
   >
   >* Wenn Sie das Feld „Gelöst von“ zur Kopfzeile eines Problems hinzufügen, ändert sich das Feld in „Problem, Aufgabe oder Projekt lösen“, wenn mit dem Problem ein Lösungsobjekt verknüpft ist.

   ![Feld zur Kopfzeile hinzufügen](assets/add-field-to-header-in-lt-list.png)

1. (Optional) Ziehen Sie die Felder in eine andere Reihenfolge.

1. Passen Sie die Layout-Vorlage weiter an. Sie können jederzeit auf **Übernehmen** klicken, um Ihren Fortschritt zu speichern.

   ODER

   Wenn Sie mit der Anpassung fertig sind, klicken Sie auf **Speichern und schließen**.

