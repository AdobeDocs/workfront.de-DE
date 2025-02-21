---
product-area: reporting
keywords: Änderung,Inhaber,Freigegeben,Bericht,Freigeben,Ausführen,Benutzer,Zugriff,Rechte,Eingegeben,Zuletzt angezeigt,Datum,Reporting,Aktivitäten
navigation-topic: report-usage
title: Erstellen eines Berichts zu Reporting-Aktivitäten
description: Wenn Sie einen Bericht über Berichte erstellen, können Sie bestimmte Berichtsinformationen identifizieren, z. B. wenn Berichte deaktivierten Benutzern zugewiesen sind, wenn Berichte mit Zugriffsrechten eines deaktivierten Benutzers ausgeführt werden sollen, wenn Benutzer auf einen Bericht zugreifen, den Sie löschen möchten, usw.
author: Nolan
feature: Reports and Dashboards
exl-id: 3861ac81-d2e4-4dec-b9cd-96eee0b66a38
source-git-commit: 70bda5a7186abfa7e8cbd26e25a4c58583a322b4
workflow-type: tm+mt
source-wordcount: '659'
ht-degree: 0%

---

# Erstellen eines Berichts zu Reporting-Aktivitäten

Wenn Sie einen Bericht über Berichte erstellen, können Sie bestimmte Berichtsinformationen identifizieren, z. B. wenn Berichte deaktivierten Benutzern zugewiesen sind, wenn Berichte mit Zugriffsrechten eines deaktivierten Benutzers ausgeführt werden sollen, wenn Benutzer auf einen Bericht zugreifen, den Sie löschen möchten, usw.

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
   <td role="rowheader">Konfigurationen der Zugriffsebene*</td> 
   <td> <p>Zugriff auf Berichte, Dashboards, Kalender bearbeiten</p> <p>Zugriff auf Filter, Ansichten, Gruppierungen bearbeiten</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Einschränkungen in Ihrer Zugriffsebene festgelegt hat. Informationen dazu, wie Workfront-Admins Ihre Zugriffsebene ändern können, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Erstellen oder Ändern benutzerdefinierter Zugriffsebenen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Verwalten von Berechtigungen für einen Bericht</p> <p>Informationen zum Anfordern zusätzlicher Zugriffsberechtigungen finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Anfordern von Zugriffsberechtigungen für Objekte </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um herauszufinden, über welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie verfügen.

## Erstellen eines Berichts zu vorhandenen Berichten {#create-the-report-about-existing-reports}

1. Klicken Sie auf **Hauptmenü**-Symbol ![Hauptmenüsymbol](assets/main-menu-icon.png) in der rechten oberen Ecke von Adobe Workfront.
1. Klicken Sie **Berichte** und dann **Neuer Bericht**.
1. Wählen Sie **Dropdown-Menü** Neuer Bericht **, um** Bericht zu vorhandenen Berichten zu erstellen.

1. Fügen Sie auf der **Spalten (Ansicht)** die gewünschten Spalten zu Ihrem Bericht hinzu.\
   Einige der folgenden Felder können nützlich sein:

   | Feld | Beschreibung |
   |---|---|
   | **Als Benutzer ausführen: Name** | Dies ist der Benutzer, der im Feld **Diesen Bericht ausführen mit den Zugriffsrechten von:** im Bericht angegeben ist. Wenn dieser Benutzer deaktiviert ist, wird für niemanden ein Bericht angezeigt, für den der Bericht freigegeben wurde. |
   | **Freigegeben für** | Dies sind alle Entitäten, für die der Bericht freigegeben ist. |
   | **Eingegeben von** | Dies ist der Besitzer des Berichts. |
   | **Zuletzt angezeigt am** | Dies ist das Datum und die Uhrzeit, zu der der Bericht zuletzt von einer Benutzerin oder einem Benutzer angezeigt wurde. |

   {style="table-layout:auto"}

1. (Optional) So beschränken Sie Ihre Berichtsliste auf bestimmte deaktivierte Benutzende:

   1. Wählen Sie die **Filter** und klicken Sie dann auf **Filterregel hinzufügen**.

   1. Fügen Sie den Filter **Als Benutzer-ID ausführen** > **Gleich“**.

   1. Geben Sie den Namen des deaktivierten Benutzers ein, den Sie dem Filter hinzufügen möchten, und klicken Sie dann auf den Namen, wenn er in der Liste angezeigt wird.
   1. Wiederholen Sie Schritt C, bis Sie alle deaktivierten Benutzer ausgewählt haben, die Sie in den Bericht aufnehmen möchten.

1. (Optional) So beschränken Sie Ihre Berichtsliste auf terminierte Berichte:

   1. Wählen Sie die **Filter** und klicken Sie dann auf **Filterregel hinzufügen**.

   1. Fügen Sie den Filter **ID des geplanten Berichts** > **Ist nicht leer** hinzu.

1. Klicken Sie **Speichern + Schließen**, geben Sie dann einen Namen für den Bericht ein und klicken Sie auf **Bericht speichern**.

   Ihre Berichtsinformationen werden angezeigt.

1. (Optional) Exportieren Sie diesen Bericht nach Excel und speichern Sie ihn auf Ihrem Computer.\
   Informationen zum Exportieren eines Berichts finden Sie unter [Exportieren von Daten](../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md).

## Aktualisieren von Informationen zu einem Bericht

Nachdem Sie Ihren Bericht erstellt haben, können Sie Ihre Berichte nach Bedarf aktualisieren.

1. Navigieren Sie zu dem Bericht, den Sie aktualisieren möchten.
1. Führen Sie je nach der gewünschten Aktion einen der folgenden Schritte aus:

   * Aktualisieren Sie das Feld **Diesen Bericht ausführen mit den Zugriffsrechten von:** für einen aktiven Benutzer: Weitere Informationen finden Sie unter [Bericht mit den Zugriffsrechten eines anderen Benutzers ausführen und bereitstellen](../../../reports-and-dashboards/reports/creating-and-managing-reports/run-deliver-report-access-rights-another-user.md).

   * Kopie des Berichts erstellen: Weitere Informationen finden Sie unter [Erstellen einer Kopie eines Berichts](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md).
   * Löschen eines Berichts: Weitere Informationen finden Sie im Abschnitt [Erstellen einer exakten Kopie ](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md#update2) Berichts“ des Artikels [Erstellen einer Kopie eines Berichts](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md).

   * Freigeben eines Berichts: Weitere Informationen finden Sie unter [Freigeben eines Berichts in Adobe Workfront](../../../reports-and-dashboards/reports/creating-and-managing-reports/share-report.md).

1. (Bedingt) Wenn Sie die Originalberichte kopieren, verwenden Sie die Informationen aus dem Bericht, den Sie in [Erstellen eines Berichts über vorhandene Berichte](#create-the-report-about-existing-reports) erstellt haben, um die neuen Kopien für dieselben Entitäten wie die Originalberichte freizugeben.
