---
product-area: projects
navigation-topic: use-predecessors
title: Erstellen einer Vorgängerbeziehung auf der Aufgabenliste
description: Sie können Vorgängeraufgaben (oder nur Vorgänger) verwenden, um Aufgaben, die von anderen Aufgaben abhängen, zu starten oder abzuschließen. Sie möchten beispielsweise keine Partei (abhängige Aufgabe) hosten, bevor Sie die Einladungen versenden (vorherige Aufgabe).
author: Alina
feature: Work Management
exl-id: a84d88ac-8dd4-4952-b83f-02fafa61e68b
source-git-commit: 420ba180dd0bfd53514c58f77ca9897ba9797320
workflow-type: tm+mt
source-wordcount: '640'
ht-degree: 0%

---

# Erstellen einer Vorgängerbeziehung auf der Aufgabenliste

Sie können Vorgängeraufgaben (oder nur Vorgänger) verwenden, um Aufgaben, die von anderen Aufgaben abhängen, zu starten oder abzuschließen. Sie möchten beispielsweise keine Partei (abhängige Aufgabe) hosten, bevor Sie die Einladungen versenden (vorherige Aufgabe).

In diesem Artikel erfahren Sie, wie Sie in der Aufgabenliste Vorgänger erstellen.

Sie können die Vorgänger von Aufgaben in den folgenden Bereichen von Adobe Workfront anzeigen:

* In der Aufgabenliste in der Spalte &quot;Vorgänger&quot;.
* In der Gantt-Grafik
* Im Abschnitt &quot;Vorgänger&quot;einer abhängigen Aufgabe

Weitere Informationen finden Sie unter [Übersicht über die Vorgänger von Aufgaben](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

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
   <td> <p>Zugriff auf Aufgaben und Projekte bearbeiten</p> <p><b>NOTIZ</b>

Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Berechtigungen für Aufgaben und Projekte verwalten</p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Erstellen eines Vorgängers

1. Wechseln Sie zu einem Projekt.
1. Klicken **Aufgaben** im linken Bereich.
1. Stellen Sie sicher, dass Ihre aktuelle Ansicht die **Vorgänger** Spalte.

   Wenn in der Ansicht die Spalte &quot;Vorgänger&quot;nicht angezeigt wird, wechseln Sie zu einer Ansicht, die dies tut, oder fügen Sie die Spalte zu Ihrer Ansicht hinzu.

1. Wählen Sie die Aufgabe aus, die Sie als abhängige Aufgabe festlegen möchten.
1. Klicken Sie in die **Vorgänger** Spalte.
1. Geben Sie die Aufgabennummer ein, die Sie als Vorgänger der ausgewählten Aufgabe festlegen möchten, und drücken Sie dann die Eingabetaste **Eingabe**.

   Das Vorgängersymbol wird grün, wenn die Vorgängeraufgabe als abgeschlossen markiert ist. Dies signalisiert, dass die abhängige Aufgabe einsatzbereit ist.

   Weitere Informationen zu den in der Spalte &quot;Vorgänger&quot;verfügbaren Beziehungstypen finden Sie unter [Übersicht über die Vorgänger von Aufgaben](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md) in [Übersicht über die Vorgänger von Aufgaben](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

## Anzeigen von Vorgängerdetails

Sie können in der Aufgabenliste schnell Details zum Vorgänger anzeigen.

1. Bewegen Sie in der Aufgabenliste den Mauszeiger über die vorangestellte Nummer in der **Vorgänger** Spalte.

   Ein Feld mit den Details des Vorgängers wird angezeigt.

   ![Details zu Vorgängern](assets/predecessor-details-in-task-list.png)

   Die folgenden Details werden angezeigt:

   **Vorgängername:** Der Name des Vorgängers, auf den verwiesen wird. Die Aufgabennummer des Vorgängers ist enthalten. Klicken Sie auf den Aufgabennamen, um ihn zu öffnen. Im obigen Beispiel ist der Vorgänger Produktion/Ausführung/Versand.

   **Projektname:** Der Name des Projekts, in dem sich der Vorgänger befindet. Das Projekt wird als aktuelles Projekt identifiziert, wenn der Vorgänger zu denselben Projekten wie die Aufgabe gehört, oder als übergreifendes Projekt, wenn der Vorgänger zu einem anderen Projekt gehört. Im obigen Beispiel lautet der Projektname Digital Asset Production (Integrated) - Project. Weitere Informationen zu projektübergreifenden Vorgängern finden Sie unter [Erstellen projektübergreifender Vorgänger](../../tasks/use-prdcssrs/cross-project-predecessors.md).

   Sie können die Projektdetails erweitern, um die geplanten Start- und Enddaten, Bedingungen, Status, Prozentsatz der Fertigstellung und Eigentümer des Projekts anzuzeigen. Für ein übergreifendes Projekt können Sie dann auf **Siehe Projekt** , um das Projekt zu öffnen.

   **ID:** Die Referenznummer des Projekts, in dem sich der Vorgänger befindet.

   **Geplanter Start:** Das geplante Startdatum der Vorgängeraufgabe.

   **Geplantes Ende:** Das geplante Abschlussdatum der Vorläuferaufgabe.

   **Anzahl der Vorgänger:** Die Anzahl der Vorgänger für den Vorgänger, auf den verwiesen wird. Im obigen Beispiel hat der Vorgänger, auf den verwiesen wird, 1 Vorgänger.

   **Anzahl der Nachfolger:** Die Anzahl der Nachfolgeaufgaben (oder abhängigen Aufgaben) für den Vorgänger, auf den verwiesen wird. Im obigen Beispiel hat der referenzierte Vorgänger 1 Nachfolger.
