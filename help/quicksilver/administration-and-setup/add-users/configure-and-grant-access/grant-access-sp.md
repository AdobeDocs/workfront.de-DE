---
title: Zugriff auf den Szenario-Planer gewähren
description: Als Adobe Workfront-Administrator können Sie eine Zugriffsebene verwenden, um den Zugriff eines Benutzers auf den Szenario-Planer zu definieren.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 4343f0ff-2f78-4556-801f-db9d94f80c95
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '688'
ht-degree: 0%

---

# Zugriff auf den Szenario-Planer gewähren

Als Adobe Workfront-Administrator können Sie mithilfe einer Zugriffsebene den Zugriff eines Benutzers auf den Szenario Planer definieren, wie unter [Übersicht über Zugriffsebenen](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

Zusätzlich zum Zugriff auf den Szenario-Planer muss ein Benutzer mit einer Nicht-Systemadministratorzugriffsstufe auch Zugriff auf Finanzdaten haben, um alle in einem Plan enthaltenen Finanzinformationen wie Budgets, Kosten und Rollen für den Arbeitsplatz sehen zu können. Weitere Informationen finden Sie unter [Zugriff auf Finanzdaten gewähren](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

## Zugriffsanforderungen

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
   <td> <p>Überprüfen oder höher. Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref" data-mc-variable-override="">Übersicht über Adobe Workfront-Lizenzen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td> <p>Sie müssen eine zusätzliche Lizenz für den Adobe Workfront-Szenario-Planer erwerben, um auf die in diesem Artikel beschriebene Funktion zugreifen zu können.</p> <p>Informationen zum Abrufen des Workfront-Szenario-Players finden Sie unter <a href="../../../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref" data-mc-variable-override="">Für die Verwendung des Szenario-Planers benötigter Zugriff</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Zugriffsebene*</td> 
   <td> <p>Zugriff auf den Szenario-Planer anzeigen oder höher</p> <p><b>NOTE</b>: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsstufe ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Objektberechtigungen</p> </td> 
   <td> <p>Berechtigungen oder höher für einen Plan anzeigen</p> <p>Informationen über die Anforderung eines zusätzlichen Zugangs zu einem Plan finden Sie unter <a href="../../../scenario-planner/request-access-to-plan.md" class="MCXref xref" data-mc-variable-override="">Anfordern des Zugriffs auf einen Plan im Szenario-Planer</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Benutzerzugriff auf den Szenario-Planer mit einer benutzerdefinierten Zugriffsebene konfigurieren

1. Erstellen oder bearbeiten Sie die Zugriffsebene, wie hier beschrieben: [Benutzerdefinierte Zugriffsebenen erstellen oder ändern](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
1. Klicken Sie auf die Option rechts neben **Szenario-Planer** die Sie für diese Zugriffsebene verwenden möchten.

   >[!NOTE]
   >
   >Der Lizenztyp Anforderung oder Externer Lizenztyp erlaubt keinen Zugriff auf den Szenario-Planer anzeigen oder bearbeiten .

1. (Optional) Um die Zugriffseinstellungen für andere Objekte und Bereiche in der Zugriffsebene zu konfigurieren, an der Sie arbeiten, fahren Sie mit einem der Artikel fort, die unter [Zugriff auf Adobe Workfront konfigurieren](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md), z. B. [Zugriff auf Aufgaben gewähren](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md) und [Zugriff auf Finanzdaten gewähren](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
1. Wenn Sie fertig sind, klicken Sie auf **Speichern**.

## Zugriff auf den Szenario-Planer nach Lizenztyp

Informationen dazu, was Benutzer in den einzelnen Zugriffsebenen mit dem Szenario-Planer tun können, finden Sie im Abschnitt . [Bereich &quot;Szenario-Planer&quot;](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#scenario) im Artikel [Für jeden Objekttyp verfügbare Funktionen](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).

## Szenario Planen des Zugriffs nach Einstellung der Zugriffsebene

Die folgenden Informationen helfen Ihnen dabei, zu verstehen, wie Sie mit den Einstellungen auf Zugriffsebene den Zugriff der Benutzer auf Informationen im Workfront-Szenario-Planer steuern können.

* [Kein Zugriff](#no-access)
* [Zugriff anzeigen](#view-access)
* [Zugriff bearbeiten](#edit-access)

### Kein Zugriff {#no-access}

Benutzer ohne Zugriff auf den Szenario-Planer können weder das Szenario-Symbol im Hauptmenü sehen, wenn er zu ihrer Layoutvorlage hinzugefügt wird, noch Pläne und Initiativen anzeigen, die für sie freigegeben sind. Wenn der Link zu einem Plan für einen Benutzer freigegeben wird, der keinen Zugriff auf den Szenario-Planer hat, kann der Benutzer den Plan nicht anzeigen oder bearbeiten.

### Zugriff anzeigen {#view-access}

Benutzer mit Zugriff auf den Szenario-Planer anzeigen können Folgendes tun:

* Das Symbol Szenarien im Hauptmenü anzeigen ![](assets/esp-icon-in-main-menu.png), obwohl der Bereich Pläne leer ist, es sei denn, der Benutzer klickt auf einen von einem anderen Benutzer freigegebenen Plan-Link.
* Sehen Sie sich einen Plan an, wenn ein anderer Benutzer den Link darauf freigegeben hat.

   Dies umfasst alle Informationen zur Rolle im Job im Plan.

   Sie enthält auch Informationen zu den Stellenraten und Kosten des Plans, wenn der Empfänger auch Zugriff auf Finanzdaten hat. Weitere Informationen finden Sie unter [Zugriff auf Finanzdaten gewähren](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

### Zugriff bearbeiten {#edit-access}

Benutzer mit Zugriff auf den Szenario-Planer bearbeiten können Folgendes tun:

* Das Symbol Szenarien im Hauptmenü anzeigen ![](assets/esp-icon-in-main-menu.png) und nutzen Sie sie für den Zugriff auf Planungsdaten.
* Erstellen Sie Pläne.
* Anzeigen, Bearbeiten und Löschen von Plänen, die sie erstellen.
* Zeigen Sie die Pläne anderer Benutzer an, bearbeiten Sie sie und löschen Sie sie, indem Sie einen freigegebenen Link verwenden.

   Dies umfasst alle Informationen zur Rolle in einem Plan.

   Sie enthält auch Informationen zu den Stellenraten und Kosten des Plans, wenn der Empfänger Zugriff auf finanzielle Daten hat. Weitere Informationen finden Sie unter [Zugriff auf Finanzdaten gewähren](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
