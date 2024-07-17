---
product-area: workfront-integrations;projects
navigation-topic: workfront-for-salesforce
title: Erstellen von [!DNL Adobe Workfront] Projekten aus  [!DNL Salesforce]  Objekten
description: Nach der Installation von [!DNL Adobe Workfront] für Salesforce können Sie Trigger definieren, die [!DNL Workfront] Projekte erstellen, wenn bestimmte Kriterien für  [!DNL Salesforce] Chancen und Konten erfüllt sind.
author: Becky
feature: Workfront Integrations and Apps
exl-id: b38c91ae-342b-4002-a947-7a0ab1aaca93
source-git-commit: ad2fc27db2a19ea231e925d5991dbef27ea48030
workflow-type: tm+mt
source-wordcount: '1496'
ht-degree: 3%

---

# Erstellen von [!DNL Adobe Workfront] Projekten aus [!DNL Salesforce] Objekten

Nach der Installation von [!DNL Adobe Workfront] für Salesforce können Sie Trigger definieren, die [!DNL Workfront] -Projekte erstellen, wenn bestimmte Kriterien für [!DNL Salesforce] [!UICONTROL Chancen] und [!UICONTROL Konten] erfüllt sind.

## Zugriffsanforderungen

Sie müssen über den folgenden Zugriff verfügen, um die in diesem Artikel beschriebene Funktion verwenden zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!UICONTROL Pro] oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td> <p>[!UICONTROL Plan]</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren [!DNL Workfront] -Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Voraussetzungen

So senden Sie eine [!DNL Workfront] -Anfrage von einem [!DNL Salesforce] [!UICONTROL Opportunity] oder Konto
Stellen Sie sicher, dass Sie Folgendes in Ihrer Umgebung haben:

* Ihr [!DNL Workfront] -Administrator hat [!DNL Workfront for Salesforce] installiert.\
   Weitere Informationen zum Installieren von [!DNL Workfront for Salesforce] finden Sie unter [Installieren [!DNL Adobe Workfront for Salesforce]](../../workfront-integrations-and-apps/using-workfront-with-salesforce/install-workfront-for-salesforce.md) .

* Ihr [!DNL Workfront] -Administrator hat Ihren [!UICONTROL Opportunity] und Ihrem Konto den Abschnitt [!DNL Workfront] hinzugefügt
Seitenlayouts.\
   Weitere Informationen zum Hinzufügen des Abschnitts [!DNL Workfront] zu einem Seitenlayout finden Sie unter [Konfigurieren des Abschnitts [!DNL Adobe Workfront] für  [!DNL Salesforce] Benutzer](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md).

* Sie haben ein [!DNL Workfront] -Konto und können sich über den Abschnitt [!DNL Workfront] in Ihrer [!UICONTROL Gelegenheit] oder Ihrem Konto bei ihm anmelden.
.

## Konfigurieren der Erstellung von [!DNL Workfront] Projekten von [!DNL Salesforce]

* [Grundlagen zur automatischen Projekterstellung](#understanding-the-automatic-creation-of-projects-understanding-the-automatic-creation-of-projects)
* [Konfigurieren von Trigger](#configuring-triggers-configuring-triggers)
* [Grundlegendes zu Projektnamen](#understanding-project-names-understanding-project-names)

### Grundlagen zur automatischen Projekterstellung {#understanding-the-automatic-creation-of-projects}

Als Systemadministrator von [!DNL Salesforce] können Sie Trigger definieren, die automatisch in [!DNL Workfront] Projekte erstellen können, wenn in [!DNL Salesforce] Folgendes geschieht:

* Die [!UICONTROL Phase] einer [!UICONTROL Gelegenheit] wird aktualisiert.
* Der [!UICONTROL Typ] eines Kontos
aktualisiert wird.

Trigger können erst konfiguriert werden, nachdem Sie [!DNL Workfront for Salesforce] installiert haben.  \
Weitere Informationen zum Installieren von [!DNL Workfront for Salesforce] finden Sie unter [Installieren [!DNL Adobe Workfront for Salesforce]](../../workfront-integrations-and-apps/using-workfront-with-salesforce/install-workfront-for-salesforce.md).

Beachten Sie Folgendes beim Konfigurieren von Triggern zum automatischen Erstellen von [!DNL Workfront]-Projekten, wenn [!DNL Salesforce] Elemente erstellt oder aktualisiert werden:

* Sie müssen ein [!DNL Salesforce] und ein [!DNL Workfront] Systemadministrator sein, um Trigger zu konfigurieren.
* Nachdem Sie die Trigger konfiguriert haben, alle, die die [!UICONTROL Phase] einer [!UICONTROL Gelegenheit] oder den [!UICONTROL Typ] eines Kontos aktualisieren
kann die Erstellung eines [!DNL Workfront] -Projekts Trigger werden. Dazu gehören [!DNL Salesforce] Benutzer, die kein [!DNL Workfront] -Konto haben.
* Es gibt keine Beschränkung für die Anzahl der Trigger, die Sie haben können.
* Sie können nicht mehrere Trigger erstellen, die auf denselben Bedingungen basieren. Trigger sind standardmäßig eindeutig.
* Nachdem das Projekt erstellt wurde, wird es automatisch mit der Gelegenheit oder dem Konto verknüpft, in dem es erstellt wurde. Sobald diese Verbindung hergestellt wurde, kann sie nicht mehr unterbrochen werden.
* Eine Chance oder ein Konto kann mit mehreren Projekten in [!DNL Workfront] verknüpft werden, wenn eine ausgelöste Bedingung während der Opportunity oder des Kontos mehrmals erfüllt wurde.

  Wenn Sie beispielsweise mehr als eine [!UICONTROL Phase] für eine [!UICONTROL Chance] definieren, um ein Projekt Trigger, wird für jede definierte Phase, die die Gelegenheit erreicht, ein Projekt erstellt, während dieser Gelegenheit. Wenn Sie außerdem die [!UICONTROL Phase] einer [!UICONTROL Gelegenheit] von einer definierten Phase zu einer anderen aktualisieren und sie dann wieder auf die definierte Phase aktualisieren, wird zum zweiten Mal ein zweites Projekt erstellt, wenn Sie das Feld [!UICONTROL Bühne] auf dieselbe definierte Phase aktualisieren.

* Ein Projekt in [!DNL Workfront] kann zu jeder Zeit nur mit einer Chance oder einem Konto in [!DNL Salesforce] verknüpft werden, jedoch nicht mit beiden gleichzeitig.

### Konfigurieren von Trigger {#configuring-triggers}

Nachdem Sie die Trigger konfiguriert haben, ist der Prozess zum Erstellen von [!DNL Workfront] -Projekten sowohl für die [!UICONTROL Salesforce Classic]- als auch für die [!DNL Lightning Experience]-Frameworks aktiviert.

So konfigurieren Sie Trigger in [!UICONTROL Salesforce]:

1. Melden Sie sich bei [!DNL Salesforce] als Systemadministrator an.
1. (Bedingt) Klicken Sie in &quot;[!DNL Salesforce Classic]&quot;auf &quot;**[!UICONTROL Setup]**&quot;und erweitern Sie unter dem Abschnitt &quot;**[!UICONTROL Build]**&quot;den Eintrag &quot;**[!UICONTROL Blitzschlag]**&quot;.

   Oder

   Klicken Sie in [!DNL Salesforce] Blitzererlebnis auf das Symbol **[!UICONTROL Einrichten]**, dann auf **[!UICONTROL Einrichtung]** und erweitern Sie unter **[!UICONTROL PLATFORM TOOLS]** den Eintrag **[!UICONTROL Apps]**.

1. Klicken Sie auf **[!UICONTROL Installierte Pakete]**.

   Beachten Sie, dass das **[!DNL Workfront]** -Paket installiert wurde.

1. Klicken Sie neben **[!DNL Workfront]** auf **[!UICONTROL Konfigurieren]** .

1. Melden Sie sich bei [!DNL Workfront] als Systemadministrator an.

   Die Seite **[!UICONTROL Trigger]** wird angezeigt.

   ![salesforce_Trigger_page_empty.png](assets/salesforce-triggers-page-empty-350x134.png)

1. Klicken Sie auf **[!UICONTROL Neuer Trigger]**.
1. Wählen Sie aus dem Dropdownmenü **[!UICONTROL [!DNL Salesforce]Objekt]** die Option **[!UICONTROL Chancen]** aus.

   Dies ist ein Pflichtfeld.

1. (Bedingt) Geben Sie Folgendes an:

   1. Wählen Sie aus dem Dropdownmenü **[!UICONTROL Bühne]** eine **[!UICONTROL Bühne]** aus.\

      Wenn eine Gelegenheit die hier angegebene [!UICONTROL Phase] erreicht, wird ein Projekt in [!DNL Workfront] erstellt. Dies ist ein Pflichtfeld.

   1. Geben Sie im Feld **[!UICONTROL Portfolio oder Programm]** den Namen eines Portfolios oder Programms ein, in das das Projekt eingefügt werden soll, und wählen Sie es aus, wenn es in der Liste angezeigt wird.\[!DNL Workfront]

      Wenn Sie kein Portfolio oder Programm angeben, wird das neue Projekt erstellt und der Liste [!UICONTROL Eigene Projekte] des Benutzers hinzugefügt, der sich bei der Konfiguration der Trigger bei [!DNL Workfront] angemeldet hat. Dieser Benutzer ist auch Projektinhaber des neuen Projekts.

   1. Beginnen Sie mit der Eingabe des Namens einer Vorlage, die Sie mit dem neuen [!DNL Workfront]-Projekt verknüpfen möchten, und wählen Sie sie aus, wenn sie in der Liste angezeigt wird.\

      Dies ist ein Pflichtfeld.


      >[!NOTE]
      >
      >Wenn Sie in der Vorlage, die Sie für diese Integration verwenden möchten, einen Vorlageninhaber angegeben haben, wird dieser zum Projektinhaber des neuen Projekts. Die neuen Projekte werden gemäß der Vorlage unter der Liste [!UICONTROL Projekte, deren Eigentümer ich bin] des Benutzers angezeigt, der Eigentümer des neuen Projekts ist.

   1. (Optional) Wählen Sie das Feld **[!UICONTROL Neues Projekt für jeden verkauften Produkttyp erstellen] aus, wenn Sie ein neues Projekt für jeden Produkttyp erstellen möchten, der unter einer beliebigen Gelegenheit verkauft wird.**
   1. (Bedingt) Wählen Sie ein **[!UICONTROL Produkt]** aus dem Dropdownmenü **[!UICONTROL Produkt]** aus.

      Dies ist ein Pflichtfeld.

   1. (Bedingt) Beginnen Sie mit der Eingabe des Namens einer **[!UICONTROL Vorlage]**, die Sie mit dem neuen [!DNL Workfront] -Projekt verknüpfen möchten, wenn das angegebene Produkt die [!UICONTROL Chance] aufweist. Wählen Sie sie aus, wenn sie in der Liste angezeigt wird.

      Dies ist ein Pflichtfeld.

      Das Projekt, das erstellt wird, wenn ein neues Produkt zur [!DNL Salesforce] -Gelegenheit hinzugefügt wird, wird in demselben Portfolio oder Programm platziert, das für die Gelegenheit ausgewählt wurde.

      >[!IMPORTANT]
      >
      >Das Projekt wird nur erstellt, wenn die Bühne auf der [!UICONTROL Opportunity] aktualisiert wird. Für jedes Produkt wird ein eindeutiges Projekt erstellt, das beim Aktualisieren des Staging-Felds angegeben wird, und nicht, da die Produkte zu [!UICONTROL Chancen] hinzugefügt werden.

1. (Optional) Klicken Sie auf **[!UICONTROL Neuer Trigger]**.
1. (Optional) Wählen Sie aus dem Dropdownmenü **[!UICONTROL [!DNL Salesforce]Objekt]** die Option &quot;Konto&quot;aus.
**.

   Dies ist ein Pflichtfeld.
1. (Bedingt) Geben Sie Folgendes an:

   1. Wählen Sie einen **[!UICONTROL Typ]** aus dem Dropdownmenü **[!UICONTROL Typ]** aus.

      Wenn ein **Konto
** als **[!UICONTROL Typ]** bezeichnet, der hier in [!DNL Salesforce] angegeben ist, wird ein **[!UICONTROL Projekt]** in [!DNL Workfront] erstellt.

      Dies ist ein Pflichtfeld.

   1. (Optional) Beginnen Sie mit der Eingabe des Namens eines **[!UICONTROL Portfolios]** oder **[!UICONTROL Programms]**, in das Sie das Projekt in [!DNL Workfront] im Feld **[!UICONTROL Portfolio oder Programm]** einfügen möchten, und wählen Sie es aus, wenn es in der Liste angezeigt wird.

      Wenn Sie kein Portfolio oder Programm angeben, wird das neue Projekt erstellt und der Liste **[!UICONTROL Eigene Projekte]** des Benutzers hinzugefügt, der sich von [!DNL Salesforce] bei [!DNL Workfront] angemeldet hat. Der Benutzer ist auch Projektinhaber des neuen Projekts.

   1. Geben Sie den Namen einer **[!UICONTROL Vorlage]** ein, die Sie mit dem neuen [!DNL Workfront] Projekt verknüpfen möchten, und wählen Sie sie dann aus, wenn sie in der Liste angezeigt wird.

      Dies ist ein Pflichtfeld.

      >[!NOTE]
      >
      >Wenn Sie in der Vorlage, die Sie für diese Integration verwenden möchten, einen Vorlageninhaber angegeben haben, wird dieser zum Projektinhaber des neuen Projekts. Die neuen Projekte werden gemäß der Vorlage unter der Liste **[!UICONTROL Projekte, deren Eigentümer ich bin]** des Benutzers angezeigt, der Eigentümer des neuen Projekts ist.

   ![salesforce_Trigger_page_with_cleanup_template_names.png](assets/salesforce-triggers-page-with-cleaned-up-template-names-350x157.png)

1. Klicken Sie auf **[!UICONTROL Speichern]**.

   [!DNL Workfront] -Projekte werden jetzt jedes Mal generiert, wenn ein Trigger erfüllt wird.

### Grundlegendes zu Projektnamen {#understanding-project-names}

Je nachdem, welcher Trigger die Projekte generiert hat, können die Projektnamen in [!DNL Workfront] einem der folgenden Muster folgen:

* Wenn das Projekt basierend auf einem Opportunities- oder Account-Trigger erstellt wird, lautet der Projektname: *`<Salesforce object name>`: `<Project template name>` (über [!DNL Salesforce])*.
* Wenn das Projekt auf Grundlage eines Opportunity-Triggers erstellt wird, der auch das Hinzufügen eines neuen Produkts umfasst, lautet der Projektname: *`<Salesforce object name>`: `<Salesforce product name>` (über [!DNL Salesforce])*.

## Anzeigen von [!DNL Workfront] Projekten

Wenn Ihr [!DNL Workfront]-Administrator Ihren [!UICONTROL Opportunity] oder Ihrem Konto den Abschnitt [!DNL Workfront] hinzugefügt hat
Seitenlayout, werden die automatisch erstellten Projekte auf der Registerkarte [!UICONTROL Projekte] dieses Abschnitts angezeigt.\
Weitere Informationen zum Hinzufügen des Bereichs [!DNL Workfront] zum Seitenlayout einer [!UICONTROL Gelegenheit] oder eines Kontos
, siehe Abschnitt [Konfigurieren des [!DNL Adobe Workfront] Abschnitts für [!DNL Salesforce] Benutzer](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md).

Sie müssen über ein [!DNL Workfront] -Konto verfügen und bei [!DNL Workfront] angemeldet sein, um die Registerkarte [!UICONTROL Projekte] anzuzeigen.

So zeigen Sie Projekte an, die aus einer [!UICONTROL Chance] oder einem Konto erstellt wurden
:

1. Gehen Sie zu einem [!UICONTROL Opportunity]- oder -Konto
.
1. Wechseln Sie zum Abschnitt &quot;**[!DNL Workfront]**&quot;.

   >[!NOTE]
   >
   >Je nachdem, wie Ihr [!DNL Workfront] -Administrator diesen Abschnitt konfiguriert hat, kann er einen anderen Namen haben.

1. Wählen Sie die Registerkarte **[!UICONTROL Projekte]** aus.

   Alle von definierten Triggern erstellten Projekte werden auf dieser Registerkarte aufgelistet. Jeder Benutzer in [!DNL Salesforce], der auch über ein [!DNL Workfront] -Konto verfügt und möglicherweise berechtigt ist, diese Projekte in [!DNL Workfront] anzuzeigen, kann sie auch in [!DNL Salesforce] für die [!UICONTROL Gelegenheit] oder das Konto sehen
die sie generiert haben.

   Sie können die folgenden Informationen zu den von der Integration erstellten Projekten anzeigen:

   * Projektname
   * Referenznummer
   * Eingabedatum
   * Name des Inhabers
   * Status
   * Bedingung
   * Geplantes Abschlussdatum
   * Prozent abgeschlossen

     Wenn diese Informationen in [!DNL Workfront] aktualisiert werden, werden die in dieser Liste aktualisierten Felder angezeigt.

1. (Optional) Klicken Sie auf den Namen eines Projekts, um es in Workfront zu öffnen.
1. (Optional) Klicken Sie im Bereich [!UICONTROL Projektdetails] auf [!UICONTROL **[!UICONTROL Gehe zu Salesforce]**] oder in der Projektheader, um auf die [!UICONTROL Gelegenheit] oder das Konto zuzugreifen.
wo das Projekt seinen Ursprung hat. Ihr System- oder Gruppenadministrator muss das Feld [!UICONTROL Integrationen] zu Ihrer Layoutvorlage hinzufügen, um es in der Projektheader zu finden.

   >[!NOTE]
   >
   >Der Link [!UICONTROL Gehe zu Salesforce] ist für alle [!DNL Workfront] Benutzer sichtbar, die das Projekt anzeigen können. Sie müssen über ein [!DNL Salesforce] -Konto verfügen, um zur [!DNL Salesforce] Gelegenheit oder zum Konto wechseln zu können, von dem aus das Projekt generiert wurde.
