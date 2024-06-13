---
user-type: administrator
content-type: how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: Installieren eines Umgebungsförderungspakets
description: Die Umgebungsförderungsfunktion soll die Möglichkeit bieten, konfigurationsbezogene Objekte von einer Umgebung in eine andere zu verschieben. Erfahren Sie, wie Sie ein Umgebungsförderungspaket in einer Zielumgebung installieren.
author: Becky
feature: System Setup and Administration
role: Admin
recommendations: noDisplay, noCatalog
exl-id: fe213fe7-5bb8-479c-926b-761cbdd7ba4e
source-git-commit: b26f20b13a18c6e727fcf9e267ba9c53e5b566dc
workflow-type: tm+mt
source-wordcount: '912'
ht-degree: 0%

---

# Installieren eines Umgebungsförderungspakets

Nachdem Sie ein Paket erstellt haben, können Sie es in einer anderen Umgebung installieren.

Sie müssen ein Paket in der Umgebung installieren, in die Sie Objekte kopieren möchten **nach**. Wenn Sie beispielsweise ein Projekt in Ihrer Sandbox für benutzerdefinierte Aktualisierung konfigurieren und in Ihrer Produktionsumgebung für dieses Projekt werben, müssen Sie das Paket in Ihrer Produktionsumgebung installieren.

>[!IMPORTANT]
>
>Wenn Ihre Sandbox für benutzerdefinierte Aktualisierung aktualisiert wird, während Sie das Objekt für die Umgebungsförderung konfigurieren, geht diese Konfiguration bei der Aktualisierung verloren. Es wird empfohlen, die benutzerdefinierte Aktualisierungs-Sandbox nur dann zu aktualisieren, wenn alle ausstehenden Umgebungsförderungsobjekte und -pakete erfolgreich beworben wurden.

## Zugriffsanforderungen

Sie müssen über Folgendes verfügen:

<table>
  <tr>
   <td><strong>[!DNL Adobe Workfront] plan</strong>
   </td>
   <td> Prime oder Ultimate (nur neue Pläne)
   </td>
  </tr>
  <tr>
   <td><strong>[!DNL Adobe Workfront] Lizenzen</strong>
   </td>
   <td> [!UICONTROL Standard]
   </td>
  </tr>
   <tr>
   <td>Konfigurationen auf Zugriffsebene
   </td>
   <td>Sie müssen [!DNL Workfront] Administrator.
   </td>
  </tr>
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Voraussetzungen

Vor der Installation muss ein Umgebungs-Promotionpaket erstellt werden.

Anweisungen finden Sie unter [Erstellen oder Bearbeiten eines Umgebungs-Promotion-Pakets](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-create-package.md).

## Paketstatus für die Installation

Ein Paket muss den Status AKTIV aufweisen, damit es in Ihrer Produktionsumgebung installiert werden kann.

Es wird empfohlen, das Paket in den TESTING-Status zu verschieben und es in einer anderen Sandbox zu installieren, um das Paket zu testen.  Wenn dieser Test erfolgreich und fehlerfrei ist, verschieben Sie das Paket nach ACTIVE , um es in Ihrer Produktionsumgebung zu installieren.

So bearbeiten Sie den Status eines Pakets:

1. Wählen Sie das Paket wie unter  [Bearbeiten oder Zusammenführen eines vorhandenen Pakets](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-create-package.md#create-or-edit-an-environment-promotion-package) im Artikel Erstellen und Bearbeiten von Umgebungs-Promotion-Paketen.
1. Klicks **Paket bearbeiten**.
1. Klicks **Status**.
1. Wählen Sie den gewünschten Status aus dem Dropdownmenü aus.

Weitere Informationen zu Status finden Sie unter [Status der Umgebungsförderung](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-in-wf.md#environment-promotion-statuses) im Artikel Überblick über das Verschieben von Objekten zwischen Workfront-Umgebungen.

## Paket installieren

>[!NOTE]
>
>* Um ein Paket zu installieren, müssen Sie in der Umgebung angemeldet sein, in der Sie das Paket installieren möchten. Dies ist die Umgebung, in die Sie Objekte kopieren **nach**.

1. Gehen Sie zur Umgebung, in der Sie das Paket installieren möchten.
1. Klicken Sie auf **[!UICONTROL Hauptmenü]** icon ![Hauptmenü](/help/_includes/assets/main-menu-icon.png) in der oberen rechten Ecke von Adobe Workfront oder (falls verfügbar) klicken Sie auf das **[!UICONTROL Hauptmenü]** icon ![Hauptmenü](/help/_includes/assets/main-menu-icon-left-nav.png) in der oberen linken Ecke auf **[!UICONTROL Einrichtung]** ![Einrichtungssymbol](/help/_includes/assets/gear-icon-setup.png).
1. Auswählen **System** Wählen Sie im linken Navigationsbereich die Option **Umgebungsförderung**.
1. Wählen Sie das Paket aus der angezeigten Liste aus.
1. Wählen Sie für jedes Objekt mit einer Kollision aus, wie die Kollision gelöst werden soll.

   Um eine Kollision zu beheben, klicken Sie auf den Dropdown-Pfeil neben dem Objekttyp und wählen Sie die gewünschte Aktion aus.

   Weitere Informationen finden Sie unter [Kollisionen](#collisions) in diesem Artikel
1. Um das Paket in der neuen Umgebung bereitzustellen, klicken Sie auf **Bereitstellen** oben rechts auf dem Bildschirm.

## Kollisionen

Eine Kollision ist ein Objekt in der Zielumgebung einer Installation, das mit einem der in der Quellumgebung installierten Objekte übereinstimmt. Kollisionen werden erkannt, indem die Namen und IDs der Quellobjekte mit den Objekten in der Zielumgebung verglichen werden. Kollisionen werden auch erkannt, indem Quellobjekte mit Datensätzen zuvor installierter Objekte verglichen werden.

Wenn eine Kollision auftritt, können Sie auswählen, wie die Kollision gelöst werden soll. Kollisionen werden auf Objektebene aufgelöst.

Sie können Kollisionen anzeigen, indem Sie auf die Dropdown-Liste neben jedem Objekttyp klicken. Kollisionen werden in der Spalte Kollision angezeigt.

>[!NOTE]
>
>Möglicherweise sind Kollisionen nicht die Objekte, die Sie in Ihrer Installation überschreiben oder verwenden möchten. Es wird empfohlen, erkannte Kollisionen zu validieren, um sicherzustellen, dass die Installationsziele korrekt sind.

Um eine Kollision zu beheben, wählen Sie eine Aktion in der Spalte Aktion für Freigabe aus oder verwenden Sie die bereits angezeigte Standardaktion.

* **Erstellen mit neuem Namen**: Erstellen Sie ein neues Objekt in der Zielumgebung. Wenn das Objekt in der Zielumgebung vorhanden ist, können Sie ein neues Objekt mit einem neuen Namen erstellen. Wenn es nicht in der Zielumgebung vorhanden ist, können Sie das Objekt mit einem neuen Namen oder mit dem Namen erstellen, den das Objekt im Paket hat.
* **Vorhandene verwenden**: Das Objekt im Paket wird nicht installiert und das Objekt, das bereits in der Zielumgebung vorhanden war, bleibt unverändert.
* **Überschreiben**: Das Objekt im Paket ersetzt das vorhandene Objekt in der Zielumgebung.

  Sie können auch Objekte auswählen, die überschrieben werden sollen, selbst wenn keine Kollision erkannt wird.

  Weitere Informationen dazu, wie Überschreibungen sich auf übergeordnete und untergeordnete Objekte auswirken, finden Sie unter [Überschreiben von übergeordneten und untergeordneten Objekten](#overwriting-parent-and-child-objects) in diesem Artikel.
<!--
* Do not use: The object in the package is not installed in the target environment. If you select Do not use, an error message will appear detailing how this choice will affect other objects or fields.
-->

Die Standardwerte sind `Create new` , wenn das Objekt nicht in der Zielumgebung vorhanden ist, und `Use existing` , wenn das Objekt in der Zielumgebung vorhanden ist. Sie können zur Standardzuordnung zurückkehren, indem Sie auf **Auf Standardzuordnung zurücksetzen**.

## Überschreiben von übergeordneten und untergeordneten Objekten

Einige Objekte in Ihrem Promotion-Paket enthalten möglicherweise untergeordnete Objekte. Beispielsweise hat ein Projekt (übergeordnetes Projekt) Aufgaben (untergeordnete Elemente). Beim Überschreiben eines übergeordneten Objekts werden untergeordnete Objekte wie folgt behandelt:

* Untergeordnete Objekte, die sowohl im Paket als auch in der Zielgruppe vorhanden sind, werden im Ziel aktualisiert und dem Paket entsprechend angepasst.
* Untergeordnete Objekte, die im Paket, aber nicht im Ziel vorhanden sind, werden erstellt.
* Untergeordnete Objekte, die im Ziel, aber nicht im Paket vorhanden sind, bleiben unverändert.

Diese Funktion wirkt sich auf die folgenden übergeordneten und untergeordneten Objekte aus:

| Übergeordnetes Objekt | Untergeordnete Objekte |
|---|---|
| Projekt | Aufgabe<br>QueueDef (Queue Definition)<br>RoutingRule |
| Vorlage | TemplateTask<br>QueueDef (Queue Definition)<br>RoutingRule |
| Parameter (Feld für benutzerdefiniertes Formular) | ParameterOption (Option für benutzerdefinierte Formularfelder) |
| CalendarInfo | CalendarSection |
| QueueDef (Queue Definition) | QueueTopicGroup<br>QueueTopic |

