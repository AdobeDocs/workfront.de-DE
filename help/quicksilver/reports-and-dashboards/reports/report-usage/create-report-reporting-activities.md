---
product-area: reporting
keywords: change,owner,shared,report,share,run,user,access,rights,red,last,displayed,date,reporting,activities
navigation-topic: report-usage
title: Erstellen eines Berichts über Berichtsaktivitäten
description: Wenn Sie einen Bericht zu Berichten erstellen, können Sie spezifische Berichtinformationen identifizieren, z. B. wenn Berichte deaktivierten Benutzern zugewiesen werden, wenn Berichte mit Zugriffsrechten eines deaktivierten Benutzers ausgeführt werden, wenn Benutzer auf einen Bericht zugreifen, den Sie löschen möchten, usw.
author: Nolan
feature: Reports and Dashboards
exl-id: 3861ac81-d2e4-4dec-b9cd-96eee0b66a38
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '656'
ht-degree: 0%

---

# Erstellen eines Berichts über Berichtsaktivitäten

Wenn Sie einen Bericht zu Berichten erstellen, können Sie spezifische Berichtinformationen identifizieren, z. B. wenn Berichte deaktivierten Benutzern zugewiesen werden, wenn Berichte mit Zugriffsrechten eines deaktivierten Benutzers ausgeführt werden, wenn Benutzer auf einen Bericht zugreifen, den Sie löschen möchten, usw.

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Alle</p> </td> 
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
   <td> <p>Berechtigungen für einen Bericht verwalten</p> <p>Weitere Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Anfordern des Zugriffs auf Objekte </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Erstellen eines Berichts über vorhandene Berichte {#create-the-report-about-existing-reports}

1. Klicken Sie oben rechts in Adobe Workfront auf das Symbol **Hauptmenü** ![](assets/main-menu-icon.png).
1. Klicken Sie auf **Berichte** und dann auf **Neuer Bericht**.
1. Wählen Sie im Dropdownmenü **Neuer Bericht** die Option **Bericht** aus, um einen Bericht zu vorhandenen Berichten zu erstellen.

1. Fügen Sie auf der Registerkarte **Spalten (Ansicht)** die gewünschten Spalten in Ihren Bericht ein.\
   Einige der folgenden Felder können nützlich sein:

   | Feld | Beschreibung |
   |---|---|
   | **Als Benutzer ausführen: Name** | Dies ist der Benutzer, der im Feld **Diesen Bericht ausführen mit den Zugriffsrechten von:** im Bericht angegeben ist. Wenn dieser Benutzer deaktiviert ist, wird für niemanden, für den der Bericht freigegeben ist, ein Bericht angezeigt. |
   | **Für** freigegeben | Dies sind alle Entitäten, für die der Bericht freigegeben ist. |
   | **eingegeben von** | Dies ist der Eigentümer des Berichts. |
   | **Datum der letzten Anzeige** | Dies ist das Datum und die Uhrzeit, zu der der Bericht zuletzt von einem Benutzer angezeigt wurde. |

   {style="table-layout:auto"}

1. (Optional) So beschränken Sie Ihre Berichtsliste auf bestimmte deaktivierte Benutzer:

   1. Wählen Sie die Registerkarte **Filter** und klicken Sie dann auf **Filterregel hinzufügen**.

   1. Fügen Sie den Filter **Als Benutzer-ID ausführen** > **Gleich** hinzu.

   1. Geben Sie den Namen des deaktivierten Benutzers ein, den Sie dem Filter hinzufügen möchten, und klicken Sie dann auf den Namen, wenn er in der Liste angezeigt wird.
   1. Wiederholen Sie Schritt C, bis Sie alle deaktivierten Benutzer ausgewählt haben, die Sie in den Bericht aufnehmen möchten.

1. (Optional) So beschränken Sie Ihre Berichtliste auf terminierte Berichte:

   1. Wählen Sie die Registerkarte **Filter** und klicken Sie dann auf **Filterregel hinzufügen**.

   1. Fügen Sie den Filter **Kennung des terminierten Berichts** > **ist nicht leer** hinzu.

1. Klicken Sie auf **Speichern + Schließen**, geben Sie einen Namen für den Bericht ein und klicken Sie auf **Bericht speichern**.

   Ihre Berichtinformationen werden angezeigt.

1. (Optional) Exportieren Sie diesen Bericht in Excel und speichern Sie ihn auf Ihrem Computer.\
   Informationen zum Exportieren eines Berichts finden Sie unter [Daten exportieren](../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md).

## Berichtinformationen aktualisieren

Nach der Erstellung Ihres Berichts können Sie Ihre Berichte nach Bedarf aktualisieren.

1. Markieren Sie den Bericht, den Sie aktualisieren möchten.
1. Führen Sie je nach der gewünschten Aktion einen der folgenden Schritte aus:

   * Aktualisieren Sie das Feld **Diesen Bericht ausführen mit dem Feld Zugriffsrechte von:** für einen aktiven Benutzer: Weitere Informationen finden Sie unter [Ausführen und Bereitstellen eines Berichts mit den Zugriffsrechten eines anderen Benutzers](../../../reports-and-dashboards/reports/creating-and-managing-reports/run-deliver-report-access-rights-another-user.md).

   * Erstellen Sie eine Kopie des Berichts: Weitere Informationen finden Sie unter [Erstellen einer Kopie eines Berichts](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md).
   * Einen Bericht löschen: Weitere Informationen finden Sie im Abschnitt [Erstellen einer exakten Kopie eines Berichts](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md#update2) des Artikels [Erstellen einer Kopie eines Berichts](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md) .

   * Berichtfreigabe: Weitere Informationen finden Sie unter [Berichtfreigabe in Adobe Workfront](../../../reports-and-dashboards/reports/creating-and-managing-reports/share-report.md).

1. (Bedingt) Wenn Sie die Originalberichte kopieren, verwenden Sie die Informationen aus dem Bericht, den Sie in [Bericht über vorhandene Berichte erstellen](#create-the-report-about-existing-reports) erstellt haben, um die neuen Kopien für dieselben Entitäten wie die Originalberichte freizugeben.
