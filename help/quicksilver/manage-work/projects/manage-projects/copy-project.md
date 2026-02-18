---
product-area: projects
navigation-topic: manage-projects
title: Kopieren eines Projekts
description: Sie können ein Projekt kopieren, anstatt es von Grund auf neu zu erstellen. Sie können jeweils nur ein Projekt kopieren. Projekte können nicht stapelweise kopiert werden.
author: Alina
feature: Projects, Work Management
role: User
exl-id: 1bb133a8-eb76-46b8-969f-37f57f9453b4
source-git-commit: 93db334537b5ec12dc0c77d51f8b2d83d8348f3d
workflow-type: tm+mt
source-wordcount: '751'
ht-degree: 7%

---

# Kopieren eines Projekts

<!--
<(LINKED TO THE PRODUCT IN THE COPY PROJECT BOX)</p>
-->

<!-- Audited: 5/2025 -->

Sie können ein Projekt aus einem vorhandenen kopieren, anstatt eines von Grund auf neu zu erstellen, was Zeit spart.

Beachten Sie, dass Sie Projekte nicht stapelweise kopieren können.

>[!IMPORTANT]
>
>Die folgenden Elemente werden niemals aus einem vorhandenen Projekt in ein neues kopiert:
>
>* Probleme
>* Abrechnungssätze
>* Abrechnungseinträge
>* Anmerkungen
>* Stunden
>* Projektübergreifende Vorgänger
>* Veranschlagte Stunden
>
>Die folgenden Elemente werden immer aus einem vorhandenen Projekt in ein neues kopiert:
>
>* Aufgaben
>* Vorlage
>* Risiken
>* Informationen zur Warteschlangeneinrichtung
>* Portfolio und Programm
>* Scorecard
>* Standardinformationen zu Aufgaben (Standardgenehmigungsprozess für Aufgaben, Standardmäßige benutzerdefinierte Forms für Aufgaben)
>
> Die Termine der Aufgaben des ursprünglichen Projekts werden in das neue Projekt kopiert. Sie müssen das Start- oder Abschlussdatum des Projekts (je nach Planungsmodus) ändern, um die Aufgabendaten zu aktualisieren. Aufgrund von Aufgabenbeschränkungen können Sie möglicherweise die Daten im Projekt nicht ändern.

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.
Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>Adobe Workfront-Paket</p> </td>  
   <td>Beliebig</td> 
  </tr> 
  <tr> 
   <td> <p>Adobe Workfront-Lizenz</p> </td> 
   <td> <p>Standard</p> 
   <p>Plan</p>
      </td> 
  </tr> 
     <td>Konfigurationen der Zugriffsebene </td> 
   <td> <p>Zugriff auf Projekte mit der Möglichkeit zum Erstellen und Kopieren von Projekten bearbeiten</p> </td> 
  </tr>

<td> <p>Objektberechtigungen </p> </td> 
   <td> <p>Anzeigen von Berechtigungen oder höher für das Projekt</p>  </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:
 
 <table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>Adobe Workfront plan</p> </td> 
   <td>Any</td> 
  </tr> 
  <tr> 
   <td> <p>Adobe Workfront license</p> </td> 
   <td> <p>New: Standard </p> 
   <p>Or</p>
   <p>Current: Plan </p>
   
   </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Access level configurations </td> 
   <td> <p>Edit access to Projects with ability to Create <span>and Copy</span> projects</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>Object permissions </p> </td> 
   <td> <p>View permissions or higher to the project</p>  </td> 
  </tr> 
 </tbody> 
</table>-->

## Zu beachten

* Beim Kopieren eines Projekts gibt es ein Verarbeitungslimit von 5 Minuten. Wenn an das Projekt eine große Anzahl von Dokumenten angehängt ist und es nicht kopiert werden kann, müssen Sie möglicherweise einige der Dokumente entfernen und erneut versuchen.

## Einzelnes Projekt kopieren

Beim Kopieren eines Projekts werden auch einige Informationen aus dem ursprünglichen Projekt in das neue Projekt kopiert. Sie können auch angeben, welche Elemente während des Kopiervorgangs nicht in das neue Projekt kopiert werden sollen.

Kopieren eines Projekts:

{{step1-to-projects}}

1. Wählen Sie das Projekt aus, das Sie kopieren möchten, und klicken Sie dann auf das **Mehr**-Symbol ![Mehr &#x200B;](assets/more-icon.png) rechts neben dem Projektnamen.

   ODER

   Gehen Sie zu einer Projektliste oder einem Bericht, wählen Sie ein Projekt aus und klicken Sie dann oben in der Liste auf das **Mehr**-Symbol ![](assets/more-icon.png)Mehr Menü).

1. Klicken Sie **Dropdown** Menü „Mehr“ auf **Kopieren**. Das **Kopie von [Projektname]** wird angezeigt.

1. (Optional) Aktualisieren Sie den **Projektnamen**. Standardmäßig lautet der neue Name **Kopie von [Originalprojektname]**.

   ![Projektfeld kopieren](assets/copy-of-project-box.png)

1. Wählen Sie einen **Status** aus. Standardmäßig ist der Status des ursprünglichen Projekts ausgewählt.

1. (Optional) Heben Sie die Markierung der Elemente auf, die Sie nicht in das neue Projekt kopieren möchten. In der folgenden Tabelle wird beschrieben, was passiert, wenn die Auswahl der Elemente aufgehoben wird:


   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Alle auswählen</td> 
      <td> <p>Wählt alle Optionen aus und löscht alle Felder und Objekte aus dem neuen Projekt. </p>

   <p> Wenn Sie diese Option deaktivieren, werden alle Elemente deaktiviert. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Arbeitsaufträge</td> 
      <td>Entfernt alle Projekt- und Aufgabenzuweisungen.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Fortschritt</td> 
      <td>Entfernt den Fortschritt bei allen Aufgaben und zeigt sie als Neu an. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Benutzerdefinierte Daten</td> 
      <td> <p>Entfernt die Informationen aus dem benutzerdefinierten Formular für das Projekt sowie die Informationen zu den benutzerdefinierten Formularen, die den folgenden Elementen zugeordnet sind:</p> 
       <ul> 
        <li>Aufgaben</li> 
        <li>Ausgaben</li> 
        <li> Dokumente</li> 
       </ul> 
      <p>Die benutzerdefinierten Formulare bleiben an die Aufgaben, Ausgaben, Dokumente und das Projekt angehängt, aber die Informationen in den benutzerdefinierten Feldern des Formulars werden nicht in das neue Projekt kopiert. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Dokumente</td> 
      <td> <p>Entfernt alle Elemente auf der Registerkarte „Dokumente“, einschließlich Dokumentversionen, verknüpfter Dokumente und Ordner.</p> <p>Standardmäßig können Korrekturabzüge und Genehmigungen nicht in ein anderes Projekt kopiert werden. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Alle Vorgänger</td> 
      <td> <p>Entfernt alle Vorgängerbeziehungen zwischen den Aufgaben im Projekt. </p> <p>

   Projektübergreifende Vorgänger werden niemals in das neue Projekt übertragen, unabhängig davon, ob dies ausgewählt ist oder nicht. </p> </td>
   </tr>

<tr> 
      <td role="rowheader">Veranschlagte Stunden</td> 
      <td> <p>Entfernt die budgetierten Stunden im Bereich Ressourcenplanung des Business Case des Projekts aus dem kopierten Projekt.</p> 
    <p>
   Mit dem Szenario-Planer budgetierte Stunden werden niemals in das neue Projekt kopiert, da das neue Projekt nicht mit einer Initiative im Szenario-Planer verknüpft ist. Weitere Informationen finden Sie unter <a href="../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case-use-scenario-planner.md">Budgetressourcen im Business Case mit dem Szenario-Planer</a></p>
   </tr></td>
    <tr> 
      <td role="rowheader">Finanzinformationen</td> 
      <td> <p>Entfernt die Informationen in den folgenden Bereichen: </p> 
       <ul> 
        <li>Unterregisterkarte „Finanzen“ des Projekts</li> 
        <li> Geplanter Vorteil im Business Case</li> 
        <li>Finanzinformationen aus allen Aufgaben<br></li> 
       </ul> <p>Weitere Informationen zur Unterregisterkarte Projektfinanzierung finden Sie unter <a href="../../../manage-work/projects/project-finances/manage-project-finance-area.md" class="MCXref xref">Verwalten von Informationen im Bereich Projektfinanzierung</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Genehmigungsprozess</td> 
      <td>Entfernt alle Genehmigungen, die mit den Aufgaben oder dem Projekt verbunden sind. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Erinnerungsnachrichten</td> 
      <td> Entfernt die mit den Aufgaben oder dem Projekt verknüpften Erinnerungsnachrichten. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ausgaben</td> 
      <td>Entfernt Ausgaben im Zusammenhang mit den Aufgaben oder dem Projekt. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Berechtigungen</td> 
      <td> Entfernt Berechtigungen für alle Benutzer, die Aufgaben oder das Projekt ausführen.</td> 
     </tr> 
    </tbody> 
   </table>

1. Klicken Sie **Projekt kopieren**. Das kopierte Projekt wird erstellt.
