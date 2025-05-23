---
product-area: templates
navigation-topic: templates-navigation-topic
title: Vorlage aus Projekt erstellen
description: Beim Speichern eines vorhandenen Projekts als Vorlage können Sie Vorlagen erstellen.
author: Alina
feature: Work Management, Projects
role: User
exl-id: 923deab4-205b-4312-9ec4-4471fd6cea26
source-git-commit: f21fd0761d942916039f6364e62f489a07217bfe
workflow-type: tm+mt
source-wordcount: '493'
ht-degree: 1%

---

# Vorlage aus Projekt erstellen

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(Note: Keep this article in the Creating and Managing Templates area with the detailed information that this contains. Since this is an article about creating TEMPLATES, this needs to be detailed under Templates; there is a similar article with almost the same title in Managing projects that points to this one - since this functionality is in the UI under Projects, this article must have a presence in that areas as well. Keep both, but make this one the only editable one (iterative))</p>
-->

Beim Speichern eines vorhandenen Projekts als Vorlage können Sie Vorlagen erstellen.

Nachdem Sie ein vorhandenes Projekt als Vorlage gespeichert haben, können Sie die neue Vorlage verwenden, um neue Projekte zu erstellen. Dies vereinfacht und beschleunigt den Projekterstellungsprozess.

>[!NOTE]
>
>Beim Speichern eines Projekts als Vorlage werden die tatsächlichen Daten der Aufgaben und des Projekts nicht für die Vorlage gespeichert.
>
>Eine Vorlage und ihre Aufgaben haben keine tatsächlichen Daten, sondern einen Hinweis darauf, an welchem Tag (ab dem das zukünftige Projekt beginnen könnte) eine Aufgabe beginnen könnte und an welchem Tag sie abgeschlossen werden muss. Wenn Sie Vorlagen zur Erstellung künftiger Projekte verwenden, erhalten die Projekte tatsächliche Termine. Weitere Informationen finden Sie unter [Erstellen eines Projekts](../create-projects/create-project.md).

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
   <td role="rowheader">Konfigurationen der Zugriffsebene*</td> 
   <td> <p>Zugriff auf Vorlagen bearbeiten</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Einschränkungen in Ihrer Zugriffsebene festgelegt hat. Informationen dazu, wie Workfront-Admins Ihre Zugriffsebene ändern können, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Erstellen oder Ändern benutzerdefinierter Zugriffsebenen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Anzeigen oder Erweitern von Berechtigungen für ein Projekt </p> <p>Sie erhalten Verwaltungsberechtigungen für die Vorlage, nachdem Sie sie erstellt haben</p> <p>Informationen zum Anfordern zusätzlicher Zugriffsberechtigungen finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Anfordern von Zugriffsberechtigungen für Objekte </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um herauszufinden, über welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie verfügen.

## Vorlage aus Projekt erstellen

1. Wechseln Sie zu dem Projekt, das Sie als Vorlage speichern möchten.
1. Klicken Sie auf das **Mehr**-Menü ![Mehr-Symbol](assets/qs-more-icon-on-an-object.png) und dann **Als Vorlage speichern**.
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
      <td>Geben Sie eine Beschreibung für die Vorlage an.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ist aktiv</td> 
      <td> <p>Wählen Sie aus den folgenden Optionen aus:</p> 
       <ul> 
        <li> <p><strong>Ja</strong>: Andere Benutzer können die Vorlage finden und sie an Projekte anhängen.</p> </li> 
        <li><strong>Nein</strong>: Andere Benutzer können die Vorlage nicht finden und sie nicht an Projekte anhängen.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Benutzerdefinierte Formulare</td> 
      <td>Verwenden Sie die Dropdown-Liste, um benutzerdefinierte Formulare auszuwählen, die an die Vorlage angehängt werden sollen. Wenn bereits benutzerdefinierte Formulare mit dem Projekt verknüpft wurden, werden alle Datenfelder aus diesen benutzerdefinierten Formularen angezeigt.<br>Sie können bis zu 10 benutzerdefinierte Formulare in eine Vorlage aufnehmen.</td> 
     </tr> 
    </tbody> 
   </table>

1. Klicken Sie auf **Forms verwalten**, um die Formulare zu entfernen oder neu anzuordnen. Informationen zum Entfernen und Neuanordnen benutzerdefinierter Formulare aus der Vorlage finden Sie unter [Benutzerdefinierte Formulare](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-and-manage-custom-forms.md).

   ![Als Vorlage speichern erster Schritt](assets/save-as-template-first-step-350x159.png)

1. Klicken Sie auf **Nächster Schritt.**
1. Aktivieren **im Abschnitt Optionen** Kontrollkästchen neben den Informationen, die Sie aus der Vorlage entfernen möchten.

   ![Als Vorlagenoptionen speichern](assets/save-as-template-options-step-350x109.png)

1. Klicken Sie auf **Nächster Schritt.**
1. Wählen Sie im **Ausschließen** alle Aufgaben aus, die Sie aus dem Projekt ausschließen möchten.

   ![Als Vorlage speichern ausschließen](assets/save-as-template-exclude-350x205.png)

1. Klicken Sie auf **Beenden und Vorlage speichern.**

   Ihre Vorlage wird jetzt in der Liste der verfügbaren Vorlagen angezeigt und kann entweder an ein vorhandenes Projekt angehängt oder zum Erstellen eines neuen verwendet werden.

 
