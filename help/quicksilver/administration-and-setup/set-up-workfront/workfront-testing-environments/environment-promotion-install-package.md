---
user-type: administrator
content-type: how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: Installieren eines Umgebungs-Promotion-Pakets
description: Die Funktion zum Hochstufen der Umgebung soll die Möglichkeit bieten, konfigurationsbezogene Objekte von einer Umgebung in eine andere zu verschieben. Erfahren Sie, wie Sie ein Umgebungs-Promotion-Paket in einer Zielumgebung installieren.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: fe213fe7-5bb8-479c-926b-761cbdd7ba4e
source-git-commit: 7ca27795ec115a112acb55113bfade4a5fee15ad
workflow-type: tm+mt
source-wordcount: '946'
ht-degree: 0%

---

# Installieren eines Umgebungs-Promotion-Pakets

Nachdem Sie ein Paket erstellt haben, können Sie es in einer anderen Umgebung installieren.

Sie müssen ein Paket in der Umgebung installieren, in die Sie Objekte (**)** möchten. Wenn Sie beispielsweise ein Projekt in Ihrer benutzerdefinierten Aktualisierungs-Sandbox-Umgebung konfigurieren und es in Ihre Produktionsumgebung übertragen, müssen Sie das Paket in Ihrer Produktionsumgebung installieren.

>[!IMPORTANT]
>
>* Wenn Ihre benutzerdefinierte Aktualisierungs-Sandbox aktualisiert wird, während Sie das Objekt für die Umgebungsweiterleitung konfigurieren, geht diese Konfiguration bei der Aktualisierung verloren. Es wird empfohlen, die benutzerdefinierte Aktualisierungs-Sandbox nur zu aktualisieren, wenn alle ausstehenden Objekte und Pakete zur Umgebungsförderung erfolgreich beworben wurden.
>* Objekte, die in der Zielumgebung als Teil der Paketinstallation erstellt wurden **haben nicht** ID wie das Objekt in der ursprünglichen Umgebung. Das liegt daran, dass IDs vom System zugewiesen werden, wenn Objekte erstellt werden.

## Zugriffsanforderungen

Sie müssen über Folgendes verfügen:

<table>
  <tr>
   <td>Adobe Workfront-Paket
   </td>
   <td> <p>Prime oder Ultimate</p>
   </td>
  </tr>
  <tr>
   <td><strong>Workfront-Lizenzen</strong>
   </td>
   <td> <p>Standard</p>&gt;
   </td>
  </tr>
   <tr>
   <td>Konfigurationen der Zugriffsebene
   </td>
   <td><p>Sie müssen ein Workfront-Administrator sein.</p>
   </td>
  </tr>
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Voraussetzungen

Ein Umgebungs-Promotion-Paket muss erstellt werden, bevor es installiert werden kann.

Anweisungen finden Sie unter [Erstellen oder Bearbeiten eines Umgebungs-Promotion-Pakets](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-create-package.md).

## Paketstatus für die Installation

Ein Paket muss den Status AKTIV haben, damit es in Ihrer Produktionsumgebung installiert werden kann.

Es wird empfohlen, das Paket in den Status TESTEN zu versetzen und in einer anderen Sandbox zu installieren, um das Paket zu testen.  Wenn dieser Test erfolgreich und fehlerfrei durchgeführt werden kann, verschieben Sie das Paket nach ACTIVE, um es in Ihrer Produktionsumgebung zu installieren.

So bearbeiten Sie den Status eines Pakets:

1. Wählen Sie das Paket aus, wie [&#x200B; im Artikel Erstellen und Bearbeiten &#x200B;](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-create-package.md#create-or-edit-an-environment-promotion-package) Promotion-Paketen für Umgebungen unter „Bearbeiten oder Zusammenstellen eines vorhandenen Pakets“ beschrieben.
1. Klicken Sie **Paket bearbeiten**.
1. Klicken Sie **Status**.
1. Wählen Sie den gewünschten Status aus dem Dropdown-Menü aus.

Weitere Informationen zum Status finden Sie [Umgebungsförderungsstatus](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-in-wf.md#environment-promotion-statuses) im Artikel Übersicht über das Verschieben von Objekten zwischen Workfront-Umgebungen.

## Package installieren

>[!NOTE]
>
>* Um ein Paket zu installieren, müssen Sie bei der Umgebung angemeldet sein, in der Sie das Paket installieren möchten. Dies ist die Umgebung, in die Sie Objekte **kopieren**.

1. Wechseln Sie zu der Umgebung, in der Sie das Paket installieren möchten.
1. Klicken Sie auf das **[!UICONTROL Hauptmenü]**-Symbol ![Hauptmenü](/help/_includes/assets/main-menu-icon.png) in der oberen rechten Ecke von Adobe Workfront oder (falls verfügbar) klicken Sie auf das **[!UICONTROL Hauptmenü]**-Symbol ![Hauptmenü](/help/_includes/assets/main-menu-icon-left-nav.png) in der oberen linken Ecke und klicken Sie dann auf **&#x200B;**&#x200B;Setup![Setup-Symbol](/help/_includes/assets/gear-icon-setup.png).
1. Wählen Sie **linken Navigationsbereich die Option** System“ und dann **Umgebungs-Promotion** aus.
1. Wählen Sie das Paket aus der angezeigten Liste aus.
1. Wählen Sie für jedes Objekt, das eine Kollision aufweist, die Art und Weise aus, wie die Kollision aufgelöst werden soll.

   Um eine Kollision zu beheben, klicken Sie auf den Dropdown-Pfeil neben dem Objekttyp und wählen Sie die gewünschte Aktion aus.

   Weitere Informationen finden Sie unter [Konflikte](#collisions) in diesem Artikel
1. Um das Paket in der neuen Umgebung bereitzustellen, klicken **oben** auf dem Bildschirm auf „Bereitstellen“.

## Kollisionen

Eine Kollision ist ein Objekt, das in der Zielumgebung einer Installation gefunden wird und mit einem der Objekte übereinstimmt, die aus der Quellumgebung installiert werden. Kollisionen werden erkannt, indem die Namen und IDs der Quellobjekte mit Objekten in der Zielumgebung verglichen werden. Kollisionen werden auch erkannt, indem Quellobjekte mit Datensätzen zuvor installierter Objekte verglichen werden.

Bei einer Kollision können Sie auswählen, wie die Kollision aufgelöst werden soll. Kollisionen werden auf Objektebene aufgelöst.

Sie können Kollisionen anzeigen, indem Sie auf die Dropdown-Liste neben jedem Objekttyp klicken. Kollisionen werden in der Spalte Kollision angezeigt.

>[!NOTE]
>
>Erkannte Kollisionen sind möglicherweise nicht die Objekte, die Sie überschreiben oder in Ihrer Installation verwenden möchten. Es wird empfohlen, erkannte Kollisionen zu validieren, um sicherzustellen, dass die Installationsziele korrekt sind.

Um eine Kollision zu beheben, wählen Sie eine Aktion in der Spalte „Bereitstellungsaktion“ aus oder verwenden Sie die bereits angezeigte Standardaktion.

* **Mit neuem Namen erstellen**: Erstellen eines neuen Objekts in der Zielumgebung. Wenn das Objekt in der Zielumgebung vorhanden ist, können Sie ein neues Objekt mit einem neuen Namen erstellen. Wenn es nicht in der Zielumgebung vorhanden ist, können Sie das Objekt mit einem neuen Namen oder mit dem Namen erstellen, den das Objekt im Paket hat.
* **Vorhandenes verwenden**: Das Objekt im Paket ist nicht installiert und das bereits in der Zielumgebung vorhandene Objekt ist unverändert.
* **Überschreiben**: Das Objekt im Paket ersetzt das vorhandene Objekt in der Zielumgebung.

  Sie können auch Objekte auswählen, die überschrieben werden sollen, selbst wenn keine Kollision erkannt wird.

  Weitere Informationen darüber, wie sich das Überschreiben auf übergeordnete und untergeordnete Objekte auswirkt, finden Sie unter [Überschreiben von übergeordneten und untergeordneten Objekten](#overwriting-parent-and-child-objects) in diesem Artikel.
<!--
* Do not use: The object in the package is not installed in the target environment. If you select Do not use, an error message will appear detailing how this choice will affect other objects or fields.
-->

Standardwerte werden `Create new`, wenn das Objekt nicht in der Zielumgebung vorhanden ist, und `Use existing`, wenn das Objekt in der Zielumgebung vorhanden ist. Sie können die Standardzuordnung wiederherstellen, indem Sie auf **Auf Standardzuordnung zurücksetzen** klicken.

## Überschreiben von übergeordneten und untergeordneten Objekten

Einige Objekte in Ihrem Promotion-Paket können untergeordnete Objekte haben. Beispielsweise hat ein Projekt (übergeordnetes Element) Aufgaben (untergeordnete Elemente). Beim Überschreiben eines übergeordneten -Objekts werden untergeordnete -Objekte wie folgt behandelt:

* Untergeordnete Objekte, die sowohl im Paket als auch im Ziel vorhanden sind, werden im Ziel aktualisiert, damit sie mit dem Paket übereinstimmen.
* Untergeordnete Objekte, die im Paket, aber nicht im Ziel vorhanden sind, werden erstellt.
* Untergeordnete Objekte, die im Ziel, aber nicht im Paket vorhanden sind, bleiben unverändert.

Diese Funktion wirkt sich auf die folgenden übergeordneten und untergeordneten Objekte aus:

| Übergeordnetes Objekt | Untergeordnete Objekte |
|---|---|
| Projekt | Task<br>QueueDef (Warteschlangendefinition)<br>RoutingRule |
| Vorlage | templateTask<br>QueueDef (Warteschlangendefinition)<br>RoutingRule |
| Parameter (benutzerdefiniertes Formularfeld) | ParameterOption (Option für benutzerdefiniertes Formularfeld) |
| CalendarInfo | Kalenderabschnitt |
| QueueDef (Warteschlangendefinition) | QueueTopicGroup<br>QueueTopic |

