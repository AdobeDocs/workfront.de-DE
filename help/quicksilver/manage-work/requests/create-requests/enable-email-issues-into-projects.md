---
product-area: requests
navigation-topic: create-requests
title: Benutzern die Möglichkeit geben, ein Problem per E-Mail an ein Anfrage-Warteschlangenprojekt zu senden
description: Sie können ein Projekt so konfigurieren, dass Benutzende dem Projekt Probleme per E-Mail hinzufügen können.
author: Alina, Courtney
feature: Work Management
exl-id: 556775e8-7ac9-482d-8c1c-863678584aa4
source-git-commit: bca543ad2ee8ead26cfa662900eb513af36f743c
workflow-type: tm+mt
source-wordcount: '812'
ht-degree: 0%

---

# Benutzern die Möglichkeit geben, ein Problem per E-Mail an ein Anfrage-Warteschlangen-Projekt zu senden

<!-- Audited: 4/2025 -->

<!--
<p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;When updating POP account information here, also update information in these articles: Allowing users to reply to email notifications, Configuring Email Notifications, Understanding the Queue Details Tab in a Project )</p>
-->

Sie können ein Projekt so konfigurieren, dass Benutzende dem Projekt Probleme per E-Mail hinzufügen können. Sie können nur dann zulassen, dass Probleme per E-Mail an ein Projekt gesendet werden, wenn das Projekt als Anfrage-Warteschlange festgelegt ist. Weitere Informationen zum Erstellen eines Anfrage-Warteschlangenprojekts finden Sie unter [Erstellen einer Anfrage-Warteschlange](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan</td> 
   <td> <p>Beliebig </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td> <p>Neu: Mitwirkender oder höher</p>
   Oder
   <p>Aktuell: Anforderung oder höher</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriff auf Anfragen bearbeiten</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> Produkt</td> 
   <td> <ul><li>Adobe Workfront</li><li>Sie müssen über Adobe Workfront Planning verfügen, um Planungsanfragen oder Anfrageformulare anzuzeigen</td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Voraussetzungen

Die folgenden Bedingungen sind erforderlich, um ein Projekt so zu konfigurieren, dass Benutzende dem Projekt Probleme per E-Mail hinzufügen können:

* Benutzende, die Probleme an dieses Konto senden, müssen aktive Benutzende mit einer Lizenz für Workfront sein.
* Benutzer, die Probleme an dieses Konto senden, müssen über die Berechtigung „Problem hinzufügen“ für das Projekt verfügen.
* Externe Benutzer können Probleme nicht per E-Mail an eine Anfrage-Warteschlange senden, da sie keinen Zugriff zum Erstellen von Problemen haben.
* Nur E-Mails von einer E-Mail-Adresse, die einem aktiven Workfront-Benutzer zugeordnet ist, dürfen Probleme an das Projekt senden. E-Mails, die von einer E-Mail-Adresse, die nicht mit einem Workfront-Konto verknüpft ist, an einen aktiven Workfront-Benutzer weitergeleitet werden, können keine Probleme im Rahmen des Projekts erstellen, da die E-Mail-Adresse des ursprünglichen Absenders mit einem aktiven Workfront-Konto verknüpft werden muss.
* Das Projekt wird als Anfrage-Warteschlange eingerichtet.
* Das mit dem Projekt verknüpfte E-Mail-Konto ist nicht mit einem Workfront-Benutzerkonto verknüpft.

## Konfigurieren des Projekts in Workfront

>[!NOTE]
>
>Beachten Sie beim Aktivieren der E-Mail-Warteschlangeneinstellungen Folgendes:
>
>* Workfront ermöglicht eine eindeutige E-Mail pro Anfrage-Warteschlange für alle Cluster. Wenn Sie Ihre Anfrage-Warteschlange deaktivieren, behalten Sie die von Ihnen erstellte E-Mail-Adresse so lange bei, wie sie sich noch im Feld Eingangs-E-Mail-Adresse befindet. Wenn Sie die Verwendung der Eingangs-E-Mail einstellen möchten, müssen Sie sie aus dem Feld Eingangs-E-Mail löschen, damit sie für die zukünftige Verwendung verfügbar ist.
>
>* Wenn die Anfrage-Warteschlange mehrere Warteschlangenthemen oder Themengruppen enthält, wählt Workfront nach dem Zufallsprinzip das Warteschlangenthema aus, an das die per E-Mail gesendeten Anfragen gesendet werden, wodurch E-Mail gesendete Anfragen schwer zu verwalten sind.
>  &#x200B;>Es wird empfohlen, dass das Projekt, das Sie für den Empfang von Anfragen per E-Mail eingerichtet haben, nicht mehr als ein Warteschlangen-Thema haben sollte. Wenn die gesendeten Anfragen für verschiedene Ressourcen oder Projekte vorgesehen sind, sollten Sie sie nach dem Senden manuell weiterleiten oder verschieben.

1. Navigieren Sie zu dem Projekt, das Sie aktivieren möchten, um Probleme per E-Mail zu empfangen.
1. Klicken Sie **linken Bedienfeld** Warteschlangendetails“.
1. Wählen **Bereich &quot;**&quot; die Option **Als Warteschlange für Hilfeanfragen veröffentlichen**.

1. Scrollen Sie nach unten zum Bereich **E-Mail-Warteschlangeneinstellungen** und wählen Sie dann **Anforderungsaufnahme per E-Mail aktivieren** aus.

1. Geben Sie den Anfang der E-Mail-Adresse in das Feld **Eingangs-E-Mail-**&quot; ein.

   Sie müssen eine eindeutige E-Mail-Adresse erstellen. Es wird empfohlen, den Namen Ihres Unternehmens als Teil Ihrer Eingangs-E-Mail-Adresse zu verwenden.

   >[!CAUTION]
   >
   >* Diese E-Mail-Adresse kann nicht aus dem Papierkorb wiederhergestellt werden, wenn das Projekt, das die Anfrage-Warteschlange enthält, gelöscht wird.
   >
   >* Da diese E-Mail-Adresse eindeutig sein muss, ist sie in Zukunft möglicherweise nicht mehr verfügbar, wenn sie gelöscht wird.
   <!--
   >This was the case previously, but it's not working this way anymore, since August 2022: * Emails forwarded to this email address are not added as issues to the project in&nbsp;Workfront. Only emails created from this email address are added as issues.
   -->

1. (Optional) Wählen Sie die **Alle Probleme weiterleiten, die nicht per E-Mail gesendet werden können** und geben Sie dann eine Weiterleitungs-E-Mail-Adresse in das Feld unten ein.

   Diese E-Mail-Adresse empfängt Informationen zu E-Mails, die nicht an das Projekt gesendet werden konnten.

1. Klicken Sie auf **Speichern**. Wenn jetzt Benutzende mit einem aktiven Workfront-Konto eine E-Mail an diese E-Mail-Adresse senden, wird im Workfront-Projekt ein Problem erstellt.

   >[!NOTE]
   >
   >Benutzer müssen Zugriff haben, um Probleme im Projekt erstellen zu können, damit sie es per E-Mail senden können. Sie können diesen Zugriff im Dialogfeld Freigabe unter Erweiterte Einstellungen gewähren.
   >
   >Externe Benutzer können Probleme nicht per E-Mail an eine Anfrage-Warteschlange senden, da sie keinen Zugriff zum Erstellen von Problemen haben.

## Anfrage in Workfront empfangen

Wenn ein Workfront-Benutzer eine E-Mail an Workfront sendet, passiert Folgendes:

* Die Betreffzeile der E-Mail wird zum Problemnamen.
* Der Textkörper der E-Mail wird zur Beschreibung des Problems.
* Wenn der E-Mail Dokumente beigefügt sind, werden diese Dokumente dem Problem in Workfront beigefügt.

  >[!NOTE]
  >
  > MSG-Dateien werden nicht unterstützt und nicht an das Problem in Workfront angehängt.

* Der Benutzer, der die E-Mail sendet, wird zum Primären Ansprechpartner für das neue Problem in Workfront.
* Der Textkörper der E-Mail darf 4.000 Zeichen nicht überschreiten.
* E-Mail-Anhänge dürfen insgesamt 7 MB nicht überschreiten.
