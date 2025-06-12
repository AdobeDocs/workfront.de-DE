---
product-area: projects;templates
navigation-topic: manage-projects
title: Speichern eines Projekts als Vorlage
description: Speichern eines Projekts als Vorlage „Als Vorlage speichern“ auf Projektebene, damit die Benutzer dies in der Benutzeroberfläche sehen. Es gibt einen anderen Artikel, auf den dieser Link verweist, der ausführlicher ist (Schritt-für-Schritt). Diese Funktion muss in beiden Bereichen von Projekten UND Vorlagen beibehalten werden.)“
author: Alina
feature: Work Management
exl-id: 4b5dfe12-f984-47c6-8e19-78b549f19159
source-git-commit: 939f3d9a4fac609c014acfc3be3d1485f469e947
workflow-type: tm+mt
source-wordcount: '787'
ht-degree: 1%

---

# Speichern eines Projekts als Vorlage

<!--Audited: 6/2025-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Keep this the way it is in the Managing Projects area because the functionality in the UI is "Save as template" at the project level, so users see that in the UI; there is another article that this links to which is more in depth (step-by-step). This functionality needs to stay in both projects AND templates areas.)</p>
-->

<div class="preview">

Die hervorgehobenen Informationen auf dieser Seite beziehen sich auf Funktionen, die noch nicht allgemein verfügbar sind. Sie ist nur in der Vorschau -Umgebung für alle Kunden verfügbar. Dieselben Funktionen werden nach einer Woche ab der Vorschau-Version auch in der Produktionsumgebung für alle Kunden verfügbar sein.

Weitere Informationen finden Sie unter [Schnittstellenmodernisierung](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md).

</div>

Wenn Sie festlegen, dass ein Projekt zu einem späteren Zeitpunkt wieder ausgeführt werden soll, können Sie aus diesem vorhandenen Projekt eine Vorlage erstellen. Anschließend können Sie die Vorlage erneut verwenden, um zukünftige Projekte zu erstellen, die ähnliche Informationen enthalten oder möglicherweise dieselbe Zeitleiste oder dieselben Zuweisungen für das vorhandene Projekt verwenden.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan</td> 
   <td> <p>Beliebig </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Neu: Standard </p>
   Oder 
   <p>Aktuell: Plan </p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriff auf Vorlagen bearbeiten</p> /td&gt; 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Anzeigen oder Erweitern von Berechtigungen für ein Projekt </p> <p>Sie erhalten Verwaltungsberechtigungen für die Vorlage, nachdem Sie das Projekt als Vorlage gespeichert haben</p> </td> 
  </tr> 
 </tbody> 
</table>

*Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Speichern eines Projekts als Vorlage

Das Speichern eines Projekts als Vorlage unterscheidet sich in der Produktions- und in der Vorschau-Umgebung.

### Speichern eines Projekts als Vorlage in der Produktionsumgebung

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

   ![](assets/save-as-template-first-step-350x159.png)

1. Klicken Sie auf **Nächster Schritt.**
1. Aktivieren **im Abschnitt** das Kontrollkästchen neben den Informationen, die Sie aus der Vorlage entfernen möchten.

   ![](assets/save-as-template-options-step-350x109.png)

1. Klicken Sie auf **Nächster Schritt.**
1. Wählen Sie im **Ausschließen** alle Aufgaben aus, die Sie aus dem Projekt ausschließen möchten.

   ![](assets/save-as-template-exclude-350x205.png)

1. Klicken Sie auf **Beenden und Vorlage speichern.**

   Ihre Vorlage wird jetzt in der Liste der verfügbaren Vorlagen angezeigt und kann entweder an ein vorhandenes Projekt angehängt oder zum Erstellen eines neuen verwendet werden.


<div class="preview">

### Speichern eines Projekts als Vorlage in der Vorschau-Umgebung

1. Wechseln Sie zu dem Projekt, das Sie als Vorlage speichern möchten.
1. Klicken Sie auf das **Mehr**-Menü ![Mehr-Symbol](assets/qs-more-icon-on-an-object.png) und dann **Als Vorlage speichern**.
1. Geben **im Abschnitt „Als Vorlage**&quot; die folgenden Informationen für die Vorlage an:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Vorlagenname</td> 
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

1. Klicken Sie **linken Bereich auf** Benutzerdefinierte Forms&quot;, um die Formulare zu entfernen oder neu anzuordnen.

   Um die Formulare neu anzuordnen, ziehen Sie sie per Drag-and-Drop in die richtige Reihenfolge.
Um ein Formular zu entfernen, wählen Sie es aus und klicken Sie auf **Entfernen**. Klicken Sie **Abbrechen**, um die ausgewählten Formulare zu entfernen.

   ![Benutzerdefinierte Formulare im Feld Als Vorlage speichern](assets/custom-forms-ara-in-save-as-template-box.png)

1. Aktualisieren Sie bei Bedarf die Informationen in den angehängten benutzerdefinierten Formularen. Die Informationen werden auf die Vorlage übertragen.

1. Klicken Sie **Abschnitt** Optionen“ im linken Bereich und aktivieren Sie dann das Kontrollkästchen neben den Informationen, die Sie auf die Vorlage übertragen möchten. Nicht ausgewählte Elemente werden nicht in die Vorlage übertragen. Standardmäßig sind alle Optionen deaktiviert.

   ![Optionen im Feld Als Vorlage speichern](assets/options-area-in-save-as-template-box.png)

1. Klicken Sie **linken** auf „Ausschließen“ und wählen Sie dann alle Aufgaben aus, die Sie aus dem Projekt ausschließen möchten. Standardmäßig sind alle Aufgaben deaktiviert.

   ![Bereich im Feld Als Vorlage speichern ausschließen](assets/exclude-area-save-as-template-box.png)

1. Klicken Sie auf **Beenden und Vorlage speichern.**

   Ihre Vorlage wird jetzt in der Liste der verfügbaren Vorlagen angezeigt und kann entweder an ein vorhandenes Projekt angehängt oder zum Erstellen eines neuen verwendet werden.

</span>