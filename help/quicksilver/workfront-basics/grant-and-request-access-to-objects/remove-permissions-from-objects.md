---
product-area: user-management;portfolios
navigation-topic: grant-and-request-access-to-objects
title: Berechtigungen aus Objekten entfernen
description: Sie können Berechtigungen anderer Benutzer für Objekte entfernen, auf die Sie Zugriff auf die Freigabe haben. Das Entfernen von Berechtigungen aus Objekten ist für alle Objekte identisch, die freigegeben werden können.
author: Alina
feature: Get Started with Workfront
exl-id: 8e191b5e-31df-4291-8b9d-9ca69be27561
source-git-commit: 71d5e15c38b26b9a833ac2418d5782afd249a24c
workflow-type: tm+mt
source-wordcount: '1144'
ht-degree: 0%

---

# Berechtigungen aus Objekten entfernen

<!--Audited: 01/2024-->

Sie können Berechtigungen anderer Benutzer für Objekte entfernen, auf die Sie Zugriff auf die Freigabe haben. Das Entfernen von Berechtigungen aus Objekten ist für alle Objekte identisch, die freigegeben werden können.

Ähnliche Überlegungen wie beim Freigeben von Objekten gelten für das Entfernen von Berechtigungen aus Objekten. Weitere Informationen finden Sie im Abschnitt [Überlegungen zum Freigeben von Objekten](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md#consider) im Artikel [Überblick über die Freigabe von Berechtigungen für Objekte](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md)

## Zugriffsanforderungen

Sie müssen über Folgendes verfügen, um Objekte freizugeben:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Abo</td> 
   <td> <p>Alle </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Workfront-Lizenz*</td> 
   <td> <p>Neue Lizenz: Mitarbeiter oder höher</p>
   Oder  
   <p>Aktuelle Lizenz: Anfrage oder höher</p>
   <p><b>NOTIZ</b></p>

<p>Einige Objekte benötigen einen höheren Zugriff als die Anforderung. </p>

<p>Beispielsweise kann ein Mitarbeiter für die neue Lizenz Probleme freigeben, aber nur Benutzer mit Standardlizenz können ein Projekt freigeben.</p>

<p>Für die aktuelle Lizenz kann ein Anforderer Probleme freigeben, aber nur Arbeitnehmer oder Planer können ein Projekt freigeben.</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Zugriff auf die freizugebenden Objekte oder höher anzeigen</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Berechtigungen für die freizugebenden Objekte anzeigen oder höher</p> <p>Verwalten von Berechtigungen zum Entfernen von geerbten Berechtigungen für Objekte</p>  </td> 
  </tr> 
 </tbody> 
</table>

*Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben. Weitere Informationen finden Sie unter [Zugriffsanforderungen für die Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Entfernen von Entitäten aus der Freigabeliste eines Objekts {#remove-entities-from-the-sharing-list-of-an-object}

Sie können Entitäten (Benutzer, Stellenrollen, Teams, Gruppen, Unternehmen) aus der Freigabeliste eines Objekts entfernen. Dadurch werden ihre Berechtigungen für das Objekt entfernt.

1. Wechseln Sie zu dem Objekt, aus dem Sie Berechtigungen entfernen möchten.

   Informationen dazu, welche Objekte freigegeben werden können, finden Sie unter [Übersicht über die Freigabe von Berechtigungen für Objekte](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

1. (Bedingt) Gehen Sie für Programme, Portfolios und Dokumente wie folgt vor:

   1. Klicken Sie auf das Symbol **Mehr** ![](assets/more-icon.png) neben dem Objektnamen und dann auf **Freigabe** oder **Freigabe**.

      ![](assets/share-a-document-350x160.png)

   1. Klicken Sie auf das Symbol **x** neben dem Namen eines Benutzers, eines Teams, einer Gruppe, eines Unternehmens oder einer Auftragsrolle, um diese im Feld für den Objektzugriff zu entfernen.

      ![](assets/remove-permissions-on-portfolio.png)

   1. Wählen Sie im Dropdown-Menü &quot;**&lt; Benutzername >&quot;aus, ob der Workfront-Zugriff von dem ausgewählten Objekt oder von allen ihm zugeordneten untergeordneten Objekten entfernt werden soll.**

1. (Bedingt) Gehen Sie für Projekte, Aufgaben und Probleme wie folgt vor:

   1. Klicken Sie rechts neben dem Objektnamen auf **Freigeben** .

      ![](assets/new-share-button.png)
   1. Suchen Sie den Benutzer, die Rolle, das Team, die Gruppe oder das Unternehmen, den/das Sie aus dem Objekt entfernen möchten.
   1. Klicken Sie auf **Entfernen**.
Wählen Sie im Dropdownmenü **Entfernen &lt; Benutzername > aus** aus, ob ihr Zugriff nur aus dem ausgewählten Objekt oder aus allen ihm zugeordneten untergeordneten Objekten entfernt werden soll.

      ![](assets/remove-permissions-on-project-nwe-350x479.png)

   Die folgenden Szenarien existieren:

   * Wenn Sie die Entität nur aus dem Objekt entfernen, verliert diese Entität ihre Berechtigungen für das Objekt und ihre geerbten Berechtigungen für die untergeordneten Objekte. Wenn ihnen zuvor Berechtigungen für die untergeordneten Elemente einzeln gewährt wurden, behalten sie bei der Auswahl dieser Option dieselben Berechtigungen für alle untergeordneten Objekte bei, die mit ihnen verknüpft sind.
   * Wenn Sie die Entität aus dem Objekt und allen untergeordneten Objekten entfernen, verliert diese Entität ihre Berechtigungen für das Objekt sowie alle untergeordneten Objekte, selbst wenn ihnen zuvor individuelle Berechtigungen für jedes untergeordnete Objekt erteilt wurden.

1. Klicken Sie auf **Speichern**.

## Berechtigungen für mehrere Objekte stapelweise entfernen

Sie können Entitäten (Benutzer, Auftragsrollen, Teams, Gruppen, Unternehmen) gleichzeitig aus mehreren Objekten entfernen, wenn Sie sie in einer Liste stapelweise auswählen.

>[!NOTE]
>
>Sie können nicht anzeigen, welche Zugriffseinheiten für alle ausgewählten Objekte vorhanden sind, wenn Sie sie stapelweise auswählen. Sie müssen wissen, welche Entität Sie aus der Freigabe der ausgewählten Objekte entfernen möchten, bevor Sie deren Berechtigungen entfernen.

1. Navigieren Sie zur Liste der Objekte, die Sie freigeben möchten.

   Informationen dazu, welche Objekte freigegeben werden können, finden Sie unter [Übersicht über die Freigabe von Berechtigungen für Objekte](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

1. Wählen Sie mehrere Objekte in der Liste aus und klicken Sie dann oben in der Liste auf das Symbol **Freigabe** ![](assets/share-icon.png) .
1. Geben Sie den Namen des Benutzers, der Rolle, des Teams, der Gruppe oder des Unternehmens ein, für den bzw. das Sie den Zugriff entfernen möchten, im Feld **Zugriff bearbeiten `<Object Name>` auf** ein.
1. Wählen Sie im Dropdown-Menü für den Zugriff die Option **Kein Zugriff**.

   ![](assets/no-access-option-removing-permissions-bulk-tasks-nwe-350x166.png)

1. Wählen Sie im Dropdown-Menü für den Workfront-Zugriff von `<User Name>` aus, ob der Zugriff von diesen nur aus den ausgewählten Objekten oder allen anderen untergeordneten Objekten, die mit ihnen verknüpft sind, entfernt werden soll.\
   Die folgenden Szenarien existieren:

   * Wenn Sie die Entität nur aus dem Objekt entfernen, verliert diese Entität ihre Berechtigungen für das Objekt und ihre geerbten Berechtigungen für die untergeordneten Objekte. Wenn ihnen zuvor Berechtigungen für die untergeordneten Elemente einzeln gewährt wurden, behalten sie bei der Auswahl dieser Option dieselben Berechtigungen für alle untergeordneten Objekte bei, die mit ihnen verknüpft sind. 
   * Wenn Sie die Entität aus dem Objekt und allen untergeordneten Objekten entfernen, verliert diese Entität ihre Berechtigungen für das Objekt sowie alle untergeordneten Objekte, selbst wenn ihnen zuvor individuelle Berechtigungen für jedes untergeordnete Objekt erteilt wurden.

   **Beispiel:** Wählen Sie aus, ob Berechtigungen nur für die Aufgaben, die Sie in einer Liste ausgewählt haben, oder für die Probleme und Dokumente, die ebenfalls mit den Aufgaben verbunden sind, entfernt werden sollen.

   ![](assets/remove-permissions-bulk-drop-down-for-attached-objects-nwe-350x96.png)

1. (Optional) Um die Berechtigungen für mehrere Objekte stapelweise zu ändern, wählen Sie eine andere Freigabeebene für die ausgewählte Entität aus.

   Wenn sie beispielsweise über Verwaltungsberechtigungen verfügen, wählen Sie stattdessen Contribute oder Anzeigen aus.

1. Klicken Sie auf **Speichern**.

## Ererbte Berechtigungen entfernen

Vererbte Berechtigungen können aus Objekten entfernt werden, sodass Eigentümer spezifisch ermitteln können, wer Zugriff auf untergeordnete Objekte erhält, unabhängig vom Zugriff eines Benutzers auf ein übergeordnetes Objekt.

>[!IMPORTANT]
>
>Nur Benutzer mit der Berechtigung Verwalten können geerbte Berechtigungen entfernen.

So entfernen Sie geerbte Berechtigungen:

1. Rufen Sie ein Objekt auf, für das Sie über die Berechtigung &quot;Verwalten&quot;verfügen. Gehen Sie beispielsweise zu einer Aufgabe.
1. Wechseln Sie zum Feld für den Objektzugriff, wie im Abschnitt [Entitäten aus der Freigabeliste eines Objekts entfernen](#remove-entities-from-the-sharing-list-of-an-object) in diesem Artikel beschrieben.
1. Wählen Sie im Freigabefeld die **x** neben **Vererbte Berechtigung** aus, um alle dort aufgeführten Personen zu entfernen.

   ![](assets/remove-inherited-permissions-on-project-nwe-350x475.png)

   Dadurch wird sichergestellt, dass niemand, dem Berechtigungen für das übergeordnete Objekt (z. B. das Projekt) erteilt wurden, standardmäßig über Berechtigungen für diese Aufgabe verfügt. Sie müssen auflisten  einzelne Entitäten in der Freigabeliste der Aufgabe, um Berechtigungen für die Aufgabe zu erteilen.

   >[!TIP]
   >
   >Einzelne Entitäten können nicht aus der Liste &quot;Vererbte Berechtigungen&quot;entfernt werden. Sie können die geerbten Berechtigungen nur für alle aufgelisteten Entitäten deaktivieren.

1. Klicken Sie auf **Speichern**. 

## Privates Objekt

Wenn Sie ein Objekt systemweit freigegeben haben oder es für externe Benutzer freigegeben haben, indem Sie es öffentlich machen, können Sie es wieder privat machen, indem Sie die systemweiten oder öffentlichen Berechtigungen entfernen. 

Weitere Informationen dazu, wie Sie ein Objekt systemweit oder öffentlich verfügbar machen, finden Sie unter [Freigeben eines Objekts](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md).

So erstellen Sie ein privates Objekt:

1. Gehen Sie zu dem Objekt, das Sie privat machen möchten.\
   Navigieren Sie beispielsweise zu einem Bericht.
1. Klicken Sie auf **Berichtaktionen** und dann auf **Freigabe**.

   ![](assets/report-permissions-make-private-nwe-350x477.png)

1. Klicken Sie auf **Öffentlichen Zugriff entfernen** , um den Zugriff externer Benutzer auf die Anzeige des Berichts zu entfernen.
1. Klicken Sie auf **Systemweiten Zugriff entfernen** , um die Freigabe für alle Workfront-Benutzer zu beenden. 
1. Klicken Sie auf **Speichern**.
