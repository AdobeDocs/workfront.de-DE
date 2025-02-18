---
title: Freigeben eines benutzerdefinierten Formulars
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: Sie können den Zugriff für ein benutzerdefiniertes Formular konfigurieren, um zu steuern, wer es anzeigen, freigeben und bearbeiten kann - Person, Rolle, Gruppe, Team, Unternehmen.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: a264512f-54ab-426e-8dd7-5602ece81c57
source-git-commit: 2a356b2cc98f8226d2a616cdd907a3aebaeecee0
workflow-type: tm+mt
source-wordcount: '1530'
ht-degree: 0%

---

# Freigeben eines benutzerdefinierten Formulars

Sie können den Zugriff für ein benutzerdefiniertes Formular konfigurieren, um zu steuern, wer es anzeigen, freigeben und bearbeiten kann - Person, Rolle, Gruppe, Team, Unternehmen.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über Folgendes verfügen, um die Schritte in diesem Artikel auszuführen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Adobe Workfront-Plan</p> </td> 
   <td>Beliebig</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td>
   <p>Neu: Standard</p>
   <p>oder</p>
   <p>Aktuell: Plan</p></td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Administrativer Zugriff auf benutzerdefinierte Formulare</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Zugriff auf benutzerdefinierte Formulare {#access-to-custom-forms}

Wenn Sie ein neues benutzerdefiniertes Formular erstellen und jemand es an ein Objekt anhängt, kann standardmäßig jeder Benutzer, der dem Objekt zugewiesen ist, das Formular anzeigen und ausfüllen. Dazu gehören Benutzer mit Anfragelizenzen und externe Benutzer.

Bei einem Objekt, an das das benutzerdefinierte Formular noch nicht angehängt wurde, kann ein Benutzer (selbst wenn er über eine Zugriffsebene für Planer verfügt) es jedoch nicht über das Dropdown-Menü Benutzerdefinierte Forms anhängen, es sei denn, einer der folgenden Punkte ist erfüllt:

* Jemand hat das benutzerdefinierte Formular für den Benutzer oder dessen Team, Aufgabengebiet, Gruppe oder Unternehmen freigegeben und gewährt mindestens die Berechtigung zum Anzeigen mit der ausgewählten Option „An benutzerdefinierte Daten anhängen“
* Der Benutzer verfügt über eine Planlizenz und die Zugriffsebene erlaubt administrativen Zugriff auf benutzerdefinierte Formulare

## Freigeben eines benutzerdefinierten Formulars aus der Formularliste

Anstatt ein benutzerdefiniertes Formular im Standardfreigabestatus zu belassen (beschrieben unter [Zugriff auf benutzerdefinierte Formulare](#access-to-custom-forms) in diesem Artikel), können Sie bestimmte Zugriffsebenen für das Formular für bestimmte Benutzer, Aufgabengebiete, Gruppen, Teams und Unternehmen konfigurieren.

{{step-1-to-setup}}

1. Klicken Sie im linken Bedienfeld auf **Benutzerdefinierte Forms**.
1. Wählen Sie das benutzerdefinierte Formular aus und klicken Sie dann auf ![Freigabesymbol](assets/share-icon.png).
1. Geben Sie in das angezeigte Feld unter **Zugriff auf benutzerdefinierte Formulare erteilen** den Namen des Benutzers, Teams, Aufgabengebiets, der Gruppe oder des Unternehmens ein, für den bzw. das Sie das benutzerdefinierte Formular freigeben möchten, und drücken Sie dann die **Eingabetaste** wenn der Name angezeigt wird.
1. Um den Zugriff für den soeben hinzugefügten Benutzer, das Team, das Aufgabengebiet, die Gruppe oder das Unternehmen anzupassen, klicken Sie auf das Dropdown-Menü rechts neben dem Namen und konfigurieren Sie dann eine der folgenden verfügbaren Optionen und eine seiner erweiterten Einstellungen:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Anzeigen</td> 
      <td> <p>Diese Option bietet die Möglichkeit, das benutzerdefinierte Formular für Objekte anzuzeigen und auszufüllen. Auf Objektebene müssen Benutzer außerdem mindestens über Beitragszugriff verfügen, wenn die erweiterte Einstellung <strong>Benutzerdefiniertes Formular bearbeiten</strong> aktiviert ist. Wenn das Formular beispielsweise an ein Projekt angehängt ist, müssen Benutzende Beitragszugriff auf dieses Projekt haben, sonst können sie das Formular nicht ausfüllen.</p>

   <p><b>HINWEIS</b>: Für Benutzende mit Light- und Contributor-Lizenzen (oder Arbeits-, Prüfungs- und Anfragelizenzen) ist dies die höchste verfügbare Option.</p>

   <p>Klicken Sie <strong>Erweiterte Einstellungen</strong>, um anzugeben, ob Folgendes zulässig sein soll:</p> 
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
1. (Optional) Wenn Sie den Zugriff auf das benutzerdefinierte Formular (auf Objekte, an die es angehängt ist) auf die in den vorherigen Schritten angegebenen beschränken möchten, klicken Sie auf das Zahnradsymbol ![](assets/gear-icon-settings-with-dn-arrow.jpg) in der oberen rechten Ecke des Freigabefelds und dann auf **Systemweiten Zugriff entfernen**.

   Wenn Sie Ihre Meinung ändern, können Sie auf **Systemweit sichtbar machen** (Standardoption) klicken.

   >[!NOTE]
   >
   >* Wenn Sie ein benutzerdefiniertes Formular systemweit sichtbar machen, lassen Sie es Benutzerinnen und Benutzern nur für die Objekte anzeigen und ausfüllen, denen sie zugewiesen sind, nicht aber, es an andere Objekte anzuhängen. Sie können das benutzerdefinierte Formular mit der Option „An benutzerdefinierte Daten anhängen“, die in Schritt 5 erläutert wird, an Objekte anhängen.
   >* Die meisten Unternehmen möchten sicherstellen, dass jeder im System ein benutzerdefiniertes Formular ausfüllen kann, wenn es an Objekte angehängt wird, an denen er arbeitet, und seine Daten in Berichten anzeigen kann. Wenn dies für Ihr Unternehmen zutrifft, empfehlen wir, **Systemweit sichtbar machen** zu verwenden. Wenn die Option auf diese Weise konfiguriert ist, wird im Dialogfeld „Systemweit sichtbar“ angezeigt:
   >   
   >![](assets/visible-system-wide-350x480.png)
   >   
   >Wenn Sie Bedenken bei einem benutzerdefinierten Formular haben, bei dem Benutzer möglicherweise vertrauliche Daten eingeben, wenn es an bestimmte Objekte angehängt ist, ist es möglicherweise besser, die Freigabe für diese *Objekte* einzuschränken, anstatt den Zugriff auf das Formular selbst zu beschränken.

1. Klicken Sie auf **Speichern**.

## Freigeben eines benutzerdefinierten Formulars im Formular-Designer

{{step-1-to-setup}}

1. Klicken Sie im linken Bedienfeld auf **Benutzerdefinierte Forms**.
1. Ein benutzerdefiniertes Formular öffnen oder ein neues benutzerdefiniertes Formular erstellen.
1. Klicken **oben rechts** Formular-Designer auf „Freigeben“, wenn Sie zum Freigeben des Formulars bereit sind.
1. Beginnen Sie in dem angezeigten Feld unter **Zugriff auf benutzerdefinierte Formulare gewähren** mit der Eingabe des Namens des Benutzers, Teams, Aufgabengebiets, der Gruppe oder des Unternehmens, für den bzw. die Sie das benutzerdefinierte Formular freigeben möchten, und drücken Sie dann die **Eingabetaste** wenn der Name angezeigt wird.
1. Um den Zugriff für den soeben hinzugefügten Benutzer, das Team, das Aufgabengebiet, die Gruppe oder das Unternehmen anzupassen, klicken Sie auf das Dropdown-Menü rechts neben dem Namen und konfigurieren Sie dann eine der folgenden verfügbaren Optionen und eine seiner erweiterten Einstellungen:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Anzeigen</td> 
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

1. (Optional) Wiederholen Sie die Schritte 5 bis 6, um der Liste weitere Namen hinzuzufügen und ihre Optionen zu konfigurieren.
1. (Optional) Wenn Sie den Zugriff auf das benutzerdefinierte Formular (auf Objekte, an die es angehängt ist) auf die in den vorherigen Schritten angegebenen beschränken möchten, klicken Sie auf den Dropdown-Pfeil unter **Wer hat Zugriff** und wählen Sie dann **Nur eingeladene Personen können Zugriff**.

   Wenn Sie Ihre Meinung ändern, können Sie **Alle im System können anzeigen** auswählen.

   >[!NOTE]
   >
   >* Wenn Sie ein benutzerdefiniertes Formular systemweit sichtbar machen, lassen Sie es Benutzerinnen und Benutzern nur für die Objekte anzeigen und ausfüllen, denen sie zugewiesen sind, nicht aber, es an andere Objekte anzuhängen. Sie können das benutzerdefinierte Formular mit der Option „An benutzerdefinierte Daten anhängen“, die in Schritt 6 erläutert wird, an Objekte anhängen.
   >* Die meisten Unternehmen möchten sicherstellen, dass jeder im System ein benutzerdefiniertes Formular ausfüllen kann, wenn es an Objekte angehängt wird, an denen er arbeitet, und seine Daten in Berichten anzeigen kann. Wenn dies für Ihre Organisation zutrifft, empfehlen wir die Verwendung von **Jeder im System kann anzeigen**. Wenn die Option auf diese Weise konfiguriert ist, wird im Dialogfeld „Systemweit sichtbar“ angezeigt:
   >   
   >![Benutzerdefiniertes Formular freigeben](assets/share-custom-form-in-designer.png)
   >   
   >Wenn Sie Bedenken bei einem benutzerdefinierten Formular haben, bei dem Benutzer möglicherweise vertrauliche Daten eingeben, wenn es an bestimmte Objekte angehängt ist, ist es möglicherweise besser, die Freigabe für diese *Objekte* einzuschränken, anstatt den Zugriff auf das Formular selbst zu beschränken.

1. Klicken Sie auf **Speichern**.

## Entfernen des Zugriffs auf ein benutzerdefiniertes Formular aus der Formularliste

{{step-1-to-setup}}

1. Klicken Sie im linken Bedienfeld auf **Benutzerdefinierte Forms**.
1. Wählen Sie das benutzerdefinierte Formular aus und klicken Sie dann auf ![Freigabesymbol](assets/share-icon.png).
1. Klicken Sie in dem angezeigten Feld rechts neben dem Namen des Benutzers, Teams, der Rolle, der Gruppe oder des Unternehmens auf das X, dem bzw. der Sie keinen besonderen Zugriff mehr auf das Formular gewähren möchten.
1. (Optional) Wiederholen Sie den vorherigen Schritt bis für andere Namen, die Sie entfernen möchten.
1. Klicken Sie auf **Speichern**.
