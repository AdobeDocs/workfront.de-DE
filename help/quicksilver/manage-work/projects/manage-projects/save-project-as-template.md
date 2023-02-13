---
product-area: projects;templates
navigation-topic: manage-projects
title: Projekt als Vorlage speichern
description: Speichern Sie ein Projekt als Vorlage "Als Vorlage speichern"auf Projektebene, damit Benutzer dies in der Benutzeroberfläche sehen; Es gibt einen weiteren Artikel, zu dem dieser Link ausführlicher (Schritt für Schritt) ist. Diese Funktion muss sowohl in Projekt- als auch in Vorlagenbereichen verbleiben.)"
author: Alina
feature: Work Management
exl-id: 4b5dfe12-f984-47c6-8e19-78b549f19159
source-git-commit: dc3461803e23f61877c31efa2c52fffdc7bd79bf
workflow-type: tm+mt
source-wordcount: '449'
ht-degree: 2%

---

# Projekt als Vorlage speichern

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Keep this the way it is in the Managing Projects area because the functionality in the UI is "Save as template" at the project level, so users see that in the UI; there is another article that this links to which is more in depth (step-by-step). This functionality needs to stay in both projects AND templates areas.)</p>
-->

Wenn Sie sich entscheiden, dass ein Projekt irgendwann in der Zukunft erneut durchgeführt wird, können Sie eine Vorlage aus diesem vorhandenen Projekt erstellen. Anschließend können Sie die Vorlage erneut verwenden, um zukünftige Projekte zu erstellen, die möglicherweise ähnliche Informationen enthalten oder dieselbe Timeline oder dieselben Zuweisungen für das vorhandene Projekt freigeben.

## Zugriffsanforderungen

<!--drafted for P&P:
<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Standard </p>
   Or 
   <p>Legacy license: Plan </p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Templates</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View or higher permissions to a project </p> <p>You obtain Manage permissions to the template after you save the project as a template</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Beliebig </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf Vorlagen bearbeiten</p> <p><b>NOTIZ</b>

Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Anzeigen von oder höheren Berechtigungen für ein Projekt </p> <p>Sie erhalten nach dem Speichern des Projekts als Vorlage Verwaltungsberechtigungen für die Vorlage.</p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Projekt als Vorlage speichern

1. Wechseln Sie zu dem Projekt, das Sie als Vorlage speichern möchten.
1. Klicken Sie auf **Mehr** Menü ![](assets/qs-more-icon-on-an-object.png), dann **Als Vorlage speichern**.
1. Geben Sie die folgenden Informationen für die Vorlage an:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Name</td> 
      <td>Geben Sie einen Namen für die Vorlage an.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Beschreibung</td> 
      <td>Geben Sie eine Beschreibung für die Vorlage ein.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ist aktiv</td> 
      <td> <p>Wählen Sie aus den folgenden Optionen aus:</p> 
       <ul> 
        <li> <p><strong>Ja</strong>: Andere Benutzer können die Vorlage finden und an Projekte anhängen.</p> </li> 
        <li><strong>Nein</strong>: Andere Benutzer können die Vorlage nicht finden und nicht an Projekte anhängen.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Benutzerdefinierte Formulare</td> 
      <td>Wählen Sie in der Dropdown-Liste alle benutzerdefinierten Formulare aus, die an die Vorlage angehängt werden sollen. Wenn dem Projekt bereits benutzerdefinierte Formulare zugeordnet wurden, werden alle Datenfelder aus diesen benutzerdefinierten Formularen angezeigt.<br>Sie können bis zu 10 benutzerdefinierte Formulare in eine Vorlage aufnehmen.</td> 
     </tr> 
    </tbody> 
   </table>

1. Klicken **Verwalten von Forms** , um die Formulare zu entfernen oder neu anzuordnen. Informationen zum Entfernen und Neuanordnen von benutzerdefinierten Formularen in der Vorlage finden Sie unter [Benutzerdefinierte Formulare](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-and-manage-custom-forms.md).

   ![](assets/save-as-template-first-step-350x159.png)

1. Klicken **Nächster Schritt.**
1. Im **Optionen** aktivieren Sie das Kontrollkästchen neben allen Informationen, die Sie aus der Vorlage löschen möchten.

   ![](assets/save-as-template-options-step-350x109.png)

1. Klicken **Nächster Schritt.**
1. Im **Ausschließen** auswählen Sie alle Aufgaben, die Sie aus dem Projekt ausschließen möchten.

   ![](assets/save-as-template-exclude-350x205.png)

1. Klicken **Vorlage abschließen und speichern**

   Ihre Vorlage wird jetzt in der Liste der verfügbaren Vorlagen angezeigt und kann entweder an ein vorhandenes Projekt angehängt oder zum Erstellen eines neuen Projekts verwendet werden.
