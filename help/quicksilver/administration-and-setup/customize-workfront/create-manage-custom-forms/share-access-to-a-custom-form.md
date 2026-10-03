---
title: Freigeben eines benutzerdefinierten Formulars
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: Sie können den Zugriff für ein benutzerdefiniertes Formular konfigurieren, um zu steuern, wer es anzeigen, freigeben und bearbeiten kann.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: a264512f-54ab-426e-8dd7-5602ece81c57
TQID: 'https://experienceleague.adobe.com/gpJQedqcdtjaxvhVuWKgJVpfAPAT2ICSgO6nRFLvimM'
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
  - id: d5896d07-2812-5418-8b18-8957a0d7f0fb
    internal-label: System Setup and Administration
subfeature_v2:
  - id: d87de1f9-8e24-4c4d-aa4c-a403075091a1
    internal-label: Custom forms
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: ecee8b1aadd804a45ff0830e04e77981a3269cff
workflow-type: tm+mt
source-wordcount: '967'
ht-degree: 5%
---
# Freigeben eines benutzerdefinierten Formulars

Sie können den Zugriff für ein benutzerdefiniertes Formular konfigurieren, um zu steuern, wer es anzeigen, freigeben und bearbeiten kann - Person, Rolle, Gruppe, Team, Unternehmen, Geschäftsprofil.

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront-Paket</td> 
   <td><p>Beliebig</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront-Lizenz</td> 
   <td><p>Standard</p>
       <p>Abo</p></td>
  </tr> 
  <tr> 
   <td>Konfigurationen der Zugriffsebene</td> 
   <td> <p>Administrativer Zugriff auf benutzerdefinierte Formulare</p> </td> 
  </tr>  
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Zugriff auf benutzerdefinierte Formulare {#access-to-custom-forms}

Wenn Sie ein neues benutzerdefiniertes Formular erstellen und jemand es an ein Objekt anhängt, kann standardmäßig jeder Benutzer, der dem Objekt zugewiesen ist, das Formular anzeigen und ausfüllen. Dazu gehören Benutzer mit einer Beitragenden - oder Anfragelizenz sowie externe Benutzer.

Bei einem Objekt, an das das benutzerdefinierte Formular noch nicht angehängt wurde, kann ein Benutzer (selbst wenn er über eine Standard- oder Planerzugriffsebene verfügt) es jedoch nicht über das Dropdown-Menü Benutzerdefinierte Forms anhängen, es sei denn, einer der folgenden Punkte ist erfüllt:

* Jemand hat das benutzerdefinierte Formular als „Jeder im System kann anzeigen und anhängen“ freigegeben.
* Jemand hat das benutzerdefinierte Formular für den Benutzer oder dessen Team, Aufgabengebiet, Gruppe, Unternehmen oder Geschäftsprofil freigegeben, wobei mindestens die Berechtigung zum Anzeigen mit der ausgewählten Option „An benutzerdefinierte Daten anhängen“ gewährt wurde
* Der Benutzer verfügt über eine Standard- oder Planlizenz und die Zugriffsebene ermöglicht den administrativen Zugriff auf benutzerdefinierte Formulare

## Freigeben eines benutzerdefinierten Formulars

Anstatt ein benutzerdefiniertes Formular im Standardfreigabestatus zu belassen (beschrieben unter [Zugriff auf benutzerdefinierte Formulare](#access-to-custom-forms) in diesem Artikel), können Sie bestimmte Zugriffsebenen für das Formular für bestimmte Benutzer, Aufgabengebiete, Gruppen, Teams, Unternehmen und Geschäftsprofile konfigurieren.

{{step-1-to-setup}}

1. Klicken Sie im linken Bedienfeld auf **Benutzerdefinierte Forms**.
1. Wählen Sie das benutzerdefinierte Formular in der Liste aus und klicken Sie dann auf ![Freigabesymbol](assets/share-icon.png).

   ODER

   Ein benutzerdefiniertes Formular öffnen oder ein neues benutzerdefiniertes Formular erstellen. Klicken Sie dann oben **im Formular** Designer auf „Freigeben“.

1. Geben Sie im Freigabefeld unter **Zugriff auf benutzerdefinierte Formulare gewähren** den Namen des Benutzers, Teams, Aufgabengebiets, der Gruppe, des Unternehmens oder des Geschäftsprofils ein, für den Sie das benutzerdefinierte Formular freigeben möchten, und drücken Sie dann die **Eingabetaste** wenn der Name angezeigt wird.
1. Um den Zugriff für den soeben hinzugefügten Benutzer, das Team, das Aufgabengebiet, die Gruppe, das Unternehmen oder das Geschäftsprofil anzupassen, klicken Sie auf das Dropdown-Menü rechts neben dem Namen und konfigurieren Sie dann eine der folgenden verfügbaren Optionen und eine ihrer erweiterten Einstellungen:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Ansicht</td> 
      <td> <p>Diese Option bietet die Möglichkeit, das benutzerdefinierte Formular für Objekte anzuzeigen und auszufüllen. Auf Objektebene müssen Benutzer außerdem mindestens über Beitragszugriff verfügen, wenn die erweiterte Einstellung <strong>Benutzerdefiniertes Formular bearbeiten</strong> aktiviert ist. Wenn das Formular beispielsweise an ein Projekt angehängt ist, müssen Benutzende Beitragszugriff auf dieses Projekt haben, sonst können sie das Formular nicht ausfüllen.</p>

   <p><b>HINWEIS</b>: Für Benutzende mit Light- und Contributor-Lizenzen (oder Arbeits-, Prüfungs- und Anfragelizenzen) ist dies die höchste verfügbare Option.</p> <p>Klicken Sie <strong>Erweiterte Einstellungen</strong>, um anzugeben, ob Folgendes zulässig sein soll:</p> 
       <ul> 
        <li><strong>An benutzerdefinierte Daten anhängen</strong>: Möglichkeit, das benutzerdefinierte Formular an Projekte, Aufgaben und Probleme anzuhängen, für die sie Verwaltungszugriff haben</li> 
        <li> <p><strong>Freigeben</strong>: Möglichkeit, das benutzerdefinierte Formular für andere Personen im System freizugeben</p> <p>Benutzende mit einer Light- oder Contributor-Lizenz (oder Arbeits-, Prüfungs- oder Anfragelizenz) können ein benutzerdefiniertes Formular nur über die API oder einen benutzerdefinierten Formularbericht freigeben.</p> </li>
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Verwalten</td> 
      <td> <p>Diese Option ist nur für Benutzer mit einer Standard- oder Planlizenz verfügbar. </p> <p>Benutzer können das Formular nicht nur zu Objekten hinzufügen, auf die sie Zugriff haben, um es zu bearbeiten, sondern auch das benutzerdefinierte Formular vollständig bearbeiten, einschließlich Felder hinzufügen, bearbeiten und löschen.</p> <p>Klicken Sie <strong>Erweiterte Einstellungen</strong>, um anzugeben, ob Folgendes zulässig sein soll:</p> 
       <ul> 
        <li> <p><strong>An benutzerdefinierte Daten anhängen</strong>: Möglichkeit, das benutzerdefinierte Formular an Projekte, Aufgaben und Probleme anzuhängen, für die sie Verwaltungszugriff haben</p> </li> 
        <li><strong>Löschen</strong>: Löschen des benutzerdefinierten Formulars aus dem System</li> 
        <li><strong>Freigeben</strong>: Freigeben des benutzerdefinierten Formulars für andere Personen im System</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Optional) Wiederholen Sie die Schritte 4 bis 5, um der Liste weitere Namen hinzuzufügen und ihre Optionen zu konfigurieren.
1. (Optional) Wenn Sie den Zugriff auf das benutzerdefinierte Formular (auf Objekte, an die es angehängt ist) auf die in den vorherigen Schritten angegebenen beschränken möchten, klicken Sie auf den Dropdown-Pfeil unter **Wer hat Zugriff** und wählen Sie dann **Nur eingeladene Personen können Zugriff**.

   Wenn Sie Ihre Meinung ändern, können Sie **Alle im System können anzeigen** auswählen.

   >[!NOTE]
   >
   >* Wenn Sie ein benutzerdefiniertes Formular systemweit sichtbar machen, lassen Sie es Benutzerinnen und Benutzern nur für die Objekte anzeigen und ausfüllen, denen sie zugewiesen sind, nicht aber, es an andere Objekte anzuhängen. Sie können das benutzerdefinierte Formular mit der Option „An benutzerdefinierte Daten anhängen“, die in Schritt 5 erläutert wird, an Objekte anhängen.
   >* Die meisten Unternehmen möchten sicherstellen, dass jeder im System ein benutzerdefiniertes Formular ausfüllen kann, wenn es an Objekte angehängt wird, an denen er arbeitet, und seine Daten in Berichten anzeigen kann. Wenn dies für Ihre Organisation zutrifft, empfehlen wir die Verwendung von **Jeder im System kann anzeigen**.
   >* Wenn Sie die **Alle im System können anzeigen und anhängen** auswählen, können alle Benutzer das Formular an andere Objekte anhängen.
   >
   >![Benutzerdefiniertes Formular freigeben](assets/share-custom-forms-all-can-attach.png)
   >   
   >Wenn Sie Bedenken bei einem benutzerdefinierten Formular haben, bei dem Benutzer möglicherweise vertrauliche Daten eingeben, wenn sie an bestimmte Objekte angehängt sind, ist es möglicherweise effektiver, die Freigabe für diese *Objekte* zu beschränken, anstatt den Zugriff auf das Formular selbst zu beschränken.

1. Klicken Sie auf **Speichern**.

## Entfernen des Zugriffs auf ein benutzerdefiniertes Formular

{{step-1-to-setup}}

1. Klicken Sie im linken Bedienfeld auf **Benutzerdefinierte Forms**.
1. Wählen Sie das benutzerdefinierte Formular in der Liste aus und klicken Sie dann auf ![Freigabesymbol](assets/share-icon.png).
1. Klicken Sie im Freigabefeld auf das Dropdown-Menü rechts neben dem Namen des Benutzers, Teams, der Rolle, der Gruppe, der Firma oder des Geschäftsprofils, auf die bzw. das Sie keinen besonderen Zugriff mehr auf das Formular haben möchten, und wählen Sie **Entfernen**.
1. (Optional) Wiederholen Sie den vorherigen Schritt für andere Namen, die Sie entfernen möchten.
1. Klicken Sie auf **Speichern**.

