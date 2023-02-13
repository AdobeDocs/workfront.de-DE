---
product-area: workfront-integrations;projects
navigation-topic: workfront-for-salesforce
title: Erstellen [!DNL Adobe Workfront] Projekte aus [!DNL Salesforce] Objekte
description: Nach der Installation [!DNL Adobe Workfront] Für Salesforce können Sie Trigger definieren, die [!DNL Workfront] Projekte, bei denen bestimmte Kriterien erfüllt sind [!DNL Salesforce] Möglichkeiten und Konten.
author: Becky
feature: Workfront Integrations and Apps
exl-id: b38c91ae-342b-4002-a947-7a0ab1aaca93
source-git-commit: 5b889633a96d634a359181bfd53ec106b0f3705c
workflow-type: tm+mt
source-wordcount: '1507'
ht-degree: 3%

---

# Erstellen [!DNL Adobe Workfront] Projekte aus [!DNL Salesforce] Objekte

Nach der Installation [!DNL Adobe Workfront] Für Salesforce können Sie Trigger definieren, die [!DNL Workfront] Projekte, bei denen bestimmte Kriterien erfüllt sind [!DNL Salesforce] [!UICONTROL Chancen] und [!UICONTROL Konten].

## Zugriffsanforderungen

Sie müssen über den folgenden Zugriff verfügen, um die in diesem Artikel beschriebene Funktion verwenden zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Plan*</td> 
   <td> <p>[!UICONTROL Pro] oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td> <p>[!UICONTROL Plan]</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren [!DNL Workfront] Administrator.

## Voraussetzungen

So senden Sie eine [!DNL Workfront] Anfrage von [!DNL Salesforce] [!UICONTROL Chancen] oder Konto stellen Sie sicher, dass Sie Folgendes in Ihrer Umgebung haben:

* Ihre [!DNL Workfront] Der Administrator hat [!DNL Workfront for Salesforce].\
   Weitere Informationen zur Installation [!DNL Workfront for Salesforce], siehe [Installieren [!DNL Adobe Workfront for Salesforce]](../../workfront-integrations-and-apps/using-workfront-with-salesforce/install-workfront-for-salesforce.md)

* Ihre [!DNL Workfront] -Administrator hat [!DNL Workfront] zu Ihrer [!UICONTROL Chancen] und Kontoseitenlayouts.\
   Weitere Informationen zum Hinzufügen des [!DNL Workfront] Abschnitt zu einem Seitenlayout hinzufügen, siehe [Konfigurieren Sie die [!DNL Adobe Workfront] Abschnitt für [!DNL Salesforce] Benutzer](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md).

* Sie haben eine [!DNL Workfront] und Sie können sich über das [!DNL Workfront] Abschnitt in [!UICONTROL Chancen] oder Konto .

## Konfigurieren der Erstellung von [!DNL Workfront] Projekte aus [!DNL Salesforce]

* [Grundlagen zur automatischen Projekterstellung](#understanding-the-automatic-creation-of-projects-understanding-the-automatic-creation-of-projects)
* [Konfigurieren von Trigger](#configuring-triggers-configuring-triggers)
* [Grundlegendes zu Projektnamen](#understanding-project-names-understanding-project-names)

### Grundlagen zur automatischen Projekterstellung {#understanding-the-automatic-creation-of-projects}

Als [!DNL Salesforce] Systemadministrator: Sie können Trigger definieren, die automatisch Projekte in erstellen können. [!DNL Workfront] wenn folgende Vorgänge in [!DNL Salesforce]:

* Die [!UICONTROL Staging] von [!UICONTROL Chancen] aktualisiert wird.
* Die [!UICONTROL Typ] eines Kontos aktualisiert wird.

Trigger können erst nach der Installation konfiguriert werden [!DNL Workfront for Salesforce].  \
Informationen zur Installation [!DNL Workfront for Salesforce], siehe [Installieren [!DNL Adobe Workfront for Salesforce]](../../workfront-integrations-and-apps/using-workfront-with-salesforce/install-workfront-for-salesforce.md).

Beachten Sie Folgendes bei der Konfiguration von Triggern zur automatischen Erstellung [!DNL Workfront] Projekte, wenn [!DNL Salesforce] Elemente werden erstellt oder aktualisiert:

* Sie müssen [!DNL Salesforce] und [!DNL Workfront] Systemadministrator zum Konfigurieren von Triggern.
* Nach der Konfiguration der Trigger wird jeder Benutzer, der die [!UICONTROL Staging] von [!UICONTROL Chancen] oder [!UICONTROL Typ] eines Kontos kann die Erstellung eines [!DNL Workfront] Projekt. Dazu gehören [!DNL Salesforce] Benutzer ohne [!DNL Workfront] -Konto.
* Es gibt keine Beschränkung für die Anzahl der Trigger, die Sie haben können.
* Sie können nicht mehrere Trigger erstellen, die auf denselben Bedingungen basieren. Trigger sind standardmäßig eindeutig.
* Nachdem das Projekt erstellt wurde, wird es automatisch mit der Gelegenheit oder dem Konto verknüpft, in dem es erstellt wurde. Sobald diese Verbindung hergestellt wurde, kann sie nicht mehr unterbrochen werden.
* Eine Möglichkeit oder ein Konto kann mit mehreren Projekten in verknüpft werden. [!DNL Workfront] wenn eine ausgelöste Bedingung während der Lebensdauer der Gelegenheit oder des Kontos mehrmals erfüllt wurde.

   Wenn Sie beispielsweise mehr als eine [!UICONTROL Staging] für [!UICONTROL Chancen] zum Trigger eines Projekts wird ein Projekt für jede definierte Phase erstellt, die die Chance erreicht, für die Dauer dieser Gelegenheit. Wenn Sie die [!UICONTROL Staging] von [!UICONTROL Chancen] von einem definierten Schritt zum nächsten und dann zurück zum definierten Schritt, wird ein zweites Projekt erstellt, wenn Sie die [!UICONTROL Staging] auf dieselbe definierte Phase.

* Ein Projekt in [!DNL Workfront] kann nur mit einer Chance oder einem Konto in verknüpft werden. [!DNL Salesforce] zu jeder Zeit, aber nicht zu beiden gleichzeitig.

### Konfigurieren von Trigger {#configuring-triggers}

Nachdem Sie die Trigger konfiguriert haben, wird die [!DNL Workfront] -Projekte für beide [!UICONTROL Salesforce Classic] oder [!DNL Lightning Experience] Frameworks.

So konfigurieren Sie Trigger in [!UICONTROL Salesforce]:

1. Anmelden bei [!DNL Salesforce] als Systemadministrator.
1. (Bedingt) in [!DNL Salesforce Classic]klicken **[!UICONTROL Einrichtung]** und unter **[!UICONTROL Build]** Abschnitt erweitern **[!UICONTROL Blitzschlag]**.

   Oder

   In [!DNL Salesforce] Blitzererlebnis: Klicken Sie auf das **[!UICONTROL Einrichtung] icon**, dann **[!UICONTROL Einrichtung]** und **[!UICONTROL PLATTFORMWERKZEUGE]** Erweitern **[!UICONTROL Apps]**.

1. Klicken **[!UICONTROL Installierte Pakete]**.

   Beachten Sie, dass **[!DNL Workfront]** -Paket installiert wurde.

1. Klicken **[!UICONTROL Konfigurieren]** neben **[!DNL Workfront]**.

1. Anmelden bei [!DNL Workfront] als Systemadministrator.

   Die **[!UICONTROL Trigger]** angezeigt.

   ![salesforce_Trigger_page_empty.png](assets/salesforce-triggers-page-empty-350x134.png)

1. Klicken **[!UICONTROL Neuer Trigger]**.
1. Aus dem **[!UICONTROL [!DNL Salesforce]Objekt]** Dropdown-Menü auswählen **[!UICONTROL Chancen]**.

   Dies ist ein Pflichtfeld.

1. (Bedingt) Geben Sie Folgendes an:

   1. Aus dem **[!UICONTROL Staging]** Dropdown-Menü, wählen Sie eine **[!UICONTROL Staging]**.\

      Wenn eine Gelegenheit die [!UICONTROL Staging] Hier angegeben, wird ein Projekt erstellt in [!DNL Workfront]. Dies ist ein Pflichtfeld.

   1. Im **[!UICONTROL Portfolio oder Programm]** ein, geben Sie den Namen eines Portfolios oder Programms ein, in das das Projekt eingefügt werden soll. [!DNL Workfront]und wählen Sie sie dann aus, wenn sie in der Liste angezeigt wird.\

      Wenn Sie kein Portfolio oder Programm angeben, wird das neue Projekt erstellt und zum [!UICONTROL Eigene Projekte] Liste des Benutzers, der sich bei [!DNL Workfront] bei der Konfiguration der Trigger. Dieser Benutzer ist auch Projektinhaber des neuen Projekts.

   1. Beginnen Sie mit der Eingabe des Namens einer Vorlage, die Sie mit der neuen [!DNL Workfront] und wählen Sie es aus, wenn es in der Liste angezeigt wird.\

      Dies ist ein Pflichtfeld.


      >[!NOTE]
      >
      >Wenn Sie in der Vorlage, die Sie für diese Integration verwenden möchten, einen Vorlageninhaber angegeben haben, wird dieser zum Projektinhaber des neuen Projekts. Die neuen Projekte werden im [!UICONTROL Eigene Projekte] Liste des Benutzers, der Eigentümer des neuen Projekts ist, gemäß der Vorlage.

   1. (Optional) Wählen Sie die **[!UICONTROL Erstellen eines neuen Projekts für jeden verkauften Produkttyp] field**, wenn Sie ein neues Projekt für jeden Produkttyp erstellen möchten, der unter einer beliebigen Gelegenheit verkauft wird.
   1. (Bedingt) Wählen Sie eine **[!UICONTROL Produkt]** im **[!UICONTROL Produkt]** Dropdown-Menü.

      Dies ist ein Pflichtfeld.

   1. (Bedingt) Beginnen Sie mit der Eingabe des Namens eines **[!UICONTROL Vorlage]** , die Sie mit dem neuen [!DNL Workfront] -Projekt, wenn sich das angegebene Produkt im [!UICONTROL Chancen]. Wählen Sie sie aus, wenn sie in der Liste angezeigt wird.

      Dies ist ein Pflichtfeld.

      Das Projekt, das erstellt wird, wenn ein neues Produkt zum [!DNL Salesforce] im selben Portfolio oder Programm platziert wird, das für die Gelegenheit ausgewählt wurde.

      >[!IMPORTANT]
      >
      >Das Projekt wird nur erstellt, wenn die Bühne auf der [!UICONTROL Chancen]. Für jedes Produkt wird ein eindeutiges Projekt erstellt, das beim Aktualisieren des Staging-Felds angegeben wird, und nicht, da die Produkte zu [!UICONTROL Chancen].

1. (Optional) Klicken Sie auf **[!UICONTROL Neuer Trigger]**.
1. (Optional) Wählen Sie im **[!UICONTROL [!DNL Salesforce]Objekt]** Dropdownmenü die Option &quot;Konto&quot;auswählen.

   Dies ist ein Pflichtfeld.
1. (Bedingt) Geben Sie Folgendes an:

   1. Wählen Sie eine **[!UICONTROL Typ]** von **[!UICONTROL Typ]** Dropdown-Menü.

      Wenn ein **Konto ** als **[!UICONTROL Typ]** hier angegeben in [!DNL Salesforce], **[!UICONTROL Projekt]** wird in [!DNL Workfront].

      Dies ist ein Pflichtfeld.

   1. (Optional) Beginnen Sie mit der Eingabe des Namens eines **[!UICONTROL Portfolio]** oder **[!UICONTROL Programm]** wo das Projekt platziert werden soll [!DNL Workfront] im **[!UICONTROL Portfolio oder Programm]** und wählen Sie es aus, wenn es in der Liste angezeigt wird.

      Wenn Sie kein Portfolio oder Programm angeben, wird das neue Projekt erstellt und zum **[!UICONTROL Eigene Projekte]** Liste des Benutzers, der sich bei [!DNL Workfront] von [!DNL Salesforce]. Der Benutzer ist auch Projektinhaber des neuen Projekts.

   1. Geben Sie den Namen eines **[!UICONTROL Vorlage]** , die Sie mit dem neuen [!DNL Workfront] und wählen Sie es aus, wenn es in der Liste angezeigt wird.

      Dies ist ein Pflichtfeld.

      >[!NOTE]
      >
      >Wenn Sie in der Vorlage, die Sie für diese Integration verwenden möchten, einen Vorlageninhaber angegeben haben, wird dieser zum Projektinhaber des neuen Projekts. Die neuen Projekte werden im **[!UICONTROL Eigene Projekte]** Liste des Benutzers, der Eigentümer des neuen Projekts ist, gemäß der Vorlage.
   ![salesforce_Trigger_page_with_cleanup_template_names.png](assets/salesforce-triggers-page-with-cleaned-up-template-names-350x157.png)

1. Klicken Sie auf **[!UICONTROL Speichern]**.

   [!DNL Workfront] -Projekte werden jetzt jedes Mal erstellt, wenn ein Trigger erfüllt wird.

### Grundlegendes zu Projektnamen {#understanding-project-names}

Je nachdem, welcher Trigger die Projekte generiert hat, werden die Projektnamen in [!DNL Workfront] kann einem der folgenden Muster folgen:

* Wenn das Projekt auf der Grundlage eines Opportunity- oder Account-Triggers erstellt wird, lautet der Projektname: *`<Salesforce object name>`: `<Project template name>` (via [!DNL Salesforce])*.
* Wenn das Projekt auf Grundlage eines Opportunity-Triggers erstellt wird, der auch das Hinzufügen eines neuen Produkts umfasst, lautet der Projektname: *`<Salesforce object name>`: `<Salesforce product name>` (via [!DNL Salesforce])*.

## Ansicht [!DNL Workfront] Projekte

Wenn [!DNL Workfront] Administrator hat [!DNL Workfront] zu Ihrer [!UICONTROL Chancen] oder dem Seiten-Layout Konto die automatisch erstellten Projekte im [!UICONTROL Projekte] in diesem Abschnitt.\
Weitere Informationen zum Hinzufügen des [!DNL Workfront] zum Seitenlayout eines [!UICONTROL Chancen] oder Konto , siehe [Konfigurieren Sie die [!DNL Adobe Workfront] Abschnitt für [!DNL Salesforce] Benutzer](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md).

Sie müssen über eine [!DNL Workfront] -Konto und -Anmeldung bei [!DNL Workfront] , um die [!UICONTROL Projekte] Registerkarte.

So zeigen Sie Projekte an, die aus einem [!UICONTROL Chancen] oder Konto :

1. Gehen Sie zu einer [!UICONTROL Chancen] oder Konto .
1. Navigieren Sie zu **[!DNL Workfront]** Abschnitt.

   >[!NOTE]
   >
   >Je nachdem, wie Ihre [!DNL Workfront] Administrator diesen Abschnitt konfiguriert haben, kann es einen anderen Namen haben.

1. Wählen Sie die **[!UICONTROL Projekte]** Registerkarte.

   Alle von definierten Triggern erstellten Projekte werden auf dieser Registerkarte aufgelistet. Jeder Benutzer in [!DNL Salesforce] , die auch [!DNL Workfront] und wer möglicherweise berechtigt ist, diese Projekte in [!DNL Workfront] kann sie auch in [!DNL Salesforce] für [!UICONTROL Chancen] oder das Konto, von dem sie generiert wurden.

   ![[!DNL salesforce_projects_tab_with_projects_listed].png](assets/salesforce-projects-tab-with-projects-listed-350x150.png)

   Sie können die folgenden Informationen zu den von der Integration erstellten Projekten anzeigen:

   * Projektname
   * Referenznummer
   * Eingabedatum
   * Name des Inhabers
   * Status
   * Bedingung
   * Geplantes Abschlussdatum
   * Prozent abgeschlossen

      Wenn diese Informationen aktualisiert werden in [!DNL Workfront]angezeigt, können Sie die in dieser Liste aktualisierten Felder sehen.

1. (Optional) Klicken Sie auf den Namen eines Projekts, um es in Workfront zu öffnen.
1. (Optional) Klicken Sie auf [!UICONTROL **[!UICONTROL Gehe zu Salesforce]**] im [!UICONTROL Projektdetails] -Bereich oder der Projektheader, um auf die [!UICONTROL Chancen] oder das Konto, aus dem das Projekt stammt. Ihr System- oder Gruppenadministrator muss [!UICONTROL Integrationen] in Ihre Layout-Vorlage ein, um sie in der Projektheader zu finden.

   >[!NOTE]
   >
   >Die [!UICONTROL Gehe zu Salesforce] Link für alle sichtbar [!DNL Workfront] Benutzer, die das Projekt anzeigen können. Sie müssen über eine [!DNL Salesforce] -Konto, um zur [!DNL Salesforce] Gelegenheit oder Konto, von dem aus das Projekt generiert wurde.
