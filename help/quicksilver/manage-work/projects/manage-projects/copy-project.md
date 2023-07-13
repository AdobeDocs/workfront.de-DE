---
product-area: projects
navigation-topic: manage-projects
title: Projekt kopieren
description: Sie können ein Projekt kopieren, anstatt es von Grund auf neu zu erstellen. Sie können jeweils nur ein Projekt kopieren. Sie können keine Projekte in großen Mengen kopieren.
author: Alina
feature: Projects, Work Management
role: User
exl-id: 1bb133a8-eb76-46b8-969f-37f57f9453b4
source-git-commit: 79822d258642675331e1998dd3552e3078db41f8
workflow-type: tm+mt
source-wordcount: '764'
ht-degree: 5%

---

# Projekt kopieren

<!--
<(LINKED TO THE PRODUCT IN THE COPY PROJECT BOX)</p>
-->

Sie können ein Projekt kopieren, anstatt es von Grund auf neu zu erstellen. Sie können jeweils nur ein Projekt kopieren. Sie können keine Projekte in großen Mengen kopieren.

>[!IMPORTANT]
>
>Die folgenden Elemente werden nie aus einem vorhandenen Projekt in ein neues kopiert:
>
>* Probleme
>* Abrechnungssätze
>* Rechnungsnachweise
>* Notizen
>* Stunden
>* Projektübergreifende Vorkenntnisse
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
>* Standardinformationen für Aufgaben (Prozess für die Standardgenehmigung für Aufgaben, benutzerdefinierte Forms für Aufgaben)
>
> Die Daten der ursprünglichen Aufgaben auf den Projekten werden in das neue Projekt kopiert. Sie müssen das Start- oder Abschlussdatum des Projekts ändern (je nach Zeitplan-Modus), um die Daten für die Aufgaben zu aktualisieren. Aufgabeneinschränkungen verhindern möglicherweise, dass Sie die Daten des Projekts ändern.

## Zugriffsanforderungen

<!-- drafted for P&P:
<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>Adobe Workfront plan*</p> </td> 
   <td>Any</td> 
  </tr> 
  <tr> 
   <td> <p>Adobe Workfront license*</p> </td> 
   <td> <p>Current license: Standard </p> 
   Or
   <p>Legacy license: Plan </p>
   </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><strong>Access level configurations*</strong> </td> 
   <td> <p>Edit access to Projects with ability to Create <span>and Copy</span> projects</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><strong>Object permissions</strong> </p> </td> 
   <td> <p>View permissions or higher to the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->
Sie müssen über Folgendes verfügen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>Adobe Workfront-Plan*</p> </td> 
   <td>Beliebig</td> 
  </tr> 
  <tr> 
   <td> <p>Adobe Workfront-Lizenz*</p> </td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><strong>Konfigurationen auf Zugriffsebene*</strong> </td> 
   <td> <p>Bearbeiten des Zugriffs auf Projekte mit der Möglichkeit zum Erstellen <span>und kopieren</span> Projekte</p> <p><b>NOTIZ</b>

Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsstufe ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td>
</tr> 
  <tr data-mc-conditions=""> 
   <td> <p><strong>Objektberechtigungen</strong> </p> </td> 
   <td> <p>Anzeigen von Berechtigungen oder höher für das Projekt</p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Kopieren einzelner Projekte

Beim Kopieren eines Projekts werden auch einige Informationen aus dem ursprünglichen Projekt in das neue Projekt kopiert. Sie können auch angeben, welche Elemente während des Kopiervorgangs nicht in das neue Projekt kopiert werden sollen.

So kopieren Sie ein Projekt:

1. Wechseln Sie zu dem Projekt, das Sie kopieren möchten, und klicken Sie auf das **Mehr** icon ![](assets/qs-more-menu.png) rechts neben dem Projektnamen

   ![](assets/project-level-more-drop-down-expanded-nwe-350x516.png)

   Oder

   Wechseln Sie zu einer Projektliste oder einem Bericht und wählen Sie ein Projekt aus. Klicken Sie dann auf das **Mehr** icon ![](assets/qs-more-menu.png) oben in der Liste.

   ![](assets/more-menu-expanded-in-a-list-one-project-selected-nwe.png)

1. Klicken **Kopieren**.

1. Aktualisieren Sie den Namen des neuen Projekts.

   Standardmäßig lautet der neue Name **Kopie von `<Original project name>`.**

   ![](assets/copy-project-box-nwe-350x276.png)

1. Wählen Sie die **Status** für das neue Projekt.

   Standardmäßig wird die **Status** entspricht dem des ursprünglichen Projekts.

1. (Optional) Heben Sie die Auswahl der Elemente auf, die Sie nicht in das neue Projekt kopieren möchten. In der folgenden Tabelle wird beschrieben, was passiert, wenn Sie die Elemente deaktivieren:


   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Alle auswählen</td> 
      <td> <p>Wählt alle Optionen aus und löscht alle im neuen Projekt aufgelisteten Felder und Objekte.</p> <p><b>TIPP</b>

   Auswahl aufheben <strong>Alle auswählen</strong> Hebt die Auswahl aller Elemente auf. </p> </td>
   </tr> 
     <tr> 
      <td role="rowheader">Arbeitsaufträge</td> 
      <td>Entfernt alle Projekt- und Aufgabenzuweisungen</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Fortschritt</td> 
      <td>Entfernt den Fortschritt aller Aufgaben und sie werden als "Neu"angezeigt. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Benutzerdefinierte Daten</td> 
      <td> <p>Entfernt die Informationen aus dem benutzerdefinierten Formular im Projekt sowie die Informationen zu den benutzerdefinierten Formularen, die mit den folgenden Elementen verknüpft sind:</p> 
       <ul> 
        <li>Aufgaben</li> 
        <li>Ausgaben</li> 
        <li> Dokumente</li> 
       </ul> <p><b>NOTIZ</b>

   Die benutzerdefinierten Formulare bleiben an die Aufgaben, Ausgaben, Dokumente und das Projekt angehängt, die Informationen in den benutzerdefinierten Feldern der Formulare werden jedoch nicht in das neue Projekt kopiert. </p> </td>
   </tr> 
     <tr> 
      <td role="rowheader">Dokumente</td> 
      <td> <p>Entfernt alle Elemente auf der Registerkarte "Dokumente", einschließlich Dokumentversionen, verknüpften Dokumenten und Ordnern.</p> <p>Standardmäßig können Dokumentsendungen und -genehmigungen nicht in ein anderes Projekt kopiert werden. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Alle Vorgänger</td> 
      <td> <p>Entfernt alle Vorgängerbeziehungen zwischen den Aufgaben im Projekt. </p> <p><b>TIPP</b>

   Projektübergreifende Vorgänger werden nie in das neue Projekt übertragen, unabhängig davon, ob dies ausgewählt ist oder nicht. </p> </td>
   </tr>

<tr> 
      <td role="rowheader">Veranschlagte Stunden</td> 
      <td> <p>Entfernt die im Bereich Ressourcenplanung des Geschäftsszenarios des Projekts vorgesehenen Stunden aus dem kopierten Projekt.</p>

<b>NOTIZ</b>

Mit dem Szenario-Planer in den Haushalt eingestellte Stunden werden nie in das neue Projekt kopiert, da das neue Projekt nicht mit einer Initiative im Szenario-Planer verknüpft ist. Weitere Informationen finden Sie unter <a href="../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case-use-scenario-planner.md">Budgetressourcen im Geschäftsfall mit dem Szenario-Planer</a>
</tr></td>
    <tr> 
      <td role="rowheader">Finanzinformationen</td> 
      <td> <p>Entfernt die Informationen in den folgenden Bereichen: </p> 
       <ul> 
        <li>Unterregisterkarte "Finanzen"des Projekts</li> 
        <li> Geplanter Vorteil im Geschäftsfall</li> 
        <li>Finanzinformationen zu allen Aufgaben<br></li> 
       </ul> <p>Weitere Informationen zur Unterregisterkarte "Projekt-Finanzen"finden Sie unter <a href="../../../manage-work/projects/project-finances/manage-project-finance-area.md" class="MCXref xref">Informationen im Bereich "Projekt-Finanzen"verwalten</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Genehmigungsprozess</td> 
      <td>Entfernt alle Genehmigungen, die mit den Aufgaben oder dem Projekt verknüpft sind. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Erinnerungsnachrichten</td> 
      <td> Entfernt die mit den Aufgaben oder dem Projekt verknüpften Erinnerungsbenachrichtigungen. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ausgaben</td> 
      <td>Entfernt Ausgaben, die mit den Aufgaben oder dem Projekt verbunden sind. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Berechtigungen</td> 
      <td> Entfernt Berechtigungen für alle Benutzer der Aufgaben oder des Projekts.</td> 
     </tr> 
    </tbody> 
   </table>

1. Klicken **Kopieren** , um eine Kopie des Projekts zu erstellen.

   Dadurch wird ein neues Projekt erstellt, das dem kopierten Projekt ähnlich ist.

   Sie können Änderungen am neuen kopierten Projekt vornehmen, z. B. Aufgabenzuweisungen überprüfen oder Zeitpläne anpassen.
