---
content-type: reference
product-area: reports and dashboards
navigation-topic: data connect
title: Erstellen eines Leserkontos (Dienstkontos) für Snowflake
description: Um auf Daten in Data Connect zugreifen zu können, müssen Sie zunächst ein Snowflake-Leserkonto erstellen.
author: Nolan
feature: Reports and Dashboards
recommendations: noDisplay, noCatalog
exl-id: 70d83a10-f926-4229-ac10-7659f2ca5e7a
source-git-commit: c3e18716aa74ed91e21e542437a017586a58d0b3
workflow-type: tm+mt
source-wordcount: '496'
ht-degree: 0%

---

# Erstellen eines Leserkontos (Dienstkontos) für Snowflake

Um auf Daten in Data Connect zugreifen zu können, müssen Sie zunächst für jede neue Verbindung ein Snowflake-Leser- (oder Service-)Konto erstellen. Nachdem Sie eine Verbindung erstellt haben, können Sie die zugehörige URL und den zugehörigen Benutzernamen finden, indem Sie auf der Seite **Datenzugriff** (**Hauptmenü** > **Setup** > **System** > **Datenzugriff**) auf der Registerkarte **Vorhandene Verbindungen** klicken.

Informationen zur Verwendung einer neu erstellten Verbindung mit einem externen Produkt finden Sie unter [Herstellen einer Verbindung mit Workfront Data Connect](/help/quicksilver/reports-and-dashboards/data-lake/share-data-externally.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Abo</td> 
   <td><p>In den folgenden Plänen enthalten:</p>
    <ul>
        <li>Ultimativ</li> 
    </ul>    
   <p>Kann als Zusatzprodukt zu den folgenden Plänen erworben werden:</p> 
    <ul>
        <li>Auswählen</li> 
        <li>Erstklassig</li>
    </ul> 
    <p>Workfront Data Connect ist nicht für ältere Workfront-Pläne verfügbar.</p> 
   </td> </td> 
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

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Leserkonto erstellen

1. Klicken Sie auf das Symbol **[!UICONTROL Hauptmenü]** ![Hauptmenü](/help/_includes/assets/main-menu-icon.png) oben rechts in Adobe Workfront oder (falls verfügbar) auf das Symbol **[!UICONTROL Hauptmenü]**, das Symbol ![Hauptmenü](/help/_includes/assets/main-menu-icon-left-nav.png) oben links und klicken Sie dann auf **Setup**.

1. Klicken Sie im linken Bereich auf **System** > **Datenzugriff**.

1. Klicken Sie auf **Neue Verbindung erstellen**

1. Geben Sie im sich öffnenden Fenster in **Verbindungsreferenz-Beschreibung** einen Namen für Ihre Verbindung und in **Verbindungsbenutzer** einen Benutzernamen ein und klicken Sie dann auf **Verbindung erzeugen**.

   ![Leserkonto erstellen](/help/quicksilver/reports-and-dashboards/data-lake/assets/new-reader-connection.png) {width="500"}

1. Es wird ein **Standardkennwort** sowie eine URL generiert, über die Ihre Daten über Snowflake angezeigt werden können. Sie müssen das Passwort zusammen mit dem Benutzernamen verwenden, den Sie zum ersten Mal bei Snowflake angemeldet haben, um sicherzustellen, dass Sie es sowie die URL aufzeichnen. Markieren Sie das Kästchen, wenn Sie dies getan haben, und klicken Sie dann auf **Schließen**.

   ![Standardkennwort des Kontos](/help/quicksilver/reports-and-dashboards/data-lake/assets/default-password-reader-account.png) {width="500"}

1. Öffnen Sie die Snowflake mithilfe eines Browsers, um von der vorherigen Etappe zur URL zu navigieren, geben Sie den ausgewählten Benutzernamen und das Standardkennwort aus dem vorherigen Schritt ein und klicken Sie dann auf **Anmelden**.

1. Nach der ersten Anmeldung werden Sie aufgefordert, ein neues Kennwort auszuwählen. Geben Sie in die Felder **Neues Kennwort** und **Kennwort bestätigen** ein Kennwort Ihrer Wahl ein und klicken Sie dann auf **Senden**.

   ![Snowflake-Kennwort zurücksetzen](/help/quicksilver/reports-and-dashboards/data-lake/assets/reset-snowflake-password.png) {width="300"}

1. Sie können jetzt Ihren Benutzernamen und Ihr neues Kennwort verwenden, um auf Ihren Data Connect Data Lake in der Snowflake oder das Geschäftsvisualisierungs-Tool Ihrer Wahl zuzugreifen.

## Leserkonto sperren

1. Klicken Sie auf das Symbol **[!UICONTROL Hauptmenü]** ![Hauptmenü](/help/_includes/assets/main-menu-icon.png) oben rechts in Adobe Workfront oder (falls verfügbar) auf das Symbol **[!UICONTROL Hauptmenü]**, das Symbol ![Hauptmenü](/help/_includes/assets/main-menu-icon-left-nav.png) oben links und klicken Sie dann auf **Setup**.

1. Klicken Sie im linken Bereich auf **System** > **Datenzugriff**.

1. Klicken Sie auf das Papierkorbsymbol ![Löschsymbol](/help/quicksilver/reports-and-dashboards/data-lake/assets/delete.png) rechts neben dem Konto, das Sie widerrufen möchten.

1. Aktivieren Sie im sich öffnenden Fenster das Kontrollkästchen zur Bestätigung und klicken Sie auf **Löschen**.
