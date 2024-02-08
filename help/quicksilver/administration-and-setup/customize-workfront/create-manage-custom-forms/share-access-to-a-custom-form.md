---
title: Freigeben eines benutzerdefinierten Formulars
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: Sie können den Zugriff für ein benutzerdefiniertes Formular konfigurieren, um zu steuern, wer - Person, Rolle, Gruppe, Team, Unternehmen - es anzeigen, freigeben und bearbeiten kann.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: a264512f-54ab-426e-8dd7-5602ece81c57
source-git-commit: 35de4535970d5cd15fcd68f79bf849803f94a77e
workflow-type: tm+mt
source-wordcount: '848'
ht-degree: 1%

---

# Freigeben eines benutzerdefinierten Formulars

{{highlighted-preview}}

Sie können den Zugriff für ein benutzerdefiniertes Formular konfigurieren, um zu steuern, wer - Person, Rolle, Gruppe, Team, Unternehmen - es anzeigen, freigeben und bearbeiten kann.

## Zugriffsanforderungen

Sie müssen über Folgendes verfügen, um die Schritte in diesem Artikel durchzuführen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Adobe Workfront-Abo</p> </td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td>
   <p>Neu: Standard</p>
   <p>oder</p>
   <p>Aktuell: Plan</p></td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Administratorzugriff auf benutzerdefinierte Formulare</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Zugriff auf benutzerdefinierte Formulare {#access-to-custom-forms}

Wenn Sie ein neues benutzerdefiniertes Formular erstellen und es von einer Person an ein Objekt angehängt wird, kann jeder Benutzer, der dem Objekt zugewiesen ist, das Formular standardmäßig anzeigen und ausfüllen. Dazu gehören Benutzer mit Lizenzen anfordern und externe Benutzer.

Bei einem Objekt, an das das benutzerdefinierte Formular noch nicht angehängt ist, kann ein Benutzer (auch wenn er über eine Planner-Zugriffsstufe verfügt) es nicht über das Dropdown-Menü &quot;Benutzerdefinierte Forms&quot;anhängen, es sei denn, eine der folgenden Eigenschaften ist wahr:

* Jemand hat das benutzerdefinierte Formular für den Benutzer oder für das Team, die Rolle, die Gruppe oder das Unternehmen freigegeben und mindestens die Berechtigung zum Anzeigen mit der ausgewählten Option &quot;An benutzerdefinierte Daten anhängen&quot;gewährt.
* Der Benutzer verfügt über eine Planungslizenz und seine Zugriffsstufe ermöglicht den Administratorzugriff auf benutzerdefinierte Formulare

## Freigeben eines benutzerdefinierten Formulars

Anstatt ein benutzerdefiniertes Formular im standardmäßigen Freigabestatus zu hinterlassen (siehe [Zugriff auf benutzerdefinierte Formulare](#access-to-custom-forms) in diesem Artikel) können Sie bestimmte Zugriffsebenen für das Formular für bestimmte Benutzer, Jobrollen, Gruppen, Teams und Unternehmen konfigurieren.

{{step-1-to-setup}}

1. Klicken Sie im linken Bereich auf **Benutzerdefinierte Forms**.
1. Wählen Sie das benutzerdefinierte Formular aus und klicken Sie auf **Freigeben** <span class="preview">oder ![Freigabesymbol](assets/share-icon.png).</span>
1. In dem Feld, das angezeigt wird, unter **Gewähren Sie benutzerdefinierten Formularzugriff an**, beginnen Sie mit der Eingabe des Namens des Benutzers, Teams, der Rolle, Gruppe oder Firma, für die Sie das benutzerdefinierte Formular freigeben möchten, und drücken Sie dann die Eingabetaste **Eingabe** wenn der Name angezeigt wird.
1. Um den Zugriff auf den soeben hinzugefügten Benutzer, das Team, die Rolle, die Gruppe oder das Unternehmen anzupassen, klicken Sie auf das Dropdown-Menü rechts neben dem Namen und konfigurieren Sie dann eine der folgenden verfügbaren Optionen und eine der erweiterten Einstellungen:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Anzeigen</td> 
      <td> <p>Möglichkeit, das benutzerdefinierte Formular für Objekte anzuzeigen und auszufüllen.</p> <p><b>NOTE</b>: Für Benutzer mit Arbeits-, Überprüfungs- und Anforderungslizenzen ist dies die höchste verfügbare Option.</p> <p>Klicks <strong>Erweiterte Einstellungen</strong> um anzugeben, ob Folgendes zulässig sein soll:</p> 
       <ul> 
        <li><strong>Anhängen an benutzerdefinierte Daten</strong>: Möglichkeit, das benutzerdefinierte Formular an Projekte, Aufgaben und Probleme anzuhängen, auf die sie Zugriff haben Verwalten</li> 
        <li> <p><strong>Freigeben</strong>: Möglichkeit, das benutzerdefinierte Formular für andere Benutzer im System freizugeben</p> <p>Benutzer mit einer Arbeits-, Überprüfungs- oder Anforderungslizenz können ein benutzerdefiniertes Formular nur über die API oder einen Bericht für benutzerdefinierte Formulare freigeben. Weitere Informationen finden Sie unter .</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Verwalten</td> 
      <td> <p>Nur für Benutzer mit einer Planungslizenz verfügbar. </p> <p>Benutzer können das Formular nicht nur zu Objekten hinzufügen, auf die sie Zugriff haben, sondern auch das benutzerdefinierte Formular vollständig bearbeiten. Dazu gehören das Hinzufügen, Bearbeiten und Löschen von Feldern.</p> <p>Klicks <strong>Erweiterte Einstellungen</strong> um anzugeben, ob Folgendes zulässig sein soll:</p> 
       <ul> 
        <li> <p><strong>Anhängen an benutzerdefinierte Daten</strong>: Möglichkeit, das benutzerdefinierte Formular an Projekte, Aufgaben und Probleme anzuhängen, auf die sie Zugriff haben Verwalten</p> </li> 
        <li><strong>Löschen</strong>: Löschen Sie das benutzerdefinierte Formular aus dem System.</li> 
        <li><strong>Freigeben</strong>: Geben Sie das benutzerdefinierte Formular für andere Benutzer im System frei.</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Optional) Wiederholen Sie die Schritte 4 bis 5, um weitere Namen zur Liste hinzuzufügen und deren Optionen zu konfigurieren.
1. (Optional) Wenn Sie den Zugriff auf das benutzerdefinierte Formular (auf Objekte, an die es angehängt ist) auf die in den vorherigen Schritten angegebenen Elemente beschränken möchten, klicken Sie auf das Zahnradsymbol ![](assets/gear-icon-settings-with-dn-arrow.jpg) Klicken Sie in der oberen rechten Ecke des Freigabefelds auf **Systemweiten Zugriff entfernen**.

   Wenn Sie Ihre Meinung ändern, können Sie auf **Diese Funktion systemweit sichtbar machen** (Standardoption).

   >[!NOTE]
   >
   >* Wenn Sie ein benutzerdefiniertes Formular systemweit sichtbar machen, können Benutzer es nur auf Objekten sehen und ausfüllen, denen sie zugewiesen sind, und nicht an andere Objekte anhängen. Sie können das benutzerdefinierte Formular mithilfe der Option &quot;An benutzerdefinierte Daten anhängen&quot;anhängen, wie in Schritt 5 erläutert.
   >* Die meisten Unternehmen möchten sicherstellen, dass alle Benutzer im System ein benutzerdefiniertes Formular ausfüllen können, wenn es an Objekte angehängt ist, an denen sie arbeiten, und seine Daten in Berichten anzeigen. Wenn dies für Ihre Organisation zutrifft, empfehlen wir die Verwendung von &quot;**Diese Funktion systemweit sichtbar machen**.&quot; Wenn die Option auf diese Weise konfiguriert ist, wird im Dialogfeld &quot;Sichtbar systemweit&quot;angezeigt:
   >   
   >![](assets/visible-system-wide-350x480.png)
   >   
   >Wenn Sie sich Sorgen um ein benutzerdefiniertes Formular machen, in das Benutzer beim Anhängen vertrauliche Daten eingeben können, beschränken Sie die Freigabe für diese *Objekte* kann besser sein, als den Zugriff auf das Formular selbst zu beschränken.

1. Klicken Sie auf **Speichern**.

## Zugriff auf ein benutzerdefiniertes Formular entfernen

{{step-1-to-setup}}

1. Klicken Sie im linken Bereich auf **Benutzerdefinierte Forms**.
1. Wählen Sie das benutzerdefinierte Formular aus und klicken Sie auf **Freigeben** <span class="preview">oder ![Freigabesymbol](assets/share-icon.png).</span>
1. Klicken Sie in dem angezeigten Feld auf das X rechts neben dem Namen des Benutzers, Teams, der Rolle, der Gruppe oder des Unternehmens, auf das Sie keinen speziellen Zugriff mehr auf das Formular haben möchten.
1. (Optional) Wiederholen Sie den vorherigen Schritt nach für weitere Namen, die Sie entfernen möchten.
1. Klicken Sie auf **Speichern**.
