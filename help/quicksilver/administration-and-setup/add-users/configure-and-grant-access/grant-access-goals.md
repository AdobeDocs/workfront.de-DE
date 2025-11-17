---
title: Zugriff auf Adobe Workfront-Ziele gewähren
user-type: administrator
product-area: system-administration;documents
navigation-topic: configure-access-to-workfront
description: Als Adobe Workfront-Administrator können Sie eine Zugriffsebene verwenden, um den Zugriff eines Benutzers auf Workfront-Ziele zu definieren.
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: 8639da14-d545-4f9a-894b-12c29699b0db
source-git-commit: 6948f9462c59bad9e6db67d6169e5f9dec4157fe
workflow-type: tm+mt
source-wordcount: '267'
ht-degree: 6%

---

# Zugriff auf Adobe Workfront-Ziele gewähren

Als Adobe Workfront-Administrator können Sie eine Zugriffsebene verwenden, um den Zugriff eines Benutzers auf Adobe Workfront-Ziele zu definieren, wie in [Übersicht über Zugriffsebenen](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md) beschrieben.

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

Sie müssen über Folgendes verfügen, um Benutzenden Zugriff auf Workfront Goals zu gewähren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Workfront-Paket</td> 
   <td> <p>Workfront Ultimate</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td><p>Standard</p>
   <p>Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfiguration der Zugriffsebene</td> 
   <td> <p>Sie müssen über die Zugriffsebene „Systemadministrator“ verfügen.</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Workfront plan</td> 
   <td> <p>Pro or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Workfront Goals <p>Contact your Workfront account manager to learn about a Workfront Goals license. </p> <p>Workfront Goals is available only in the new Adobe Workfront experience.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configuration*</td> 
   <td> <p>You must have the System Administrator access level.</p> <p><b>NOTE</b>: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Gewähren des Benutzerzugriffs auf Workfront-Ziele mithilfe einer benutzerdefinierten Zugriffsebene

1. Erstellen oder bearbeiten Sie die Zugriffsebene, wie unter [Erstellen oder Ändern benutzerdefinierter Zugriffsebenen“ &#x200B;](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
1. Klicken Sie auf die Option rechts neben **Ziele**, die Sie für diese Zugriffsebene verwenden möchten.


   >[!NOTE]
   >
   >Der externe Lizenztyp lässt keine Anzeige- oder Bearbeitungsberechtigungen für Workfront-Ziele zu.

1. (Optional) Um Zugriffseinstellungen für andere Objekte und Bereiche in der Zugriffsebene, an der Sie arbeiten, zu konfigurieren, fahren Sie mit einem der in [Zugriff auf Adobe Workfront konfigurieren](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md) aufgelisteten Artikel fort, z. B. [Zugriff auf Aufgaben gewähren](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md) und [Zugriff auf Finanzdaten gewähren](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
1. Wenn Sie fertig sind, klicken Sie auf **Speichern**.

## Zugriff auf Workfront-Ziele nach Lizenztyp

Ein Workfront-Administrator kann über eine Zugriffsebene Benutzenden mit den folgenden Lizenzen Zugriff auf Workfront-Ziele gewähren:

* Standard, Licht, Mitwirkende
* Lizenz planen, bearbeiten, anfordern oder überprüfen.

Weitere Informationen zum Zugriff auf Workfront-Ziele finden Sie unter [Voraussetzungen für die Verwendung von Workfront-Zielen](../../../workfront-goals/goal-management/access-needed-for-wf-goals.md).
