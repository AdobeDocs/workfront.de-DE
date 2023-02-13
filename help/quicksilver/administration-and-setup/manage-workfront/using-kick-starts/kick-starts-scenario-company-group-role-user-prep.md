---
user-type: administrator
product-area: system-administration;user-management
keywords: kickstart,kick-start,kickstarts,kick-starts
navigation-topic: use-kick-starts
title: '"Kick-Starts-Szenario: Vorbereitung der Firmen-, Gruppen-, Rollen- und Benutzerkick-Starts'
description: Wenn Sie mit der Implementierung von Adobe Workfront beginnen, können Sie anstelle der manuellen Eingabe von Daten Ihre Kundenliste, Ihre internen Abteilungen, Ihre Jobrollen und Benutzerinformationen importieren.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: b83e2e35-dd9d-4d98-b8d4-2f8718b3c6c1
source-git-commit: 5d36c2c959dbfd00920eaf0a16409102b99de042
workflow-type: tm+mt
source-wordcount: '1103'
ht-degree: 10%

---

# Szenario für Kick-Starts: Vorbereitung von Unternehmens-, Gruppen-, Rollen- und Benutzerkick-Starts

Wenn Sie mit der Implementierung von Adobe Workfront beginnen, können Sie anstelle der manuellen Eingabe von Daten Ihre Kundenliste, Ihre internen Abteilungen, Ihre Jobrollen und Benutzerinformationen importieren.

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Abo</td> 
   <td>Beliebig</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Sie müssen Workfront-Administrator sein.</p> <p><b>NOTE</b>: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Was Sie importieren können

In der folgenden Tabelle sind die zu importierenden Unternehmen, Gruppen und Rollen aufgeführt:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Firmen</strong> </th> 
   <th><strong>Gruppen</strong> </th> 
   <th><strong>Funktionen</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td valign="top"> <p>Acme, Co</p> <p>Workfront, Inc.</p> <p><em>Ihr Unternehmen</em> </p> <p>XYZ, Inc.</p> </td> 
   <td valign="top"> <p valign="top" rowspan="7">Finanzielle Details</p> <p valign="top" rowspan="7">IT </p> <p valign="top" rowspan="7">Marketing </p> <p valign="top" rowspan="7">Verkauf</p> </td> 
   <td valign="top"> <p valign="top">Geschäftsanalyst</p> <p valign="top">Controller Creative</p> <p valign="top">Designer</p> <p valign="top">Ressourcenmanager</p> <p valign="top">Scrum Übergeordnet</p> <p valign="top">Technischer Schriftsteller</p> <p valign="top">Webentwickler</p> </td> 
  </tr> 
 </tbody> 
</table>

Die Rollennamen müssen eindeutig sein, vorhandene Vorgangsrollen können nicht importiert werden.

In den folgenden Tabellen sind die zu importierenden Benutzer sowie verschiedene Benutzerattribute für jedes aufgeführt:

### Benutzer 1

| **Vorname** | Chris |
|---|---|
| **Nachname** | Besetzung |
| **Benutzername/E-Mail** | mailto:cmanning@foo.com |
| **Kennwort** | updateMe |
| **Zugriff** | Teammitglied |
| **Firma** | &lt;*Ihr Unternehmen>* |
| **Hauptgruppe** | Marketing |
| **Aufgabengebiet** | Geschäftsanalyst |

{style=&quot;table-layout:auto&quot;}

### Benutzer 2

| **Vorname** | Jennifer |
|---|---|
| **Nachname** | Campbell |
| **Benutzername/E-Mail** | jcampbell@foo.com |
| **Kennwort** | updateMe |
| **Zugriff** | Projektleiter |
| **Firma** | &lt;*Ihr Unternehmen>* |
| **Hauptgruppe** | Marketing |
| **Aufgabengebiet** | Projektleiter |

{style=&quot;table-layout:auto&quot;}

### Benutzer 3

| **Vorname** | Jill |
|---|---|
| **Nachname** | Sullivan |
| **Benutzername/E-Mail** | jsullivan@foo.com |
| **Kennwort** | updateMe |
| **Zugriff** | Helpdesk |
| **Firma** | &lt;*Ihr Unternehmen>* |
| **Hauptgruppe** | Verkauf |
| **Aufgabengebiet** | Vertriebsmitarbeiter |

{style=&quot;table-layout:auto&quot;}

### Benutzer 4

| **Vorname** | Marc |
|---|---|
| **Nachname** | Lewis |
| **Benutzername/E-Mail** | mlewis@foo.com |
| **Kennwort** | updateMe |
| **Zugriff** | Portfolio-Manager |
| **Firma** | &lt;*Ihr Unternehmen>* |
| **Hauptgruppe** | Finanzielle Details |
| **Aufgabengebiet** | Controller |

{style=&quot;table-layout:auto&quot;}

### Benutzer 5

| **Vorname** | Pam |
|---|---|
| **Nachname** | Reynolds |
| **Benutzername/E-Mail** | preynolds@foo.com |
| **Kennwort** | updateMe |
| **Zugriff** | Projektleiter |
| **Firma** | *Ihr Unternehmen>* |
| **Hauptgruppe** | Marketing |
| **Aufgabengebiet** | IT |

{style=&quot;table-layout:auto&quot;}

### Benutzer 6

| **Vorname** | Ray |
|---|---|
| **Nachname** | Andrews |
| **Benutzername/E-Mail** | randrews@foo.com |
| **Kennwort** | updateMe |
| **Zugriff** | Administrator |
| **Firma** | *Ihr Unternehmen>* |
| **Hauptgruppe** | Ressourcenmanager |
| **Aufgabengebiet** | Keine |

{style=&quot;table-layout:auto&quot;}

## Herunterladen einer Kick-Start-Vorlage

1. Klicken Sie auf **Hauptmenü** icon ![](assets/main-menu-icon.png) Klicken Sie oben rechts in Adobe Workfront auf **Einrichtung** ![](assets/gear-icon-settings.png).

1. Klicken **System** > **Kick-Starts** > **Daten importieren.**

1. Klicken **Weitere Optionen** um die vollständige Liste der Importoptionen anzuzeigen.
1. Wählen Sie die zu importierenden Objekte &quot;Zugriffsstufe&quot;, &quot;Unternehmen&quot;, &quot;Gruppe&quot;, &quot;Auftragsrolle&quot;und &quot;Benutzer&quot;aus.

## Firmeninformationen eingeben

1. Öffnen Sie die **Workfront.xlsx** Datei, die Sie gerade heruntergeladen haben.

   >[!TIP]
   >
   >Wenn Sie mit sehr großen Datenblättern arbeiten, sollten Sie das Freeze Pane-Tool (oder ein entsprechendes Tool) Ihres Tabelleneditors verwenden, um die Arbeit mit dieser Tabelle zu vereinfachen.

1. Gehen Sie in das Blatt &quot;CMPY Company&quot;.

   Es sollte leer sein, es sei denn, die Unternehmen sind bereits im System. ![](assets/cmpysheet-350x16.png)

   ![](assets/companyid--1--350x78.png)

1. Geben Sie TRUE in den **isNew** Spalte.
1. Wiederholen Sie diese Aktion für jedes hinzugefügte Unternehmen. (In diesem Beispiel führen Sie diese Aktion für die Zeilen 3-6 aus, da vier Unternehmen hinzugefügt werden.)

   ![](assets/cmpyisnew-350x86.png)

1. Geben Sie eine eindeutige ID an.

   Dies muss für jede Zeile der ID-Spalte erfolgen. Bei der Erstellung neuer Datensätze können Ganzzahlen ab 1 problemlos verwendet werden.

   ![](assets/cmpyisnew-350x86.png)

1. Legen Sie einen Namen fest.

   Geben Sie die Namen der einzelnen Kunden im **setName** Spalte.

   ![](assets/companyid-350x78.png)

1. Gehen Sie zum Gruppenblatt .

   Sofern Sie keine bereits in Workfront erstellten Gruppen erstellt haben, sollte dieses Blatt nur die Standardgruppe anzeigen, die mit jedem Konto von Workfront bereitgestellt wurde.

   ![](assets/groupsheet-350x15.png) ![](assets/emptygroupsheet-350x85.png)

1. Legen Sie die **isNew** column.Gemäß dem Szenario werden vier Gruppen importiert. Geben Sie daher TRUE in die Zeilen 4 bis 7 für die Spalte &quot;isNew&quot;ein.
1. Geben Sie eine eindeutige ID an.

   Dies muss für jede Zeile der ID-Spalte erfolgen. Bei der Erstellung neuer Datensätze können Ganzzahlen ab 1 problemlos verwendet werden.

   ![](assets/groupids-350x85.png)

1. Legen Sie einen Namen fest.

   Geben Sie die Namen der einzelnen Abteilungen im **setName** Spalte.

   ![](assets/groupnames-350x85.png)

   Geben Sie Rolleninformationen an. Gehen Sie zum ROLE Role-Blatt.

1. Sofern Sie keine Rollen in Ihrem Konto erstellt oder gelöscht haben, sollten in diesem Arbeitsblatt acht Rollen angezeigt werden, die für jedes Konto von Workfront bereitgestellt werden.

   ![](assets/groupnames-350x85.png)

1. True-Anweisung festlegen.

   Sieben Auftragsrollen importieren und geben TRUE in die Zeilen 12 bis 18 für die Spalte &quot;isNew&quot;ein.

   ![](assets/roleisnew-350x104.png)

1. Geben Sie eine eindeutige ID an.

   Dies muss für jede Zeile der ID-Spalte erfolgen. Bei der Erstellung neuer Datensätze können Ganzzahlen ab 1 problemlos verwendet werden.

   ![](assets/usersheet-350x16.png)

   ![](assets/roleisnew--1--350x104.png)

1. Geben Sie für jede Rolle einen Namen ein, indem Sie sie in die Spalte setName eingeben.

   ![](assets/roleisnew-350x104.png)

1. Geben Sie bei Bedarf weitere Details an.

   Schließen Sie bei Bedarf Abrechnungsraten, Kostensätze und Beschreibungen für die Rollen ein, die Sie erstellen.

1. Wechseln Sie zum Blatt &quot;USER User&quot;, um Benutzerinformationen einzugeben.

   Sofern Sie in Ihrem Konto noch keine Benutzer erstellt haben, sollte auf diesem Arbeitsblatt nur der Admin-Benutzer angezeigt werden, der für jedes Konto von Workfront bereitgestellt wurde.

   ![](assets/rolenames-350x104.png) ![](assets/emptyusersheet-350x52.png)

1. Legen Sie den Wert True fest, indem Sie für die Spalte &#39;isNew&#39; TRUE in die Zeilen 4 bis 9 eingeben, da 6 Benutzer importiert werden.

   ![](assets/userisnew-350x52.png)

1. Legen Sie eine eindeutige ID fest, indem Sie in jeder Zeile für die ID-Spalte eine eindeutige ID angeben. Normalerweise funktionieren Ganzzahlen ab 1 gut für neue Datensätze.

   ![](assets/userisnew-350x52.png)

1. Geben Sie die Namen der einzelnen Benutzer in die Spalten &quot;setFirstName&quot;und &quot;setLastName&quot;ein.

   ![](assets/usernames-350x52.png)

1. Legen Sie Detailwerte fest, indem Sie Werte in die Spalten &quot;setEmail&quot;, &quot;setPassword&quot;und &quot;setUsername&quot;eingeben.

   ![](assets/usercredentials-350x52.png)

1. Geben Sie Werte für die Zugriffsebene an.

   Beispiel: Chris Manning, ein Team-Mitglied, sucht die Kennung auf der ACSLVL-Zugriffsstufe nach der Zugriffsstufe für Team-Mitglieder. Kopieren Sie die ID in die Zwischenablage und fügen Sie sie im Benutzerblatt im **setAccessLevelID** Spalte in der Zeile von Chris.

   Wiederholen Sie diesen Schritt für jeden Benutzer und jede Zugriffsebene.

   ![](assets/copyalid-350x171.png) ![](assets/pastealid-350x59.png)

1. Geben Sie Details zur Home Group an.

   Dem Szenario zufolge gehört Chris Manning zur Marketing-Gruppe. Suchen Sie im Gruppierungsgruppenblatt die Kennung für die Marketing-Gruppe, kopieren Sie sie in die Zwischenablage und fügen Sie sie im Benutzerblatt in die **setHomeGroupID** Spalte in der Zeile von Chris. &#x200B;Wiederholen Sie diesen Schritt für jede Benutzer- und Gruppenzuweisung.

   ![](assets/copygroupid-1-350x133.png) ![](assets/pastegroupid-350x59.png)

1. Geben Sie Details zum Unternehmen an.

   Alle Benutzer in diesem Szenario gehören demselben Unternehmen an. Suchen Sie im Arbeitsblatt &quot;CMPY Company&quot;die ID für das Unternehmen *Ihre eigene Firma*, kopieren Sie die ID in die Zwischenablage und fügen Sie diesen Wert auf der Registerkarte &quot;USER-Benutzer&quot;in jede Zeile der Spalte &quot;setCompanyID&quot;ein. &#x200B;

   Wiederholen Sie diesen Schritt für jede Benutzer- und Gruppenzuweisung.

   ![](assets/companyid--1--350x78.png)

   ![](assets/pastecompanyid-350x84.png)

1. Geben Sie Details zur Auftragsrolle an.

   Dem Szenario zufolge wird Chris Manning die Rolle Business Analyst haben. Suchen Sie im Arbeitsblatt ROLE Role die ID für die Rolle Business Analyst , kopieren Sie sie in die Zwischenablage und fügen Sie sie im Arbeitsblatt USER User in die Zeile setRoleID in die Zeile Chris ein. &#x200B;Wiederholen Sie diesen Schritt für jede Benutzer- und Gruppenzuweisung.

   ![](assets/copyroleid-350x149.png)

   ![](assets/pasteroleid-350x95.png)

1. Füllen Sie bei Bedarf weitere Benutzerdetails aus und speichern Sie dann die Datei.
1. Importieren Sie die Excel-Datei.

   Befolgen Sie die Anweisungen im Abschnitt **Importieren von Kick Start-Dateien** Abschnitt dieses Artikels.
