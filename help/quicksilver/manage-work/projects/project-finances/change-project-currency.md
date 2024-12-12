---
product-area: projects
navigation-topic: financials
title: Ändern der Projektwährung
description: Als Projektmanager können Sie ein Projekt so konfigurieren, dass eine andere Währung als die Standardwährung für Ihr Adobe Workfront-System verwendet wird. Auf diese Weise können Sie bei der Berechnung von Arbeitskosten und Einnahmen Finanzinformationen zu Ihrem Projekt in der gewünschten Währung anzeigen.
author: Lisa
feature: Work Management
exl-id: c496fe92-5c17-41a5-972b-1c063643bde3
source-git-commit: e5a87b92bf1f6c2e0485ba8a2eb73e52c422b2fc
workflow-type: tm+mt
source-wordcount: '529'
ht-degree: 0%

---

# Ändern der Projektwährung

Als Projektmanager können Sie ein Projekt so konfigurieren, dass eine andere Währung als die Standardwährung für Ihr Adobe Workfront-System verwendet wird. Auf diese Weise können Sie bei der Berechnung von Arbeitskosten und Einnahmen Finanzinformationen zu Ihrem Projekt in der gewünschten Währung anzeigen.

Bevor Sie alternative Währungen wie in diesem Abschnitt beschrieben verwenden können, muss der Workfront-Administrator zunächst mehrere Währungen aktivieren und konfigurieren, wie im Artikel [Einrichten von Wechselkursen](../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md) beschrieben.

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
   <td>
   <p>Neu: Standard</p>
   <p>oder</p>
   <p>Aktuell: Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td>Zugriff auf Projekte bearbeiten</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td>Berechtigungen für ein Projekt verwalten</td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Überlegungen beim Ändern der Währung eines Projekts in Workfront

* Sie können die Währung eines Projekts nicht ändern, wenn das Projekt finanzielle Informationen enthält.
* Die Sätze werden für Arbeitskosten, Umsatzberechnungen und in Zukunft für Berichtszwecke verwendet.
* Wenn Sie für ein Projekt keine andere Währung angeben, geht Workfront davon aus, dass die Währung des Projekts die Standardwährung des Systems ist. Informationen zur Standardwährung auf Systemebene finden Sie unter [Einrichten von Wechselkursen](../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md).
* Standardmäßig haben alle Benutzer mit voller Lizenz Zugriff auf Währungen und Wechselkurse. Der Workfront-Administrator muss zusätzlichen Administratorzugriff für **Wechselkurse** gewähren, damit Benutzer bestimmte Kurse für Projekte festlegen können.
* Die Wechselkurse in Workfront sind nicht dynamisch. Der Wert wird von einem Administrator festgelegt und muss bei Wechselkursänderungen aktualisiert werden.
* Wenn Sie einen Bericht erstellen, der die Währung eines Projekts widerspiegelt, werden alle Berichte standardmäßig nach der Standardwährung des Projekts gruppiert. Wenn Sie einen Bericht mit mehreren Projekten erstellen, die unterschiedliche Wechselkurse haben, spiegeln alle auf das Projekt angewendeten Gruppierungen den Standardwechselkurs auf Systemebene wider. Weitere Informationen finden Sie im Artikel [Erstellen von Finanzdatenberichten mit eindeutigen Wechselkursen](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-financial-data-reports-unique-exchange-rates.md).

## Währung für ein Projekt konfigurieren

1. Wechseln Sie zu dem Projekt, in dem Sie die Standardwährung ändern möchten.

   >[!TIP]
   >
   >Stellen Sie sicher, dass das Projekt nicht bereits über finanzielle Informationen verfügt. Stellen Sie beispielsweise sicher, dass mit dem Projekt keine geplanten oder tatsächlichen Kosten verbunden sind.

1. Klicken Sie im linken Bereich auf **Projektdetails** und gehen Sie dann zum Bereich **Finanzen** .
1. Klicken Sie im Feld **Währung** auf **Hinzufügen** und wählen Sie die Währung aus, die Sie als Standardwährung für das Projekt verwenden möchten. Alle Währungen, die Ihr Workfront-Administrator für Ihre Workfront-Instanz festgelegt hat, werden angezeigt.

   ![](assets/currency-on-project-expanded-nwe.png)

1. (Bedingt) Wenn Sie eine andere Währung als die für Ihr Workfront-System festgelegte Standardwährung auswählen, geben Sie den Wechselkurs für die gewählte Währung an, da dieser sich auf die Währung bezieht, die im System als Basiswährung festgelegt ist.
1. Klicken Sie auf **Änderungen speichern**.
