---
title: Zugriff auf den Szenario-Planer gewähren
description: Als Adobe Workfront-Administrator können Sie eine Zugriffsebene verwenden, um den Zugriff eines Benutzers auf den Szenario-Planer zu definieren.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 4343f0ff-2f78-4556-801f-db9d94f80c95
source-git-commit: c887569d59c7751210671cab97c492ee1752fffc
workflow-type: tm+mt
source-wordcount: '697'
ht-degree: 0%

---

# Zugriff auf Scenario Planner gewähren

Als Adobe Workfront-Administrator können Sie eine Zugriffsebene verwenden, um den Zugriff eines Benutzers auf den Szenario-Planer zu definieren, wie in [Übersicht über Zugriffsebenen](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md) beschrieben.

Zusätzlich zum Zugriff auf den Szenario-Planer muss ein Benutzer mit der Zugriffsebene eines Nicht-Systemadministrators auch Zugriff auf Finanzdaten haben, um die in einem Plan enthaltenen Finanzinformationen anzuzeigen, z. B. Budgets, Kosten und Aufgabengebiets-Raten. Weitere Informationen finden Sie unter [Zugriff auf Finanzdaten gewähren](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über Folgendes verfügen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Adobe Workfront-Plan*</p> </td> 
   <td>Unternehmen oder höher</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Überprüfen Sie oder höher. Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref" data-mc-variable-override="">Lizenzen - Übersicht</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td> <p>Sie müssen eine zusätzliche Lizenz für den Adobe Workfront Scenario Planner erwerben, um auf die in diesem Artikel beschriebenen Funktionen zugreifen zu können.</p> <p>Informationen zum Abrufen des Workfront-Szenarioplaners finden Sie unter <a href="../../../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref" data-mc-variable-override="">Zugriff für die Verwendung des Szenarioplaners erforderlich</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Zugriffsebene*</td> 
   <td> <p>Anzeigen des Zugriffs auf den Szenario-Planer oder höher</p> <p><b>HINWEIS</b>: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Einschränkungen in Ihrer Zugriffsebene festgelegt hat. Informationen dazu, wie Workfront-Admins Ihre Zugriffsebene ändern können, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">Erstellen oder Ändern benutzerdefinierter Zugriffsebenen</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Objektberechtigungen</p> </td> 
   <td> <p>Anzeigen von Berechtigungen oder höher für einen Plan</p> <p>Informationen zum Anfordern zusätzlichen Zugriffs auf einen Plan finden Sie unter <a href="../../../scenario-planner/request-access-to-plan.md" class="MCXref xref" data-mc-variable-override="">Anfordern des Zugriffs auf einen Plan im Szenario-Planer</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um herauszufinden, über welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie verfügen.

+++

## Konfigurieren des Benutzerzugriffs auf den Szenario-Planer mithilfe einer benutzerdefinierten Zugriffsebene

1. Erstellen oder bearbeiten Sie die Zugriffsebene, wie unter [Erstellen oder Ändern benutzerdefinierter Zugriffsebenen“ ](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
1. Klicken Sie auf die Option rechts neben **Szenario-Planer**, die Sie für diese Zugriffsebene verwenden möchten.

   >[!NOTE]
   >
   >Der Anforderungs- oder externe Lizenztyp lässt keine Anzeige- oder Bearbeitungsberechtigungen für den Szenario-Planer zu.

1. (Optional) Um Zugriffseinstellungen für andere Objekte und Bereiche in der Zugriffsebene, an der Sie arbeiten, zu konfigurieren, fahren Sie mit einem der in [Zugriff auf Adobe Workfront konfigurieren](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md) aufgelisteten Artikel fort, z. B. [Zugriff auf Aufgaben gewähren](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md) und [Zugriff auf Finanzdaten gewähren](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
1. Wenn Sie fertig sind, klicken Sie auf **Speichern**.

## Zugriff auf den Szenario-Planer nach Lizenztyp

Informationen dazu, was Benutzer in den einzelnen Zugriffsebenen mit dem Szenarienplaner tun können, finden Sie im Abschnitt [Szenarienplaner-Bereich](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#scenario) im Artikel [Für jeden Objekttyp verfügbare Funktionen](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).

## Zugriff durch Zugriffsebenen-Einstellung für Szenario-Planer

Die folgenden Informationen helfen Ihnen zu verstehen, wie Sie mit den Einstellungen der Zugriffsebene den Zugriff der Benutzenden auf Informationen im Workfront-Szenarioplaner steuern können.

* [Kein Zugriff](#no-access)
* [Ansichtszugriff](#view-access)
* [Zugriff bearbeiten](#edit-access)

### Kein Zugriff {#no-access}

Benutzende ohne Zugriff auf den Szenario-Planer können weder das Szenario -Symbol im Hauptmenü sehen, wenn es zu ihrer Layout-Vorlage hinzugefügt wird, noch Pläne und Initiativen anzeigen, die für sie freigegeben sind. Wenn der Link zu einem Plan für einen Benutzer freigegeben wird, der keinen Zugriff auf den Szenario-Planer hat, kann der Benutzer den Plan nicht anzeigen oder bearbeiten.

### Ansichtszugriff {#view-access}

Benutzende mit Ansichtszugriff auf den Szenario-Planer können Folgendes tun:

* Siehe das Symbol Szenarien im Hauptmenü ![](assets/esp-icon-in-main-menu.png), obwohl der Bereich Pläne leer ist, es sei denn, der Benutzer klickt auf einen Plan-Link, der von einem anderen Benutzer freigegeben wurde.
* Zeigen Sie einen Plan an, wenn ein anderer Benutzer den Link dazu freigibt.

  Dazu gehören alle Informationen zu Aufgabengebieten im Plan.

  Es enthält auch Tarife für Aufgabengebiete und Kosteninformationen im Plan, falls der empfangende Benutzer auch Zugriff auf Finanzdaten hat. Weitere Informationen finden Sie unter [Zugriff auf Finanzdaten gewähren](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

### Zugriff bearbeiten {#edit-access}

Benutzende mit Bearbeitungszugriff auf den Szenario-Planer können Folgendes tun:

* Zeigen Sie das Symbol Szenarien im Hauptmenü ![](assets/esp-icon-in-main-menu.png) an und verwenden Sie es, um auf Plandaten zuzugreifen.
* Pläne erstellen.
* Von ihnen erstellte Pläne anzeigen, bearbeiten und löschen.
* Pläne anderer Benutzer, auf die sie über einen freigegebenen Link zugreifen, anzeigen, bearbeiten und löschen.

  Dazu gehören alle Informationen zu Aufgabengebieten in einem Plan.

  Es enthält auch Tarife für Aufgabengebiete und Kosteninformationen im Plan, sofern der empfangende Benutzer Zugriff auf Finanzdaten hat. Weitere Informationen finden Sie unter [Zugriff auf Finanzdaten gewähren](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
