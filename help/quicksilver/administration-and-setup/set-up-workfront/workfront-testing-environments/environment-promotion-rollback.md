---
user-type: administrator
content-type: how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: Zurücksetzen eines Umgebungs-Promotion-Pakets
description: Die Funktion zum Hochstufen der Umgebung soll die Möglichkeit bieten, konfigurationsbezogene Objekte von einer Umgebung in eine andere zu verschieben. Erfahren Sie, wie Sie ein installiertes Promotion-Paket aus einer Zielumgebung zurücksetzen.
author: Becky
feature: System Setup and Administration
role: Admin
recommendations: noDisplay, noCatalog
exl-id: 70f7e2a8-bb27-4546-afb7-53e0eec30bf1
source-git-commit: 7ca27795ec115a112acb55113bfade4a5fee15ad
workflow-type: tm+mt
source-wordcount: '384'
ht-degree: 0%

---

# Zurücksetzen eines Umgebungs-Promotion-Pakets



Nachdem Sie ein Paket installiert haben, können Sie es zurücksetzen. Dadurch werden die Änderungen entfernt, die das Paket in der Zielumgebung vorgenommen hat, und die betroffenen Objekte auf ihre vorherigen Konfigurationen zurückgesetzt.

Sie können ein Promotion-Paket innerhalb von 24 Stunden nach seiner Installation zurücksetzen. Nach 24 Stunden ist die Rollback-Funktion für diese Installation nicht mehr verfügbar.

## Zugriffsanforderungen

Sie müssen über Folgendes verfügen:

<table>
  <tr>
   <td>Adobe Workfront-Paket
   </td>
   <td> <p>Prime oder Ultimate</p>
   </td>
  </tr>
  <tr>
   <td><strong>Workfront-Lizenzen</strong>
   </td>
   <td> <p>Standard</p>&gt;
   </td>
  </tr>
   <tr>
   <td>Konfigurationen der Zugriffsebene
   </td>
   <td><p>Sie müssen ein Workfront-Administrator sein.</p>
   </td>
  </tr>
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Voraussetzungen

* Ein Umgebungs-Promotion-Paket muss installiert werden, bevor es zurückgesetzt werden kann.

  Anweisungen finden Sie unter [Installieren eines Umgebungs-Promotion-Pakets](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-install-package.md).


## Ermitteln, ob eine bestimmte Paketbereitstellung zurückgesetzt werden kann

Um herauszufinden, ob eine bestimmte Paketbereitstellung zurückgesetzt werden kann, beachten Sie Folgendes:

* Seit der Installation des Pakets müssen weniger als 24 Stunden vergangen sein.
* Nur die neueste Paketbereitstellung kann zurückgesetzt werden.
* Eine fehlgeschlagene Bereitstellung kann zurückgesetzt werden.
* Rollbacks können nicht zurückgesetzt werden.


## Zurücksetzen eines installierten Umgebungs-Promotion-Pakets

1. Wechseln Sie zur Umgebung, in der das Paket installiert wurde.
1. Klicken Sie auf das **[!UICONTROL Hauptmenü]**-Symbol ![Hauptmenü](/help/_includes/assets/main-menu-icon.png) in der oberen rechten Ecke von Adobe Workfront oder (falls verfügbar) klicken Sie auf das **[!UICONTROL Hauptmenü]**-Symbol ![Hauptmenü](/help/_includes/assets/main-menu-icon-left-nav.png) in der oberen linken Ecke und klicken Sie dann auf **&#x200B;**&#x200B;Setup![Setup-Symbol](/help/_includes/assets/gear-icon-setup.png).
1. Wählen **im** Navigationsbereich die Option „Umgebungsförderung“ aus.
1. Wählen Sie das Paket aus, das Sie zurücksetzen möchten, und klicken Sie auf **Bereitstellungen**.
1. Bewegen Sie den Mauszeiger über die Bereitstellung (Installation), die Sie zurücksetzen möchten, und klicken Sie dann auf Zurücksetzen , wenn sie rechts neben der Zeile dieser Bereitstellung angezeigt wird.

   Oder

   Klicken Sie auf die Bereitstellung, für die Sie ein Rollback durchführen möchten, und klicken Sie **Paket zurücksetzen** in der oberen rechten Ecke des Bildschirms.

   >[!IMPORTANT]
   >
   >Die Bereitstellung muss weniger als 24 Stunden vor dem Rollback erfolgen. Installationen, die älter als 24 Stunden sind, können nicht zurückgesetzt werden.

1. (Optional) Zeigen Sie im Bereich Vorschau für Rollback die Änderungen an, die auftreten, wenn die Bereitstellung zurückgesetzt wird.
1. Klicken **oben rechts** Bildschirm auf „Zurücksetzen“.
