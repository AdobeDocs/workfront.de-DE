---
product-area: workfront-integrations;projects
navigation-topic: workfront-for-salesforce
title: Create [!DNL Adobe Workfront] projects from [!DNL Salesforce] objects
description: Nach der Installation  [!DNL Adobe Workfront]  Salesforce können Sie Trigger definieren, die  [!DNL Workfront]  erstellen, wenn bestimmte Kriterien für  [!DNL Salesforce]  und Accounts erfüllt sind.
author: Becky
feature: Workfront Integrations and Apps
exl-id: b38c91ae-342b-4002-a947-7a0ab1aaca93
source-git-commit: f9af669b023309abc132421f35a2ece974e796b0
workflow-type: tm+mt
source-wordcount: '1581'
ht-degree: 3%

---

# Erstellen [!DNL Adobe Workfront] Projekte aus [!DNL Salesforce] Objekten

>[!IMPORTANT]
>
>Um stabilere und skalierbarere Integrationen bereitzustellen, wechseln wir mithilfe von Workfront Automation and Integration (Fusion) zu einem modernen, flexiblen Integrationsansatz. Im Rahmen dieses Übergangsprozesses wird die Integration von Workfront mit Salesforce nach dem 28. **2026 nicht mehr**.
>
>Es wird empfohlen, Workfront-Automatisierung und -Integration für die Integrationsanforderungen Ihres Unternehmens mit Salesforce zu verwenden.
>
>Einen Überblick über die Automatisierung und Integration von Workfront finden Sie unter [Übersicht über Adobe Workfront Fusion](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview).
>
>Informationen zu den spezifischen Funktionen der Workfront-Automatisierungs- und Integrationsmodule für Salesforce finden Sie unter [Salesforce-Module](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/salesforce-modules).

Nach der Installation von [!DNL Adobe Workfront] für Salesforce können Sie Trigger definieren, die [!DNL Workfront] erstellen, wenn bestimmte Kriterien in [!DNL Salesforce] ([!UICONTROL ) ] [!UICONTROL Accounts] erfüllt sind.

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die in diesem Artikel beschriebenen Funktionen nutzen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Plan*</td> 
   <td> <p>[!UICONTROL Pro] oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Lizenz*</td> 
   <td> <p>[!UICONTROL-Plan]</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren [!DNL Workfront], um herauszufinden, über welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie verfügen.

## Voraussetzungen

So senden Sie eine [!DNL Workfront] von einem [!DNL Salesforce] ([!UICONTROL ) ] Konto
Stellen Sie sicher, dass Ihre Umgebung über Folgendes verfügt:

* Ihr [!DNL Workfront] hat [!DNL Workfront for Salesforce] installiert.\
   Weitere Informationen zum Installieren von [!DNL Workfront for Salesforce] finden Sie unter [Installieren [!DNL Adobe Workfront for Salesforce]](../../workfront-integrations-and-apps/using-workfront-with-salesforce/install-workfront-for-salesforce.md)

* Ihr [!DNL Workfront] hat den Abschnitt [!DNL Workfront] zu Ihrem Konto [!UICONTROL Opportunity] hinzugefügt
Seiten-Layouts.\
   Weitere Informationen zum Hinzufügen des Abschnitts &quot;[!DNL Workfront]&quot; zu einem Seitenlayout finden Sie unter [Konfigurieren  [!DNL Adobe Workfront]  Abschnitts für  [!DNL Salesforce] -](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md).

* Sie haben ein [!DNL Workfront] Konto und können sich über den [!DNL Workfront] Abschnitt in Ihrem [!UICONTROL Opportunity] oder Konto anmelden
.

## Konfigurieren der Erstellung [!DNL Workfront] Projekte aus [!DNL Salesforce]

* [Grundlegendes zur automatischen Erstellung von Projekten](#understanding-the-automatic-creation-of-projects-understanding-the-automatic-creation-of-projects)
* [Konfigurieren von Triggern](#configuring-triggers-configuring-triggers)
* [Grundlegendes zu Projektnamen](#understanding-project-names-understanding-project-names)

### Grundlegendes zur automatischen Erstellung von Projekten {#understanding-the-automatic-creation-of-projects}

Als [!DNL Salesforce] können Sie Trigger definieren, die automatisch Projekte in [!DNL Workfront] erstellen können, wenn Folgendes in [!DNL Salesforce] passiert:

* Die [!UICONTROL Phase] einer [!UICONTROL Opportunity] wird aktualisiert.
* Der [!UICONTROL Typ] eines Kontos
wird aktualisiert.

Trigger können erst konfiguriert werden, nachdem Sie [!DNL Workfront for Salesforce] installiert haben.  \
Informationen zur Installation von [!DNL Workfront for Salesforce] finden Sie unter [Installieren [!DNL Adobe Workfront for Salesforce]](../../workfront-integrations-and-apps/using-workfront-with-salesforce/install-workfront-for-salesforce.md).

Beachten Sie Folgendes beim Konfigurieren von Triggern zum automatischen Erstellen [!DNL Workfront] Projekte, wenn [!DNL Salesforce] Elemente erstellt oder aktualisiert werden:

* Sie müssen ein [!DNL Salesforce] und ein [!DNL Workfront] Systemadministrator sein, um Trigger zu konfigurieren.
* Nachdem Sie die Trigger konfiguriert haben, gilt für alle, die [!UICONTROL Phase] einer [!UICONTROL Opportunity] oder den [!UICONTROL Typ] eines Kontos aktualisieren
kann die Erstellung eines [!DNL Workfront]-Projekts als Trigger speichern. Dazu gehören [!DNL Salesforce] Benutzer, die kein [!DNL Workfront]-Konto haben.
* Es gibt keine Begrenzung dafür, wie viele Trigger Sie haben können.
* Es ist nicht möglich, mehrere Trigger auf der Grundlage derselben Bedingungen zu erstellen. Trigger sind standardmäßig eindeutig.
* Nachdem das Projekt erstellt wurde, wird es automatisch mit der Opportunity oder dem Konto verknüpft, in dem es generiert wurde. Sobald diese Verbindung hergestellt ist, kann sie nicht mehr unterbrochen werden.
* Eine Opportunity oder ein Account kann in [!DNL Workfront] mit mehreren Projekten verknüpft werden, wenn eine ausgelöste Bedingung im Verlauf der Opportunity oder des Accounts mehrmals erfüllt wurde.

  Wenn Sie beispielsweise mehr als ein [!UICONTROL Stadium] für eine [!UICONTROL Opportunity] zum Trigger eines Projekts definieren, wird für jedes definierte Stadium, das die Opportunity erreicht, ein Projekt erstellt, und zwar für die Lebensdauer dieser Opportunity. Wenn Sie außerdem das [!UICONTROL Stadium] einer [!UICONTROL Opportunity] von einem definierten Stadium auf einen anderen aktualisieren und es dann wieder auf den definierten Stadium aktualisieren, wird zum zweiten Mal ein zweites Projekt erstellt, wenn Sie das [!UICONTROL Stadium]-Feld auf denselben definierten Stadium aktualisieren.

* Ein Projekt in [!DNL Workfront] kann jeweils nur mit einer Opportunity oder einem Konto in [!DNL Salesforce] verknüpft werden, aber nicht mit beiden gleichzeitig.

### Konfigurieren von Triggern {#configuring-triggers}

Nachdem Sie die Trigger konfiguriert haben, wird der Prozess zum Erstellen [!DNL Workfront] Projekte für [!UICONTROL Salesforce Classic]- oder [!DNL Lightning Experience]-Frameworks aktiviert.

So konfigurieren Sie Trigger in [!UICONTROL Salesforce]:

1. Melden Sie sich bei [!DNL Salesforce] als Systemadministrator an.
1. (Bedingt) Klicken Sie [!DNL Salesforce Classic] auf **[!UICONTROL Setup]** und erweitern Sie im Abschnitt **[!UICONTROL Build]** (**[!UICONTROL )]**.

   Oder

   Klicken Sie [!DNL Salesforce] Lightning-Erlebnis auf **[!UICONTROL Setup]-Symbol** dann **[!UICONTROL Setup]** und erweitern Sie unter **[!UICONTROL PLATFORM TOOLS]** **[!UICONTROL Apps]**.

1. Klicken Sie auf **[!UICONTROL Installierte Pakete]**.

   Beachten Sie, dass das **[!DNL Workfront]**-Paket installiert wurde.

1. Klicken Sie **[!UICONTROL Konfigurieren]** neben **[!DNL Workfront]**.

1. Melden Sie sich bei [!DNL Workfront] als Systemadministrator an.

   Die Seite **[!UICONTROL Trigger]** wird angezeigt.

   ![salesforce_Trigger_page_empty.png](assets/salesforce-triggers-page-empty-350x134.png)

1. Klicken Sie **[!UICONTROL Neuer Trigger]**.
1. Wählen Sie im Dropdown **[!UICONTROL [!DNL Salesforce]Menü]** Objekt“ die Option **[!UICONTROL Opportunity]**.

   Dies ist ein Pflichtfeld.

1. (Bedingt) Geben Sie Folgendes an:

   1. Wählen Sie aus **[!UICONTROL Dropdown]** Menü „Phase“ eine **[!UICONTROL Phase]**.\

      Wenn eine Opportunity das [!UICONTROL Stadium] hier angegeben erreicht, wird ein Projekt in [!DNL Workfront] erstellt. Dies ist ein Pflichtfeld.

   1. Beginnen Sie im Feld **[!UICONTROL Portfolio oder Programm]** mit der Eingabe des Namens einer Portfolio oder eines Programms, in der bzw. dem das Projekt [!DNL Workfront] werden soll, und wählen Sie es aus, wenn es in der Liste angezeigt wird.\

      Wenn Sie weder eine Portfolio noch ein Programm angeben, wird das neue Projekt erstellt und der Liste [!UICONTROL Projekte in meinem Besitz] des Benutzers hinzugefügt, der bei der Konfiguration der Trigger bei [!DNL Workfront] angemeldet ist. Dieser Benutzer ist auch der Projektbesitzer für das neue Projekt.

   1. Geben Sie den Namen einer Vorlage ein, die Sie mit dem neuen [!DNL Workfront] verknüpfen möchten, und wählen Sie sie aus, wenn sie in der Liste angezeigt wird.\

      Dies ist ein Pflichtfeld.


      >[!NOTE]
      >
      >Wenn Sie für die Vorlage, die Sie für diese Integration verwenden möchten, einen Vorlagenbesitzer angegeben haben, wird dieser zum Projektbesitzer des neuen Projekts. Die neuen Projekte werden je nach Vorlage unter [!UICONTROL Projekte in meinem ]) der Benutzerin bzw. des Benutzers angezeigt, die bzw. der Besitzer des neuen Projekts ist.

   1. (Optional) Wählen Sie das Feld **[!UICONTROL Neues Projekt für jeden verkauften Produkttyp erstellen] aus** wenn Sie ein neues Projekt für jeden Produkttyp erstellen möchten, der bei einer Opportunity verkauft wird.
   1. (Bedingt) Wählen Sie im Dropdown **** Menü **[!UICONTROL Produkt]** ein Produkt aus.

      Dies ist ein Pflichtfeld.

   1. (Bedingt) Beginnen Sie mit der Eingabe des Namens einer **[!UICONTROL Vorlage]**, die Sie mit dem neuen [!DNL Workfront]-Projekt verknüpfen möchten, wenn sich das angegebene Produkt auf der [!UICONTROL Opportunity] befindet. Auswählen, wenn es in der Liste angezeigt wird.

      Dies ist ein Pflichtfeld.

      Das Projekt, das erstellt wird, wenn ein neues Produkt zur [!DNL Salesforce] Opportunity hinzugefügt wird, wird derselben Portfolio oder demselben Programm hinzugefügt, die bzw. das für die Opportunity ausgewählt wurde.

      >[!IMPORTANT]
      >
      >Das Projekt wird nur erstellt, wenn die Phase bei der [!UICONTROL Opportunity“ aktualisiert ]. Ein eindeutiges Projekt wird für jedes Produkt erstellt, das beim Aktualisieren des Felds „Phase“ angegeben wird, und nicht, wenn die Produkte zu &quot;[!UICONTROL &quot; hinzugefügt ].

1. (Optional) Klicken Sie auf **[!UICONTROL Neuer Trigger]**.
1. (Optional) Wählen Sie im Dropdown **[!UICONTROL [!DNL Salesforce]Menü]**Objekt“ die Option **Konto
**.

   Dies ist ein Pflichtfeld.
1. (Bedingt) Geben Sie Folgendes an:

   1. Wählen Sie **[!UICONTROL Dropdown]** Menü **[!UICONTROL Typ]** aus.

      Wenn ein beliebiges **Konto
** wird als **[!UICONTROL Typ]** angegeben, hier [!DNL Salesforce] wird ein **[!UICONTROL Projekt]** in [!DNL Workfront] erstellt.

      Dies ist ein Pflichtfeld.

   1. (Optional) Beginnen Sie mit der Eingabe des Namens einer **[!UICONTROL Portfolio]** oder **[!UICONTROL Program]**, bei der das Projekt [!DNL Workfront] im Feld **[!UICONTROL Portfolio oder Program]** platziert werden soll, und wählen Sie es aus, wenn es in der Liste angezeigt wird.

      Wenn Sie weder eine Portfolio noch ein Programm angeben, wird das neue Projekt erstellt und der Liste **[!UICONTROL Projekte in meinem Besitz]** des Benutzers hinzugefügt, der von [!DNL Workfront] bei [!DNL Salesforce] angemeldet ist. Der Benutzer ist auch der Projektbesitzer für das neue Projekt.

   1. Geben Sie den Namen einer **[!UICONTROL Vorlage]** ein, die Sie mit dem neuen [!DNL Workfront] verknüpfen möchten, und wählen Sie ihn aus, wenn er in der Liste angezeigt wird.

      Dies ist ein Pflichtfeld.

      >[!NOTE]
      >
      >Wenn Sie für die Vorlage, die Sie für diese Integration verwenden möchten, einen Vorlagenbesitzer angegeben haben, wird dieser zum Projektbesitzer des neuen Projekts. Die neuen Projekte werden je nach Vorlage unter **[!UICONTROL Projekte in meinem]**) der Benutzerin bzw. des Benutzers angezeigt, die bzw. der Besitzer des neuen Projekts ist.

   ![salesforce_Trigger_page_with_cleanup_template_names.png](assets/salesforce-triggers-page-with-cleaned-up-template-names-350x157.png)

1. Klicken Sie auf **[!UICONTROL Speichern]**.

   [!DNL Workfront] Projekte werden jetzt jedes Mal generiert, wenn einer der Trigger erfüllt wird.

### Grundlegendes zu Projektnamen {#understanding-project-names}

Je nachdem, welcher Trigger die Projekte generiert hat, konnten die Namen der Projekte in [!DNL Workfront] einem der folgenden Muster entsprechen:

* Wenn das Projekt auf der Grundlage eines Opportunity- oder Account-Triggers erstellt wird, lautet der Name des Projekts: *`<Salesforce object name>`: `<Project template name>` (über [!DNL Salesforce])*
* Wenn das Projekt auf der Grundlage eines Opportunity-Triggers erstellt wird, der auch das Hinzufügen eines neuen Produkts umfasst, lautet der Name des Projekts: *`<Salesforce object name>`: `<Salesforce product name>` (über [!DNL Salesforce])*.

## [!DNL Workfront] Projekte anzeigen

Wenn Ihr [!DNL Workfront] den Abschnitt [!DNL Workfront] zu Ihrem [!UICONTROL Opportunity] oder Konto hinzugefügt hat
Seiten-Layout. Die automatisch erstellten Projekte werden auf der Registerkarte [!UICONTROL Projekte] dieses Abschnitts angezeigt.\
Weitere Informationen zum Hinzufügen des Abschnitts &quot;[!DNL Workfront]&quot; zum Seiten-Layout eines (Opportunity[!UICONTROL  oder ] Kontos
, siehe [Konfigurieren des  [!DNL Adobe Workfront] -Abschnitts  [!DNL Salesforce] -users](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md).

Sie müssen über ein [!DNL Workfront]-Konto verfügen und bei [!DNL Workfront] angemeldet sein, um die Registerkarte [!UICONTROL Projekte] anzeigen zu können.

So zeigen Sie Projekte an, die aus einem (Opportunity[!UICONTROL  oder ] Konto erstellt wurden
:

1. Zu einem [!UICONTROL Opportunity] oder Konto gehen
.
1. Navigieren Sie zum Abschnitt **[!DNL Workfront]** .

   >[!NOTE]
   >
   >Je nachdem, wie Ihr [!DNL Workfront] diesen Abschnitt konfiguriert hat, kann er einen anderen Namen haben.

1. Wählen Sie die **[!UICONTROL Projekte]** aus.

   Auf dieser Registerkarte werden alle von definierten Triggern erstellten Projekte aufgelistet. Jeder Benutzer in [!DNL Salesforce], der auch über ein [!DNL Workfront]-Konto verfügt und der möglicherweise berechtigt ist, diese Projekte in [!DNL Workfront] zu sehen, kann sie auch in [!DNL Salesforce] für die [!UICONTROL Opportunity] oder das Konto sehen
die sie hervorgebracht haben.

   Sie können die folgenden Informationen zu den von der Integration erstellten Projekten anzeigen:

   * Projektname
   * Referenznummer
   * Eingabedatum
   * Name des Inhabers
   * Status
   * Bedingung
   * Geplantes Abschlussdatum
   * Prozent abgeschlossen

     Wenn diese Informationen in [!DNL Workfront] aktualisiert werden, können Sie die in dieser Liste aktualisierten Felder sehen.

1. (Optional) Klicken Sie auf den Namen eines Projekts, um es in Workfront zu öffnen.
1. (Optional) Klicken Sie [!UICONTROL **[!UICONTROL Zu Salesforce gehen]**] im Bereich [!UICONTROL Projektdetails] oder im Projekt-Header, um auf die [!UICONTROL Opportunity] oder das Konto zuzugreifen
Ausgangspunkt des Projekts. Ihr System- oder Gruppenadministrator muss das Feld [!UICONTROL Integrationen] zu Ihrer Layout-Vorlage hinzufügen, um sie im Projekt-Header zu finden.

   >[!NOTE]
   >
   >Der [!UICONTROL Zu Salesforce wechseln]-Link ist für alle [!DNL Workfront] Benutzer sichtbar, die das Projekt anzeigen können. Sie müssen über ein [!DNL Salesforce]-Konto verfügen, um zu der Opportunity oder dem Konto [!DNL Salesforce] zu können, von der bzw. dem aus das Projekt generiert wurde.
