---
product-area: documents
navigation-topic: approvals
title: Hochladen einer neuen Dokumentversion und Anfordern einer Genehmigung
description: Sie können eine neue Dokumentversion hochladen und die Genehmigung von anderen Benutzern in Adobe Workfront anfordern.
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: 0eb8cfba-2317-419c-b28f-da2e7a99401c
source-git-commit: 8270a107ba2501eddbb27f52c843c337aa1f8a99
workflow-type: tm+mt
source-wordcount: '480'
ht-degree: 0%

---

# Hochladen einer neuen Dokumentversion und Anfordern einer Genehmigung

Wenn ein Dokument als für eine vorherige Überprüfung erforderlich gekennzeichnet ist, können Sie eine neue Version in das Originaldokument hochladen und eine weitere Genehmigungsrunde starten. Nachdem Sie eine neue Version des Dokuments hochgeladen haben, werden die vorherigen Versionen gesperrt.

Wenn der Dateiname der neuen Version vom Dateinamen der vorherigen Version abweicht, zeigt Workfront das Dokument mit dem neueren Dateinamen an.

Wenn einem Dokument mit ausstehenden Genehmigungen eine neue Version hinzugefügt wird, wird die Genehmigung für die vorherige Version als „Zurückgezogen“ angezeigt. Der vorherige Genehmigungsprozess wird geschlossen, auch wenn einige Teilnehmer noch keine Entscheidung getroffen haben.

Wenn die neueste Dokumentversion gelöscht wird, bleiben die vorherigen Versionen gesperrt. Wenn Sie eine frühere Version bearbeiten müssen, müssen Sie sie manuell entsperren.


## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über Folgendes verfügen:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p> Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenzen*</td> 
   <td> <p>Aktuell: Anforderung oder höher</p>
   oder
   <p>Neu: Mitwirkender oder höher</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Konfigurationen der Zugriffsebene*</td> 
   <td> <p>Zugriff auf Dokumente bearbeiten</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Einschränkungen in Ihrer Zugriffsebene festgelegt hat. Informationen dazu, wie Workfront-Admins Ihre Zugriffsebene ändern können, finden Sie unter <a href="/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Erstellen oder Ändern benutzerdefinierter Zugriffsebenen</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Bearbeitungszugriff auf das mit dem Dokument verknüpfte Objekt</p> <p>Informationen zum Anfordern zusätzlicher Zugriffsberechtigungen finden Sie unter <a href="/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/grant-and-request-access-to-objects.md" class="MCXref xref">Anfordern von Zugriffsberechtigungen für Objekte </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

Wenden Sie sich an Ihren Workfront-Administrator, um herauszufinden, über welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie verfügen.

+++

## Verwenden von Drag-and-Drop, um eine neue Version hinzuzufügen

>[!NOTE]
>
>Drag-and-Drop funktioniert nicht mit Internet Explorer.

1. Navigieren Sie zum Bereich Dokumente , in den das Dokument hochgeladen wird.
1. Ziehen Sie die neue Version des Dokuments von Ihrem Desktop oder einer separaten Browser-Registerkarte auf die vorhandene Version in Workfront.

   Wenn Sie die neue Version ziehen, können Sie den Mauszeiger über einen Workfront-Dokumentordner bewegen, um ihn zu öffnen. Sie können dann nach oben und unten scrollen, indem Sie die Dateien an den oberen oder unteren Bildschirmrand ziehen.

1. Legen Sie die neue Version auf der Registerkarte „Dokumente **über der vorhandenen Datei**.

1. Nachdem das Dokument hochgeladen wurde, klicken Sie darauf und öffnen Sie das Bedienfeld Dokumentzusammenfassung .

1. Scrollen Sie nach unten zum Abschnitt **Genehmigungen** im Bereich Dokumentzusammenfassung und klicken Sie dann auf **Hinzufügen**.

![Genehmigende Personen in der Dokumentzusammenfassung hinzufügen](assets/doc-summary-add-approvers.png)

1. (Optional) Legen Sie eine Frist für die Genehmigung fest. Benutzer und Teams werden 72 Stunden und dann 24 Stunden vor dem angegebenen Termin per E-Mail benachrichtigt.

1. Um schnell Prüfer und genehmigende Personen aus der vorherigen Version hinzuzufügen, klicken Sie auf die Schaltfläche Hinzufügen neben den unten aufgeführten Namen.
   <!--need screenshot when working-->

1. (Optional) Ändern Sie die Rolle von „Genehmigende Person/Prüfende Person“.

1. Um neue genehmigende Personen und Prüfer hinzuzufügen, klicken Sie auf **Prüfer** oder **genehmigende Person** und beginnen Sie mit der Eingabe des Benutzers oder Teams.

   ![Genehmigende Person und Frist hinzufügen](assets/add-approver-and-deadline.png)
