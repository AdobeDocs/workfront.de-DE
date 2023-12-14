---
title: Benutzern Zugriff gewähren
description: Als Adobe Workfront-Administrator können Sie eine Zugriffsstufe verwenden, um den Zugriff eines Benutzers auf andere Benutzer in Workfront zu definieren.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 5e87cad4-4a5d-4cb2-848f-7c97ff11d0e8
source-git-commit: 3c5bcb85080a882a8b69bffcd01563a0479f98a5
workflow-type: tm+mt
source-wordcount: '768'
ht-degree: 0%

---


# Benutzern Zugriff gewähren

Als Adobe Workfront-Administrator können Sie mithilfe einer Zugriffsebene den Zugriff eines Benutzers auf andere Benutzer in Workfront definieren, wie hier beschrieben: [Übersicht über Zugriffsebenen](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

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
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Sie müssen Workfront-Administrator sein.</p> <p><b>NOTE</b>: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsstufe festgelegt hat. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Benutzerzugriff konfigurieren

Sie können verwalten, welche Informationen Benutzer für andere Benutzer anzeigen und bearbeiten können, indem Sie eine standardmäßige Zugriffsebene oder eine benutzerdefinierte Zugriffsebene verwenden, die Sie erstellen. Benutzer mit den Standardlizenzen für Plan und Arbeit können die Kontaktinformationen anderer Benutzer anzeigen. Jeder der folgenden Benutzer kann andere Benutzer erstellen und bearbeiten:

* Ein Workfront-Administrator.

  Weitere Informationen finden Sie unter [Gewähren eines vollen Administratorzugriffs](../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md).

* Ein Benutzer mit einer standardmäßigen Planungslizenz, der auch Zugriff auf Benutzer hat, wie in diesem Artikel beschrieben.

  Benutzer, die nur Benutzern aus ihrem Unternehmen oder dem primären Unternehmen angezeigt werden, haben Zugriff darauf, nur die Benutzer zu bearbeiten, die sie sehen können. Weitere Informationen finden Sie unter [Benutzerdefinierte Zugriffsebenen erstellen oder ändern](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

* Ein Benutzer mit einer standardmäßigen Planungslizenz, der auch als Manager eines anderen Benutzers angegeben ist.

  Benutzer, denen auf ihrer Zugriffsebene die Option Zugriff auf Benutzer bearbeiten gewährt wird, können Benutzer verwalten, die ihnen Berichte zuweisen. Informationen zum Verwalten eines Benutzers finden Sie unter [Organigramm anzeigen](../../../people-teams-and-groups/work-directly-with-others/view-the-org-chart.md).

* Ein Benutzer mit einer standardmäßigen Planungslizenz, der einen Benutzer erstellt hat, kann den von ihm erstellten Benutzer deaktivieren, löschen oder bearbeiten. Weitere Informationen zum Erstellen neuer Benutzer finden Sie unter [Benutzer hinzufügen](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

## Benutzerzugriff konfigurieren, um Benutzer mithilfe einer benutzerdefinierten Zugriffsebene zu bearbeiten

1. Beginnen Sie mit der Erstellung oder Bearbeitung der Zugriffsebene, wie unter [Benutzerdefinierte Zugriffsebenen erstellen oder ändern](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
1. So ändern Sie die Fähigkeit von Benutzern mit einer Plan- oder Work-Lizenz, die Profile anderer Benutzer anzuzeigen:

   1. Klicken Sie auf das Zahnradsymbol ![](assets/gear-icon-settings.png) auf **Ansicht** Schaltfläche rechts von **Benutzer**.

   1. Deaktivieren **Kontaktangaben anzeigen** und klicken Sie dann auf das X , um die **Optimieren Ihrer Einstellungen** ankreuzen.

1. Um die Fähigkeit von Benutzern mit Zugriff auf eine Planungslizenz zu ändern, klicken Sie auf das Zahnradsymbol ![](assets/gear-icon-settings.png) auf **Bearbeiten** Schaltfläche rechts von **Benutzer** und wählen Sie dann die Fähigkeiten aus, die Sie gewähren möchten:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Erstellen</strong> </td> 
      <td> <p>Ermöglicht Benutzern das Erstellen von Benutzern.<br>Diese Option ist standardmäßig aktiviert.</p> 
      &lt;!—
        <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Stellen Sie sicher, dass diese Änderung vorgenommen wird, bevor Sie diese beiden Notizen entpacken. Am 29.3.29 erklärt das Req-Dokument, dass dies von den Untersuchungsergebnissen abhängt.</p>

       &lt;p>&lt;b>HINWEIS:&lt;/b> Dies ist nicht verfügbar, wenn Ihr Unternehmen in der Adobe Admin Console integriert wurde. Wenden Sie sich an Ihren Netzwerk- oder IT-Administrator, wenn Sie weitere Informationen benötigen.&lt;/p>
       —>  &lt;/td>
   </tr> 
     <tr> 
      <td role="rowheader"><strong>Löschen</strong> </td> 
      <td> <p> Ermöglicht Benutzern das Löschen der selbst erstellten Benutzer.<br>Diese Option ist standardmäßig aktiviert.</p> <p><b>NOTE</b>: Dies ist nicht verfügbar, wenn Ihr Unternehmen in der Adobe Admin Console integriert wurde. Wenden Sie sich an Ihren Netzwerk- oder IT-Administrator, wenn Sie weitere Informationen benötigen.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Benutzerverwaltung (alle Benutzer)</strong> </td> 
      <td> <p>Ermöglicht Benutzern Folgendes für beliebige Benutzer in Workfront:</p> 
       <ul> 
        <li>Benutzer bearbeiten, löschen oder deaktivieren</li> 
        <li>Als Benutzer anmelden</li> 
        <li>Kennwort des Benutzers zurücksetzen</li> 
       </ul> <p>Diese Option ist standardmäßig deaktiviert.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Benutzerverwaltung (Gruppenbenutzer)</strong> </td> 
      <td> <p>Ermöglicht Benutzern Folgendes für jeden Benutzer in einer Gruppe, die sie verwalten: 
        <ul>
         <li><p>Benutzer bearbeiten, löschen oder deaktivieren</p></li>
         <li>Als Benutzer anmelden</li>
         <li><p>Kennwort des Benutzers zurücksetzen</p><p><b>NOTE</b>: Ein Gruppenadministrator kann sich nicht als Workfront-Administrator anmelden oder das Kennwort zurücksetzen.</p></li>
        </ul><p>Diese Option ist standardmäßig deaktiviert.</p></p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >Wenn Sie Gruppenadministratoren keinen Zugriff auf alle Mitglieder der Gruppen gewähren möchten, die sie verwalten, deaktivieren Sie die beiden oben genannten Benutzeradministratoroptionen. Gruppenadministratoren können weiterhin auf Gruppenmitglieder zugreifen, die sie zu Workfront hinzufügen oder die ihnen in Workfront Bericht erstatten.

1. (Optional) Um die Zugriffseinstellungen für andere Objekte und Bereiche in der Zugriffsebene zu konfigurieren, mit einem der Artikel fortzufahren, die unter [Zugriff auf Adobe Workfront konfigurieren](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md), beispielsweise [Zugriff auf Aufgaben gewähren](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md) und [Zugriff auf Finanzdaten gewähren](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
1. Klicken Sie abschließend auf **Speichern**.

## Zugriff auf Benutzer nach Lizenztyp

Informationen dazu, was Benutzer in den einzelnen Zugriffsebenen mit Benutzern tun können, finden Sie im Abschnitt [Benutzer](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#users) im Artikel [Für jeden Objekttyp verfügbare Funktionen](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).
