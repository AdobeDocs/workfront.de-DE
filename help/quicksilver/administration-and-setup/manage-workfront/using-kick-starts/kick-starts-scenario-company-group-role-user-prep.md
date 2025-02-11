---
user-type: administrator
product-area: system-administration;user-management
keywords: Kickstart,Kickstart,Kickstarts,Kickstarts
navigation-topic: use-kick-starts
title: 'Kickstarts-Szenario: Unternehmen, Gruppe, Rolle und Benutzer-Kickstarts Vorbereitung'
description: Wenn Sie mit der Implementierung von Adobe Workfront beginnen, können Sie anstelle der manuellen Eingabe von Daten Ihre Kundenliste, interne Abteilungen, Aufgabengebiete und Benutzerinformationen importieren.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: b83e2e35-dd9d-4d98-b8d4-2f8718b3c6c1
source-git-commit: 612243e928c6053d9b02715d9fcfef4dae25cb7a
workflow-type: tm+mt
source-wordcount: '1150'
ht-degree: 2%

---

# Kickstarts-Szenario: Unternehmen, Gruppe, Rolle und Benutzer-Kickstarts Vorbereitung

Wenn Sie mit der Implementierung von Adobe Workfront beginnen, können Sie anstelle der manuellen Eingabe von Daten Ihre Kundenliste, interne Abteilungen, Aufgabengebiete und Benutzerinformationen importieren.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan</td> 
   <td>Beliebig</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td>
   <p> Neu: Standard</p>
   oder
   <p>Aktuell: Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td>[!UICONTROL Systemadministrator]</td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Was importiert werden kann

In der folgenden Tabelle werden die zu importierenden Unternehmen, Gruppen und Rollen angezeigt:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Firmen</strong> </th> 
   <th><strong>Gruppen</strong> </th> 
   <th><strong>Rollen</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td valign="top"> <p>ACME, CO</p> <p>Workfront, Inc.</p> <p><em>Ihre Firma</em> </p> <p>XYZ, Inc.</p> </td> 
   <td valign="top"> <p valign="top" rowspan="7">Finanzielle Details</p> <p valign="top" rowspan="7">IT </p> <p valign="top" rowspan="7">Marketing </p> <p valign="top" rowspan="7">Verkauf</p> </td> 
   <td valign="top"> <p valign="top">Wirtschaftsanalytiker</p> <p valign="top">Kreativ-Controller</p> <p valign="top">Entwerfende Person</p> <p valign="top">Ressourcenmanager</p> <p valign="top">Scrum Master</p> <p valign="top">technischer Redakteur</p> <p valign="top">Web-Entwickler</p> </td> 
  </tr> 
 </tbody> 
</table>

Rollennamen müssen eindeutig sein. Vorhandene Aufgabengebiete können nicht importiert werden.

In den folgenden Tabellen werden die zu importierenden Benutzer und jeweils mehrere Benutzerattribute angezeigt:

### Benutzer 1

| **Vorname** | Chris |
|---|---|
| **Nachname** | Besatzung |
| **Benutzername/E-Mail** | mailto:cmanning@foo.com |
| **Kennwort** | updateMe |
| **Zugriff** | Teammitglied |
| **Firma** | &lt;*Ihre Firma>* |
| **Hauptgruppe** | Marketing |
| **Aufgabengebiet** | Wirtschaftsanalytiker |

{style="table-layout:auto"}

### Benutzer 2

| **Vorname** | Jennifer |
|---|---|
| **Nachname** | Campbell |
| **Benutzername/E-Mail** | jcampbell@foo.com |
| **Kennwort** | updateMe |
| **Zugriff** | Project Manager |
| **Firma** | &lt;*Ihre Firma>* |
| **Hauptgruppe** | Marketing |
| **Aufgabengebiet** | Project Manager |

{style="table-layout:auto"}

### Benutzer 3

| **Vorname** | Jill |
|---|---|
| **Nachname** | Sullivan |
| **Benutzername/E-Mail** | jsullivan@foo.com |
| **Kennwort** | updateMe |
| **Zugriff** | Helpdesk |
| **Firma** | &lt;*Ihre Firma>* |
| **Hauptgruppe** | Verkauf |
| **Aufgabengebiet** | Vertriebsmitarbeiter |

{style="table-layout:auto"}

### Benutzer 4

| **Vorname** | Trester |
|---|---|
| **Nachname** | Lewis |
| **Benutzername/E-Mail** | mlewis@foo.com |
| **Kennwort** | updateMe |
| **Zugriff** | Portfolio-Manager |
| **Firma** | &lt;*Ihre Firma>* |
| **Hauptgruppe** | Finanzielle Details |
| **Aufgabengebiet** | Controller |

{style="table-layout:auto"}

### Benutzer 5

| **Vorname** | Pam |
|---|---|
| **Nachname** | Reynolds |
| **Benutzername/E-Mail** | preynolds@foo.com |
| **Kennwort** | updateMe |
| **Zugriff** | Project Manager |
| **Firma** | *Ihre Firma>* |
| **Hauptgruppe** | Marketing |
| **Aufgabengebiet** | IT |

{style="table-layout:auto"}

### Benutzer 6

| **Vorname** | Strahl |
|---|---|
| **Nachname** | Andrews |
| **Benutzername/E-Mail** | randrews@foo.com |
| **Kennwort** | updateMe |
| **Zugriff** | Administrator |
| **Firma** | *Ihre Firma>* |
| **Hauptgruppe** | Ressourcenmanager |
| **Aufgabengebiet** | Keine |

{style="table-layout:auto"}

## Kickstart-Vorlage herunterladen

{{step-1-to-setup}}

1. Klicken Sie auf **System** > **Kickstarts** > **Daten importieren.**

1. Klicken Sie **Weitere Optionen**, um die vollständige Liste der Importoptionen anzuzeigen.
1. Wählen Sie Zugriffsebene, Unternehmen, Gruppe, Aufgabengebiet und Benutzerobjekte aus, die Sie importieren möchten.

## Firmeninformationen eingeben

1. Öffnen Sie die Datei **Workfront.xlsx**, die Sie gerade heruntergeladen haben.

   >[!TIP]
   >
   >Wenn Sie mit sehr breiten Datenblättern arbeiten, können Sie das Tool zum Einfrieren (oder Ähnliches) Ihres Tabelleneditors verwenden, um die Arbeit mit der Tabelle zu vereinfachen.

1. Zum Blatt „Firma“ gehen.

   Es sollte leer bleiben, es sei denn, Unternehmen sind bereits im System. ![Firmenblatt](assets/cmpysheet-350x16.png)

   ![Unternehmens-ID](assets/companyid--1--350x78.png)

1. Geben Sie TRUE in die Spalte **isNew** ein.
1. Wiederholen Sie diese Aktion für jede hinzugefügte Firma. (Führen Sie in diesem Beispiel diese Aktion für die Zeilen 3-6 aus, da vier Unternehmen hinzugefügt werden.)

   ![Unternehmen ist neu](assets/cmpyisnew-350x86.png)

1. Geben Sie eine eindeutige ID an.

   Dies muss für jede Zeile der Spalte ID erfolgen. Ganzzahlen, die mit 1 beginnen, funktionieren beim Erstellen neuer Datensätze gut.

   ![Unternehmen ist neu](assets/cmpyisnew-350x86.png)

1. Einen Namen festlegen.

   Geben Sie die Namen der einzelnen Kunden in der Spalte **setName** an.

   ![Unternehmens-ID](assets/companyid-350x78.png)

1. Navigieren Sie zur Tabelle GRUPPE .

   Sofern Sie noch keine Gruppen in Workfront erstellt haben, sollte dieses Blatt nur die Standardgruppe anzeigen, die mit jedem Konto von Workfront bereitgestellt wurde.

   ![Gruppenblatt](assets/groupsheet-350x15.png) ![Leeres Gruppenblatt](assets/emptygroupsheet-350x85.png)

1. Legen Sie die Spalte **isNew** fest. Je nach Szenario werden 4 Gruppen importiert. Geben Sie also „TRUE“ in die Zeilen 4 bis 7 für die Spalte „isNew“ ein.
1. Geben Sie eine eindeutige ID an.

   Dies muss für jede Zeile der Spalte ID erfolgen. Ganzzahlen, die mit 1 beginnen, funktionieren beim Erstellen neuer Datensätze gut.

   ![Gruppen-IDs](assets/groupids-350x85.png)

1. Einen Namen festlegen.

   Geben Sie die Namen der einzelnen Abteilungen in der Spalte &quot;**&quot;**.

   ![Gruppennamen](assets/groupnames-350x85.png)

   Geben Sie Rolleninformationen an. Navigieren Sie zum Funktionsblatt.

1. Sofern Sie in Ihrem Konto noch keine Rollen erstellt oder gelöscht haben, sollte dieses Blatt acht Rollen anzeigen, die mit jedem Konto von Workfront bereitgestellt werden.

   ![Gruppennamen](assets/groupnames-350x85.png)

1. True-Anweisung festlegen.

   Es werden sieben Aufgabengebiete importiert. Geben Sie TRUE in die Zeilen 12 bis 18 für die Spalte „isNew“ ein.

   ![Rolle ist neu](assets/roleisnew-350x104.png)

1. Geben Sie eine eindeutige ID an.

   Dies muss für jede Zeile der Spalte ID erfolgen. Ganzzahlen, die mit 1 beginnen, funktionieren beim Erstellen neuer Datensätze gut.

   ![Benutzerblatt](assets/usersheet-350x16.png)

   ![Rolle ist neu](assets/roleisnew--1--350x104.png)

1. Geben Sie für jede Rolle einen Namen an, indem Sie ihn in die Spalte „setName“ eingeben.

   ![Rolle ist neu](assets/roleisnew-350x104.png)

1. Geben Sie bei Bedarf zusätzliche Details an.

   Geben Sie bei Bedarf Abrechnungssätze, Kostensätze und Beschreibungen für die Rollen an, die Sie erstellen.

1. Gehen Sie zum Benutzerblatt, um Benutzerinformationen einzugeben.

   Sofern Sie noch keine Benutzenden in Ihrem Konto erstellt haben, sollte dieses Blatt nur die Admin-Benutzenden anzeigen, die mit jedem Konto von Workfront ausgestattet sind.

   ![Rollennamen](assets/rolenames-350x104.png) ![Leeres Benutzerblatt](assets/emptyusersheet-350x52.png)

1. Legen Sie den Wert „True“ fest, indem Sie TRUE in die Zeilen 4 bis 9 für die Spalte „isNew“ eingeben, da 6 Benutzer importiert werden.

   ![Benutzer ist neu](assets/userisnew-350x52.png)

1. Legen Sie eine eindeutige ID fest, indem Sie in jeder Zeile für die Spalte ID eine eindeutige ID angeben. Normalerweise funktionieren Ganzzahlen, die bei 1 beginnen, gut für neue Datensätze.

   ![Benutzer ist neu](assets/userisnew-350x52.png)

1. Die Namen der einzelnen Benutzer in die Spalten „setFirstName“ und „setLastName“ eingeben.

   ![Benutzernamen](assets/usernames-350x52.png)

1. Legen Sie Detailwerte fest, indem Sie Werte in die Spalten „setEmail“, „setPassword“ und „setUsername“ eingeben.

   ![Benutzeranmeldeinformationen](assets/usercredentials-350x52.png)

1. Geben Sie Werte für die Zugriffsebene an.

   Beispiel: Chris Manning, der ein Teammitglied ist, sucht im Blatt „ACSLVL-Zugriffsebene“ nach der ID für die Zugriffsebene der Teammitglieder. Kopieren Sie die ID in die Zwischenablage und fügen Sie sie im Benutzerblatt in die Spalte **setAccessLevelID** in der Zeile von Chris ein.

   Wiederholen Sie diesen Schritt für jeden Benutzer und jede Zugriffsebene.

   ![Zugriffsebenen-ID kopieren](assets/copyalid-350x171.png) ![Zugriffsebenen-ID einfügen](assets/pastealid-350x59.png)

1. Details zur Hauptgruppe angeben.

   Gemäß dem Szenario gehört Chris Manning zur Marketing-Gruppe. Suchen Sie auf dem Blatt GRUPPE die ID für die Marketing-Gruppe, kopieren Sie sie in die Zwischenablage und fügen Sie sie auf dem Blatt BENUTZER in die Spalte **setHomeGroupID** in der Zeile von Chris ein. &#x200B;Wiederholen Sie diesen Schritt für jede Benutzer- und Gruppenzuweisung.

   ![Gruppen-ID kopieren](assets/copygroupid-1-350x133.png) ![Gruppen-ID einfügen](assets/pastegroupid-350x59.png)

1. Geben Sie Details zum Unternehmen an.

   Alle Benutzer in diesem Szenario gehören demselben Unternehmen. Suchen Sie auf dem Blatt „Unternehmen kopieren“ die ID für das Unternehmen „Ihr eigenes Unternehmen“, kopieren Sie die ID in die Zwischenablage und fügen Sie diesen Wert auf der Registerkarte „Benutzer“ in jede Zeile der Spalte „setCompanyID“ ein&#x200B;

   Wiederholen Sie diesen Schritt für jede Benutzer- und Gruppenzuweisung.

   ![Unternehmens-ID](assets/companyid--1--350x78.png)

   ![Firmen-ID einfügen](assets/pastecompanyid-350x84.png)

1. Geben Sie Details zum Aufgabengebiet an.

   Dem Szenario zufolge wird Chris Manning die Rolle eines Unternehmensanalysten haben. Suchen Sie auf dem Blatt „Rolle“ die ID für die Rolle „Geschäftsanalyst“, kopieren Sie sie in die Zwischenablage und fügen Sie sie auf dem Blatt „Benutzer“ in die Zeile „setRoleID“ in der Zeile „Chris“ ein. &#x200B;Wiederholen Sie diesen Schritt für jede Benutzer- und Gruppenzuweisung.

   ![Rollenkennung kopieren](assets/copyroleid-350x149.png)

   ![Rollenkennung einfügen](assets/pasteroleid-350x95.png)

1. Geben Sie bei Bedarf weitere Benutzerdetails ein und speichern Sie dann die Datei.
1. Importieren Sie die Excel-Datei.

   Befolgen Sie die Anweisungen unter [Importieren von Daten in Adobe Workfront mithilfe einer Kickstart-Vorlage](/help/quicksilver/administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md).
