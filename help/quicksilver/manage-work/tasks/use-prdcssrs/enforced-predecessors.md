---
product-area: projects
navigation-topic: use-predecessors
title: Durchsetzen von Vorgängern
description: Vorläufer sind Aufgaben, von denen andere Aufgaben zur Erfüllung abhängen. Vorgängerbeziehungen wirken sich auf das Start- und Fertigstellungsdatum der Aufgaben aus und beeinflussen letztendlich die Zeitleiste des Projekts.
author: Alina
feature: Work Management
exl-id: c3242b92-9036-4770-a073-2a9c393b97fd
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '530'
ht-degree: 0%

---

# Durchsetzen von Vorgängern

Vorläufer sind Aufgaben, von denen andere Aufgaben zur Erfüllung abhängen. Vorgängerbeziehungen wirken sich auf das Start- und Fertigstellungsdatum der Aufgaben aus und beeinflussen letztendlich die Zeitleiste des Projekts.

Weitere Informationen zu Vorgängern finden Sie unter [Übersicht über die Vorgänger von Aufgaben](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

Durch das Festlegen von Vorgängerbeziehungen zwischen Aufgaben definieren Sie, wie der Start oder die Fertigstellung einer abhängigen Aufgabe vom Start oder der Fertigstellung ihrer Vorgängeraufgaben abhängt. Dazu werden verschiedene Abhängigkeitstypen verwendet.

Weitere Informationen zu Abhängigkeitstypen finden Sie unter [Übersicht über Aufgabenabhängigkeitstypen](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).

## Übersicht über erzwungene Vorgänger

>[!IMPORTANT]
>
>Sie müssen Vorgänger dazu zwingen, die Achtung von Vorgängerbeziehungen zu verlangen. Ohne Erzwingen der Vorgänger können abhängige Aufgaben unabhängig von ihren Abhängigkeitstypen unabhängig vom Start und Ende ihrer Vorgänger starten und beenden.

Sie können die Vorgängerbeziehung erzwingen, wenn Sie Vorgänger für ein Projekt festlegen.

Wenn ein Vorgänger erzwungen wird, kann die Nachfolgeaufgabe nicht gestartet werden, bevor der Vorgänger abgeschlossen ist. Beispielsweise bedeutet das Erzwingen einer Finish-Start-Beziehung zwischen Aufgabe A und Aufgabe B, dass Aufgabe B nicht starten kann (der Status muss neu bleiben und der Prozentsatz Complete muss 0 % bleiben), bis Aufgabe A als abgeschlossen markiert ist. Die Durchsetzung von Beziehungen gilt für alle Vorgängertypen.

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
   <td> <p>Zugriff auf Aufgaben und Projekte bearbeiten</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Berechtigungen für Aufgaben und Projekte verwalten</p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Erzwingen eines Vorgängers auf Aufgabenebene

1. Gehen Sie zur Nachfolgeaufgabe, deren Vorgänger Sie erzwingen möchten.
1. Klicken **Vorgänger** Klicken Sie im linken Bereich auf **Vorgänger hinzufügen**. Möglicherweise müssen Sie auf **Mehr anzeigen**, dann **Vorgänger**.
1. (Bedingt) Wenn Sie einen projektübergreifenden Vorgänger hinzufügen möchten, entfernen Sie den Namen des Projekts im **Übergeordnetes Projekt** und ersetzen Sie es durch ein anderes Projekt.
1. Geben Sie den Namen der Vorgängeraufgabe(en) im **Aufgaben** -Feld.
1. Geben Sie die **Abhängigkeitstyp** zwischen diesen beiden Aufgaben.

   Die Standardeinstellung **Abhängigkeitstyp** is **Finish-Start**.

1. Wählen Sie die **Durchgesetzt** -Feld, um den Vorgänger zu erzwingen.
1. Klicken Sie auf **Speichern**.

## Erzwingen eines Vorgängers in einer Aufgabenliste

1. Rufen Sie eine Aufgabenliste für ein Projekt auf.
1. Aus dem **Ansicht** aus dem Dropdown-Menü **Standardansicht**.

1. Notieren Sie sich die Anzahl der Aufgaben, die Sie als Vorgänger festlegen werden.
1. Suchen Sie die Nachfolgeaufgabe, deren Vorgänger Sie erzwingen möchten.
1. Im **Vorgänger** eingeben, die Nummer der Vorgängeraufgabe gefolgt von &quot;e&quot;. Geben Sie beispielsweise &quot;1e&quot;ein, um die Aufgabe Nr. 1 als Vorgänger zur ausgewählten Aufgabe hinzuzufügen.
1. Klicken Sie auf die Eingabetaste , um Ihre Vorgängerinformationen für die Aufgabe zu speichern.

   ![predecessor_enforced_in_list.png](assets/predecessor-enforced-in-list-350x308.png)
