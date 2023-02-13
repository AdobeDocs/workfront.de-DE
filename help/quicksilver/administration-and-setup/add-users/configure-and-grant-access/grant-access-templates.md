---
title: Zugriff auf Vorlagen gewähren
user-type: administrator
product-area: system-administration;templates
navigation-topic: configure-access-to-workfront
description: Als Adobe Workfront-Administrator können Sie eine Zugriffsstufe verwenden, um den Zugriff eines Benutzers auf Vorlagen in Workfront zu definieren.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: c8e6af1b-8cf3-4522-b0eb-7e5f2d34f5a9
source-git-commit: dd7f61fcd92a43303be356dd3209ec6da6a063dd
workflow-type: tm+mt
source-wordcount: '385'
ht-degree: 0%

---

# Zugriff auf Vorlagen gewähren

Als Adobe Workfront-Administrator können Sie mithilfe einer Zugriffsebene den Zugriff eines Benutzers auf Vorlagen definieren, wie hier beschrieben: [Übersicht über Zugriffsebenen](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

Nur Benutzer mit einer Planungslizenz können vollen Zugriff auf Vorlagen haben.

Informationen zur Verwendung benutzerdefinierter Zugriffsebenen zur Verwaltung des Benutzerzugriffs auf andere Objekttypen in Workfront finden Sie unter [Benutzerdefinierte Zugriffsebenen erstellen oder ändern](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Abo</td> 
   <td>Beliebig</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Sie müssen Workfront-Administrator sein.</p> <p><b>NOTE</b>: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Benutzerzugriff auf Vorlagen mithilfe einer benutzerdefinierten Zugriffsebene konfigurieren

1. Erstellen oder bearbeiten Sie die Zugriffsebene, wie hier beschrieben: [Benutzerdefinierte Zugriffsebenen erstellen oder ändern](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
1. Klicken Sie auf das Zahnradsymbol ![](assets/gear-icon-settings.png) auf **Ansicht** oder **Bearbeiten** auf der rechten Seite von Vorlagen und wählen Sie dann die Fähigkeiten aus, die Sie unter **Einstellungen anpassen**.

   ![](assets/access-level-to-templates-with-edit-expanded-1.png)

1. (Optional) Um die Zugriffseinstellungen für andere Objekte und Bereiche in der Zugriffsebene zu konfigurieren, an der Sie arbeiten, fahren Sie mit einem der Artikel fort, die unter [Zugriff auf Adobe Workfront konfigurieren](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md), z. B. [Zugriff auf Aufgaben gewähren](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md) und [Zugriff auf Finanzdaten gewähren](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
1. Wenn Sie fertig sind, klicken Sie auf **Speichern**.

   Nachdem die Zugriffsebene erstellt wurde, können Sie sie einem Benutzer zuweisen. Weitere Informationen finden Sie unter [Benutzerprofil bearbeiten](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## Zugriff auf Vorlagen nach Lizenztyp

Informationen dazu, was Benutzer in den einzelnen Zugriffsebenen mit Vorlagen tun können, finden Sie im Abschnitt [Vorlagen](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#template) im Artikel [Für jeden Objekttyp verfügbare Funktionen](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).

## Zugriff auf freigegebene Vorlagen

Als Eigentümer oder Ersteller eines Problems können Sie es mit anderen Benutzern teilen, indem Sie ihnen Berechtigungen erteilen, wie hier beschrieben: [Vorlage freigeben](../../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md).

<!--
If you make changes here, make them also in the "Grant access to" articles where this snippet had to be converted to text:
* reports, dashboards, and calendars
* financial data
* issue
-->

Wenn Sie ein Objekt für einen anderen Benutzer freigeben, werden die Rechte des Empfängers für dieses Objekt durch eine Kombination aus zwei Faktoren bestimmt:

* Die Berechtigungen, die Sie Ihrem Empfänger für das Objekt gewähren
* Einstellungen der Zugriffsebene des Empfängers für den Objekttyp
