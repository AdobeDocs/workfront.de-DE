---
content-type: reference
product-area: reports and dashboards
navigation-topic: data connect
title: Erstellen eines Leserkontos für Snowflake
description: Um auf Data Connect-Daten zuzugreifen, müssen Sie zunächst ein Snowflake-Leserkonto erstellen.
author: Nolan
feature: Reports and Dashboards
exl-id: 70d83a10-f926-4229-ac10-7659f2ca5e7a
source-git-commit: 9cf221bda04614856a6a3670100742340fb73aee
workflow-type: tm+mt
source-wordcount: '630'
ht-degree: 2%

---

# Erstellen eines Leserkontos oder einer Verbindung für Snowflake

Um auf Data Connect-Daten zuzugreifen, müssen Sie zunächst ein Snowflake-Leserkonto (oder ein Service-Konto) für Ihr Unternehmen erstellen und dann für jeden Benutzer oder jedes Tool, auf den bzw. die Sie Zugriff auf Data Connect haben möchten, eine neue Verbindung erstellen.

Nachdem Sie eine Verbindung erstellt haben, können Sie die zugehörige URL und den Benutzernamen finden, indem Sie auf der Seite „Datenverbindung“ (Hauptmenü > Setup > System > Datenverbindung) unter der Registerkarte „Vorhandene Verbindungen“ darauf klicken.

Informationen zur Verwendung einer neu erstellten Verbindung mit einem externen Produkt finden Sie unter [Herstellen einer Verbindung mit Workfront Data Connect](/help/quicksilver/reports-and-dashboards/data-lake/share-data-externally.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen anzuzeigen. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Paket</td> 
   <td><p>Ultimate</p>
    <p>Workflow Ultimate</p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td>
   <p>Standard</p>
   <p>Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Sie müssen ein Workfront-Administrator sein</p></td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Erstellen eines Leserkontos

Sie müssen ein neues Snowflake-Leserkonto für Ihr Unternehmen erstellen, bevor Sie Verbindungen erstellen können.

>[!IMPORTANT]
>
>Dieser Vorgang darf pro Organisation nur einmal abgeschlossen werden. Wenn die **Reader-Konto erstellen** an dem unten beschriebenen Speicherort nicht vorhanden ist, wurde Ihr Leserkonto bereits erstellt.

So erstellen Sie ein Leserkonto:

1. Klicken Sie auf das **[!UICONTROL Hauptmenü]**-Symbol ![Hauptmenü](/help/_includes/assets/main-menu-icon.png) in der oberen rechten Ecke von Adobe Workfront oder (falls verfügbar) klicken Sie auf das **[!UICONTROL Hauptmenü]**-Symbol ![Hauptmenü](/help/_includes/assets/main-menu-icon-left-nav.png) in der oberen linken Ecke und klicken Sie dann auf **Setup**.

1. Klicken Sie im linken Bedienfeld auf **System** > **Datenverbindung**.

1. Klicken Sie auf **Reader-Konto erstellen**, um mit der Erstellung des Leserkontos Ihrer Organisation zu beginnen. Der Vorgang wird automatisch durchgeführt, er kann jedoch bis zu 24 Stunden dauern.

1. Nach Abschluss des Vorgangs wird ein Dialogfeld angezeigt, in dem erklärt wird, dass Ihr Leserkonto jetzt aktiv ist. Aktualisieren Sie die Browser-Seite, um auf die Schaltfläche **Neue Verbindung erstellen** zuzugreifen.

Dialogfeld für das Erstellen des Reader-Kontos![](/help/quicksilver/reports-and-dashboards/data-lake/assets/data-connect-reader-account-created.png)

## Verbindung erstellen

1. Klicken Sie auf das **[!UICONTROL Hauptmenü]**-Symbol ![Hauptmenü](/help/_includes/assets/main-menu-icon.png) in der oberen rechten Ecke von Adobe Workfront oder (falls verfügbar) klicken Sie auf das **[!UICONTROL Hauptmenü]**-Symbol ![Hauptmenü](/help/_includes/assets/main-menu-icon-left-nav.png) in der oberen linken Ecke und klicken Sie dann auf **Setup**.

1. Klicken Sie im linken Bedienfeld auf **System** > **Datenverbindung**.

1. Klicken Sie **Neue Verbindung erstellen**

1. Geben Sie im sich öffnenden Fenster in „Verbindungsreferenzbeschreibung“ einen Namen für Ihre Verbindung **und** in &quot;**-Benutzer“** klicken Sie auf **Verbindung erstellen**.

   ![Neue Verbindung erstellen](/help/quicksilver/reports-and-dashboards/data-lake/assets/new-reader-connection.png) {width="500"}

1. Es **ein** Standardkennwort) sowie eine URL generiert, über die Ihre Daten über Snowflake angezeigt werden können. Sie müssen das Kennwort zusammen mit dem Benutzernamen verwenden, den Sie zum ersten Mal für die Anmeldung bei Snowflake ausgewählt haben. Vergewissern Sie sich also, dass Sie sowohl den Benutzernamen als auch die URL aufzeichnen. Markieren Sie das Kästchen mit der Angabe, dass Sie dies getan haben, und klicken Sie dann auf **Schließen**.

   ![Standardkonto-Kennwort](/help/quicksilver/reports-and-dashboards/data-lake/assets/default-password-reader-account.png) {width="500"}

1. Öffnen Sie Snowflake mithilfe eines Browsers, um zur URL aus dem vorherigen Schritt zu navigieren, geben Sie den ausgewählten Benutzernamen und das Standardkennwort aus dem vorherigen Schritt ein und klicken Sie dann auf **Anmelden**.

1. Nach der erstmaligen erfolgreichen Anmeldung werden Sie aufgefordert, ein neues Kennwort auszuwählen. Geben Sie ein Kennwort Ihrer Wahl in die Felder **Neues Kennwort** und **Kennwort bestätigen** ein und klicken Sie dann auf **Senden**.

   ![Snowflake-Kennwort zurücksetzen](/help/quicksilver/reports-and-dashboards/data-lake/assets/reset-snowflake-password.png) {width="300"}

1. Sie können jetzt Ihren Benutzernamen und Ihr neues Passwort verwenden, um auf Ihren Data Connect Data Lake in Snowflake oder das Business-Visualisierungs-Tool Ihrer Wahl zuzugreifen.

## Widerrufen eines Leserkontos

1. Klicken Sie auf das **[!UICONTROL Hauptmenü]**-Symbol ![Hauptmenü](/help/_includes/assets/main-menu-icon.png) in der oberen rechten Ecke von Adobe Workfront oder (falls verfügbar) klicken Sie auf das **[!UICONTROL Hauptmenü]**-Symbol ![Hauptmenü](/help/_includes/assets/main-menu-icon-left-nav.png) in der oberen linken Ecke und klicken Sie dann auf **Setup**.

1. Klicken Sie im linken Bedienfeld auf **System** > **Datenzugriff**.

1. Klicken Sie auf das Papierkorb![Symbol „Löschen](/help/quicksilver/reports-and-dashboards/data-lake/assets/delete.png) rechts neben dem Konto, das Sie widerrufen möchten.

1. Markieren Sie im eingeblendeten Fenster das Kontrollkästchen zur Bestätigung und klicken Sie dann auf **Löschen**.
