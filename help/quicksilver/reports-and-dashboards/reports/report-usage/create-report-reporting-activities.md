---
product-area: reporting
keywords: change,owner,shared,report,share,run,user,access,rights,red,last,displayed,date,reporting,activities
navigation-topic: report-usage
title: Erstellen eines Berichts über Berichtsaktivitäten
description: Wenn Sie einen Bericht zu Berichten erstellen, können Sie spezifische Berichtinformationen identifizieren, z. B. wenn Berichte deaktivierten Benutzern zugewiesen werden, wenn Berichte mit Zugriffsrechten eines deaktivierten Benutzers ausgeführt werden, wenn Benutzer auf einen zu löschenden Bericht zugreifen usw.
author: Nolan
feature: Reports and Dashboards
exl-id: 3861ac81-d2e4-4dec-b9cd-96eee0b66a38
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '673'
ht-degree: 2%

---

# Erstellen eines Berichts über Berichtsaktivitäten

Wenn Sie einen Bericht zu Berichten erstellen, können Sie spezifische Berichtinformationen identifizieren, z. B. wenn Berichte deaktivierten Benutzern zugewiesen werden, wenn Berichte mit Zugriffsrechten eines deaktivierten Benutzers ausgeführt werden, wenn Benutzer auf einen zu löschenden Bericht zugreifen usw.

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
   <td> <p>Zugriff auf Berichte, Dashboards und Kalender bearbeiten</p> <p>Zugriff auf Filter, Ansichten, Gruppierungen bearbeiten</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Berechtigungen für einen Bericht verwalten</p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Erstellen eines Berichts über vorhandene Berichte {#create-the-report-about-existing-reports}

1. Klicken Sie auf **Hauptmenü** icon ![](assets/main-menu-icon.png) in der rechten oberen Ecke von Adobe Workfront.
1. Klicken **Berichte**, dann **Neuer Bericht**.
1. Im **Neuer Bericht** Dropdown-Menü auswählen **Bericht** , um einen Bericht zu vorhandenen Berichten zu erstellen.

1. Im **Spalten (Ansicht)** hinzufügen, fügen Sie die gewünschten Spalten in Ihren Bericht ein.\
   Einige der folgenden Felder können nützlich sein:

   | Feld | Beschreibung |
   |---|---|
   | **Als Benutzer ausführen: Name** | Dies ist der Benutzer, der in der Variablen **Führen Sie diesen Bericht mit den Zugriffsrechten von aus:** im Bericht ein. Wenn dieser Benutzer deaktiviert ist, wird für niemanden, für den der Bericht freigegeben ist, ein Bericht angezeigt. |
   | **Freigegeben für** | Dies sind alle Entitäten, für die der Bericht freigegeben ist. |
   | **Eingegeben von** | Dies ist der Eigentümer des Berichts. |
   | **Zuletzt angezeigt am** | Dies ist das Datum und die Uhrzeit, zu der der Bericht zuletzt von einem Benutzer angezeigt wurde. |

   {style=&quot;table-layout:auto&quot;}

1. (Optional) So beschränken Sie Ihre Berichtsliste auf bestimmte deaktivierte Benutzer:

   1. Wählen Sie die **Filter** Registerkarte und klicken Sie dann auf **Filterregel hinzufügen**.

   1. Filter hinzufügen **Als Benutzer-ID ausführen** > **Gleich**.

   1. Geben Sie den Namen des deaktivierten Benutzers ein, den Sie dem Filter hinzufügen möchten, und klicken Sie dann auf den Namen, wenn er in der Liste angezeigt wird.
   1. Wiederholen Sie Schritt C, bis Sie alle deaktivierten Benutzer ausgewählt haben, die Sie in den Bericht aufnehmen möchten.

1. (Optional) So beschränken Sie Ihre Berichtliste auf terminierte Berichte:

   1. Wählen Sie die **Filter** Registerkarte und klicken Sie dann auf **Filterregel hinzufügen**.

   1. Filter hinzufügen **Kennung des terminierten Berichts** > **Ist nicht leer**.

1. Klicken **Speichern und schließen**, geben Sie einen Namen für den Bericht ein und klicken Sie auf **Bericht speichern**.

   Ihre Berichtinformationen werden angezeigt.

1. (Optional) Exportieren Sie diesen Bericht in Excel und speichern Sie ihn auf Ihrem Computer.\
   Informationen zum Exportieren eines Berichts finden Sie unter [Daten exportieren](../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md).

## Berichtinformationen aktualisieren

Nach der Erstellung Ihres Berichts können Sie Ihre Berichte nach Bedarf aktualisieren.

1. Markieren Sie den Bericht, den Sie aktualisieren möchten.
1. Führen Sie je nach der gewünschten Aktion einen der folgenden Schritte aus:

   * Aktualisieren Sie die **Führen Sie diesen Bericht mit den Zugriffsrechten von aus:** -Feld für einen aktiven Benutzer: Weitere Informationen finden Sie unter [Einen Bericht mit Zugriffsrechten für einen anderen Benutzer ausführen und bereitstellen](../../../reports-and-dashboards/reports/creating-and-managing-reports/run-deliver-report-access-rights-another-user.md).

   * Erstellen Sie eine Kopie des Berichts: Weitere Informationen finden Sie unter [Berichtkopie erstellen](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md).
   * Einen Bericht löschen: Weitere Informationen finden Sie unter [Erstellen einer exakten Kopie eines Berichts](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md#update2) Abschnitt des Artikels [Berichtkopie erstellen](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md).

   * Bericht freigeben: Weitere Informationen finden Sie unter [Bericht in Adobe Workfront freigeben](../../../reports-and-dashboards/reports/creating-and-managing-reports/share-report.md).

1. (Bedingt) Wenn Sie die ursprünglichen Berichte kopieren, verwenden Sie die Informationen aus dem Bericht, den Sie in [Erstellen eines Berichts über vorhandene Berichte](#create-the-report-about-existing-reports) , um die neuen Kopien für dieselben Entitäten wie die Originalberichte freizugeben.
