---
product-area: templates
navigation-topic: templates-navigation-topic
title: Vorlage aus Projekt erstellen
description: Sie können Vorlagen erstellen, wenn Sie ein vorhandenes Projekt als Vorlage speichern.
author: Alina
feature: Work Management, Projects
role: User
exl-id: 923deab4-205b-4312-9ec4-4471fd6cea26
source-git-commit: 79822d258642675331e1998dd3552e3078db41f8
workflow-type: tm+mt
source-wordcount: '477'
ht-degree: 1%

---

# Vorlage aus Projekt erstellen

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(Note: Keep this article in the Creating and Managing Templates area with the detailed information that this contains. Since this is an article about creating TEMPLATES, this needs to be detailed under Templates; there is a similar article with almost the same title in Managing projects that points to this one - since this functionality is in the UI under Projects, this article must have a presence in that areas as well. Keep both, but make this one the only editable one (iterative))</p>
-->

Sie können Vorlagen erstellen, wenn Sie ein vorhandenes Projekt als Vorlage speichern.

Nachdem Sie ein vorhandenes Projekt als Vorlage gespeichert haben, können Sie die neue Vorlage verwenden, um neue Projekte zu erstellen. Dies vereinfacht und beschleunigt die Projekterstellung.

>[!NOTE]
>
>Beim Speichern eines Projekts als Vorlage werden die tatsächlichen Daten der Aufgaben und des Projekts nicht für die Vorlage gespeichert.
>
>Eine Vorlage und ihre Aufgaben haben keine tatsächlichen Daten, sondern einen Hinweis darauf, an welchem Tag (ab dem Zeitpunkt, zu dem das zukünftige Projekt beginnen kann) eine Aufgabe beginnen kann und an welchem Tag die Aufgabe möglicherweise abgeschlossen werden muss. Wenn Sie Vorlagen zur Erstellung künftiger Projekte verwenden, erhalten die Projekte die tatsächlichen Daten. Weitere Informationen finden Sie unter [Projekt erstellen](../create-projects/create-project.md).

## Zugriffsanforderungen

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
   <td> <p>Zugriff auf Vorlagen bearbeiten</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Anzeigen von oder höheren Berechtigungen für ein Projekt </p> <p>Sie erhalten nach der Erstellung Verwaltungsberechtigungen für die Vorlage</p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Vorlage aus Projekt erstellen

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

 
