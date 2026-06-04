---
title: Gewähren von administrativem Zugriff für Benutzer auf bestimmte Bereiche
description: Als Adobe Workfront-Administrator können Sie eine Zugriffsebene verwenden, um Benutzenden mit einer Plan-Lizenz administrativen Zugriff auf bestimmte Bereiche des Systems zu gewähren.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 9d12895d-cf7f-41c6-a2ac-bb731770c187
TQID: https://experienceleague.adobe.com/1nXA0NxLQW3tiIrhCKAd5EMfqBjQW68GHNN42dQmptQ
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: ce22a157-dd2c-405f-b740-c2f204bb4c1aid: d87de1f9-8e24-4c4d-aa4c-a403075091a1
role_v2: id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2: id: bce87dde-a4ab-44c9-8a18-ad66e4ddb377id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 686
ht-degree: 11%

---

# Gewähren von administrativem Zugriff für Benutzer auf bestimmte Bereiche

<!--Linked in several places, do not rename or change URL.-->

Als Adobe Workfront-Administrator können Sie eine Zugriffsebene verwenden, um Benutzenden mit einer Standard- oder Plan-Lizenz administrativen Zugriff auf bestimmte Bereiche des Systems zu gewähren.

>[!NOTE]
>
>Dies unterscheidet sich davon, einem Benutzer vollen administrativen Zugriff auf Workfront zu gewähren, wie unter [Gewähren des vollständigen administrativen Zugriffs](../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md) erläutert&#x200B;

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

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
   <td>   <p>Standard</p>
   <p>Abo</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Sie müssen ein Workfront-Administrator sein.</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Details zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Gewähren von administrativem Zugriff für Standard- oder Planbenutzer auf bestimmte Bereiche von Workfront

>[!IMPORTANT]
>
>Es wird dringend empfohlen, die integrierten Zugriffsebenen unverändert zu lassen, damit Sie sich nach der Einrichtung Ihrer Benutzenden darauf beziehen können. Um eine Zugriffsebene anzupassen, kopieren Sie die standardmäßige Zugriffsebene und ändern Sie die Kopie. (Dies ist für jede Zugriffsebene möglich, mit Ausnahme von Systemadministrator und externem Benutzer.)

{{step-1-to-setup}}

1. Klicken Sie im linken Bedienfeld auf **Zugriffsebenen**.
1. Klicken Sie auf den Namen der Zugriffsebene, die Sie verwenden möchten, um Benutzern administrativen Zugriff auf bestimmte Bereiche von Workfront zu gewähren.
1. Aktivieren **im Abschnitt Administratorzugriff zulassen für** Kontrollkästchen, um den erforderlichen Administratorzugriff zu gewähren.

   Mit diesen Optionen können Sie die folgenden Funktionen gewähren:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Genehmigungsprozesse</td> 
      <td><p>Genehmigungsprozesse zur Verwendung im gesamten System und für bestimmte Gruppen erstellen und verwalten</p><p>Ohne diesen Zugriff können Benutzende nur Ad-hoc-Genehmigungsprozesse für Elemente erstellen, auf die sie Zugriff haben und die sie verwalten können.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Firmen</td> 
      <td><p>Hinzufügen neuer und Bearbeiten bestehender Unternehmen in Workfront</p>
      <p>Ohne diesen Zugriff können Benutzer nur vorhandene Unternehmen anzeigen.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Benutzerdefinierte Formulare</td> 
      <td><p>Erstellen und Bearbeiten (Hinzufügen, Bearbeiten und Löschen der Felder) von benutzerdefinierten Formularen innerhalb ihrer Gruppe.</p><p>Ohne diesen Zugriff können Benutzende nur vorhandene Formulare an Objekte anhängen, zu denen sie beitragen oder die sie verwalten können.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Wechselkurse</td> 
      <td> <p>Neue Währung in Workfront hinzufügen.</p> <p>Ohne diesen Zugriff kann der Benutzer nur eine vorhandene Währung zu einem von ihm erstellten Projekt hinzufügen.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ausgaben</td> 
      <td><p>Alle Ausgaben für Objekte in Workfront anzeigen.</p><p>Dadurch kann der Benutzer keine neuen Ausgabentypen erstellen.</p><p>Ohne diesen Zugriff kann der Benutzer nur Folgendes anzeigen:</p>
       <ul>
        <li>Ausgaben für von ihnen verwaltete Projekte, Aufgaben oder Probleme</li>
        <li>Ihre eigenen Kosten</li>
        <li>Die Ausgaben ihrer Untergebenen</li>
       </ul></td> 
     </tr>
     <tr> 
      <td role="rowheader">Meilensteine in meiner Gruppe</td> 
      <td>Zeigen Sie alle Meilensteinpfade im System unter dem Menü Meilensteinpfade im Setup an. Benutzer können auch alle Meilensteinpfade bearbeiten oder löschen, die zu einer ihrer Gruppen gehören. Benutzende können die Meilensteinpfade, die keiner ihrer Gruppen zugewiesen sind, nicht verwalten (bearbeiten oder löschen).<br><p>Ohne diesen Zugriff können Benutzende nur vorhandene Meilensteinpfade anzeigen und auf Projekte anwenden, auf die sie Zugriff haben.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Erinnerungsbenachrichtigungen</td> 
      <td>Erstellen und Verwalten von Erinnerungsnachrichten in Workfront<br>Ohne diesen Zugriff können Benutzende nur Benachrichtigungen empfangen und anzeigen.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Arbeitszeittabellen und Stunden</td> 
      <td> <p>Ermöglicht Benutzenden, alle Stunden und Arbeitszeittabellen in Workfront anzuzeigen.</p> <p>Wenn diese Option deaktiviert ist, können Benutzende nur Stunden anzeigen für:</p> 
       <ul> 
        <li>Von ihnen verwaltete Projekte, Aufgaben oder Probleme</li> 
        <li>Ihre eigene Arbeitszeittabelle</li> 
        <li>Arbeitszeittabelle einer Person, die ihnen unterstellt ist</li> 
        <li>Eine von ihnen genehmigte Arbeitszeittabelle</li> 
       </ul> <p><b>HINWEIS</b>:  <p>Unabhängig davon, ob diese Option aktiviert oder deaktiviert ist, können Gruppenadministratoren Arbeitszeittabellen-Profile für die von ihnen verwalteten Gruppen und Untergruppen erstellen und sie Gruppenmitgliedern zuweisen, deren Benutzerprofile bearbeitet werden können.</p> <p>Durch Aktivierung dieser Option erhalten einige Gruppenadministratoren möglicherweise zu viel Zugriff, da sie die von den Arbeitszeittabellen-Profilen erstellten Arbeitszeittabellen (und die Stunden) für alle Benutzer im System anzeigen können, nicht nur für die Benutzer in den von ihnen verwalteten Gruppen. Sie können diese Option für Gruppenadministratoren deaktivieren, die nicht so viel Zugriff benötigen.</p> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Wenn Sie fertig sind, klicken Sie auf **Speichern**.
1. Weisen Sie einem Benutzer die neue Zugriffsebene zu, wie in [Benutzer hinzufügen](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md) beschrieben.

   >[!NOTE]
   >
   >Sie können Benutzern administrativen Zugriff auf Benutzer gewähren. Weitere Informationen dazu, wie Sie Benutzern administrativen Zugriff gewähren, damit sie Benutzerkonten verwalten können, finden Sie unter [Gewähren des Zugriffs für Benutzer](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).


<!--     
     <tr> 
      <td role="rowheader">Job roles</td> 
      <td> <p><b>NOTE</b>: In the Preview environment, access to job roles is controlled as an object type in the access level. See <a href="/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-access-job-roles.md">Grant access to job roles</a>.</p>
      <p>With this access, the user is allowed to do the following:</p> 
       <ul> 
        <li>View and edit existing job roles</li> 
        <li>Add new job roles</li> 
        <li>Edit role billing and cost rates</li> 
       </ul> <p><b>IMPORTANT</b>: If you grant a Standard or Plan user administrative access to job roles, the Financial Data access setting Edit Role Billing &amp; Cost Rates is enabled for the user automatically. Later, if you disable administrative access to job roles for the Standard or Plan user, job roles are still visible to the user because the Edit Role Billing &amp; Cost Rates setting is still enabled. If this happens and you need to remove the user's access to view job roles, you need to disable the user's Edit Role Billing &amp; Cost Rates permission setting. For instructions, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md" class="MCXref xref">Grant access to financial data</a>.</p> </td> 
     </tr>
-->
