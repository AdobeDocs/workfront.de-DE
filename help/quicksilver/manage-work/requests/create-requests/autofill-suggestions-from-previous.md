---
title: Automatische Vervollständigung einer Anfrage mit Daten aus vorherigen Anfragen
content-type: reference
description: Sie können KI verwenden, um Anfragefelder mithilfe von Daten aus früheren Anfragen automatisch auszufüllen.
author: Alina
feature: Get Started with Workfront
exl-id: a0cd1fbf-d3c6-454c-a85a-ceca4b1e8a7b
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/EJR8tFVdc-sYRL5kXf-Ex9WExL0hcbkhQ1ZwEmpmU-s
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: bce87dde-a4ab-44c9-8a18-ad66e4ddb377id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 314
ht-degree: 12%

---

# Automatische Vervollständigung einer Anfrage mit Daten aus vorherigen Anfragen

KI kann Ihnen dabei helfen, Anfragefelder basierend auf früheren Anfragen automatisch auszufüllen. Sie können diese Vorschläge vor dem Absenden der Anfrage genehmigen oder ablehnen.

Bei der automatischen Vervollständigung werden bereits ausgefüllte Felder nicht überschrieben.

Benutzer erhalten keine Vorschläge für Daten, auf die sie sonst keinen Zugriff hätten.

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Paket</td> 
   <td> <p>Beliebig </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td> <p>Mitwirkende oder höher</p>
   <p>Anfragende oder höher</p>
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

Weitere Informationen finden Sie unter [Zugriffsanforderungen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) in der Dokumentation zu Workfront.

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

   ODER

   Wählen **oben auf der Seite** Alle akzeptieren **oder (Alle**) aus, um alle Vorschläge zu akzeptieren oder abzulehnen.

   >[!NOTE]
   >
   >Alle nicht überprüften Vorschläge werden automatisch akzeptiert, wenn Sie die Anfrage senden.
