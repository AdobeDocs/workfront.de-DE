---
title: Anforderungsformular in der Adobe Workfront-Planung erstellen
description: Nachdem Sie im Adobe Workfront-Planungsbereich einen Datensatztyp ausgewählt haben, können Sie ein Anforderungsformular erstellen, das diesem Datensatztyp zugeordnet ist, und einen Link mit anderen internen oder externen Benutzern teilen.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: 1ad86cd55459d92650ac7a24c41765e579f8bb94
workflow-type: tm+mt
source-wordcount: '646'
ht-degree: 2%

---

# Anforderungsformular in der Adobe Workfront-Planung erstellen

<!--update the metadata with real information when making this available in TOC and in the left nav-->

{{planning-important-intro}}

Nachdem Sie im Adobe Workfront-Planungsbereich einen Datensatztyp ausgewählt haben, können Sie ein Anforderungsformular erstellen und dieses mit diesem Datensatztyp verknüpfen. Sie können dann einen Link mit anderen internen oder externen Benutzern teilen. <!--double-check on the external part of it-->

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

Für den Zugriff auf die Workfront-Planung benötigen Sie Folgendes:

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Produkte</p> </td>
   <td>
   <ul><li><p> Adobe Workfront</p></li>
   <li><p> Adobe Workfront-Planung<p></li></ul></td>
  </tr>  
 <tr>
   <td role="rowheader"><p>Adobe Workfront-Plan*</p></td>
   <td>
<p>Die folgenden Workfront-Pläne:</p>
<ul><li>Auswählen</li>
<li>Erstklassig</li>
<li>Ultimativ</li></ul>
<p>Die Workfront-Planung ist für veraltete Workfront-Pläne nicht verfügbar</p>
   </td>

<tr>
   <td role="rowheader"><p>Adobe Workfront-Planungsplan*</p></td>
   <td>
<p>Alle </p>   </td>

<tr>
   <td role="rowheader"><p>Adobe Workfront-Plattform</p></td>
   <td>
<p>Die Workfront-Instanz Ihres Unternehmens muss in das Adobe Unified Experience integriert sein, damit Sie auf alle Funktionen der Workfront-Planung zugreifen können.</p>
<p>Weitere Informationen finden Sie unter <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p>
   </td>

</tr>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront-Lizenz*</p></td>
   <td>
   <p>Standard</p>
   <p>Für ältere Workfront-Lizenzen ist die Workfront-Planung nicht verfügbar.</p>
  </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Konfiguration der Zugriffsebene</p></td>
   <td> <p>Für die Adobe Workfront-Planung gibt es keine Zugriffssteuerungselemente</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Objektberechtigungen</p></td>
   <td>
   <ul>
   <li><p>Berechtigungen für einen Arbeitsbereich verwalten</p></li>
    <li><p>Systemadministratoren können nicht erstellte Arbeitsbereiche verwalten. </p></li>
    </ul>
   <p>Informationen zum Freigeben von Berechtigungen für Workfront Planning-Objekte finden Sie unter  
   <a href="/help/quicksilver/planning/access/sharing-permissions-overview.md">Überblick über die Freigabe von Berechtigungen in der Adobe Workfront-Planung</a> 
  </td>
  </tr>
<tr>
   <td role="rowheader"><p>Layout-Vorlage</p></td>
   <td> <p>Allen Benutzern, einschließlich Workfront-Administratoren, muss eine Layoutvorlage zugewiesen werden, die den Planungsbereich im Hauptmenü enthält. </p>  
</td>
  </tr>
 </tbody>
</table>

*Weitere Informationen zu den Zugriffsanforderungen für Workfront finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Anforderungsformular für einen Datensatztyp erstellen

{{step1-to-planning}}

1. Klicken Sie auf den Arbeitsbereich, in den Sie Datensätze hinzufügen möchten.

   Der Arbeitsbereich wird geöffnet und die Datensatztypen werden als Karten angezeigt.

1. Klicken Sie auf eine Karte vom Typ Datensatz. Informationen zum Erstellen eines Datensatztyps finden Sie unter [Erstellen von Datensatztypen](/help/quicksilver/planning/architecture/create-record-types.md).

   Die Seite mit dem Datensatztyp wird in der Ansicht geöffnet, auf die Sie zuletzt zugegriffen haben. Standardmäßig wird eine Seite vom Typ Datensatz in der Tabellenansicht geöffnet.

1. Klicken Sie auf das Menü **Mehr** rechts neben dem Namen des Datensatztyps in der Kopfzeile der Seite und klicken Sie dann auf **Anforderungsformular erstellen**.![](assets/more-menu.png)
1. Aktualisieren Sie den Namen des Anfrageformulars. Standardmäßig lautet der Name des Formulars **Unbenanntes Anforderungsformular**. <!--check this; you logged a bug to rename it to this but was it fixed?-->
1. (Optional) Fügen Sie eine **Beschreibung** für das Anfrageformular hinzu.

   <!--Not possible yet: The Description is visible when you access the request form from the Requests area of Workfront.-->

1. Klicken Sie auf **Erstellen**. Das Anfrageformular für den ausgewählten Datensatztyp wird geöffnet.

   Das Anfrageformular enthält standardmäßig die folgenden Informationen:

   * **Standardabschnitt**: Dies ist der standardmäßige Abschnittsumbruch, den Workfront auf das Anforderungsformular anwendet. Der Abschnitt Standard kann nicht umbenannt oder entfernt werden.
   * Feld **Betreff** : Das Feld, das die Anforderung in Workfront identifiziert. Diese Funktion ist noch nicht verfügbar.
   * Alle mit dem Datensatztyp verknüpften Felder.

   Die im Anfrageformular enthaltenen Felder sind für alle sichtbar, die eine Anfrage an diesen Datensatztyp senden.

1. (Optional) Entfernen Sie das Feld **Betreff** , da es in der Workfront-Planung nicht sichtbar ist. <!--remove this step when we connect intake with the Requests area in Workfront-->
1. Bewegen Sie den Mauszeiger über alle Felder im Formular, die Sie entfernen möchten. Sie werden der Registerkarte **Felder** auf der linken Seite des Formulars hinzugefügt.
1. Klicken Sie auf ein beliebiges Feld und verwenden Sie dann die Steuerelemente auf der rechten Seite des Formulars, um eine der folgenden Informationen über die Felder zu definieren:

   * **Beschriftung**: Dies ist der Name des Felds, wie er im Anfrageformular angezeigt wird. Dadurch wird der Name des Datensatzfelds nicht geändert.
   * **Anweisungen**: Fügen Sie weitere Informationen zum Feld hinzu.
   * **Machen Sie ein erforderliches Feld**: Wenn ausgewählt, muss das Feld einen Wert enthalten. Andernfalls kann das Formular nicht gesendet werden.
   * **Logik hinzufügen**: Definieren Sie, welche Bedingungen erfüllt sein müssen, damit das Feld angezeigt oder ausgeblendet wird.

1. Klicken Sie auf die Registerkarte Inhaltselemente rechts im Formular und fügen Sie eines der folgenden Elemente hinzu:

   * Beschreibender Text
   * Abschnittsumbruch

   Weitere Informationen zum Erstellen eines benutzerdefinierten Formulars finden Sie unter [Entwerfen eines Formulars mit dem Formularentwickler](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).





