---
product-area: projects
navigation-topic: use-predecessors
title: Erzwungene Vorgänger
description: Vorgänger sind Aufgaben, von deren Abschluss andere Aufgaben abhängen. Vorgängerbeziehungen wirken sich auf die Start- und Abschlussdaten der Aufgaben aus und wirken sich letztendlich auf die Timeline des Projekts aus.
author: Alina
feature: Work Management
exl-id: c3242b92-9036-4770-a073-2a9c393b97fd
source-git-commit: 5cb07cb42c3264c6629bc0a038c0e70ffc2cb509
workflow-type: tm+mt
source-wordcount: '494'
ht-degree: 0%

---

# Erzwungene Vorgänger

<!-- Audited: 2/2024 -->

Vorgänger sind Aufgaben, von deren Abschluss andere Aufgaben abhängen. Vorgängerbeziehungen wirken sich auf die Start- und Abschlussdaten der Aufgaben aus und wirken sich letztendlich auf die Timeline des Projekts aus.

Informationen zu Vorgängern finden Sie unter [Übersicht über Aufgabenvorgänger](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

Durch das Festlegen von Vorgängerbeziehungen zwischen Vorgängen legen Sie fest, wie der Beginn oder das Ende eines abhängigen Vorgangs vom Beginn oder Ende des Vorgängervorgangs abhängt. Dies geschieht mithilfe verschiedener Abhängigkeitstypen.

Informationen zu Abhängigkeitstypen finden Sie unter [Übersicht über Aufgabenabhängigkeitstypen](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).

## Übersicht über erzwungene Vorgänger

>[!IMPORTANT]
>
>Sie müssen Vorgänger erzwingen, damit Vorgängerbeziehungen respektiert werden. Ohne Erzwingung der Vorgänger können abhängige Aufgaben unabhängig vom Beginn und Ende der Vorgänger beginnen und enden, unabhängig von ihren Abhängigkeitstypen.

Sie können die Vorgängerbeziehung erzwingen, wenn Sie Vorgänger für ein Projekt festlegen.

Wenn ein Vorgänger erzwungen wird, kann die Nachfolgeaufgabe nicht gestartet werden, bevor der Vorgänger abgeschlossen ist. Wenn Sie z. B. eine Fertigstellungs-Start-Beziehung zwischen Aufgabe A und Aufgabe B erzwingen, kann Aufgabe B nicht gestartet werden (der Status muss Neu bleiben und der Prozentwert für Fertigstellungen muss 0 % bleiben), bis Aufgabe A als abgeschlossen markiert ist. Das Erzwingen von Beziehungen gilt für alle Vorgängertypen.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td>
      <p>Neu: Standard</p> 
      <p>ODER</p>
      <p>Aktuell: Plan</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriff auf Aufgaben und Projekte bearbeiten</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td><p>Verwalten der Berechtigungen für die Aufgaben und das Projekt</p></td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Erzwingen eines Vorgängers auf Aufgabenebene

1. Wechseln Sie zur Nachfolgeaufgabe, deren Vorgänger Sie erzwingen möchten.
1. Klicken Sie **linken Bereich auf** Vorgänger“ und dann auf **Vorgänger hinzufügen**. Möglicherweise müssen Sie auf **Mehr anzeigen** und dann auf **Vorgänger** klicken.
1. (Bedingt) Wenn Sie einen projektübergreifenden Vorgänger hinzufügen möchten, entfernen Sie den Namen des Projekts im Feld **Übergeordnetes Projekt** und ersetzen Sie ihn durch ein anderes Projekt.
1. Geben Sie den Namen der Vorgängeraufgabe(n) im Feld **Aufgaben** an.
1. Geben Sie den **Abhängigkeitstyp** zwischen diesen beiden Aufgaben an.

   Der standardmäßige **Abhängigkeitstyp** ist **Beenden-Start**.

1. Wählen Sie das Feld **Erzwungen** aus, um den Vorgänger zu erzwingen.
1. Klicken Sie auf **Speichern**.

## Erzwingen eines Vorgängers in einer Aufgabenliste

1. Gehe zu einer Aufgabenliste in einem Projekt.
1. Wählen Sie **Dropdown** Menü „Ansicht“ die Option **Standardansicht**.

1. Notieren Sie sich die Anzahl der Aufgaben, die Sie als Vorgänger festlegen werden.
1. Suchen Sie die Nachfolgeaufgabe, deren Vorgänger Sie erzwingen möchten.
1. Geben Sie in **Spalte** die Nummer der Vorgängeraufgabe ein, gefolgt von „e“. Geben Sie beispielsweise „1e“ ein, um die Aufgabennummer 1 als Vorgänger der ausgewählten Aufgabe hinzuzufügen.
1. Klicken Sie auf die Eingabetaste , um Ihre Vorgängerinformationen für die Aufgabe zu speichern.

   ![PREDECESSOR_ENFORCED_IN_LIST.png](assets/predecessor-enforced-in-list-350x308.png)
