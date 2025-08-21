---
product-area: projects
navigation-topic: use-the-home-area
title: Verwenden des Widgets Meine Anfragen
description: Sie können Anfragen im Widget Meine Anfragen senden. Sie können das Widget auch mit Filtern und Spalten anpassen.
author: Becky
feature: Get Started with Workfront
source-git-commit: 68379a6c41db1b694e2968d93de259cb7b0d8bc4
workflow-type: tm+mt
source-wordcount: '793'
ht-degree: 3%

---


# Verwenden des Widgets Meine Anfragen

<span class="preview">Die Informationen auf dieser Seite beziehen sich auf Funktionen, die noch nicht allgemein verfügbar sind. Sie ist nur in der Vorschau -Umgebung für alle Kunden verfügbar. Nach den monatlichen Releases in der Produktion stehen dieselben Funktionen auch in der Produktionsumgebung für Kunden zur Verfügung, die schnelle Releases aktiviert haben. </span>

<span class="preview">Informationen zu Schnellversionen finden Sie unter [Aktivieren oder Deaktivieren von Schnellversionen für Ihre Organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).

Das Widget Meine Anfragen zeigt Anfragen an, die an Ihre Organisation gesendet wurden. Sie können die Anfragen filtern, nach bestimmten Anfragen suchen oder die Spaltenreihenfolge und Sichtbarkeit anpassen. Sie können auch über das Widget Meine Anfragen eine neue Anfrage erstellen.

>[!NOTE]
>
>Wenn das Widget Meine Anfragen geladen wird, werden bis zu 50 Anfragen angezeigt. Um weitere Anfragen anzuzeigen, scrollen Sie in der Liste nach unten.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Product]</strong></td> 
   <td> <ul><li>Adobe Workfront</li><li>Sie müssen über Adobe Workfront Planning verfügen, um Planungsanfragen oder Anfrageformulare anzuzeigen</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront plan]</strong></td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] Lizenz*</strong></td> 
   <td> <p>Neu: Mitwirkender oder höher</p>
   Oder   
   <p>Aktuell: [!UICONTROL-Anfrage] oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Konfiguration der Zugriffsebene</strong></td> 
   <td> <p>Anzeigen des Zugriffs auf oder höher für alle Objekte, für die Sie in einer Konversation getaggt sind oder eine Genehmigung auflösen müssen (Projekte, Aufgaben, Probleme, Dokumente)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Objektberechtigungen</strong></td> 
   <td> <p>[!UICONTROL Anzeigen] Berechtigungen oder höher für Projekte, Aufgaben, Probleme, Dokumente, bei denen Sie in einer Konversation getaggt sind oder eine Genehmigung auflösen müssen</p> </td> 
  </tr> 
 </tbody> 
</table>

*Wenden Sie sich an Ihren [!DNL Workfront], um herauszufinden, über welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie verfügen. Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Erstellen einer Anfrage

Sie können eine Anfrage direkt über das Widget Meine Anfragen erstellen.

Anweisungen finden Sie [Erstellen einer Anfrage](/help/quicksilver/workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md#create-a-request) im Artikel Erstellen von Arbeitselementen und Projekten im Bereich „Startseite“.

## Anfragen filtern

Das Widget Meine Anfragen verfügt über einen anpassbaren Filter, mit dem Sie steuern können, welche Anfragen im Widget angezeigt werden. Sie können diesen Filter für verschiedene Felder und Werte konfigurieren und Bedingungen mithilfe von UND und ODER stapeln.

So konfigurieren Sie den Filter im Widget Meine Anfragen :

1. Klicken Sie oben rechts auf **[!UICONTROL Hauptmenü]** ![Hauptmenüsymbol](assets/main-menu-icon.png) und dann auf **[!UICONTROL Startseite]**.
1. (Bedingt) So fügen Sie das Widget **Meine Anfragen** zu Ihrem Startbildschirm hinzu. Klicken Sie **Anpassen** und suchen Sie nach **Meine Anfragen**.
1. Klicken Sie im Widget Meine Anfragen auf **Filter**.
1. Wählen Sie im Feld ganz links aus, nach was Sie filtern möchten. Verfügbare Optionen sind:

   * Arbeitsbereich
   * Objekttyp
   * Eingabedatum
   * Anfrageformular
   * Status
   * Eingegeben von

1. Wählen Sie im nächsten Feld den Operator aus, den Sie für diese Filterbedingung verwenden möchten. Die verfügbaren Operatoren hängen vom gewählten Feld ab.
1. (Bedingt) Wenn rechts neben dem Operator ein Feld angezeigt wird, wählen Sie den Wert aus, nach dem Sie filtern möchten.
1. (Optional) Um eine weitere Filterbedingung hinzuzufügen, klicken Sie auf **Bedingung hinzufügen** und wiederholen Sie die Schritte 4 bis 6.
1. (Optional und bedingt) Wenn mehrere Bedingungen vorliegen, schalten Sie den Und- oder Oder-Wert um, indem Sie **Und** oder **Oder** links von der Bedingung klicken.

Der Filter wird automatisch gespeichert.

>[!TIP]
>
>Wenn Ihr Unternehmen Workfront Planning erworben hat, enthält das Widget Meine Anfragen sowohl Workfront- als auch Workfront-Planungsanfragen.
> 
>* Um nur nach Workfront-Anfragen zu filtern, setzen Sie den Filter auf **Objekttyp** > **Hat beliebige von** > **Probleme**.
>* Um nur nach Workfront Planning-Anfragen zu filtern, setzen Sie den Filter auf **Objekttyp** > **Hat keine von** > **Probleme**.

## Spalten anpassen

Sie können auswählen, welche der verfügbaren Spalten im Widget Meine Anfragen angezeigt werden, und ihre Reihenfolge festlegen.

Zu den verfügbaren Spalten gehören:

* Betreff
* Objekt erstellt
* Objekttyp
* Status
* Anfrageformular
* Eingabedatum
* Eingegeben von

So passen Sie die Spalten im Widget Meine Anfragen an:

1. Klicken Sie oben rechts auf **[!UICONTROL Hauptmenü]** ![Hauptmenüsymbol](assets/main-menu-icon.png) und dann auf **[!UICONTROL Startseite]**.
1. (Bedingt) So fügen Sie das Widget **Meine Anfragen** zu Ihrem Startbildschirm hinzu. Klicken Sie **Anpassen** und suchen Sie nach **Meine Anfragen**.
1. Klicken Sie im Widget Meine Anfragen auf **Spalten**.
1. (Optional) Um die Spalten neu anzuordnen, klicken Sie auf den Ziehgriff ![Ziehgriff](assets/drag-handle.png) der Spalte, die Sie verschieben möchten, und ziehen Sie sie an die gewünschten Positionen. Die Spalte oben in der Liste wird im Widget Meine Anfragen als Spalte ganz links angezeigt.
1. (Optional) Verwenden Sie den Umschalter, um zu steuern, ob eine Spalte im Widget „Meine Anfragen“ angezeigt wird.

Spalteneinstellungen werden automatisch gespeichert.

## Suchanfragen

So suchen Sie im Widget „Meine Anfragen“ nach bestimmten Anfragen:

1. Klicken Sie oben rechts auf **[!UICONTROL Hauptmenü]** ![Hauptmenüsymbol](assets/main-menu-icon.png) und dann auf **[!UICONTROL Startseite]**.
1. (Bedingt) So fügen Sie das Widget **Meine Anfragen** zu Ihrem Startbildschirm hinzu. Klicken Sie **Anpassen** und suchen Sie nach **Meine Anfragen**.
1. Geben Sie in der Suchleiste rechts oben im Widget Meine Anfragen den Begriff ein, nach dem Sie suchen möchten.

   Anfragen, die den Begriff enthalten, sind orange hervorgehoben.

1. (Optional) Um zu den hervorgehobenen Anfragen zu springen, klicken Sie in der Suchleiste auf die Pfeile nach oben oder unten.





