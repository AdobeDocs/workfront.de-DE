---
title: Verwalten von Benutzern in Adobe Workfront Planning als eigenständiges Produkt
description: In diesem Artikel wird beschrieben, wie Sie Benutzer und Teams in Adobe Workfront Planning verwalten können, wenn Planning als eigenständiges Produkt erworben wird.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
source-git-commit: 697499fadf4d5d22292ededed381cb72e53fcae3
workflow-type: tm+mt
source-wordcount: '835'
ht-degree: 1%

---


# Verwalten von Benutzern in Adobe Workfront Planning als eigenständiges Produkt

>[!IMPORTANT]
>
>Die Informationen in diesem Artikel beziehen sich auf Adobe Workfront Planning, wenn es als eigenständiges Produkt gekauft wird. Lesen Sie diesen Artikel, wenn Ihr Unternehmen ein reines Adobe Workfront Planning-Paket erworben und kein Workfront Workflow-Paket gekauft hat.
>
>Informationen zu Adobe Workfront Planning beim Kauf zusammen mit einem Workfront-Paket finden Sie unter [Erste Schritte mit Adobe Workfront Planning](/help/quicksilver/planning/general/planning-overview.md).
>

Sie können Benutzende in Adobe Workfront Planning als eigenständiges Produkt auf dieselbe Weise verwalten wie in Adobe Workfront.

Es gibt einige Einschränkungen bei den Zugriffsebenen, die Sie Benutzenden in Workfront Planning zuweisen können.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktion in diesem Artikel anzuzeigen. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
</tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront-Planungspaket</p></td> 
   <td> 
<p>Beliebige Workfront-Planung als eigenständiges Paket</p>

</td> </tr>
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-Lizenz</p></td> 
   <td><p>Planungsadmin</p>
   </td> 
  </tr>

</tbody> 
</table>

Weitere Informationen zum Zugriff für Workfront als eigenständiges Paket finden Sie unter [Zugriff für Adobe Workfront Planning als eigenständiges Produkt erforderlich](/help/quicksilver/planning/planning-sta/access-needed-for-planning-sta.md).
+++    

## Zugriffsebenen in Adobe Workfront Planning

Benutzenden in Workfront Planning können beim Kauf als eigenständiges Produkt die folgenden Zugriffsebenen zugewiesen werden:

* Planungsadmin
* Planungsstandard

Weitere Informationen zu den in den einzelnen Zugriffsfunktionen enthaltenen Funktionen finden Sie unter [Zugriff erforderlich für Adobe Workfront Planning als eigenständiges Produkt](/help/quicksilver/planning/planning-sta/access-needed-for-planning-sta.md).

Beachten Sie beim Arbeiten mit Zugriffsebenen in Workfront Planning als eigenständiges Produkt Folgendes:

* Zugriffsebenen in Workfront Planning können nicht erstellt oder geändert werden. Sie sind vorkonfiguriert.

* Nachdem Sie Benutzende als Admin für das Workfront-Produkt zur Adobe Admin Console hinzugefügt haben, werden sie in Workfront Planning automatisch dieser Zugriffsebene zugewiesen und ihre Zugriffsebene kann in Planning nicht bearbeitet werden.
* Eine Planning Standard-Zugriffsebene kann nur Benutzern in Planning zugewiesen werden, nachdem die Benutzer zur Admin Console hinzugefügt wurden. Dies ist die einzige Zugriffsebene, die Sie einem Benutzer manuell zuweisen können.

## Verwalten von Benutzern in Workfront Planning als eigenständiges Produkt

1. Führen Sie als Planning-Admin einen der folgenden Schritte aus:

   * Wenn Sie Neukunde von Workfront Planning sind, erhalten Sie eine E-Mail von Adobe Workfront, in der Sie darauf hingewiesen werden, dass Sie jetzt über ein Konto in Adobe Workfront verfügen. Verwenden Sie den Link in der E-Mail, um sich bei der Admin Console anzumelden.

   * Wenn Sie bereits ein Workfront Planning-Administrator sind und andere zu Ihrem Konto hinzufügen möchten, melden Sie sich bei Admin Console an.

   Weitere Informationen finden Sie unter [Verwalten von Benutzern in der Adobe Admin Console](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/admin-console.md).

1. Beginnen Sie in der Admin Console damit, Benutzer auf einer der folgenden Registerkarten hinzuzufügen:

   * **Administratoren**: Benutzer werden in Planning automatisch als Planning-Administratorbenutzer erstellt.
   * **Benutzer**: In Workfront Planning muss eine Zugriffsebene zugewiesen werden.

1. (Bedingt) Melden Sie sich von der Adobe CX Enterprise-Startseite aus bei Workfront an.

   Workfront Planning wird geöffnet.
1. Klicken Sie auf **Hauptmenü** > **Benutzer** > **Neuer Benutzer**.

   ![Neues Benutzerfeld in Planning eigenständig](assets/new-user-box-planning-sta.png)

1. Aktualisieren Sie **Feld** Neuer Benutzer“ die folgenden Informationen:

   * **Vorname(n)**: Der Name, den Sie der Admin Console hinzugefügt haben.
   * **Nachname**: Der Name, den Sie der Admin Console hinzugefügt haben.
   * **E-Mail-Adresse (Benutzername)**: Dieselbe E-Mail, die Sie der Admin Console hinzugefügt haben.
   * **Benutzer ist aktiv**: Um anzugeben, dass der Benutzer aktiv ist und sich bei Workfront Planning anmelden und Datensätzen zugewiesen werden kann, aktivieren Sie die Einstellung.
   * **Zugriffsebene**: Wählen Sie „Planning Standard“ für Benutzer ohne Administratorrechte aus. Das ist die einzige Option.

     >[!TIP]
     >
     >Durch das Hinzufügen eines Benutzers, der bereits als Administrator in der Admin Console eingerichtet wurde, wird dem Benutzer automatisch die Zugriffsebene „Planning-Administrator“ hinzugefügt. Dieser kann nicht bearbeitet werden.

   * **Teams**: Wählen Sie aus dem Dropdown-Menü Teams aus, die mit dem Benutzer verknüpft werden sollen. Teams müssen erstellt werden, bevor Sie sie Benutzern zuweisen können.

     Weitere Informationen finden Sie unter [Verwalten von Teams](/help/quicksilver/planning/planning-sta/manage-teams-in-planning-sta.md).

1. Klicken Sie **Jetzt hochladen**, um ein Profilbild hinzuzufügen, und klicken Sie dann auf **Speichern**.

1. Klicken Sie auf **Speichern** oder **Person hinzufügen und eine andere**, um den Benutzer zu speichern und eine weitere hinzuzufügen.

   Benutzende werden hinzugefügt und erhalten eine E-Mail, um sich bei Workfront Planning anzumelden.
1. (Optional) Führen Sie einen der folgenden Schritte aus, um einen vorhandenen Benutzer zu bearbeiten:

   * Bewegen Sie den Mauszeiger über den Namen des Benutzers in der Liste und klicken Sie dann auf das Menü **Mehr** ![Mehr Menü](assets/more-menu.png) > **Benutzer bearbeiten**
   * Wählen Sie den Benutzer in der Liste aus und klicken **auf** Benutzer bearbeiten“ in der blauen Symbolleiste am unteren Rand der Seite.
1. (Optional) Führen Sie einen der folgenden Schritte aus, um einen Benutzer zu löschen:

   * Bewegen Sie den Mauszeiger über den Namen des Benutzers in der Liste und klicken Sie dann auf das Menü **Mehr** ![Mehr Menü](assets/more-menu.png) > **Benutzer löschen**
   * Wählen Sie das Team in der Liste aus **klicken Sie dann unten auf** blauen Symbolleiste auf der Seite auf „Benutzer löschen“
1. Klicken Sie **zur Bestätigung** „Löschen“.
1. (Optional) Führen Sie einen der folgenden Schritte aus, um einen Benutzer zu deaktivieren:

   * Bewegen Sie den Mauszeiger über den Namen des Benutzers in der Liste und klicken Sie dann auf das Menü **Mehr** ![Mehr Menü](assets/more-menu.png) > **Deaktivieren**
   * Wählen Sie das Team in der Liste aus **klicken Sie dann unten** der Seite in der blauen Symbolleiste auf „Deaktivieren“
1. Klicken Sie **Bestätigung auf** Deaktivieren“.

   Um historische Aufzeichnungen über Ihre Arbeit zu speichern, empfehlen wir, Benutzer zu deaktivieren, anstatt sie zu löschen.

