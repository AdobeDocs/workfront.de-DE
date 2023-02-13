---
title: Benutzern administrativen Zugriff auf bestimmte Bereiche gewähren
description: Als Adobe Workfront-Administrator können Sie eine Zugriffsstufe verwenden, um Benutzern mit einer Planungslizenz Administratorzugriff auf bestimmte Systembereiche zu gewähren.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 9d12895d-cf7f-41c6-a2ac-bb731770c187
source-git-commit: 253a116e04e0b3a729331f5d0a29405e82808390
workflow-type: tm+mt
source-wordcount: '846'
ht-degree: 2%

---

# Benutzern administrativen Zugriff auf bestimmte Bereiche gewähren

<!--Linked in several places, do not rename or change URL.-->

Als Adobe Workfront-Administrator können Sie eine Zugriffsstufe verwenden, um Benutzern mit einer Planungslizenz Administratorzugriff auf bestimmte Systembereiche zu gewähren.

>[!NOTE]
>
>Dies unterscheidet sich von der Ermöglichung des uneingeschränkten Administratorzugriffs für einen Benutzer auf Workfront, wie hier beschrieben: [Gewähren eines vollen Administratorzugriffs](../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md)&#x200B;

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
   <td> <p>Sie müssen Workfront-Administrator sein.</p> <p><b>NOTE</b>: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Gewähren Sie Benutzern von der Planung Administratorzugriff auf bestimmte Bereiche von Workfront

>[!IMPORTANT]
>
>Wir empfehlen dringend, die integrierten Zugriffsebenen unverändert zu lassen, damit Sie nach der Einrichtung Ihrer Benutzer darauf verweisen können. Um eine Zugriffsebene anzupassen, kopieren Sie die standardmäßige Zugriffsebene und ändern Sie die Kopie. (Sie können dies für jede Zugriffsstufe mit Ausnahme von &quot;Systemadministrator&quot;und &quot;Externer Benutzer&quot;tun.)

1. Klicken Sie auf **Hauptmenü** icon ![](assets/main-menu-icon.png) Klicken Sie oben rechts in Adobe Workfront auf **Einrichtung** ![](assets/gear-icon-settings.png).

1. Klicken Sie im linken Bereich auf **Zugriffsebenen**.
1. Klicken Sie auf den Namen der Zugriffsstufe, die Sie verwenden möchten, um Benutzern Administratorzugriff auf bestimmte Bereiche von Workfront zu gewähren.
1. Im **Administratorzugriff zulassen für** aktivieren, um den erforderlichen Administratorzugriff zu gewähren.

   Mit diesen Optionen können Sie die folgenden Funktionen erteilen:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Genehmigungsprozesse</td> 
      <td><p>Erstellen und verwalten Sie Validierungsprozesse für die Verwendung im gesamten System und für bestimmte Gruppen.</p><p>Ohne diesen Zugriff können Benutzer nur Ad-hoc-Genehmigungsprozesse für Elemente erstellen, auf die sie Zugriff haben.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Firmen</td> 
      <td><p>Hinzufügen neuer und Bearbeiten vorhandener Unternehmen in Workfront</p>
      <p>Ohne diesen Zugriff können Benutzer nur bestehende Unternehmen anzeigen.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Benutzerdefinierte Formulare</td> 
      <td><p>Erstellen und bearbeiten (fügen Sie die Felder hinzu, bearbeiten und löschen Sie sie) benutzerdefinierte Formulare innerhalb ihrer Gruppe.</p><p>Ohne diesen Zugriff können Benutzer nur vorhandene Formulare an Objekte anhängen, zu denen sie Zugriff haben, um sie beizutragen oder zu verwalten.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Wechselkurse</td> 
      <td> <p>Neue Währung in Workfront hinzufügen.</p> <p>Ohne diesen Zugriff kann der Benutzer einem von ihm erstellten Projekt nur eine vorhandene Währung hinzufügen.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ausgaben</td> 
      <td><p>Zeigen Sie alle Ausgaben für Objekte in Workfront an.</p><p>Dadurch kann der Benutzer keine neuen Ausgabentypen erstellen.</p><p>Ohne diesen Zugriff kann der Benutzer nur Folgendes anzeigen:</p>
       <ul>
        <li>Ausgaben für von ihnen verwaltete Projekte, Aufgaben oder Probleme</li>
        <li>Ihre eigenen Ausgaben</li>
        <li>Die Kosten für ihre Untergebenen</li>
       </ul></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Aufgabengebiete</td> 
      <td> <p>Mit diesem Zugriff kann der Benutzer Folgendes tun:</p> 
       <ul> 
        <li>Vorhandene Auftrags-Rollen anzeigen und bearbeiten</li> 
        <li>Hinzufügen neuer Vorgangsrollen</li> 
        <li>Bearbeiten der Rollenabrechnung und der Kostensätze</li> 
       </ul> <p><b>WICHTIG</b>: Wenn Sie einem Planer Benutzer administrativen Zugriff auf Stellenrollen gewähren, wird die Einstellung Zugriff auf Finanzdaten bearbeiten Rollenabrechnung und Kostensätze automatisch für den Benutzer aktiviert. Wenn Sie später den administrativen Zugriff auf Stellenrollen für den Planer-Benutzer deaktivieren, sind die Auftragsrollen für den Benutzer weiterhin sichtbar, da die Einstellung Rollenabrechnung und -kosten bearbeiten weiterhin aktiviert ist. Wenn dies eintritt und Sie den Zugriff des Benutzers entfernen müssen, um Vorgangsrollen anzuzeigen, müssen Sie die Berechtigungseinstellung "Rollenabrechnung und -kosten bearbeiten"des Benutzers deaktivieren. Anweisungen finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md" class="MCXref xref">Zugriff auf Finanzdaten gewähren</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Meilensteine in meiner Gruppe</td> 
      <td>Zeigen Sie alle Meilensteinpfade im System unter dem Menü Meilensteinpfade im Setup an. Benutzer können auch alle Meilensteinpfade bearbeiten oder löschen, die zu einer ihrer Gruppen gehören. Benutzer können die Meilensteinpfade, die keiner ihrer Gruppen zugewiesen sind, nicht verwalten (bearbeiten oder löschen).<br><p>Ohne diesen Zugriff können Benutzer nur vorhandene Meilensteinpfade anzeigen und auf Projekte anwenden, auf die sie Zugriff haben.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Erinnerungsbenachrichtigungen</td> 
      <td>Erstellen und verwalten Sie Erinnerungsbenachrichtigungen in Workfront.<br>Ohne diesen Zugriff können Benutzer nur Benachrichtigungen empfangen und anzeigen.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Arbeitszeittabellen und Stunden</td> 
      <td> <p>Ermöglicht Benutzern die Anzeige aller Stunden und Timesheets in Workfront.</p> <p>Wenn diese Option deaktiviert ist, können Benutzer nur Stunden anzeigen für:</p> 
       <ul> 
        <li>Von ihnen verwaltete Projekte, Aufgaben oder Probleme</li> 
        <li>Ihre eigenen Zeitpläne</li> 
        <li>Ein Timesheet für einen Benutzer, der ihm Berichte übermittelt</li> 
        <li>Ein von ihnen genehmigtes Zeitblatt</li> 
       </ul> <p><b>NOTIZ</b>:  <p>Unabhängig davon, ob diese Option aktiviert oder deaktiviert ist, können Gruppenadministratoren für die von ihnen verwalteten Gruppen und Untergruppen Zeitplanprofile erstellen und sie Gruppenmitgliedern zuweisen, deren Benutzerprofile sie bearbeiten können.</p> <p>Die Aktivierung dieser Option bietet einigen Gruppenadministratoren möglicherweise zu viel Zugriff, da sie die von Timesheet-Profilen erzeugten Timesheets (und die Stunden) für alle Benutzer im System anzeigen können, nicht nur für die Benutzer in den von ihnen verwalteten Gruppen. Sie können diese Option für Gruppenadministratoren deaktivieren, die nicht so viel Zugriff benötigen.</p> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Wenn Sie fertig sind, klicken Sie auf **Speichern**.
1. Weisen Sie die neue Zugriffsebene einem Benutzer zu, wie unter [Benutzer hinzufügen](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

   >[!NOTE]
   >
   >Sie können Benutzern Administratorzugriff gewähren. Weitere Informationen dazu, wie Sie Benutzern Administratorzugriff gewähren, damit sie Benutzerkonten verwalten können, finden Sie unter [Benutzern Zugriff gewähren](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).
