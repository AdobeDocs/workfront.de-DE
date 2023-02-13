---
product-area: projects
navigation-topic: financials
title: Ändern der Projektwährung
description: Als Projektmanager können Sie ein Projekt so konfigurieren, dass eine andere Währung als die Standardwährung für Ihr Adobe Workfront-System verwendet wird. Auf diese Weise können Sie bei der Berechnung von Arbeitskosten und Einnahmen Finanzinformationen zu Ihrem Projekt in der gewünschten Währung anzeigen.
author: Alina
feature: Work Management
exl-id: c496fe92-5c17-41a5-972b-1c063643bde3
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '564'
ht-degree: 0%

---

# Ändern der Projektwährung

Als Projektmanager können Sie ein Projekt so konfigurieren, dass eine andere Währung als die Standardwährung für Ihr Adobe Workfront-System verwendet wird. Auf diese Weise können Sie bei der Berechnung von Arbeitskosten und Einnahmen Finanzinformationen zu Ihrem Projekt in der gewünschten Währung anzeigen.

Bevor Sie alternative Währungen verwenden können, wie in diesem Abschnitt beschrieben, muss der Workfront-Administrator zunächst mehrere Währungen aktivieren und konfigurieren, wie im Artikel beschrieben [Wechselkurse einrichten](../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md).

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf Projekte bearbeiten</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Berechtigungen für ein Projekt verwalten</p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Überlegungen beim Ändern der Währung eines Projekts in Workfront

* Sie können die Währung eines Projekts nicht ändern, wenn das Projekt finanzielle Informationen enthält.
* Die Sätze werden für Arbeitskosten verwendet. Umsatzberechnungen und werden künftig für Berichtszwecke verwendet.
* Wenn Sie für ein Projekt keine andere Währung angeben, geht Workfront davon aus, dass die Währung des Projekts die Standardwährung des Systems ist. Informationen zur Standardwährung auf Systemebene finden Sie unter [Wechselkurse einrichten](../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md).
* Standardmäßig haben alle Benutzer mit voller Lizenz Zugriff auf Währungen und Wechselkurse. Der Workfront-Administrator muss zusätzlichen Administratorzugriff für **Wechselkurse** , damit Benutzer spezifische Raten für Projekte festlegen können.
* Die Wechselkurse in Workfront sind nicht dynamisch. Der Wert wird von einem Administrator festgelegt und muss bei Wechselkursänderungen aktualisiert werden.
* Wenn Sie einen Bericht erstellen, der die Währung eines Projekts widerspiegelt, werden alle Berichte standardmäßig nach der Standardwährung des Projekts gruppiert. Wenn Sie einen Bericht mit mehreren Projekten erstellen, die unterschiedliche Wechselkurse haben, spiegeln alle auf das Projekt angewendeten Gruppierungen den Standardwechselkurs auf Systemebene wider. Weitere Informationen finden Sie im Artikel [Erstellen von Finanzdatenberichten mit eindeutigen Wechselkursen](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-financial-data-reports-unique-exchange-rates.md).

## Währung für ein Projekt konfigurieren

1. Wechseln Sie zu dem Projekt, in dem Sie die Standardwährung ändern möchten.

   >[!TIP]
   >
   >Stellen Sie sicher, dass das Projekt nicht bereits über finanzielle Informationen verfügt. Stellen Sie beispielsweise sicher, dass mit dem Projekt keine geplanten oder tatsächlichen Kosten verbunden sind.

1. Klicken **Projektdetails** Navigieren Sie im linken Bereich zu **Finanzen** Bereich.
1. Klicken **Hinzufügen** im **Währung** und wählen Sie die Währung aus, die Sie als Standardwährung für das Projekt verwenden möchten. Alle Währungen, die Ihr Workfront-Administrator für Ihre Workfront-Instanz festgelegt hat, werden angezeigt.

   ![](assets/currency-on-project-expanded-nwe.png)

1. (Bedingt) Wenn Sie eine andere Währung als die für Ihr Workfront-System festgelegte Standardwährung auswählen, geben Sie den Wechselkurs für die gewählte Währung an, da dieser sich auf die Währung bezieht, die im System als Basiswährung festgelegt ist.
1. Klicken **Änderungen speichern**.
