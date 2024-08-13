---
title: Gewähren von Zugriff auf Teams
description: Als Adobe Workfront-Administrator können Sie mithilfe einer Zugriffsebene den Zugriff eines Benutzers auf Teams in Workfront definieren
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 915d1520-f5c4-4e33-b645-cb219289383c
source-git-commit: c887569d59c7751210671cab97c492ee1752fffc
workflow-type: tm+mt
source-wordcount: '696'
ht-degree: 4%

---

# Gewähren von Zugriff auf Teams

Als Adobe Workfront-Administrator können Sie mithilfe einer Zugriffsebene den Zugriff eines Benutzers auf Teams in Workfront definieren, wie unter [Übersicht über Zugriffsebenen](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md) beschrieben.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

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
   <td> <p>Sie müssen Workfront-Administrator sein.</p> <p><b>HINWEIS</b>: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## Benutzerzugriff konfigurieren, um Benutzer mithilfe einer benutzerdefinierten Zugriffsebene zu bearbeiten

1. Beginnen Sie mit der Erstellung oder Bearbeitung der Zugriffsebene, wie unter [Benutzerdefinierte Zugriffsebenen erstellen oder ändern](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md) beschrieben.
1. Klicken Sie auf das Zahnradsymbol ![](assets/gear-icon-settings.png) auf der Schaltfläche **Ansicht** oder **Bearbeiten** rechts neben Teams und wählen Sie dann die Fähigkeiten aus, die Sie unter **Feinabstimmung Ihrer Einstellungen** gewähren möchten.

   * **Ansicht**: Wenn Sie konfigurieren, wie Benutzer mit einer Lizenz Teams anzeigen können, ändern Sie eine der folgenden Optionen:

     <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">Meinen Gruppen zugeordnete Teams anzeigen</td>
         <td>
          <p><b>Aktiviert</b>: Wenn Benutzer nach Teams in einem Feld mit Team-Typvorgabe suchen, können die Benutzer die mit ihren Gruppen verknüpften Teams sehen, unabhängig davon, ob es sich um Teammitglieder handelt oder nicht. </p>
          <p><b>Deaktiviert</b>: Wenn Benutzer nach Teams in einem Feld mit Team-Typvorgabe suchen, können die Benutzer die mit ihren Gruppen verknüpften Teams nur dort sehen, wo sie Teammitglieder sind.</p><p>Diese Option ist standardmäßig aktiviert.</p>
          </td>
        </tr>
        <tr>
         <td role="rowheader">Alle Teams anzeigen</td>
         <td><p>Wenn diese Option aktiviert ist und Benutzer in einem Feld für die Team-Typvorbereitung nach Teams suchen, können die Benutzer ein beliebiges Team sehen und auswählen.</p><p>Diese Option ist standardmäßig aktiviert. </p></td>
        </tr>
       </tbody>
      </table>

   * **Bearbeiten**: Wenn Sie konfigurieren, wie Benutzer mit einer Plan-Lizenz und einer Work-Lizenz Teams verwalten können, ändern Sie eine der folgenden Optionen:

     <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">Erstellen</td>
         <td><p>Ermöglicht Benutzern mit einer Planlizenz oder Work-Lizenz, Teams zu erstellen.</p><p>Diese Option ist standardmäßig aktiviert.</p></td>
        </tr>
        <tr>
         <td role="rowheader">Löschen</td>
         <td><p> Ermöglicht Benutzern mit einer Planungslizenz, die Teams zu löschen, auf die sie Zugriff haben (für Benutzer mit einer Work-Lizenz nicht verfügbar).</p><p>Diese Option ist standardmäßig aktiviert.</p></td>
        </tr>
        <tr>
         <td role="rowheader">Teams in von mir verwalteten Gruppen bearbeiten (nur Gruppenadmins)</td>
         <td><p>Ermöglicht die Planung von Lizenzbenutzern, die als Gruppenadministratoren benannt sind, die Bearbeitung von Teams, die mit den von ihnen verwalteten Gruppen verbunden sind.</p><p>Diese Option ist standardmäßig aktiviert.</p></td>
        </tr>
        <tr>
         <td role="rowheader">Teams bearbeiten, in denen ich bin</td>
         <td><p>Ermöglicht Benutzern, eine Lizenz oder Arbeitslizenz zu planen, um Teams zu bearbeiten, in denen sie Mitglied sind.</p><p>Diese Option ist standardmäßig deaktiviert.</p></td>
        </tr>
        <tr>
         <td role="rowheader">Meinen Gruppen zugeordnete Teams anzeigen</td>
         <td>
         <p><b>Aktiviert</b> Wenn Benutzer nach Teams in einem Feld mit Team-Typvorgabe suchen, können die Benutzer die mit ihren Gruppen verknüpften Teams sehen, unabhängig davon, ob es sich um Teammitglieder handelt oder nicht. </p>
         <p><b>Deaktiviert</b>: Wenn Benutzer nach Teams in einem Feld mit Team-Typvorgabe suchen, können die Benutzer die mit ihren Gruppen verknüpften Teams nur dort sehen, wo sie Teammitglieder sind.</p><p>Diese Option ist standardmäßig aktiviert.</p>
         </td>
        </tr>
        <tr>
         <td role="rowheader">Alle Teams anzeigen</td>
         <td><p>Wenn diese Option aktiviert ist und Benutzer in einem Feld für die Team-Typvorbereitung nach Teams suchen, können die Benutzer ein beliebiges Team sehen und auswählen.</p><p>Diese Option ist standardmäßig aktiviert. </p></td>
        </tr>
       </tbody>
      </table>

1. Klicken Sie auf das X, um das Feld **Einstellungen optimieren** zu schließen.
1. (Optional) Um die Zugriffseinstellungen für andere Objekte und Bereiche in der Zugriffsebene zu konfigurieren, an der Sie arbeiten, fahren Sie mit einem der unter [Zugriff auf Adobe Workfront konfigurieren](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md) aufgelisteten Artikel fort, z. B. [Zugriff auf Aufgaben gewähren](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md) und [Zugriff auf Finanzdaten gewähren](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
1. Wenn Sie fertig sind, klicken Sie auf **Speichern**.

>[!NOTE]
>
>* Folgendes gilt unabhängig von den Einstellungen der Zugriffsstufe:
>
>   * Teambesitzer können ihre Teams jederzeit anzeigen und bearbeiten
>   * Benutzer haben immer Zugriff auf die Ansicht der Teams, in denen sie sich befinden
>
>* Die Konfiguration aller Optionen, die sowohl für die Ansicht als auch für die Bearbeitung verfügbar sind (z. B. &quot;Mit meinen Gruppen verknüpfte Teams anzeigen&quot;), wird beibehalten, wenn Sie anstelle der Option &quot;Bearbeiten&quot;oder &quot;Bearbeiten&quot;in einer Zugriffsebene die Option &quot;Ansicht&quot;auswählen.
>

## Zugriff auf Teams nach Lizenztyp

Informationen dazu, was Benutzer in den einzelnen Zugriffsebenen mit Problemen tun können, finden Sie im Abschnitt [Teams](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#teams) im Artikel [Für jeden Objekttyp verfügbare Funktionen](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).
