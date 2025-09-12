---
title: Automatische Vervollständigung einer Anfrage mit Daten aus vorherigen Anfragen
content-type: reference
description: Sie können KI verwenden, um Anfragefelder mithilfe von Daten aus früheren Anfragen automatisch auszufüllen.
author: Becky
feature: Get Started with Workfront
exl-id: a0cd1fbf-d3c6-454c-a85a-ceca4b1e8a7b
source-git-commit: 1c2e382908ed8fead7c2222e8d46988656df29c4
workflow-type: tm+mt
source-wordcount: '350'
ht-degree: 0%

---

# Automatische Vervollständigung einer Anfrage mit Daten aus vorherigen Anfragen

>[!NOTE]
>
>* Diese Funktion wird als offene Beta-Version nach dem folgenden Zeitplan verfügbar sein:
>
>   * Monatliche Version: 11. September 2025
>   * Vierteljährliche Veröffentlichung: 16. Oktober 2025

KI kann Ihnen dabei helfen, Anfragefelder basierend auf früheren Anfragen automatisch auszufüllen. Sie können diese Vorschläge vor dem Absenden der Anfrage genehmigen oder ablehnen.

Bei der automatischen Vervollständigung werden bereits ausgefüllte Felder nicht überschrieben.

Benutzer erhalten keine Vorschläge für Daten, auf die sie sonst keinen Zugriff hätten.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan</td> 
   <td> <p>Beliebig </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td> <p>Neu: Mitwirkender oder höher</p>
   Oder
   <p>Aktuell: Anforderung oder höher</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriff auf Anfragen bearbeiten</p>  </td> 
  </tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td><p>Zugriff zum Hinzufügen von Anfragen zu einer Anfragewarteschlange</p> <p>Anzeigen von oder höheren Berechtigungen für die vorhandene Anfrage</p> <p>Informationen zum Einrichten einer Anfrage-Warteschlange finden Sie unter <a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">Erstellen einer Anfrage-Warteschlange</a>. </p> </td> 
  <tr>
  </tr>
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Vorschläge beim Ausfüllen des Formulars einholen

Beim automatischen Ausfüllen des Formulars können Werte aus den Feldern vorgeschlagen werden. Wenn Sie Werte in die Anfragefelder eingeben, vergleicht Workfront diese Werte mit vorherigen Anfragen. Wenn der eingegebene Wert eng mit anderen Feldwerten in ähnlichen Kontexten in früheren Anfragen korreliert, schlägt Workfront diese Werte vor.

Wenn beispielsweise eine Klinik immer denselben Abrechnungscode verwendet, schlägt Workfront vor, dass sich der Abrechnungscode bei Eingabe des Kliniknamens im entsprechenden Feld befindet.

So verwenden Sie Vorschläge basierend auf früheren Anfragen:

1. Erstellen Sie eine Anfrage.

   Anweisungen finden Sie unter [Erstellen und Senden von Anfragen](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md).

1. Felder ausfüllen.

   Beim Ausfüllen von Feldern können andere Felder Vorschläge anzeigen.

1. Wählen Sie für jeden Feldvorschlag **Feld** Akzeptieren“ oder **Ablehnen** aus.

   ![Vorschlag annehmen oder ablehnen](assets/accept-reject-suggestion.png)

   Oder

   Wählen **oben auf der Seite** Alle akzeptieren **oder (Alle**) aus, um alle Vorschläge zu akzeptieren oder abzulehnen.

   >[!NOTE]
   >
   >Alle nicht überprüften Vorschläge werden automatisch akzeptiert, wenn Sie die Anfrage senden.
