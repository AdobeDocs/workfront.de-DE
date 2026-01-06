---
content-type: overview;reference
product-previous: workfront-goals
navigation-topic: goal-management
title: Übersicht über den Zielstatus in Adobe Workfront Goals
description: Der Zielstatus gibt an, ob ein Ziel aktiv ist und derzeit den Fortschritt erfasst oder ob es inaktiv, entworfen oder bereits erreicht ist.
author: Alina
feature: Workfront Goals
exl-id: dc70dfac-2bdd-41ab-b316-0cd20f749423
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '793'
ht-degree: 4%

---

# Übersicht über den Zielstatus in Adobe Workfront Goals

<!--Audited: 4/2025-->

>[!NOTE]
>
>Ihr Unternehmen könnte sich dafür entscheiden, weiterhin Adobe Workfront Goals zu verwenden, wenn es dieses Paket in der Vergangenheit gekauft hat. Weitere Informationen erhalten Sie von Ihrem Kundenbetreuer.
>
>Adobe Workfront Goals ist nicht mehr erhältlich.
>
>Weitere Informationen zum Zugriff auf Workfront-Ziele finden Sie unter [Voraussetzungen für die Verwendung von Workfront-Zielen](/help/quicksilver/workfront-goals/goal-management/access-needed-for-wf-goals.md).

<!--Old:

>[!IMPORTANT]
>
>Your organization must have the following to use the functionality described in this article:
>
>* For the new plan and license structure:
>
>   * The Ultimate Workfront plan 
>    
>* For the current plan and license structure: 
>
>   * A Pro or higher Workfront plan
>   * An Adobe Workfront Goals license in addition to a Workfront license.
>
>Contact your Workfront account manager to learn about a Workfront Goals license.    
> 
>For additional information about access to Workfront Goals, see [Requirements to use Workfront Goals](/help/quicksilver/workfront-goals/goal-management/access-needed-for-wf-goals.md).   -->

## Überlegungen zur Aktualisierung des Zielstatus in Workfront Goals

* Sie können den Status von Zielen, die Sie erstellt haben oder die für Sie freigegeben wurden, nicht manuell aktualisieren. Der Status der Ziele wird je nach den Aktionen, die Sie für das Ziel ausführen, aktualisiert. Wenn Sie beispielsweise ein Ziel aktivieren, ändert sich der Entwurfsstatus in „Aktiv“.
* Es gibt einige Einschränkungen, und manchmal kann der Status eines Ziels gemäß den folgenden Regeln nicht in einen anderen Status geändert werden:

  | Von/bis | Entwurf | Aktiv | Inaktiv | Geschlossen |
  |---|---|---|---|---|
  | Entwurf | – | Ja | Nein | Nein |
  | Aktiv | Nein | – | Ja | Ja |
  | Inaktiv | Nein | Ja | – | Nein |
  | Geschlossen | Nein | Ja | Nein | – |

* Das Öffnen eines geschlossenen Ziels aktualisiert auch den Fortschritt des Ziels.
* Bestimmte Aktionen, die Sie für ein Ziel ausführen, aktualisieren auch dessen Status. Informationen dazu, wie Sie den Zielstatus aktualisieren können, finden Sie in den folgenden Artikeln:

   * [Erstellen von Zielen in Adobe Workfront-Zielen](../../workfront-goals/goal-management/create-goals.md)
   * [Aktivieren von Zielen in Adobe Workfront-Zielen](../../workfront-goals/goal-management/activate-goals.md)
   * [Löschen und Deaktivieren von Zielen in Adobe Workfront-Zielen](../../workfront-goals/goal-management/delete-and-deactivate-goals.md)
   * [Schließen und erneutes Öffnen von Zielen in Adobe Workfront-Zielen](../../workfront-goals/goal-management/close-and-reopen-goals.md)

## Übersicht über die Zielstatus in Workfront Goals

Informationen zum Erstellen von Workfront-Zielen finden Sie unter [Erstellen von Zielen in Adobe Workfront-Zielen](../../workfront-goals/goal-management/create-goals.md).

Informationen zum Aktivieren von Zielen finden Sie unter [Aktivieren von Zielen in Adobe Workfront](../../workfront-goals/goal-management/activate-goals.md).

Ziele können einen der folgenden Status in Workfront Goals haben:

* [Entwurf](#draft)
* [aktiv](#active)
* [Inaktiv](#inactive)
* [Geschlossen](#closed)

### Entwurf {#draft}

* Dies ist der Standardstatus für ein neu erstelltes Ziel. Informationen zum Erstellen von Zielen finden Sie unter [Erstellen von Zielen in Adobe Workfront](../../workfront-goals/goal-management/create-goals.md).
* Workfront-Ziele zeichnen den Fortschritt bei einem Zielentwurf nicht auf.
* Sie können den Fortschritt eines Zielentwurfs nicht aktualisieren.
* Entworfene Ziele können nicht geschlossen oder deaktiviert werden, da sie keine Fortschrittsinformationen enthalten.
* Entworfene Ziele tragen nicht zur Fortschrittsberechnung anderer Ziele bei und werden in Diagrammen nicht berücksichtigt.
* Die entworfenen Ziele werden in den folgenden Bereichen der Workfront-Ziele angezeigt:

   * Liste der Ziele
   * Abschnitt „Zielausrichtung“ (nur als abgestimmtes Ziel)


>[!IMPORTANT]
>
>Nachdem Sie den Status eines Ziels in einen anderen Status geändert haben, kann das Ziel nie wieder in den Status Entwurf versetzt werden.

### Aktiv {#active}

* Ein Entwurfsziel kann nur aktiviert werden, wenn Sie es mit einem Ergebnis oder einer Aktivität verknüpfen oder ein anderes Ziel daran ausrichten. Beim Aktivieren des Ziels ändert sich sein Status in „Aktiv“. Informationen zum Aktivieren von Zielen finden Sie unter [Aktivieren von Zielen in Adobe Workfront](../../workfront-goals/goal-management/activate-goals.md).
* Workfront-Ziele zeichnen den Fortschritt bei aktiven Zielen auf.
* Aktive Ziele tragen zur Fortschrittsberechnung anderer Ziele bei und werden in Diagrammen berücksichtigt.
* Aktive Ziele werden in den folgenden Bereichen von Workfront-Zielen angezeigt:

   * Liste der Ziele
   * Abschnitt „Zielausrichtung“
   * Der Fortschritt aktiver Ziele wird in Diagrammen angezeigt

* Sie können ein geschlossenes oder inaktives Ziel reaktivieren.

### Inaktiv {#inactive}

* Sie können ein aktives Ziel deaktivieren, wenn der Besitzer die Arbeit daran vorübergehend oder dauerhaft beendet hat. Sie können ihn zur Verlaufskontrolle aufbewahren. Dadurch wird der Status des Ziels auf Inaktiv gesetzt.

  Informationen zur Deaktivierung von Zielen finden Sie im Abschnitt „Deaktivierung von Zielen“ im Artikel [Löschen und Deaktivieren von Zielen in Adobe Workfront-Zielen](../../workfront-goals/goal-management/delete-and-deactivate-goals.md).

* Ein entworfenes oder geschlossenes Ziel kann nicht deaktiviert werden.
* Sie können ein inaktives Ziel reaktivieren und weiter daran arbeiten.
* Workfront-Ziele berechnen den Fortschritt bei inaktiven Zielen nicht.
* Der Fortschritt eines inaktiven Ziels kann nicht aktualisiert werden.
* Inaktive Ziele tragen nicht zur Fortschrittsberechnung anderer Ziele bei und werden in Diagrammen nicht berücksichtigt.
* Inaktive Ziele haben einen Fortschrittsverlauf, da sie früher aktiv waren, im Gegensatz zu den entworfenen Zielen.
* Inaktive Ziele werden in den folgenden Bereichen von Workfront-Zielen angezeigt:

   * Liste der Ziele
   * Abschnitt „Zielausrichtung“ (nur als abgestimmte Ziele)

### Geschlossen {#closed}

* Sie können ein Ziel schließen, wenn Sie anzeigen möchten, dass Sie es erreicht haben oder nicht mehr daran arbeiten, oder dies in Zukunft tun werden. Informationen zum Schließen von Zielen finden Sie unter [Schließen und erneut öffnen von Zielen in Adobe Workfront-](../../workfront-goals/goal-management/close-and-reopen-goals.md).

  >[!TIP]
  >
  >Wenn Sie später an einem Ziel arbeiten möchten, das noch nicht erreicht wurde, empfehlen wir, den Status in „Inaktiv“ anstelle von „Geschlossen“ zu ändern.

* Ziele, die noch nie aktiviert wurden, wie z. B. entworfene Ziele, können nicht geschlossen werden.
* Sie können ein geschlossenes Ziel erneut öffnen und es weiter bearbeiten.
* Workfront-Ziele : Stoppt die Aufzeichnung des Fortschritts bei abgeschlossenen Zielen.
* Sie können den Fortschritt eines geschlossenen Ziels nicht aktualisieren.
* Geschlossene Ziele werden im folgenden Bereich von Workfront-Ziele angezeigt:

   * Liste der Ziele
   * Abschnitt „Zielausrichtung“ (nur als abgestimmte Ziele)
   * Informationen aus abgeschlossenen Zielen werden auch im Abschnitt Diagramme berücksichtigt.
