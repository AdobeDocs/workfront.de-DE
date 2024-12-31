---
title: Gewähren von administrativem Zugriff für Benutzer auf bestimmte Bereiche
description: Als Adobe Workfront-Administrator können Sie eine Zugriffsebene verwenden, um Benutzenden mit einer Plan-Lizenz administrativen Zugriff auf bestimmte Bereiche des Systems zu gewähren.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 9d12895d-cf7f-41c6-a2ac-bb731770c187
source-git-commit: c887569d59c7751210671cab97c492ee1752fffc
workflow-type: tm+mt
source-wordcount: '843'
ht-degree: 2%

---

# Gewähren von administrativem Zugriff für Benutzer auf bestimmte Bereiche

<!--Linked in several places, do not rename or change URL.-->

Als Adobe Workfront-Administrator können Sie eine Zugriffsebene verwenden, um Benutzenden mit einer Plan-Lizenz administrativen Zugriff auf bestimmte Bereiche des Systems zu gewähren.

>[!NOTE]
>
>Dies unterscheidet sich davon, einem Benutzer vollen administrativen Zugriff auf Workfront zu gewähren, wie unter [Gewähren des vollständigen administrativen Zugriffs](../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md) erläutert&#x200B;

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
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Sie müssen ein Workfront-Administrator sein.</p> <p><b>HINWEIS</b>: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Einschränkungen in Ihrer Zugriffsebene festgelegt hat. Informationen dazu, wie Workfront-Admins Ihre Zugriffsebene ändern können, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">Erstellen oder Ändern benutzerdefinierter Zugriffsebenen</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## Planbenutzern administrativen Zugriff auf bestimmte Bereiche von Workfront gewähren

>[!IMPORTANT]
>
>Es wird dringend empfohlen, die integrierten Zugriffsebenen unverändert zu lassen, damit Sie nach der Einrichtung Ihrer Benutzer darauf verweisen können. Um eine Zugriffsebene anzupassen, kopieren Sie die standardmäßige Zugriffsebene und ändern Sie die Kopie. (Dies ist für jede Zugriffsebene möglich, mit Ausnahme von Systemadministrator und externem Benutzer.)

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
      <td role="rowheader">Aufgabengebiete</td> 
      <td> <p>Mit diesem Zugriff kann der Benutzer Folgendes tun:</p> 
       <ul> 
        <li>Anzeigen und Bearbeiten vorhandener Aufgabengebiete</li> 
        <li>Neue Aufgabengebiete hinzufügen</li> 
        <li>Funktionsbezogene Abrechnung und Kostensätze bearbeiten</li> 
       </ul> <p><b>WICHTIG</b>: Wenn Sie einem Planer-Benutzer administrativen Zugriff auf Aufgabengebiete gewähren, wird die Einstellung „Finanzdatenzugriff“ „Aufgabengebiet bearbeiten - Abrechnung und Kostensätze“ für den Benutzer automatisch aktiviert. Wenn Sie später den administrativen Zugriff auf Aufgabengebiete für den Planenden-Benutzer deaktivieren, sind für den Benutzer weiterhin Aufgabengebiete sichtbar, da die Einstellung „Aufgabengebiet bearbeiten - Abrechnung und Kostensätze“ weiterhin aktiviert ist. Wenn dies eintritt und Sie den Zugriff des Benutzers auf die Anzeige von Aufgabengebieten entfernen müssen, müssen Sie die Berechtigungseinstellung „Rolle bearbeiten - Abrechnung und Kostensätze“ des Benutzers deaktivieren. Anweisungen finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md" class="MCXref xref">Zugriff auf Finanzdaten gewähren</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Meilensteine in meiner Gruppe</td> 
      <td>Zeigen Sie alle Meilensteinpfade im System unter dem Menü Meilensteinpfade im Setup an. Benutzer können auch alle Meilensteinpfade bearbeiten oder löschen, die zu einer ihrer Gruppen gehören. Benutzende können die Meilensteinpfade, die keiner ihrer Gruppen zugewiesen sind, nicht verwalten (bearbeiten oder löschen).<br><p>Ohne diesen Zugriff können Benutzende nur vorhandene Meilensteinpfade anzeigen und auf Projekte anwenden, auf die sie Zugriff haben.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Erinnerungsbenachrichtigungen</td> 
      <td>Erstellen und Verwalten von Erinnerungsnachrichten in Workfront.<br>Ohne diesen Zugriff sind die Benutzenden darauf beschränkt, Benachrichtigungen zu empfangen und anzuzeigen.</td> 
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
