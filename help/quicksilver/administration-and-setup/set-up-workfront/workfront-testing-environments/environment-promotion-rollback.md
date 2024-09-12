---
user-type: administrator
content-type: how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: Zurücksetzen eines Umgebungs-Promotion-Pakets
description: Die Umgebungsförderungsfunktion soll die Möglichkeit bieten, konfigurationsbezogene Objekte von einer Umgebung in eine andere zu verschieben. Erfahren Sie, wie Sie ein installiertes Promotion-Paket aus einer Zielumgebung zurücksetzen.
author: Becky
feature: System Setup and Administration
role: Admin
recommendations: noDisplay, noCatalog
exl-id: 70f7e2a8-bb27-4546-afb7-53e0eec30bf1
source-git-commit: 7e15301dae4b761d19c85a3581bfdb4540ed40fd
workflow-type: tm+mt
source-wordcount: '397'
ht-degree: 1%

---

# Zurücksetzen eines Umgebungs-Promotion-Pakets



Nachdem Sie ein Paket installiert haben, können Sie es zurücksetzen. Dadurch werden die Änderungen entfernt, die das Paket in der Zielumgebung vorgenommen hat, und die betroffenen Objekte in ihren vorherigen Konfigurationen wiederhergestellt.

Sie können ein Promotion-Paket innerhalb von 24 Stunden nach seiner Installation zurücksetzen. Nach 24 Stunden ist die Rollback-Funktion für diese Installation nicht mehr verfügbar.

## Zugriffsanforderungen

Sie müssen über Folgendes verfügen:

<table>
  <tr>
   <td><strong>[!DNL Adobe Workfront] plan</strong>
   </td>
   <td> <p>Neu: Prime oder Ultimate</p><p>Oder</p><p>Aktuell: Nicht verfügbar</p>
   </td>
  </tr>
  <tr>
   <td><strong>[!DNL Adobe Workfront] licenses</strong>
   </td>
   <td> <p>[!UICONTROL Standard]</p><p>Oder</p><p>Aktuell: Nicht verfügbar</p>
   </td>
  </tr>
   <tr>
   <td>Konfigurationen auf Zugriffsebene
   </td>
   <td>Sie müssen ein [!DNL Workfront] -Administrator sein.
   </td>
  </tr>
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Voraussetzungen

* Ein Umgebungsförderungspaket muss installiert sein, bevor es zurückgesetzt werden kann.

  Anweisungen finden Sie unter [Installieren eines Umgebungsförderungspakets](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-install-package.md).


## Bestimmen, ob ein Rollback für eine bestimmte Paketbereitstellung möglich ist

Beachten Sie Folgendes, um festzustellen, ob ein bestimmter Paketeinsatz zurückgesetzt werden kann:

* Es müssen weniger als 24 Stunden vergangen sein, seit das Paket installiert wurde.
* Nur die neueste Paketbereitstellung kann zurückgesetzt werden.
* Eine fehlgeschlagene Bereitstellung kann zurückgesetzt werden.
* Rollbacks können nicht zurückgesetzt werden.


## Zurücksetzen eines installierten Umgebungs-Promotion-Pakets

1. Wechseln Sie zur Umgebung, in der das Paket installiert wurde.
1. Klicken Sie auf das Symbol **[!UICONTROL Hauptmenü]** ![Hauptmenü](/help/_includes/assets/main-menu-icon.png) oben rechts in Adobe Workfront oder (falls verfügbar) auf das Symbol **[!UICONTROL Hauptmenü]** (6}Hauptmenü](/help/_includes/assets/main-menu-icon-left-nav.png) oben links und klicken Sie dann auf das Symbol **[!UICONTROL Setup]** ![Setup](/help/_includes/assets/gear-icon-setup.png).![
1. Wählen Sie im linken Navigationsbereich **Umgebungsförderung** aus.
1. Wählen Sie das Paket aus, für das Sie einen Rollback durchführen möchten, und klicken Sie auf **Bereitstellungen**.
1. Bewegen Sie den Mauszeiger über die Bereitstellung (Installation), die Sie wiederherstellen möchten, und klicken Sie dann auf &quot;Zurücksetzen&quot;, wenn sie rechts neben der Zeile der Bereitstellung angezeigt wird.

   Oder

   Klicken Sie auf die Bereitstellung, die Sie zurücksetzen möchten, und klicken Sie dann oben rechts im Bildschirm auf **Paket zurücksetzen** .

   >[!IMPORTANT]
   >
   >Die Bereitstellung muss weniger als 24 Stunden vor der Zurücksetzung erfolgen. Installationen, die älter als 24 Stunden sind, können nicht zurückgesetzt werden.

1. (Optional) Zeigen Sie im Bereich Rollback-Vorschau die Änderungen an, die auftreten, wenn die Bereitstellung zurückgesetzt wird.
1. Klicken Sie oben rechts im Bildschirm auf **Zurückrollen** .
