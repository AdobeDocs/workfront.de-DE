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
source-git-commit: 6c43d836c24f893d1b7d7d01c1dd0b1cc3fba357
workflow-type: tm+mt
source-wordcount: '1408'
ht-degree: 1%

---

# Freigeben eines benutzerdefinierten Formulars

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

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Zugriff auf benutzerdefinierte Formulare {#access-to-custom-forms}

Wenn Sie ein neues benutzerdefiniertes Formular erstellen und es von einer Person an ein Objekt angehängt wird, kann jeder Benutzer, der dem Objekt zugewiesen ist, das Formular standardmäßig anzeigen und ausfüllen. Dazu gehören Benutzer mit Lizenzen anfordern und externe Benutzer.

Bei einem Objekt, an das das benutzerdefinierte Formular noch nicht angehängt ist, kann ein Benutzer (auch wenn er über eine Planner-Zugriffsstufe verfügt) es nicht über das Dropdown-Menü &quot;Benutzerdefinierte Forms&quot;anhängen, es sei denn, eine der folgenden Eigenschaften ist wahr:

* Jemand hat das benutzerdefinierte Formular für den Benutzer oder für das Team, die Rolle, die Gruppe oder das Unternehmen freigegeben und mindestens die Berechtigung zum Anzeigen mit der ausgewählten Option &quot;An benutzerdefinierte Daten anhängen&quot;gewährt.
* Der Benutzer verfügt über eine Planungslizenz und seine Zugriffsstufe ermöglicht den Administratorzugriff auf benutzerdefinierte Formulare

## Freigeben eines benutzerdefinierten Formulars in der Liste der Formulare

Anstatt ein benutzerdefiniertes Formular im standardmäßigen Freigabestatus zu belassen (wie in diesem Artikel unter [Zugriff auf benutzerdefinierte Formulare](#access-to-custom-forms) beschrieben), können Sie bestimmte Zugriffsebenen für bestimmte Benutzer, Jobrollen, Gruppen, Teams und Unternehmen auf das Formular konfigurieren.

{{step-1-to-setup}}

1. Klicken Sie im linken Bereich auf **Benutzerdefinierter Forms**.
1. Wählen Sie das benutzerdefinierte Formular aus und klicken Sie dann auf das Symbol ![Freigeben](assets/share-icon.png).
1. Geben Sie in das Feld, das angezeigt wird, unter **Erteilen Sie benutzerdefinierten Formularzugriff auf** den Namen des Benutzers, Teams, der Rolle, der Gruppe oder des Unternehmens ein, für den/das Sie das benutzerdefinierte Formular freigeben möchten, und drücken Sie dann bei der Anzeige des Namens die Eingabetaste **3}.**
1. Um den Zugriff auf den soeben hinzugefügten Benutzer, das Team, die Rolle, die Gruppe oder das Unternehmen anzupassen, klicken Sie auf das Dropdown-Menü rechts neben dem Namen und konfigurieren Sie dann eine der folgenden verfügbaren Optionen und eine der erweiterten Einstellungen:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Anzeigen</td> 
      <td> <p>Möglichkeit, das benutzerdefinierte Formular für Objekte anzuzeigen und auszufüllen.</p> <p><b>HINWEIS</b>: Für Benutzer mit Light- und Contributor-Lizenzen (oder Arbeits-, Review- und Anforderungslizenzen) ist dies die höchste verfügbare Option.</p> <p>Klicken Sie auf <strong>Erweiterte Einstellungen</strong> , um festzulegen, ob Folgendes zulässig sein soll:</p> 
       <ul> 
        <li><strong>Anhängen an benutzerdefinierte Daten</strong>: Möglichkeit, das benutzerdefinierte Formular an Projekte, Aufgaben und Probleme anzuhängen, auf die sie Zugriff haben Verwalten</li> 
        <li> <p><strong>Freigeben</strong>: Möglichkeit, das benutzerdefinierte Formular für andere Benutzer im System freizugeben</p> <p>Benutzer mit einer Light- oder Contributor-Lizenz (oder Arbeits-, Review- oder Anforderungslizenz) können ein benutzerdefiniertes Formular nur über die API oder einen benutzerdefinierten Formularbericht freigeben.</p> </li>
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Verwalten</td> 
      <td> <p>Nur für Benutzer mit einer Standard- oder Plan-Lizenz verfügbar. </p> <p>Benutzer können das Formular nicht nur zu Objekten hinzufügen, auf die sie Zugriff haben, sondern auch das benutzerdefinierte Formular vollständig bearbeiten. Dazu gehören das Hinzufügen, Bearbeiten und Löschen von Feldern.</p> <p>Klicken Sie auf <strong>Erweiterte Einstellungen</strong> , um festzulegen, ob Folgendes zulässig sein soll:</p> 
       <ul> 
        <li> <p><strong>Anhängen an benutzerdefinierte Daten</strong>: Möglichkeit, das benutzerdefinierte Formular an Projekte, Aufgaben und Probleme anzuhängen, auf die sie Zugriff haben Verwalten</p> </li> 
        <li><strong>Löschen</strong>: Löschen Sie das benutzerdefinierte Formular aus dem System.</li> 
        <li><strong>Freigeben</strong>: Geben Sie das benutzerdefinierte Formular für andere Benutzer im System frei.</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Optional) Wiederholen Sie die Schritte 4 bis 5, um weitere Namen zur Liste hinzuzufügen und deren Optionen zu konfigurieren.
1. (Optional) Wenn Sie den Zugriff auf das benutzerdefinierte Formular (auf Objekte, an die es angehängt ist) auf die in den vorherigen Schritten angegebenen Elemente beschränken möchten, klicken Sie auf das Zahnradsymbol ![](assets/gear-icon-settings-with-dn-arrow.jpg) in der oberen rechten Ecke des Freigabefelds und klicken Sie dann auf **Systemweiten Zugriff entfernen**.

   Wenn Sie Ihre Meinung ändern, können Sie auf **Diese Option systemweit anzeigen** (Standardoption).

   >[!NOTE]
   >
   >* Wenn Sie ein benutzerdefiniertes Formular systemweit sichtbar machen, können Benutzer es nur auf Objekten sehen und ausfüllen, denen sie zugewiesen sind, und nicht an andere Objekte anhängen. Sie können das benutzerdefinierte Formular mithilfe der Option &quot;An benutzerdefinierte Daten anhängen&quot;anhängen, wie in Schritt 5 erläutert.
   >* Die meisten Unternehmen möchten sicherstellen, dass alle Benutzer im System ein benutzerdefiniertes Formular ausfüllen können, wenn es an Objekte angehängt ist, an denen sie arbeiten, und seine Daten in Berichten anzeigen. Wenn dies für Ihre Organisation zutrifft, empfehlen wir, **Dieses Skript systemweit sichtbar zu machen**. Wenn die Option auf diese Weise konfiguriert ist, wird im Dialogfeld &quot;Sichtbar systemweit&quot;angezeigt:
   >   
   >![](assets/visible-system-wide-350x480.png)
   >   
   >Wenn Sie sich wegen eines benutzerdefinierten Formulars Sorgen machen, bei dem Benutzer möglicherweise sensible Daten eingeben, wenn sie an bestimmte Objekte angehängt sind, ist es möglicherweise besser, die Freigabe für diese *Objekte* zu beschränken, anstatt den Zugriff auf das Formular selbst zu beschränken.

1. Klicken Sie auf **Speichern**.

## Freigeben eines benutzerdefinierten Formulars aus dem Formularentwickler

{{step-1-to-setup}}

1. Klicken Sie im linken Bereich auf **Benutzerdefinierter Forms**.
1. Öffnen Sie ein benutzerdefiniertes Formular oder erstellen Sie ein neues benutzerdefiniertes Formular.
1. Klicken Sie oben rechts im Formularentwickler auf **Freigeben** , wenn Sie bereit sind, das Formular freizugeben.
1. Geben Sie in das Feld, das angezeigt wird, unter **Gewähren des benutzerdefinierten Formulars Zugriff auf**, den Namen des Benutzers, Teams, der Rolle, der Gruppe oder des Unternehmens ein, für den bzw. das Sie das benutzerdefinierte Formular freigeben möchten, und drücken Sie dann bei der Anzeige des Namens die Eingabetaste.****
1. Um den Zugriff auf den soeben hinzugefügten Benutzer, das Team, die Rolle, die Gruppe oder das Unternehmen anzupassen, klicken Sie auf das Dropdown-Menü rechts neben dem Namen und konfigurieren Sie dann eine der folgenden verfügbaren Optionen und eine der erweiterten Einstellungen:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Anzeigen</td> 
      <td> <p>Möglichkeit, das benutzerdefinierte Formular für Objekte anzuzeigen und auszufüllen.</p> <p><b>HINWEIS</b>: Für Benutzer mit Light- und Contributor-Lizenzen (oder Arbeits-, Review- und Anforderungslizenzen) ist dies die höchste verfügbare Option.</p> <p>Klicken Sie auf <strong>Erweiterte Einstellungen</strong> , um festzulegen, ob Folgendes zulässig sein soll:</p> 
       <ul> 
        <li><strong>Anhängen an benutzerdefinierte Daten</strong>: Möglichkeit, das benutzerdefinierte Formular an Projekte, Aufgaben und Probleme anzuhängen, auf die sie Zugriff haben Verwalten</li> 
        <li> <p><strong>Freigeben</strong>: Möglichkeit, das benutzerdefinierte Formular für andere Benutzer im System freizugeben</p> <p>Benutzer mit einer Light- oder Contributor-Lizenz (oder Arbeits-, Review- oder Anforderungslizenz) können ein benutzerdefiniertes Formular nur über die API oder einen benutzerdefinierten Formularbericht freigeben.</p> </li>
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Verwalten</td> 
      <td> <p>Nur für Benutzer mit einer Standard- oder Plan-Lizenz verfügbar. </p> <p>Benutzer können das Formular nicht nur zu Objekten hinzufügen, auf die sie Zugriff haben, sondern auch das benutzerdefinierte Formular vollständig bearbeiten. Dazu gehören das Hinzufügen, Bearbeiten und Löschen von Feldern.</p> <p>Klicken Sie auf <strong>Erweiterte Einstellungen</strong> , um festzulegen, ob Folgendes zulässig sein soll:</p> 
       <ul> 
        <li> <p><strong>Anhängen an benutzerdefinierte Daten</strong>: Möglichkeit, das benutzerdefinierte Formular an Projekte, Aufgaben und Probleme anzuhängen, auf die sie Zugriff haben Verwalten</p> </li> 
        <li><strong>Löschen</strong>: Löschen Sie das benutzerdefinierte Formular aus dem System.</li> 
        <li><strong>Freigeben</strong>: Geben Sie das benutzerdefinierte Formular für andere Benutzer im System frei.</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Optional) Wiederholen Sie die Schritte 5 bis 6, um weitere Namen zur Liste hinzuzufügen und deren Optionen zu konfigurieren.
1. (Optional) Wenn Sie den Zugriff auf das benutzerdefinierte Formular (auf Objekte, an die es angehängt ist) auf die in den vorherigen Schritten angegebenen begrenzen möchten, klicken Sie auf den Dropdown-Pfeil unter &quot;**Wer Zugriff hat&quot;** und wählen Sie dann &quot;**Nur eingeladene Personen können auf &quot;**&quot;zugreifen.

   Wenn Sie Ihre Meinung ändern, können Sie **Alle im System können** anzeigen.

   >[!NOTE]
   >
   >* Wenn Sie ein benutzerdefiniertes Formular systemweit sichtbar machen, können Benutzer es nur auf Objekten sehen und ausfüllen, denen sie zugewiesen sind, und nicht an andere Objekte anhängen. Sie können das benutzerdefinierte Formular mithilfe der Option &quot;An benutzerdefinierte Daten anhängen&quot;anhängen, wie in Schritt 6 erläutert.
   >* Die meisten Unternehmen möchten sicherstellen, dass alle Benutzer im System ein benutzerdefiniertes Formular ausfüllen können, wenn es an Objekte angehängt ist, an denen sie arbeiten, und seine Daten in Berichten anzeigen. Wenn dies für Ihre Organisation zutrifft, empfehlen wir, **Alle Benutzer im System können** anzeigen. Wenn die Option auf diese Weise konfiguriert ist, wird im Dialogfeld &quot;Sichtbar systemweit&quot;angezeigt:
   >   
   >![ Benutzerdefiniertes Formular freigeben](assets/share-custom-form-in-designer.png)
   >   
   >Wenn Sie sich wegen eines benutzerdefinierten Formulars Sorgen machen, bei dem Benutzer möglicherweise sensible Daten eingeben, wenn sie an bestimmte Objekte angehängt sind, ist es möglicherweise besser, die Freigabe für diese *Objekte* zu beschränken, anstatt den Zugriff auf das Formular selbst zu beschränken.

1. Klicken Sie auf **Speichern**.

## Zugriff auf ein benutzerdefiniertes Formular aus der Liste der Formulare entfernen

{{step-1-to-setup}}

1. Klicken Sie im linken Bereich auf **Benutzerdefinierter Forms**.
1. Wählen Sie das benutzerdefinierte Formular aus und klicken Sie dann auf das Symbol ![Freigeben](assets/share-icon.png).
1. Klicken Sie in dem angezeigten Feld auf das X rechts neben dem Namen des Benutzers, Teams, der Rolle, der Gruppe oder des Unternehmens, auf das Sie keinen speziellen Zugriff mehr auf das Formular haben möchten.
1. (Optional) Wiederholen Sie den vorherigen Schritt nach für weitere Namen, die Sie entfernen möchten.
1. Klicken Sie auf **Speichern**.
