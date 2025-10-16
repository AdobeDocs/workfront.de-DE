---
title: Zugriff auf den Szenario-Planer gewähren
description: Als Adobe Workfront-Administrator können Sie eine Zugriffsebene verwenden, um den Zugriff eines Benutzers auf den Szenario-Planer zu definieren.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 4343f0ff-2f78-4556-801f-db9d94f80c95
source-git-commit: 2a83e5a415ff254cf5525d6f44ecb0e447e7e70a
workflow-type: tm+mt
source-wordcount: '609'
ht-degree: 0%

---

# Zugriff auf Scenario Planner gewähren

Als Adobe Workfront-Administrator können Sie eine Zugriffsebene verwenden, um den Zugriff eines Benutzers auf den Szenario-Planer zu definieren, wie in [Übersicht über Zugriffsebenen](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md) beschrieben.

Zusätzlich zum Zugriff auf den Szenario-Planer muss ein Benutzer mit der Zugriffsebene eines Nicht-Systemadministrators auch Zugriff auf Finanzdaten haben, um die in einem Plan enthaltenen Finanzinformationen anzuzeigen, z. B. Budgets, Kosten und Aufgabengebiets-Raten. Weitere Informationen finden Sie unter [Zugriff auf Finanzdaten gewähren](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Adobe Workfront-Paket</p> </td> 
   <td>Unternehmen oder höher</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td> 
   <p>Licht oder höher</p>
   <p>Überprüfen oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td> <p>Sie müssen eine zusätzliche Lizenz für den Adobe Workfront Scenario Planner erwerben.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Anzeigen des Zugriffs auf den Szenario-Planer oder höher</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Objektberechtigungen</p> </td> 
   <td> <p>Anzeigen von Berechtigungen oder höher für einen Plan</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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
