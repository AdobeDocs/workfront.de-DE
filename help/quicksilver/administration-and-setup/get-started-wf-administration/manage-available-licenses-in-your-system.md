---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: start-with-workfront-administration
title: Verwalten der verfügbaren Lizenzen in Ihrem System
description: Als Adobe Workfront-Administrator können Sie auf Informationen zu Ihrem Workfront-Konto zugreifen, einschließlich der Anzahl der für Ihr Unternehmen erworbenen Lizenzen sowie der Anzahl der aktuell verwendeten Lizenzen.
author: Lisa, Becky
feature: System Setup and Administration
role: Admin
exl-id: ea580dd0-efb7-4f56-beb3-07ad044efc8a
source-git-commit: e971f08a1ee9bbf27a78916dbec57ca729407c03
workflow-type: tm+mt
source-wordcount: '1058'
ht-degree: 0%

---

# Verwalten der verfügbaren Lizenzen in Ihrem System

<!-- Audited: 12/2023 -->

Als Adobe Workfront-Administrator können Sie auf Informationen zu Ihrem Workfront-Konto zugreifen, einschließlich der Anzahl der für Ihr Unternehmen erworbenen Lizenzen sowie der Anzahl der aktuell verwendeten Lizenzen.

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Abo</td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td>
    <p>Neu: Standard</p>
    <p>oder</p>
    <p>Aktuell: Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Sie müssen Workfront-Administrator sein. Weitere Informationen finden Sie unter <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Gewähren eines vollen Administratorzugriffs</a>.</p> <p><b>NOTE</b>: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsstufe festgelegt hat. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Lizenzen Ihres Unternehmens anzeigen

Die Anzahl der verwendeten Lizenzen wird automatisch aktualisiert, wenn Sie den Benutzern, die Sie zu Workfront hinzufügen, Zugriffsebenen zuweisen. Weitere Informationen finden Sie unter [Benutzer hinzufügen](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

So zeigen Sie Lizenzinformationen in Ihrem System an:

{{step-1-to-setup}}

1. Klicken Sie unten im linken Bedienfeld auf **System** > **Lizenzen**.

   Weitere Informationen zu den auf dieser Seite aufgelisteten Lizenzen finden Sie unter [Überblick über Lizenzen](../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md).

   >[!NOTE]
   >
   >Testlizenzen stehen nur Kunden zur Verfügung, die zusätzlich zu ihrer Workfront-Lizenz das gebührenpflichtige Workfront Testversand-Add-on erworben haben. Weitere Informationen zu diesem Add-on finden Sie unter [Workfront-Testversand: Artikelindex](../../workfront-proof/workfront-proof.md).

1. (Bedingt) Wenn die Nachricht angezeigt wird **Um ein Maximum festzulegen, müssen Sie eine Startseite hinzufügen**, fügen Sie in Ihrem System eine Home Groups hinzu, wie im Abschnitt beschrieben. [Hinzufügen oder Entfernen einer Homepage-Gruppe zur Seite Lizenzen](#add-or-remove-a-home-group-to-the-licenses-page) in diesem Artikel.

## Anzeigen von Informationen zu Lizenzen für Workfront-Add-ons

Wenn Ihr Unternehmen über das gebührenpflichtige Workfront Testversand-Add-on verfügt, werden die Anzahl der verwendeten Lizenzen und die Anzahl der verfügbaren Lizenzen angezeigt. Beispiel: **5 von 10 Lizenzen** gibt an, dass das Unternehmen derzeit 5 der 10 von ihm erworbenen Workfront-Testlizenzen verwendet.

![Lizenz für Workfront-Add-ons](assets/updated-licenses-page.png)

Wenn Ihr Unternehmen Workfront-Ziele erworben hat, werden hier auch die Lizenzinformationen für dieses Produkt angezeigt. In diesem Fall können Sie die folgenden Informationen anzeigen:

* Gesamtanzahl der Workfront Goals-Lizenzen, die Ihr Unternehmen erworben hat
* Die Anzahl der Workfront Goals-Lizenzen, die mit Benutzern verknüpft sind. Dies ist die Anzahl der Benutzer, denen in ihrer Zugriffsebene mindestens Zugriff auf Ziele anzeigen gewährt werden soll.

Weitere Informationen zu Workfront-Zielen finden Sie unter [Übersicht über Adobe Workfront-Ziele](../../workfront-goals/goal-management/wf-goals-overview.md). Informationen zum Zugriff auf Workfront-Ziele finden Sie unter [Zugriff auf Adobe Workfront-Ziele gewähren](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md).

>[!NOTE]
>
>Mit Workfront können Sie weitere Workfront Goals-Lizenzen zuweisen, die Sie erworben haben. Wenn Sie jedoch mehr Lizenzen zuweisen, als Ihr Workfront Goals-Vertrag zulässt, setzt sich ein Workfront-Kundenbetreuer mit Ihnen in Verbindung, um Ihnen mitzuteilen, dass Sie Ihre Vertragsnummer überschritten haben.
>

<!--
If an organization has other paid add-on products, their license information also displays here. If the organization doesn't have any paid add-on products, nothing displays here. (Drafted this because not sure this is accurate: Scenario Planner is an add-on product and its licenses are not displayed there.)
-->

>[!TIP]
>
>Benutzer ohne Administratorzugriff können einen Gruppenbericht verwenden, um die Lizenzanzahl anzuzeigen. Erstellen Sie im Tab Bericht einen neuen Gruppenbericht und fügen Sie die folgenden Spalten hinzu:
>
>* Lizenztyp-Limit: Worker Limit
>* Lizenztyp-Limit: Planner Limit
>
>Weitere Informationen zum Erstellen eines Berichts finden Sie unter [Benutzerdefinierten Bericht erstellen](../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

## Anzeigen von Informationen zu monatlichen Zuweisungen von Testsendungen und Dokumententscheidungen

>[!IMPORTANT]
>
>Die Entscheidungsgrenzen für Beweise und Dokumente gelten nur für Benutzer der neuen Lizenzen. Weitere Informationen finden Sie unter [Übersicht über neue Lizenzen](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/licenses-overview.md).

Die Entscheidung über den Nachweis und die Unterlagen ist auf alle nicht bezahlten Workfront-Lizenzen beschränkt. Die Beschränkungen werden jeden Monat auf Benutzerbasis zurückgesetzt.

Die Entscheidungsgrenzen für jede Lizenz variieren je nach Plan. Sie können Ihre monatliche Zuteilung unter Einrichtung > Lizenzen anzeigen.

Weitere Informationen zu den Beschränkungen für Testsendungen und Dokumentenentscheidungen finden Sie unter [Begrenzte Dokument- und Testentscheidung für nicht bezahlte Benutzer - Überblick](/help/quicksilver/review-and-approve-work/proof-doc-decision-limits.md).

![Monatliche Entscheidungszuweisung](assets/monthly-decision-allotment.png)

## Hinzufügen oder Entfernen einer Homepage-Gruppe zur Seite Lizenzen {#add-or-remove-a-home-group-to-the-licenses-page}

<!--A Business or Enterprise Workfront Plan is required to use this feature. For more information about the various plans available, see [Workfront Plans.](https://www.workfront.com/plans)-->

Jeder Benutzer kann nur einer Home Group zugewiesen werden. Workfront bietet eine gruppenorientierte Lizenzanzahl, indem berechnet wird, wie viele Lizenzen in jeder Home Group zugewiesen und aktuell verwendet werden.

Wenn die Nachricht angezeigt wird **Um ein Maximum festzulegen, müssen Sie eine Startseite hinzufügen** auf der Seite Lizenzen müssen Sie mindestens eine Home Group zur Seite Lizenzen hinzufügen.

>[!IMPORTANT]
>
>* Um Lizenzen effektiv mit Stammgruppen verwalten zu können, empfehlen wir, spezifische Home Groups für Geschäftseinheiten einzurichten, bevor die maximale Lizenzanzahl aktualisiert wird. Weitere Informationen finden Sie unter [Übersicht über Startsegmente](../../administration-and-setup/manage-groups/groups-overview/home-groups.md).
>* Sie können nur Gruppen der obersten Ebene als Startseite und keine Untergruppen hinzufügen. Wenn einem Benutzer eine Untergruppe zugewiesen wurde, wird seine Lizenz zur Lizenzanzahl für die Gruppe der obersten Ebene oberhalb dieser Untergruppe hinzugefügt.
>

So fügen Sie der Lizenzseite eine Startseite hinzu oder entfernen sie:

{{step-1-to-setup}}

1. Klicken Sie unten im linken Bedienfeld auf **System** > **Lizenzen**.

1. Klicks **Gruppenliste verwalten**.
1. Geben Sie den Namen der Gruppe der obersten Ebene in die **Startseiten-Gruppen** ankreuzen.
1. Um die Gruppe hinzuzufügen, klicken Sie auf ihren Namen, sobald sie angezeigt wird.

   Oder

   Um die Gruppe zu entfernen, klicken Sie auf das X-Symbol rechts neben ihrem Namen.

1. Klicken Sie auf **Speichern**.

Als Workfront-Administrator können Sie für die Home Groups Höchstlizenzen festlegen, um zu verhindern, dass ein Geschäftsbereich Workfront-Lizenzen verwendet, die für andere Geschäftsbereiche erworben wurden. Anweisungen finden Sie unter [Maximale Lizenzanzahl für eine Home Group festlegen](#set-the-maximum-license-count-for-a-home-group) in diesem Artikel.

## Maximale Lizenzanzahl für eine Home Group festlegen {#set-the-maximum-license-count-for-a-home-group}

Als Workfront-Administrator können Sie die maximale Lizenzanzahl für die Home Groups der obersten Ebene in Ihrem System festlegen. Auf diese Weise können Sie verhindern, dass eine Geschäftseinheit Workfront-Lizenzen verwendet, die für andere Geschäftsbereiche in Ihrem Unternehmen erworben wurden.

Standardmäßig ist die maximale Lizenzanzahl auf &quot;N/A&quot;gesetzt, was bedeutet, dass es keine Beschränkung gibt.

Gruppenadministratoren können die Anzahl der erteilten und verwendeten Lizenzen in einer von ihnen verwalteten Home Group anzeigen. Weitere Informationen finden Sie unter [Anzahl der in einer Gruppe zugewiesenen und verwendeten Lizenzen anzeigen](../../administration-and-setup/manage-groups/create-and-manage-groups/view-number-licenses-allocated-used-group.md).

So legen Sie die maximale Lizenzanzahl für eine Home Group fest:

{{step-1-to-setup}}

1. Klicken Sie unten im linken Bedienfeld auf **System** > **Lizenzen**.

1. Suchen Sie die Startseite in der Liste.
1. Im **Max** -Spalte der Gruppe auf den Wert klicken, für den Sie ein Maximum festlegen möchten.
1. Geben Sie die Höchstzahl ein und drücken Sie dann die Eingabetaste.

   ![](assets/updated-max.png)

   >[!NOTE]
   >
   >Um den maximalen Lizenzwert einer Gruppe auf den Standardwert zurückzusetzen, geben Sie nicht 0 ein. Löschen Sie stattdessen die Nummer im Feld. Wird der maximale Lizenzwert auf 0 gesetzt, bedeutet dies, dass dieser Gruppe keine Lizenzen zugewiesen sind.
