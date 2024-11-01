---
product-area: projects
navigation-topic: approvals
title: Validierungsanfrage delegieren
description: Durch die Delegierung von Validierungsanfragen können Sie einen anderen Benutzer zuweisen, der Ihre Anfragen für einen bestimmten Zeitraum validiert, z. B. wenn Sie im Urlaub nicht im Hause sein werden.
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: 01b76dd5-98cb-4f0d-97ff-7e665f843a9c
source-git-commit: 69c1e99b996025615e96a84bc8e91cbe2ae6ee48
workflow-type: tm+mt
source-wordcount: '1194'
ht-degree: 0%

---

# Validierungsanfrage delegieren

Sie können die Arbeit, der Sie zugewiesen sind, während Sie nicht im Büro sind, vorübergehend delegieren. Sie können Aufgaben- und Problemzuweisungen delegieren oder Genehmigungsanfragen delegieren. In diesem Artikel wird beschrieben, wie Sie Genehmigungsanfragen delegieren. Informationen zum Delegieren von Aufgaben und Problemzuweisungen finden Sie unter [Aufgaben und Probleme delegieren](../../manage-work/delegate-work/how-to-delegate-work.md).

Sie können die folgenden Arten von Genehmigungen delegieren, unabhängig davon, wie die Genehmigung Ihnen zugewiesen wurde (unabhängig davon, ob sie Ihnen direkt zugewiesen wurden, einem Team, dem Sie angehören, oder Ihrer beruflichen Rolle):

* Projektgenehmigungen
* Aufgabenvalidierungen
* Genehmigungen ausstellen

Sie können keine Zeitblatt-, Dokument- oder Testversandgenehmigungen delegieren.

>[!NOTE]
>
>Um sicherzustellen, dass keine Inkonsistenzen mit den Daten auftreten, die Sie für die Zuweisung Ihrer Genehmigungen planen, empfehlen wir, dass die Zeitzone Ihres Benutzerprofils mit der Ihres Zeitplans übereinstimmt. Weitere Informationen finden Sie in den folgenden Artikeln:
>
>* [Erstellen eines Zeitplans](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)
>* [Bearbeiten des Benutzerprofils](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)
>

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-Plan*</p></td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-Lizenz*</p></td> 
   <td> <p>Überprüfen oder höher</p> </td> 
  </tr> 
 </tbody> 
</table>

Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan oder welchen Lizenztyp Sie haben.

+++

## Grundlegendes zum Benutzerzugriff für delegierte Genehmigungen

Während des festgelegten Genehmigungszeitraums hat der Benutzer, an den Sie eine Genehmigungsanfrage delegieren, die folgenden Möglichkeiten:

* Können bestehende Genehmigungsanfragen genehmigen oder ablehnen, wenn keine Entscheidung getroffen wurde
* Kann neue Validierungsanfragen, die in einem bestimmten Zeitraum empfangen wurden, genehmigen und ablehnen
* Ermöglicht Zugriff auf Objekte anzeigen, die auf die Genehmigung warten

  >[!NOTE]
  >
  > Der Adobe Workfront-Administrator kann den Zugriff auf bestimmte Objekttypen einschränken. Wenn ein Benutzer keinen Zugriff auf einen Objekttyp hat und eine Genehmigung dieses Typs an den Benutzer delegiert wird, hat der Benutzer keinen Zugriff auf Ansicht auf das Objekt. Der Benutzer kann jedoch weiterhin Genehmigungsanfragen von der Seite **Startseite** genehmigen oder ablehnen, wie unter [Arbeit validieren](../../review-and-approve-work/manage-approvals/approving-work.md) beschrieben.\
  >Beispielsweise gehört Benutzer A zu Gruppe A. Der Workfront-Administrator hat die Zugriffsrechte für Gruppe A eingeschränkt, sodass Benutzer dieser Gruppe Aufgaben in Workfront nicht anzeigen können. Wenn eine Aufgabengenehmigungsanforderung an Benutzer A delegiert wird, kann Benutzer A die Aufgabe, mit der die Genehmigung verknüpft ist, nicht anzeigen. Benutzer A kann die Genehmigungsanfrage jedoch auf der Startseite genehmigen oder ablehnen.

  Informationen dazu, wie der Workfront-Administrator den Zugriff auf Objekttypen in der Einrichtung beschränken kann, finden Sie unter  [Erstellen oder ändern Sie benutzerdefinierte Zugriffsebenen](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). 

Nachdem die Genehmigungsdelegierung beendet oder abgebrochen wurde, hat der Benutzer folgende Berechtigungen:

* Hat keinen Zugriff mehr auf die Genehmigung der Arbeit für Elemente, die genehmigt werden müssen
* Erhalten Sie weiterhin Zugriff auf Arbeitselemente anzeigen .\
  Benutzer, denen der Zugriff auf Objekte über eine Genehmigungsdelegation gewährt wurde, behalten den Zugriff auf die Option Anzeigen auch dann bei, wenn die Validierungsdelegation beendet oder zurückgerufen wird. Um den Zugriff auf alle Objekte anzeigen zu entfernen, auf die der Benutzer während der Zeit, in der die Genehmigungen delegiert wurden, Zugriff hatte, müssen Sie zum Objekt gehen und die Zugriffsrechte direkt vom Objekt entfernen.

## Delegieren von Genehmigungen an einen anderen Benutzer {#delegate-your-approvals-to-another-user}

Sie können die folgenden Arten von Genehmigungen delegieren, unabhängig davon, wie die Genehmigung Ihnen zugewiesen wurde (unabhängig davon, ob sie Ihnen direkt zugewiesen wurden, einem Team, dem Sie angehören, oder Ihrer beruflichen Rolle):

* Projektgenehmigungen
* Aufgabenvalidierungen
* Genehmigungen ausstellen

Sie können keine Zeitblatt-, Dokument- oder Testversandgenehmigungen delegieren.

Beachten Sie beim Delegieren von Genehmigungen Folgendes:

* Wenn Sie Genehmigungen delegieren, werden alle Ihre Genehmigungen delegiert. Sie können keine individuellen Genehmigungsanfragen delegieren.
* Sie können Genehmigungen nur an einen Benutzer delegieren. Sie können Genehmigungen nicht gleichzeitig an mehrere Benutzer delegieren.\
  Alle Genehmigungen für alle Projekte, Aufgaben und Probleme werden an den Benutzer delegiert, den Sie bestimmen.
* Maximal 5 Benutzer können Genehmigungen gleichzeitig an denselben Benutzer delegieren. Mit anderen Worten: Ein einzelner Benutzer kann nicht für mehr als fünf Benutzer gleichzeitig als temporärer Genehmiger bestimmt werden.
* Die Aktivität bezüglich der Validierungen wird auf der Registerkarte Aktualisierungen angezeigt. Sie müssen Systemaktualisierungen anzeigen aktiviert haben. Sowohl der Benutzer, der die Validierung delegiert, als auch der Benutzer, dem Validierungen zugewiesen werden, erhalten eine E-Mail-Benachrichtigung zur Validierungsaktivität.

### Delegieren von Genehmigungen aus dem Startbereich


So delegieren Sie Genehmigungen an einen anderen Benutzer:

1. Klicken Sie oben rechts auf das Hauptmenü ]**![](assets/main-menu-icon.png) und dann auf**[!UICONTROL  Startseite ]**.**[!UICONTROL 
1. (Bedingt) Klicken Sie auf **Anpassen** , um das Widget **Meine Genehmigungen** hinzuzufügen.
1. Gehen Sie zum Widget Meine Genehmigungen und klicken Sie dann auf **Meine Genehmigungen delegieren**.

   >[!NOTE]
   >
   >Workfront-Administratoren können die Validierungsdelegationen im Setup-Bereich deaktivieren. Wenn die Validierungsdelegationen deaktiviert sind, wird die Schaltfläche Validierungen delegieren nicht angezeigt.

   ![](assets/delegate-approvals-home.png)

1. Geben Sie die folgenden Informationen im Abschnitt &quot;Meine Genehmigungen delegieren&quot;an:

   * **Name**: Beginnen Sie mit der Eingabe des Namens des Benutzers, an den Sie Genehmigungen delegieren möchten, und klicken Sie dann auf den Namen, wenn er im Dropdown-Menü angezeigt wird.
   * **Startdatum**: Wählen Sie das Datum aus, an dem die Weiterleitung der Validierungen beginnen soll. Die Weiterleitung beginnt um 12:00 Uhr des von Ihnen ausgewählten Datums.\
     Das Startdatum muss das aktuelle oder ein künftiges Datum sein.
   * **Enddatum**: Führen Sie einen der folgenden Schritte aus:
      * Wählen Sie das Datum aus, an dem die Weiterleitung der Validierungen beendet werden soll. Die Weiterleitung endet um 11:59 Uhr an dem von Ihnen ausgewählten Datum.
      * Wählen Sie **Kein Enddatum** aus, um Workfront so zu konfigurieren, dass Genehmigungen unbegrenzt delegiert werden.

1. Klicken Sie auf **Speichern**.

### Delegieren von Genehmigungen aus Ihrem Benutzerprofil

1. Klicken Sie im linken Bereich auf das Symbol **Hauptmenü** > **Ihr Name** > **Ausschaltzeit** .
1. Klicken Sie auf **Genehmigungen delegieren**.

   >[!NOTE]
   >
   >Workfront-Administratoren können die Validierungsdelegationen im Setup-Bereich deaktivieren. Wenn die Validierungsdelegationen deaktiviert sind, wird die Schaltfläche Validierungen delegieren nicht angezeigt.
1. Geben Sie die folgenden Informationen im Abschnitt &quot;Meine Genehmigungen delegieren&quot;an:

   * **Name**: Beginnen Sie mit der Eingabe des Namens des Benutzers, an den Sie Genehmigungen delegieren möchten, und klicken Sie dann auf den Namen, wenn er im Dropdown-Menü angezeigt wird.
   * **Startdatum**: Wählen Sie das Datum aus, an dem die Weiterleitung der Validierungen beginnen soll. Die Weiterleitung beginnt um 12:00 Uhr des von Ihnen ausgewählten Datums.\
     Das Startdatum muss das aktuelle oder ein künftiges Datum sein.
   * **Enddatum**: Führen Sie einen der folgenden Schritte aus:
      * Wählen Sie das Datum aus, an dem die Weiterleitung der Validierungen beendet werden soll. Die Weiterleitung endet um 11:59 Uhr an dem von Ihnen ausgewählten Datum.
      * Wählen Sie **Kein Enddatum** aus, um Workfront so zu konfigurieren, dass Genehmigungen unbegrenzt delegiert werden.

## Validierungsdelegationen aktualisieren oder stoppen {#update-or-stop-an-approval-delegation}

1. Klicken Sie oben rechts auf das Hauptmenü ]**![](assets/main-menu-icon.png) und dann auf**[!UICONTROL  Startseite ]**.**[!UICONTROL 
1. (Bedingt) Klicken Sie auf **Anpassen** , um das Widget **Meine Genehmigungen** hinzuzufügen.

1. Gehen Sie zum Widget Meine Genehmigungen und klicken Sie dann auf **Delegation bearbeiten**.
   ![](assets/edit-delegations.png)
<!--
   Or

   If your system or group administrator enabled task and issue delegation, click **Edit delegation**, then click **Delegate approvals**.   -->

1. (Bedingt) Führen Sie einen der folgenden Schritte aus:

   * Um die vorhandene Genehmigungsdelegierung zu aktualisieren: Ändern Sie die angezeigten Informationen und klicken Sie auf **Speichern**.

   * Um die vorhandene Zuweisung zu stoppen: Klicken Sie auf **Delegierung stoppen** und dann zur Bestätigung auf **Delegierung stoppen** .

## Delegierte Genehmigungen anzeigen {#view-delegated-approvals}

Im Widget Meine Genehmigungen können Sie nur die folgenden Arten von Validierungsdelegationen anzeigen:

* Projektgenehmigungen
* Aufgabenvalidierungen
* Genehmigungen ausstellen

So zeigen Sie delegierte Genehmigungen an:

1. Klicken Sie oben rechts auf das Hauptmenü ]**![](assets/main-menu-icon.png) und dann auf**[!UICONTROL  Startseite ]**.**[!UICONTROL 
1. (Bedingt) Klicken Sie auf **Anpassen** , um das Widget **Meine Genehmigungen** hinzuzufügen.
1. Klicken Sie im Widget **Meine Genehmigungen** auf das Dropdown-Menü **Filter** und dann auf **Delegierte Genehmigungen**.\
   Alle Ihnen zugewiesenen Genehmigungen werden in der Liste angezeigt.
