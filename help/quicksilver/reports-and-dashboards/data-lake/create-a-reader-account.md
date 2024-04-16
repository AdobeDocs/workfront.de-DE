---
content-type: reference
product-area: reports and dashboards
navigation-topic: data lake
title: Erstellen eines Leserkontos (Dienstkontos) für Snowflake
description: Um auf die Daten im Workfront Data Lake zuzugreifen, müssen Sie zunächst ein Leserkonto für Snowflake erstellen.
author: Nolan
feature: Reports and Dashboards
recommendations: noDisplay, noCatalog
exl-id: 70d83a10-f926-4229-ac10-7659f2ca5e7a
source-git-commit: 912f46c87170d6b678d885ccc1fb0170526578df
workflow-type: tm+mt
source-wordcount: '564'
ht-degree: 0%

---

# Erstellen eines Leserkontos (Dienstkontos) für Snowflake

Um auf Workfront Data Lake-Daten zugreifen zu können, müssen Sie zunächst ein Leserkonto für Snowflake erstellen. Darüber hinaus müssen Sie der Zulassungsliste IPs für alle externen Tools hinzufügen, die Sie für die Verbindung mit den Daten planen.

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Abo</td> 
   <td>TBD</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Sie müssen Workfront-Administrator sein.</p></td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Leserkonto erstellen

1. Klicken Sie auf **[!UICONTROL Hauptmenü]** icon ![Hauptmenü](/help/_includes/assets/main-menu-icon.png) in der oberen rechten Ecke von Adobe Workfront oder (falls verfügbar) klicken Sie auf das **[!UICONTROL Hauptmenü]** icon ![Hauptmenü](/help/_includes/assets/main-menu-icon-left-nav.png) in der oberen linken Ecke auf **Einrichtung**.

1. Klicken Sie im linken Bereich auf **System** > **Datenzugriff**.

1. Klicks **Neue Verbindung erstellen**

1. Geben Sie in dem sich öffnenden Fenster einen Namen für Ihre Verbindung ein in **Verbindungsreferenz-Beschreibung** und einen Benutzernamen in **Verbindungsbenutzer** Klicken Sie auf **Verbindung generieren**.

   ![Leserkonto erstellen](/help/quicksilver/reports-and-dashboards/data-lake/assets/new-reader-connection.png) {width="500"}

1. A **Standardkennwort** werden sowie eine URL generiert, über die Ihre Daten über Snowflake angezeigt werden können. Sie müssen das Passwort zusammen mit dem Benutzernamen verwenden, den Sie zum ersten Mal bei Snowflake angemeldet haben, um sicherzustellen, dass Sie es sowie die URL aufzeichnen. Markieren Sie das Kästchen und klicken Sie auf **Schließen**.

   ![Standardkontonpasswort](/help/quicksilver/reports-and-dashboards/data-lake/assets/default-password-reader-account.png) {width="500"}

1. Öffnen Sie die Snowflake mithilfe eines Browsers, um von der vorherigen Etappe zur URL zu navigieren, geben Sie den ausgewählten Benutzernamen und das Standardkennwort aus dem vorherigen Schritt ein und klicken Sie dann auf **Anmelden**.

1. Nach der ersten Anmeldung werden Sie aufgefordert, ein neues Kennwort auszuwählen. Geben Sie ein Kennwort Ihrer Wahl in beide **Neues Kennwort** und **Kennwort bestätigen** Felder und klicken Sie auf **Einsenden**.

   ![Snowflake-Kennwort zurücksetzen](/help/quicksilver/reports-and-dashboards/data-lake/assets/reset-snowflake-password.png) {width="300"}

1. Sie können jetzt Ihren Benutzernamen und Ihr neues Passwort verwenden, um auf Ihren Workfront Data Lake in Snowflake oder das Geschäftsvisualisierungs-Tool Ihrer Wahl zuzugreifen.

## Hinzufügen von IPs zur Zulassungsliste

1. Klicken Sie auf **[!UICONTROL Hauptmenü]** icon ![Hauptmenü](/help/_includes/assets/main-menu-icon.png) in der oberen rechten Ecke von Adobe Workfront oder (falls verfügbar) klicken Sie auf das **[!UICONTROL Hauptmenü]** icon ![Hauptmenü](/help/_includes/assets/main-menu-icon-left-nav.png) in der oberen linken Ecke auf **Einrichtung**.

1. Klicken Sie im linken Bereich auf **System** > **Datenzugriff**.

1. Klicken Sie auf **Zulässige IPs** und klicken Sie auf die **Hinzufügen einer IP-Adresse zu Ihrer Zulassungsliste** Schaltfläche.

1. Geben Sie einen Namen für die IP-Adresse in **Beschreibung der IP-Adresse** und geben Sie die IP-Adresse für das Tool ein, das Sie in verwenden möchten **IP-Adresse** Klicken Sie auf **Hinzufügen von IP-Adresse zur Zulassungsliste**.

   ![IP-Adresse hinzufügen](/help/quicksilver/reports-and-dashboards/data-lake/assets/add-IP-allowlist.png) {width="500"}

## Reader-Konto sperren oder eine IP-Adresse aus der Zulassungsliste entfernen

1. Klicken Sie auf **[!UICONTROL Hauptmenü]** icon ![Hauptmenü](/help/_includes/assets/main-menu-icon.png) in der oberen rechten Ecke von Adobe Workfront oder (falls verfügbar) klicken Sie auf das **[!UICONTROL Hauptmenü]** icon ![Hauptmenü](/help/_includes/assets/main-menu-icon-left-nav.png) in der oberen linken Ecke auf **Einrichtung**.

1. Klicken Sie im linken Bereich auf **System** > **Datenzugriff**.

1. Klicken Sie auf das Papierkorbsymbol ![Löschsymbol](/help/quicksilver/reports-and-dashboards/data-lake/assets/delete.png) rechts neben dem Konto, das Sie widerrufen möchten.

   ODER

   Klicken Sie auf **Zulässige IPs** Registerkarte und dann auf das Papierkorbsymbol ![Löschsymbol](/help/quicksilver/reports-and-dashboards/data-lake/assets/delete.png) rechts neben der IP-Adresse, die Sie entfernen möchten.

1. Markieren Sie im sich öffnenden Fenster das zu validierende Kästchen und klicken Sie auf **Löschen**.
