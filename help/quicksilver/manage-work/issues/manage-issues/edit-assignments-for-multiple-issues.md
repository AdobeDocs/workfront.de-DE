---
product-area: projects
navigation-topic: manage-issues
title: Ändern von Benutzerzuweisungen für mehrere Probleme in einer Liste
description: Ändern von Benutzerzuweisungen für mehrere Probleme in einer Liste
author: Alina
feature: Work Management
exl-id: e1e75027-1847-44cf-afeb-b19394dc3ea5
source-git-commit: daba001c28df268721c87df7d2516ffb76e535d9
workflow-type: tm+mt
source-wordcount: '773'
ht-degree: 1%

---

# Ändern von Benutzerzuweisungen für mehrere Probleme in einer Liste

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: similar article exists for tasks)</p>
-->

Sie können Benutzerzuweisungen gleichzeitig für mehrere Probleme ändern. Weitere Informationen zum Bearbeiten oder Zuweisen von Problemen finden Sie in den folgenden Artikeln:

* [Probleme bearbeiten](../../../manage-work/issues/manage-issues/edit-issues.md)
* [Zuweisen von Problemen](../../../manage-work/issues/manage-issues/assign-issues.md)

Allgemeine Informationen zum Zuweisen von Problemen finden Sie unter [Überblick über das Ändern von Problemzuweisungen](../../../manage-work/issues/manage-issues/modify-issue-assignments-overview.md).

>[!NOTE]
>
>Sie müssen mindestens über Contribute-Berechtigungen für ein Problem verfügen, um dem Problem Zuweisungen zuweisen zu können.

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Alle </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenzen*</td> 
   <td> <p>Anforderung oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf Probleme bearbeiten</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Berechtigungen für das Problem verwalten</p> <p>Weitere Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Anfordern des Zugriffs auf Objekte </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>When to modify user assignments on issues</h2>
<p>(NOTE:&nbsp;drafted and moved to the overview article: Modify issue assignments overview)</p>
<p>You might want to modify the user assignments for multiple issues for a variety of&nbsp;reasons, including the following:</p>
<ul>
<li>Users join or leave&nbsp;your team</li>
<li>A user takes a vacation that extends beyond the issue&nbsp;due dates</li>
<li>A specific role or user is set as the assignee for multiple issues and you want to quickly modify all items to be assigned to a different user or role</li>
</ul>
</div>
-->

## Ändern von Zuweisungen für mehrere Probleme

1. Gehen Sie zur Problemliste, die die Probleme enthält, deren Zuweisungen Sie ändern möchten.
1. (Optional) Erstellen Sie einen Filter, um nur die dem Empfänger zugewiesenen Probleme anzuzeigen, den Sie ändern möchten.

   Sie können beispielsweise einen Filter erstellen, um nur Probleme mit einer bestimmten Rolle als Verantwortlicher anzuzeigen. Anschließend können Sie die Rolle durch einen bestimmten Benutzer ersetzen. Gehen Sie wie folgt vor:

   1. Klicken Sie auf die Dropdownliste **Filter** und dann auf **Neuer Filter**.

      Das Dialogfeld Neuer Filter wird angezeigt.

   1. Klicken Sie auf **Filterregel hinzufügen**.
   1. Um nach einer bestimmten Rolle zu filtern, erweitern Sie **Zuweisungsrollen** und klicken Sie dann auf **ID**.

      Oder

      Um nach einem bestimmten Benutzer zu filtern, erweitern Sie **Zuweisungsbenutzer** und klicken Sie dann auf **ID**.

      >[!TIP]
      >
      >Verwenden Sie nicht &quot;**Zugeordnet zu**&quot;, da dieses Feld nur auf den Eigentümer des Problems und nicht auf alle Verantwortlichen verweist.

   1. Wählen Sie in der Dropdownliste **Gleich** als Filterqualifikator aus.
   1. Beginnen Sie mit der Eingabe des Namens des Benutzers oder der Rolle, nach dem/der Sie filtern möchten, und klicken Sie dann auf den Namen, wenn er/sie in der Dropdown-Liste angezeigt wird.
   1. Klicken Sie auf **Filter speichern.**

1. Wählen Sie die Probleme aus, für die Sie Zuweisungen ändern möchten, und klicken Sie dann auf das Symbol **Bearbeiten** ![](assets/qs-edit-icon.png).

   Der Eintrag **Probleme bearbeiten** wird angezeigt. Die bearbeiteten Elemente werden in der oberen linken Ecke der Seite angezeigt.

1. Wechseln Sie zum Abschnitt **Zuweisungen** und wählen Sie dann **Bevollmächtigter** aus.

   ![](assets/classic-assignmens-area-on-edit-box-350x119.png)

1. Führen Sie einen der folgenden Schritte aus:

   1. So fügen Sie einen neuen Bevollmächtigten hinzu:

      1. Geben Sie den Namen eines Benutzers, einer Rolle oder eines Teams ein und wählen Sie ihn aus, wenn er in der Liste angezeigt wird. Die Zuweisung wird hinzugefügt und ersetzt nicht die aktuellen Zuweisungen zu den ausgewählten Problemen.

         >[!TIP]
         >
         >Sie können mehrere Benutzer, Auftragsrollen oder Teams zuweisen. Sie können nur aktive Benutzer, Stellenrollen und Teams zuweisen.
         >
         >Wenn ein Benutzer, eine Rolle oder ein Team zugewiesen wurde, bevor sie deaktiviert wurden, bleiben sie dem Arbeitselement zugewiesen. In diesem Fall empfehlen wir Folgendes:
         >
         >* Weisen Sie das Arbeitselement aktiven Ressourcen erneut zu.
         >* Verknüpfen Sie die Benutzer in einem deaktivierten Team mit einem aktiven Team und weisen Sie das Arbeitselement dem aktiven Team erneut zu.

         Informationen, die in allen ausgewählten Problemen gängig sind, werden angezeigt. Wenn beispielsweise derselbe Benutzer allen Problemen zugewiesen ist, wird dieser Benutzer in der Spalte **Zuweisung** angezeigt. Wenn Informationen nicht in allen ausgewählten Problemen gängig sind, werden keine Informationen angezeigt.

   1. So entfernen Sie einzelne Bevollmächtigte:

      1. Klicken Sie auf das Symbol **X** neben dem Namen des Empfängers, den Sie entfernen möchten, wenn der Verantwortliche in der Liste Zuweisungen angezeigt wird.

         Oder

         (Bedingt) Wenn der zu entfernende Bevollmächtigte nicht im Abschnitt &quot;Zuweisungen&quot;angezeigt wird, da der Bevollmächtigte nur bestimmten von Ihnen ausgewählten Problemen zugewiesen ist, klicken Sie auf **Bevollmächtigten entfernen** und geben Sie den Namen des Bevollmächtigten ein, den Sie entfernen möchten, und klicken Sie dann auf den Namen, wenn er in der Dropdownliste angezeigt wird.

      1. Klicken Sie erneut auf **Bevollmächtigten entfernen** , um einen weiteren zu entfernenden Bevollmächtigten hinzuzufügen.

   1. So entfernen Sie alle vorhandenen Bevollmächtigten:

      1. Klicken Sie auf **Alle vorhandenen Zuweisungen entfernen** und dann auf **Ja, alle Zuweisungen löschen**.

         Dadurch werden nicht nur häufig verwendete Bevollmächtigte (Bevollmächtigte, die im Dialogfeld &quot;Bearbeiten&quot;angezeigt werden), sondern auch alle Bevollmächtigten für alle ausgewählten Probleme entfernt.

1. (Optional) Ändern Sie eine der folgenden Optionen für die von Ihnen ausgewählten Bevollmächtigten, die mit den Problemen verknüpft werden sollen:

   * **Eigentümer des Problems:** Wählen Sie das Optionsfeld aus, um anzugeben, welcher Verantwortliche als Eigentümer der Probleme benannt ist. Wenn diese Option nicht ausgewählt ist, bestimmt Adobe Workfront den ersten Verantwortlichen als Eigentümer des Problems. Dies ist nicht für Teamzuweisungen verfügbar.
   * **Rolle des Bevollmächtigten**: Wählen Sie eine Rolle aus der Dropdownliste aus. Wenn die Option nicht ausgewählt ist, wählt Workfront automatisch die Primäre Rolle des Benutzers aus.

1. Klicken Sie auf **Änderungen speichern**.
