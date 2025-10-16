---
product-area: projects
navigation-topic: financials
title: Projektwährung ändern
description: Als Projekt-Manager können Sie ein Projekt so konfigurieren, dass es eine andere Währung als die Standardwährung für Ihr Adobe Workfront-System verwendet. Auf diese Weise können Sie bei der Berechnung von Arbeitskosten und Umsatz Finanzinformationen zu Ihrem Projekt in der gewünschten Währung anzeigen.
author: Lisa
feature: Work Management
exl-id: c496fe92-5c17-41a5-972b-1c063643bde3
source-git-commit: 23a4d055871c9138818e70fa1cd936581dbd7552
workflow-type: tm+mt
source-wordcount: '509'
ht-degree: 1%

---

# Projektwährung ändern

Als Projekt-Manager können Sie ein Projekt so konfigurieren, dass es eine andere Währung als die Standardwährung für Ihr Adobe Workfront-System verwendet. Auf diese Weise können Sie bei der Berechnung von Arbeitskosten und Umsatz Finanzinformationen zu Ihrem Projekt in der gewünschten Währung anzeigen.

Bevor Sie alternative Währungen wie in diesem Abschnitt beschrieben verwenden können, muss der Workfront-Administrator zunächst mehrere Währungen aktivieren und konfigurieren, wie im Artikel [Einrichten von Wechselkursen](../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md) beschrieben.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront-Paket</td> 
   <td>Beliebig </td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront-Lizenz</td> 
   <td>
   <p>Standard</p>
   <p>Plan</p></td> 
  </tr> 
  <tr> 
   <td>Konfigurationen der Zugriffsebene</td> 
   <td>Zugriff auf Projekte bearbeiten</td> 
  </tr> 
  <tr> 
   <td>Objektberechtigungen</td> 
   <td>Verwalten von Berechtigungen für das Projekt</td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Überlegungen zum Ändern der Projektwährung in Workfront

* Sie können die Währung eines Projekts nicht ändern, wenn im Projekt Finanzinformationen vorhanden sind.
* Die Sätze werden für Arbeitskosten, Einnahmenberechnungen und in Zukunft für Berichtszwecke verwendet.
* Wenn Sie für ein Projekt keine andere Währung angeben, geht Workfront davon aus, dass die Projektwährung die Standardwährung des Systems ist. Informationen zur Standardwährung auf Systemebene finden Sie unter [Einrichten von Wechselkursen](../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md).
* Standardmäßig haben alle Benutzer mit Volllizenz Zugriff auf Währungen und Wechselkurse. Der Workfront-Administrator muss zusätzlichen administrativen Zugriff für **Wechselkurse“ gewähren** damit Benutzende bestimmte Kurse für Projekte festlegen können.
* Die Wechselkurse in Workfront sind nicht dynamisch. Der Wert wird von einem Administrator festgelegt und muss aktualisiert werden, wenn Wechselkursänderungen auftreten.
* Wenn Sie einen Bericht erstellen, der die Währung eines Projekts widerspiegelt, werden standardmäßig alle Berichte nach der Standardwährung des Projekts gruppiert. Wenn Sie einen Bericht mit mehreren Projekten mit unterschiedlichen Wechselkursen erstellen, spiegeln alle auf das Projekt angewendeten Gruppierungen den Standardwechselkurs auf Systemebene wider. Weitere Informationen finden Sie im Artikel [Erstellen von Finanzdatenberichten mit eindeutigen Wechselkursen](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-financial-data-reports-unique-exchange-rates.md).

## Währung für ein Projekt konfigurieren

1. Wechseln Sie zu dem Projekt, in dem Sie die Standardwährung ändern möchten.

   >[!TIP]
   >
   >Stellen Sie sicher, dass das Projekt noch über keine Finanzinformationen verfügt. Stellen Sie beispielsweise sicher, dass mit dem Projekt keine geplanten Kosten oder Istkosten verknüpft sind.

1. Klicken Sie **linken Bereich auf** Projektdetails“ und navigieren Sie dann zum Bereich **Finanzen**.
1. Klicken Sie **&#x200B;**&#x200B;Feld **Währung** auf „Hinzufügen“ und wählen Sie die Währung aus, die Sie als Standardwährung für das Projekt verwenden möchten. Alle Währungen, die Ihr Workfront-Administrator für Ihre Workfront-Instanz festgelegt hat, werden angezeigt.

   ![Währung des Projekts](assets/currency-on-project-expanded-nwe.png)

1. (Bedingt) Wenn Sie eine andere Währung als die Standardwährung auswählen, die für Ihr Workfront-System festgelegt wurde, geben Sie den Kurs für die ausgewählte Währung an, da sie sich auf die Währung bezieht, die im System als Basiswährung festgelegt wurde.
1. Klicken Sie auf **Änderungen speichern**.
