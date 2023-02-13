---
user-type: administrator
product-area: system-administration;setup
navigation-topic: exchange-rates
title: Als Adobe Workfront-Administrator können Sie in Workfront Wechselkurse einrichten.
description: Wechselkurse einrichten
feature: System Setup and Administration
role: Admin
exl-id: 149c08de-fd3a-465a-afd1-0b53012d30d8
source-git-commit: 5d36c2c959dbfd00920eaf0a16409102b99de042
workflow-type: tm+mt
source-wordcount: '560'
ht-degree: 0%

---

# Wechselkurse einrichten

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">*** DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

Als Adobe Workfront-Administrator können Sie in Workfront Wechselkurse einrichten. Dazu gehört Folgendes:

* Festlegen der Standardwährung für das Workfront-System
* Aktualisierung der Wechselkurse in Workfront entsprechend den aktuellen Wechselkursen
* Wechselkurse für mehrere Währungen konfigurieren (dies ermöglicht Benutzern, für einzelne Projekte eine Standardwährung auszuwählen)

Wechselkurse wirken sich auf alle Finanzelemente in Workfront aus. Die Basiswährung ist die Standardwährung für alle Projekte im gesamten System, es sei denn, sie wird für ein bestimmtes Projekt oder eine bestimmte Auftragsrolle überschrieben. Sie können auch auswählen, ob Finanzinformationen in den in Ihrem System verfügbaren Währungen angezeigt werden sollen, die sich von der Basiswährung oder der des Projekts unterscheiden, wenn Sie sie in einem Bericht oder einer Liste anzeigen. Weitere Informationen finden Sie unter [Erstellen von Finanzdatenberichten mit eindeutigen Wechselkursen](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-financial-data-reports-unique-exchange-rates.md).

Weitere Informationen zum Überschreiben der Basiswährung in Workfront für Projekte und Stellenrollen finden Sie in den folgenden Artikeln:

* [Ändern der Projektwährung](../../../manage-work/projects/project-finances/change-project-currency.md)
* [Erstellen und Verwalten von Vorgangsrollen](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md)

Die Art und Weise, wie Sie Wechselkurse einrichten, beeinflusst, ob Benutzer die Wechselkurse für ein bestimmtes Projekt ändern können.

>[!IMPORTANT]
>
>Die Wechselkurse in Workfront sind nicht dynamisch. der von Ihnen festgelegte Wert muss bei Wechselkursänderungen aktualisiert werden.

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

## Wechselkurse einrichten

1. Klicken Sie auf **Hauptmenü** icon ![](assets/main-menu-icon.png) Klicken Sie oben rechts in Adobe Workfront auf **Einrichtung** ![](assets/gear-icon-settings.png).

1. Klicken **Projektvoreinstellungen** > **Wechselkurse.**

1. Klicken **Währung hinzufügen.**
1. Beginnen Sie mit der Eingabe des Währungsnamens und klicken Sie dann auf die Währung, wenn sie in der Dropdown-Liste angezeigt wird.

1. Geben Sie im bereitgestellten Feld den Wechselkurs für die gewählte Währung an, da er sich auf die Währung bezieht, die im System als Basiswährung festgelegt ist.
1. (Optional) Legen Sie die Währung als Basiswährung (Standard) für Workfront fest.

   Dies ist die Währung, die als Standard für alle Projekte und Berichte im gesamten System verwendet wird.

1. Klicken **Speichern** , um Ihre Änderungen zu speichern.

## Benutzer können die Standardwährung für ein Projekt ändern

Benutzer können die Standardwährung für ein Projekt ändern, wenn die folgenden Bedingungen erfüllt sind:

* Der Benutzer verfügt über eine Planungslizenz mit Administratorzugriff auf Wechselkurse.

   Weitere Informationen finden Sie unter [Benutzern administrativen Zugriff auf bestimmte Bereiche gewähren](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

* Im Workfront-System ist mehr als eine Währung aktiviert.

Informationen dazu, wie Benutzer die Standardwährung für ein bestimmtes Projekt ändern können, finden Sie unter [Ändern der Projektwährung](../../../manage-work/projects/project-finances/change-project-currency.md).

## Benutzern ermöglichen, die Standardwährung für eine Auftragsrolle zu ändern

Benutzer können die Währung für eine Auftragsrolle ändern, wenn die folgenden Bedingungen erfüllt sind:

* Der Benutzer verfügt über eine Planungslizenz mit Administratorzugriff auf &quot;Vorgangsrollen&quot;.

   Weitere Informationen finden Sie unter [Benutzern administrativen Zugriff auf bestimmte Bereiche gewähren](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

* Im Workfront-System ist mehr als eine Währung aktiviert.

Informationen dazu, wie Benutzer die Standardwährung für eine bestimmte Auftragsrolle ändern können, finden Sie unter [Erstellen und Verwalten von Vorgangsrollen](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).
