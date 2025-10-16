---
title: Zugriff auf Berichte, Dashboards und Kalender gewähren
user-type: administrator
product-area: system-administration;dashboards;calendars
navigation-topic: configure-access-to-workfront
description: Als Adobe Workfront-Administrator können Sie eine Zugriffsebene verwenden, um den Zugriff eines Benutzers auf Berichte, Dashboards und Kalender in Workfront zu definieren.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 776bb223-3481-4ea9-8049-276b2dec95c5
source-git-commit: 2a83e5a415ff254cf5525d6f44ecb0e447e7e70a
workflow-type: tm+mt
source-wordcount: '576'
ht-degree: 0%

---

# Zugriff auf Berichte, Dashboards und Kalender gewähren

Als Adobe Workfront-Administrator können Sie eine Zugriffsebene verwenden, um den Zugriff eines Benutzers auf Berichte, Dashboards und Kalender zu definieren, wie in [Übersicht über Zugriffsebenen](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md) beschrieben.

Dieser Zugriff umfasst auch den Zugriff auf externe Seiten. Informationen zu externen Seiten finden Sie unter [Zugriff auf Finanzdaten gewähren](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

>[!NOTE]
>
>* Wenn Sie Benutzern Zugriff auf Berichte, Dashboards und Kalender gewähren möchten, müssen Sie diesen Benutzern auch Zugriff auf Filter, Ansichten und Gruppierungen gewähren. Anweisungen finden Sie unter [Zugriff auf Filter, Ansichten und Gruppierungen gewähren](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-fvg.md).
>* Wenn jemand einen Bericht, ein Dashboard oder einen Kalender für einen anderen Benutzer freigibt, werden die Rechte des Empfängers durch eine Kombination zweier Dinge bestimmt: die Zugriffsebenen-Einstellung des Empfängers für Berichte, Dashboards und Kalender _und_ Berechtigungen, die der Freigabe für den Bericht, das Dashboard oder den Kalender gewährt hat
>
>Informationen zu Berechtigungen, die Benutzende für einen Bericht, ein Dashboard oder einen Kalender bei der Freigabe erteilen können, finden Sie [Freigeben von Berichten, Dashboards und Kalendern](../../../workfront-basics/grant-and-request-access-to-objects/permissions-reports-dashboards-calendars.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Paket</td> 
   <td>Beliebig</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td><p>Standard</p>
   <p>Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Sie müssen ein Workfront-Administrator sein.</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Konfigurieren des Benutzerzugriffs auf Berichte, Dashboards und Kalender mit einer benutzerdefinierten Zugriffsebene

1. Erstellen oder bearbeiten Sie die Zugriffsebene, wie unter [Erstellen oder Ändern benutzerdefinierter Zugriffsebenen“ &#x200B;](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
1. Klicken Sie auf das Zahnradsymbol ![](assets/gear-icon-settings.png) der Schaltfläche **Anzeigen** oder **Bearbeiten** rechts neben „Berichte“ und wählen Sie dann die Funktionen aus, die Sie unter **Einstellungen optimieren** gewähren möchten.

   ![reports_access.png](assets/reports-access.png)

   Die folgenden Optionen sind standardmäßig aktiviert:

   * **Erstellen**
   * **Löschen**
   * **Integrierte Berichte anzeigen**: Dies muss ausgewählt sein, um die von Workfront erstellten Berichte anzuzeigen.
   * **Freigeben**
   * **Berichte öffentlich freigeben**: Berichte können öffentlich freigegeben werden, indem ein öffentlicher Link zum Bericht für alle freigegeben wird, die kein Workfront-Konto haben. Diese Option muss ausgewählt werden, um diese Freigabeebene zu ermöglichen.
   * **Systemweit freigeben** Berichte können für alle Personen im System freigegeben werden, die über eine Workfront-Lizenz verfügen. Diese Option muss ausgewählt werden, um diese Freigabeebene zu ermöglichen.

     Informationen zum Freigeben von Berichten, Dashboards und Kalendern finden Sie unter [Freigeben von Berichten, Dashboards und Kalendern](../../../workfront-basics/grant-and-request-access-to-objects/permissions-reports-dashboards-calendars.md).

1. (Optional) Um Zugriffseinstellungen für andere Objekte und Bereiche in der Zugriffsebene, an der Sie arbeiten, zu konfigurieren, fahren Sie mit einem der in [Zugriff auf Adobe Workfront konfigurieren](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md) aufgelisteten Artikel fort, z. B. [Zugriff auf Aufgaben gewähren](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md) und [Zugriff auf Finanzdaten gewähren](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
1. Wenn Sie fertig sind, klicken Sie auf **Speichern**.

   Nachdem die Zugriffsebene erstellt wurde, können Sie sie einem Benutzer zuweisen. Weitere Informationen finden Sie [Bearbeiten des Benutzerprofils](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## Zugriff auf Berichte, Dashboards und Kalender nach Lizenztyp

Informationen dazu, was Benutzer in den einzelnen Zugriffsebenen mit Problemen tun können, finden Sie im Abschnitt [Berichte](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#reports) im Artikel [Für jeden Objekttyp verfügbare Funktionen](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).

## Zugriff auf freigegebene Berichte, Dashboards und Kalender

Als Verantwortlicher oder Ersteller eines Berichts, Dashboards oder Kalenders können Sie ihn für andere Benutzer freigeben, indem Sie ihnen die entsprechenden Berechtigungen erteilen, wie unter [Freigeben von Berichten, Dashboards und Kalendern](../../../workfront-basics/grant-and-request-access-to-objects/permissions-reports-dashboards-calendars.md) beschrieben.

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>If you make changes here, make them also in the "Grant access to" articles where this snippet had to be converted to text:</p>
<p>* reports, dashboards, and calendars</p>
<p>* financial data</p>
<p>* issue</p>
</div>
-->

Wenn Sie ein Objekt für einen anderen Benutzer freigeben, werden die Rechte des Empfängers durch eine Kombination zweier Dinge bestimmt:

* Die Berechtigungen, die Sie Ihrem Empfänger für das Objekt erteilen
* Die Zugriffsebenen-Einstellungen des Empfängers für den Objekttyp
